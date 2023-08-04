# Comparing `tmp/types-aiobotocore-ecr-public-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ecr-public-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ecr-public-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-ecr-public-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:49 2023, max compression
```

## Comparing `types-aiobotocore-ecr-public-2.5.2.post1.tar` & `types-aiobotocore-ecr-public-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.385594 types-aiobotocore-ecr-public-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-08-02 14:52:14.381594 types-aiobotocore-ecr-public-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14587 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.385594 types-aiobotocore-ecr-public-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.373594 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22126 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22090 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    23744 2023-08-02 14:37:54.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:37:53.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.381594 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16116 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:14.000000 types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:49.960049 types-aiobotocore-ecr-public-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:19.000000 types-aiobotocore-ecr-public-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-08-04 12:00:49.960049 types-aiobotocore-ecr-public-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-08-04 11:45:19.000000 types-aiobotocore-ecr-public-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:49.960049 types-aiobotocore-ecr-public-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-08-04 11:45:19.000000 types-aiobotocore-ecr-public-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:49.960049 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-04 11:45:19.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-04 11:45:19.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-08-04 11:45:19.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22126 2023-08-04 11:45:19.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22090 2023-08-04 11:45:19.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8722 2023-08-04 11:45:20.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-08-04 11:45:20.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-08-04 11:45:19.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-08-04 11:45:19.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:19.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23744 2023-08-04 11:45:20.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23709 2023-08-04 11:45:20.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:19.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:49.960049 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-08-04 12:00:49.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:00:49.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:49.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:49.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:49.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:00:49.000000 types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/LICENSE` & `types-aiobotocore-ecr-public-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/PKG-INFO` & `types-aiobotocore-ecr-public-2.5.2.post2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ecr-public
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/
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
 [types-aiobotocore-ecr-public docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -303,111 +303,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ecr_public.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `ECRPublic` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/literals/).
+
 ```python
-from types_aiobotocore_ecr_public.literals import (
-    DescribeImageTagsPaginatorName,
-    DescribeImagesPaginatorName,
-    DescribeRegistriesPaginatorName,
-    DescribeRepositoriesPaginatorName,
-    ImageFailureCodeType,
-    LayerAvailabilityType,
-    LayerFailureCodeType,
-    RegistryAliasStatusType,
-    ECRPublicServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_ecr_public.literals import DescribeImageTagsPaginatorName
 
 
 def check_value(value: DescribeImageTagsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ecr_public.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ECRPublic` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/type_defs/).
+
 ```python
-from types_aiobotocore_ecr_public.type_defs import (
-    AuthorizationDataTypeDef,
-    BatchCheckLayerAvailabilityRequestRequestTypeDef,
-    LayerFailureTypeDef,
-    LayerTypeDef,
-    ResponseMetadataTypeDef,
-    ImageIdentifierTypeDef,
-    BlobTypeDef,
-    CompleteLayerUploadRequestRequestTypeDef,
-    TagTypeDef,
-    RepositoryCatalogDataTypeDef,
-    RepositoryTypeDef,
-    DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeImageTagsRequestRequestTypeDef,
-    ImageDetailTypeDef,
-    DescribeRegistriesRequestRequestTypeDef,
-    DescribeRepositoriesRequestRequestTypeDef,
-    RegistryCatalogDataTypeDef,
-    GetRepositoryCatalogDataRequestRequestTypeDef,
-    GetRepositoryPolicyRequestRequestTypeDef,
-    ReferencedImageDetailTypeDef,
-    InitiateLayerUploadRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutImageRequestRequestTypeDef,
-    PutRegistryCatalogDataRequestRequestTypeDef,
-    RegistryAliasTypeDef,
-    SetRepositoryPolicyRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    BatchCheckLayerAvailabilityResponseTypeDef,
-    CompleteLayerUploadResponseTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
-    InitiateLayerUploadResponseTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
-    UploadLayerPartResponseTypeDef,
-    BatchDeleteImageRequestRequestTypeDef,
-    DescribeImagesRequestRequestTypeDef,
-    ImageFailureTypeDef,
-    ImageTypeDef,
-    RepositoryCatalogDataInputTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    GetRepositoryCatalogDataResponseTypeDef,
-    PutRepositoryCatalogDataResponseTypeDef,
-    CreateRepositoryResponseTypeDef,
-    DeleteRepositoryResponseTypeDef,
-    DescribeRepositoriesResponseTypeDef,
-    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
-    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
-    DescribeImagesResponseTypeDef,
-    GetRegistryCatalogDataResponseTypeDef,
-    PutRegistryCatalogDataResponseTypeDef,
-    ImageTagDetailTypeDef,
-    RegistryTypeDef,
-    BatchDeleteImageResponseTypeDef,
-    PutImageResponseTypeDef,
-    CreateRepositoryRequestRequestTypeDef,
-    PutRepositoryCatalogDataRequestRequestTypeDef,
-    DescribeImageTagsResponseTypeDef,
-    DescribeRegistriesResponseTypeDef,
-)
+from types_aiobotocore_ecr_public.type_defs import AuthorizationDataTypeDef
 
 
 def get_value() -> AuthorizationDataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/README.md` & `types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-ecr-public
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore ecr-public type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ecr-public"></a>
 
 # types-aiobotocore-ecr-public
 
 [![PyPI - types-aiobotocore-ecr-public](https://img.shields.io/pypi/v/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ecr-public.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ecr-public)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/)
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
 [types-aiobotocore-ecr-public docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/).
 
 See how it helps to find and fix potential bugs:
 
@@ -271,111 +303,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_ecr_public.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `ECRPublic` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/literals/).
+
 ```python
-from types_aiobotocore_ecr_public.literals import (
-    DescribeImageTagsPaginatorName,
-    DescribeImagesPaginatorName,
-    DescribeRegistriesPaginatorName,
-    DescribeRepositoriesPaginatorName,
-    ImageFailureCodeType,
-    LayerAvailabilityType,
-    LayerFailureCodeType,
-    RegistryAliasStatusType,
-    ECRPublicServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_ecr_public.literals import DescribeImageTagsPaginatorName
 
 
 def check_value(value: DescribeImageTagsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_ecr_public.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ECRPublic` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public/type_defs/).
+
 ```python
-from types_aiobotocore_ecr_public.type_defs import (
-    AuthorizationDataTypeDef,
-    BatchCheckLayerAvailabilityRequestRequestTypeDef,
-    LayerFailureTypeDef,
-    LayerTypeDef,
-    ResponseMetadataTypeDef,
-    ImageIdentifierTypeDef,
-    BlobTypeDef,
-    CompleteLayerUploadRequestRequestTypeDef,
-    TagTypeDef,
-    RepositoryCatalogDataTypeDef,
-    RepositoryTypeDef,
-    DeleteRepositoryPolicyRequestRequestTypeDef,
-    DeleteRepositoryRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    DescribeImageTagsRequestRequestTypeDef,
-    ImageDetailTypeDef,
-    DescribeRegistriesRequestRequestTypeDef,
-    DescribeRepositoriesRequestRequestTypeDef,
-    RegistryCatalogDataTypeDef,
-    GetRepositoryCatalogDataRequestRequestTypeDef,
-    GetRepositoryPolicyRequestRequestTypeDef,
-    ReferencedImageDetailTypeDef,
-    InitiateLayerUploadRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    PutImageRequestRequestTypeDef,
-    PutRegistryCatalogDataRequestRequestTypeDef,
-    RegistryAliasTypeDef,
-    SetRepositoryPolicyRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    BatchCheckLayerAvailabilityResponseTypeDef,
-    CompleteLayerUploadResponseTypeDef,
-    DeleteRepositoryPolicyResponseTypeDef,
-    GetAuthorizationTokenResponseTypeDef,
-    GetRepositoryPolicyResponseTypeDef,
-    InitiateLayerUploadResponseTypeDef,
-    SetRepositoryPolicyResponseTypeDef,
-    UploadLayerPartResponseTypeDef,
-    BatchDeleteImageRequestRequestTypeDef,
-    DescribeImagesRequestRequestTypeDef,
-    ImageFailureTypeDef,
-    ImageTypeDef,
-    RepositoryCatalogDataInputTypeDef,
-    UploadLayerPartRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    GetRepositoryCatalogDataResponseTypeDef,
-    PutRepositoryCatalogDataResponseTypeDef,
-    CreateRepositoryResponseTypeDef,
-    DeleteRepositoryResponseTypeDef,
-    DescribeRepositoriesResponseTypeDef,
-    DescribeImageTagsRequestDescribeImageTagsPaginateTypeDef,
-    DescribeImagesRequestDescribeImagesPaginateTypeDef,
-    DescribeRegistriesRequestDescribeRegistriesPaginateTypeDef,
-    DescribeRepositoriesRequestDescribeRepositoriesPaginateTypeDef,
-    DescribeImagesResponseTypeDef,
-    GetRegistryCatalogDataResponseTypeDef,
-    PutRegistryCatalogDataResponseTypeDef,
-    ImageTagDetailTypeDef,
-    RegistryTypeDef,
-    BatchDeleteImageResponseTypeDef,
-    PutImageResponseTypeDef,
-    CreateRepositoryRequestRequestTypeDef,
-    PutRepositoryCatalogDataRequestRequestTypeDef,
-    DescribeImageTagsResponseTypeDef,
-    DescribeRegistriesResponseTypeDef,
-)
+from types_aiobotocore_ecr_public.type_defs import AuthorizationDataTypeDef
 
 
 def get_value() -> AuthorizationDataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/setup.py` & `types-aiobotocore-ecr-public-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ecr-public",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ecr_public"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ECRPublic 2.5.2 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/__init__.py` & `types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/__init__.pyi` & `types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/__main__.py` & `types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ECRPublic 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.ECRPublic 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ecr_public//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ecr-public.html#ECRPublic\nOther"
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

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/client.py` & `types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/client.pyi` & `types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/literals.py` & `types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/literals.pyi` & `types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/paginator.py` & `types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/paginator.pyi` & `types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/type_defs.py` & `types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public/type_defs.pyi` & `types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ecr-public-2.5.2.post1/types_aiobotocore_ecr_public.egg-info/SOURCES.txt` & `types-aiobotocore-ecr-public-2.5.2.post2/types_aiobotocore_ecr_public.egg-info/SOURCES.txt`

 * *Files identical despite different names*

