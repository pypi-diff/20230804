# Comparing `tmp/calitp_map_utils-2023.8.1.tar.gz` & `tmp/calitp_map_utils-2023.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calitp_map_utils-2023.8.1.tar", max compression
+gzip compressed data, was "calitp_map_utils-2023.8.2.tar", max compression
```

## Comparing `calitp_map_utils-2023.8.1.tar` & `calitp_map_utils-2023.8.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3674 2023-07-24 19:16:34.269930 calitp_map_utils-2023.8.1/README.md
--rw-r--r--   0        0        0     5113 2023-07-31 15:40:25.453826 calitp_map_utils-2023.8.1/calitp_map_utils/__init__.py
--rw-r--r--   0        0        0       44 2023-06-26 17:16:54.925708 calitp_map_utils-2023.8.1/calitp_map_utils/__main__.py
--rw-r--r--   0        0        0     1441 2023-06-26 17:16:54.926512 calitp_map_utils-2023.8.1/calitp_map_utils/cli.py
--rw-r--r--   0        0        0      637 2023-08-01 21:43:12.769889 calitp_map_utils-2023.8.1/pyproject.toml
--rw-r--r--   0        0        0     4296 1970-01-01 00:00:00.000000 calitp_map_utils-2023.8.1/PKG-INFO
+-rw-r--r--   0        0        0     3674 2023-08-04 18:45:45.347002 calitp_map_utils-2023.8.2/README.md
+-rw-r--r--   0        0        0     5454 2023-08-04 18:45:45.347002 calitp_map_utils-2023.8.2/calitp_map_utils/__init__.py
+-rw-r--r--   0        0        0       44 2023-08-04 18:45:45.347002 calitp_map_utils-2023.8.2/calitp_map_utils/__main__.py
+-rw-r--r--   0        0        0     1441 2023-08-04 18:45:45.347002 calitp_map_utils-2023.8.2/calitp_map_utils/cli.py
+-rw-r--r--   0        0        0      637 2023-08-04 18:45:45.347002 calitp_map_utils-2023.8.2/pyproject.toml
+-rw-r--r--   0        0        0     4296 1970-01-01 00:00:00.000000 calitp_map_utils-2023.8.2/PKG-INFO
```

### Comparing `calitp_map_utils-2023.8.1/README.md` & `calitp_map_utils-2023.8.2/README.md`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.8.1/calitp_map_utils/__init__.py` & `calitp_map_utils-2023.8.2/calitp_map_utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import base64
 import gzip
 import json
 import os
 from enum import Enum
-from typing import Any, Dict, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Union
 
-import gcsfs
+import gcsfs  # type: ignore[import]
 import requests
 import typer
-from furl import furl
+from furl import furl  # type: ignore[import]
 from geojson_pydantic import Feature, FeatureCollection, MultiPolygon, Point, Polygon
 from geojson_pydantic.geometries import Geometry
 from geojson_pydantic.types import Position
 from pydantic import BaseModel, Field, HttpUrl, ValidationError, conlist, root_validator
 from tqdm import tqdm
 
 MAP_APP_URL_ENV_VAR = "CALITP_MAP_APP_URL"
@@ -28,24 +28,31 @@
 
 
 class Tooltip(BaseModel):
     html: str
     style: Optional[Dict[str, Any]]
 
 
+# https://github.com/pydantic/pydantic/discussions/5528#discussioncomment-5663312
+if TYPE_CHECKING:
+    Color = Optional[list[int]]
+else:
+    # we add alpha in the JS if only 3 colors are passed
+    Color = Optional[conlist(int, min_items=3, max_items=4)]
+
+
 class Speedmap(BaseModel):
     stop_id: Optional[str]
     stop_name: Optional[str]
     route_id: Optional[str]
     tooltip: Optional[Tooltip]
     avg_mph: Optional[float]
     p20_mph: Optional[float] = Field(alias="_20p_mph")
-    # we add alpha in the JS if only 3 colors are passed
-    color: Optional[conlist(int, min_items=3, max_items=4)]
-    highlight_color: Optional[conlist(int, min_items=3, max_items=4)]
+    color: Color
+    highlight_color: Color
 
     @root_validator
     def some_identifier_exists(cls, values):
         assert any(key in values for key in ["stop_id", "stop_name", "route_id"])
         return values
 
 
@@ -85,15 +92,18 @@
         with openf(path, "rb" if is_compressed else "r") as f:
             if is_compressed:
                 f = gzip.GzipFile(fileobj=f)
             d = json.load(f)
 
     collection = FeatureCollection(**d)
 
-    layer_type_class = LAYER_FEATURE_TYPES.get(layer_type, Feature[Geometry, Dict])
+    if layer_type:
+        layer_type_class = LAYER_FEATURE_TYPES.get(layer_type, Feature[Geometry, Dict])
+    else:
+        layer_type_class = Feature[Geometry, Dict]
 
     if verbose:
         typer.secho(
             f"Validating that features are {typer.style(str(layer_type_class), fg=typer.colors.YELLOW)}..."
         )
     for feature in tqdm(collection.features):
         try:
@@ -113,21 +123,26 @@
 
 
 class BasemapConfig(BaseModel):
     url: str
     options: Dict[str, Any]
 
 
+if TYPE_CHECKING:
+    LayerList = list[Layer]
+else:
+    # this will not render in erdantic; needs to be List[Layer] but then pydantic2ts will not set min_items
+    LayerList = conlist(Layer, min_items=1)
+
+
 # Any positions in this are flipped from typical geojson
 # leaflet wants lat/lon
 class State(BaseModel):
     name: Optional[str]
-    layers: conlist(
-        Layer, min_items=1
-    )  # this will not render in erdantic; needs to be List[Layer] but then pydantic2ts will not set min_items
+    layers: LayerList
     lat_lon: Optional[Position]
     zoom: Optional[int]
     bbox: Optional[Tuple[Position, Position]]
     basemap_config: Optional[BasemapConfig]
     legend_url: Optional[HttpUrl]
 
     def validate_layers(
@@ -147,15 +162,15 @@
             except requests.exceptions.HTTPError:
                 typer.secho(f"Failed to find file at {layer.url}", fg=typer.colors.RED)
                 raise
 
             if data:
                 validate_geojson(layer.url, layer.typ, verbose=verbose)
 
-    def iframe_url(self, host: str = None) -> str:
+    def iframe_url(self, host: Optional[str] = None) -> str:
         host = host or MAP_APP_URL
         if not host:
             raise RuntimeError(
                 "Must provide host parameter or MAP_APP_URL environment variable."
             )
 
         return (
```

### Comparing `calitp_map_utils-2023.8.1/calitp_map_utils/cli.py` & `calitp_map_utils-2023.8.2/calitp_map_utils/cli.py`

 * *Files identical despite different names*

### Comparing `calitp_map_utils-2023.8.1/pyproject.toml` & `calitp_map_utils-2023.8.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "calitp_map_utils"
-version = "2023.8.1"
+version = "2023.8.2"
 description = ""
 authors = ["Andrew Vaccaro <andrew.v@jarv.us>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "~3.9"
 pyyaml = "^6.0"
```

### Comparing `calitp_map_utils-2023.8.1/PKG-INFO` & `calitp_map_utils-2023.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: calitp-map-utils
-Version: 2023.8.1
+Version: 2023.8.2
 Summary: 
 Author: Andrew Vaccaro
 Author-email: andrew.v@jarv.us
 Requires-Python: >=3.9,<3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: furl (>=2.1.3,<3.0.0)
```

