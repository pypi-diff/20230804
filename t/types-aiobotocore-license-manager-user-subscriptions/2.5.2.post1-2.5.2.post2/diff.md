# Comparing `tmp/types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:34 2023, max compression
+gzip compressed data, was "types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
```

## Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1.tar` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:34.493538 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16537 2023-08-02 14:52:34.493538 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14914 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:34.493538 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:34.493538 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15974 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8761 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6642 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16132 2023-08-02 14:42:17.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16103 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:34.493538 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16537 2023-08-02 14:52:34.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-08-02 14:52:34.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:34.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:34.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:34.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 14:52:34.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.346643 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15090 2023-08-04 13:59:15.346643 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13467 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.346643 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2261 2023-08-04 13:43:02.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.346643 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1580 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1579 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1045 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15988 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15964 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8856 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8854 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6648 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6642 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15847 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15818 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:03.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.346643 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15090 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1326 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       53 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/LICENSE` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/PKG-INFO` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-license-manager-user-subscriptions
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/
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
 [types-aiobotocore-license-manager-user-subscriptions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,25 +311,20 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_license_manager_user_subscriptions.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `LicenseManagerUserSubscriptions` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/literals/).
+
 ```python
 from types_aiobotocore_license_manager_user_subscriptions.literals import (
     ListIdentityProvidersPaginatorName,
-    ListInstancesPaginatorName,
-    ListProductSubscriptionsPaginatorName,
-    ListUserAssociationsPaginatorName,
-    LicenseManagerUserSubscriptionsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
 )
 
 
 def check_value(value: ListIdentityProvidersPaginatorName) -> bool:
     ...
 ```
 
@@ -337,55 +332,20 @@
 
 ### Type definitions
 
 `types_aiobotocore_license_manager_user_subscriptions.type_defs` module
 contains structures and shapes assembled to typed dictionaries and unions for
 additional type checking.
 
+Full list of `LicenseManagerUserSubscriptions` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/type_defs/).
+
 ```python
 from types_aiobotocore_license_manager_user_subscriptions.type_defs import (
     ActiveDirectoryIdentityProviderTypeDef,
-    ResponseMetadataTypeDef,
-    FilterTypeDef,
-    SettingsOutputTypeDef,
-    InstanceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ListIdentityProvidersRequestRequestTypeDef,
-    SettingsTypeDef,
-    UpdateSettingsTypeDef,
-    IdentityProviderTypeDef,
-    ListInstancesRequestRequestTypeDef,
-    ListInstancesResponseTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
-    SettingsUnionTypeDef,
-    AssociateUserRequestRequestTypeDef,
-    DeregisterIdentityProviderRequestRequestTypeDef,
-    DisassociateUserRequestRequestTypeDef,
-    IdentityProviderSummaryTypeDef,
-    InstanceUserSummaryTypeDef,
-    ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
-    ListProductSubscriptionsRequestRequestTypeDef,
-    ListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
-    ListUserAssociationsRequestRequestTypeDef,
-    ProductUserSummaryTypeDef,
-    RegisterIdentityProviderRequestRequestTypeDef,
-    StartProductSubscriptionRequestRequestTypeDef,
-    StopProductSubscriptionRequestRequestTypeDef,
-    UpdateIdentityProviderSettingsRequestRequestTypeDef,
-    DeregisterIdentityProviderResponseTypeDef,
-    ListIdentityProvidersResponseTypeDef,
-    RegisterIdentityProviderResponseTypeDef,
-    UpdateIdentityProviderSettingsResponseTypeDef,
-    AssociateUserResponseTypeDef,
-    DisassociateUserResponseTypeDef,
-    ListUserAssociationsResponseTypeDef,
-    ListProductSubscriptionsResponseTypeDef,
-    StartProductSubscriptionResponseTypeDef,
-    StopProductSubscriptionResponseTypeDef,
 )
 
 
 def get_value() -> ActiveDirectoryIdentityProviderTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/README.md` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-license-manager-user-subscriptions
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore license-manager-user-subscriptions type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-license-manager-user-subscriptions"></a>
 
 # types-aiobotocore-license-manager-user-subscriptions
 
 [![PyPI - types-aiobotocore-license-manager-user-subscriptions](https://img.shields.io/pypi/v/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/)
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
 [types-aiobotocore-license-manager-user-subscriptions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -279,25 +311,20 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_license_manager_user_subscriptions.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `LicenseManagerUserSubscriptions` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/literals/).
+
 ```python
 from types_aiobotocore_license_manager_user_subscriptions.literals import (
     ListIdentityProvidersPaginatorName,
-    ListInstancesPaginatorName,
-    ListProductSubscriptionsPaginatorName,
-    ListUserAssociationsPaginatorName,
-    LicenseManagerUserSubscriptionsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
 )
 
 
 def check_value(value: ListIdentityProvidersPaginatorName) -> bool:
     ...
 ```
 
@@ -305,55 +332,20 @@
 
 ### Type definitions
 
 `types_aiobotocore_license_manager_user_subscriptions.type_defs` module
 contains structures and shapes assembled to typed dictionaries and unions for
 additional type checking.
 
+Full list of `LicenseManagerUserSubscriptions` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/type_defs/).
+
 ```python
 from types_aiobotocore_license_manager_user_subscriptions.type_defs import (
     ActiveDirectoryIdentityProviderTypeDef,
-    ResponseMetadataTypeDef,
-    FilterTypeDef,
-    SettingsOutputTypeDef,
-    InstanceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ListIdentityProvidersRequestRequestTypeDef,
-    SettingsTypeDef,
-    UpdateSettingsTypeDef,
-    IdentityProviderTypeDef,
-    ListInstancesRequestRequestTypeDef,
-    ListInstancesResponseTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
-    SettingsUnionTypeDef,
-    AssociateUserRequestRequestTypeDef,
-    DeregisterIdentityProviderRequestRequestTypeDef,
-    DisassociateUserRequestRequestTypeDef,
-    IdentityProviderSummaryTypeDef,
-    InstanceUserSummaryTypeDef,
-    ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
-    ListProductSubscriptionsRequestRequestTypeDef,
-    ListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
-    ListUserAssociationsRequestRequestTypeDef,
-    ProductUserSummaryTypeDef,
-    RegisterIdentityProviderRequestRequestTypeDef,
-    StartProductSubscriptionRequestRequestTypeDef,
-    StopProductSubscriptionRequestRequestTypeDef,
-    UpdateIdentityProviderSettingsRequestRequestTypeDef,
-    DeregisterIdentityProviderResponseTypeDef,
-    ListIdentityProvidersResponseTypeDef,
-    RegisterIdentityProviderResponseTypeDef,
-    UpdateIdentityProviderSettingsResponseTypeDef,
-    AssociateUserResponseTypeDef,
-    DisassociateUserResponseTypeDef,
-    ListUserAssociationsResponseTypeDef,
-    ListProductSubscriptionsResponseTypeDef,
-    StartProductSubscriptionResponseTypeDef,
-    StopProductSubscriptionResponseTypeDef,
 )
 
 
 def get_value() -> ActiveDirectoryIdentityProviderTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/setup.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-license-manager-user-subscriptions",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_license_manager_user_subscriptions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.5.2 service generated"
-        " with mypy-boto3-builder 7.17.1"
+        " with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/__init__.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/__init__.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/__main__.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions\nOther"
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

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/client.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     FilterTypeDef,
     IdentityProviderTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListInstancesResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     ListUserAssociationsResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
-    SettingsUnionTypeDef,
+    SettingsTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
     UpdateIdentityProviderSettingsResponseTypeDef,
     UpdateSettingsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -212,15 +212,15 @@
         """
 
     async def register_identity_provider(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
-        Settings: SettingsUnionTypeDef = ...
+        Settings: SettingsTypeDef = ...
     ) -> RegisterIdentityProviderResponseTypeDef:
         """
         Registers an identity provider for user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.register_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#register_identity_provider)
         """
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/client.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     FilterTypeDef,
     IdentityProviderTypeDef,
     ListIdentityProvidersResponseTypeDef,
     ListInstancesResponseTypeDef,
     ListProductSubscriptionsResponseTypeDef,
     ListUserAssociationsResponseTypeDef,
     RegisterIdentityProviderResponseTypeDef,
-    SettingsUnionTypeDef,
+    SettingsTypeDef,
     StartProductSubscriptionResponseTypeDef,
     StopProductSubscriptionResponseTypeDef,
     UpdateIdentityProviderSettingsResponseTypeDef,
     UpdateSettingsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
@@ -197,15 +197,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#list_user_associations)
         """
     async def register_identity_provider(
         self,
         *,
         IdentityProvider: IdentityProviderTypeDef,
         Product: str,
-        Settings: SettingsUnionTypeDef = ...
+        Settings: SettingsTypeDef = ...
     ) -> RegisterIdentityProviderResponseTypeDef:
         """
         Registers an identity provider for user-based subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-user-subscriptions.html#LicenseManagerUserSubscriptions.Client.register_identity_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/client/#register_identity_provider)
         """
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/literals.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
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
@@ -151,14 +152,15 @@
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
@@ -237,26 +239,28 @@
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

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/literals.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,15 @@
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
@@ -149,14 +150,15 @@
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
@@ -235,26 +237,28 @@
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

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/paginator.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/paginator.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/type_defs.py` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,38 +8,36 @@
     ```python
     from types_aiobotocore_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderTypeDef
 
     data: ActiveDirectoryIdentityProviderTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ActiveDirectoryIdentityProviderTypeDef",
     "ResponseMetadataTypeDef",
     "FilterTypeDef",
-    "SettingsOutputTypeDef",
+    "SettingsTypeDef",
     "InstanceSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
-    "SettingsTypeDef",
     "UpdateSettingsTypeDef",
     "IdentityProviderTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
     "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListInstancesRequestListInstancesPaginateTypeDef",
-    "SettingsUnionTypeDef",
     "AssociateUserRequestRequestTypeDef",
     "DeregisterIdentityProviderRequestRequestTypeDef",
     "DisassociateUserRequestRequestTypeDef",
     "IdentityProviderSummaryTypeDef",
     "InstanceUserSummaryTypeDef",
     "ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     "ListProductSubscriptionsRequestRequestTypeDef",
@@ -87,16 +85,16 @@
         "Attribute": str,
         "Operation": str,
         "Value": str,
     },
     total=False,
 )
 
-SettingsOutputTypeDef = TypedDict(
-    "SettingsOutputTypeDef",
+SettingsTypeDef = TypedDict(
+    "SettingsTypeDef",
     {
         "SecurityGroupId": str,
         "Subnets": List[str],
     },
 )
 
 _RequiredInstanceSummaryTypeDef = TypedDict(
@@ -136,22 +134,14 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-SettingsTypeDef = TypedDict(
-    "SettingsTypeDef",
-    {
-        "SecurityGroupId": str,
-        "Subnets": Sequence[str],
-    },
-)
-
 _RequiredUpdateSettingsTypeDef = TypedDict(
     "_RequiredUpdateSettingsTypeDef",
     {
         "AddSubnets": Sequence[str],
         "RemoveSubnets": Sequence[str],
     },
 )
@@ -208,15 +198,14 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-SettingsUnionTypeDef = Union[SettingsTypeDef, SettingsOutputTypeDef]
 _RequiredAssociateUserRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
         "Username": str,
     },
@@ -268,15 +257,15 @@
 
 
 _RequiredIdentityProviderSummaryTypeDef = TypedDict(
     "_RequiredIdentityProviderSummaryTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
-        "Settings": SettingsOutputTypeDef,
+        "Settings": SettingsTypeDef,
         "Status": str,
     },
 )
 _OptionalIdentityProviderSummaryTypeDef = TypedDict(
     "_OptionalIdentityProviderSummaryTypeDef",
     {
         "FailureMessage": str,
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions/type_defs.pyi` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -8,37 +8,35 @@
     ```python
     from types_aiobotocore_license_manager_user_subscriptions.type_defs import ActiveDirectoryIdentityProviderTypeDef
 
     data: ActiveDirectoryIdentityProviderTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActiveDirectoryIdentityProviderTypeDef",
     "ResponseMetadataTypeDef",
     "FilterTypeDef",
-    "SettingsOutputTypeDef",
+    "SettingsTypeDef",
     "InstanceSummaryTypeDef",
     "PaginatorConfigTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
-    "SettingsTypeDef",
     "UpdateSettingsTypeDef",
     "IdentityProviderTypeDef",
     "ListInstancesRequestRequestTypeDef",
     "ListInstancesResponseTypeDef",
     "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListInstancesRequestListInstancesPaginateTypeDef",
-    "SettingsUnionTypeDef",
     "AssociateUserRequestRequestTypeDef",
     "DeregisterIdentityProviderRequestRequestTypeDef",
     "DisassociateUserRequestRequestTypeDef",
     "IdentityProviderSummaryTypeDef",
     "InstanceUserSummaryTypeDef",
     "ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef",
     "ListProductSubscriptionsRequestRequestTypeDef",
@@ -86,16 +84,16 @@
         "Attribute": str,
         "Operation": str,
         "Value": str,
     },
     total=False,
 )
 
-SettingsOutputTypeDef = TypedDict(
-    "SettingsOutputTypeDef",
+SettingsTypeDef = TypedDict(
+    "SettingsTypeDef",
     {
         "SecurityGroupId": str,
         "Subnets": List[str],
     },
 )
 
 _RequiredInstanceSummaryTypeDef = TypedDict(
@@ -133,22 +131,14 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-SettingsTypeDef = TypedDict(
-    "SettingsTypeDef",
-    {
-        "SecurityGroupId": str,
-        "Subnets": Sequence[str],
-    },
-)
-
 _RequiredUpdateSettingsTypeDef = TypedDict(
     "_RequiredUpdateSettingsTypeDef",
     {
         "AddSubnets": Sequence[str],
         "RemoveSubnets": Sequence[str],
     },
 )
@@ -203,15 +193,14 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-SettingsUnionTypeDef = Union[SettingsTypeDef, SettingsOutputTypeDef]
 _RequiredAssociateUserRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateUserRequestRequestTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "InstanceId": str,
         "Username": str,
     },
@@ -259,15 +248,15 @@
     pass
 
 _RequiredIdentityProviderSummaryTypeDef = TypedDict(
     "_RequiredIdentityProviderSummaryTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeDef,
         "Product": str,
-        "Settings": SettingsOutputTypeDef,
+        "Settings": SettingsTypeDef,
         "Status": str,
     },
 )
 _OptionalIdentityProviderSummaryTypeDef = TypedDict(
     "_OptionalIdentityProviderSummaryTypeDef",
     {
         "FailureMessage": str,
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/PKG-INFO` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-license-manager-user-subscriptions
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.LicenseManagerUserSubscriptions 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore license-manager-user-subscriptions type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-license-manager-user-subscriptions"></a>
 
 # types-aiobotocore-license-manager-user-subscriptions
 
 [![PyPI - types-aiobotocore-license-manager-user-subscriptions](https://img.shields.io/pypi/v/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-license-manager-user-subscriptions.svg?color=blue)](https://pypi.org/project/types-aiobotocore-license-manager-user-subscriptions)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/)
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
 [types-aiobotocore-license-manager-user-subscriptions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -311,25 +279,20 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_license_manager_user_subscriptions.literals` module contains
 literals extracted from shapes that can be used in user code for type checking.
 
+Full list of `LicenseManagerUserSubscriptions` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/literals/).
+
 ```python
 from types_aiobotocore_license_manager_user_subscriptions.literals import (
     ListIdentityProvidersPaginatorName,
-    ListInstancesPaginatorName,
-    ListProductSubscriptionsPaginatorName,
-    ListUserAssociationsPaginatorName,
-    LicenseManagerUserSubscriptionsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
 )
 
 
 def check_value(value: ListIdentityProvidersPaginatorName) -> bool:
     ...
 ```
 
@@ -337,55 +300,20 @@
 
 ### Type definitions
 
 `types_aiobotocore_license_manager_user_subscriptions.type_defs` module
 contains structures and shapes assembled to typed dictionaries and unions for
 additional type checking.
 
+Full list of `LicenseManagerUserSubscriptions` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_user_subscriptions/type_defs/).
+
 ```python
 from types_aiobotocore_license_manager_user_subscriptions.type_defs import (
     ActiveDirectoryIdentityProviderTypeDef,
-    ResponseMetadataTypeDef,
-    FilterTypeDef,
-    SettingsOutputTypeDef,
-    InstanceSummaryTypeDef,
-    PaginatorConfigTypeDef,
-    ListIdentityProvidersRequestRequestTypeDef,
-    SettingsTypeDef,
-    UpdateSettingsTypeDef,
-    IdentityProviderTypeDef,
-    ListInstancesRequestRequestTypeDef,
-    ListInstancesResponseTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    ListInstancesRequestListInstancesPaginateTypeDef,
-    SettingsUnionTypeDef,
-    AssociateUserRequestRequestTypeDef,
-    DeregisterIdentityProviderRequestRequestTypeDef,
-    DisassociateUserRequestRequestTypeDef,
-    IdentityProviderSummaryTypeDef,
-    InstanceUserSummaryTypeDef,
-    ListProductSubscriptionsRequestListProductSubscriptionsPaginateTypeDef,
-    ListProductSubscriptionsRequestRequestTypeDef,
-    ListUserAssociationsRequestListUserAssociationsPaginateTypeDef,
-    ListUserAssociationsRequestRequestTypeDef,
-    ProductUserSummaryTypeDef,
-    RegisterIdentityProviderRequestRequestTypeDef,
-    StartProductSubscriptionRequestRequestTypeDef,
-    StopProductSubscriptionRequestRequestTypeDef,
-    UpdateIdentityProviderSettingsRequestRequestTypeDef,
-    DeregisterIdentityProviderResponseTypeDef,
-    ListIdentityProvidersResponseTypeDef,
-    RegisterIdentityProviderResponseTypeDef,
-    UpdateIdentityProviderSettingsResponseTypeDef,
-    AssociateUserResponseTypeDef,
-    DisassociateUserResponseTypeDef,
-    ListUserAssociationsResponseTypeDef,
-    ListProductSubscriptionsResponseTypeDef,
-    StartProductSubscriptionResponseTypeDef,
-    StopProductSubscriptionResponseTypeDef,
 )
 
 
 def get_value() -> ActiveDirectoryIdentityProviderTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_user_subscriptions.egg-info/SOURCES.txt` & `types-aiobotocore-license-manager-user-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_user_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

