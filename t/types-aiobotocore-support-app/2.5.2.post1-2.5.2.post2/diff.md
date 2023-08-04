# Comparing `tmp/types-aiobotocore-support-app-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-support-app-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-support-app-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:06 2023, max compression
+gzip compressed data, was "types-aiobotocore-support-app-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
```

## Comparing `types-aiobotocore-support-app-2.5.2.post1.tar` & `types-aiobotocore-support-app-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.273441 types-aiobotocore-support-app-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-08-02 14:53:06.273441 types-aiobotocore-support-app-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11496 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:06.273441 types-aiobotocore-support-app-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.273441 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10743 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7155 2023-08-02 14:50:26.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-08-02 14:50:26.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:25.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.273441 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13029 2023-08-02 14:53:06.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:53:06.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:53:06.000000 types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.386643 types-aiobotocore-support-app-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12456 2023-08-04 13:59:28.386643 types-aiobotocore-support-app-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10923 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.386643 types-aiobotocore-support-app-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2099 2023-08-04 13:54:49.000000 types-aiobotocore-support-app-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.376643 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      469 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      468 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      957 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10743 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10725 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7885 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7883 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7155 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7146 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:50.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.386643 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12456 2023-08-04 13:59:28.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      802 2023-08-04 13:59:28.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:28.000000 types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-support-app-2.5.2.post1/LICENSE` & `types-aiobotocore-support-app-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2.post1/PKG-INFO` & `types-aiobotocore-support-app-2.5.2.post2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-support-app
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SupportApp 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore support-app type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-support-app"></a>
 
 # types-aiobotocore-support-app
 
 [![PyPI - types-aiobotocore-support-app](https://img.shields.io/pypi/v/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/)
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
 [types-aiobotocore-support-app docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,54 +234,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_support_app.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SupportApp` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/literals/).
+
 ```python
-from types_aiobotocore_support_app.literals import (
-    AccountTypeType,
-    NotificationSeverityLevelType,
-    SupportAppServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_support_app.literals import AccountTypeType
 
 
 def check_value(value: AccountTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_support_app.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SupportApp` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/type_defs/).
+
 ```python
 from types_aiobotocore_support_app.type_defs import (
     CreateSlackChannelConfigurationRequestRequestTypeDef,
-    DeleteSlackChannelConfigurationRequestRequestTypeDef,
-    DeleteSlackWorkspaceConfigurationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ListSlackChannelConfigurationsRequestRequestTypeDef,
-    SlackChannelConfigurationTypeDef,
-    ListSlackWorkspaceConfigurationsRequestRequestTypeDef,
-    SlackWorkspaceConfigurationTypeDef,
-    PutAccountAliasRequestRequestTypeDef,
-    RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef,
-    UpdateSlackChannelConfigurationRequestRequestTypeDef,
-    GetAccountAliasResultTypeDef,
-    RegisterSlackWorkspaceForOrganizationResultTypeDef,
-    UpdateSlackChannelConfigurationResultTypeDef,
-    ListSlackChannelConfigurationsResultTypeDef,
-    ListSlackWorkspaceConfigurationsResultTypeDef,
 )
 
 
 def get_value() -> CreateSlackChannelConfigurationRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-support-app-2.5.2.post1/README.md` & `types-aiobotocore-support-app-2.5.2.post2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-support-app
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SupportApp 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore support-app type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-support-app"></a>
 
 # types-aiobotocore-support-app
 
 [![PyPI - types-aiobotocore-support-app](https://img.shields.io/pypi/v/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-support-app.svg?color=blue)](https://pypi.org/project/types-aiobotocore-support-app)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/)
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
 [types-aiobotocore-support-app docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,54 +266,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_support_app.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SupportApp` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/literals/).
+
 ```python
-from types_aiobotocore_support_app.literals import (
-    AccountTypeType,
-    NotificationSeverityLevelType,
-    SupportAppServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_support_app.literals import AccountTypeType
 
 
 def check_value(value: AccountTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_support_app.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SupportApp` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/type_defs/).
+
 ```python
 from types_aiobotocore_support_app.type_defs import (
     CreateSlackChannelConfigurationRequestRequestTypeDef,
-    DeleteSlackChannelConfigurationRequestRequestTypeDef,
-    DeleteSlackWorkspaceConfigurationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ListSlackChannelConfigurationsRequestRequestTypeDef,
-    SlackChannelConfigurationTypeDef,
-    ListSlackWorkspaceConfigurationsRequestRequestTypeDef,
-    SlackWorkspaceConfigurationTypeDef,
-    PutAccountAliasRequestRequestTypeDef,
-    RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef,
-    UpdateSlackChannelConfigurationRequestRequestTypeDef,
-    GetAccountAliasResultTypeDef,
-    RegisterSlackWorkspaceForOrganizationResultTypeDef,
-    UpdateSlackChannelConfigurationResultTypeDef,
-    ListSlackChannelConfigurationsResultTypeDef,
-    ListSlackWorkspaceConfigurationsResultTypeDef,
 )
 
 
 def get_value() -> CreateSlackChannelConfigurationRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-support-app-2.5.2.post1/setup.py` & `types-aiobotocore-support-app-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-support-app",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_support_app"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SupportApp 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/__main__.py` & `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SupportApp 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SupportApp 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/support-app.html#SupportApp\nOther"
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

### Comparing `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/client.py` & `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/client.pyi` & `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/literals.py` & `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,25 +14,23 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AccountTypeType",
     "NotificationSeverityLevelType",
     "SupportAppServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AccountTypeType = Literal["management", "member"]
 NotificationSeverityLevelType = Literal["all", "high", "none"]
 SupportAppServiceName = Literal["support-app"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -43,14 +41,15 @@
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
@@ -146,14 +145,15 @@
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
@@ -232,26 +232,28 @@
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

### Comparing `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/literals.pyi` & `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,23 +14,25 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AccountTypeType",
     "NotificationSeverityLevelType",
     "SupportAppServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 AccountTypeType = Literal["management", "member"]
 NotificationSeverityLevelType = Literal["all", "high", "none"]
 SupportAppServiceName = Literal["support-app"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
@@ -41,14 +43,15 @@
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
@@ -144,14 +147,15 @@
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
@@ -230,26 +234,28 @@
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

### Comparing `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/type_defs.py` & `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app/type_defs.pyi` & `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/PKG-INFO` & `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-support-app
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SupportApp 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SupportApp 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/
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
 [types-aiobotocore-support-app docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,54 +266,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_support_app.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `SupportApp` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/literals/).
+
 ```python
-from types_aiobotocore_support_app.literals import (
-    AccountTypeType,
-    NotificationSeverityLevelType,
-    SupportAppServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_support_app.literals import AccountTypeType
 
 
 def check_value(value: AccountTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_support_app.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SupportApp` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_support_app/type_defs/).
+
 ```python
 from types_aiobotocore_support_app.type_defs import (
     CreateSlackChannelConfigurationRequestRequestTypeDef,
-    DeleteSlackChannelConfigurationRequestRequestTypeDef,
-    DeleteSlackWorkspaceConfigurationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ListSlackChannelConfigurationsRequestRequestTypeDef,
-    SlackChannelConfigurationTypeDef,
-    ListSlackWorkspaceConfigurationsRequestRequestTypeDef,
-    SlackWorkspaceConfigurationTypeDef,
-    PutAccountAliasRequestRequestTypeDef,
-    RegisterSlackWorkspaceForOrganizationRequestRequestTypeDef,
-    UpdateSlackChannelConfigurationRequestRequestTypeDef,
-    GetAccountAliasResultTypeDef,
-    RegisterSlackWorkspaceForOrganizationResultTypeDef,
-    UpdateSlackChannelConfigurationResultTypeDef,
-    ListSlackChannelConfigurationsResultTypeDef,
-    ListSlackWorkspaceConfigurationsResultTypeDef,
 )
 
 
 def get_value() -> CreateSlackChannelConfigurationRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-support-app-2.5.2.post1/types_aiobotocore_support_app.egg-info/SOURCES.txt` & `types-aiobotocore-support-app-2.5.2.post2/types_aiobotocore_support_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

