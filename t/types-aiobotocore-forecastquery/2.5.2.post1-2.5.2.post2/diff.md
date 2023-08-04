# Comparing `tmp/types-aiobotocore-forecastquery-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-forecastquery-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-forecastquery-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-forecastquery-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:55 2023, max compression
```

## Comparing `types-aiobotocore-forecastquery-2.5.2.post1.tar` & `types-aiobotocore-forecastquery-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.361582 types-aiobotocore-forecastquery-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-08-02 14:52:19.357582 types-aiobotocore-forecastquery-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10997 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:19.361582 types-aiobotocore-forecastquery-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.353582 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:57.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.357582 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-08-02 14:52:19.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 14:52:19.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:19.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:19.000000 types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.756265 types-aiobotocore-forecastquery-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:27.000000 types-aiobotocore-forecastquery-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-08-04 12:00:55.756265 types-aiobotocore-forecastquery-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11036 2023-08-04 11:46:27.000000 types-aiobotocore-forecastquery-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:55.756265 types-aiobotocore-forecastquery-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-04 11:46:27.000000 types-aiobotocore-forecastquery-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.756265 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-04 11:46:27.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-04 11:46:27.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-04 11:46:27.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-08-04 11:46:28.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-08-04 11:46:28.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-08-04 11:46:28.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7817 2023-08-04 11:46:28.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:27.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-08-04 11:46:28.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-08-04 11:46:28.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:27.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:55.756265 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-08-04 12:00:55.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-04 12:00:55.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:55.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:55.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 12:00:55.000000 types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/LICENSE` & `types-aiobotocore-forecastquery-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/PKG-INFO` & `types-aiobotocore-forecastquery-2.5.2.post2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-forecastquery
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ForecastQueryService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ForecastQueryService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/
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
 [types-aiobotocore-forecastquery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,44 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_forecastquery.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ForecastQueryService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/literals/).
+
 ```python
-from types_aiobotocore_forecastquery.literals import (
-    ForecastQueryServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_forecastquery.literals import ForecastQueryServiceServiceName
 
 
 def check_value(value: ForecastQueryServiceServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_forecastquery.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ForecastQueryService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/type_defs/).
+
 ```python
-from types_aiobotocore_forecastquery.type_defs import (
-    DataPointTypeDef,
-    QueryForecastRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    QueryWhatIfForecastRequestRequestTypeDef,
-    ForecastTypeDef,
-    QueryForecastResponseTypeDef,
-    QueryWhatIfForecastResponseTypeDef,
-)
+from types_aiobotocore_forecastquery.type_defs import DataPointTypeDef
 
 
 def get_value() -> DataPointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/README.md` & `types-aiobotocore-forecastquery-2.5.2.post2/README.md`

 * *Files 3% similar despite different names*

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
 [types-aiobotocore-forecastquery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,44 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_forecastquery.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ForecastQueryService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/literals/).
+
 ```python
-from types_aiobotocore_forecastquery.literals import (
-    ForecastQueryServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_forecastquery.literals import ForecastQueryServiceServiceName
 
 
 def check_value(value: ForecastQueryServiceServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_forecastquery.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ForecastQueryService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/type_defs/).
+
 ```python
-from types_aiobotocore_forecastquery.type_defs import (
-    DataPointTypeDef,
-    QueryForecastRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    QueryWhatIfForecastRequestRequestTypeDef,
-    ForecastTypeDef,
-    QueryForecastResponseTypeDef,
-    QueryWhatIfForecastResponseTypeDef,
-)
+from types_aiobotocore_forecastquery.type_defs import DataPointTypeDef
 
 
 def get_value() -> DataPointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/setup.py` & `types-aiobotocore-forecastquery-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-forecastquery",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_forecastquery"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ForecastQueryService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/__init__.py` & `types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/__init__.pyi` & `types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/__main__.py` & `types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ForecastQueryService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecastquery.html#ForecastQueryService\nOther"
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

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/client.py` & `types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/client.pyi` & `types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/literals.py` & `types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/literals.pyi` & `types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/type_defs.py` & `types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery/type_defs.pyi` & `types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery.egg-info/PKG-INFO` & `types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-forecastquery
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ForecastQueryService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ForecastQueryService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/
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
 [types-aiobotocore-forecastquery docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,44 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_forecastquery.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ForecastQueryService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/literals/).
+
 ```python
-from types_aiobotocore_forecastquery.literals import (
-    ForecastQueryServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_forecastquery.literals import ForecastQueryServiceServiceName
 
 
 def check_value(value: ForecastQueryServiceServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_forecastquery.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ForecastQueryService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecastquery/type_defs/).
+
 ```python
-from types_aiobotocore_forecastquery.type_defs import (
-    DataPointTypeDef,
-    QueryForecastRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    QueryWhatIfForecastRequestRequestTypeDef,
-    ForecastTypeDef,
-    QueryForecastResponseTypeDef,
-    QueryWhatIfForecastResponseTypeDef,
-)
+from types_aiobotocore_forecastquery.type_defs import DataPointTypeDef
 
 
 def get_value() -> DataPointTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-forecastquery-2.5.2.post1/types_aiobotocore_forecastquery.egg-info/SOURCES.txt` & `types-aiobotocore-forecastquery-2.5.2.post2/types_aiobotocore_forecastquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

