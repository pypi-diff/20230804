# Comparing `tmp/types-aiobotocore-workmailmessageflow-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-workmailmessageflow-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-workmailmessageflow-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-workmailmessageflow-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:30 2023, max compression
```

## Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1.tar` & `types-aiobotocore-workmailmessageflow-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.289424 types-aiobotocore-workmailmessageflow-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:21.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-08-02 14:53:11.289424 types-aiobotocore-workmailmessageflow-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-08-02 14:51:21.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:11.289424 types-aiobotocore-workmailmessageflow-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-02 14:51:21.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.289424 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-02 14:51:21.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-02 14:51:21.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-02 14:51:22.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-08-02 14:51:22.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5586 2023-08-02 14:51:22.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-08-02 14:51:22.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-08-02 14:51:22.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:22.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:51:22.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-08-02 14:51:22.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:21.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.289424 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12784 2023-08-02 14:53:11.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-02 14:53:11.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:11.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:11.000000 types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.216643 types-aiobotocore-workmailmessageflow-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12897 2023-08-04 13:59:30.216643 types-aiobotocore-workmailmessageflow-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11331 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.216643 types-aiobotocore-workmailmessageflow-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2132 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.216643 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      538 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      537 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      991 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5596 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5586 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7708 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7706 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2104 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:56:17.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:30.216643 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12897 2023-08-04 13:59:30.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      938 2023-08-04 13:59:30.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:30.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:30.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:30.000000 types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/LICENSE` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/PKG-INFO` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workmailmessageflow
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.WorkMailMessageFlow 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.WorkMailMessageFlow 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmailmessageflow/
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
 [types-aiobotocore-workmailmessageflow docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmailmessageflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,42 +266,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_workmailmessageflow.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `WorkMailMessageFlow` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmailmessageflow/literals/).
+
 ```python
-from types_aiobotocore_workmailmessageflow.literals import (
-    WorkMailMessageFlowServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_workmailmessageflow.literals import WorkMailMessageFlowServiceName
 
 
 def check_value(value: WorkMailMessageFlowServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_workmailmessageflow.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `WorkMailMessageFlow` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmailmessageflow/type_defs/).
+
 ```python
 from types_aiobotocore_workmailmessageflow.type_defs import (
     GetRawMessageContentRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    S3ReferenceTypeDef,
-    GetRawMessageContentResponseTypeDef,
-    RawMessageContentTypeDef,
-    PutRawMessageContentRequestRequestTypeDef,
 )
 
 
 def get_value() -> GetRawMessageContentRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/README.md` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/README.md`

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
 [types-aiobotocore-workmailmessageflow docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmailmessageflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,42 +234,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_workmailmessageflow.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `WorkMailMessageFlow` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmailmessageflow/literals/).
+
 ```python
-from types_aiobotocore_workmailmessageflow.literals import (
-    WorkMailMessageFlowServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_workmailmessageflow.literals import WorkMailMessageFlowServiceName
 
 
 def check_value(value: WorkMailMessageFlowServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_workmailmessageflow.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `WorkMailMessageFlow` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmailmessageflow/type_defs/).
+
 ```python
 from types_aiobotocore_workmailmessageflow.type_defs import (
     GetRawMessageContentRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    S3ReferenceTypeDef,
-    GetRawMessageContentResponseTypeDef,
-    RawMessageContentTypeDef,
-    PutRawMessageContentRequestRequestTypeDef,
 )
 
 
 def get_value() -> GetRawMessageContentRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/setup.py` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-workmailmessageflow",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_workmailmessageflow"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.WorkMailMessageFlow 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/__init__.py` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/__init__.pyi` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/__main__.py` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.WorkMailMessageFlow 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmailmessageflow//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/workmailmessageflow.html#WorkMailMessageFlow\nOther"
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

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/client.py` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/client.pyi` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/literals.py` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
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
@@ -137,14 +138,15 @@
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
@@ -223,26 +225,28 @@
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

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/literals.pyi` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
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
@@ -135,14 +136,15 @@
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
@@ -221,26 +223,28 @@
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

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/type_defs.py` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow/type_defs.pyi` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow.egg-info/PKG-INFO` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-workmailmessageflow
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.WorkMailMessageFlow 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.WorkMailMessageFlow 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmailmessageflow/
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
 [types-aiobotocore-workmailmessageflow docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmailmessageflow/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,42 +266,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_workmailmessageflow.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `WorkMailMessageFlow` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmailmessageflow/literals/).
+
 ```python
-from types_aiobotocore_workmailmessageflow.literals import (
-    WorkMailMessageFlowServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_workmailmessageflow.literals import WorkMailMessageFlowServiceName
 
 
 def check_value(value: WorkMailMessageFlowServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_workmailmessageflow.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `WorkMailMessageFlow` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_workmailmessageflow/type_defs/).
+
 ```python
 from types_aiobotocore_workmailmessageflow.type_defs import (
     GetRawMessageContentRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    S3ReferenceTypeDef,
-    GetRawMessageContentResponseTypeDef,
-    RawMessageContentTypeDef,
-    PutRawMessageContentRequestRequestTypeDef,
 )
 
 
 def get_value() -> GetRawMessageContentRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-workmailmessageflow-2.5.2.post1/types_aiobotocore_workmailmessageflow.egg-info/SOURCES.txt` & `types-aiobotocore-workmailmessageflow-2.5.2.post2/types_aiobotocore_workmailmessageflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

