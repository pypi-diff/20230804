# Comparing `tmp/types-aiobotocore-cloud9-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cloud9-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloud9-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloud9-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:33 2023, max compression
```

## Comparing `types-aiobotocore-cloud9-2.5.2.post1.tar` & `types-aiobotocore-cloud9-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.849637 types-aiobotocore-cloud9-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-08-02 14:51:59.849637 types-aiobotocore-cloud9-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:59.849637 types-aiobotocore-cloud9-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.845637 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-08-02 14:34:19.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-08-02 14:34:19.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-08-02 14:34:19.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-08-02 14:34:19.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.849637 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-08-02 14:51:59.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:51:59.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:51:59.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.603425 types-aiobotocore-cloud9-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:31.000000 types-aiobotocore-cloud9-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13057 2023-08-04 12:00:33.591424 types-aiobotocore-cloud9-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-08-04 11:41:31.000000 types-aiobotocore-cloud9-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:33.603425 types-aiobotocore-cloud9-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-04 11:41:31.000000 types-aiobotocore-cloud9-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.587424 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-04 11:41:31.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-04 11:41:31.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-04 11:41:32.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-08-04 11:41:32.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-08-04 11:41:32.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-08-04 11:41:33.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-08-04 11:41:32.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-08-04 11:41:32.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-08-04 11:41:32.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:32.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-08-04 11:41:33.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-08-04 11:41:33.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:31.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:33.591424 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13057 2023-08-04 12:00:33.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:00:33.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:33.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:33.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:00:33.000000 types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/LICENSE` & `types-aiobotocore-cloud9-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/PKG-INFO` & `types-aiobotocore-cloud9-2.5.2.post2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloud9
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Cloud9 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Cloud9 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/
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
 [types-aiobotocore-cloud9 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,77 +296,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloud9.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Cloud9` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/literals/).
+
 ```python
-from types_aiobotocore_cloud9.literals import (
-    ConnectionTypeType,
-    DescribeEnvironmentMembershipsPaginatorName,
-    EnvironmentLifecycleStatusType,
-    EnvironmentStatusType,
-    EnvironmentTypeType,
-    ListEnvironmentsPaginatorName,
-    ManagedCredentialsActionType,
-    ManagedCredentialsStatusType,
-    MemberPermissionsType,
-    PermissionsType,
-    Cloud9ServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_cloud9.literals import ConnectionTypeType
 
 
 def check_value(value: ConnectionTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloud9.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Cloud9` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/type_defs/).
+
 ```python
-from types_aiobotocore_cloud9.type_defs import (
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    CreateEnvironmentMembershipRequestRequestTypeDef,
-    EnvironmentMemberTypeDef,
-    DeleteEnvironmentMembershipRequestRequestTypeDef,
-    DeleteEnvironmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeEnvironmentMembershipsRequestRequestTypeDef,
-    DescribeEnvironmentStatusRequestRequestTypeDef,
-    DescribeEnvironmentsRequestRequestTypeDef,
-    EnvironmentLifecycleTypeDef,
-    ListEnvironmentsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateEnvironmentMembershipRequestRequestTypeDef,
-    UpdateEnvironmentRequestRequestTypeDef,
-    CreateEnvironmentEC2RequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateEnvironmentEC2ResultTypeDef,
-    DescribeEnvironmentStatusResultTypeDef,
-    ListEnvironmentsResultTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    CreateEnvironmentMembershipResultTypeDef,
-    DescribeEnvironmentMembershipsResultTypeDef,
-    UpdateEnvironmentMembershipResultTypeDef,
-    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
-    EnvironmentTypeDef,
-    DescribeEnvironmentsResultTypeDef,
-)
+from types_aiobotocore_cloud9.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/README.md` & `types-aiobotocore-cloud9-2.5.2.post2/README.md`

 * *Files 21% similar despite different names*

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
 [types-aiobotocore-cloud9 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,77 +264,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloud9.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Cloud9` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/literals/).
+
 ```python
-from types_aiobotocore_cloud9.literals import (
-    ConnectionTypeType,
-    DescribeEnvironmentMembershipsPaginatorName,
-    EnvironmentLifecycleStatusType,
-    EnvironmentStatusType,
-    EnvironmentTypeType,
-    ListEnvironmentsPaginatorName,
-    ManagedCredentialsActionType,
-    ManagedCredentialsStatusType,
-    MemberPermissionsType,
-    PermissionsType,
-    Cloud9ServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_cloud9.literals import ConnectionTypeType
 
 
 def check_value(value: ConnectionTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloud9.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Cloud9` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/type_defs/).
+
 ```python
-from types_aiobotocore_cloud9.type_defs import (
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    CreateEnvironmentMembershipRequestRequestTypeDef,
-    EnvironmentMemberTypeDef,
-    DeleteEnvironmentMembershipRequestRequestTypeDef,
-    DeleteEnvironmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeEnvironmentMembershipsRequestRequestTypeDef,
-    DescribeEnvironmentStatusRequestRequestTypeDef,
-    DescribeEnvironmentsRequestRequestTypeDef,
-    EnvironmentLifecycleTypeDef,
-    ListEnvironmentsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateEnvironmentMembershipRequestRequestTypeDef,
-    UpdateEnvironmentRequestRequestTypeDef,
-    CreateEnvironmentEC2RequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateEnvironmentEC2ResultTypeDef,
-    DescribeEnvironmentStatusResultTypeDef,
-    ListEnvironmentsResultTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    CreateEnvironmentMembershipResultTypeDef,
-    DescribeEnvironmentMembershipsResultTypeDef,
-    UpdateEnvironmentMembershipResultTypeDef,
-    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
-    EnvironmentTypeDef,
-    DescribeEnvironmentsResultTypeDef,
-)
+from types_aiobotocore_cloud9.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/setup.py` & `types-aiobotocore-cloud9-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloud9",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cloud9"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Cloud9 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/__init__.py` & `types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/__init__.pyi` & `types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/__main__.py` & `types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Cloud9 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Cloud9 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9\nOther"
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

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/client.py` & `types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/client.pyi` & `types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/literals.py` & `types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/literals.pyi` & `types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/paginator.py` & `types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/paginator.pyi` & `types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/type_defs.py` & `types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/type_defs.pyi` & `types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/PKG-INFO` & `types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloud9
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Cloud9 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Cloud9 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/
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
 [types-aiobotocore-cloud9 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/).
 
 See how it helps to find and fix potential bugs:
 
@@ -296,77 +296,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloud9.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Cloud9` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/literals/).
+
 ```python
-from types_aiobotocore_cloud9.literals import (
-    ConnectionTypeType,
-    DescribeEnvironmentMembershipsPaginatorName,
-    EnvironmentLifecycleStatusType,
-    EnvironmentStatusType,
-    EnvironmentTypeType,
-    ListEnvironmentsPaginatorName,
-    ManagedCredentialsActionType,
-    ManagedCredentialsStatusType,
-    MemberPermissionsType,
-    PermissionsType,
-    Cloud9ServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_cloud9.literals import ConnectionTypeType
 
 
 def check_value(value: ConnectionTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloud9.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Cloud9` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/type_defs/).
+
 ```python
-from types_aiobotocore_cloud9.type_defs import (
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    CreateEnvironmentMembershipRequestRequestTypeDef,
-    EnvironmentMemberTypeDef,
-    DeleteEnvironmentMembershipRequestRequestTypeDef,
-    DeleteEnvironmentRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeEnvironmentMembershipsRequestRequestTypeDef,
-    DescribeEnvironmentStatusRequestRequestTypeDef,
-    DescribeEnvironmentsRequestRequestTypeDef,
-    EnvironmentLifecycleTypeDef,
-    ListEnvironmentsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateEnvironmentMembershipRequestRequestTypeDef,
-    UpdateEnvironmentRequestRequestTypeDef,
-    CreateEnvironmentEC2RequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateEnvironmentEC2ResultTypeDef,
-    DescribeEnvironmentStatusResultTypeDef,
-    ListEnvironmentsResultTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    CreateEnvironmentMembershipResultTypeDef,
-    DescribeEnvironmentMembershipsResultTypeDef,
-    UpdateEnvironmentMembershipResultTypeDef,
-    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
-    EnvironmentTypeDef,
-    DescribeEnvironmentsResultTypeDef,
-)
+from types_aiobotocore_cloud9.type_defs import TagTypeDef
 
 
 def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/SOURCES.txt` & `types-aiobotocore-cloud9-2.5.2.post2/types_aiobotocore_cloud9.egg-info/SOURCES.txt`

 * *Files identical despite different names*

