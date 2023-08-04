# Comparing `tmp/heatfall-0.0.2.tar.gz` & `tmp/heatfall-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heatfall-0.0.2.tar", last modified: Tue Aug  1 18:42:27 2023, max compression
+gzip compressed data, was "heatfall-0.1.0.tar", last modified: Fri Aug  4 17:16:30 2023, max compression
```

## Comparing `heatfall-0.0.2.tar` & `heatfall-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 18:42:27.889318 heatfall-0.0.2/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-08-01 14:52:25.000000 heatfall-0.0.2/LICENSE
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2072 2023-08-01 18:42:27.889459 heatfall-0.0.2/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)     1440 2023-08-01 18:41:12.000000 heatfall-0.0.2/README.md
--rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-08-01 14:52:21.000000 heatfall-0.0.2/pyproject.toml
--rw-r--r--   0 odosmatthews   (501) staff       (20)      968 2023-08-01 18:42:27.890544 heatfall-0.0.2/setup.cfg
--rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-08-01 14:43:18.000000 heatfall-0.0.2/setup.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 18:42:27.879739 heatfall-0.0.2/src/
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 18:42:27.882591 heatfall-0.0.2/src/heatfall/
--rw-r--r--   0 odosmatthews   (501) staff       (20)       66 2023-08-01 18:38:37.000000 heatfall-0.0.2/src/heatfall/__init__.py
--rw-r--r--   0 odosmatthews   (501) staff       (20)     5964 2023-07-21 17:24:03.000000 heatfall-0.0.2/src/heatfall/heat.py
-drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-01 18:42:27.889093 heatfall-0.0.2/src/heatfall.egg-info/
--rw-r--r--   0 odosmatthews   (501) staff       (20)     2072 2023-08-01 18:42:27.000000 heatfall-0.0.2/src/heatfall.egg-info/PKG-INFO
--rw-r--r--   0 odosmatthews   (501) staff       (20)      311 2023-08-01 18:42:27.000000 heatfall-0.0.2/src/heatfall.egg-info/SOURCES.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-08-01 18:42:27.000000 heatfall-0.0.2/src/heatfall.egg-info/dependency_links.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-08-01 16:54:12.000000 heatfall-0.0.2/src/heatfall.egg-info/not-zip-safe
--rw-r--r--   0 odosmatthews   (501) staff       (20)      152 2023-08-01 18:42:27.000000 heatfall-0.0.2/src/heatfall.egg-info/requires.txt
--rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-08-01 18:42:27.000000 heatfall-0.0.2/src/heatfall.egg-info/top_level.txt
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-04 17:16:30.503157 heatfall-0.1.0/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1068 2023-08-01 14:52:25.000000 heatfall-0.1.0/LICENSE
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     2072 2023-08-04 17:16:30.503390 heatfall-0.1.0/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     1440 2023-08-01 18:41:12.000000 heatfall-0.1.0/README.md
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      499 2023-08-01 14:52:21.000000 heatfall-0.1.0/pyproject.toml
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      972 2023-08-04 17:16:30.506424 heatfall-0.1.0/setup.cfg
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       68 2023-08-01 14:43:18.000000 heatfall-0.1.0/setup.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-04 17:16:30.493505 heatfall-0.1.0/src/
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-04 17:16:30.497453 heatfall-0.1.0/src/heatfall/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)       81 2023-08-04 14:40:19.000000 heatfall-0.1.0/src/heatfall/__init__.py
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     7229 2023-08-04 17:15:30.000000 heatfall-0.1.0/src/heatfall/heat.py
+drwxr-xr-x   0 odosmatthews   (501) staff       (20)        0 2023-08-04 17:16:30.502925 heatfall-0.1.0/src/heatfall.egg-info/
+-rw-r--r--   0 odosmatthews   (501) staff       (20)     2072 2023-08-04 17:16:30.000000 heatfall-0.1.0/src/heatfall.egg-info/PKG-INFO
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      311 2023-08-04 17:16:30.000000 heatfall-0.1.0/src/heatfall.egg-info/SOURCES.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-08-04 17:16:30.000000 heatfall-0.1.0/src/heatfall.egg-info/dependency_links.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        1 2023-08-01 16:54:12.000000 heatfall-0.1.0/src/heatfall.egg-info/not-zip-safe
+-rw-r--r--   0 odosmatthews   (501) staff       (20)      155 2023-08-04 17:16:30.000000 heatfall-0.1.0/src/heatfall.egg-info/requires.txt
+-rw-r--r--   0 odosmatthews   (501) staff       (20)        9 2023-08-04 17:16:30.000000 heatfall-0.1.0/src/heatfall.egg-info/top_level.txt
```

### Comparing `heatfall-0.0.2/LICENSE` & `heatfall-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heatfall-0.0.2/PKG-INFO` & `heatfall-0.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatfall
-Version: 0.0.2
+Version: 0.1.0
 Summary: Easy to use functions to plot heat maps of geospatial data using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `heatfall-0.0.2/README.md` & `heatfall-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `heatfall-0.0.2/setup.cfg` & `heatfall-0.1.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = heatfall
-version = 0.0.2
+version = 0.1.0
 description = Easy to use functions to plot heat maps of geospatial data using staticmaps.
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 author = Odos Matthews
 license = MIT
 license_file = LICENSE
 platforms = unix, linux, osx, cygwin, win32
@@ -21,14 +21,15 @@
 install_requires = 
 	range_key_dict
 	geodude
 	py-staticmaps
 	Pillow<=9.5.0
 	more_itertools
 	tinytim
+	h3
 python_requires = >=3.8
 package_dir = 
 	=src
 zip_safe = no
 
 [options.extras_require]
 testing =
```

### Comparing `heatfall-0.0.2/src/heatfall/heat.py` & `heatfall-0.1.0/src/heatfall/heat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """
 Functions for plotting heatmaps of points.
 """
 
-from typing import Optional
+from typing import List, Optional
 
 import staticmaps
 import pygeodesy
 from range_key_dict import RangeKeyDict
 from geodude import calculate_geohashes
 from tinytim.columns import value_counts
 from more_itertools import numeric_range
+import h3
 
 
 tp = staticmaps.tile_provider_OSM
 TRED = staticmaps.Color(255, 0, 0, 100)
 RED = staticmaps.RED
 TYELLOW = staticmaps.Color(255, 255, 0, 100)
 YELLOW = staticmaps.YELLOW
@@ -32,14 +33,28 @@
         color
     ) -> None:
         self.add_object(staticmaps.Area(
             make_hash_poly_points(h),
             fill_color=fill_color,
             width=width,
             color=color))
+        
+    def add_h3_poly(
+        self,
+        h,
+        fill_color,
+        width,
+        color
+    ) -> None:
+        self.add_object(staticmaps.Area(
+            make_h3_poly_points(h),
+            fill_color=fill_color,
+            width=width,
+            color=color
+        ))
 
     def add_neighbor_hash_polys(
         self,
         h, 
         fill_color,
         width,
         color
@@ -61,36 +76,58 @@
         colors=None
     ) -> None:
         for lat, lon, id, day in zip(cluster.lats, cluster.lons, cluster.ids, cluster.days):
             if colors is not None:
                 color = colors[id]
             point = staticmaps.create_latlng(lat, lon)
             self.add_object(staticmaps.Marker(point, color=color, size=size))
+
     def add_heat_hashes(self, lats, lons, precision):
         hashes = calculate_geohashes(lats, lons, precision)
         counts = dict(value_counts(hashes))
         colors = density_colors(list(counts.values()))
         for h, count in counts.items():
             c = colors[count]
             self.add_hash_poly(h, c, 1, staticmaps.TRANSPARENT)
 
+    def add_heat_h3s(self, lats, lons, precision: int) -> None:
+        hashes = calculate_h3_hashes(lats, lons, precision)
+        counts = dict(value_counts(hashes))
+        colors = density_colors(list(counts.values()))
+        for h, count in counts.items():
+            c = colors[count]
+            self.add_h3_poly(h, c, 1, staticmaps.TRANSPARENT)
+
 
 def plot_heat_hashes(
     lats,
     lons,
     percision,
     tileprovider=tp,
     size=(800, 500)
 ):
     context = Context()
     context.set_tile_provider(tileprovider)
     context.add_heat_hashes(lats, lons, percision)
     return context.render_pillow(*size)
 
 
+def plot_heat_h3s(
+    lats,
+    lons,
+    precision,
+    tileprovider=tp,
+    size=(800, 500)
+):
+    context = Context()
+    context.set_tile_provider(tileprovider)
+    context.add_heat_h3s(lats, lons, precision)
+    return context.render_pillow(*size)
+
+
 def density_colors(counts: list, transparency=150):
    RED = staticmaps.Color(255, 0, 0, transparency)
    ORANGE = staticmaps.Color(255, 128, 0, transparency)
    YELLOW = staticmaps.Color(255, 255, 0, transparency)
    GREEN = staticmaps.Color(0, 255, 0, transparency)
    BLUE = staticmaps.Color(0, 0, 255, transparency)
    colors = [BLUE, GREEN, YELLOW, ORANGE, RED]
@@ -138,24 +175,29 @@
     context = Context()
     context.set_tile_provider(tileprovider)
     lats, lons = super_cluster.lats, super_cluster.lons
     context.add_heat_hashes(lats, lons, p)
     return context.render_pillow(*size)
 
 
-def make_hash_poly_points(h):
+def make_hash_poly_points(h) -> List:
     b = pygeodesy.geohash.bounds(h)
     sw = b.latS, b.lonW
     nw = b.latN, b.lonW
     ne = b.latN, b.lonE
     se = b.latS, b.lonE
     polygon = [sw, nw, ne, se, sw]
     return [staticmaps.create_latlng(lat, lon) for lat, lon in polygon]
 
 
+def make_h3_poly_points(h: str) -> List:
+    points = list(h3.h3_to_geo_boundary(h, geo_json=True))
+    return [staticmaps.create_latlng(lat, lon) for lon, lat in points]
+
+
 def plot_hash(h, tileprovider=tp, size=(800, 500)):
     context = Context()
     context.set_tile_provider(tileprovider)
     context.add_hash_poly(h,
                           fill_color=staticmaps.parse_color('#00FF003F'),
                           width=2,
                           color=staticmaps.BLUE)
@@ -180,8 +222,12 @@
                           fill_color=staticmaps.parse_color('#00FF010F'),
                           width=5,
                           color=staticmaps.BLUE)
     context.add_neighbor_hash_polys(h,
                                     fill_color=staticmaps.parse_color('#00FF003F'),
                                     width=2,
                                     color=staticmaps.BLUE)
-    return context.render_pillow(*size)
+    return context.render_pillow(*size)
+
+
+def calculate_h3_hashes(latitudes, longitudes, precision) -> List[str]:
+    return [h3.geo_to_h3(lat, lon, precision) for lat, lon in zip(latitudes, longitudes)]
```

### Comparing `heatfall-0.0.2/src/heatfall.egg-info/PKG-INFO` & `heatfall-0.1.0/src/heatfall.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heatfall
-Version: 0.0.2
+Version: 0.1.0
 Summary: Easy to use functions to plot heat maps of geospatial data using staticmaps.
 Author: Odos Matthews
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

