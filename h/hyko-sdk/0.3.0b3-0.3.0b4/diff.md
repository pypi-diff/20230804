# Comparing `tmp/hyko_sdk-0.3.0b3.tar.gz` & `tmp/hyko_sdk-0.3.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyko_sdk-0.3.0b3.tar", last modified: Fri Aug  4 18:48:54 2023, max compression
+gzip compressed data, was "hyko_sdk-0.3.0b4.tar", last modified: Fri Aug  4 19:48:33 2023, max compression
```

## Comparing `hyko_sdk-0.3.0b3.tar` & `hyko_sdk-0.3.0b4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 18:48:54.845292 hyko_sdk-0.3.0b3/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 18:48:54.845292 hyko_sdk-0.3.0b3/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      411 2023-05-19 16:11:29.000000 hyko_sdk-0.3.0b3/README.md
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 18:48:54.845292 hyko_sdk-0.3.0b3/hyko_sdk/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       60 2023-06-26 13:00:23.000000 hyko_sdk-0.3.0b3/hyko_sdk/__init__.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      682 2023-07-04 08:21:39.000000 hyko_sdk-0.3.0b3/hyko_sdk/error.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)    14655 2023-08-04 18:46:43.000000 hyko_sdk-0.3.0b3/hyko_sdk/io.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1425 2023-08-04 18:44:43.000000 hyko_sdk-0.3.0b3/hyko_sdk/metadata.py
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2263 2023-07-18 08:50:54.000000 hyko_sdk-0.3.0b3/hyko_sdk/utils.py
-drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 18:48:54.845292 hyko_sdk-0.3.0b3/hyko_sdk.egg-info/
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 18:48:54.000000 hyko_sdk-0.3.0b3/hyko_sdk.egg-info/PKG-INFO
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      286 2023-08-04 18:48:54.000000 hyko_sdk-0.3.0b3/hyko_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-08-04 18:48:54.000000 hyko_sdk-0.3.0b3/hyko_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       54 2023-08-04 18:48:54.000000 hyko_sdk-0.3.0b3/hyko_sdk.egg-info/requires.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-08-04 18:48:54.000000 hyko_sdk-0.3.0b3/hyko_sdk.egg-info/top_level.txt
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.3.0b3/pyproject.toml
--rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      381 2023-08-04 18:48:54.845292 hyko_sdk-0.3.0b3/setup.cfg
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 19:48:33.944241 hyko_sdk-0.3.0b4/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 19:48:33.944241 hyko_sdk-0.3.0b4/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       16 2023-08-04 19:47:01.000000 hyko_sdk-0.3.0b4/README.md
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 19:48:33.944241 hyko_sdk-0.3.0b4/hyko_sdk/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       60 2023-06-26 13:00:23.000000 hyko_sdk-0.3.0b4/hyko_sdk/__init__.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      682 2023-07-04 08:21:39.000000 hyko_sdk-0.3.0b4/hyko_sdk/error.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)    14646 2023-08-04 19:43:32.000000 hyko_sdk-0.3.0b4/hyko_sdk/io.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     1377 2023-08-04 19:41:51.000000 hyko_sdk-0.3.0b4/hyko_sdk/metadata.py
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)     2263 2023-07-18 08:50:54.000000 hyko_sdk-0.3.0b4/hyko_sdk/utils.py
+drwxr-xr-x   0 dahmadjid  (1000) dahmadjid  (1000)        0 2023-08-04 19:48:33.944241 hyko_sdk-0.3.0b4/hyko_sdk.egg-info/
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      194 2023-08-04 19:48:33.000000 hyko_sdk-0.3.0b4/hyko_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      286 2023-08-04 19:48:33.000000 hyko_sdk-0.3.0b4/hyko_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        1 2023-08-04 19:48:33.000000 hyko_sdk-0.3.0b4/hyko_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      116 2023-08-04 19:48:33.000000 hyko_sdk-0.3.0b4/hyko_sdk.egg-info/requires.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)        9 2023-08-04 19:48:33.000000 hyko_sdk-0.3.0b4/hyko_sdk.egg-info/top_level.txt
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)       80 2023-06-21 08:15:38.000000 hyko_sdk-0.3.0b4/pyproject.toml
+-rw-r--r--   0 dahmadjid  (1000) dahmadjid  (1000)      443 2023-08-04 19:48:33.944241 hyko_sdk-0.3.0b4/setup.cfg
```

### Comparing `hyko_sdk-0.3.0b3/hyko_sdk/error.py` & `hyko_sdk-0.3.0b4/hyko_sdk/error.py`

 * *Files identical despite different names*

### Comparing `hyko_sdk-0.3.0b3/hyko_sdk/io.py` & `hyko_sdk-0.3.0b4/hyko_sdk/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
     @classmethod
     def __get_pydantic_json_schema__(
         cls,
         _core_schema: core_schema.CoreSchema,
         handler: GetJsonSchemaHandler
     ):
         schema = handler(_core_schema)
-        schema["subtype"] = "image"
+        schema["type"] = "image"
         return schema
         
         
 
 class Audio(HykoBaseType):
 
     @staticmethod
@@ -257,15 +257,15 @@
     @classmethod
     def __get_pydantic_json_schema__(
         cls,
         _core_schema: core_schema.CoreSchema,
         handler: GetJsonSchemaHandler
     ):
         schema = handler(_core_schema)
-        schema["subtype"] = "audio"
+        schema["type"] = "audio"
         return schema
         
         
     _SUBTYPE2DTYPE = {
         "PCM_S8": "int8",
         "PCM_U8": "uint8",
         "PCM_16": "int16",
@@ -416,12 +416,12 @@
     @classmethod
     def __get_pydantic_json_schema__(
         cls,
         _core_schema: core_schema.CoreSchema,
         handler: GetJsonSchemaHandler
     ):
         schema = handler(_core_schema)
-        schema["subtype"] = "video"
+        schema["type"] = "video"
         return schema
     
 class CoreModel(BaseModel):
     pass
```

### Comparing `hyko_sdk-0.3.0b3/hyko_sdk/metadata.py` & `hyko_sdk-0.3.0b4/hyko_sdk/metadata.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 
 class HykoExtraTypes(str, Enum):
     IMAGE = "image"
     AUDIO = "audio"
     VIDEO = "video"
     
 class Property(BaseModel):
-    type: Optional[IOPortType] = None
-    subtype: Optional[HykoExtraTypes] = None
+    type: IOPortType | HykoExtraTypes
     anyOf: Optional [List['Property']] = None
     items: Optional[Union['Property', List['Property']]] = None
     prefixItems: Optional[List['Property']] = None
     minItems: Optional[int] = None
     maxItems: Optional[int] = None
     description: Optional[str] = None
     default: Optional[Any] = None
@@ -46,10 +45,8 @@
 
 
 def metadata_to_docker_label(metadata: MetaData) -> str:
     return metadata.model_dump_json(exclude_unset=True, exclude_none=True).replace('"', "'")
 
     
 def docker_label_to_metadata(label: str) -> MetaData:
-    return MetaData(**json.loads(label.replace("'", '"')))
-
-
+    return MetaData(**json.loads(label.replace("'", '"')))
```

### Comparing `hyko_sdk-0.3.0b3/hyko_sdk/utils.py` & `hyko_sdk-0.3.0b4/hyko_sdk/utils.py`

 * *Files identical despite different names*

