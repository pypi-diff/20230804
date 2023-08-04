# Comparing `tmp/types-aiobotocore-sagemaker-edge-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sagemaker-edge-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-edge-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-edge-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
```

## Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1.tar` & `types-aiobotocore-sagemaker-edge-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.033469 types-aiobotocore-sagemaker-edge-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-08-02 14:52:57.033469 types-aiobotocore-sagemaker-edge-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11367 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:57.033469 types-aiobotocore-sagemaker-edge-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.029469 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.033469 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12919 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.066643 types-aiobotocore-sagemaker-edge-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12597 2023-08-04 13:59:25.066643 types-aiobotocore-sagemaker-edge-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11045 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.066643 types-aiobotocore-sagemaker-edge-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2127 2023-08-04 13:52:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.066643 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      528 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      527 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      983 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6228 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6217 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8169 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8167 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4886 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4884 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:25.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.066643 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12597 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      853 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/LICENSE` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/PKG-INFO` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-edge
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/
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
 [types-aiobotocore-sagemaker-edge docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,57 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sagemaker_edge.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SagemakerEdgeManager` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/literals/).
+
 ```python
-from types_aiobotocore_sagemaker_edge.literals import (
-    ChecksumTypeType,
-    DeploymentStatusType,
-    DeploymentTypeType,
-    FailureHandlingPolicyType,
-    ModelStateType,
-    SagemakerEdgeManagerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_sagemaker_edge.literals import ChecksumTypeType
 
 
 def check_value(value: ChecksumTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sagemaker_edge.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SagemakerEdgeManager` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/type_defs/).
+
 ```python
-from types_aiobotocore_sagemaker_edge.type_defs import (
-    ChecksumTypeDef,
-    DeploymentModelTypeDef,
-    TimestampTypeDef,
-    ResponseMetadataTypeDef,
-    GetDeploymentsRequestRequestTypeDef,
-    GetDeviceRegistrationRequestRequestTypeDef,
-    DefinitionTypeDef,
-    DeploymentResultTypeDef,
-    EdgeMetricTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDeviceRegistrationResultTypeDef,
-    EdgeDeploymentTypeDef,
-    ModelTypeDef,
-    GetDeploymentsResultTypeDef,
-    SendHeartbeatRequestRequestTypeDef,
-)
+from types_aiobotocore_sagemaker_edge.type_defs import ChecksumTypeDef
 
 
 def get_value() -> ChecksumTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/README.md` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/README.md`

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
 [types-aiobotocore-sagemaker-edge docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,57 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sagemaker_edge.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SagemakerEdgeManager` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/literals/).
+
 ```python
-from types_aiobotocore_sagemaker_edge.literals import (
-    ChecksumTypeType,
-    DeploymentStatusType,
-    DeploymentTypeType,
-    FailureHandlingPolicyType,
-    ModelStateType,
-    SagemakerEdgeManagerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_sagemaker_edge.literals import ChecksumTypeType
 
 
 def check_value(value: ChecksumTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sagemaker_edge.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SagemakerEdgeManager` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/type_defs/).
+
 ```python
-from types_aiobotocore_sagemaker_edge.type_defs import (
-    ChecksumTypeDef,
-    DeploymentModelTypeDef,
-    TimestampTypeDef,
-    ResponseMetadataTypeDef,
-    GetDeploymentsRequestRequestTypeDef,
-    GetDeviceRegistrationRequestRequestTypeDef,
-    DefinitionTypeDef,
-    DeploymentResultTypeDef,
-    EdgeMetricTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDeviceRegistrationResultTypeDef,
-    EdgeDeploymentTypeDef,
-    ModelTypeDef,
-    GetDeploymentsResultTypeDef,
-    SendHeartbeatRequestRequestTypeDef,
-)
+from types_aiobotocore_sagemaker_edge.type_defs import ChecksumTypeDef
 
 
 def get_value() -> ChecksumTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/setup.py` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker-edge",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sagemaker_edge"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/__init__.py` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/__init__.pyi` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/__main__.py` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-edge.html#SagemakerEdgeManager\nOther"
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

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/client.py` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/client.pyi` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/literals.py` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
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
@@ -152,14 +153,15 @@
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
@@ -238,26 +240,28 @@
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

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/literals.pyi` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
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
@@ -150,14 +151,15 @@
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
@@ -236,26 +238,28 @@
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

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/type_defs.py` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge/type_defs.pyi` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/PKG-INFO` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-edge
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SagemakerEdgeManager 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/
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
 [types-aiobotocore-sagemaker-edge docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,57 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sagemaker_edge.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SagemakerEdgeManager` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/literals/).
+
 ```python
-from types_aiobotocore_sagemaker_edge.literals import (
-    ChecksumTypeType,
-    DeploymentStatusType,
-    DeploymentTypeType,
-    FailureHandlingPolicyType,
-    ModelStateType,
-    SagemakerEdgeManagerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_sagemaker_edge.literals import ChecksumTypeType
 
 
 def check_value(value: ChecksumTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sagemaker_edge.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SagemakerEdgeManager` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_edge/type_defs/).
+
 ```python
-from types_aiobotocore_sagemaker_edge.type_defs import (
-    ChecksumTypeDef,
-    DeploymentModelTypeDef,
-    TimestampTypeDef,
-    ResponseMetadataTypeDef,
-    GetDeploymentsRequestRequestTypeDef,
-    GetDeviceRegistrationRequestRequestTypeDef,
-    DefinitionTypeDef,
-    DeploymentResultTypeDef,
-    EdgeMetricTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDeviceRegistrationResultTypeDef,
-    EdgeDeploymentTypeDef,
-    ModelTypeDef,
-    GetDeploymentsResultTypeDef,
-    SendHeartbeatRequestRequestTypeDef,
-)
+from types_aiobotocore_sagemaker_edge.type_defs import ChecksumTypeDef
 
 
 def get_value() -> ChecksumTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sagemaker-edge-2.5.2.post1/types_aiobotocore_sagemaker_edge.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-edge-2.5.2.post2/types_aiobotocore_sagemaker_edge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

