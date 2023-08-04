# Comparing `tmp/types-aiobotocore-kendra-ranking-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-kendra-ranking-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kendra-ranking-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-kendra-ranking-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:13 2023, max compression
```

## Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1.tar` & `types-aiobotocore-kendra-ranking-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:30.817550 types-aiobotocore-kendra-ranking-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-08-02 14:52:30.813550 types-aiobotocore-kendra-ranking-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:30.817550 types-aiobotocore-kendra-ranking-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:30.809550 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9954 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6894 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:24.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:30.813550 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13193 2023-08-02 14:52:30.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-02 14:52:30.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:30.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:30.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:30.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:30.000000 types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.976642 types-aiobotocore-kendra-ranking-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:52.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12598 2023-08-04 13:59:13.976642 types-aiobotocore-kendra-ranking-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11053 2023-08-04 13:41:52.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:13.976642 types-aiobotocore-kendra-ranking-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2120 2023-08-04 13:41:52.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.976642 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      493 2023-08-04 13:41:53.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      492 2023-08-04 13:41:53.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      969 2023-08-04 13:41:53.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9954 2023-08-04 13:41:53.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9937 2023-08-04 13:41:53.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8351 2023-08-04 13:41:53.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8349 2023-08-04 13:41:53.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:53.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6901 2023-08-04 13:41:53.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6894 2023-08-04 13:41:53.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:53.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:13.976642 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12598 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      853 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:13.000000 types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1/LICENSE` & `types-aiobotocore-kendra-ranking-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1/PKG-INFO` & `types-aiobotocore-kendra-ranking-2.5.2.post2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kendra-ranking
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.KendraRanking 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KendraRanking 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/
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
 [types-aiobotocore-kendra-ranking docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,59 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kendra_ranking.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `KendraRanking` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/literals/).
+
 ```python
-from types_aiobotocore_kendra_ranking.literals import (
-    RescoreExecutionPlanStatusType,
-    KendraRankingServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_kendra_ranking.literals import RescoreExecutionPlanStatusType
 
 
 def check_value(value: RescoreExecutionPlanStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kendra_ranking.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `KendraRanking` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/type_defs/).
+
 ```python
-from types_aiobotocore_kendra_ranking.type_defs import (
-    CapacityUnitsConfigurationTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteRescoreExecutionPlanRequestRequestTypeDef,
-    DescribeRescoreExecutionPlanRequestRequestTypeDef,
-    DocumentTypeDef,
-    ListRescoreExecutionPlansRequestRequestTypeDef,
-    RescoreExecutionPlanSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    RescoreResultItemTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateRescoreExecutionPlanRequestRequestTypeDef,
-    CreateRescoreExecutionPlanRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateRescoreExecutionPlanResponseTypeDef,
-    DescribeRescoreExecutionPlanResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RescoreRequestRequestTypeDef,
-    ListRescoreExecutionPlansResponseTypeDef,
-    RescoreResultTypeDef,
-)
+from types_aiobotocore_kendra_ranking.type_defs import CapacityUnitsConfigurationTypeDef
 
 
 def get_value() -> CapacityUnitsConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1/README.md` & `types-aiobotocore-kendra-ranking-2.5.2.post2/README.md`

 * *Files 12% similar despite different names*

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
 [types-aiobotocore-kendra-ranking docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,59 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kendra_ranking.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `KendraRanking` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/literals/).
+
 ```python
-from types_aiobotocore_kendra_ranking.literals import (
-    RescoreExecutionPlanStatusType,
-    KendraRankingServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_kendra_ranking.literals import RescoreExecutionPlanStatusType
 
 
 def check_value(value: RescoreExecutionPlanStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kendra_ranking.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `KendraRanking` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/type_defs/).
+
 ```python
-from types_aiobotocore_kendra_ranking.type_defs import (
-    CapacityUnitsConfigurationTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteRescoreExecutionPlanRequestRequestTypeDef,
-    DescribeRescoreExecutionPlanRequestRequestTypeDef,
-    DocumentTypeDef,
-    ListRescoreExecutionPlansRequestRequestTypeDef,
-    RescoreExecutionPlanSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    RescoreResultItemTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateRescoreExecutionPlanRequestRequestTypeDef,
-    CreateRescoreExecutionPlanRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateRescoreExecutionPlanResponseTypeDef,
-    DescribeRescoreExecutionPlanResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RescoreRequestRequestTypeDef,
-    ListRescoreExecutionPlansResponseTypeDef,
-    RescoreResultTypeDef,
-)
+from types_aiobotocore_kendra_ranking.type_defs import CapacityUnitsConfigurationTypeDef
 
 
 def get_value() -> CapacityUnitsConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1/setup.py` & `types-aiobotocore-kendra-ranking-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kendra-ranking",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_kendra_ranking"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KendraRanking 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/__main__.py` & `types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.KendraRanking 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kendra-ranking.html#KendraRanking\nOther"
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

### Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/client.py` & `types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/client.pyi` & `types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/literals.py` & `types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/literals.py`

 * *Files 1% similar despite different names*

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
@@ -408,14 +412,15 @@
     "ca-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
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

### Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/literals.pyi` & `types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -39,14 +39,15 @@
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
@@ -142,14 +143,15 @@
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
@@ -228,26 +230,28 @@
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
@@ -406,14 +410,15 @@
     "ca-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
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

### Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/type_defs.py` & `types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking/type_defs.pyi` & `types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking.egg-info/PKG-INFO` & `types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kendra-ranking
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.KendraRanking 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.KendraRanking 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/
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
 [types-aiobotocore-kendra-ranking docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,59 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_kendra_ranking.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `KendraRanking` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/literals/).
+
 ```python
-from types_aiobotocore_kendra_ranking.literals import (
-    RescoreExecutionPlanStatusType,
-    KendraRankingServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_kendra_ranking.literals import RescoreExecutionPlanStatusType
 
 
 def check_value(value: RescoreExecutionPlanStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_kendra_ranking.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `KendraRanking` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kendra_ranking/type_defs/).
+
 ```python
-from types_aiobotocore_kendra_ranking.type_defs import (
-    CapacityUnitsConfigurationTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteRescoreExecutionPlanRequestRequestTypeDef,
-    DescribeRescoreExecutionPlanRequestRequestTypeDef,
-    DocumentTypeDef,
-    ListRescoreExecutionPlansRequestRequestTypeDef,
-    RescoreExecutionPlanSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    RescoreResultItemTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateRescoreExecutionPlanRequestRequestTypeDef,
-    CreateRescoreExecutionPlanRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    CreateRescoreExecutionPlanResponseTypeDef,
-    DescribeRescoreExecutionPlanResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    RescoreRequestRequestTypeDef,
-    ListRescoreExecutionPlansResponseTypeDef,
-    RescoreResultTypeDef,
-)
+from types_aiobotocore_kendra_ranking.type_defs import CapacityUnitsConfigurationTypeDef
 
 
 def get_value() -> CapacityUnitsConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-kendra-ranking-2.5.2.post1/types_aiobotocore_kendra_ranking.egg-info/SOURCES.txt` & `types-aiobotocore-kendra-ranking-2.5.2.post2/types_aiobotocore_kendra_ranking.egg-info/SOURCES.txt`

 * *Files identical despite different names*

