# Comparing `tmp/types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:31 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
```

## Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1.tar` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.385549 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-08-02 14:52:31.381549 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:31.385549 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.381549 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.381549 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.326643 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13329 2023-08-04 13:59:14.326643 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11730 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.326643 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2219 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.326643 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      595 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      594 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1021 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5283 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5274 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8134 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8132 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1181 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1180 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:04.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.326643 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13329 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1091 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       47 2023-08-04 13:59:14.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/LICENSE` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/PKG-INFO` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-webrtc-storage
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/
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
 [types-aiobotocore-kinesis-video-webrtc-storage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,20 +270,20 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesis_video_webrtc_storage.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideoWebRTCStorage` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/literals/).
+
 ```python
 from types_aiobotocore_kinesis_video_webrtc_storage.literals import (
     KinesisVideoWebRTCStorageServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
 )
 
 
 def check_value(value: KinesisVideoWebRTCStorageServiceName) -> bool:
     ...
 ```
 
@@ -291,20 +291,19 @@
 
 ### Type definitions
 
 `types_aiobotocore_kinesis_video_webrtc_storage.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `KinesisVideoWebRTCStorage` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/type_defs/).
+
 ```python
-from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import (
-    ResponseMetadataTypeDef,
-    JoinStorageSessionInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-)
+from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/README.md` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/README.md`

 * *Files 2% similar despite different names*

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
 [types-aiobotocore-kinesis-video-webrtc-storage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -238,20 +238,20 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesis_video_webrtc_storage.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideoWebRTCStorage` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/literals/).
+
 ```python
 from types_aiobotocore_kinesis_video_webrtc_storage.literals import (
     KinesisVideoWebRTCStorageServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
 )
 
 
 def check_value(value: KinesisVideoWebRTCStorageServiceName) -> bool:
     ...
 ```
 
@@ -259,20 +259,19 @@
 
 ### Type definitions
 
 `types_aiobotocore_kinesis_video_webrtc_storage.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `KinesisVideoWebRTCStorage` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/type_defs/).
+
 ```python
-from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import (
-    ResponseMetadataTypeDef,
-    JoinStorageSessionInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-)
+from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/setup.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesis-video-webrtc-storage",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_kinesis_video_webrtc_storage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2 service generated with"
-        " mypy-boto3-builder 7.17.1"
+        " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage\nOther"
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

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/client.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/literals.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/literals.py`

 * *Files 2% similar despite different names*

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

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
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
@@ -140,14 +141,15 @@
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
@@ -226,26 +228,28 @@
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

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-webrtc-storage
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/
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
 [types-aiobotocore-kinesis-video-webrtc-storage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -270,20 +270,20 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kinesis_video_webrtc_storage.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `KinesisVideoWebRTCStorage` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/literals/).
+
 ```python
 from types_aiobotocore_kinesis_video_webrtc_storage.literals import (
     KinesisVideoWebRTCStorageServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
 )
 
 
 def check_value(value: KinesisVideoWebRTCStorageServiceName) -> bool:
     ...
 ```
 
@@ -291,20 +291,19 @@
 
 ### Type definitions
 
 `types_aiobotocore_kinesis_video_webrtc_storage.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `KinesisVideoWebRTCStorage` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/type_defs/).
+
 ```python
-from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import (
-    ResponseMetadataTypeDef,
-    JoinStorageSessionInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-)
+from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import ResponseMetadataTypeDef
 
 
 def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

