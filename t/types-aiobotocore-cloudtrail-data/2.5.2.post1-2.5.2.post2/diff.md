# Comparing `tmp/types-aiobotocore-cloudtrail-data-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cloudtrail-data-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudtrail-data-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudtrail-data-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:35 2023, max compression
```

## Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1.tar` & `types-aiobotocore-cloudtrail-data-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.201627 types-aiobotocore-cloudtrail-data-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-08-02 14:52:02.201627 types-aiobotocore-cloudtrail-data-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11054 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.201627 types-aiobotocore-cloudtrail-data-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.201627 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-08-02 14:34:47.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-02 14:34:47.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-08-02 14:34:47.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.201627 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:35.823509 types-aiobotocore-cloudtrail-data-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-08-04 12:00:35.823509 types-aiobotocore-cloudtrail-data-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11152 2023-08-04 11:42:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:35.823509 types-aiobotocore-cloudtrail-data-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-04 11:42:01.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:35.823509 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-04 11:42:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-08-04 11:42:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-04 11:42:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-08-04 11:42:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-08-04 11:42:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-08-04 11:42:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-08-04 11:42:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-04 11:42:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2414 2023-08-04 11:42:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:02.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:35.823509 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-08-04 12:00:35.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:00:35.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:35.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:35.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:35.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-04 12:00:35.000000 types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/LICENSE` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/PKG-INFO` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudtrail-data
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CloudTrailDataService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudTrailDataService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/
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
 [types-aiobotocore-cloudtrail-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,43 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloudtrail_data.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CloudTrailDataService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/literals/).
+
 ```python
-from types_aiobotocore_cloudtrail_data.literals import (
-    CloudTrailDataServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_cloudtrail_data.literals import CloudTrailDataServiceServiceName
 
 
 def check_value(value: CloudTrailDataServiceServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloudtrail_data.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudTrailDataService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/type_defs/).
+
 ```python
-from types_aiobotocore_cloudtrail_data.type_defs import (
-    AuditEventResultEntryTypeDef,
-    AuditEventTypeDef,
-    ResponseMetadataTypeDef,
-    ResultErrorEntryTypeDef,
-    PutAuditEventsRequestRequestTypeDef,
-    PutAuditEventsResponseTypeDef,
-)
+from types_aiobotocore_cloudtrail_data.type_defs import AuditEventResultEntryTypeDef
 
 
 def get_value() -> AuditEventResultEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/README.md` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/README.md`

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
 [types-aiobotocore-cloudtrail-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,43 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloudtrail_data.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CloudTrailDataService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/literals/).
+
 ```python
-from types_aiobotocore_cloudtrail_data.literals import (
-    CloudTrailDataServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_cloudtrail_data.literals import CloudTrailDataServiceServiceName
 
 
 def check_value(value: CloudTrailDataServiceServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloudtrail_data.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudTrailDataService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/type_defs/).
+
 ```python
-from types_aiobotocore_cloudtrail_data.type_defs import (
-    AuditEventResultEntryTypeDef,
-    AuditEventTypeDef,
-    ResponseMetadataTypeDef,
-    ResultErrorEntryTypeDef,
-    PutAuditEventsRequestRequestTypeDef,
-    PutAuditEventsResponseTypeDef,
-)
+from types_aiobotocore_cloudtrail_data.type_defs import AuditEventResultEntryTypeDef
 
 
 def get_value() -> AuditEventResultEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/setup.py` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudtrail-data",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cloudtrail_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudTrailDataService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/__init__.py` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/__init__.pyi` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/__main__.py` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CloudTrailDataService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail-data.html#CloudTrailDataService\nOther"
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

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/client.py` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/client.pyi` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/literals.py` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/literals.pyi` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/type_defs.py` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data/type_defs.pyi` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/PKG-INFO` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudtrail-data
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CloudTrailDataService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CloudTrailDataService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/
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
 [types-aiobotocore-cloudtrail-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,43 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cloudtrail_data.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `CloudTrailDataService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/literals/).
+
 ```python
-from types_aiobotocore_cloudtrail_data.literals import (
-    CloudTrailDataServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_cloudtrail_data.literals import CloudTrailDataServiceServiceName
 
 
 def check_value(value: CloudTrailDataServiceServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cloudtrail_data.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CloudTrailDataService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail_data/type_defs/).
+
 ```python
-from types_aiobotocore_cloudtrail_data.type_defs import (
-    AuditEventResultEntryTypeDef,
-    AuditEventTypeDef,
-    ResponseMetadataTypeDef,
-    ResultErrorEntryTypeDef,
-    PutAuditEventsRequestRequestTypeDef,
-    PutAuditEventsResponseTypeDef,
-)
+from types_aiobotocore_cloudtrail_data.type_defs import AuditEventResultEntryTypeDef
 
 
 def get_value() -> AuditEventResultEntryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cloudtrail-data-2.5.2.post1/types_aiobotocore_cloudtrail_data.egg-info/SOURCES.txt` & `types-aiobotocore-cloudtrail-data-2.5.2.post2/types_aiobotocore_cloudtrail_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

