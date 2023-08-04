# Comparing `tmp/types-aiobotocore-apigatewaymanagementapi-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-apigatewaymanagementapi-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-apigatewaymanagementapi-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-apigatewaymanagementapi-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:22 2023, max compression
```

## Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1.tar` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.445660 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-08-02 14:51:50.445660 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.445660 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.437660 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.445660 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.759005 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:08.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-08-04 12:00:22.759005 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11466 2023-08-04 11:40:08.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:22.763005 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-04 11:40:08.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.751004 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-04 11:40:08.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-04 11:40:08.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-04 11:40:08.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-08-04 11:40:08.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-08-04 11:40:08.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-08-04 11:40:09.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-08-04 11:40:09.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:08.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-04 11:40:09.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-08-04 11:40:09.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:08.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.759005 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-08-04 12:00:22.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-04 12:00:22.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:22.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-04 12:00:22.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/LICENSE` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/PKG-INFO` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigatewaymanagementapi
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ApiGatewayManagementApi 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ApiGatewayManagementApi 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/
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
 [types-aiobotocore-apigatewaymanagementapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,45 +266,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_apigatewaymanagementapi.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ApiGatewayManagementApi` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/literals/).
+
 ```python
-from types_aiobotocore_apigatewaymanagementapi.literals import (
-    ApiGatewayManagementApiServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_apigatewaymanagementapi.literals import ApiGatewayManagementApiServiceName
 
 
 def check_value(value: ApiGatewayManagementApiServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_apigatewaymanagementapi.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `ApiGatewayManagementApi` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/type_defs/).
+
 ```python
-from types_aiobotocore_apigatewaymanagementapi.type_defs import (
-    BlobTypeDef,
-    DeleteConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetConnectionRequestRequestTypeDef,
-    IdentityTypeDef,
-    PostToConnectionRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetConnectionResponseTypeDef,
-)
+from types_aiobotocore_apigatewaymanagementapi.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/README.md` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/README.md`

 * *Files 4% similar despite different names*

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
 [types-aiobotocore-apigatewaymanagementapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,45 +234,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_apigatewaymanagementapi.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ApiGatewayManagementApi` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/literals/).
+
 ```python
-from types_aiobotocore_apigatewaymanagementapi.literals import (
-    ApiGatewayManagementApiServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_apigatewaymanagementapi.literals import ApiGatewayManagementApiServiceName
 
 
 def check_value(value: ApiGatewayManagementApiServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_apigatewaymanagementapi.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `ApiGatewayManagementApi` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/type_defs/).
+
 ```python
-from types_aiobotocore_apigatewaymanagementapi.type_defs import (
-    BlobTypeDef,
-    DeleteConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetConnectionRequestRequestTypeDef,
-    IdentityTypeDef,
-    PostToConnectionRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetConnectionResponseTypeDef,
-)
+from types_aiobotocore_apigatewaymanagementapi.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/setup.py` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-apigatewaymanagementapi",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_apigatewaymanagementapi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ApiGatewayManagementApi 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/__init__.py` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/__init__.pyi` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/__main__.py` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ApiGatewayManagementApi 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi\nOther"
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

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/client.py` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/client.pyi` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/literals.py` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/literals.pyi` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/type_defs.py` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/type_defs.pyi` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/PKG-INFO` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigatewaymanagementapi
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ApiGatewayManagementApi 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ApiGatewayManagementApi 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/
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
 [types-aiobotocore-apigatewaymanagementapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,45 +266,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_apigatewaymanagementapi.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ApiGatewayManagementApi` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/literals/).
+
 ```python
-from types_aiobotocore_apigatewaymanagementapi.literals import (
-    ApiGatewayManagementApiServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_apigatewaymanagementapi.literals import ApiGatewayManagementApiServiceName
 
 
 def check_value(value: ApiGatewayManagementApiServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_apigatewaymanagementapi.type_defs` module contains
 structures and shapes assembled to typed dictionaries and unions for additional
 type checking.
 
+Full list of `ApiGatewayManagementApi` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/type_defs/).
+
 ```python
-from types_aiobotocore_apigatewaymanagementapi.type_defs import (
-    BlobTypeDef,
-    DeleteConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    GetConnectionRequestRequestTypeDef,
-    IdentityTypeDef,
-    PostToConnectionRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetConnectionResponseTypeDef,
-)
+from types_aiobotocore_apigatewaymanagementapi.type_defs import BlobTypeDef
 
 
 def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/SOURCES.txt` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post2/types_aiobotocore_apigatewaymanagementapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

