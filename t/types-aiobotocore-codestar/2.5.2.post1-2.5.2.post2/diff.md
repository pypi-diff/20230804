# Comparing `tmp/types-aiobotocore-codestar-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-codestar-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codestar-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-codestar-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:39 2023, max compression
```

## Comparing `types-aiobotocore-codestar-2.5.2.post1.tar` & `types-aiobotocore-codestar-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.873618 types-aiobotocore-codestar-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15213 2023-08-02 14:52:04.873618 types-aiobotocore-codestar-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.873618 types-aiobotocore-codestar-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.873618 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17177 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17956 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:14.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.873618 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15213 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.291642 types-aiobotocore-codestar-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-08-04 12:00:39.287641 types-aiobotocore-codestar-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:39.291642 types-aiobotocore-codestar-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.283641 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17177 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17956 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:31.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.287641 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13429 2023-08-04 12:00:39.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-04 12:00:39.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:39.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 12:00:39.000000 types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codestar-2.5.2.post1/LICENSE` & `types-aiobotocore-codestar-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2.post1/PKG-INFO` & `types-aiobotocore-codestar-2.5.2.post2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CodeStar 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CodeStar 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/
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
 [types-aiobotocore-codestar docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,94 +300,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codestar.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `CodeStar` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/literals/).
+
 ```python
-from types_aiobotocore_codestar.literals import (
-    ListProjectsPaginatorName,
-    ListResourcesPaginatorName,
-    ListTeamMembersPaginatorName,
-    ListUserProfilesPaginatorName,
-    CodeStarServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_codestar.literals import ListProjectsPaginatorName
 
 
 def check_value(value: ListProjectsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codestar.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CodeStar` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/type_defs/).
+
 ```python
-from types_aiobotocore_codestar.type_defs import (
-    AssociateTeamMemberRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CodeCommitCodeDestinationTypeDef,
-    GitHubCodeDestinationTypeDef,
-    S3LocationTypeDef,
-    CreateUserProfileRequestRequestTypeDef,
-    DeleteProjectRequestRequestTypeDef,
-    DeleteUserProfileRequestRequestTypeDef,
-    DescribeProjectRequestRequestTypeDef,
-    ProjectStatusTypeDef,
-    DescribeUserProfileRequestRequestTypeDef,
-    DisassociateTeamMemberRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListProjectsRequestRequestTypeDef,
-    ProjectSummaryTypeDef,
-    ListResourcesRequestRequestTypeDef,
-    ResourceTypeDef,
-    ListTagsForProjectRequestRequestTypeDef,
-    ListTeamMembersRequestRequestTypeDef,
-    TeamMemberTypeDef,
-    ListUserProfilesRequestRequestTypeDef,
-    UserProfileSummaryTypeDef,
-    TagProjectRequestRequestTypeDef,
-    UntagProjectRequestRequestTypeDef,
-    UpdateProjectRequestRequestTypeDef,
-    UpdateTeamMemberRequestRequestTypeDef,
-    UpdateUserProfileRequestRequestTypeDef,
-    AssociateTeamMemberResultTypeDef,
-    CreateProjectResultTypeDef,
-    CreateUserProfileResultTypeDef,
-    DeleteProjectResultTypeDef,
-    DeleteUserProfileResultTypeDef,
-    DescribeUserProfileResultTypeDef,
-    ListTagsForProjectResultTypeDef,
-    TagProjectResultTypeDef,
-    UpdateTeamMemberResultTypeDef,
-    UpdateUserProfileResultTypeDef,
-    CodeDestinationTypeDef,
-    CodeSourceTypeDef,
-    ToolchainSourceTypeDef,
-    DescribeProjectResultTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
-    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
-    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
-    ListProjectsResultTypeDef,
-    ListResourcesResultTypeDef,
-    ListTeamMembersResultTypeDef,
-    ListUserProfilesResultTypeDef,
-    CodeTypeDef,
-    ToolchainTypeDef,
-    CreateProjectRequestRequestTypeDef,
-)
+from types_aiobotocore_codestar.type_defs import AssociateTeamMemberRequestRequestTypeDef
 
 
 def get_value() -> AssociateTeamMemberRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codestar-2.5.2.post1/README.md` & `types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-codestar
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CodeStar 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore codestar type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codestar"></a>
 
 # types-aiobotocore-codestar
 
 [![PyPI - types-aiobotocore-codestar](https://img.shields.io/pypi/v/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/)
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
 [types-aiobotocore-codestar docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/).
 
 See how it helps to find and fix potential bugs:
 
@@ -268,94 +300,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codestar.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `CodeStar` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/literals/).
+
 ```python
-from types_aiobotocore_codestar.literals import (
-    ListProjectsPaginatorName,
-    ListResourcesPaginatorName,
-    ListTeamMembersPaginatorName,
-    ListUserProfilesPaginatorName,
-    CodeStarServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_codestar.literals import ListProjectsPaginatorName
 
 
 def check_value(value: ListProjectsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codestar.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CodeStar` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/type_defs/).
+
 ```python
-from types_aiobotocore_codestar.type_defs import (
-    AssociateTeamMemberRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CodeCommitCodeDestinationTypeDef,
-    GitHubCodeDestinationTypeDef,
-    S3LocationTypeDef,
-    CreateUserProfileRequestRequestTypeDef,
-    DeleteProjectRequestRequestTypeDef,
-    DeleteUserProfileRequestRequestTypeDef,
-    DescribeProjectRequestRequestTypeDef,
-    ProjectStatusTypeDef,
-    DescribeUserProfileRequestRequestTypeDef,
-    DisassociateTeamMemberRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListProjectsRequestRequestTypeDef,
-    ProjectSummaryTypeDef,
-    ListResourcesRequestRequestTypeDef,
-    ResourceTypeDef,
-    ListTagsForProjectRequestRequestTypeDef,
-    ListTeamMembersRequestRequestTypeDef,
-    TeamMemberTypeDef,
-    ListUserProfilesRequestRequestTypeDef,
-    UserProfileSummaryTypeDef,
-    TagProjectRequestRequestTypeDef,
-    UntagProjectRequestRequestTypeDef,
-    UpdateProjectRequestRequestTypeDef,
-    UpdateTeamMemberRequestRequestTypeDef,
-    UpdateUserProfileRequestRequestTypeDef,
-    AssociateTeamMemberResultTypeDef,
-    CreateProjectResultTypeDef,
-    CreateUserProfileResultTypeDef,
-    DeleteProjectResultTypeDef,
-    DeleteUserProfileResultTypeDef,
-    DescribeUserProfileResultTypeDef,
-    ListTagsForProjectResultTypeDef,
-    TagProjectResultTypeDef,
-    UpdateTeamMemberResultTypeDef,
-    UpdateUserProfileResultTypeDef,
-    CodeDestinationTypeDef,
-    CodeSourceTypeDef,
-    ToolchainSourceTypeDef,
-    DescribeProjectResultTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
-    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
-    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
-    ListProjectsResultTypeDef,
-    ListResourcesResultTypeDef,
-    ListTeamMembersResultTypeDef,
-    ListUserProfilesResultTypeDef,
-    CodeTypeDef,
-    ToolchainTypeDef,
-    CreateProjectRequestRequestTypeDef,
-)
+from types_aiobotocore_codestar.type_defs import AssociateTeamMemberRequestRequestTypeDef
 
 
 def get_value() -> AssociateTeamMemberRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codestar-2.5.2.post1/setup.py` & `types-aiobotocore-codestar-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codestar",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_codestar"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeStar 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/__init__.py` & `types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/__init__.pyi` & `types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/__main__.py` & `types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CodeStar 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CodeStar 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar.html#CodeStar\nOther"
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

### Comparing `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/client.py` & `types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/client.pyi` & `types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/literals.py` & `types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/literals.pyi` & `types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/paginator.py` & `types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/paginator.pyi` & `types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/type_defs.py` & `types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar/type_defs.pyi` & `types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/PKG-INFO` & `types-aiobotocore-codestar-2.5.2.post2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-codestar
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CodeStar 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codestar type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codestar"></a>
 
 # types-aiobotocore-codestar
 
 [![PyPI - types-aiobotocore-codestar](https://img.shields.io/pypi/v/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/)
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
 [types-aiobotocore-codestar docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/).
 
 See how it helps to find and fix potential bugs:
 
@@ -300,94 +268,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codestar.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `CodeStar` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/literals/).
+
 ```python
-from types_aiobotocore_codestar.literals import (
-    ListProjectsPaginatorName,
-    ListResourcesPaginatorName,
-    ListTeamMembersPaginatorName,
-    ListUserProfilesPaginatorName,
-    CodeStarServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_codestar.literals import ListProjectsPaginatorName
 
 
 def check_value(value: ListProjectsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codestar.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CodeStar` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar/type_defs/).
+
 ```python
-from types_aiobotocore_codestar.type_defs import (
-    AssociateTeamMemberRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CodeCommitCodeDestinationTypeDef,
-    GitHubCodeDestinationTypeDef,
-    S3LocationTypeDef,
-    CreateUserProfileRequestRequestTypeDef,
-    DeleteProjectRequestRequestTypeDef,
-    DeleteUserProfileRequestRequestTypeDef,
-    DescribeProjectRequestRequestTypeDef,
-    ProjectStatusTypeDef,
-    DescribeUserProfileRequestRequestTypeDef,
-    DisassociateTeamMemberRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListProjectsRequestRequestTypeDef,
-    ProjectSummaryTypeDef,
-    ListResourcesRequestRequestTypeDef,
-    ResourceTypeDef,
-    ListTagsForProjectRequestRequestTypeDef,
-    ListTeamMembersRequestRequestTypeDef,
-    TeamMemberTypeDef,
-    ListUserProfilesRequestRequestTypeDef,
-    UserProfileSummaryTypeDef,
-    TagProjectRequestRequestTypeDef,
-    UntagProjectRequestRequestTypeDef,
-    UpdateProjectRequestRequestTypeDef,
-    UpdateTeamMemberRequestRequestTypeDef,
-    UpdateUserProfileRequestRequestTypeDef,
-    AssociateTeamMemberResultTypeDef,
-    CreateProjectResultTypeDef,
-    CreateUserProfileResultTypeDef,
-    DeleteProjectResultTypeDef,
-    DeleteUserProfileResultTypeDef,
-    DescribeUserProfileResultTypeDef,
-    ListTagsForProjectResultTypeDef,
-    TagProjectResultTypeDef,
-    UpdateTeamMemberResultTypeDef,
-    UpdateUserProfileResultTypeDef,
-    CodeDestinationTypeDef,
-    CodeSourceTypeDef,
-    ToolchainSourceTypeDef,
-    DescribeProjectResultTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListResourcesRequestListResourcesPaginateTypeDef,
-    ListTeamMembersRequestListTeamMembersPaginateTypeDef,
-    ListUserProfilesRequestListUserProfilesPaginateTypeDef,
-    ListProjectsResultTypeDef,
-    ListResourcesResultTypeDef,
-    ListTeamMembersResultTypeDef,
-    ListUserProfilesResultTypeDef,
-    CodeTypeDef,
-    ToolchainTypeDef,
-    CreateProjectRequestRequestTypeDef,
-)
+from types_aiobotocore_codestar.type_defs import AssociateTeamMemberRequestRequestTypeDef
 
 
 def get_value() -> AssociateTeamMemberRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codestar-2.5.2.post1/types_aiobotocore_codestar.egg-info/SOURCES.txt` & `types-aiobotocore-codestar-2.5.2.post2/types_aiobotocore_codestar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

