# Comparing `tmp/types-aiobotocore-codestar-notifications-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-codestar-notifications-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codestar-notifications-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-codestar-notifications-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:39 2023, max compression
```

## Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1.tar` & `types-aiobotocore-codestar-notifications-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.865619 types-aiobotocore-codestar-notifications-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-08-02 14:52:04.865619 types-aiobotocore-codestar-notifications-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.865619 types-aiobotocore-codestar-notifications-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.861618 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-08-02 14:35:17.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-08-02 14:35:17.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-08-02 14:35:17.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.865619 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15438 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.291642 types-aiobotocore-codestar-notifications-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:33.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14044 2023-08-04 12:00:39.291642 types-aiobotocore-codestar-notifications-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-08-04 11:42:33.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:39.291642 types-aiobotocore-codestar-notifications-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-08-04 11:42:33.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.283641 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-04 11:42:33.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-04 11:42:33.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-04 11:42:33.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15312 2023-08-04 11:42:33.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15287 2023-08-04 11:42:33.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-08-04 11:42:34.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9026 2023-08-04 11:42:33.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-08-04 11:42:33.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-08-04 11:42:33.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:33.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-08-04 11:42:34.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10916 2023-08-04 11:42:34.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:33.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.291642 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14044 2023-08-04 12:00:39.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-04 12:00:39.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:39.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 12:00:39.000000 types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/LICENSE` & `types-aiobotocore-codestar-notifications-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/PKG-INFO` & `types-aiobotocore-codestar-notifications-2.5.2.post2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-notifications
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CodeStarNotifications 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CodeStarNotifications 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/
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
 [types-aiobotocore-codestar-notifications docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,83 +297,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codestar_notifications.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CodeStarNotifications` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/literals/).
+
 ```python
-from types_aiobotocore_codestar_notifications.literals import (
-    DetailTypeType,
-    ListEventTypesFilterNameType,
-    ListEventTypesPaginatorName,
-    ListNotificationRulesFilterNameType,
-    ListNotificationRulesPaginatorName,
-    ListTargetsFilterNameType,
-    ListTargetsPaginatorName,
-    NotificationRuleStatusType,
-    TargetStatusType,
-    CodeStarNotificationsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_codestar_notifications.literals import DetailTypeType
 
 
 def check_value(value: DetailTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codestar_notifications.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `CodeStarNotifications` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/type_defs/).
+
 ```python
-from types_aiobotocore_codestar_notifications.type_defs import (
-    TargetTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteNotificationRuleRequestRequestTypeDef,
-    DeleteTargetRequestRequestTypeDef,
-    DescribeNotificationRuleRequestRequestTypeDef,
-    EventTypeSummaryTypeDef,
-    TargetSummaryTypeDef,
-    ListEventTypesFilterTypeDef,
-    PaginatorConfigTypeDef,
-    ListNotificationRulesFilterTypeDef,
-    NotificationRuleSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListTargetsFilterTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UnsubscribeRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CreateNotificationRuleRequestRequestTypeDef,
-    SubscribeRequestRequestTypeDef,
-    UpdateNotificationRuleRequestRequestTypeDef,
-    CreateNotificationRuleResultTypeDef,
-    DeleteNotificationRuleResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    SubscribeResultTypeDef,
-    TagResourceResultTypeDef,
-    UnsubscribeResultTypeDef,
-    ListEventTypesResultTypeDef,
-    DescribeNotificationRuleResultTypeDef,
-    ListTargetsResultTypeDef,
-    ListEventTypesRequestRequestTypeDef,
-    ListEventTypesRequestListEventTypesPaginateTypeDef,
-    ListNotificationRulesRequestListNotificationRulesPaginateTypeDef,
-    ListNotificationRulesRequestRequestTypeDef,
-    ListNotificationRulesResultTypeDef,
-    ListTargetsRequestListTargetsPaginateTypeDef,
-    ListTargetsRequestRequestTypeDef,
-)
+from types_aiobotocore_codestar_notifications.type_defs import TargetTypeDef
 
 
 def get_value() -> TargetTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/README.md` & `types-aiobotocore-codestar-notifications-2.5.2.post2/README.md`

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
 [types-aiobotocore-codestar-notifications docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,83 +265,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codestar_notifications.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CodeStarNotifications` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/literals/).
+
 ```python
-from types_aiobotocore_codestar_notifications.literals import (
-    DetailTypeType,
-    ListEventTypesFilterNameType,
-    ListEventTypesPaginatorName,
-    ListNotificationRulesFilterNameType,
-    ListNotificationRulesPaginatorName,
-    ListTargetsFilterNameType,
-    ListTargetsPaginatorName,
-    NotificationRuleStatusType,
-    TargetStatusType,
-    CodeStarNotificationsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_codestar_notifications.literals import DetailTypeType
 
 
 def check_value(value: DetailTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codestar_notifications.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `CodeStarNotifications` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/type_defs/).
+
 ```python
-from types_aiobotocore_codestar_notifications.type_defs import (
-    TargetTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteNotificationRuleRequestRequestTypeDef,
-    DeleteTargetRequestRequestTypeDef,
-    DescribeNotificationRuleRequestRequestTypeDef,
-    EventTypeSummaryTypeDef,
-    TargetSummaryTypeDef,
-    ListEventTypesFilterTypeDef,
-    PaginatorConfigTypeDef,
-    ListNotificationRulesFilterTypeDef,
-    NotificationRuleSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListTargetsFilterTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UnsubscribeRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CreateNotificationRuleRequestRequestTypeDef,
-    SubscribeRequestRequestTypeDef,
-    UpdateNotificationRuleRequestRequestTypeDef,
-    CreateNotificationRuleResultTypeDef,
-    DeleteNotificationRuleResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    SubscribeResultTypeDef,
-    TagResourceResultTypeDef,
-    UnsubscribeResultTypeDef,
-    ListEventTypesResultTypeDef,
-    DescribeNotificationRuleResultTypeDef,
-    ListTargetsResultTypeDef,
-    ListEventTypesRequestRequestTypeDef,
-    ListEventTypesRequestListEventTypesPaginateTypeDef,
-    ListNotificationRulesRequestListNotificationRulesPaginateTypeDef,
-    ListNotificationRulesRequestRequestTypeDef,
-    ListNotificationRulesResultTypeDef,
-    ListTargetsRequestListTargetsPaginateTypeDef,
-    ListTargetsRequestRequestTypeDef,
-)
+from types_aiobotocore_codestar_notifications.type_defs import TargetTypeDef
 
 
 def get_value() -> TargetTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/setup.py` & `types-aiobotocore-codestar-notifications-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codestar-notifications",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_codestar_notifications"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeStarNotifications 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/__init__.py` & `types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/__init__.pyi` & `types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/__main__.py` & `types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CodeStarNotifications 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-notifications.html#CodeStarNotifications\nOther"
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

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/client.py` & `types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/client.pyi` & `types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/literals.py` & `types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/literals.pyi` & `types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/paginator.py` & `types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/paginator.pyi` & `types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/type_defs.py` & `types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications/type_defs.pyi` & `types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO` & `types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-notifications
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CodeStarNotifications 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CodeStarNotifications 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/
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
 [types-aiobotocore-codestar-notifications docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/).
 
 See how it helps to find and fix potential bugs:
 
@@ -297,83 +297,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codestar_notifications.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CodeStarNotifications` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/literals/).
+
 ```python
-from types_aiobotocore_codestar_notifications.literals import (
-    DetailTypeType,
-    ListEventTypesFilterNameType,
-    ListEventTypesPaginatorName,
-    ListNotificationRulesFilterNameType,
-    ListNotificationRulesPaginatorName,
-    ListTargetsFilterNameType,
-    ListTargetsPaginatorName,
-    NotificationRuleStatusType,
-    TargetStatusType,
-    CodeStarNotificationsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_codestar_notifications.literals import DetailTypeType
 
 
 def check_value(value: DetailTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codestar_notifications.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `CodeStarNotifications` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_notifications/type_defs/).
+
 ```python
-from types_aiobotocore_codestar_notifications.type_defs import (
-    TargetTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteNotificationRuleRequestRequestTypeDef,
-    DeleteTargetRequestRequestTypeDef,
-    DescribeNotificationRuleRequestRequestTypeDef,
-    EventTypeSummaryTypeDef,
-    TargetSummaryTypeDef,
-    ListEventTypesFilterTypeDef,
-    PaginatorConfigTypeDef,
-    ListNotificationRulesFilterTypeDef,
-    NotificationRuleSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    ListTargetsFilterTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UnsubscribeRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    CreateNotificationRuleRequestRequestTypeDef,
-    SubscribeRequestRequestTypeDef,
-    UpdateNotificationRuleRequestRequestTypeDef,
-    CreateNotificationRuleResultTypeDef,
-    DeleteNotificationRuleResultTypeDef,
-    ListTagsForResourceResultTypeDef,
-    SubscribeResultTypeDef,
-    TagResourceResultTypeDef,
-    UnsubscribeResultTypeDef,
-    ListEventTypesResultTypeDef,
-    DescribeNotificationRuleResultTypeDef,
-    ListTargetsResultTypeDef,
-    ListEventTypesRequestRequestTypeDef,
-    ListEventTypesRequestListEventTypesPaginateTypeDef,
-    ListNotificationRulesRequestListNotificationRulesPaginateTypeDef,
-    ListNotificationRulesRequestRequestTypeDef,
-    ListNotificationRulesResultTypeDef,
-    ListTargetsRequestListTargetsPaginateTypeDef,
-    ListTargetsRequestRequestTypeDef,
-)
+from types_aiobotocore_codestar_notifications.type_defs import TargetTypeDef
 
 
 def get_value() -> TargetTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codestar-notifications-2.5.2.post1/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt` & `types-aiobotocore-codestar-notifications-2.5.2.post2/types_aiobotocore_codestar_notifications.egg-info/SOURCES.txt`

 * *Files identical despite different names*

