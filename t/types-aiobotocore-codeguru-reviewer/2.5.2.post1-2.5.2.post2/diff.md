# Comparing `tmp/types-aiobotocore-codeguru-reviewer-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-codeguru-reviewer-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codeguru-reviewer-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-codeguru-reviewer-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:36 2023, max compression
```

## Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1.tar` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.637625 types-aiobotocore-codeguru-reviewer-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16908 2023-08-02 14:52:02.629625 types-aiobotocore-codeguru-reviewer-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15351 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.637625 types-aiobotocore-codeguru-reviewer-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.621625 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20977 2023-08-02 14:35:08.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-02 14:35:07.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.629625 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16908 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:02.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.655540 types-aiobotocore-codeguru-reviewer-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-08-04 12:00:36.655540 types-aiobotocore-codeguru-reviewer-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:36.655540 types-aiobotocore-codeguru-reviewer-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.651540 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16599 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9667 2023-08-04 11:42:24.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9665 2023-08-04 11:42:24.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-08-04 11:42:25.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20977 2023-08-04 11:42:25.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-04 11:42:23.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.655540 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14522 2023-08-04 12:00:36.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-04 12:00:36.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:36.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 12:00:36.000000 types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/LICENSE` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/PKG-INFO` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codeguru-reviewer
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/
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
 [types-aiobotocore-codeguru-reviewer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,110 +322,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codeguru_reviewer.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CodeGuruReviewer` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/literals/).
+
 ```python
-from types_aiobotocore_codeguru_reviewer.literals import (
-    AnalysisTypeType,
-    CodeReviewCompletedWaiterName,
-    ConfigFileStateType,
-    EncryptionOptionType,
-    JobStateType,
-    ListRepositoryAssociationsPaginatorName,
-    ProviderTypeType,
-    ReactionType,
-    RecommendationCategoryType,
-    RepositoryAssociationStateType,
-    RepositoryAssociationSucceededWaiterName,
-    SeverityType,
-    TypeType,
-    VendorNameType,
-    CodeGuruReviewerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_codeguru_reviewer.literals import AnalysisTypeType
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codeguru_reviewer.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CodeGuruReviewer` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/type_defs/).
+
 ```python
-from types_aiobotocore_codeguru_reviewer.type_defs import (
-    KMSKeyDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    BranchDiffSourceCodeTypeTypeDef,
-    CodeArtifactsTypeDef,
-    CodeCommitRepositoryTypeDef,
-    MetricsSummaryTypeDef,
-    MetricsTypeDef,
-    CommitDiffSourceCodeTypeTypeDef,
-    WaiterConfigTypeDef,
-    DescribeCodeReviewRequestRequestTypeDef,
-    DescribeRecommendationFeedbackRequestRequestTypeDef,
-    RecommendationFeedbackTypeDef,
-    DescribeRepositoryAssociationRequestRequestTypeDef,
-    DisassociateRepositoryRequestRequestTypeDef,
-    EventInfoTypeDef,
-    ListCodeReviewsRequestRequestTypeDef,
-    ListRecommendationFeedbackRequestRequestTypeDef,
-    RecommendationFeedbackSummaryTypeDef,
-    ListRecommendationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListRepositoryAssociationsRequestRequestTypeDef,
-    RepositoryAssociationSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutRecommendationFeedbackRequestRequestTypeDef,
-    RuleMetadataTypeDef,
-    RepositoryHeadSourceCodeTypeTypeDef,
-    S3RepositoryTypeDef,
-    ThirdPartySourceRepositoryTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    S3RepositoryDetailsTypeDef,
-    DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
-    DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
-    DescribeRecommendationFeedbackResponseTypeDef,
-    RequestMetadataTypeDef,
-    ListRecommendationFeedbackResponseTypeDef,
-    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
-    ListRepositoryAssociationsResponseTypeDef,
-    RecommendationSummaryTypeDef,
-    RepositoryTypeDef,
-    RepositoryAssociationTypeDef,
-    S3BucketRepositoryTypeDef,
-    ListRecommendationsResponseTypeDef,
-    AssociateRepositoryRequestRequestTypeDef,
-    AssociateRepositoryResponseTypeDef,
-    DescribeRepositoryAssociationResponseTypeDef,
-    DisassociateRepositoryResponseTypeDef,
-    SourceCodeTypeTypeDef,
-    CodeReviewSummaryTypeDef,
-    CodeReviewTypeDef,
-    RepositoryAnalysisTypeDef,
-    ListCodeReviewsResponseTypeDef,
-    CreateCodeReviewResponseTypeDef,
-    DescribeCodeReviewResponseTypeDef,
-    CodeReviewTypeTypeDef,
-    CreateCodeReviewRequestRequestTypeDef,
-)
+from types_aiobotocore_codeguru_reviewer.type_defs import KMSKeyDetailsTypeDef
 
 
 def get_value() -> KMSKeyDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/README.md` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-codeguru-reviewer
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore codeguru-reviewer type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codeguru-reviewer"></a>
 
 # types-aiobotocore-codeguru-reviewer
 
 [![PyPI - types-aiobotocore-codeguru-reviewer](https://img.shields.io/pypi/v/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
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
 [types-aiobotocore-codeguru-reviewer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,110 +322,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codeguru_reviewer.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CodeGuruReviewer` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/literals/).
+
 ```python
-from types_aiobotocore_codeguru_reviewer.literals import (
-    AnalysisTypeType,
-    CodeReviewCompletedWaiterName,
-    ConfigFileStateType,
-    EncryptionOptionType,
-    JobStateType,
-    ListRepositoryAssociationsPaginatorName,
-    ProviderTypeType,
-    ReactionType,
-    RecommendationCategoryType,
-    RepositoryAssociationStateType,
-    RepositoryAssociationSucceededWaiterName,
-    SeverityType,
-    TypeType,
-    VendorNameType,
-    CodeGuruReviewerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_codeguru_reviewer.literals import AnalysisTypeType
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codeguru_reviewer.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CodeGuruReviewer` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/type_defs/).
+
 ```python
-from types_aiobotocore_codeguru_reviewer.type_defs import (
-    KMSKeyDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    BranchDiffSourceCodeTypeTypeDef,
-    CodeArtifactsTypeDef,
-    CodeCommitRepositoryTypeDef,
-    MetricsSummaryTypeDef,
-    MetricsTypeDef,
-    CommitDiffSourceCodeTypeTypeDef,
-    WaiterConfigTypeDef,
-    DescribeCodeReviewRequestRequestTypeDef,
-    DescribeRecommendationFeedbackRequestRequestTypeDef,
-    RecommendationFeedbackTypeDef,
-    DescribeRepositoryAssociationRequestRequestTypeDef,
-    DisassociateRepositoryRequestRequestTypeDef,
-    EventInfoTypeDef,
-    ListCodeReviewsRequestRequestTypeDef,
-    ListRecommendationFeedbackRequestRequestTypeDef,
-    RecommendationFeedbackSummaryTypeDef,
-    ListRecommendationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListRepositoryAssociationsRequestRequestTypeDef,
-    RepositoryAssociationSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutRecommendationFeedbackRequestRequestTypeDef,
-    RuleMetadataTypeDef,
-    RepositoryHeadSourceCodeTypeTypeDef,
-    S3RepositoryTypeDef,
-    ThirdPartySourceRepositoryTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    S3RepositoryDetailsTypeDef,
-    DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
-    DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
-    DescribeRecommendationFeedbackResponseTypeDef,
-    RequestMetadataTypeDef,
-    ListRecommendationFeedbackResponseTypeDef,
-    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
-    ListRepositoryAssociationsResponseTypeDef,
-    RecommendationSummaryTypeDef,
-    RepositoryTypeDef,
-    RepositoryAssociationTypeDef,
-    S3BucketRepositoryTypeDef,
-    ListRecommendationsResponseTypeDef,
-    AssociateRepositoryRequestRequestTypeDef,
-    AssociateRepositoryResponseTypeDef,
-    DescribeRepositoryAssociationResponseTypeDef,
-    DisassociateRepositoryResponseTypeDef,
-    SourceCodeTypeTypeDef,
-    CodeReviewSummaryTypeDef,
-    CodeReviewTypeDef,
-    RepositoryAnalysisTypeDef,
-    ListCodeReviewsResponseTypeDef,
-    CreateCodeReviewResponseTypeDef,
-    DescribeCodeReviewResponseTypeDef,
-    CodeReviewTypeTypeDef,
-    CreateCodeReviewRequestRequestTypeDef,
-)
+from types_aiobotocore_codeguru_reviewer.type_defs import KMSKeyDetailsTypeDef
 
 
 def get_value() -> KMSKeyDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/setup.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codeguru-reviewer",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_codeguru_reviewer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/__init__.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/__init__.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/__main__.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CodeGuruReviewer 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codeguru-reviewer.html#CodeGuruReviewer\nOther"
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

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/client.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/client.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/literals.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/literals.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/paginator.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/paginator.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/type_defs.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/type_defs.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/waiter.py` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer/waiter.pyi` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/PKG-INFO` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-codeguru-reviewer
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CodeGuruReviewer 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codeguru-reviewer type-annotations botocore mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-codeguru-reviewer"></a>
 
 # types-aiobotocore-codeguru-reviewer
 
 [![PyPI - types-aiobotocore-codeguru-reviewer](https://img.shields.io/pypi/v/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codeguru-reviewer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codeguru-reviewer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/)
@@ -47,15 +15,15 @@
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
 [types-aiobotocore-codeguru-reviewer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/).
 
 See how it helps to find and fix potential bugs:
 
@@ -322,110 +290,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codeguru_reviewer.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CodeGuruReviewer` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/literals/).
+
 ```python
-from types_aiobotocore_codeguru_reviewer.literals import (
-    AnalysisTypeType,
-    CodeReviewCompletedWaiterName,
-    ConfigFileStateType,
-    EncryptionOptionType,
-    JobStateType,
-    ListRepositoryAssociationsPaginatorName,
-    ProviderTypeType,
-    ReactionType,
-    RecommendationCategoryType,
-    RepositoryAssociationStateType,
-    RepositoryAssociationSucceededWaiterName,
-    SeverityType,
-    TypeType,
-    VendorNameType,
-    CodeGuruReviewerServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    WaiterName,
-    RegionName,
-)
+from types_aiobotocore_codeguru_reviewer.literals import AnalysisTypeType
 
 
 def check_value(value: AnalysisTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codeguru_reviewer.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CodeGuruReviewer` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codeguru_reviewer/type_defs/).
+
 ```python
-from types_aiobotocore_codeguru_reviewer.type_defs import (
-    KMSKeyDetailsTypeDef,
-    ResponseMetadataTypeDef,
-    BranchDiffSourceCodeTypeTypeDef,
-    CodeArtifactsTypeDef,
-    CodeCommitRepositoryTypeDef,
-    MetricsSummaryTypeDef,
-    MetricsTypeDef,
-    CommitDiffSourceCodeTypeTypeDef,
-    WaiterConfigTypeDef,
-    DescribeCodeReviewRequestRequestTypeDef,
-    DescribeRecommendationFeedbackRequestRequestTypeDef,
-    RecommendationFeedbackTypeDef,
-    DescribeRepositoryAssociationRequestRequestTypeDef,
-    DisassociateRepositoryRequestRequestTypeDef,
-    EventInfoTypeDef,
-    ListCodeReviewsRequestRequestTypeDef,
-    ListRecommendationFeedbackRequestRequestTypeDef,
-    RecommendationFeedbackSummaryTypeDef,
-    ListRecommendationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListRepositoryAssociationsRequestRequestTypeDef,
-    RepositoryAssociationSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutRecommendationFeedbackRequestRequestTypeDef,
-    RuleMetadataTypeDef,
-    RepositoryHeadSourceCodeTypeTypeDef,
-    S3RepositoryTypeDef,
-    ThirdPartySourceRepositoryTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    S3RepositoryDetailsTypeDef,
-    DescribeCodeReviewRequestCodeReviewCompletedWaitTypeDef,
-    DescribeRepositoryAssociationRequestRepositoryAssociationSucceededWaitTypeDef,
-    DescribeRecommendationFeedbackResponseTypeDef,
-    RequestMetadataTypeDef,
-    ListRecommendationFeedbackResponseTypeDef,
-    ListRepositoryAssociationsRequestListRepositoryAssociationsPaginateTypeDef,
-    ListRepositoryAssociationsResponseTypeDef,
-    RecommendationSummaryTypeDef,
-    RepositoryTypeDef,
-    RepositoryAssociationTypeDef,
-    S3BucketRepositoryTypeDef,
-    ListRecommendationsResponseTypeDef,
-    AssociateRepositoryRequestRequestTypeDef,
-    AssociateRepositoryResponseTypeDef,
-    DescribeRepositoryAssociationResponseTypeDef,
-    DisassociateRepositoryResponseTypeDef,
-    SourceCodeTypeTypeDef,
-    CodeReviewSummaryTypeDef,
-    CodeReviewTypeDef,
-    RepositoryAnalysisTypeDef,
-    ListCodeReviewsResponseTypeDef,
-    CreateCodeReviewResponseTypeDef,
-    DescribeCodeReviewResponseTypeDef,
-    CodeReviewTypeTypeDef,
-    CreateCodeReviewRequestRequestTypeDef,
-)
+from types_aiobotocore_codeguru_reviewer.type_defs import KMSKeyDetailsTypeDef
 
 
 def get_value() -> KMSKeyDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codeguru-reviewer-2.5.2.post1/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt` & `types-aiobotocore-codeguru-reviewer-2.5.2.post2/types_aiobotocore_codeguru_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

