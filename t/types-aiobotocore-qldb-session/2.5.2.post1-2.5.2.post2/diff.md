# Comparing `tmp/types-aiobotocore-qldb-session-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-qldb-session-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-qldb-session-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-qldb-session-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:22 2023, max compression
```

## Comparing `types-aiobotocore-qldb-session-2.5.2.post1.tar` & `types-aiobotocore-qldb-session-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.353490 types-aiobotocore-qldb-session-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-08-02 14:52:50.345490 types-aiobotocore-qldb-session-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11260 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:50.353490 types-aiobotocore-qldb-session-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.345490 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7795 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:45:14.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:50.345490 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12797 2023-08-02 14:52:50.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:52:50.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:50.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:50.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:50.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:50.000000 types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.056643 types-aiobotocore-qldb-session-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:47:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12458 2023-08-04 13:59:22.046643 types-aiobotocore-qldb-session-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10921 2023-08-04 13:47:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:22.056643 types-aiobotocore-qldb-session-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2106 2023-08-04 13:47:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.046643 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      477 2023-08-04 13:47:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      476 2023-08-04 13:47:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      961 2023-08-04 13:47:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5310 2023-08-04 13:47:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5301 2023-08-04 13:47:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7892 2023-08-04 13:47:22.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7890 2023-08-04 13:47:22.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:47:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5455 2023-08-04 13:47:23.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5452 2023-08-04 13:47:23.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:47:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:22.046643 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12458 2023-08-04 13:59:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      819 2023-08-04 13:59:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:21.000000 types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-qldb-session-2.5.2.post1/LICENSE` & `types-aiobotocore-qldb-session-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qldb-session-2.5.2.post1/PKG-INFO` & `types-aiobotocore-qldb-session-2.5.2.post2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-qldb-session
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.QLDBSession 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.QLDBSession 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb_session/
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
 [types-aiobotocore-qldb-session docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb_session/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,57 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_qldb_session.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `QLDBSession` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb_session/literals/).
+
 ```python
-from types_aiobotocore_qldb_session.literals import (
-    QLDBSessionServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_qldb_session.literals import QLDBSessionServiceName
 
 
 def check_value(value: QLDBSessionServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_qldb_session.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `QLDBSession` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb_session/type_defs/).
+
 ```python
-from types_aiobotocore_qldb_session.type_defs import (
-    TimingInformationTypeDef,
-    BlobTypeDef,
-    IOUsageTypeDef,
-    FetchPageRequestTypeDef,
-    ValueHolderOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartSessionRequestTypeDef,
-    AbortTransactionResultTypeDef,
-    EndSessionResultTypeDef,
-    StartSessionResultTypeDef,
-    StartTransactionResultTypeDef,
-    CommitTransactionRequestTypeDef,
-    ValueHolderTypeDef,
-    CommitTransactionResultTypeDef,
-    PageTypeDef,
-    ExecuteStatementRequestTypeDef,
-    ExecuteStatementResultTypeDef,
-    FetchPageResultTypeDef,
-    SendCommandRequestRequestTypeDef,
-    SendCommandResultTypeDef,
-)
+from types_aiobotocore_qldb_session.type_defs import TimingInformationTypeDef
 
 
 def get_value() -> TimingInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-qldb-session-2.5.2.post1/README.md` & `types-aiobotocore-qldb-session-2.5.2.post2/README.md`

 * *Files 10% similar despite different names*

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
 [types-aiobotocore-qldb-session docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb_session/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,57 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_qldb_session.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `QLDBSession` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb_session/literals/).
+
 ```python
-from types_aiobotocore_qldb_session.literals import (
-    QLDBSessionServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_qldb_session.literals import QLDBSessionServiceName
 
 
 def check_value(value: QLDBSessionServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_qldb_session.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `QLDBSession` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb_session/type_defs/).
+
 ```python
-from types_aiobotocore_qldb_session.type_defs import (
-    TimingInformationTypeDef,
-    BlobTypeDef,
-    IOUsageTypeDef,
-    FetchPageRequestTypeDef,
-    ValueHolderOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartSessionRequestTypeDef,
-    AbortTransactionResultTypeDef,
-    EndSessionResultTypeDef,
-    StartSessionResultTypeDef,
-    StartTransactionResultTypeDef,
-    CommitTransactionRequestTypeDef,
-    ValueHolderTypeDef,
-    CommitTransactionResultTypeDef,
-    PageTypeDef,
-    ExecuteStatementRequestTypeDef,
-    ExecuteStatementResultTypeDef,
-    FetchPageResultTypeDef,
-    SendCommandRequestRequestTypeDef,
-    SendCommandResultTypeDef,
-)
+from types_aiobotocore_qldb_session.type_defs import TimingInformationTypeDef
 
 
 def get_value() -> TimingInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-qldb-session-2.5.2.post1/setup.py` & `types-aiobotocore-qldb-session-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-qldb-session",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_qldb_session"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.QLDBSession 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/__main__.py` & `types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.QLDBSession 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.QLDBSession 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb_session//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession\nOther"
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

### Comparing `types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/client.py` & `types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/client.pyi` & `types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/literals.py` & `types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
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
@@ -137,14 +138,15 @@
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
@@ -223,26 +225,28 @@
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

### Comparing `types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/literals.pyi` & `types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
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
@@ -135,14 +136,15 @@
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
@@ -221,26 +223,28 @@
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

### Comparing `types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/type_defs.py` & `types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,35 +17,33 @@
 from aiobotocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TimingInformationTypeDef",
     "BlobTypeDef",
     "IOUsageTypeDef",
     "FetchPageRequestTypeDef",
-    "ValueHolderOutputTypeDef",
     "ResponseMetadataTypeDef",
     "StartSessionRequestTypeDef",
     "AbortTransactionResultTypeDef",
     "EndSessionResultTypeDef",
     "StartSessionResultTypeDef",
     "StartTransactionResultTypeDef",
     "CommitTransactionRequestTypeDef",
     "ValueHolderTypeDef",
     "CommitTransactionResultTypeDef",
-    "PageTypeDef",
     "ExecuteStatementRequestTypeDef",
+    "PageTypeDef",
+    "SendCommandRequestRequestTypeDef",
     "ExecuteStatementResultTypeDef",
     "FetchPageResultTypeDef",
-    "SendCommandRequestRequestTypeDef",
     "SendCommandResultTypeDef",
 )
 
 TimingInformationTypeDef = TypedDict(
     "TimingInformationTypeDef",
     {
         "ProcessingTimeMilliseconds": int,
@@ -67,23 +65,14 @@
     "FetchPageRequestTypeDef",
     {
         "TransactionId": str,
         "NextPageToken": str,
     },
 )
 
-ValueHolderOutputTypeDef = TypedDict(
-    "ValueHolderOutputTypeDef",
-    {
-        "IonBinary": bytes,
-        "IonText": str,
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -156,23 +145,14 @@
         "CommitDigest": bytes,
         "TimingInformation": TimingInformationTypeDef,
         "ConsumedIOs": IOUsageTypeDef,
     },
     total=False,
 )
 
-PageTypeDef = TypedDict(
-    "PageTypeDef",
-    {
-        "Values": List[ValueHolderOutputTypeDef],
-        "NextPageToken": str,
-    },
-    total=False,
-)
-
 _RequiredExecuteStatementRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementRequestTypeDef",
     {
         "TransactionId": str,
         "Statement": str,
     },
 )
@@ -180,20 +160,42 @@
     "_OptionalExecuteStatementRequestTypeDef",
     {
         "Parameters": Sequence[ValueHolderTypeDef],
     },
     total=False,
 )
 
-
 class ExecuteStatementRequestTypeDef(
     _RequiredExecuteStatementRequestTypeDef, _OptionalExecuteStatementRequestTypeDef
 ):
     pass
 
+PageTypeDef = TypedDict(
+    "PageTypeDef",
+    {
+        "Values": List[ValueHolderTypeDef],
+        "NextPageToken": str,
+    },
+    total=False,
+)
+
+SendCommandRequestRequestTypeDef = TypedDict(
+    "SendCommandRequestRequestTypeDef",
+    {
+        "SessionToken": str,
+        "StartSession": StartSessionRequestTypeDef,
+        "StartTransaction": Mapping[str, Any],
+        "EndSession": Mapping[str, Any],
+        "CommitTransaction": CommitTransactionRequestTypeDef,
+        "AbortTransaction": Mapping[str, Any],
+        "ExecuteStatement": ExecuteStatementRequestTypeDef,
+        "FetchPage": FetchPageRequestTypeDef,
+    },
+    total=False,
+)
 
 ExecuteStatementResultTypeDef = TypedDict(
     "ExecuteStatementResultTypeDef",
     {
         "FirstPage": PageTypeDef,
         "TimingInformation": TimingInformationTypeDef,
         "ConsumedIOs": IOUsageTypeDef,
@@ -207,29 +209,14 @@
         "Page": PageTypeDef,
         "TimingInformation": TimingInformationTypeDef,
         "ConsumedIOs": IOUsageTypeDef,
     },
     total=False,
 )
 
-SendCommandRequestRequestTypeDef = TypedDict(
-    "SendCommandRequestRequestTypeDef",
-    {
-        "SessionToken": str,
-        "StartSession": StartSessionRequestTypeDef,
-        "StartTransaction": Mapping[str, Any],
-        "EndSession": Mapping[str, Any],
-        "CommitTransaction": CommitTransactionRequestTypeDef,
-        "AbortTransaction": Mapping[str, Any],
-        "ExecuteStatement": ExecuteStatementRequestTypeDef,
-        "FetchPage": FetchPageRequestTypeDef,
-    },
-    total=False,
-)
-
 SendCommandResultTypeDef = TypedDict(
     "SendCommandResultTypeDef",
     {
         "StartSession": StartSessionResultTypeDef,
         "StartTransaction": StartTransactionResultTypeDef,
         "EndSession": EndSessionResultTypeDef,
         "CommitTransaction": CommitTransactionResultTypeDef,
```

### Comparing `types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session/type_defs.pyi` & `types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,34 +17,34 @@
 from aiobotocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TimingInformationTypeDef",
     "BlobTypeDef",
     "IOUsageTypeDef",
     "FetchPageRequestTypeDef",
-    "ValueHolderOutputTypeDef",
     "ResponseMetadataTypeDef",
     "StartSessionRequestTypeDef",
     "AbortTransactionResultTypeDef",
     "EndSessionResultTypeDef",
     "StartSessionResultTypeDef",
     "StartTransactionResultTypeDef",
     "CommitTransactionRequestTypeDef",
     "ValueHolderTypeDef",
     "CommitTransactionResultTypeDef",
-    "PageTypeDef",
     "ExecuteStatementRequestTypeDef",
+    "PageTypeDef",
+    "SendCommandRequestRequestTypeDef",
     "ExecuteStatementResultTypeDef",
     "FetchPageResultTypeDef",
-    "SendCommandRequestRequestTypeDef",
     "SendCommandResultTypeDef",
 )
 
 TimingInformationTypeDef = TypedDict(
     "TimingInformationTypeDef",
     {
         "ProcessingTimeMilliseconds": int,
@@ -66,23 +66,14 @@
     "FetchPageRequestTypeDef",
     {
         "TransactionId": str,
         "NextPageToken": str,
     },
 )
 
-ValueHolderOutputTypeDef = TypedDict(
-    "ValueHolderOutputTypeDef",
-    {
-        "IonBinary": bytes,
-        "IonText": str,
-    },
-    total=False,
-)
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -155,23 +146,14 @@
         "CommitDigest": bytes,
         "TimingInformation": TimingInformationTypeDef,
         "ConsumedIOs": IOUsageTypeDef,
     },
     total=False,
 )
 
-PageTypeDef = TypedDict(
-    "PageTypeDef",
-    {
-        "Values": List[ValueHolderOutputTypeDef],
-        "NextPageToken": str,
-    },
-    total=False,
-)
-
 _RequiredExecuteStatementRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementRequestTypeDef",
     {
         "TransactionId": str,
         "Statement": str,
     },
 )
@@ -179,35 +161,26 @@
     "_OptionalExecuteStatementRequestTypeDef",
     {
         "Parameters": Sequence[ValueHolderTypeDef],
     },
     total=False,
 )
 
+
 class ExecuteStatementRequestTypeDef(
     _RequiredExecuteStatementRequestTypeDef, _OptionalExecuteStatementRequestTypeDef
 ):
     pass
 
-ExecuteStatementResultTypeDef = TypedDict(
-    "ExecuteStatementResultTypeDef",
-    {
-        "FirstPage": PageTypeDef,
-        "TimingInformation": TimingInformationTypeDef,
-        "ConsumedIOs": IOUsageTypeDef,
-    },
-    total=False,
-)
 
-FetchPageResultTypeDef = TypedDict(
-    "FetchPageResultTypeDef",
+PageTypeDef = TypedDict(
+    "PageTypeDef",
     {
-        "Page": PageTypeDef,
-        "TimingInformation": TimingInformationTypeDef,
-        "ConsumedIOs": IOUsageTypeDef,
+        "Values": List[ValueHolderTypeDef],
+        "NextPageToken": str,
     },
     total=False,
 )
 
 SendCommandRequestRequestTypeDef = TypedDict(
     "SendCommandRequestRequestTypeDef",
     {
@@ -219,14 +192,34 @@
         "AbortTransaction": Mapping[str, Any],
         "ExecuteStatement": ExecuteStatementRequestTypeDef,
         "FetchPage": FetchPageRequestTypeDef,
     },
     total=False,
 )
 
+ExecuteStatementResultTypeDef = TypedDict(
+    "ExecuteStatementResultTypeDef",
+    {
+        "FirstPage": PageTypeDef,
+        "TimingInformation": TimingInformationTypeDef,
+        "ConsumedIOs": IOUsageTypeDef,
+    },
+    total=False,
+)
+
+FetchPageResultTypeDef = TypedDict(
+    "FetchPageResultTypeDef",
+    {
+        "Page": PageTypeDef,
+        "TimingInformation": TimingInformationTypeDef,
+        "ConsumedIOs": IOUsageTypeDef,
+    },
+    total=False,
+)
+
 SendCommandResultTypeDef = TypedDict(
     "SendCommandResultTypeDef",
     {
         "StartSession": StartSessionResultTypeDef,
         "StartTransaction": StartTransactionResultTypeDef,
         "EndSession": EndSessionResultTypeDef,
         "CommitTransaction": CommitTransactionResultTypeDef,
```

### Comparing `types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session.egg-info/PKG-INFO` & `types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-qldb-session
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.QLDBSession 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.QLDBSession 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb_session/
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
 [types-aiobotocore-qldb-session docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb_session/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,57 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_qldb_session.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `QLDBSession` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb_session/literals/).
+
 ```python
-from types_aiobotocore_qldb_session.literals import (
-    QLDBSessionServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_qldb_session.literals import QLDBSessionServiceName
 
 
 def check_value(value: QLDBSessionServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_qldb_session.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `QLDBSession` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_qldb_session/type_defs/).
+
 ```python
-from types_aiobotocore_qldb_session.type_defs import (
-    TimingInformationTypeDef,
-    BlobTypeDef,
-    IOUsageTypeDef,
-    FetchPageRequestTypeDef,
-    ValueHolderOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartSessionRequestTypeDef,
-    AbortTransactionResultTypeDef,
-    EndSessionResultTypeDef,
-    StartSessionResultTypeDef,
-    StartTransactionResultTypeDef,
-    CommitTransactionRequestTypeDef,
-    ValueHolderTypeDef,
-    CommitTransactionResultTypeDef,
-    PageTypeDef,
-    ExecuteStatementRequestTypeDef,
-    ExecuteStatementResultTypeDef,
-    FetchPageResultTypeDef,
-    SendCommandRequestRequestTypeDef,
-    SendCommandResultTypeDef,
-)
+from types_aiobotocore_qldb_session.type_defs import TimingInformationTypeDef
 
 
 def get_value() -> TimingInformationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-qldb-session-2.5.2.post1/types_aiobotocore_qldb_session.egg-info/SOURCES.txt` & `types-aiobotocore-qldb-session-2.5.2.post2/types_aiobotocore_qldb_session.egg-info/SOURCES.txt`

 * *Files identical despite different names*

