# Comparing `tmp/types-aiobotocore-iotsecuretunneling-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iotsecuretunneling-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotsecuretunneling-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotsecuretunneling-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
```

## Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1.tar` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:27.513560 types-aiobotocore-iotsecuretunneling-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-08-02 14:52:27.513560 types-aiobotocore-iotsecuretunneling-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:27.513560 types-aiobotocore-iotsecuretunneling-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:27.513560 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:27.513560 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-08-02 14:52:27.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-02 14:52:27.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:27.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:27.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:27.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 14:52:27.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:58:49.626642 types-aiobotocore-iotsecuretunneling-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12785 2023-08-04 13:59:12.456642 types-aiobotocore-iotsecuretunneling-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11223 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.456642 types-aiobotocore-iotsecuretunneling-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2149 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:58:49.626642 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      530 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      529 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      987 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9213 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9197 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8302 2023-08-04 13:41:10.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8300 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6508 2023-08-04 13:41:10.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6501 2023-08-04 13:41:10.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:41:09.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.456642 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12785 2023-08-04 13:59:12.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      921 2023-08-04 13:59:12.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       37 2023-08-04 13:59:12.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/LICENSE` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/PKG-INFO` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotsecuretunneling
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/
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
 [types-aiobotocore-iotsecuretunneling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,62 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iotsecuretunneling.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `IoTSecureTunneling` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/literals/).
+
 ```python
-from types_aiobotocore_iotsecuretunneling.literals import (
-    ClientModeType,
-    ConnectionStatusType,
-    TunnelStatusType,
-    IoTSecureTunnelingServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_iotsecuretunneling.literals import ClientModeType
 
 
 def check_value(value: ClientModeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iotsecuretunneling.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTSecureTunneling` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/type_defs/).
+
 ```python
-from types_aiobotocore_iotsecuretunneling.type_defs import (
-    CloseTunnelRequestRequestTypeDef,
-    ConnectionStateTypeDef,
-    DescribeTunnelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DestinationConfigOutputTypeDef,
-    DestinationConfigTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
-    ListTunnelsRequestRequestTypeDef,
-    TunnelSummaryTypeDef,
-    TimeoutConfigTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    OpenTunnelResponseTypeDef,
-    RotateTunnelAccessTokenResponseTypeDef,
-    DestinationConfigUnionTypeDef,
-    RotateTunnelAccessTokenRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListTunnelsResponseTypeDef,
-    OpenTunnelRequestRequestTypeDef,
-    TunnelTypeDef,
-    DescribeTunnelResponseTypeDef,
-)
+from types_aiobotocore_iotsecuretunneling.type_defs import CloseTunnelRequestRequestTypeDef
 
 
 def get_value() -> CloseTunnelRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/README.md` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-iotsecuretunneling
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore iotsecuretunneling type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotsecuretunneling"></a>
 
 # types-aiobotocore-iotsecuretunneling
 
 [![PyPI - types-aiobotocore-iotsecuretunneling](https://img.shields.io/pypi/v/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/)
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
 [types-aiobotocore-iotsecuretunneling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,62 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iotsecuretunneling.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `IoTSecureTunneling` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/literals/).
+
 ```python
-from types_aiobotocore_iotsecuretunneling.literals import (
-    ClientModeType,
-    ConnectionStatusType,
-    TunnelStatusType,
-    IoTSecureTunnelingServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_iotsecuretunneling.literals import ClientModeType
 
 
 def check_value(value: ClientModeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iotsecuretunneling.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTSecureTunneling` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/type_defs/).
+
 ```python
-from types_aiobotocore_iotsecuretunneling.type_defs import (
-    CloseTunnelRequestRequestTypeDef,
-    ConnectionStateTypeDef,
-    DescribeTunnelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DestinationConfigOutputTypeDef,
-    DestinationConfigTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
-    ListTunnelsRequestRequestTypeDef,
-    TunnelSummaryTypeDef,
-    TimeoutConfigTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    OpenTunnelResponseTypeDef,
-    RotateTunnelAccessTokenResponseTypeDef,
-    DestinationConfigUnionTypeDef,
-    RotateTunnelAccessTokenRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListTunnelsResponseTypeDef,
-    OpenTunnelRequestRequestTypeDef,
-    TunnelTypeDef,
-    DescribeTunnelResponseTypeDef,
-)
+from types_aiobotocore_iotsecuretunneling.type_defs import CloseTunnelRequestRequestTypeDef
 
 
 def get_value() -> CloseTunnelRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/setup.py` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotsecuretunneling",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iotsecuretunneling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTSecureTunneling 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/__init__.py` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/__init__.pyi` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/__main__.py` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.IoTSecureTunneling 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling\nOther"
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

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/client.py` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ClientModeType
 from .type_defs import (
     DescribeTunnelResponseTypeDef,
-    DestinationConfigUnionTypeDef,
+    DestinationConfigTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelResponseTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
     TagTypeDef,
     TimeoutConfigTypeDef,
 )
@@ -132,15 +132,15 @@
         """
 
     async def open_tunnel(
         self,
         *,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        destinationConfig: DestinationConfigUnionTypeDef = ...,
+        destinationConfig: DestinationConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...
     ) -> OpenTunnelResponseTypeDef:
         """
         Creates a new tunnel, and returns two client access tokens for clients to use to
         connect to the IoT Secure Tunneling proxy server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.open_tunnel)
@@ -148,15 +148,15 @@
         """
 
     async def rotate_tunnel_access_token(
         self,
         *,
         tunnelId: str,
         clientMode: ClientModeType,
-        destinationConfig: DestinationConfigUnionTypeDef = ...
+        destinationConfig: DestinationConfigTypeDef = ...
     ) -> RotateTunnelAccessTokenResponseTypeDef:
         """
         Revokes the current client access token (CAT) and returns new CAT for clients to
         use when reconnecting to secure tunneling to access the same tunnel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.rotate_tunnel_access_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/client/#rotate_tunnel_access_token)
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/client.pyi` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ClientModeType
 from .type_defs import (
     DescribeTunnelResponseTypeDef,
-    DestinationConfigUnionTypeDef,
+    DestinationConfigTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelResponseTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
     TagTypeDef,
     TimeoutConfigTypeDef,
 )
@@ -121,30 +121,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/client/#list_tunnels)
         """
     async def open_tunnel(
         self,
         *,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        destinationConfig: DestinationConfigUnionTypeDef = ...,
+        destinationConfig: DestinationConfigTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...
     ) -> OpenTunnelResponseTypeDef:
         """
         Creates a new tunnel, and returns two client access tokens for clients to use to
         connect to the IoT Secure Tunneling proxy server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.open_tunnel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/client/#open_tunnel)
         """
     async def rotate_tunnel_access_token(
         self,
         *,
         tunnelId: str,
         clientMode: ClientModeType,
-        destinationConfig: DestinationConfigUnionTypeDef = ...
+        destinationConfig: DestinationConfigTypeDef = ...
     ) -> RotateTunnelAccessTokenResponseTypeDef:
         """
         Revokes the current client access token (CAT) and returns new CAT for clients to
         use when reconnecting to secure tunneling to access the same tunnel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.rotate_tunnel_access_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/client/#rotate_tunnel_access_token)
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/literals.py` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,15 @@
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
@@ -148,14 +149,15 @@
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
@@ -234,26 +236,28 @@
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

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/literals.pyi` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
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
@@ -146,14 +147,15 @@
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
@@ -232,26 +234,28 @@
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

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/type_defs.py` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,40 +9,37 @@
     from types_aiobotocore_iotsecuretunneling.type_defs import CloseTunnelRequestRequestTypeDef
 
     data: CloseTunnelRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import ClientModeType, ConnectionStatusType, TunnelStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CloseTunnelRequestRequestTypeDef",
     "ConnectionStateTypeDef",
     "DescribeTunnelRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "DestinationConfigOutputTypeDef",
     "DestinationConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListTunnelsRequestRequestTypeDef",
     "TunnelSummaryTypeDef",
     "TimeoutConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "OpenTunnelResponseTypeDef",
     "RotateTunnelAccessTokenResponseTypeDef",
-    "DestinationConfigUnionTypeDef",
     "RotateTunnelAccessTokenRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTunnelsResponseTypeDef",
     "OpenTunnelRequestRequestTypeDef",
     "TunnelTypeDef",
     "DescribeTunnelResponseTypeDef",
@@ -58,21 +55,19 @@
     "_OptionalCloseTunnelRequestRequestTypeDef",
     {
         "delete": bool,
     },
     total=False,
 )
 
-
 class CloseTunnelRequestRequestTypeDef(
     _RequiredCloseTunnelRequestRequestTypeDef, _OptionalCloseTunnelRequestRequestTypeDef
 ):
     pass
 
-
 ConnectionStateTypeDef = TypedDict(
     "ConnectionStateTypeDef",
     {
         "status": ConnectionStatusType,
         "lastUpdatedAt": datetime,
     },
     total=False,
@@ -92,56 +87,33 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredDestinationConfigOutputTypeDef = TypedDict(
-    "_RequiredDestinationConfigOutputTypeDef",
-    {
-        "services": List[str],
-    },
-)
-_OptionalDestinationConfigOutputTypeDef = TypedDict(
-    "_OptionalDestinationConfigOutputTypeDef",
-    {
-        "thingName": str,
-    },
-    total=False,
-)
-
-
-class DestinationConfigOutputTypeDef(
-    _RequiredDestinationConfigOutputTypeDef, _OptionalDestinationConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredDestinationConfigTypeDef = TypedDict(
     "_RequiredDestinationConfigTypeDef",
     {
-        "services": Sequence[str],
+        "services": List[str],
     },
 )
 _OptionalDestinationConfigTypeDef = TypedDict(
     "_OptionalDestinationConfigTypeDef",
     {
         "thingName": str,
     },
     total=False,
 )
 
-
 class DestinationConfigTypeDef(
     _RequiredDestinationConfigTypeDef, _OptionalDestinationConfigTypeDef
 ):
     pass
 
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -209,15 +181,14 @@
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DestinationConfigUnionTypeDef = Union[DestinationConfigTypeDef, DestinationConfigOutputTypeDef]
 _RequiredRotateTunnelAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "tunnelId": str,
         "clientMode": ClientModeType,
     },
 )
@@ -225,22 +196,20 @@
     "_OptionalRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "destinationConfig": DestinationConfigTypeDef,
     },
     total=False,
 )
 
-
 class RotateTunnelAccessTokenRequestRequestTypeDef(
     _RequiredRotateTunnelAccessTokenRequestRequestTypeDef,
     _OptionalRotateTunnelAccessTokenRequestRequestTypeDef,
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -278,15 +247,15 @@
     {
         "tunnelId": str,
         "tunnelArn": str,
         "status": TunnelStatusType,
         "sourceConnectionState": ConnectionStateTypeDef,
         "destinationConnectionState": ConnectionStateTypeDef,
         "description": str,
-        "destinationConfig": DestinationConfigOutputTypeDef,
+        "destinationConfig": DestinationConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "tags": List[TagTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/type_defs.pyi` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,39 +9,38 @@
     from types_aiobotocore_iotsecuretunneling.type_defs import CloseTunnelRequestRequestTypeDef
 
     data: CloseTunnelRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import ClientModeType, ConnectionStatusType, TunnelStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CloseTunnelRequestRequestTypeDef",
     "ConnectionStateTypeDef",
     "DescribeTunnelRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
-    "DestinationConfigOutputTypeDef",
     "DestinationConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListTunnelsRequestRequestTypeDef",
     "TunnelSummaryTypeDef",
     "TimeoutConfigTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "OpenTunnelResponseTypeDef",
     "RotateTunnelAccessTokenResponseTypeDef",
-    "DestinationConfigUnionTypeDef",
     "RotateTunnelAccessTokenRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTunnelsResponseTypeDef",
     "OpenTunnelRequestRequestTypeDef",
     "TunnelTypeDef",
     "DescribeTunnelResponseTypeDef",
@@ -57,19 +56,21 @@
     "_OptionalCloseTunnelRequestRequestTypeDef",
     {
         "delete": bool,
     },
     total=False,
 )
 
+
 class CloseTunnelRequestRequestTypeDef(
     _RequiredCloseTunnelRequestRequestTypeDef, _OptionalCloseTunnelRequestRequestTypeDef
 ):
     pass
 
+
 ConnectionStateTypeDef = TypedDict(
     "ConnectionStateTypeDef",
     {
         "status": ConnectionStatusType,
         "lastUpdatedAt": datetime,
     },
     total=False,
@@ -89,52 +90,35 @@
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
     },
 )
 
-_RequiredDestinationConfigOutputTypeDef = TypedDict(
-    "_RequiredDestinationConfigOutputTypeDef",
-    {
-        "services": List[str],
-    },
-)
-_OptionalDestinationConfigOutputTypeDef = TypedDict(
-    "_OptionalDestinationConfigOutputTypeDef",
-    {
-        "thingName": str,
-    },
-    total=False,
-)
-
-class DestinationConfigOutputTypeDef(
-    _RequiredDestinationConfigOutputTypeDef, _OptionalDestinationConfigOutputTypeDef
-):
-    pass
-
 _RequiredDestinationConfigTypeDef = TypedDict(
     "_RequiredDestinationConfigTypeDef",
     {
-        "services": Sequence[str],
+        "services": List[str],
     },
 )
 _OptionalDestinationConfigTypeDef = TypedDict(
     "_OptionalDestinationConfigTypeDef",
     {
         "thingName": str,
     },
     total=False,
 )
 
+
 class DestinationConfigTypeDef(
     _RequiredDestinationConfigTypeDef, _OptionalDestinationConfigTypeDef
 ):
     pass
 
+
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -202,15 +186,14 @@
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DestinationConfigUnionTypeDef = Union[DestinationConfigTypeDef, DestinationConfigOutputTypeDef]
 _RequiredRotateTunnelAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "tunnelId": str,
         "clientMode": ClientModeType,
     },
 )
@@ -218,20 +201,22 @@
     "_OptionalRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "destinationConfig": DestinationConfigTypeDef,
     },
     total=False,
 )
 
+
 class RotateTunnelAccessTokenRequestRequestTypeDef(
     _RequiredRotateTunnelAccessTokenRequestRequestTypeDef,
     _OptionalRotateTunnelAccessTokenRequestRequestTypeDef,
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -269,15 +254,15 @@
     {
         "tunnelId": str,
         "tunnelArn": str,
         "status": TunnelStatusType,
         "sourceConnectionState": ConnectionStateTypeDef,
         "destinationConnectionState": ConnectionStateTypeDef,
         "description": str,
-        "destinationConfig": DestinationConfigOutputTypeDef,
+        "destinationConfig": DestinationConfigTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "tags": List[TagTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-iotsecuretunneling
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.5.2 service generated with mypy-boto3-builder 7.17.1
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotsecuretunneling type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotsecuretunneling"></a>
 
 # types-aiobotocore-iotsecuretunneling
 
 [![PyPI - types-aiobotocore-iotsecuretunneling](https://img.shields.io/pypi/v/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/)
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
 [types-aiobotocore-iotsecuretunneling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,62 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iotsecuretunneling.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `IoTSecureTunneling` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/literals/).
+
 ```python
-from types_aiobotocore_iotsecuretunneling.literals import (
-    ClientModeType,
-    ConnectionStatusType,
-    TunnelStatusType,
-    IoTSecureTunnelingServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_iotsecuretunneling.literals import ClientModeType
 
 
 def check_value(value: ClientModeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iotsecuretunneling.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoTSecureTunneling` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/type_defs/).
+
 ```python
-from types_aiobotocore_iotsecuretunneling.type_defs import (
-    CloseTunnelRequestRequestTypeDef,
-    ConnectionStateTypeDef,
-    DescribeTunnelRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DestinationConfigOutputTypeDef,
-    DestinationConfigTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagTypeDef,
-    ListTunnelsRequestRequestTypeDef,
-    TunnelSummaryTypeDef,
-    TimeoutConfigTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    OpenTunnelResponseTypeDef,
-    RotateTunnelAccessTokenResponseTypeDef,
-    DestinationConfigUnionTypeDef,
-    RotateTunnelAccessTokenRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
-    ListTunnelsResponseTypeDef,
-    OpenTunnelRequestRequestTypeDef,
-    TunnelTypeDef,
-    DescribeTunnelResponseTypeDef,
-)
+from types_aiobotocore_iotsecuretunneling.type_defs import CloseTunnelRequestRequestTypeDef
 
 
 def get_value() -> CloseTunnelRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt` & `types-aiobotocore-iotsecuretunneling-2.5.2.post2/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

