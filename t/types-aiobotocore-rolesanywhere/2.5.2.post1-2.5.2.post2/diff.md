# Comparing `tmp/types-aiobotocore-rolesanywhere-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-rolesanywhere-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-rolesanywhere-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:54 2023, max compression
+gzip compressed data, was "types-aiobotocore-rolesanywhere-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
```

## Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1.tar` & `types-aiobotocore-rolesanywhere-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.181477 types-aiobotocore-rolesanywhere-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-08-02 14:52:54.173477 types-aiobotocore-rolesanywhere-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13728 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:54.181477 types-aiobotocore-rolesanywhere-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.173477 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22225 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-08-02 14:48:00.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15346 2023-08-02 14:48:00.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15327 2023-08-02 14:48:00.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:59.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.173477 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15273 2023-08-02 14:52:53.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:54.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:53.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:54.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:54.000000 types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.826643 types-aiobotocore-rolesanywhere-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13643 2023-08-04 13:59:23.826643 types-aiobotocore-rolesanywhere-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12098 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.826643 types-aiobotocore-rolesanywhere-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2117 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.816643 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1258 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1257 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      973 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22225 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22184 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8892 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8890 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5378 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5372 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15346 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15327 2023-08-04 13:50:58.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:50:57.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.826643 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13643 2023-08-04 13:59:23.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      927 2023-08-04 13:59:23.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       32 2023-08-04 13:59:23.000000 types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/LICENSE` & `types-aiobotocore-rolesanywhere-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/PKG-INFO` & `types-aiobotocore-rolesanywhere-2.5.2.post2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rolesanywhere
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/
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
 [types-aiobotocore-rolesanywhere docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,92 +299,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_rolesanywhere.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IAMRolesAnywhere` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/literals/).
+
 ```python
-from types_aiobotocore_rolesanywhere.literals import (
-    ListCrlsPaginatorName,
-    ListProfilesPaginatorName,
-    ListSubjectsPaginatorName,
-    ListTrustAnchorsPaginatorName,
-    NotificationChannelType,
-    NotificationEventType,
-    TrustAnchorTypeType,
-    IAMRolesAnywhereServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_rolesanywhere.literals import ListCrlsPaginatorName
 
 
 def check_value(value: ListCrlsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_rolesanywhere.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IAMRolesAnywhere` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/type_defs/).
+
 ```python
-from types_aiobotocore_rolesanywhere.type_defs import (
-    BlobTypeDef,
-    TagTypeDef,
-    NotificationSettingTypeDef,
-    CredentialSummaryTypeDef,
-    CrlDetailTypeDef,
-    ResponseMetadataTypeDef,
-    InstancePropertyTypeDef,
-    ProfileDetailTypeDef,
-    PaginatorConfigTypeDef,
-    ListRequestRequestTypeDef,
-    SubjectSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    NotificationSettingDetailTypeDef,
-    NotificationSettingKeyTypeDef,
-    ScalarCrlRequestRequestTypeDef,
-    ScalarProfileRequestRequestTypeDef,
-    ScalarSubjectRequestRequestTypeDef,
-    ScalarTrustAnchorRequestRequestTypeDef,
-    SourceDataTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateProfileRequestRequestTypeDef,
-    UpdateCrlRequestRequestTypeDef,
-    CreateProfileRequestRequestTypeDef,
-    ImportCrlRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    PutNotificationSettingsRequestRequestTypeDef,
-    CrlDetailResponseTypeDef,
-    ListCrlsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SubjectDetailTypeDef,
-    ListProfilesResponseTypeDef,
-    ProfileDetailResponseTypeDef,
-    ListRequestListCrlsPaginateTypeDef,
-    ListRequestListProfilesPaginateTypeDef,
-    ListRequestListSubjectsPaginateTypeDef,
-    ListRequestListTrustAnchorsPaginateTypeDef,
-    ListSubjectsResponseTypeDef,
-    ResetNotificationSettingsRequestRequestTypeDef,
-    SourceTypeDef,
-    SubjectDetailResponseTypeDef,
-    CreateTrustAnchorRequestRequestTypeDef,
-    TrustAnchorDetailTypeDef,
-    UpdateTrustAnchorRequestRequestTypeDef,
-    ListTrustAnchorsResponseTypeDef,
-    PutNotificationSettingsResponseTypeDef,
-    ResetNotificationSettingsResponseTypeDef,
-    TrustAnchorDetailResponseTypeDef,
-)
+from types_aiobotocore_rolesanywhere.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/README.md` & `types-aiobotocore-rolesanywhere-2.5.2.post2/README.md`

 * *Files 25% similar despite different names*

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
 [types-aiobotocore-rolesanywhere docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
 
@@ -267,92 +267,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_rolesanywhere.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IAMRolesAnywhere` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/literals/).
+
 ```python
-from types_aiobotocore_rolesanywhere.literals import (
-    ListCrlsPaginatorName,
-    ListProfilesPaginatorName,
-    ListSubjectsPaginatorName,
-    ListTrustAnchorsPaginatorName,
-    NotificationChannelType,
-    NotificationEventType,
-    TrustAnchorTypeType,
-    IAMRolesAnywhereServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_rolesanywhere.literals import ListCrlsPaginatorName
 
 
 def check_value(value: ListCrlsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_rolesanywhere.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IAMRolesAnywhere` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/type_defs/).
+
 ```python
-from types_aiobotocore_rolesanywhere.type_defs import (
-    BlobTypeDef,
-    TagTypeDef,
-    NotificationSettingTypeDef,
-    CredentialSummaryTypeDef,
-    CrlDetailTypeDef,
-    ResponseMetadataTypeDef,
-    InstancePropertyTypeDef,
-    ProfileDetailTypeDef,
-    PaginatorConfigTypeDef,
-    ListRequestRequestTypeDef,
-    SubjectSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    NotificationSettingDetailTypeDef,
-    NotificationSettingKeyTypeDef,
-    ScalarCrlRequestRequestTypeDef,
-    ScalarProfileRequestRequestTypeDef,
-    ScalarSubjectRequestRequestTypeDef,
-    ScalarTrustAnchorRequestRequestTypeDef,
-    SourceDataTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateProfileRequestRequestTypeDef,
-    UpdateCrlRequestRequestTypeDef,
-    CreateProfileRequestRequestTypeDef,
-    ImportCrlRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    PutNotificationSettingsRequestRequestTypeDef,
-    CrlDetailResponseTypeDef,
-    ListCrlsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SubjectDetailTypeDef,
-    ListProfilesResponseTypeDef,
-    ProfileDetailResponseTypeDef,
-    ListRequestListCrlsPaginateTypeDef,
-    ListRequestListProfilesPaginateTypeDef,
-    ListRequestListSubjectsPaginateTypeDef,
-    ListRequestListTrustAnchorsPaginateTypeDef,
-    ListSubjectsResponseTypeDef,
-    ResetNotificationSettingsRequestRequestTypeDef,
-    SourceTypeDef,
-    SubjectDetailResponseTypeDef,
-    CreateTrustAnchorRequestRequestTypeDef,
-    TrustAnchorDetailTypeDef,
-    UpdateTrustAnchorRequestRequestTypeDef,
-    ListTrustAnchorsResponseTypeDef,
-    PutNotificationSettingsResponseTypeDef,
-    ResetNotificationSettingsResponseTypeDef,
-    TrustAnchorDetailResponseTypeDef,
-)
+from types_aiobotocore_rolesanywhere.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/setup.py` & `types-aiobotocore-rolesanywhere-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-rolesanywhere",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_rolesanywhere"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/__init__.py` & `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/__init__.pyi` & `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/__main__.py` & `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/rolesanywhere.html#IAMRolesAnywhere\nOther"
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

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/client.py` & `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/client.pyi` & `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/literals.py` & `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/literals.py`

 * *Files 1% similar despite different names*

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

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/literals.pyi` & `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/literals.pyi`

 * *Files 1% similar despite different names*

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
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/paginator.py` & `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/paginator.pyi` & `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/type_defs.py` & `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere/type_defs.pyi` & `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO` & `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-rolesanywhere
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IAMRolesAnywhere 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/
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
 [types-aiobotocore-rolesanywhere docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/).
 
 See how it helps to find and fix potential bugs:
 
@@ -299,92 +299,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_rolesanywhere.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `IAMRolesAnywhere` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/literals/).
+
 ```python
-from types_aiobotocore_rolesanywhere.literals import (
-    ListCrlsPaginatorName,
-    ListProfilesPaginatorName,
-    ListSubjectsPaginatorName,
-    ListTrustAnchorsPaginatorName,
-    NotificationChannelType,
-    NotificationEventType,
-    TrustAnchorTypeType,
-    IAMRolesAnywhereServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_rolesanywhere.literals import ListCrlsPaginatorName
 
 
 def check_value(value: ListCrlsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_rolesanywhere.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IAMRolesAnywhere` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_rolesanywhere/type_defs/).
+
 ```python
-from types_aiobotocore_rolesanywhere.type_defs import (
-    BlobTypeDef,
-    TagTypeDef,
-    NotificationSettingTypeDef,
-    CredentialSummaryTypeDef,
-    CrlDetailTypeDef,
-    ResponseMetadataTypeDef,
-    InstancePropertyTypeDef,
-    ProfileDetailTypeDef,
-    PaginatorConfigTypeDef,
-    ListRequestRequestTypeDef,
-    SubjectSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    NotificationSettingDetailTypeDef,
-    NotificationSettingKeyTypeDef,
-    ScalarCrlRequestRequestTypeDef,
-    ScalarProfileRequestRequestTypeDef,
-    ScalarSubjectRequestRequestTypeDef,
-    ScalarTrustAnchorRequestRequestTypeDef,
-    SourceDataTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateProfileRequestRequestTypeDef,
-    UpdateCrlRequestRequestTypeDef,
-    CreateProfileRequestRequestTypeDef,
-    ImportCrlRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    PutNotificationSettingsRequestRequestTypeDef,
-    CrlDetailResponseTypeDef,
-    ListCrlsResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    SubjectDetailTypeDef,
-    ListProfilesResponseTypeDef,
-    ProfileDetailResponseTypeDef,
-    ListRequestListCrlsPaginateTypeDef,
-    ListRequestListProfilesPaginateTypeDef,
-    ListRequestListSubjectsPaginateTypeDef,
-    ListRequestListTrustAnchorsPaginateTypeDef,
-    ListSubjectsResponseTypeDef,
-    ResetNotificationSettingsRequestRequestTypeDef,
-    SourceTypeDef,
-    SubjectDetailResponseTypeDef,
-    CreateTrustAnchorRequestRequestTypeDef,
-    TrustAnchorDetailTypeDef,
-    UpdateTrustAnchorRequestRequestTypeDef,
-    ListTrustAnchorsResponseTypeDef,
-    PutNotificationSettingsResponseTypeDef,
-    ResetNotificationSettingsResponseTypeDef,
-    TrustAnchorDetailResponseTypeDef,
-)
+from types_aiobotocore_rolesanywhere.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-rolesanywhere-2.5.2.post1/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt` & `types-aiobotocore-rolesanywhere-2.5.2.post2/types_aiobotocore_rolesanywhere.egg-info/SOURCES.txt`

 * *Files identical despite different names*

