# Comparing `tmp/types-aiobotocore-appconfigdata-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-appconfigdata-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appconfigdata-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-appconfigdata-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:22 2023, max compression
```

## Comparing `types-aiobotocore-appconfigdata-2.5.2.post1.tar` & `types-aiobotocore-appconfigdata-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.541660 types-aiobotocore-appconfigdata-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-08-02 14:51:50.541660 types-aiobotocore-appconfigdata-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10955 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.541660 types-aiobotocore-appconfigdata-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.541660 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-02 14:33:08.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-02 14:33:08.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:07.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.541660 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-08-02 14:51:50.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 14:51:50.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:51:50.000000 types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.775005 types-aiobotocore-appconfigdata-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-08-04 12:00:22.767005 types-aiobotocore-appconfigdata-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:22.775005 types-aiobotocore-appconfigdata-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.767005 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8110 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8108 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:15.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.767005 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12562 2023-08-04 12:00:22.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-04 12:00:22.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:22.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:00:22.000000 types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post1/LICENSE` & `types-aiobotocore-appconfigdata-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post1/PKG-INFO` & `types-aiobotocore-appconfigdata-2.5.2.post2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfigdata
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/
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
 [types-aiobotocore-appconfigdata docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,42 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_appconfigdata.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `AppConfigData` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/literals/).
+
 ```python
-from types_aiobotocore_appconfigdata.literals import (
-    AppConfigDataServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_appconfigdata.literals import AppConfigDataServiceName
 
 
 def check_value(value: AppConfigDataServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_appconfigdata.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `AppConfigData` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/type_defs/).
+
 ```python
-from types_aiobotocore_appconfigdata.type_defs import (
-    GetLatestConfigurationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartConfigurationSessionRequestRequestTypeDef,
-    GetLatestConfigurationResponseTypeDef,
-    StartConfigurationSessionResponseTypeDef,
-)
+from types_aiobotocore_appconfigdata.type_defs import GetLatestConfigurationRequestRequestTypeDef
 
 
 def get_value() -> GetLatestConfigurationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post1/README.md` & `types-aiobotocore-appconfigdata-2.5.2.post2/README.md`

 * *Files 8% similar despite different names*

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
 [types-aiobotocore-appconfigdata docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,42 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_appconfigdata.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `AppConfigData` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/literals/).
+
 ```python
-from types_aiobotocore_appconfigdata.literals import (
-    AppConfigDataServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_appconfigdata.literals import AppConfigDataServiceName
 
 
 def check_value(value: AppConfigDataServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_appconfigdata.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `AppConfigData` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/type_defs/).
+
 ```python
-from types_aiobotocore_appconfigdata.type_defs import (
-    GetLatestConfigurationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartConfigurationSessionRequestRequestTypeDef,
-    GetLatestConfigurationResponseTypeDef,
-    StartConfigurationSessionResponseTypeDef,
-)
+from types_aiobotocore_appconfigdata.type_defs import GetLatestConfigurationRequestRequestTypeDef
 
 
 def get_value() -> GetLatestConfigurationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post1/setup.py` & `types-aiobotocore-appconfigdata-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appconfigdata",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_appconfigdata"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/__main__.py` & `types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.AppConfigData 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appconfigdata.html#AppConfigData\nOther"
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

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/client.py` & `types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/client.pyi` & `types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/literals.py` & `types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/literals.pyi` & `types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/type_defs.py` & `types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata/type_defs.pyi` & `types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/PKG-INFO` & `types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appconfigdata
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.AppConfigData 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/
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
 [types-aiobotocore-appconfigdata docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,42 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_appconfigdata.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `AppConfigData` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/literals/).
+
 ```python
-from types_aiobotocore_appconfigdata.literals import (
-    AppConfigDataServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_appconfigdata.literals import AppConfigDataServiceName
 
 
 def check_value(value: AppConfigDataServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_appconfigdata.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `AppConfigData` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appconfigdata/type_defs/).
+
 ```python
-from types_aiobotocore_appconfigdata.type_defs import (
-    GetLatestConfigurationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartConfigurationSessionRequestRequestTypeDef,
-    GetLatestConfigurationResponseTypeDef,
-    StartConfigurationSessionResponseTypeDef,
-)
+from types_aiobotocore_appconfigdata.type_defs import GetLatestConfigurationRequestRequestTypeDef
 
 
 def get_value() -> GetLatestConfigurationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-appconfigdata-2.5.2.post1/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt` & `types-aiobotocore-appconfigdata-2.5.2.post2/types_aiobotocore_appconfigdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

