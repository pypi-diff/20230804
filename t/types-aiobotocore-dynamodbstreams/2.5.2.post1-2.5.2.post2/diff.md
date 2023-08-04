# Comparing `tmp/types-aiobotocore-dynamodbstreams-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-dynamodbstreams-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dynamodbstreams-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-dynamodbstreams-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:47 2023, max compression
```

## Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1.tar` & `types-aiobotocore-dynamodbstreams-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.249600 types-aiobotocore-dynamodbstreams-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12983 2023-08-02 14:52:12.245600 types-aiobotocore-dynamodbstreams-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11433 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.249600 types-aiobotocore-dynamodbstreams-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.245600 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.245600 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12983 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.711964 types-aiobotocore-dynamodbstreams-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-08-04 12:00:47.711964 types-aiobotocore-dynamodbstreams-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:47.711964 types-aiobotocore-dynamodbstreams-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.699963 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:44:17.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.711964 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-08-04 12:00:47.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:00:47.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:47.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-04 12:00:47.000000 types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1/LICENSE` & `types-aiobotocore-dynamodbstreams-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1/PKG-INFO` & `types-aiobotocore-dynamodbstreams-2.5.2.post2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodbstreams
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.DynamoDBStreams 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.DynamoDBStreams 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/
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
 [types-aiobotocore-dynamodbstreams docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,60 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_dynamodbstreams.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `DynamoDBStreams` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/literals/).
+
 ```python
-from types_aiobotocore_dynamodbstreams.literals import (
-    KeyTypeType,
-    OperationTypeType,
-    ShardIteratorTypeType,
-    StreamStatusType,
-    StreamViewTypeType,
-    DynamoDBStreamsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_dynamodbstreams.literals import KeyTypeType
 
 
 def check_value(value: KeyTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_dynamodbstreams.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DynamoDBStreams` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/type_defs/).
+
 ```python
-from types_aiobotocore_dynamodbstreams.type_defs import (
-    AttributeValueTypeDef,
-    DescribeStreamInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetRecordsInputRequestTypeDef,
-    GetShardIteratorInputRequestTypeDef,
-    IdentityTypeDef,
-    KeySchemaElementTypeDef,
-    ListStreamsInputRequestTypeDef,
-    StreamTypeDef,
-    StreamRecordTypeDef,
-    SequenceNumberRangeTypeDef,
-    GetShardIteratorOutputTypeDef,
-    ListStreamsOutputTypeDef,
-    RecordTypeDef,
-    ShardTypeDef,
-    GetRecordsOutputTypeDef,
-    StreamDescriptionTypeDef,
-    DescribeStreamOutputTypeDef,
-)
+from types_aiobotocore_dynamodbstreams.type_defs import AttributeValueTypeDef
 
 
 def get_value() -> AttributeValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1/README.md` & `types-aiobotocore-dynamodbstreams-2.5.2.post2/README.md`

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
 [types-aiobotocore-dynamodbstreams docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,60 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_dynamodbstreams.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `DynamoDBStreams` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/literals/).
+
 ```python
-from types_aiobotocore_dynamodbstreams.literals import (
-    KeyTypeType,
-    OperationTypeType,
-    ShardIteratorTypeType,
-    StreamStatusType,
-    StreamViewTypeType,
-    DynamoDBStreamsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_dynamodbstreams.literals import KeyTypeType
 
 
 def check_value(value: KeyTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_dynamodbstreams.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DynamoDBStreams` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/type_defs/).
+
 ```python
-from types_aiobotocore_dynamodbstreams.type_defs import (
-    AttributeValueTypeDef,
-    DescribeStreamInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetRecordsInputRequestTypeDef,
-    GetShardIteratorInputRequestTypeDef,
-    IdentityTypeDef,
-    KeySchemaElementTypeDef,
-    ListStreamsInputRequestTypeDef,
-    StreamTypeDef,
-    StreamRecordTypeDef,
-    SequenceNumberRangeTypeDef,
-    GetShardIteratorOutputTypeDef,
-    ListStreamsOutputTypeDef,
-    RecordTypeDef,
-    ShardTypeDef,
-    GetRecordsOutputTypeDef,
-    StreamDescriptionTypeDef,
-    DescribeStreamOutputTypeDef,
-)
+from types_aiobotocore_dynamodbstreams.type_defs import AttributeValueTypeDef
 
 
 def get_value() -> AttributeValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1/setup.py` & `types-aiobotocore-dynamodbstreams-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dynamodbstreams",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_dynamodbstreams"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DynamoDBStreams 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/__main__.py` & `types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.DynamoDBStreams 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams\nOther"
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

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/client.py` & `types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/client.pyi` & `types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/literals.py` & `types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/literals.pyi` & `types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/type_defs.py` & `types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/type_defs.pyi` & `types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO` & `types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodbstreams
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.DynamoDBStreams 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.DynamoDBStreams 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/
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
 [types-aiobotocore-dynamodbstreams docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,60 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_dynamodbstreams.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `DynamoDBStreams` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/literals/).
+
 ```python
-from types_aiobotocore_dynamodbstreams.literals import (
-    KeyTypeType,
-    OperationTypeType,
-    ShardIteratorTypeType,
-    StreamStatusType,
-    StreamViewTypeType,
-    DynamoDBStreamsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_dynamodbstreams.literals import KeyTypeType
 
 
 def check_value(value: KeyTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_dynamodbstreams.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DynamoDBStreams` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/type_defs/).
+
 ```python
-from types_aiobotocore_dynamodbstreams.type_defs import (
-    AttributeValueTypeDef,
-    DescribeStreamInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetRecordsInputRequestTypeDef,
-    GetShardIteratorInputRequestTypeDef,
-    IdentityTypeDef,
-    KeySchemaElementTypeDef,
-    ListStreamsInputRequestTypeDef,
-    StreamTypeDef,
-    StreamRecordTypeDef,
-    SequenceNumberRangeTypeDef,
-    GetShardIteratorOutputTypeDef,
-    ListStreamsOutputTypeDef,
-    RecordTypeDef,
-    ShardTypeDef,
-    GetRecordsOutputTypeDef,
-    StreamDescriptionTypeDef,
-    DescribeStreamOutputTypeDef,
-)
+from types_aiobotocore_dynamodbstreams.type_defs import AttributeValueTypeDef
 
 
 def get_value() -> AttributeValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt` & `types-aiobotocore-dynamodbstreams-2.5.2.post2/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt`

 * *Files identical despite different names*

