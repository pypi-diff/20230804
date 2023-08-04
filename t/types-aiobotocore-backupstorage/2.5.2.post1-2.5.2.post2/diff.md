# Comparing `tmp/types-aiobotocore-backupstorage-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-backupstorage-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-backupstorage-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-backupstorage-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:28 2023, max compression
```

## Comparing `types-aiobotocore-backupstorage-2.5.2.post1.tar` & `types-aiobotocore-backupstorage-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.337648 types-aiobotocore-backupstorage-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-08-02 14:51:55.333648 types-aiobotocore-backupstorage-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.337648 types-aiobotocore-backupstorage-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.329648 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-08-02 14:33:47.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.333648 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-08-02 14:51:55.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 14:51:55.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:55.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:51:55.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.387228 types-aiobotocore-backupstorage-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-08-04 12:00:28.387228 types-aiobotocore-backupstorage-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:28.387228 types-aiobotocore-backupstorage-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.379228 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:58.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:28.387228 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-08-04 12:00:28.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-04 12:00:28.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:28.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:28.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:28.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:00:28.000000 types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-backupstorage-2.5.2.post1/LICENSE` & `types-aiobotocore-backupstorage-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2.post1/PKG-INFO` & `types-aiobotocore-backupstorage-2.5.2.post2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backupstorage
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.BackupStorage 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.BackupStorage 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/
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
 [types-aiobotocore-backupstorage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,62 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_backupstorage.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `BackupStorage` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/literals/).
+
 ```python
-from types_aiobotocore_backupstorage.literals import (
-    DataChecksumAlgorithmType,
-    SummaryChecksumAlgorithmType,
-    BackupStorageServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_backupstorage.literals import DataChecksumAlgorithmType
 
 
 def check_value(value: DataChecksumAlgorithmType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_backupstorage.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `BackupStorage` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/type_defs/).
+
 ```python
-from types_aiobotocore_backupstorage.type_defs import (
-    BackupObjectTypeDef,
-    BlobTypeDef,
-    ChunkTypeDef,
-    DeleteObjectInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetChunkInputRequestTypeDef,
-    GetObjectMetadataInputRequestTypeDef,
-    ListChunksInputRequestTypeDef,
-    TimestampTypeDef,
-    StartObjectInputRequestTypeDef,
-    NotifyObjectCompleteInputRequestTypeDef,
-    PutChunkInputRequestTypeDef,
-    PutObjectInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChunkOutputTypeDef,
-    GetObjectMetadataOutputTypeDef,
-    ListChunksOutputTypeDef,
-    ListObjectsOutputTypeDef,
-    NotifyObjectCompleteOutputTypeDef,
-    PutChunkOutputTypeDef,
-    PutObjectOutputTypeDef,
-    StartObjectOutputTypeDef,
-    ListObjectsInputRequestTypeDef,
-)
+from types_aiobotocore_backupstorage.type_defs import BackupObjectTypeDef
 
 
 def get_value() -> BackupObjectTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-backupstorage-2.5.2.post1/README.md` & `types-aiobotocore-backupstorage-2.5.2.post2/README.md`

 * *Files 7% similar despite different names*

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
 [types-aiobotocore-backupstorage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,62 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_backupstorage.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `BackupStorage` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/literals/).
+
 ```python
-from types_aiobotocore_backupstorage.literals import (
-    DataChecksumAlgorithmType,
-    SummaryChecksumAlgorithmType,
-    BackupStorageServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_backupstorage.literals import DataChecksumAlgorithmType
 
 
 def check_value(value: DataChecksumAlgorithmType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_backupstorage.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `BackupStorage` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/type_defs/).
+
 ```python
-from types_aiobotocore_backupstorage.type_defs import (
-    BackupObjectTypeDef,
-    BlobTypeDef,
-    ChunkTypeDef,
-    DeleteObjectInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetChunkInputRequestTypeDef,
-    GetObjectMetadataInputRequestTypeDef,
-    ListChunksInputRequestTypeDef,
-    TimestampTypeDef,
-    StartObjectInputRequestTypeDef,
-    NotifyObjectCompleteInputRequestTypeDef,
-    PutChunkInputRequestTypeDef,
-    PutObjectInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChunkOutputTypeDef,
-    GetObjectMetadataOutputTypeDef,
-    ListChunksOutputTypeDef,
-    ListObjectsOutputTypeDef,
-    NotifyObjectCompleteOutputTypeDef,
-    PutChunkOutputTypeDef,
-    PutObjectOutputTypeDef,
-    StartObjectOutputTypeDef,
-    ListObjectsInputRequestTypeDef,
-)
+from types_aiobotocore_backupstorage.type_defs import BackupObjectTypeDef
 
 
 def get_value() -> BackupObjectTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-backupstorage-2.5.2.post1/setup.py` & `types-aiobotocore-backupstorage-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-backupstorage",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_backupstorage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.BackupStorage 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/__main__.py` & `types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.BackupStorage 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage\nOther"
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

### Comparing `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/client.py` & `types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/client.pyi` & `types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/literals.py` & `types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/literals.pyi` & `types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/type_defs.py` & `types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/type_defs.pyi` & `types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/PKG-INFO` & `types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backupstorage
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.BackupStorage 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.BackupStorage 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/
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
 [types-aiobotocore-backupstorage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,62 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_backupstorage.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `BackupStorage` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/literals/).
+
 ```python
-from types_aiobotocore_backupstorage.literals import (
-    DataChecksumAlgorithmType,
-    SummaryChecksumAlgorithmType,
-    BackupStorageServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_backupstorage.literals import DataChecksumAlgorithmType
 
 
 def check_value(value: DataChecksumAlgorithmType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_backupstorage.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `BackupStorage` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/type_defs/).
+
 ```python
-from types_aiobotocore_backupstorage.type_defs import (
-    BackupObjectTypeDef,
-    BlobTypeDef,
-    ChunkTypeDef,
-    DeleteObjectInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetChunkInputRequestTypeDef,
-    GetObjectMetadataInputRequestTypeDef,
-    ListChunksInputRequestTypeDef,
-    TimestampTypeDef,
-    StartObjectInputRequestTypeDef,
-    NotifyObjectCompleteInputRequestTypeDef,
-    PutChunkInputRequestTypeDef,
-    PutObjectInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetChunkOutputTypeDef,
-    GetObjectMetadataOutputTypeDef,
-    ListChunksOutputTypeDef,
-    ListObjectsOutputTypeDef,
-    NotifyObjectCompleteOutputTypeDef,
-    PutChunkOutputTypeDef,
-    PutObjectOutputTypeDef,
-    StartObjectOutputTypeDef,
-    ListObjectsInputRequestTypeDef,
-)
+from types_aiobotocore_backupstorage.type_defs import BackupObjectTypeDef
 
 
 def get_value() -> BackupObjectTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/SOURCES.txt` & `types-aiobotocore-backupstorage-2.5.2.post2/types_aiobotocore_backupstorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

