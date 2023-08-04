# Comparing `tmp/types-aiobotocore-route53-recovery-cluster-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-route53-recovery-cluster-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53-recovery-cluster-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:54 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53-recovery-cluster-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
```

## Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1.tar` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.677476 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-08-02 14:52:54.677476 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:54.677476 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.673476 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.677476 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.856643 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13997 2023-08-04 13:59:23.856643 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12413 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.856643 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2181 2023-08-04 13:51:06.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.856643 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      805 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      804 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1007 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8343 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8329 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8011 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8009 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2282 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2279 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4499 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4495 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:07.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.856643 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13997 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1136 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       43 2023-08-04 13:59:23.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/LICENSE` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/PKG-INFO` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-cluster
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Route53RecoveryCluster 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Route53RecoveryCluster 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/
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
 [types-aiobotocore-route53-recovery-cluster docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,50 +291,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_route53_recovery_cluster.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `Route53RecoveryCluster` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/literals/).
+
 ```python
-from types_aiobotocore_route53_recovery_cluster.literals import (
-    ListRoutingControlsPaginatorName,
-    RoutingControlStateType,
-    Route53RecoveryClusterServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_route53_recovery_cluster.literals import ListRoutingControlsPaginatorName
 
 
 def check_value(value: ListRoutingControlsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_route53_recovery_cluster.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `Route53RecoveryCluster` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/type_defs/).
+
 ```python
 from types_aiobotocore_route53_recovery_cluster.type_defs import (
     GetRoutingControlStateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    ListRoutingControlsRequestRequestTypeDef,
-    RoutingControlTypeDef,
-    UpdateRoutingControlStateEntryTypeDef,
-    UpdateRoutingControlStateRequestRequestTypeDef,
-    GetRoutingControlStateResponseTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-    ListRoutingControlsResponseTypeDef,
-    UpdateRoutingControlStatesRequestRequestTypeDef,
 )
 
 
 def get_value() -> GetRoutingControlStateRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/README.md` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/README.md`

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
 [types-aiobotocore-route53-recovery-cluster docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/).
 
 See how it helps to find and fix potential bugs:
 
@@ -259,50 +259,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_route53_recovery_cluster.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `Route53RecoveryCluster` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/literals/).
+
 ```python
-from types_aiobotocore_route53_recovery_cluster.literals import (
-    ListRoutingControlsPaginatorName,
-    RoutingControlStateType,
-    Route53RecoveryClusterServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_route53_recovery_cluster.literals import ListRoutingControlsPaginatorName
 
 
 def check_value(value: ListRoutingControlsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_route53_recovery_cluster.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `Route53RecoveryCluster` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/type_defs/).
+
 ```python
 from types_aiobotocore_route53_recovery_cluster.type_defs import (
     GetRoutingControlStateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    ListRoutingControlsRequestRequestTypeDef,
-    RoutingControlTypeDef,
-    UpdateRoutingControlStateEntryTypeDef,
-    UpdateRoutingControlStateRequestRequestTypeDef,
-    GetRoutingControlStateResponseTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-    ListRoutingControlsResponseTypeDef,
-    UpdateRoutingControlStatesRequestRequestTypeDef,
 )
 
 
 def get_value() -> GetRoutingControlStateRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/setup.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53-recovery-cluster",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_route53_recovery_cluster"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Route53RecoveryCluster 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/__init__.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/__init__.pyi` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/__main__.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.Route53RecoveryCluster 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster\nOther"
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

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/client.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/client.pyi` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/literals.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
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
@@ -146,14 +147,15 @@
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
@@ -232,26 +234,28 @@
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

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/literals.pyi` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/literals.pyi`

 * *Files 2% similar despite different names*

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

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/paginator.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/paginator.pyi` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/type_defs.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/type_defs.pyi` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/PKG-INFO` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-cluster
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Route53RecoveryCluster 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Route53RecoveryCluster 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/
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
 [types-aiobotocore-route53-recovery-cluster docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,50 +291,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_route53_recovery_cluster.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `Route53RecoveryCluster` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/literals/).
+
 ```python
-from types_aiobotocore_route53_recovery_cluster.literals import (
-    ListRoutingControlsPaginatorName,
-    RoutingControlStateType,
-    Route53RecoveryClusterServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-)
+from types_aiobotocore_route53_recovery_cluster.literals import ListRoutingControlsPaginatorName
 
 
 def check_value(value: ListRoutingControlsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_route53_recovery_cluster.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `Route53RecoveryCluster` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/type_defs/).
+
 ```python
 from types_aiobotocore_route53_recovery_cluster.type_defs import (
     GetRoutingControlStateRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    ListRoutingControlsRequestRequestTypeDef,
-    RoutingControlTypeDef,
-    UpdateRoutingControlStateEntryTypeDef,
-    UpdateRoutingControlStateRequestRequestTypeDef,
-    GetRoutingControlStateResponseTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
-    ListRoutingControlsResponseTypeDef,
-    UpdateRoutingControlStatesRequestRequestTypeDef,
 )
 
 
 def get_value() -> GetRoutingControlStateRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/SOURCES.txt` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post2/types_aiobotocore_route53_recovery_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

