# Comparing `tmp/types-aiobotocore-sagemaker-metrics-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sagemaker-metrics-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-metrics-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-metrics-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
```

## Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1.tar` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.413468 types-aiobotocore-sagemaker-metrics-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:01.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-08-02 14:52:57.413468 types-aiobotocore-sagemaker-metrics-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-08-02 14:49:01.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:57.413468 types-aiobotocore-sagemaker-metrics-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:49:00.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.413468 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-02 14:49:01.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-02 14:49:01.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:49:01.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-08-02 14:49:01.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4716 2023-08-02 14:49:01.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-02 14:49:01.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-02 14:49:01.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:01.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:49:01.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-08-02 14:49:01.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:01.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:57.413468 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12670 2023-08-02 14:52:57.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-08-02 14:52:57.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:57.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:57.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:57.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:57.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.996643 types-aiobotocore-sagemaker-metrics-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12731 2023-08-04 13:59:24.996643 types-aiobotocore-sagemaker-metrics-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11174 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:24.996643 types-aiobotocore-sagemaker-metrics-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2141 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.996643 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      517 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      516 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      981 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4725 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4716 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8417 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8415 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2097 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:52:30.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:24.996643 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12731 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      904 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       36 2023-08-04 13:59:24.000000 types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/LICENSE` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/PKG-INFO` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-metrics
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SageMakerMetrics 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SageMakerMetrics 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/
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
 [types-aiobotocore-sagemaker-metrics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,44 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sagemaker_metrics.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `SageMakerMetrics` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/literals/).
+
 ```python
-from types_aiobotocore_sagemaker_metrics.literals import (
-    PutMetricsErrorCodeType,
-    SageMakerMetricsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_sagemaker_metrics.literals import PutMetricsErrorCodeType
 
 
 def check_value(value: PutMetricsErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sagemaker_metrics.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SageMakerMetrics` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/type_defs/).
+
 ```python
-from types_aiobotocore_sagemaker_metrics.type_defs import (
-    BatchPutMetricsErrorTypeDef,
-    ResponseMetadataTypeDef,
-    TimestampTypeDef,
-    BatchPutMetricsResponseTypeDef,
-    RawMetricDataTypeDef,
-    BatchPutMetricsRequestRequestTypeDef,
-)
+from types_aiobotocore_sagemaker_metrics.type_defs import BatchPutMetricsErrorTypeDef
 
 
 def get_value() -> BatchPutMetricsErrorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/README.md` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/README.md`

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
 [types-aiobotocore-sagemaker-metrics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,44 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sagemaker_metrics.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `SageMakerMetrics` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/literals/).
+
 ```python
-from types_aiobotocore_sagemaker_metrics.literals import (
-    PutMetricsErrorCodeType,
-    SageMakerMetricsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_sagemaker_metrics.literals import PutMetricsErrorCodeType
 
 
 def check_value(value: PutMetricsErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sagemaker_metrics.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SageMakerMetrics` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/type_defs/).
+
 ```python
-from types_aiobotocore_sagemaker_metrics.type_defs import (
-    BatchPutMetricsErrorTypeDef,
-    ResponseMetadataTypeDef,
-    TimestampTypeDef,
-    BatchPutMetricsResponseTypeDef,
-    RawMetricDataTypeDef,
-    BatchPutMetricsRequestRequestTypeDef,
-)
+from types_aiobotocore_sagemaker_metrics.type_defs import BatchPutMetricsErrorTypeDef
 
 
 def get_value() -> BatchPutMetricsErrorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/setup.py` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker-metrics",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sagemaker_metrics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SageMakerMetrics 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/__init__.py` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/__init__.pyi` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/__main__.py` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.SageMakerMetrics 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-metrics.html#SageMakerMetrics\nOther"
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

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/client.py` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/client.pyi` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/literals.py` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/literals.py`

 * *Files 1% similar despite different names*

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
@@ -412,14 +416,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/literals.pyi` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/literals.pyi`

 * *Files 0% similar despite different names*

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
@@ -410,14 +414,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/type_defs.py` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics/type_defs.pyi` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics.egg-info/PKG-INFO` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-metrics
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SageMakerMetrics 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SageMakerMetrics 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/
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
 [types-aiobotocore-sagemaker-metrics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,44 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sagemaker_metrics.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `SageMakerMetrics` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/literals/).
+
 ```python
-from types_aiobotocore_sagemaker_metrics.literals import (
-    PutMetricsErrorCodeType,
-    SageMakerMetricsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_sagemaker_metrics.literals import PutMetricsErrorCodeType
 
 
 def check_value(value: PutMetricsErrorCodeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sagemaker_metrics.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SageMakerMetrics` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_metrics/type_defs/).
+
 ```python
-from types_aiobotocore_sagemaker_metrics.type_defs import (
-    BatchPutMetricsErrorTypeDef,
-    ResponseMetadataTypeDef,
-    TimestampTypeDef,
-    BatchPutMetricsResponseTypeDef,
-    RawMetricDataTypeDef,
-    BatchPutMetricsRequestRequestTypeDef,
-)
+from types_aiobotocore_sagemaker_metrics.type_defs import BatchPutMetricsErrorTypeDef
 
 
 def get_value() -> BatchPutMetricsErrorTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sagemaker-metrics-2.5.2.post1/types_aiobotocore_sagemaker_metrics.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-metrics-2.5.2.post2/types_aiobotocore_sagemaker_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

