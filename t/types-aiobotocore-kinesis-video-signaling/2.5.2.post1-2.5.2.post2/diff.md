# Comparing `tmp/types-aiobotocore-kinesis-video-signaling-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-kinesis-video-signaling-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesis-video-signaling-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesis-video-signaling-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
```

## Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1.tar` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.337549 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-08-02 14:52:31.337549 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:31.337549 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.337549 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8000 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.337549 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13053 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.166643 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13121 2023-08-04 13:59:14.166643 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11533 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.166643 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2182 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.166643 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      600 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      599 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1019 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6389 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6378 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8097 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8095 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2513 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2510 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:03.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.166643 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13121 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1006 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       42 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/LICENSE` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/PKG-INFO` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-signaling
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.KinesisVideoSignalingChannels 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KinesisVideoSignalingChannels 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-kinesis-video-signaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,44 +266,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesis_video_signaling.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideoSignalingChannels` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/literals/).
+
 ```python
-from types_aiobotocore_kinesis_video_signaling.literals import (
-    ServiceType,
-    KinesisVideoSignalingChannelsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_kinesis_video_signaling.literals import ServiceType
 
 
 def check_value(value: ServiceType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kinesis_video_signaling.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `KinesisVideoSignalingChannels` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/type_defs/).
+
 ```python
 from types_aiobotocore_kinesis_video_signaling.type_defs import (
     GetIceServerConfigRequestRequestTypeDef,
-    IceServerTypeDef,
-    ResponseMetadataTypeDef,
-    SendAlexaOfferToMasterRequestRequestTypeDef,
-    GetIceServerConfigResponseTypeDef,
-    SendAlexaOfferToMasterResponseTypeDef,
 )
 
 
 def get_value() -> GetIceServerConfigRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/README.md` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-kinesis-video-signaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,44 +234,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesis_video_signaling.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideoSignalingChannels` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/literals/).
+
 ```python
-from types_aiobotocore_kinesis_video_signaling.literals import (
-    ServiceType,
-    KinesisVideoSignalingChannelsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_kinesis_video_signaling.literals import ServiceType
 
 
 def check_value(value: ServiceType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kinesis_video_signaling.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `KinesisVideoSignalingChannels` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/type_defs/).
+
 ```python
 from types_aiobotocore_kinesis_video_signaling.type_defs import (
     GetIceServerConfigRequestRequestTypeDef,
-    IceServerTypeDef,
-    ResponseMetadataTypeDef,
-    SendAlexaOfferToMasterRequestRequestTypeDef,
-    GetIceServerConfigResponseTypeDef,
-    SendAlexaOfferToMasterResponseTypeDef,
 )
 
 
 def get_value() -> GetIceServerConfigRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/setup.py` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesis-video-signaling",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_kinesis_video_signaling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KinesisVideoSignalingChannels 2.5.2 service generated"
-        " with mypy-boto3-builder 7.17.1"
+        " with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/__init__.py` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/__init__.pyi` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/__main__.py` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.KinesisVideoSignalingChannels 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-signaling.html#KinesisVideoSignalingChannels\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post1")
+    print("2.5.2.post2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/client.py` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/client.pyi` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/literals.py` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -144,14 +145,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -230,26 +232,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/literals.pyi` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "amplifybackend",
     "amplifyuibuilder",
     "apigateway",
     "apigatewaymanagementapi",
     "apigatewayv2",
     "appconfig",
     "appconfigdata",
+    "appfabric",
     "appflow",
     "appintegrations",
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
@@ -142,14 +143,15 @@
     "elasticbeanstalk",
     "elastictranscoder",
     "elb",
     "elbv2",
     "emr",
     "emr-containers",
     "emr-serverless",
+    "entityresolution",
     "es",
     "events",
     "evidently",
     "finspace",
     "finspace-data",
     "firehose",
     "fis",
@@ -228,26 +230,28 @@
     "lookoutmetrics",
     "lookoutvision",
     "m2",
     "machinelearning",
     "macie",
     "macie2",
     "managedblockchain",
+    "managedblockchain-query",
     "marketplace-catalog",
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
     "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
+    "medical-imaging",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
     "migration-hub-refactor-spaces",
     "migrationhub-config",
     "migrationhuborchestrator",
```

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/type_defs.py` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling/type_defs.pyi` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling.egg-info/PKG-INFO` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-signaling
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.KinesisVideoSignalingChannels 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KinesisVideoSignalingChannels 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-kinesis-video-signaling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,44 +266,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesis_video_signaling.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideoSignalingChannels` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/literals/).
+
 ```python
-from types_aiobotocore_kinesis_video_signaling.literals import (
-    ServiceType,
-    KinesisVideoSignalingChannelsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_kinesis_video_signaling.literals import ServiceType
 
 
 def check_value(value: ServiceType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kinesis_video_signaling.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `KinesisVideoSignalingChannels` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_signaling/type_defs/).
+
 ```python
 from types_aiobotocore_kinesis_video_signaling.type_defs import (
     GetIceServerConfigRequestRequestTypeDef,
-    IceServerTypeDef,
-    ResponseMetadataTypeDef,
-    SendAlexaOfferToMasterRequestRequestTypeDef,
-    GetIceServerConfigResponseTypeDef,
-    SendAlexaOfferToMasterResponseTypeDef,
 )
 
 
 def get_value() -> GetIceServerConfigRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-kinesis-video-signaling-2.5.2.post1/types_aiobotocore_kinesis_video_signaling.egg-info/SOURCES.txt` & `types-aiobotocore-kinesis-video-signaling-2.5.2.post2/types_aiobotocore_kinesis_video_signaling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

