# Comparing `tmp/types-aiobotocore-personalize-runtime-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-personalize-runtime-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-personalize-runtime-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-personalize-runtime-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
```

## Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1.tar` & `types-aiobotocore-personalize-runtime-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.681498 types-aiobotocore-personalize-runtime-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:44.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-08-02 14:52:47.681498 types-aiobotocore-personalize-runtime-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11247 2023-08-02 14:44:44.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:47.681498 types-aiobotocore-personalize-runtime-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-02 14:44:43.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.673498 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-02 14:44:44.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-02 14:44:44.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 14:44:44.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5978 2023-08-02 14:44:44.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-08-02 14:44:44.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7609 2023-08-02 14:44:44.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-08-02 14:44:44.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:44.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-08-02 14:44:44.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-08-02 14:44:44.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:44.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.681498 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12812 2023-08-02 14:52:47.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-02 14:52:47.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:47.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:47.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:47.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:47.000000 types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.036643 types-aiobotocore-personalize-runtime-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12890 2023-08-04 13:59:21.036643 types-aiobotocore-personalize-runtime-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11325 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.036643 types-aiobotocore-personalize-runtime-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2131 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.036643 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      533 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      532 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      989 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5978 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5968 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7704 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7702 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3067 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3064 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:36.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.036643 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12890 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      938 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.000000 types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/LICENSE` & `types-aiobotocore-personalize-runtime-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/PKG-INFO` & `types-aiobotocore-personalize-runtime-2.5.2.post2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-personalize-runtime
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.PersonalizeRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.PersonalizeRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_runtime/
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
 [types-aiobotocore-personalize-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,43 +266,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_personalize_runtime.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `PersonalizeRuntime` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_runtime/literals/).
+
 ```python
-from types_aiobotocore_personalize_runtime.literals import (
-    PersonalizeRuntimeServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_personalize_runtime.literals import PersonalizeRuntimeServiceName
 
 
 def check_value(value: PersonalizeRuntimeServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_personalize_runtime.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `PersonalizeRuntime` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_runtime/type_defs/).
+
 ```python
 from types_aiobotocore_personalize_runtime.type_defs import (
     GetPersonalizedRankingRequestRequestTypeDef,
-    PredictedItemTypeDef,
-    ResponseMetadataTypeDef,
-    PromotionTypeDef,
-    GetPersonalizedRankingResponseTypeDef,
-    GetRecommendationsResponseTypeDef,
-    GetRecommendationsRequestRequestTypeDef,
 )
 
 
 def get_value() -> GetPersonalizedRankingRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/README.md` & `types-aiobotocore-personalize-runtime-2.5.2.post2/README.md`

 * *Files 4% similar despite different names*

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
 [types-aiobotocore-personalize-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,43 +234,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_personalize_runtime.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `PersonalizeRuntime` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_runtime/literals/).
+
 ```python
-from types_aiobotocore_personalize_runtime.literals import (
-    PersonalizeRuntimeServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_personalize_runtime.literals import PersonalizeRuntimeServiceName
 
 
 def check_value(value: PersonalizeRuntimeServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_personalize_runtime.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `PersonalizeRuntime` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_runtime/type_defs/).
+
 ```python
 from types_aiobotocore_personalize_runtime.type_defs import (
     GetPersonalizedRankingRequestRequestTypeDef,
-    PredictedItemTypeDef,
-    ResponseMetadataTypeDef,
-    PromotionTypeDef,
-    GetPersonalizedRankingResponseTypeDef,
-    GetRecommendationsResponseTypeDef,
-    GetRecommendationsRequestRequestTypeDef,
 )
 
 
 def get_value() -> GetPersonalizedRankingRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/setup.py` & `types-aiobotocore-personalize-runtime-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-personalize-runtime",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_personalize_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.PersonalizeRuntime 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/__init__.py` & `types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/__init__.pyi` & `types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/__main__.py` & `types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.PersonalizeRuntime 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/personalize-runtime.html#PersonalizeRuntime\nOther"
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

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/client.py` & `types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/client.pyi` & `types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/literals.py` & `types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PersonalizeRuntimeServiceName", "ServiceName", "ResourceServiceName")
 
-
 PersonalizeRuntimeServiceName = Literal["personalize-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -34,14 +32,15 @@
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
@@ -137,14 +136,15 @@
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
@@ -223,26 +223,28 @@
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

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/literals.pyi` & `types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("PersonalizeRuntimeServiceName", "ServiceName", "ResourceServiceName")
 
+
 PersonalizeRuntimeServiceName = Literal["personalize-runtime"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
     "alexaforbusiness",
@@ -32,14 +34,15 @@
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
@@ -135,14 +138,15 @@
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
@@ -221,26 +225,28 @@
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

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/type_defs.py` & `types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime/type_defs.pyi` & `types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime.egg-info/PKG-INFO` & `types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-personalize-runtime
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.PersonalizeRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.PersonalizeRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_runtime/
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
 [types-aiobotocore-personalize-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_runtime/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,43 +266,39 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_personalize_runtime.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `PersonalizeRuntime` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_runtime/literals/).
+
 ```python
-from types_aiobotocore_personalize_runtime.literals import (
-    PersonalizeRuntimeServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_personalize_runtime.literals import PersonalizeRuntimeServiceName
 
 
 def check_value(value: PersonalizeRuntimeServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_personalize_runtime.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `PersonalizeRuntime` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_personalize_runtime/type_defs/).
+
 ```python
 from types_aiobotocore_personalize_runtime.type_defs import (
     GetPersonalizedRankingRequestRequestTypeDef,
-    PredictedItemTypeDef,
-    ResponseMetadataTypeDef,
-    PromotionTypeDef,
-    GetPersonalizedRankingResponseTypeDef,
-    GetRecommendationsResponseTypeDef,
-    GetRecommendationsRequestRequestTypeDef,
 )
 
 
 def get_value() -> GetPersonalizedRankingRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-personalize-runtime-2.5.2.post1/types_aiobotocore_personalize_runtime.egg-info/SOURCES.txt` & `types-aiobotocore-personalize-runtime-2.5.2.post2/types_aiobotocore_personalize_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

