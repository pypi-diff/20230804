# Comparing `tmp/types-aiobotocore-osis-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-osis-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-osis-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:45 2023, max compression
+gzip compressed data, was "types-aiobotocore-osis-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:20 2023, max compression
```

## Comparing `types-aiobotocore-osis-2.5.2.post1.tar` & `types-aiobotocore-osis-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.665504 types-aiobotocore-osis-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-02 14:52:45.665504 types-aiobotocore-osis-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11927 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:45.665504 types-aiobotocore-osis-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.661504 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-08-02 14:44:31.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-08-02 14:44:31.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-08-02 14:44:31.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-08-02 14:44:31.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-08-02 14:44:31.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-08-02 14:44:31.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:30.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.665504 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-08-02 14:52:45.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-02 14:52:45.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:45.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 14:52:45.000000 types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.356643 types-aiobotocore-osis-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:17.000000 types-aiobotocore-osis-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12198 2023-08-04 13:59:20.356643 types-aiobotocore-osis-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10677 2023-08-04 13:46:17.000000 types-aiobotocore-osis-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:20.356643 types-aiobotocore-osis-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2042 2023-08-04 13:46:17.000000 types-aiobotocore-osis-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.346643 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      493 2023-08-04 13:46:17.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      492 2023-08-04 13:46:17.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      950 2023-08-04 13:46:17.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12421 2023-08-04 13:46:17.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12399 2023-08-04 13:46:17.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8364 2023-08-04 13:46:18.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8362 2023-08-04 13:46:18.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:17.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10487 2023-08-04 13:46:18.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10480 2023-08-04 13:46:18.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:17.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:20.356643 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12198 2023-08-04 13:59:20.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      683 2023-08-04 13:59:20.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:20.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:20.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       23 2023-08-04 13:59:20.000000 types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-osis-2.5.2.post1/LICENSE` & `types-aiobotocore-osis-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-osis-2.5.2.post1/PKG-INFO` & `types-aiobotocore-osis-2.5.2.post2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-osis
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.OpenSearchIngestion 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.OpenSearchIngestion 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/
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
 [types-aiobotocore-osis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,80 +265,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_osis.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `OpenSearchIngestion` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/literals/).
+
 ```python
-from types_aiobotocore_osis.literals import (
-    ChangeProgressStageStatusesType,
-    ChangeProgressStatusesType,
-    PipelineStatusType,
-    OpenSearchIngestionServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_osis.literals import ChangeProgressStageStatusesType
 
 
 def check_value(value: ChangeProgressStageStatusesType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_osis.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `OpenSearchIngestion` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/type_defs/).
+
 ```python
-from types_aiobotocore_osis.type_defs import (
-    ChangeProgressStageTypeDef,
-    CloudWatchLogDestinationTypeDef,
-    TagTypeDef,
-    VpcOptionsTypeDef,
-    ResponseMetadataTypeDef,
-    DeletePipelineRequestRequestTypeDef,
-    GetPipelineBlueprintRequestRequestTypeDef,
-    PipelineBlueprintTypeDef,
-    GetPipelineChangeProgressRequestRequestTypeDef,
-    GetPipelineRequestRequestTypeDef,
-    PipelineBlueprintSummaryTypeDef,
-    ListPipelinesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PipelineStatusReasonTypeDef,
-    StartPipelineRequestRequestTypeDef,
-    StopPipelineRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ValidatePipelineRequestRequestTypeDef,
-    ValidationMessageTypeDef,
-    VpcOptionsOutputTypeDef,
-    ChangeProgressStatusTypeDef,
-    LogPublishingOptionsTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetPipelineBlueprintResponseTypeDef,
-    ListPipelineBlueprintsResponseTypeDef,
-    PipelineSummaryTypeDef,
-    ValidatePipelineResponseTypeDef,
-    VpcEndpointTypeDef,
-    VpcOptionsUnionTypeDef,
-    GetPipelineChangeProgressResponseTypeDef,
-    CreatePipelineRequestRequestTypeDef,
-    UpdatePipelineRequestRequestTypeDef,
-    ListPipelinesResponseTypeDef,
-    PipelineTypeDef,
-    CreatePipelineResponseTypeDef,
-    GetPipelineResponseTypeDef,
-    StartPipelineResponseTypeDef,
-    StopPipelineResponseTypeDef,
-    UpdatePipelineResponseTypeDef,
-)
+from types_aiobotocore_osis.type_defs import ChangeProgressStageTypeDef
 
 
 def get_value() -> ChangeProgressStageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-osis-2.5.2.post1/README.md` & `types-aiobotocore-osis-2.5.2.post2/README.md`

 * *Files 14% similar despite different names*

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
 [types-aiobotocore-osis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -233,80 +233,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_osis.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `OpenSearchIngestion` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/literals/).
+
 ```python
-from types_aiobotocore_osis.literals import (
-    ChangeProgressStageStatusesType,
-    ChangeProgressStatusesType,
-    PipelineStatusType,
-    OpenSearchIngestionServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_osis.literals import ChangeProgressStageStatusesType
 
 
 def check_value(value: ChangeProgressStageStatusesType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_osis.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `OpenSearchIngestion` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/type_defs/).
+
 ```python
-from types_aiobotocore_osis.type_defs import (
-    ChangeProgressStageTypeDef,
-    CloudWatchLogDestinationTypeDef,
-    TagTypeDef,
-    VpcOptionsTypeDef,
-    ResponseMetadataTypeDef,
-    DeletePipelineRequestRequestTypeDef,
-    GetPipelineBlueprintRequestRequestTypeDef,
-    PipelineBlueprintTypeDef,
-    GetPipelineChangeProgressRequestRequestTypeDef,
-    GetPipelineRequestRequestTypeDef,
-    PipelineBlueprintSummaryTypeDef,
-    ListPipelinesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PipelineStatusReasonTypeDef,
-    StartPipelineRequestRequestTypeDef,
-    StopPipelineRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ValidatePipelineRequestRequestTypeDef,
-    ValidationMessageTypeDef,
-    VpcOptionsOutputTypeDef,
-    ChangeProgressStatusTypeDef,
-    LogPublishingOptionsTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetPipelineBlueprintResponseTypeDef,
-    ListPipelineBlueprintsResponseTypeDef,
-    PipelineSummaryTypeDef,
-    ValidatePipelineResponseTypeDef,
-    VpcEndpointTypeDef,
-    VpcOptionsUnionTypeDef,
-    GetPipelineChangeProgressResponseTypeDef,
-    CreatePipelineRequestRequestTypeDef,
-    UpdatePipelineRequestRequestTypeDef,
-    ListPipelinesResponseTypeDef,
-    PipelineTypeDef,
-    CreatePipelineResponseTypeDef,
-    GetPipelineResponseTypeDef,
-    StartPipelineResponseTypeDef,
-    StopPipelineResponseTypeDef,
-    UpdatePipelineResponseTypeDef,
-)
+from types_aiobotocore_osis.type_defs import ChangeProgressStageTypeDef
 
 
 def get_value() -> ChangeProgressStageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-osis-2.5.2.post1/setup.py` & `types-aiobotocore-osis-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-osis",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_osis"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.OpenSearchIngestion 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/__main__.py` & `types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.OpenSearchIngestion 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion\nOther"
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

### Comparing `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/client.py` & `types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ListTagsForResourceResponseTypeDef,
     LogPublishingOptionsTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     TagTypeDef,
     UpdatePipelineResponseTypeDef,
     ValidatePipelineResponseTypeDef,
-    VpcOptionsUnionTypeDef,
+    VpcOptionsTypeDef,
 )
 
 __all__ = ("OpenSearchIngestionClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -96,15 +96,15 @@
         self,
         *,
         PipelineName: str,
         MinUnits: int,
         MaxUnits: int,
         PipelineConfigurationBody: str,
         LogPublishingOptions: LogPublishingOptionsTypeDef = ...,
-        VpcOptions: VpcOptionsUnionTypeDef = ...,
+        VpcOptions: VpcOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates an OpenSearch Ingestion pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/client/#create_pipeline)
```

### Comparing `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/client.pyi` & `types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ListTagsForResourceResponseTypeDef,
     LogPublishingOptionsTypeDef,
     StartPipelineResponseTypeDef,
     StopPipelineResponseTypeDef,
     TagTypeDef,
     UpdatePipelineResponseTypeDef,
     ValidatePipelineResponseTypeDef,
-    VpcOptionsUnionTypeDef,
+    VpcOptionsTypeDef,
 )
 
 __all__ = ("OpenSearchIngestionClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -90,15 +90,15 @@
         self,
         *,
         PipelineName: str,
         MinUnits: int,
         MaxUnits: int,
         PipelineConfigurationBody: str,
         LogPublishingOptions: LogPublishingOptionsTypeDef = ...,
-        VpcOptions: VpcOptionsUnionTypeDef = ...,
+        VpcOptions: VpcOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         Creates an OpenSearch Ingestion pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/osis.html#OpenSearchIngestion.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/client/#create_pipeline)
```

### Comparing `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/literals.py` & `types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
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
@@ -159,14 +160,15 @@
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
@@ -245,26 +247,28 @@
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

### Comparing `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/literals.pyi` & `types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/literals.pyi`

 * *Files 2% similar despite different names*

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
```

### Comparing `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/type_defs.py` & `types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_osis.type_defs import ChangeProgressStageTypeDef
 
     data: ChangeProgressStageTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     ChangeProgressStageStatusesType,
     ChangeProgressStatusesType,
     PipelineStatusType,
 )
 
@@ -43,30 +43,28 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "PipelineStatusReasonTypeDef",
     "StartPipelineRequestRequestTypeDef",
     "StopPipelineRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ValidatePipelineRequestRequestTypeDef",
     "ValidationMessageTypeDef",
-    "VpcOptionsOutputTypeDef",
     "ChangeProgressStatusTypeDef",
     "LogPublishingOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "VpcEndpointTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "GetPipelineBlueprintResponseTypeDef",
     "ListPipelineBlueprintsResponseTypeDef",
     "PipelineSummaryTypeDef",
     "ValidatePipelineResponseTypeDef",
-    "VpcEndpointTypeDef",
-    "VpcOptionsUnionTypeDef",
     "GetPipelineChangeProgressResponseTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
-    "ListPipelinesResponseTypeDef",
     "PipelineTypeDef",
+    "ListPipelinesResponseTypeDef",
     "CreatePipelineResponseTypeDef",
     "GetPipelineResponseTypeDef",
     "StartPipelineResponseTypeDef",
     "StopPipelineResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
 )
 
@@ -228,33 +226,14 @@
     "ValidationMessageTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
 
-_RequiredVpcOptionsOutputTypeDef = TypedDict(
-    "_RequiredVpcOptionsOutputTypeDef",
-    {
-        "SubnetIds": List[str],
-    },
-)
-_OptionalVpcOptionsOutputTypeDef = TypedDict(
-    "_OptionalVpcOptionsOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-    },
-    total=False,
-)
-
-
-class VpcOptionsOutputTypeDef(_RequiredVpcOptionsOutputTypeDef, _OptionalVpcOptionsOutputTypeDef):
-    pass
-
-
 ChangeProgressStatusTypeDef = TypedDict(
     "ChangeProgressStatusTypeDef",
     {
         "StartTime": datetime,
         "Status": ChangeProgressStatusesType,
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
@@ -275,14 +254,24 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+VpcEndpointTypeDef = TypedDict(
+    "VpcEndpointTypeDef",
+    {
+        "VpcEndpointId": str,
+        "VpcId": str,
+        "VpcOptions": VpcOptionsTypeDef,
+    },
+    total=False,
+)
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -323,25 +312,14 @@
     {
         "isValid": bool,
         "Errors": List[ValidationMessageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VpcEndpointTypeDef = TypedDict(
-    "VpcEndpointTypeDef",
-    {
-        "VpcEndpointId": str,
-        "VpcId": str,
-        "VpcOptions": VpcOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-VpcOptionsUnionTypeDef = Union[VpcOptionsTypeDef, VpcOptionsOutputTypeDef]
 GetPipelineChangeProgressResponseTypeDef = TypedDict(
     "GetPipelineChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatuses": List[ChangeProgressStatusTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -392,23 +370,14 @@
 
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
 
-ListPipelinesResponseTypeDef = TypedDict(
-    "ListPipelinesResponseTypeDef",
-    {
-        "NextToken": str,
-        "Pipelines": List[PipelineSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "PipelineName": str,
         "PipelineArn": str,
         "MinUnits": int,
         "MaxUnits": int,
@@ -420,14 +389,23 @@
         "IngestEndpointUrls": List[str],
         "LogPublishingOptions": LogPublishingOptionsTypeDef,
         "VpcEndpoints": List[VpcEndpointTypeDef],
     },
     total=False,
 )
 
+ListPipelinesResponseTypeDef = TypedDict(
+    "ListPipelinesResponseTypeDef",
+    {
+        "NextToken": str,
+        "Pipelines": List[PipelineSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis/type_defs.pyi` & `types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_osis.type_defs import ChangeProgressStageTypeDef
 
     data: ChangeProgressStageTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     ChangeProgressStageStatusesType,
     ChangeProgressStatusesType,
     PipelineStatusType,
 )
 
@@ -42,30 +42,28 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "PipelineStatusReasonTypeDef",
     "StartPipelineRequestRequestTypeDef",
     "StopPipelineRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ValidatePipelineRequestRequestTypeDef",
     "ValidationMessageTypeDef",
-    "VpcOptionsOutputTypeDef",
     "ChangeProgressStatusTypeDef",
     "LogPublishingOptionsTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "VpcEndpointTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "GetPipelineBlueprintResponseTypeDef",
     "ListPipelineBlueprintsResponseTypeDef",
     "PipelineSummaryTypeDef",
     "ValidatePipelineResponseTypeDef",
-    "VpcEndpointTypeDef",
-    "VpcOptionsUnionTypeDef",
     "GetPipelineChangeProgressResponseTypeDef",
     "CreatePipelineRequestRequestTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
-    "ListPipelinesResponseTypeDef",
     "PipelineTypeDef",
+    "ListPipelinesResponseTypeDef",
     "CreatePipelineResponseTypeDef",
     "GetPipelineResponseTypeDef",
     "StartPipelineResponseTypeDef",
     "StopPipelineResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
 )
 
@@ -225,31 +223,14 @@
     "ValidationMessageTypeDef",
     {
         "Message": str,
     },
     total=False,
 )
 
-_RequiredVpcOptionsOutputTypeDef = TypedDict(
-    "_RequiredVpcOptionsOutputTypeDef",
-    {
-        "SubnetIds": List[str],
-    },
-)
-_OptionalVpcOptionsOutputTypeDef = TypedDict(
-    "_OptionalVpcOptionsOutputTypeDef",
-    {
-        "SecurityGroupIds": List[str],
-    },
-    total=False,
-)
-
-class VpcOptionsOutputTypeDef(_RequiredVpcOptionsOutputTypeDef, _OptionalVpcOptionsOutputTypeDef):
-    pass
-
 ChangeProgressStatusTypeDef = TypedDict(
     "ChangeProgressStatusTypeDef",
     {
         "StartTime": datetime,
         "Status": ChangeProgressStatusesType,
         "TotalNumberOfStages": int,
         "ChangeProgressStages": List[ChangeProgressStageTypeDef],
@@ -270,14 +251,24 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+VpcEndpointTypeDef = TypedDict(
+    "VpcEndpointTypeDef",
+    {
+        "VpcEndpointId": str,
+        "VpcId": str,
+        "VpcOptions": VpcOptionsTypeDef,
+    },
+    total=False,
+)
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -318,25 +309,14 @@
     {
         "isValid": bool,
         "Errors": List[ValidationMessageTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-VpcEndpointTypeDef = TypedDict(
-    "VpcEndpointTypeDef",
-    {
-        "VpcEndpointId": str,
-        "VpcId": str,
-        "VpcOptions": VpcOptionsOutputTypeDef,
-    },
-    total=False,
-)
-
-VpcOptionsUnionTypeDef = Union[VpcOptionsTypeDef, VpcOptionsOutputTypeDef]
 GetPipelineChangeProgressResponseTypeDef = TypedDict(
     "GetPipelineChangeProgressResponseTypeDef",
     {
         "ChangeProgressStatuses": List[ChangeProgressStatusTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -383,23 +363,14 @@
 )
 
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
-ListPipelinesResponseTypeDef = TypedDict(
-    "ListPipelinesResponseTypeDef",
-    {
-        "NextToken": str,
-        "Pipelines": List[PipelineSummaryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 PipelineTypeDef = TypedDict(
     "PipelineTypeDef",
     {
         "PipelineName": str,
         "PipelineArn": str,
         "MinUnits": int,
         "MaxUnits": int,
@@ -411,14 +382,23 @@
         "IngestEndpointUrls": List[str],
         "LogPublishingOptions": LogPublishingOptionsTypeDef,
         "VpcEndpoints": List[VpcEndpointTypeDef],
     },
     total=False,
 )
 
+ListPipelinesResponseTypeDef = TypedDict(
+    "ListPipelinesResponseTypeDef",
+    {
+        "NextToken": str,
+        "Pipelines": List[PipelineSummaryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/PKG-INFO` & `types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-osis
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.OpenSearchIngestion 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.OpenSearchIngestion 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/
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
 [types-aiobotocore-osis docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,80 +265,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_osis.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `OpenSearchIngestion` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/literals/).
+
 ```python
-from types_aiobotocore_osis.literals import (
-    ChangeProgressStageStatusesType,
-    ChangeProgressStatusesType,
-    PipelineStatusType,
-    OpenSearchIngestionServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_osis.literals import ChangeProgressStageStatusesType
 
 
 def check_value(value: ChangeProgressStageStatusesType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_osis.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `OpenSearchIngestion` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_osis/type_defs/).
+
 ```python
-from types_aiobotocore_osis.type_defs import (
-    ChangeProgressStageTypeDef,
-    CloudWatchLogDestinationTypeDef,
-    TagTypeDef,
-    VpcOptionsTypeDef,
-    ResponseMetadataTypeDef,
-    DeletePipelineRequestRequestTypeDef,
-    GetPipelineBlueprintRequestRequestTypeDef,
-    PipelineBlueprintTypeDef,
-    GetPipelineChangeProgressRequestRequestTypeDef,
-    GetPipelineRequestRequestTypeDef,
-    PipelineBlueprintSummaryTypeDef,
-    ListPipelinesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PipelineStatusReasonTypeDef,
-    StartPipelineRequestRequestTypeDef,
-    StopPipelineRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ValidatePipelineRequestRequestTypeDef,
-    ValidationMessageTypeDef,
-    VpcOptionsOutputTypeDef,
-    ChangeProgressStatusTypeDef,
-    LogPublishingOptionsTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    GetPipelineBlueprintResponseTypeDef,
-    ListPipelineBlueprintsResponseTypeDef,
-    PipelineSummaryTypeDef,
-    ValidatePipelineResponseTypeDef,
-    VpcEndpointTypeDef,
-    VpcOptionsUnionTypeDef,
-    GetPipelineChangeProgressResponseTypeDef,
-    CreatePipelineRequestRequestTypeDef,
-    UpdatePipelineRequestRequestTypeDef,
-    ListPipelinesResponseTypeDef,
-    PipelineTypeDef,
-    CreatePipelineResponseTypeDef,
-    GetPipelineResponseTypeDef,
-    StartPipelineResponseTypeDef,
-    StopPipelineResponseTypeDef,
-    UpdatePipelineResponseTypeDef,
-)
+from types_aiobotocore_osis.type_defs import ChangeProgressStageTypeDef
 
 
 def get_value() -> ChangeProgressStageTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-osis-2.5.2.post1/types_aiobotocore_osis.egg-info/SOURCES.txt` & `types-aiobotocore-osis-2.5.2.post2/types_aiobotocore_osis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

