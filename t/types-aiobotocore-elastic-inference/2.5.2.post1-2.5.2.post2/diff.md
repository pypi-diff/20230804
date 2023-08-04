# Comparing `tmp/types-aiobotocore-elastic-inference-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-elastic-inference-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elastic-inference-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-elastic-inference-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:50 2023, max compression
```

## Comparing `types-aiobotocore-elastic-inference-2.5.2.post1.tar` & `types-aiobotocore-elastic-inference-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.605594 types-aiobotocore-elastic-inference-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-08-02 14:52:14.601594 types-aiobotocore-elastic-inference-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.605594 types-aiobotocore-elastic-inference-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.601594 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-08-02 14:38:07.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:06.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.601594 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14094 2023-08-02 14:52:14.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:52:14.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:14.000000 types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.300062 types-aiobotocore-elastic-inference-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-08-04 12:00:50.288061 types-aiobotocore-elastic-inference-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:50.300062 types-aiobotocore-elastic-inference-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.284061 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:34.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.288061 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13564 2023-08-04 12:00:50.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 12:00:50.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:50.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:50.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:50.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:00:50.000000 types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/LICENSE` & `types-aiobotocore-elastic-inference-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/PKG-INFO` & `types-aiobotocore-elastic-inference-2.5.2.post2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastic-inference
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ElasticInference 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ElasticInference 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/
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
 [types-aiobotocore-elastic-inference docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,59 +291,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_elastic_inference.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ElasticInference` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/literals/).
+
 ```python
-from types_aiobotocore_elastic_inference.literals import (
-    DescribeAcceleratorsPaginatorName,
-    LocationTypeType,
-    ElasticInferenceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_elastic_inference.literals import DescribeAcceleratorsPaginatorName
 
 
 def check_value(value: DescribeAcceleratorsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_elastic_inference.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ElasticInference` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/type_defs/).
+
 ```python
-from types_aiobotocore_elastic_inference.type_defs import (
-    AcceleratorTypeOfferingTypeDef,
-    KeyValuePairTypeDef,
-    MemoryInfoTypeDef,
-    DescribeAcceleratorOfferingsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    FilterTypeDef,
-    PaginatorConfigTypeDef,
-    ElasticInferenceAcceleratorHealthTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AcceleratorTypeTypeDef,
-    DescribeAcceleratorOfferingsResponseTypeDef,
-    ListTagsForResourceResultTypeDef,
-    DescribeAcceleratorsRequestRequestTypeDef,
-    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
-    ElasticInferenceAcceleratorTypeDef,
-    DescribeAcceleratorTypesResponseTypeDef,
-    DescribeAcceleratorsResponseTypeDef,
-)
+from types_aiobotocore_elastic_inference.type_defs import AcceleratorTypeOfferingTypeDef
 
 
 def get_value() -> AcceleratorTypeOfferingTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/README.md` & `types-aiobotocore-elastic-inference-2.5.2.post2/README.md`

 * *Files 8% similar despite different names*

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
 [types-aiobotocore-elastic-inference docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
 
@@ -259,59 +259,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_elastic_inference.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ElasticInference` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/literals/).
+
 ```python
-from types_aiobotocore_elastic_inference.literals import (
-    DescribeAcceleratorsPaginatorName,
-    LocationTypeType,
-    ElasticInferenceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_elastic_inference.literals import DescribeAcceleratorsPaginatorName
 
 
 def check_value(value: DescribeAcceleratorsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_elastic_inference.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ElasticInference` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/type_defs/).
+
 ```python
-from types_aiobotocore_elastic_inference.type_defs import (
-    AcceleratorTypeOfferingTypeDef,
-    KeyValuePairTypeDef,
-    MemoryInfoTypeDef,
-    DescribeAcceleratorOfferingsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    FilterTypeDef,
-    PaginatorConfigTypeDef,
-    ElasticInferenceAcceleratorHealthTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AcceleratorTypeTypeDef,
-    DescribeAcceleratorOfferingsResponseTypeDef,
-    ListTagsForResourceResultTypeDef,
-    DescribeAcceleratorsRequestRequestTypeDef,
-    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
-    ElasticInferenceAcceleratorTypeDef,
-    DescribeAcceleratorTypesResponseTypeDef,
-    DescribeAcceleratorsResponseTypeDef,
-)
+from types_aiobotocore_elastic_inference.type_defs import AcceleratorTypeOfferingTypeDef
 
 
 def get_value() -> AcceleratorTypeOfferingTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/setup.py` & `types-aiobotocore-elastic-inference-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elastic-inference",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_elastic_inference"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElasticInference 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/__init__.py` & `types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/__init__.pyi` & `types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/__main__.py` & `types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ElasticInference 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastic-inference.html#ElasticInference\nOther"
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

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/client.py` & `types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/client.pyi` & `types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/literals.py` & `types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/literals.pyi` & `types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/paginator.py` & `types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/paginator.pyi` & `types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/type_defs.py` & `types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference/type_defs.pyi` & `types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/PKG-INFO` & `types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastic-inference
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ElasticInference 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ElasticInference 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/
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
 [types-aiobotocore-elastic-inference docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,59 +291,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_elastic_inference.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ElasticInference` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/literals/).
+
 ```python
-from types_aiobotocore_elastic_inference.literals import (
-    DescribeAcceleratorsPaginatorName,
-    LocationTypeType,
-    ElasticInferenceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_elastic_inference.literals import DescribeAcceleratorsPaginatorName
 
 
 def check_value(value: DescribeAcceleratorsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_elastic_inference.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ElasticInference` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastic_inference/type_defs/).
+
 ```python
-from types_aiobotocore_elastic_inference.type_defs import (
-    AcceleratorTypeOfferingTypeDef,
-    KeyValuePairTypeDef,
-    MemoryInfoTypeDef,
-    DescribeAcceleratorOfferingsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    FilterTypeDef,
-    PaginatorConfigTypeDef,
-    ElasticInferenceAcceleratorHealthTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    AcceleratorTypeTypeDef,
-    DescribeAcceleratorOfferingsResponseTypeDef,
-    ListTagsForResourceResultTypeDef,
-    DescribeAcceleratorsRequestRequestTypeDef,
-    DescribeAcceleratorsRequestDescribeAcceleratorsPaginateTypeDef,
-    ElasticInferenceAcceleratorTypeDef,
-    DescribeAcceleratorTypesResponseTypeDef,
-    DescribeAcceleratorsResponseTypeDef,
-)
+from types_aiobotocore_elastic_inference.type_defs import AcceleratorTypeOfferingTypeDef
 
 
 def get_value() -> AcceleratorTypeOfferingTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-elastic-inference-2.5.2.post1/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt` & `types-aiobotocore-elastic-inference-2.5.2.post2/types_aiobotocore_elastic_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

