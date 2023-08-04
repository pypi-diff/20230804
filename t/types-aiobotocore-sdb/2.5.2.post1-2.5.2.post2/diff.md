# Comparing `tmp/types-aiobotocore-sdb-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sdb-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sdb-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-sdb-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
```

## Comparing `types-aiobotocore-sdb-2.5.2.post1.tar` & `types-aiobotocore-sdb-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.289462 types-aiobotocore-sdb-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-08-02 14:52:59.281462 types-aiobotocore-sdb-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:59.289462 types-aiobotocore-sdb-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-08-02 14:49:04.000000 types-aiobotocore-sdb-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.277462 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11682 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.281462 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-08-02 14:52:59.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:59.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:59.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:59.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.716643 types-aiobotocore-sdb-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12794 2023-08-04 13:59:25.716643 types-aiobotocore-sdb-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11287 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.716643 types-aiobotocore-sdb-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2025 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.716643 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      754 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      753 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      926 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11703 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11682 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8032 2023-08-04 13:52:42.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8030 2023-08-04 13:52:42.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2923 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2919 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8650 2023-08-04 13:52:42.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8631 2023-08-04 13:52:42.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:41.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.716643 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12794 2023-08-04 13:59:25.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:25.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:25.000000 types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sdb-2.5.2.post1/LICENSE` & `types-aiobotocore-sdb-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post1/PKG-INFO` & `types-aiobotocore-sdb-2.5.2.post2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sdb
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SimpleDB 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SimpleDB 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/
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
 [types-aiobotocore-sdb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,65 +288,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sdb.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `SimpleDB` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/literals/).
+
 ```python
-from types_aiobotocore_sdb.literals import (
-    ListDomainsPaginatorName,
-    SelectPaginatorName,
-    SimpleDBServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_sdb.literals import ListDomainsPaginatorName
 
 
 def check_value(value: ListDomainsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sdb.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SimpleDB` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/type_defs/).
+
 ```python
-from types_aiobotocore_sdb.type_defs import (
-    AttributeTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    UpdateConditionTypeDef,
-    DeleteDomainRequestRequestTypeDef,
-    DomainMetadataRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetAttributesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListDomainsRequestRequestTypeDef,
-    ReplaceableAttributeTypeDef,
-    SelectRequestRequestTypeDef,
-    DeletableItemTypeDef,
-    ItemTypeDef,
-    DeleteAttributesRequestRequestTypeDef,
-    DomainMetadataResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAttributesResultTypeDef,
-    ListDomainsResultTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    SelectRequestSelectPaginateTypeDef,
-    PutAttributesRequestRequestTypeDef,
-    ReplaceableItemTypeDef,
-    BatchDeleteAttributesRequestRequestTypeDef,
-    SelectResultTypeDef,
-    BatchPutAttributesRequestRequestTypeDef,
-)
+from types_aiobotocore_sdb.type_defs import AttributeTypeDef
 
 
 def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sdb-2.5.2.post1/README.md` & `types-aiobotocore-sdb-2.5.2.post2/README.md`

 * *Files 11% similar despite different names*

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
 [types-aiobotocore-sdb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -256,65 +256,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sdb.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `SimpleDB` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/literals/).
+
 ```python
-from types_aiobotocore_sdb.literals import (
-    ListDomainsPaginatorName,
-    SelectPaginatorName,
-    SimpleDBServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_sdb.literals import ListDomainsPaginatorName
 
 
 def check_value(value: ListDomainsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sdb.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SimpleDB` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/type_defs/).
+
 ```python
-from types_aiobotocore_sdb.type_defs import (
-    AttributeTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    UpdateConditionTypeDef,
-    DeleteDomainRequestRequestTypeDef,
-    DomainMetadataRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetAttributesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListDomainsRequestRequestTypeDef,
-    ReplaceableAttributeTypeDef,
-    SelectRequestRequestTypeDef,
-    DeletableItemTypeDef,
-    ItemTypeDef,
-    DeleteAttributesRequestRequestTypeDef,
-    DomainMetadataResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAttributesResultTypeDef,
-    ListDomainsResultTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    SelectRequestSelectPaginateTypeDef,
-    PutAttributesRequestRequestTypeDef,
-    ReplaceableItemTypeDef,
-    BatchDeleteAttributesRequestRequestTypeDef,
-    SelectResultTypeDef,
-    BatchPutAttributesRequestRequestTypeDef,
-)
+from types_aiobotocore_sdb.type_defs import AttributeTypeDef
 
 
 def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sdb-2.5.2.post1/setup.py` & `types-aiobotocore-sdb-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sdb",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SimpleDB 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/__init__.py` & `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/__init__.pyi` & `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/__main__.py` & `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SimpleDB 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SimpleDB 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB\nOther"
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

### Comparing `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/client.py` & `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/client.pyi` & `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/literals.py` & `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,15 @@
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
@@ -147,14 +148,15 @@
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
@@ -233,26 +235,28 @@
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

### Comparing `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/literals.pyi` & `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,15 @@
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
@@ -145,14 +146,15 @@
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
@@ -231,26 +233,28 @@
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

### Comparing `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/paginator.py` & `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/paginator.pyi` & `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/type_defs.py` & `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/type_defs.pyi` & `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/PKG-INFO` & `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sdb
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SimpleDB 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SimpleDB 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/
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
 [types-aiobotocore-sdb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/).
 
 See how it helps to find and fix potential bugs:
 
@@ -288,65 +288,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sdb.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `SimpleDB` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/literals/).
+
 ```python
-from types_aiobotocore_sdb.literals import (
-    ListDomainsPaginatorName,
-    SelectPaginatorName,
-    SimpleDBServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_sdb.literals import ListDomainsPaginatorName
 
 
 def check_value(value: ListDomainsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sdb.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SimpleDB` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/type_defs/).
+
 ```python
-from types_aiobotocore_sdb.type_defs import (
-    AttributeTypeDef,
-    CreateDomainRequestRequestTypeDef,
-    UpdateConditionTypeDef,
-    DeleteDomainRequestRequestTypeDef,
-    DomainMetadataRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetAttributesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListDomainsRequestRequestTypeDef,
-    ReplaceableAttributeTypeDef,
-    SelectRequestRequestTypeDef,
-    DeletableItemTypeDef,
-    ItemTypeDef,
-    DeleteAttributesRequestRequestTypeDef,
-    DomainMetadataResultTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetAttributesResultTypeDef,
-    ListDomainsResultTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    SelectRequestSelectPaginateTypeDef,
-    PutAttributesRequestRequestTypeDef,
-    ReplaceableItemTypeDef,
-    BatchDeleteAttributesRequestRequestTypeDef,
-    SelectResultTypeDef,
-    BatchPutAttributesRequestRequestTypeDef,
-)
+from types_aiobotocore_sdb.type_defs import AttributeTypeDef
 
 
 def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/SOURCES.txt` & `types-aiobotocore-sdb-2.5.2.post2/types_aiobotocore_sdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

