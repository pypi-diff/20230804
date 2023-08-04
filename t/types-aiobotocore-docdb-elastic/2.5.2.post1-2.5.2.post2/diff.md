# Comparing `tmp/types-aiobotocore-docdb-elastic-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-docdb-elastic-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-docdb-elastic-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-docdb-elastic-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:47 2023, max compression
```

## Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1.tar` & `types-aiobotocore-docdb-elastic-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.953601 types-aiobotocore-docdb-elastic-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14465 2023-08-02 14:52:11.949601 types-aiobotocore-docdb-elastic-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12924 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:11.953601 types-aiobotocore-docdb-elastic-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.933601 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-08-02 14:36:40.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:38.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:11.949601 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14465 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:11.000000 types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.235946 types-aiobotocore-docdb-elastic-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:44:00.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13387 2023-08-04 12:00:47.223945 types-aiobotocore-docdb-elastic-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11846 2023-08-04 11:44:00.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:47.235946 types-aiobotocore-docdb-elastic-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-04 11:44:00.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.223945 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-08-04 11:44:00.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-04 11:44:00.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-04 11:44:00.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-08-04 11:44:01.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14206 2023-08-04 11:44:00.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-08-04 11:44:01.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-08-04 11:44:01.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-08-04 11:44:01.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-08-04 11:44:01.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:44:00.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-08-04 11:44:02.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10276 2023-08-04 11:44:01.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:44:00.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.223945 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13387 2023-08-04 12:00:47.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-04 12:00:47.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:47.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:00:47.000000 types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/LICENSE` & `types-aiobotocore-docdb-elastic-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/PKG-INFO` & `types-aiobotocore-docdb-elastic-2.5.2.post2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb-elastic
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.DocDBElastic 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.DocDBElastic 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/
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
 [types-aiobotocore-docdb-elastic docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,73 +295,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_docdb_elastic.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `DocDBElastic` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/literals/).
+
 ```python
-from types_aiobotocore_docdb_elastic.literals import (
-    AuthType,
-    ListClusterSnapshotsPaginatorName,
-    ListClustersPaginatorName,
-    StatusType,
-    DocDBElasticServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_docdb_elastic.literals import AuthType
 
 
 def check_value(value: AuthType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_docdb_elastic.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DocDBElastic` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/type_defs/).
+
 ```python
-from types_aiobotocore_docdb_elastic.type_defs import (
-    ClusterInListTypeDef,
-    ClusterSnapshotInListTypeDef,
-    ClusterSnapshotTypeDef,
-    ClusterTypeDef,
-    CreateClusterInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateClusterSnapshotInputRequestTypeDef,
-    DeleteClusterInputRequestTypeDef,
-    DeleteClusterSnapshotInputRequestTypeDef,
-    GetClusterInputRequestTypeDef,
-    GetClusterSnapshotInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListClusterSnapshotsInputRequestTypeDef,
-    ListClustersInputRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    RestoreClusterFromSnapshotInputRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateClusterInputRequestTypeDef,
-    CreateClusterOutputTypeDef,
-    CreateClusterSnapshotOutputTypeDef,
-    DeleteClusterOutputTypeDef,
-    DeleteClusterSnapshotOutputTypeDef,
-    GetClusterOutputTypeDef,
-    GetClusterSnapshotOutputTypeDef,
-    ListClusterSnapshotsOutputTypeDef,
-    ListClustersOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RestoreClusterFromSnapshotOutputTypeDef,
-    UpdateClusterOutputTypeDef,
-    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
-)
+from types_aiobotocore_docdb_elastic.type_defs import ClusterInListTypeDef
 
 
 def get_value() -> ClusterInListTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/README.md` & `types-aiobotocore-docdb-elastic-2.5.2.post2/README.md`

 * *Files 16% similar despite different names*

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
 [types-aiobotocore-docdb-elastic docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/).
 
 See how it helps to find and fix potential bugs:
 
@@ -263,73 +263,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_docdb_elastic.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `DocDBElastic` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/literals/).
+
 ```python
-from types_aiobotocore_docdb_elastic.literals import (
-    AuthType,
-    ListClusterSnapshotsPaginatorName,
-    ListClustersPaginatorName,
-    StatusType,
-    DocDBElasticServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_docdb_elastic.literals import AuthType
 
 
 def check_value(value: AuthType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_docdb_elastic.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DocDBElastic` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/type_defs/).
+
 ```python
-from types_aiobotocore_docdb_elastic.type_defs import (
-    ClusterInListTypeDef,
-    ClusterSnapshotInListTypeDef,
-    ClusterSnapshotTypeDef,
-    ClusterTypeDef,
-    CreateClusterInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateClusterSnapshotInputRequestTypeDef,
-    DeleteClusterInputRequestTypeDef,
-    DeleteClusterSnapshotInputRequestTypeDef,
-    GetClusterInputRequestTypeDef,
-    GetClusterSnapshotInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListClusterSnapshotsInputRequestTypeDef,
-    ListClustersInputRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    RestoreClusterFromSnapshotInputRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateClusterInputRequestTypeDef,
-    CreateClusterOutputTypeDef,
-    CreateClusterSnapshotOutputTypeDef,
-    DeleteClusterOutputTypeDef,
-    DeleteClusterSnapshotOutputTypeDef,
-    GetClusterOutputTypeDef,
-    GetClusterSnapshotOutputTypeDef,
-    ListClusterSnapshotsOutputTypeDef,
-    ListClustersOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RestoreClusterFromSnapshotOutputTypeDef,
-    UpdateClusterOutputTypeDef,
-    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
-)
+from types_aiobotocore_docdb_elastic.type_defs import ClusterInListTypeDef
 
 
 def get_value() -> ClusterInListTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/setup.py` & `types-aiobotocore-docdb-elastic-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-docdb-elastic",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_docdb_elastic"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DocDBElastic 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/__init__.py` & `types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/__init__.pyi` & `types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/__main__.py` & `types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DocDBElastic 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.DocDBElastic 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/docdb-elastic.html#DocDBElastic\nOther"
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

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/client.py` & `types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/client.pyi` & `types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/literals.py` & `types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/literals.pyi` & `types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/paginator.py` & `types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/paginator.pyi` & `types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/type_defs.py` & `types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic/type_defs.pyi` & `types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO` & `types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-docdb-elastic
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.DocDBElastic 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.DocDBElastic 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/
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
 [types-aiobotocore-docdb-elastic docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/).
 
 See how it helps to find and fix potential bugs:
 
@@ -295,73 +295,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_docdb_elastic.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `DocDBElastic` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/literals/).
+
 ```python
-from types_aiobotocore_docdb_elastic.literals import (
-    AuthType,
-    ListClusterSnapshotsPaginatorName,
-    ListClustersPaginatorName,
-    StatusType,
-    DocDBElasticServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_docdb_elastic.literals import AuthType
 
 
 def check_value(value: AuthType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_docdb_elastic.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `DocDBElastic` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_docdb_elastic/type_defs/).
+
 ```python
-from types_aiobotocore_docdb_elastic.type_defs import (
-    ClusterInListTypeDef,
-    ClusterSnapshotInListTypeDef,
-    ClusterSnapshotTypeDef,
-    ClusterTypeDef,
-    CreateClusterInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateClusterSnapshotInputRequestTypeDef,
-    DeleteClusterInputRequestTypeDef,
-    DeleteClusterSnapshotInputRequestTypeDef,
-    GetClusterInputRequestTypeDef,
-    GetClusterSnapshotInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListClusterSnapshotsInputRequestTypeDef,
-    ListClustersInputRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    RestoreClusterFromSnapshotInputRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateClusterInputRequestTypeDef,
-    CreateClusterOutputTypeDef,
-    CreateClusterSnapshotOutputTypeDef,
-    DeleteClusterOutputTypeDef,
-    DeleteClusterSnapshotOutputTypeDef,
-    GetClusterOutputTypeDef,
-    GetClusterSnapshotOutputTypeDef,
-    ListClusterSnapshotsOutputTypeDef,
-    ListClustersOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RestoreClusterFromSnapshotOutputTypeDef,
-    UpdateClusterOutputTypeDef,
-    ListClusterSnapshotsInputListClusterSnapshotsPaginateTypeDef,
-    ListClustersInputListClustersPaginateTypeDef,
-)
+from types_aiobotocore_docdb_elastic.type_defs import ClusterInListTypeDef
 
 
 def get_value() -> ClusterInListTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-docdb-elastic-2.5.2.post1/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt` & `types-aiobotocore-docdb-elastic-2.5.2.post2/types_aiobotocore_docdb_elastic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

