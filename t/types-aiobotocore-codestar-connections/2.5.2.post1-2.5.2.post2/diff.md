# Comparing `tmp/types-aiobotocore-codestar-connections-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-codestar-connections-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-codestar-connections-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-codestar-connections-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:39 2023, max compression
```

## Comparing `types-aiobotocore-codestar-connections-2.5.2.post1.tar` & `types-aiobotocore-codestar-connections-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.745619 types-aiobotocore-codestar-connections-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-08-02 14:52:04.745619 types-aiobotocore-codestar-connections-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11923 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.745619 types-aiobotocore-codestar-connections-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.733619 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11763 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-08-02 14:35:16.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:15.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.745619 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 14:52:04.000000 types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.155636 types-aiobotocore-codestar-connections-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-08-04 12:00:39.151636 types-aiobotocore-codestar-connections-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11295 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:39.155636 types-aiobotocore-codestar-connections-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.151636 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11748 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11728 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8152 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:32.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.151636 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-08-04 12:00:38.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:00:38.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:38.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:38.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:38.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-04 12:00:38.000000 types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/LICENSE` & `types-aiobotocore-codestar-connections-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/PKG-INFO` & `types-aiobotocore-codestar-connections-2.5.2.post2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-codestar-connections
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CodeStarconnections 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore codestar-connections type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codestar-connections"></a>
 
 # types-aiobotocore-codestar-connections
 
 [![PyPI - types-aiobotocore-codestar-connections](https://img.shields.io/pypi/v/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/)
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
 [types-aiobotocore-codestar-connections docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,66 +234,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codestar_connections.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CodeStarconnections` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/literals/).
+
 ```python
-from types_aiobotocore_codestar_connections.literals import (
-    ConnectionStatusType,
-    ProviderTypeType,
-    CodeStarconnectionsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_codestar_connections.literals import ConnectionStatusType
 
 
 def check_value(value: ConnectionStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codestar_connections.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `CodeStarconnections` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/type_defs/).
+
 ```python
-from types_aiobotocore_codestar_connections.type_defs import (
-    ConnectionTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    VpcConfigurationTypeDef,
-    DeleteConnectionInputRequestTypeDef,
-    DeleteHostInputRequestTypeDef,
-    GetConnectionInputRequestTypeDef,
-    GetHostInputRequestTypeDef,
-    VpcConfigurationOutputTypeDef,
-    ListConnectionsInputRequestTypeDef,
-    ListHostsInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CreateConnectionInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateConnectionOutputTypeDef,
-    CreateHostOutputTypeDef,
-    GetConnectionOutputTypeDef,
-    ListConnectionsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    CreateHostInputRequestTypeDef,
-    UpdateHostInputRequestTypeDef,
-    GetHostOutputTypeDef,
-    HostTypeDef,
-    VpcConfigurationUnionTypeDef,
-    ListHostsOutputTypeDef,
-)
+from types_aiobotocore_codestar_connections.type_defs import ConnectionTypeDef
 
 
 def get_value() -> ConnectionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/README.md` & `types-aiobotocore-codestar-connections-2.5.2.post2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-codestar-connections
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CodeStarconnections 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore codestar-connections type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-codestar-connections"></a>
 
 # types-aiobotocore-codestar-connections
 
 [![PyPI - types-aiobotocore-codestar-connections](https://img.shields.io/pypi/v/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-codestar-connections.svg?color=blue)](https://pypi.org/project/types-aiobotocore-codestar-connections)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/)
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
 [types-aiobotocore-codestar-connections docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,66 +266,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codestar_connections.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CodeStarconnections` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/literals/).
+
 ```python
-from types_aiobotocore_codestar_connections.literals import (
-    ConnectionStatusType,
-    ProviderTypeType,
-    CodeStarconnectionsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_codestar_connections.literals import ConnectionStatusType
 
 
 def check_value(value: ConnectionStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codestar_connections.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `CodeStarconnections` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/type_defs/).
+
 ```python
-from types_aiobotocore_codestar_connections.type_defs import (
-    ConnectionTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    VpcConfigurationTypeDef,
-    DeleteConnectionInputRequestTypeDef,
-    DeleteHostInputRequestTypeDef,
-    GetConnectionInputRequestTypeDef,
-    GetHostInputRequestTypeDef,
-    VpcConfigurationOutputTypeDef,
-    ListConnectionsInputRequestTypeDef,
-    ListHostsInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CreateConnectionInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateConnectionOutputTypeDef,
-    CreateHostOutputTypeDef,
-    GetConnectionOutputTypeDef,
-    ListConnectionsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    CreateHostInputRequestTypeDef,
-    UpdateHostInputRequestTypeDef,
-    GetHostOutputTypeDef,
-    HostTypeDef,
-    VpcConfigurationUnionTypeDef,
-    ListHostsOutputTypeDef,
-)
+from types_aiobotocore_codestar_connections.type_defs import ConnectionTypeDef
 
 
 def get_value() -> ConnectionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/setup.py` & `types-aiobotocore-codestar-connections-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-codestar-connections",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_codestar_connections"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CodeStarconnections 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/__init__.py` & `types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/__init__.pyi` & `types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/__main__.py` & `types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CodeStarconnections 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections\nOther"
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

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/client.py` & `types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,37 +25,34 @@
     CreateHostOutputTypeDef,
     GetConnectionOutputTypeDef,
     GetHostOutputTypeDef,
     ListConnectionsOutputTypeDef,
     ListHostsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagTypeDef,
-    VpcConfigurationUnionTypeDef,
+    VpcConfigurationTypeDef,
 )
 
 __all__ = ("CodeStarconnectionsClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceUnavailableException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
-
 class CodeStarconnectionsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/)
     """
 
     meta: ClientMeta
@@ -64,31 +61,28 @@
     def exceptions(self) -> Exceptions:
         """
         CodeStarconnectionsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#close)
         """
-
     async def create_connection(
         self,
         *,
         ConnectionName: str,
         ProviderType: ProviderTypeType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         HostArn: str = ...
@@ -96,146 +90,132 @@
         """
         Creates a connection that can then be given to other AWS services like
         CodePipeline so that it can access third-party code repositories.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#create_connection)
         """
-
     async def create_host(
         self,
         *,
         Name: str,
         ProviderType: ProviderTypeType,
         ProviderEndpoint: str,
-        VpcConfiguration: VpcConfigurationUnionTypeDef = ...,
+        VpcConfiguration: VpcConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateHostOutputTypeDef:
         """
         Creates a resource that represents the infrastructure where a third-party
         provider is installed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_host)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#create_host)
         """
-
     async def delete_connection(self, *, ConnectionArn: str) -> Dict[str, Any]:
         """
         The connection to be deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.delete_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#delete_connection)
         """
-
     async def delete_host(self, *, HostArn: str) -> Dict[str, Any]:
         """
         The host to be deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.delete_host)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#delete_host)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#generate_presigned_url)
         """
-
     async def get_connection(self, *, ConnectionArn: str) -> GetConnectionOutputTypeDef:
         """
         Returns the connection ARN and details such as status, owner, and provider type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.get_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#get_connection)
         """
-
     async def get_host(self, *, HostArn: str) -> GetHostOutputTypeDef:
         """
         Returns the host ARN and details such as status, provider type, endpoint, and,
         if applicable, the VPC configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.get_host)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#get_host)
         """
-
     async def list_connections(
         self,
         *,
         ProviderTypeFilter: ProviderTypeType = ...,
         HostArnFilter: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListConnectionsOutputTypeDef:
         """
         Lists the connections associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.list_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#list_connections)
         """
-
     async def list_hosts(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListHostsOutputTypeDef:
         """
         Lists the hosts associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.list_hosts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#list_hosts)
         """
-
     async def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceOutputTypeDef:
         """
         Gets the set of key-value pairs (metadata) that are used to manage the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#list_tags_for_resource)
         """
-
     async def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds to or modifies the tags of the given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#tag_resource)
         """
-
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from an AWS resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#untag_resource)
         """
-
     async def update_host(
         self,
         *,
         HostArn: str,
         ProviderEndpoint: str = ...,
-        VpcConfiguration: VpcConfigurationUnionTypeDef = ...
+        VpcConfiguration: VpcConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a specified host with the provided configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.update_host)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#update_host)
         """
-
     async def __aenter__(self) -> "CodeStarconnectionsClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/)
         """
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/client.pyi` & `types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,34 +25,37 @@
     CreateHostOutputTypeDef,
     GetConnectionOutputTypeDef,
     GetHostOutputTypeDef,
     ListConnectionsOutputTypeDef,
     ListHostsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagTypeDef,
-    VpcConfigurationUnionTypeDef,
+    VpcConfigurationTypeDef,
 )
 
 __all__ = ("CodeStarconnectionsClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ResourceUnavailableException: Type[BotocoreClientError]
     UnsupportedOperationException: Type[BotocoreClientError]
 
+
 class CodeStarconnectionsClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/)
     """
 
     meta: ClientMeta
@@ -61,28 +64,31 @@
     def exceptions(self) -> Exceptions:
         """
         CodeStarconnectionsClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#close)
         """
+
     async def create_connection(
         self,
         *,
         ConnectionName: str,
         ProviderType: ProviderTypeType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         HostArn: str = ...
@@ -90,132 +96,146 @@
         """
         Creates a connection that can then be given to other AWS services like
         CodePipeline so that it can access third-party code repositories.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#create_connection)
         """
+
     async def create_host(
         self,
         *,
         Name: str,
         ProviderType: ProviderTypeType,
         ProviderEndpoint: str,
-        VpcConfiguration: VpcConfigurationUnionTypeDef = ...,
+        VpcConfiguration: VpcConfigurationTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateHostOutputTypeDef:
         """
         Creates a resource that represents the infrastructure where a third-party
         provider is installed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.create_host)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#create_host)
         """
+
     async def delete_connection(self, *, ConnectionArn: str) -> Dict[str, Any]:
         """
         The connection to be deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.delete_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#delete_connection)
         """
+
     async def delete_host(self, *, HostArn: str) -> Dict[str, Any]:
         """
         The host to be deleted.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.delete_host)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#delete_host)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#generate_presigned_url)
         """
+
     async def get_connection(self, *, ConnectionArn: str) -> GetConnectionOutputTypeDef:
         """
         Returns the connection ARN and details such as status, owner, and provider type.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.get_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#get_connection)
         """
+
     async def get_host(self, *, HostArn: str) -> GetHostOutputTypeDef:
         """
         Returns the host ARN and details such as status, provider type, endpoint, and,
         if applicable, the VPC configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.get_host)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#get_host)
         """
+
     async def list_connections(
         self,
         *,
         ProviderTypeFilter: ProviderTypeType = ...,
         HostArnFilter: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListConnectionsOutputTypeDef:
         """
         Lists the connections associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.list_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#list_connections)
         """
+
     async def list_hosts(
         self, *, MaxResults: int = ..., NextToken: str = ...
     ) -> ListHostsOutputTypeDef:
         """
         Lists the hosts associated with your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.list_hosts)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#list_hosts)
         """
+
     async def list_tags_for_resource(self, *, ResourceArn: str) -> ListTagsForResourceOutputTypeDef:
         """
         Gets the set of key-value pairs (metadata) that are used to manage the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#list_tags_for_resource)
         """
+
     async def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds to or modifies the tags of the given resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#tag_resource)
         """
+
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes tags from an AWS resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#untag_resource)
         """
+
     async def update_host(
         self,
         *,
         HostArn: str,
         ProviderEndpoint: str = ...,
-        VpcConfiguration: VpcConfigurationUnionTypeDef = ...
+        VpcConfiguration: VpcConfigurationTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a specified host with the provided configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client.update_host)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/#update_host)
         """
+
     async def __aenter__(self) -> "CodeStarconnectionsClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/client/)
         """
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/literals.py` & `types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/literals.pyi` & `types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/type_defs.py` & `types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -8,50 +8,47 @@
     ```python
     from types_aiobotocore_codestar_connections.type_defs import ConnectionTypeDef
 
     data: ConnectionTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import ConnectionStatusType, ProviderTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ConnectionTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "VpcConfigurationTypeDef",
     "DeleteConnectionInputRequestTypeDef",
     "DeleteHostInputRequestTypeDef",
     "GetConnectionInputRequestTypeDef",
     "GetHostInputRequestTypeDef",
-    "VpcConfigurationOutputTypeDef",
     "ListConnectionsInputRequestTypeDef",
     "ListHostsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "CreateConnectionInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateConnectionOutputTypeDef",
     "CreateHostOutputTypeDef",
     "GetConnectionOutputTypeDef",
     "ListConnectionsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "CreateHostInputRequestTypeDef",
-    "UpdateHostInputRequestTypeDef",
     "GetHostOutputTypeDef",
     "HostTypeDef",
-    "VpcConfigurationUnionTypeDef",
+    "UpdateHostInputRequestTypeDef",
     "ListHostsOutputTypeDef",
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ConnectionName": str,
@@ -95,19 +92,17 @@
     "_OptionalVpcConfigurationTypeDef",
     {
         "TlsCertificate": str,
     },
     total=False,
 )
 
-
 class VpcConfigurationTypeDef(_RequiredVpcConfigurationTypeDef, _OptionalVpcConfigurationTypeDef):
     pass
 
-
 DeleteConnectionInputRequestTypeDef = TypedDict(
     "DeleteConnectionInputRequestTypeDef",
     {
         "ConnectionArn": str,
     },
 )
 
@@ -128,37 +123,14 @@
 GetHostInputRequestTypeDef = TypedDict(
     "GetHostInputRequestTypeDef",
     {
         "HostArn": str,
     },
 )
 
-_RequiredVpcConfigurationOutputTypeDef = TypedDict(
-    "_RequiredVpcConfigurationOutputTypeDef",
-    {
-        "VpcId": str,
-        "SubnetIds": List[str],
-        "SecurityGroupIds": List[str],
-    },
-)
-_OptionalVpcConfigurationOutputTypeDef = TypedDict(
-    "_OptionalVpcConfigurationOutputTypeDef",
-    {
-        "TlsCertificate": str,
-    },
-    total=False,
-)
-
-
-class VpcConfigurationOutputTypeDef(
-    _RequiredVpcConfigurationOutputTypeDef, _OptionalVpcConfigurationOutputTypeDef
-):
-    pass
-
-
 ListConnectionsInputRequestTypeDef = TypedDict(
     "ListConnectionsInputRequestTypeDef",
     {
         "ProviderTypeFilter": ProviderTypeType,
         "HostArnFilter": str,
         "MaxResults": int,
         "NextToken": str,
@@ -202,21 +174,19 @@
         "ProviderType": ProviderTypeType,
         "Tags": Sequence[TagTypeDef],
         "HostArn": str,
     },
     total=False,
 )
 
-
 class CreateConnectionInputRequestTypeDef(
     _RequiredCreateConnectionInputRequestTypeDef, _OptionalCreateConnectionInputRequestTypeDef
 ):
     pass
 
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -277,70 +247,65 @@
     {
         "VpcConfiguration": VpcConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateHostInputRequestTypeDef(
     _RequiredCreateHostInputRequestTypeDef, _OptionalCreateHostInputRequestTypeDef
 ):
     pass
 
-
-_RequiredUpdateHostInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateHostInputRequestTypeDef",
-    {
-        "HostArn": str,
-    },
-)
-_OptionalUpdateHostInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateHostInputRequestTypeDef",
-    {
-        "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateHostInputRequestTypeDef(
-    _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
-):
-    pass
-
-
 GetHostOutputTypeDef = TypedDict(
     "GetHostOutputTypeDef",
     {
         "Name": str,
         "Status": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+        "VpcConfiguration": VpcConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "Name": str,
         "HostArn": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+        "VpcConfiguration": VpcConfigurationTypeDef,
         "Status": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
-VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
+_RequiredUpdateHostInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateHostInputRequestTypeDef",
+    {
+        "HostArn": str,
+    },
+)
+_OptionalUpdateHostInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateHostInputRequestTypeDef",
+    {
+        "ProviderEndpoint": str,
+        "VpcConfiguration": VpcConfigurationTypeDef,
+    },
+    total=False,
+)
+
+class UpdateHostInputRequestTypeDef(
+    _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
+):
+    pass
+
 ListHostsOutputTypeDef = TypedDict(
     "ListHostsOutputTypeDef",
     {
         "Hosts": List[HostTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections/type_defs.pyi` & `types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,49 +8,48 @@
     ```python
     from types_aiobotocore_codestar_connections.type_defs import ConnectionTypeDef
 
     data: ConnectionTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import ConnectionStatusType, ProviderTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ConnectionTypeDef",
     "TagTypeDef",
     "ResponseMetadataTypeDef",
     "VpcConfigurationTypeDef",
     "DeleteConnectionInputRequestTypeDef",
     "DeleteHostInputRequestTypeDef",
     "GetConnectionInputRequestTypeDef",
     "GetHostInputRequestTypeDef",
-    "VpcConfigurationOutputTypeDef",
     "ListConnectionsInputRequestTypeDef",
     "ListHostsInputRequestTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "CreateConnectionInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "CreateConnectionOutputTypeDef",
     "CreateHostOutputTypeDef",
     "GetConnectionOutputTypeDef",
     "ListConnectionsOutputTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "CreateHostInputRequestTypeDef",
-    "UpdateHostInputRequestTypeDef",
     "GetHostOutputTypeDef",
     "HostTypeDef",
-    "VpcConfigurationUnionTypeDef",
+    "UpdateHostInputRequestTypeDef",
     "ListHostsOutputTypeDef",
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ConnectionName": str,
@@ -94,17 +93,19 @@
     "_OptionalVpcConfigurationTypeDef",
     {
         "TlsCertificate": str,
     },
     total=False,
 )
 
+
 class VpcConfigurationTypeDef(_RequiredVpcConfigurationTypeDef, _OptionalVpcConfigurationTypeDef):
     pass
 
+
 DeleteConnectionInputRequestTypeDef = TypedDict(
     "DeleteConnectionInputRequestTypeDef",
     {
         "ConnectionArn": str,
     },
 )
 
@@ -125,35 +126,14 @@
 GetHostInputRequestTypeDef = TypedDict(
     "GetHostInputRequestTypeDef",
     {
         "HostArn": str,
     },
 )
 
-_RequiredVpcConfigurationOutputTypeDef = TypedDict(
-    "_RequiredVpcConfigurationOutputTypeDef",
-    {
-        "VpcId": str,
-        "SubnetIds": List[str],
-        "SecurityGroupIds": List[str],
-    },
-)
-_OptionalVpcConfigurationOutputTypeDef = TypedDict(
-    "_OptionalVpcConfigurationOutputTypeDef",
-    {
-        "TlsCertificate": str,
-    },
-    total=False,
-)
-
-class VpcConfigurationOutputTypeDef(
-    _RequiredVpcConfigurationOutputTypeDef, _OptionalVpcConfigurationOutputTypeDef
-):
-    pass
-
 ListConnectionsInputRequestTypeDef = TypedDict(
     "ListConnectionsInputRequestTypeDef",
     {
         "ProviderTypeFilter": ProviderTypeType,
         "HostArnFilter": str,
         "MaxResults": int,
         "NextToken": str,
@@ -197,19 +177,21 @@
         "ProviderType": ProviderTypeType,
         "Tags": Sequence[TagTypeDef],
         "HostArn": str,
     },
     total=False,
 )
 
+
 class CreateConnectionInputRequestTypeDef(
     _RequiredCreateConnectionInputRequestTypeDef, _OptionalCreateConnectionInputRequestTypeDef
 ):
     pass
 
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -270,66 +252,69 @@
     {
         "VpcConfiguration": VpcConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateHostInputRequestTypeDef(
     _RequiredCreateHostInputRequestTypeDef, _OptionalCreateHostInputRequestTypeDef
 ):
     pass
 
-_RequiredUpdateHostInputRequestTypeDef = TypedDict(
-    "_RequiredUpdateHostInputRequestTypeDef",
-    {
-        "HostArn": str,
-    },
-)
-_OptionalUpdateHostInputRequestTypeDef = TypedDict(
-    "_OptionalUpdateHostInputRequestTypeDef",
-    {
-        "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationTypeDef,
-    },
-    total=False,
-)
-
-class UpdateHostInputRequestTypeDef(
-    _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
-):
-    pass
 
 GetHostOutputTypeDef = TypedDict(
     "GetHostOutputTypeDef",
     {
         "Name": str,
         "Status": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+        "VpcConfiguration": VpcConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HostTypeDef = TypedDict(
     "HostTypeDef",
     {
         "Name": str,
         "HostArn": str,
         "ProviderType": ProviderTypeType,
         "ProviderEndpoint": str,
-        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+        "VpcConfiguration": VpcConfigurationTypeDef,
         "Status": str,
         "StatusMessage": str,
     },
     total=False,
 )
 
-VpcConfigurationUnionTypeDef = Union[VpcConfigurationTypeDef, VpcConfigurationOutputTypeDef]
+_RequiredUpdateHostInputRequestTypeDef = TypedDict(
+    "_RequiredUpdateHostInputRequestTypeDef",
+    {
+        "HostArn": str,
+    },
+)
+_OptionalUpdateHostInputRequestTypeDef = TypedDict(
+    "_OptionalUpdateHostInputRequestTypeDef",
+    {
+        "ProviderEndpoint": str,
+        "VpcConfiguration": VpcConfigurationTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateHostInputRequestTypeDef(
+    _RequiredUpdateHostInputRequestTypeDef, _OptionalUpdateHostInputRequestTypeDef
+):
+    pass
+
+
 ListHostsOutputTypeDef = TypedDict(
     "ListHostsOutputTypeDef",
     {
         "Hosts": List[HostTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/PKG-INFO` & `types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-codestar-connections
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CodeStarconnections 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CodeStarconnections 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/
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
 [types-aiobotocore-codestar-connections docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,66 +266,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_codestar_connections.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CodeStarconnections` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/literals/).
+
 ```python
-from types_aiobotocore_codestar_connections.literals import (
-    ConnectionStatusType,
-    ProviderTypeType,
-    CodeStarconnectionsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_codestar_connections.literals import ConnectionStatusType
 
 
 def check_value(value: ConnectionStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_codestar_connections.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `CodeStarconnections` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_codestar_connections/type_defs/).
+
 ```python
-from types_aiobotocore_codestar_connections.type_defs import (
-    ConnectionTypeDef,
-    TagTypeDef,
-    ResponseMetadataTypeDef,
-    VpcConfigurationTypeDef,
-    DeleteConnectionInputRequestTypeDef,
-    DeleteHostInputRequestTypeDef,
-    GetConnectionInputRequestTypeDef,
-    GetHostInputRequestTypeDef,
-    VpcConfigurationOutputTypeDef,
-    ListConnectionsInputRequestTypeDef,
-    ListHostsInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CreateConnectionInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    CreateConnectionOutputTypeDef,
-    CreateHostOutputTypeDef,
-    GetConnectionOutputTypeDef,
-    ListConnectionsOutputTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    CreateHostInputRequestTypeDef,
-    UpdateHostInputRequestTypeDef,
-    GetHostOutputTypeDef,
-    HostTypeDef,
-    VpcConfigurationUnionTypeDef,
-    ListHostsOutputTypeDef,
-)
+from types_aiobotocore_codestar_connections.type_defs import ConnectionTypeDef
 
 
 def get_value() -> ConnectionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-codestar-connections-2.5.2.post1/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt` & `types-aiobotocore-codestar-connections-2.5.2.post2/types_aiobotocore_codestar_connections.egg-info/SOURCES.txt`

 * *Files identical despite different names*

