# Comparing `tmp/types-aiobotocore-chime-sdk-identity-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-chime-sdk-identity-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-identity-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-identity-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:31 2023, max compression
```

## Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1.tar` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.633642 types-aiobotocore-chime-sdk-identity-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-08-02 14:51:57.633642 types-aiobotocore-chime-sdk-identity-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.633642 types-aiobotocore-chime-sdk-identity-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.633642 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24651 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24613 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25346 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25317 2023-08-02 14:34:07.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:05.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.633642 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15864 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:31.031328 types-aiobotocore-chime-sdk-identity-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-08-04 12:00:31.031328 types-aiobotocore-chime-sdk-identity-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-08-04 11:41:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:31.031328 types-aiobotocore-chime-sdk-identity-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-08-04 11:41:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:31.031328 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-04 11:41:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 11:41:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-04 11:41:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24651 2023-08-04 11:41:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24613 2023-08-04 11:41:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8338 2023-08-04 11:41:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-08-04 11:41:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25346 2023-08-04 11:41:19.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25317 2023-08-04 11:41:19.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:18.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:31.031328 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 12:00:30.000000 types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1/LICENSE` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1/README.md` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-chime-sdk-identity
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ChimeSDKIdentity 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore chime-sdk-identity type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-chime-sdk-identity"></a>
 
 # types-aiobotocore-chime-sdk-identity
 
 [![PyPI - types-aiobotocore-chime-sdk-identity](https://img.shields.io/pypi/v/types-aiobotocore-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-chime-sdk-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-chime-sdk-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/)
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
 [types-aiobotocore-chime-sdk-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,120 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_chime_sdk_identity.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ChimeSDKIdentity` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/literals/).
+
 ```python
-from types_aiobotocore_chime_sdk_identity.literals import (
-    AllowMessagesType,
-    AppInstanceUserEndpointTypeType,
-    EndpointStatusReasonType,
-    EndpointStatusType,
-    ExpirationCriterionType,
-    RespondsToType,
-    StandardMessagesType,
-    TargetedMessagesType,
-    ChimeSDKIdentityServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_chime_sdk_identity.literals import AllowMessagesType
 
 
 def check_value(value: AllowMessagesType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_chime_sdk_identity.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ChimeSDKIdentity` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity/type_defs/).
+
 ```python
-from types_aiobotocore_chime_sdk_identity.type_defs import (
-    IdentityTypeDef,
-    AppInstanceBotSummaryTypeDef,
-    ChannelRetentionSettingsTypeDef,
-    AppInstanceSummaryTypeDef,
-    AppInstanceTypeDef,
-    EndpointStateTypeDef,
-    EndpointAttributesTypeDef,
-    AppInstanceUserSummaryTypeDef,
-    ExpirationSettingsTypeDef,
-    CreateAppInstanceAdminRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    TagTypeDef,
-    DeleteAppInstanceAdminRequestRequestTypeDef,
-    DeleteAppInstanceBotRequestRequestTypeDef,
-    DeleteAppInstanceRequestRequestTypeDef,
-    DeleteAppInstanceUserRequestRequestTypeDef,
-    DeregisterAppInstanceUserEndpointRequestRequestTypeDef,
-    DescribeAppInstanceAdminRequestRequestTypeDef,
-    DescribeAppInstanceBotRequestRequestTypeDef,
-    DescribeAppInstanceRequestRequestTypeDef,
-    DescribeAppInstanceUserEndpointRequestRequestTypeDef,
-    DescribeAppInstanceUserRequestRequestTypeDef,
-    GetAppInstanceRetentionSettingsRequestRequestTypeDef,
-    InvokedByTypeDef,
-    ListAppInstanceAdminsRequestRequestTypeDef,
-    ListAppInstanceBotsRequestRequestTypeDef,
-    ListAppInstanceUserEndpointsRequestRequestTypeDef,
-    ListAppInstanceUsersRequestRequestTypeDef,
-    ListAppInstancesRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateAppInstanceRequestRequestTypeDef,
-    UpdateAppInstanceUserEndpointRequestRequestTypeDef,
-    UpdateAppInstanceUserRequestRequestTypeDef,
-    AppInstanceAdminSummaryTypeDef,
-    AppInstanceAdminTypeDef,
-    AppInstanceRetentionSettingsTypeDef,
-    AppInstanceUserEndpointSummaryTypeDef,
-    AppInstanceUserEndpointTypeDef,
-    RegisterAppInstanceUserEndpointRequestRequestTypeDef,
-    AppInstanceUserTypeDef,
-    PutAppInstanceUserExpirationSettingsRequestRequestTypeDef,
-    CreateAppInstanceAdminResponseTypeDef,
-    CreateAppInstanceBotResponseTypeDef,
-    CreateAppInstanceResponseTypeDef,
-    CreateAppInstanceUserResponseTypeDef,
-    DescribeAppInstanceResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAppInstanceBotsResponseTypeDef,
-    ListAppInstanceUsersResponseTypeDef,
-    ListAppInstancesResponseTypeDef,
-    PutAppInstanceUserExpirationSettingsResponseTypeDef,
-    RegisterAppInstanceUserEndpointResponseTypeDef,
-    UpdateAppInstanceBotResponseTypeDef,
-    UpdateAppInstanceResponseTypeDef,
-    UpdateAppInstanceUserEndpointResponseTypeDef,
-    UpdateAppInstanceUserResponseTypeDef,
-    CreateAppInstanceRequestRequestTypeDef,
-    CreateAppInstanceUserRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    LexConfigurationTypeDef,
-    ListAppInstanceAdminsResponseTypeDef,
-    DescribeAppInstanceAdminResponseTypeDef,
-    GetAppInstanceRetentionSettingsResponseTypeDef,
-    PutAppInstanceRetentionSettingsRequestRequestTypeDef,
-    PutAppInstanceRetentionSettingsResponseTypeDef,
-    ListAppInstanceUserEndpointsResponseTypeDef,
-    DescribeAppInstanceUserEndpointResponseTypeDef,
-    DescribeAppInstanceUserResponseTypeDef,
-    ConfigurationTypeDef,
-    AppInstanceBotTypeDef,
-    CreateAppInstanceBotRequestRequestTypeDef,
-    UpdateAppInstanceBotRequestRequestTypeDef,
-    DescribeAppInstanceBotResponseTypeDef,
-)
+from types_aiobotocore_chime_sdk_identity.type_defs import IdentityTypeDef
 
 
 def get_value() -> IdentityTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1/setup.py` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-identity",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_chime_sdk_identity"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ChimeSDKIdentity 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/__init__.py` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/__init__.pyi` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/__main__.py` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ChimeSDKIdentity 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_identity//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-identity.html#ChimeSDKIdentity\nOther"
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

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/client.py` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/client.pyi` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/literals.py` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/literals.pyi` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/type_defs.py` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity/type_defs.pyi` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-identity-2.5.2.post1/types_aiobotocore_chime_sdk_identity.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-identity-2.5.2.post2/types_aiobotocore_chime_sdk_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

