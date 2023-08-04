# Comparing `tmp/types-aiobotocore-migrationhub-config-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-migrationhub-config-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-migrationhub-config-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:41 2023, max compression
+gzip compressed data, was "types-aiobotocore-migrationhub-config-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
```

## Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1.tar` & `types-aiobotocore-migrationhub-config-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:41.141519 types-aiobotocore-migrationhub-config-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12834 2023-08-02 14:52:41.141519 types-aiobotocore-migrationhub-config-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11269 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:41.141519 types-aiobotocore-migrationhub-config-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:41.141519 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3244 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:42.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:41.141519 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12834 2023-08-02 14:52:40.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-02 14:52:40.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:40.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:40.000000 types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.736643 types-aiobotocore-migrationhub-config-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12791 2023-08-04 13:59:18.736643 types-aiobotocore-migrationhub-config-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11226 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.736643 types-aiobotocore-migrationhub-config-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2131 2023-08-04 13:45:05.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.736643 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      533 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      532 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      989 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6471 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6460 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7716 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7714 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3244 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3239 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:45:06.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.736643 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12791 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      938 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.000000 types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/LICENSE` & `types-aiobotocore-migrationhub-config-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/PKG-INFO` & `types-aiobotocore-migrationhub-config-2.5.2.post2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-migrationhub-config
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MigrationHubConfig 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore migrationhub-config type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-migrationhub-config"></a>
 
 # types-aiobotocore-migrationhub-config
 
 [![PyPI - types-aiobotocore-migrationhub-config](https://img.shields.io/pypi/v/types-aiobotocore-migrationhub-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhub-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhub-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/)
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
 [types-aiobotocore-migrationhub-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,46 +234,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_migrationhub_config.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `MigrationHubConfig` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/literals/).
+
 ```python
-from types_aiobotocore_migrationhub_config.literals import (
-    TargetTypeType,
-    MigrationHubConfigServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_migrationhub_config.literals import TargetTypeType
 
 
 def check_value(value: TargetTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_migrationhub_config.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `MigrationHubConfig` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/type_defs/).
+
 ```python
-from types_aiobotocore_migrationhub_config.type_defs import (
-    TargetTypeDef,
-    ResponseMetadataTypeDef,
-    CreateHomeRegionControlRequestRequestTypeDef,
-    DescribeHomeRegionControlsRequestRequestTypeDef,
-    HomeRegionControlTypeDef,
-    GetHomeRegionResultTypeDef,
-    CreateHomeRegionControlResultTypeDef,
-    DescribeHomeRegionControlsResultTypeDef,
-)
+from types_aiobotocore_migrationhub_config.type_defs import TargetTypeDef
 
 
 def get_value() -> TargetTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/README.md` & `types-aiobotocore-migrationhub-config-2.5.2.post2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-migrationhub-config
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MigrationHubConfig 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore migrationhub-config type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-migrationhub-config"></a>
 
 # types-aiobotocore-migrationhub-config
 
 [![PyPI - types-aiobotocore-migrationhub-config](https://img.shields.io/pypi/v/types-aiobotocore-migrationhub-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhub-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-migrationhub-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-migrationhub-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/)
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
 [types-aiobotocore-migrationhub-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,46 +266,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_migrationhub_config.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `MigrationHubConfig` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/literals/).
+
 ```python
-from types_aiobotocore_migrationhub_config.literals import (
-    TargetTypeType,
-    MigrationHubConfigServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_migrationhub_config.literals import TargetTypeType
 
 
 def check_value(value: TargetTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_migrationhub_config.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `MigrationHubConfig` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/type_defs/).
+
 ```python
-from types_aiobotocore_migrationhub_config.type_defs import (
-    TargetTypeDef,
-    ResponseMetadataTypeDef,
-    CreateHomeRegionControlRequestRequestTypeDef,
-    DescribeHomeRegionControlsRequestRequestTypeDef,
-    HomeRegionControlTypeDef,
-    GetHomeRegionResultTypeDef,
-    CreateHomeRegionControlResultTypeDef,
-    DescribeHomeRegionControlsResultTypeDef,
-)
+from types_aiobotocore_migrationhub_config.type_defs import TargetTypeDef
 
 
 def get_value() -> TargetTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/setup.py` & `types-aiobotocore-migrationhub-config-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-migrationhub-config",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_migrationhub_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MigrationHubConfig 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/__init__.py` & `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/__init__.pyi` & `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/__main__.py` & `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.MigrationHubConfig 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/migrationhub-config.html#MigrationHubConfig\nOther"
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

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/client.py` & `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/client.pyi` & `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/literals.py` & `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,16 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("TargetTypeType", "MigrationHubConfigServiceName", "ServiceName", "ResourceServiceName")
 
-
 TargetTypeType = Literal["ACCOUNT"]
 MigrationHubConfigServiceName = Literal["migrationhub-config"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -35,14 +33,15 @@
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
@@ -138,14 +137,15 @@
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
@@ -224,26 +224,28 @@
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

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/literals.pyi` & `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("TargetTypeType", "MigrationHubConfigServiceName", "ServiceName", "ResourceServiceName")
 
+
 TargetTypeType = Literal["ACCOUNT"]
 MigrationHubConfigServiceName = Literal["migrationhub-config"]
 ServiceName = Literal[
     "accessanalyzer",
     "account",
     "acm",
     "acm-pca",
@@ -33,14 +35,15 @@
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
@@ -136,14 +139,15 @@
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
@@ -222,26 +226,28 @@
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

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/type_defs.py` & `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config/type_defs.pyi` & `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config.egg-info/PKG-INFO` & `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-migrationhub-config
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.MigrationHubConfig 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.MigrationHubConfig 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/
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
 [types-aiobotocore-migrationhub-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,46 +266,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_migrationhub_config.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `MigrationHubConfig` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/literals/).
+
 ```python
-from types_aiobotocore_migrationhub_config.literals import (
-    TargetTypeType,
-    MigrationHubConfigServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_migrationhub_config.literals import TargetTypeType
 
 
 def check_value(value: TargetTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_migrationhub_config.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `MigrationHubConfig` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_migrationhub_config/type_defs/).
+
 ```python
-from types_aiobotocore_migrationhub_config.type_defs import (
-    TargetTypeDef,
-    ResponseMetadataTypeDef,
-    CreateHomeRegionControlRequestRequestTypeDef,
-    DescribeHomeRegionControlsRequestRequestTypeDef,
-    HomeRegionControlTypeDef,
-    GetHomeRegionResultTypeDef,
-    CreateHomeRegionControlResultTypeDef,
-    DescribeHomeRegionControlsResultTypeDef,
-)
+from types_aiobotocore_migrationhub_config.type_defs import TargetTypeDef
 
 
 def get_value() -> TargetTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-migrationhub-config-2.5.2.post1/types_aiobotocore_migrationhub_config.egg-info/SOURCES.txt` & `types-aiobotocore-migrationhub-config-2.5.2.post2/types_aiobotocore_migrationhub_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

