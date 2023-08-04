# Comparing `tmp/hyko_sdk-0.3.0b2.tar.gz` & `tmp/hyko_sdk-0.3.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyko_sdk-0.3.0b2.tar", last modified: Mon Jul 31 09:45:49 2023, max compression
+gzip compressed data, was "hyko_sdk-0.3.0b3.tar", last modified: Fri Aug  4 18:48:54 2023, max compression
```

## Comparing `hyko_sdk-0.3.0b2.tar` & `hyko_sdk-0.3.0b3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-07-31 09:45:49.738474 hyko_sdk-0.3.0b2/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-07-31 09:45:49.741807 hyko_sdk-0.3.0b2/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      411 2023-05-19 16:11:29.000000 hyko_sdk-0.3.0b2/README.md
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-07-31 09:45:49.738474 hyko_sdk-0.3.0b2/hyko_sdk/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       60 2023-06-26 13:00:23.000000 hyko_sdk-0.3.0b2/hyko_sdk/__init__.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      682 2023-07-04 08:21:39.000000 hyko_sdk-0.3.0b2/hyko_sdk/error.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)    14691 2023-07-31 09:38:24.000000 hyko_sdk-0.3.0b2/hyko_sdk/io.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1402 2023-07-30 15:01:20.000000 hyko_sdk-0.3.0b2/hyko_sdk/metadata.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2263 2023-07-18 08:50:54.000000 hyko_sdk-0.3.0b2/hyko_sdk/utils.py
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-07-31 09:45:49.738474 hyko_sdk-0.3.0b2/hyko_sdk.egg-info/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-07-31 09:45:49.000000 hyko_sdk-0.3.0b2/hyko_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      286 2023-07-31 09:45:49.000000 hyko_sdk-0.3.0b2/hyko_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-07-31 09:45:49.000000 hyko_sdk-0.3.0b2/hyko_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       54 2023-07-31 09:45:49.000000 hyko_sdk-0.3.0b2/hyko_sdk.egg-info/requires.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-07-31 09:45:49.000000 hyko_sdk-0.3.0b2/hyko_sdk.egg-info/top_level.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.3.0b2/pyproject.toml
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      381 2023-07-31 09:45:49.741807 hyko_sdk-0.3.0b2/setup.cfg
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 18:48:54.845292 hyko_sdk-0.3.0b3/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 18:48:54.845292 hyko_sdk-0.3.0b3/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      411 2023-05-19 16:11:29.000000 hyko_sdk-0.3.0b3/README.md
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 18:48:54.845292 hyko_sdk-0.3.0b3/hyko_sdk/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       60 2023-06-26 13:00:23.000000 hyko_sdk-0.3.0b3/hyko_sdk/__init__.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      682 2023-07-04 08:21:39.000000 hyko_sdk-0.3.0b3/hyko_sdk/error.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)    14655 2023-08-04 18:46:43.000000 hyko_sdk-0.3.0b3/hyko_sdk/io.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1425 2023-08-04 18:44:43.000000 hyko_sdk-0.3.0b3/hyko_sdk/metadata.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2263 2023-07-18 08:50:54.000000 hyko_sdk-0.3.0b3/hyko_sdk/utils.py
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 18:48:54.845292 hyko_sdk-0.3.0b3/hyko_sdk.egg-info/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 18:48:54.000000 hyko_sdk-0.3.0b3/hyko_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      286 2023-08-04 18:48:54.000000 hyko_sdk-0.3.0b3/hyko_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-08-04 18:48:54.000000 hyko_sdk-0.3.0b3/hyko_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       54 2023-08-04 18:48:54.000000 hyko_sdk-0.3.0b3/hyko_sdk.egg-info/requires.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-08-04 18:48:54.000000 hyko_sdk-0.3.0b3/hyko_sdk.egg-info/top_level.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.3.0b3/pyproject.toml
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      381 2023-08-04 18:48:54.845292 hyko_sdk-0.3.0b3/setup.cfg
```

### Comparing `hyko_sdk-0.3.0b2/hyko_sdk/error.py` & `hyko_sdk-0.3.0b3/hyko_sdk/error.py`

 * *Files identical despite different names*

### Comparing `hyko_sdk-0.3.0b2/hyko_sdk/io.py` & `hyko_sdk-0.3.0b3/hyko_sdk/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 from typing import Any, Union, Optional, Tuple
 
 from typing import Any, Type
 
 from pydantic_core import core_schema
-from pydantic import BaseModel as PBaseModel, GetCoreSchemaHandler, GetJsonSchemaHandler
+from pydantic import BaseModel, GetCoreSchemaHandler, GetJsonSchemaHandler
 import numpy as np
 from PIL import Image as PIL_Image
 import soundfile
 import os
 import subprocess
 import io
 
@@ -418,14 +418,10 @@
         cls,
         _core_schema: core_schema.CoreSchema,
         handler: GetJsonSchemaHandler
     ):
         schema = handler(_core_schema)
         schema["subtype"] = "video"
         return schema
-        
-        
-
     
-class BaseModel(PBaseModel):
-    pass
-
+class CoreModel(BaseModel):
+    pass
```

### Comparing `hyko_sdk-0.3.0b2/hyko_sdk/metadata.py` & `hyko_sdk-0.3.0b3/hyko_sdk/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,11 +42,14 @@
 class MetaData(MetaDataBase):
     version: str
     name: str
     category: str
 
 
 def metadata_to_docker_label(metadata: MetaData) -> str:
-    return metadata.model_dump_json(exclude_unset=True).replace('"', "'")
+    return metadata.model_dump_json(exclude_unset=True, exclude_none=True).replace('"', "'")
+
     
 def docker_label_to_metadata(label: str) -> MetaData:
-    return MetaData(**json.loads(label.replace("'", '"')))
+    return MetaData(**json.loads(label.replace("'", '"')))
+
+
```

### Comparing `hyko_sdk-0.3.0b2/hyko_sdk/utils.py` & `hyko_sdk-0.3.0b3/hyko_sdk/utils.py`

 * *Files identical despite different names*

