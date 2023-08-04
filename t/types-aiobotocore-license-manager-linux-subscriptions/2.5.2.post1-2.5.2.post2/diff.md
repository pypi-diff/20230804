# Comparing `tmp/types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
```

## Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1.tar` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.717542 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-08-02 14:52:33.717542 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13847 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.717542 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.717542 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9227 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8999 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-08-02 14:42:14.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.717542 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15474 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.316643 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:00.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14828 2023-08-04 13:59:15.316643 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13201 2023-08-04 13:43:00.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.316643 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2268 2023-08-04 13:43:00.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.316643 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1207 2023-08-04 13:43:00.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1206 2023-08-04 13:43:00.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1049 2023-08-04 13:43:00.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9217 2023-08-04 13:43:00.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9202 2023-08-04 13:43:00.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9094 2023-08-04 13:43:01.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9092 2023-08-04 13:43:00.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4010 2023-08-04 13:43:00.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4006 2023-08-04 13:43:00.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:00.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5827 2023-08-04 13:43:01.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5824 2023-08-04 13:43:01.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:00.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.316643 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14828 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1345 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       54 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/LICENSE` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/PKG-INFO` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-license-manager-linux-subscriptions
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.LicenseManagerLinuxSubscriptions 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.LicenseManagerLinuxSubscriptions 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/
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
 [types-aiobotocore-license-manager-linux-subscriptions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,27 +306,20 @@
 
 ### Literals
 
 `types_aiobotocore_license_manager_linux_subscriptions.literals` module
 contains literals extracted from shapes that can be used in user code for type
 checking.
 
+Full list of `LicenseManagerLinuxSubscriptions` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/literals/).
+
 ```python
 from types_aiobotocore_license_manager_linux_subscriptions.literals import (
     LinuxSubscriptionsDiscoveryType,
-    ListLinuxSubscriptionInstancesPaginatorName,
-    ListLinuxSubscriptionsPaginatorName,
-    OperatorType,
-    OrganizationIntegrationType,
-    StatusType,
-    LicenseManagerLinuxSubscriptionsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
 )
 
 
 def check_value(value: LinuxSubscriptionsDiscoveryType) -> bool:
     ...
 ```
 
@@ -334,34 +327,19 @@
 
 ### Type definitions
 
 `types_aiobotocore_license_manager_linux_subscriptions.type_defs` module
 contains structures and shapes assembled to typed dictionaries and unions for
 additional type checking.
 
+Full list of `LicenseManagerLinuxSubscriptions` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/type_defs/).
+
 ```python
-from types_aiobotocore_license_manager_linux_subscriptions.type_defs import (
-    FilterTypeDef,
-    LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
-    ResponseMetadataTypeDef,
-    InstanceTypeDef,
-    LinuxSubscriptionsDiscoverySettingsTypeDef,
-    PaginatorConfigTypeDef,
-    SubscriptionTypeDef,
-    ListLinuxSubscriptionInstancesRequestRequestTypeDef,
-    ListLinuxSubscriptionsRequestRequestTypeDef,
-    GetServiceSettingsResponseTypeDef,
-    UpdateServiceSettingsResponseTypeDef,
-    ListLinuxSubscriptionInstancesResponseTypeDef,
-    LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
-    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
-    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
-    ListLinuxSubscriptionsResponseTypeDef,
-)
+from types_aiobotocore_license_manager_linux_subscriptions.type_defs import FilterTypeDef
 
 
 def get_value() -> FilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/README.md` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/README.md`

 * *Files 6% similar despite different names*

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
 [types-aiobotocore-license-manager-linux-subscriptions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -274,27 +274,20 @@
 
 ### Literals
 
 `types_aiobotocore_license_manager_linux_subscriptions.literals` module
 contains literals extracted from shapes that can be used in user code for type
 checking.
 
+Full list of `LicenseManagerLinuxSubscriptions` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/literals/).
+
 ```python
 from types_aiobotocore_license_manager_linux_subscriptions.literals import (
     LinuxSubscriptionsDiscoveryType,
-    ListLinuxSubscriptionInstancesPaginatorName,
-    ListLinuxSubscriptionsPaginatorName,
-    OperatorType,
-    OrganizationIntegrationType,
-    StatusType,
-    LicenseManagerLinuxSubscriptionsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
 )
 
 
 def check_value(value: LinuxSubscriptionsDiscoveryType) -> bool:
     ...
 ```
 
@@ -302,34 +295,19 @@
 
 ### Type definitions
 
 `types_aiobotocore_license_manager_linux_subscriptions.type_defs` module
 contains structures and shapes assembled to typed dictionaries and unions for
 additional type checking.
 
+Full list of `LicenseManagerLinuxSubscriptions` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/type_defs/).
+
 ```python
-from types_aiobotocore_license_manager_linux_subscriptions.type_defs import (
-    FilterTypeDef,
-    LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
-    ResponseMetadataTypeDef,
-    InstanceTypeDef,
-    LinuxSubscriptionsDiscoverySettingsTypeDef,
-    PaginatorConfigTypeDef,
-    SubscriptionTypeDef,
-    ListLinuxSubscriptionInstancesRequestRequestTypeDef,
-    ListLinuxSubscriptionsRequestRequestTypeDef,
-    GetServiceSettingsResponseTypeDef,
-    UpdateServiceSettingsResponseTypeDef,
-    ListLinuxSubscriptionInstancesResponseTypeDef,
-    LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
-    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
-    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
-    ListLinuxSubscriptionsResponseTypeDef,
-)
+from types_aiobotocore_license_manager_linux_subscriptions.type_defs import FilterTypeDef
 
 
 def get_value() -> FilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/setup.py` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-license-manager-linux-subscriptions",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_license_manager_linux_subscriptions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LicenseManagerLinuxSubscriptions 2.5.2 service generated"
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

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/__init__.py` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/__init__.pyi` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/__main__.py` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.LicenseManagerLinuxSubscriptions 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions\nOther"
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

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/client.py` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from botocore.client import ClientMeta
 
 from .literals import LinuxSubscriptionsDiscoveryType
 from .paginator import ListLinuxSubscriptionInstancesPaginator, ListLinuxSubscriptionsPaginator
 from .type_defs import (
     FilterTypeDef,
     GetServiceSettingsResponseTypeDef,
-    LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
+    LinuxSubscriptionsDiscoverySettingsTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
     UpdateServiceSettingsResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -131,15 +131,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/client/#list_linux_subscriptions)
         """
 
     async def update_service_settings(
         self,
         *,
         LinuxSubscriptionsDiscovery: LinuxSubscriptionsDiscoveryType,
-        LinuxSubscriptionsDiscoverySettings: LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
+        LinuxSubscriptionsDiscoverySettings: LinuxSubscriptionsDiscoverySettingsTypeDef,
         AllowUpdate: bool = ...
     ) -> UpdateServiceSettingsResponseTypeDef:
         """
         Updates the service settings for Linux subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.update_service_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/client/#update_service_settings)
```

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/client.pyi` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from botocore.client import ClientMeta
 
 from .literals import LinuxSubscriptionsDiscoveryType
 from .paginator import ListLinuxSubscriptionInstancesPaginator, ListLinuxSubscriptionsPaginator
 from .type_defs import (
     FilterTypeDef,
     GetServiceSettingsResponseTypeDef,
-    LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
+    LinuxSubscriptionsDiscoverySettingsTypeDef,
     ListLinuxSubscriptionInstancesResponseTypeDef,
     ListLinuxSubscriptionsResponseTypeDef,
     UpdateServiceSettingsResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
@@ -120,15 +120,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.list_linux_subscriptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/client/#list_linux_subscriptions)
         """
     async def update_service_settings(
         self,
         *,
         LinuxSubscriptionsDiscovery: LinuxSubscriptionsDiscoveryType,
-        LinuxSubscriptionsDiscoverySettings: LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
+        LinuxSubscriptionsDiscoverySettings: LinuxSubscriptionsDiscoverySettingsTypeDef,
         AllowUpdate: bool = ...
     ) -> UpdateServiceSettingsResponseTypeDef:
         """
         Updates the service settings for Linux subscriptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager-linux-subscriptions.html#LicenseManagerLinuxSubscriptions.Client.update_service_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/client/#update_service_settings)
```

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/literals.py` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/literals.py`

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

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/literals.pyi` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
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
@@ -153,14 +154,15 @@
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
@@ -239,26 +241,28 @@
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

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/paginator.py` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/paginator.pyi` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/type_defs.py` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_license_manager_linux_subscriptions.type_defs import FilterTypeDef
 
     data: FilterTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     LinuxSubscriptionsDiscoveryType,
     OperatorType,
     OrganizationIntegrationType,
     StatusType,
 )
@@ -25,27 +25,25 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FilterTypeDef",
-    "LinuxSubscriptionsDiscoverySettingsOutputTypeDef",
+    "LinuxSubscriptionsDiscoverySettingsTypeDef",
     "ResponseMetadataTypeDef",
     "InstanceTypeDef",
-    "LinuxSubscriptionsDiscoverySettingsTypeDef",
     "PaginatorConfigTypeDef",
     "SubscriptionTypeDef",
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
     "ListLinuxSubscriptionsRequestRequestTypeDef",
+    "UpdateServiceSettingsRequestRequestTypeDef",
     "GetServiceSettingsResponseTypeDef",
     "UpdateServiceSettingsResponseTypeDef",
     "ListLinuxSubscriptionInstancesResponseTypeDef",
-    "LinuxSubscriptionsDiscoverySettingsUnionTypeDef",
-    "UpdateServiceSettingsRequestRequestTypeDef",
     "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
     "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsResponseTypeDef",
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
@@ -53,16 +51,16 @@
         "Name": str,
         "Operator": OperatorType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-LinuxSubscriptionsDiscoverySettingsOutputTypeDef = TypedDict(
-    "LinuxSubscriptionsDiscoverySettingsOutputTypeDef",
+LinuxSubscriptionsDiscoverySettingsTypeDef = TypedDict(
+    "LinuxSubscriptionsDiscoverySettingsTypeDef",
     {
         "OrganizationIntegration": OrganizationIntegrationType,
         "SourceRegions": List[str],
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
@@ -89,22 +87,14 @@
         "Status": str,
         "SubscriptionName": str,
         "UsageOperation": str,
     },
     total=False,
 )
 
-LinuxSubscriptionsDiscoverySettingsTypeDef = TypedDict(
-    "LinuxSubscriptionsDiscoverySettingsTypeDef",
-    {
-        "OrganizationIntegration": OrganizationIntegrationType,
-        "SourceRegions": Sequence[str],
-    },
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -137,32 +127,55 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateServiceSettingsRequestRequestTypeDef",
+    {
+        "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
+        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
+    },
+)
+_OptionalUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateServiceSettingsRequestRequestTypeDef",
+    {
+        "AllowUpdate": bool,
+    },
+    total=False,
+)
+
+
+class UpdateServiceSettingsRequestRequestTypeDef(
+    _RequiredUpdateServiceSettingsRequestRequestTypeDef,
+    _OptionalUpdateServiceSettingsRequestRequestTypeDef,
+):
+    pass
+
+
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "HomeRegions": List[str],
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
-        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
+        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
         "Status": StatusType,
         "StatusMessage": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceSettingsResponseTypeDef = TypedDict(
     "UpdateServiceSettingsResponseTypeDef",
     {
         "HomeRegions": List[str],
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
-        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
+        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
         "Status": StatusType,
         "StatusMessage": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLinuxSubscriptionInstancesResponseTypeDef = TypedDict(
@@ -170,40 +183,14 @@
     {
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LinuxSubscriptionsDiscoverySettingsUnionTypeDef = Union[
-    LinuxSubscriptionsDiscoverySettingsTypeDef, LinuxSubscriptionsDiscoverySettingsOutputTypeDef
-]
-_RequiredUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateServiceSettingsRequestRequestTypeDef",
-    {
-        "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
-        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
-    },
-)
-_OptionalUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateServiceSettingsRequestRequestTypeDef",
-    {
-        "AllowUpdate": bool,
-    },
-    total=False,
-)
-
-
-class UpdateServiceSettingsRequestRequestTypeDef(
-    _RequiredUpdateServiceSettingsRequestRequestTypeDef,
-    _OptionalUpdateServiceSettingsRequestRequestTypeDef,
-):
-    pass
-
-
 ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef = TypedDict(
     "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
```

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions/type_defs.pyi` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_license_manager_linux_subscriptions.type_defs import FilterTypeDef
 
     data: FilterTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     LinuxSubscriptionsDiscoveryType,
     OperatorType,
     OrganizationIntegrationType,
     StatusType,
 )
@@ -24,27 +24,25 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FilterTypeDef",
-    "LinuxSubscriptionsDiscoverySettingsOutputTypeDef",
+    "LinuxSubscriptionsDiscoverySettingsTypeDef",
     "ResponseMetadataTypeDef",
     "InstanceTypeDef",
-    "LinuxSubscriptionsDiscoverySettingsTypeDef",
     "PaginatorConfigTypeDef",
     "SubscriptionTypeDef",
     "ListLinuxSubscriptionInstancesRequestRequestTypeDef",
     "ListLinuxSubscriptionsRequestRequestTypeDef",
+    "UpdateServiceSettingsRequestRequestTypeDef",
     "GetServiceSettingsResponseTypeDef",
     "UpdateServiceSettingsResponseTypeDef",
     "ListLinuxSubscriptionInstancesResponseTypeDef",
-    "LinuxSubscriptionsDiscoverySettingsUnionTypeDef",
-    "UpdateServiceSettingsRequestRequestTypeDef",
     "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
     "ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef",
     "ListLinuxSubscriptionsResponseTypeDef",
 )
 
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
@@ -52,16 +50,16 @@
         "Name": str,
         "Operator": OperatorType,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-LinuxSubscriptionsDiscoverySettingsOutputTypeDef = TypedDict(
-    "LinuxSubscriptionsDiscoverySettingsOutputTypeDef",
+LinuxSubscriptionsDiscoverySettingsTypeDef = TypedDict(
+    "LinuxSubscriptionsDiscoverySettingsTypeDef",
     {
         "OrganizationIntegration": OrganizationIntegrationType,
         "SourceRegions": List[str],
     },
 )
 
 ResponseMetadataTypeDef = TypedDict(
@@ -88,22 +86,14 @@
         "Status": str,
         "SubscriptionName": str,
         "UsageOperation": str,
     },
     total=False,
 )
 
-LinuxSubscriptionsDiscoverySettingsTypeDef = TypedDict(
-    "LinuxSubscriptionsDiscoverySettingsTypeDef",
-    {
-        "OrganizationIntegration": OrganizationIntegrationType,
-        "SourceRegions": Sequence[str],
-    },
-)
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -136,32 +126,53 @@
         "Filters": Sequence[FilterTypeDef],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+_RequiredUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateServiceSettingsRequestRequestTypeDef",
+    {
+        "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
+        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
+    },
+)
+_OptionalUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateServiceSettingsRequestRequestTypeDef",
+    {
+        "AllowUpdate": bool,
+    },
+    total=False,
+)
+
+class UpdateServiceSettingsRequestRequestTypeDef(
+    _RequiredUpdateServiceSettingsRequestRequestTypeDef,
+    _OptionalUpdateServiceSettingsRequestRequestTypeDef,
+):
+    pass
+
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "HomeRegions": List[str],
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
-        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
+        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
         "Status": StatusType,
         "StatusMessage": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServiceSettingsResponseTypeDef = TypedDict(
     "UpdateServiceSettingsResponseTypeDef",
     {
         "HomeRegions": List[str],
         "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
-        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
+        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
         "Status": StatusType,
         "StatusMessage": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLinuxSubscriptionInstancesResponseTypeDef = TypedDict(
@@ -169,38 +180,14 @@
     {
         "Instances": List[InstanceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LinuxSubscriptionsDiscoverySettingsUnionTypeDef = Union[
-    LinuxSubscriptionsDiscoverySettingsTypeDef, LinuxSubscriptionsDiscoverySettingsOutputTypeDef
-]
-_RequiredUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateServiceSettingsRequestRequestTypeDef",
-    {
-        "LinuxSubscriptionsDiscovery": LinuxSubscriptionsDiscoveryType,
-        "LinuxSubscriptionsDiscoverySettings": LinuxSubscriptionsDiscoverySettingsTypeDef,
-    },
-)
-_OptionalUpdateServiceSettingsRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateServiceSettingsRequestRequestTypeDef",
-    {
-        "AllowUpdate": bool,
-    },
-    total=False,
-)
-
-class UpdateServiceSettingsRequestRequestTypeDef(
-    _RequiredUpdateServiceSettingsRequestRequestTypeDef,
-    _OptionalUpdateServiceSettingsRequestRequestTypeDef,
-):
-    pass
-
 ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef = TypedDict(
     "ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
```

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions.egg-info/PKG-INFO` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-license-manager-linux-subscriptions
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.LicenseManagerLinuxSubscriptions 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.LicenseManagerLinuxSubscriptions 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/
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
 [types-aiobotocore-license-manager-linux-subscriptions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -306,27 +306,20 @@
 
 ### Literals
 
 `types_aiobotocore_license_manager_linux_subscriptions.literals` module
 contains literals extracted from shapes that can be used in user code for type
 checking.
 
+Full list of `LicenseManagerLinuxSubscriptions` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/literals/).
+
 ```python
 from types_aiobotocore_license_manager_linux_subscriptions.literals import (
     LinuxSubscriptionsDiscoveryType,
-    ListLinuxSubscriptionInstancesPaginatorName,
-    ListLinuxSubscriptionsPaginatorName,
-    OperatorType,
-    OrganizationIntegrationType,
-    StatusType,
-    LicenseManagerLinuxSubscriptionsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
 )
 
 
 def check_value(value: LinuxSubscriptionsDiscoveryType) -> bool:
     ...
 ```
 
@@ -334,34 +327,19 @@
 
 ### Type definitions
 
 `types_aiobotocore_license_manager_linux_subscriptions.type_defs` module
 contains structures and shapes assembled to typed dictionaries and unions for
 additional type checking.
 
+Full list of `LicenseManagerLinuxSubscriptions` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager_linux_subscriptions/type_defs/).
+
 ```python
-from types_aiobotocore_license_manager_linux_subscriptions.type_defs import (
-    FilterTypeDef,
-    LinuxSubscriptionsDiscoverySettingsOutputTypeDef,
-    ResponseMetadataTypeDef,
-    InstanceTypeDef,
-    LinuxSubscriptionsDiscoverySettingsTypeDef,
-    PaginatorConfigTypeDef,
-    SubscriptionTypeDef,
-    ListLinuxSubscriptionInstancesRequestRequestTypeDef,
-    ListLinuxSubscriptionsRequestRequestTypeDef,
-    GetServiceSettingsResponseTypeDef,
-    UpdateServiceSettingsResponseTypeDef,
-    ListLinuxSubscriptionInstancesResponseTypeDef,
-    LinuxSubscriptionsDiscoverySettingsUnionTypeDef,
-    UpdateServiceSettingsRequestRequestTypeDef,
-    ListLinuxSubscriptionInstancesRequestListLinuxSubscriptionInstancesPaginateTypeDef,
-    ListLinuxSubscriptionsRequestListLinuxSubscriptionsPaginateTypeDef,
-    ListLinuxSubscriptionsResponseTypeDef,
-)
+from types_aiobotocore_license_manager_linux_subscriptions.type_defs import FilterTypeDef
 
 
 def get_value() -> FilterTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post1/types_aiobotocore_license_manager_linux_subscriptions.egg-info/SOURCES.txt` & `types-aiobotocore-license-manager-linux-subscriptions-2.5.2.post2/types_aiobotocore_license_manager_linux_subscriptions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

