# Comparing `tmp/types-aiobotocore-pi-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-pi-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pi-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-pi-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
```

## Comparing `types-aiobotocore-pi-2.5.2.post1.tar` & `types-aiobotocore-pi-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.729498 types-aiobotocore-pi-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:44.000000 types-aiobotocore-pi-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-08-02 14:52:47.729498 types-aiobotocore-pi-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-08-02 14:44:44.000000 types-aiobotocore-pi-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:47.729498 types-aiobotocore-pi-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-08-02 14:44:44.000000 types-aiobotocore-pi-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.729498 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-02 14:44:44.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-08-02 14:44:44.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-08-02 14:44:44.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-08-02 14:44:44.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8741 2023-08-02 14:44:44.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-08-02 14:44:44.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-08-02 14:44:44.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:44.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-08-02 14:44:45.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10529 2023-08-02 14:44:45.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:44.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.729498 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12800 2023-08-02 14:52:47.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-02 14:52:47.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:47.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:47.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:47.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 14:52:47.000000 types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.136643 types-aiobotocore-pi-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11907 2023-08-04 13:59:21.136643 types-aiobotocore-pi-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10409 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.136643 types-aiobotocore-pi-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2002 2023-08-04 13:46:37.000000 types-aiobotocore-pi-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.136643 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      402 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      401 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      912 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8755 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8741 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8581 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8579 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10546 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10529 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:38.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.136643 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11907 2023-08-04 13:59:21.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      649 2023-08-04 13:59:21.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       21 2023-08-04 13:59:21.000000 types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pi-2.5.2.post1/LICENSE` & `types-aiobotocore-pi-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.5.2.post1/PKG-INFO` & `types-aiobotocore-pi-2.5.2.post2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-pi
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.PI 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.PI 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/
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
 [types-aiobotocore-pi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,68 +264,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_pi.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `PI` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/literals/).
+
 ```python
-from types_aiobotocore_pi.literals import (
-    DetailStatusType,
-    FeatureStatusType,
-    PeriodAlignmentType,
-    ServiceTypeType,
-    PIServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_pi.literals import DetailStatusType
 
 
 def check_value(value: DetailStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_pi.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `PI` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/type_defs/).
+
 ```python
-from types_aiobotocore_pi.type_defs import (
-    DataPointTypeDef,
-    DimensionGroupTypeDef,
-    TimestampTypeDef,
-    DimensionKeyDescriptionTypeDef,
-    ResponseMetadataTypeDef,
-    ResponsePartitionKeyTypeDef,
-    DimensionDetailTypeDef,
-    DimensionKeyDetailTypeDef,
-    FeatureMetadataTypeDef,
-    GetDimensionKeyDetailsRequestRequestTypeDef,
-    GetResourceMetadataRequestRequestTypeDef,
-    ListAvailableResourceDimensionsRequestRequestTypeDef,
-    ListAvailableResourceMetricsRequestRequestTypeDef,
-    ResponseResourceMetricTypeDef,
-    ResponseResourceMetricKeyTypeDef,
-    MetricQueryTypeDef,
-    DescribeDimensionKeysRequestRequestTypeDef,
-    DescribeDimensionKeysResponseTypeDef,
-    DimensionGroupDetailTypeDef,
-    GetDimensionKeyDetailsResponseTypeDef,
-    GetResourceMetadataResponseTypeDef,
-    ListAvailableResourceMetricsResponseTypeDef,
-    MetricKeyDataPointsTypeDef,
-    GetResourceMetricsRequestRequestTypeDef,
-    MetricDimensionGroupsTypeDef,
-    GetResourceMetricsResponseTypeDef,
-    ListAvailableResourceDimensionsResponseTypeDef,
-)
+from types_aiobotocore_pi.type_defs import DataPointTypeDef
 
 
 def get_value() -> DataPointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-pi-2.5.2.post1/README.md` & `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-pi
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.PI 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore pi type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-pi"></a>
 
 # types-aiobotocore-pi
 
 [![PyPI - types-aiobotocore-pi](https://img.shields.io/pypi/v/types-aiobotocore-pi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-pi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-pi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/)
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
 [types-aiobotocore-pi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -232,68 +264,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_pi.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `PI` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/literals/).
+
 ```python
-from types_aiobotocore_pi.literals import (
-    DetailStatusType,
-    FeatureStatusType,
-    PeriodAlignmentType,
-    ServiceTypeType,
-    PIServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_pi.literals import DetailStatusType
 
 
 def check_value(value: DetailStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_pi.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `PI` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi/type_defs/).
+
 ```python
-from types_aiobotocore_pi.type_defs import (
-    DataPointTypeDef,
-    DimensionGroupTypeDef,
-    TimestampTypeDef,
-    DimensionKeyDescriptionTypeDef,
-    ResponseMetadataTypeDef,
-    ResponsePartitionKeyTypeDef,
-    DimensionDetailTypeDef,
-    DimensionKeyDetailTypeDef,
-    FeatureMetadataTypeDef,
-    GetDimensionKeyDetailsRequestRequestTypeDef,
-    GetResourceMetadataRequestRequestTypeDef,
-    ListAvailableResourceDimensionsRequestRequestTypeDef,
-    ListAvailableResourceMetricsRequestRequestTypeDef,
-    ResponseResourceMetricTypeDef,
-    ResponseResourceMetricKeyTypeDef,
-    MetricQueryTypeDef,
-    DescribeDimensionKeysRequestRequestTypeDef,
-    DescribeDimensionKeysResponseTypeDef,
-    DimensionGroupDetailTypeDef,
-    GetDimensionKeyDetailsResponseTypeDef,
-    GetResourceMetadataResponseTypeDef,
-    ListAvailableResourceMetricsResponseTypeDef,
-    MetricKeyDataPointsTypeDef,
-    GetResourceMetricsRequestRequestTypeDef,
-    MetricDimensionGroupsTypeDef,
-    GetResourceMetricsResponseTypeDef,
-    ListAvailableResourceDimensionsResponseTypeDef,
-)
+from types_aiobotocore_pi.type_defs import DataPointTypeDef
 
 
 def get_value() -> DataPointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-pi-2.5.2.post1/setup.py` & `types-aiobotocore-pi-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pi",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_pi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for aiobotocore.PI 2.5.2 service generated with mypy-boto3-builder 7.17.1"
+        "Type annotations for aiobotocore.PI 2.5.2 service generated with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/__main__.py` & `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.PI 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.PI 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pi//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pi.html#PI\nOther"
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

### Comparing `types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/client.py` & `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/client.pyi` & `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/literals.py` & `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
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
@@ -157,14 +158,15 @@
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
@@ -243,26 +245,28 @@
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
@@ -423,14 +427,15 @@
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

### Comparing `types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/literals.pyi` & `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,15 @@
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
@@ -155,14 +156,15 @@
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
@@ -241,26 +243,28 @@
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
@@ -421,14 +425,15 @@
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

### Comparing `types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/type_defs.py` & `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi/type_defs.pyi` & `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pi-2.5.2.post1/types_aiobotocore_pi.egg-info/SOURCES.txt` & `types-aiobotocore-pi-2.5.2.post2/types_aiobotocore_pi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

