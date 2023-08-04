# Comparing `tmp/types-aiobotocore-ebs-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ebs-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ebs-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-ebs-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:47 2023, max compression
```

## Comparing `types-aiobotocore-ebs-2.5.2.post1.tar` & `types-aiobotocore-ebs-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.409600 types-aiobotocore-ebs-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12412 2023-08-02 14:52:12.409600 types-aiobotocore-ebs-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10910 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.409600 types-aiobotocore-ebs-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.409600 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-02 14:36:55.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-08-02 14:36:56.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-08-02 14:36:55.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:54.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.409600 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12412 2023-08-02 14:52:12.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 14:52:12.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:12.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:12.000000 types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.771966 types-aiobotocore-ebs-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:44:18.000000 types-aiobotocore-ebs-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-08-04 12:00:47.763966 types-aiobotocore-ebs-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10474 2023-08-04 11:44:18.000000 types-aiobotocore-ebs-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:47.771966 types-aiobotocore-ebs-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:44:17.000000 types-aiobotocore-ebs-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.763966 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-04 11:44:18.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-04 11:44:18.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:44:18.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-08-04 11:44:18.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-08-04 11:44:18.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-04 11:44:18.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-04 11:44:18.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:44:18.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-08-04 11:44:18.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7068 2023-08-04 11:44:18.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:44:18.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.763966 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-08-04 12:00:47.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-04 12:00:47.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:47.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:47.000000 types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ebs-2.5.2.post1/LICENSE` & `types-aiobotocore-ebs-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.5.2.post1/PKG-INFO` & `types-aiobotocore-ebs-2.5.2.post2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ebs
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.EBS 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.EBS 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/
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
 [types-aiobotocore-ebs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,57 +264,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ebs.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `EBS` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/literals/).
+
 ```python
-from types_aiobotocore_ebs.literals import (
-    ChecksumAggregationMethodType,
-    ChecksumAlgorithmType,
-    StatusType,
-    EBSServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_ebs.literals import ChecksumAggregationMethodType
 
 
 def check_value(value: ChecksumAggregationMethodType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ebs.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `EBS` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/type_defs/).
+
 ```python
-from types_aiobotocore_ebs.type_defs import (
-    BlobTypeDef,
-    BlockTypeDef,
-    ChangedBlockTypeDef,
-    CompleteSnapshotRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetSnapshotBlockRequestRequestTypeDef,
-    ListChangedBlocksRequestRequestTypeDef,
-    ListSnapshotBlocksRequestRequestTypeDef,
-    TagTypeDef,
-    PutSnapshotBlockRequestRequestTypeDef,
-    CompleteSnapshotResponseTypeDef,
-    GetSnapshotBlockResponseTypeDef,
-    ListChangedBlocksResponseTypeDef,
-    ListSnapshotBlocksResponseTypeDef,
-    PutSnapshotBlockResponseTypeDef,
-    StartSnapshotRequestRequestTypeDef,
-    StartSnapshotResponseTypeDef,
-)
+from types_aiobotocore_ebs.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ebs-2.5.2.post1/README.md` & `types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-ebs
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.EBS 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore ebs type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-ebs"></a>
 
 # types-aiobotocore-ebs
 
 [![PyPI - types-aiobotocore-ebs](https://img.shields.io/pypi/v/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ebs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ebs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/)
@@ -15,15 +47,15 @@
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
 [types-aiobotocore-ebs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/).
 
 See how it helps to find and fix potential bugs:
 
@@ -232,57 +264,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ebs.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `EBS` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/literals/).
+
 ```python
-from types_aiobotocore_ebs.literals import (
-    ChecksumAggregationMethodType,
-    ChecksumAlgorithmType,
-    StatusType,
-    EBSServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_ebs.literals import ChecksumAggregationMethodType
 
 
 def check_value(value: ChecksumAggregationMethodType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ebs.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `EBS` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs/type_defs/).
+
 ```python
-from types_aiobotocore_ebs.type_defs import (
-    BlobTypeDef,
-    BlockTypeDef,
-    ChangedBlockTypeDef,
-    CompleteSnapshotRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetSnapshotBlockRequestRequestTypeDef,
-    ListChangedBlocksRequestRequestTypeDef,
-    ListSnapshotBlocksRequestRequestTypeDef,
-    TagTypeDef,
-    PutSnapshotBlockRequestRequestTypeDef,
-    CompleteSnapshotResponseTypeDef,
-    GetSnapshotBlockResponseTypeDef,
-    ListChangedBlocksResponseTypeDef,
-    ListSnapshotBlocksResponseTypeDef,
-    PutSnapshotBlockResponseTypeDef,
-    StartSnapshotRequestRequestTypeDef,
-    StartSnapshotResponseTypeDef,
-)
+from types_aiobotocore_ebs.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ebs-2.5.2.post1/setup.py` & `types-aiobotocore-ebs-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ebs",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ebs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EBS 2.5.2 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/__main__.py` & `types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EBS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.EBS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ebs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ebs.html#EBS\nOther"
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

### Comparing `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/client.py` & `types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/client.pyi` & `types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/literals.py` & `types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/literals.pyi` & `types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/type_defs.py` & `types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs/type_defs.pyi` & `types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ebs-2.5.2.post1/types_aiobotocore_ebs.egg-info/SOURCES.txt` & `types-aiobotocore-ebs-2.5.2.post2/types_aiobotocore_ebs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

