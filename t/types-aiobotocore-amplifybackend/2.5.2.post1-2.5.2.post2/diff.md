# Comparing `tmp/types-aiobotocore-amplifybackend-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-amplifybackend-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-amplifybackend-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-amplifybackend-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:19 2023, max compression
```

## Comparing `types-aiobotocore-amplifybackend-2.5.2.post1.tar` & `types-aiobotocore-amplifybackend-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.841667 types-aiobotocore-amplifybackend-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17946 2023-08-02 14:51:47.841667 types-aiobotocore-amplifybackend-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16400 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:47.841667 types-aiobotocore-amplifybackend-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.837667 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24833 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24792 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    44462 2023-08-02 14:32:53.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    44397 2023-08-02 14:32:52.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:51.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.841667 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17946 2023-08-02 14:51:47.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:51:47.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:47.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:51:47.000000 types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.742887 types-aiobotocore-amplifybackend-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-08-04 12:00:19.738887 types-aiobotocore-amplifybackend-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:19.742887 types-aiobotocore-amplifybackend-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.734887 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24798 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24757 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9923 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    38956 2023-08-04 11:39:59.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38903 2023-08-04 11:39:58.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:39:57.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.738887 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13390 2023-08-04 12:00:19.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-04 12:00:19.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:19.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-04 12:00:19.000000 types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/LICENSE` & `types-aiobotocore-amplifybackend-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/setup.py` & `types-aiobotocore-amplifybackend-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-amplifybackend",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_amplifybackend"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AmplifyBackend 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/__init__.py` & `types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/__init__.pyi` & `types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/__main__.py` & `types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.AmplifyBackend 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend\nOther"
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

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/client.py` & `types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 from typing import Any, Dict, Mapping, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import ListBackendJobsPaginator
 from .type_defs import (
-    BackendAPIResourceConfigUnionTypeDef,
+    BackendAPIResourceConfigTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
-    CreateBackendAuthResourceConfigUnionTypeDef,
+    CreateBackendAuthResourceConfigTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResourceConfigTypeDef,
     CreateBackendStorageResponseTypeDef,
     CreateTokenResponseTypeDef,
     DeleteBackendAPIResponseTypeDef,
@@ -146,30 +146,30 @@
         """
 
     async def create_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: BackendAPIResourceConfigUnionTypeDef,
+        ResourceConfig: BackendAPIResourceConfigTypeDef,
         ResourceName: str
     ) -> CreateBackendAPIResponseTypeDef:
         """
         Creates a new backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_api)
         """
 
     async def create_backend_auth(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: CreateBackendAuthResourceConfigUnionTypeDef,
+        ResourceConfig: CreateBackendAuthResourceConfigTypeDef,
         ResourceName: str
     ) -> CreateBackendAuthResponseTypeDef:
         """
         Creates a new backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_auth)
@@ -221,15 +221,15 @@
 
     async def delete_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
     ) -> DeleteBackendAPIResponseTypeDef:
         """
         Deletes an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.delete_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#delete_backend_api)
         """
@@ -303,15 +303,15 @@
 
     async def get_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
     ) -> GetBackendAPIResponseTypeDef:
         """
         Gets the details for a backend API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.get_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#get_backend_api)
         """
@@ -442,15 +442,15 @@
 
     async def update_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
     ) -> UpdateBackendAPIResponseTypeDef:
         """
         Updates an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#update_backend_api)
         """
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/client.pyi` & `types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 from typing import Any, Dict, Mapping, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .paginator import ListBackendJobsPaginator
 from .type_defs import (
-    BackendAPIResourceConfigUnionTypeDef,
+    BackendAPIResourceConfigTypeDef,
     CloneBackendResponseTypeDef,
     CreateBackendAPIResponseTypeDef,
-    CreateBackendAuthResourceConfigUnionTypeDef,
+    CreateBackendAuthResourceConfigTypeDef,
     CreateBackendAuthResponseTypeDef,
     CreateBackendConfigResponseTypeDef,
     CreateBackendResponseTypeDef,
     CreateBackendStorageResourceConfigTypeDef,
     CreateBackendStorageResponseTypeDef,
     CreateTokenResponseTypeDef,
     DeleteBackendAPIResponseTypeDef,
@@ -137,29 +137,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend)
         """
     async def create_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: BackendAPIResourceConfigUnionTypeDef,
+        ResourceConfig: BackendAPIResourceConfigTypeDef,
         ResourceName: str
     ) -> CreateBackendAPIResponseTypeDef:
         """
         Creates a new backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_api)
         """
     async def create_backend_auth(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
-        ResourceConfig: CreateBackendAuthResourceConfigUnionTypeDef,
+        ResourceConfig: CreateBackendAuthResourceConfigTypeDef,
         ResourceName: str
     ) -> CreateBackendAuthResponseTypeDef:
         """
         Creates a new backend authentication resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.create_backend_auth)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#create_backend_auth)
@@ -206,15 +206,15 @@
         """
     async def delete_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
     ) -> DeleteBackendAPIResponseTypeDef:
         """
         Deletes an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.delete_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#delete_backend_api)
         """
@@ -281,15 +281,15 @@
         """
     async def get_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
     ) -> GetBackendAPIResponseTypeDef:
         """
         Gets the details for a backend API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.get_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#get_backend_api)
         """
@@ -408,15 +408,15 @@
         """
     async def update_backend_api(
         self,
         *,
         AppId: str,
         BackendEnvironmentName: str,
         ResourceName: str,
-        ResourceConfig: BackendAPIResourceConfigUnionTypeDef = ...
+        ResourceConfig: BackendAPIResourceConfigTypeDef = ...
     ) -> UpdateBackendAPIResponseTypeDef:
         """
         Updates an existing backend API resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifybackend.html#AmplifyBackend.Client.update_backend_api)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifybackend/client/#update_backend_api)
         """
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/literals.py` & `types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/literals.pyi` & `types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/paginator.py` & `types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/paginator.pyi` & `types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/type_defs.py` & `types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsTypeDef
 
     data: BackendAPIAppSyncAuthSettingsTypeDef = ...
     ```
 """
 import sys
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AdditionalConstraintsElementType,
     AuthenticatedElementType,
     AuthResourcesType,
     DeliveryMethodType,
     MFAModeType,
@@ -43,24 +43,21 @@
 
 __all__ = (
     "BackendAPIAppSyncAuthSettingsTypeDef",
     "BackendAPIConflictResolutionTypeDef",
     "BackendAuthAppleProviderConfigTypeDef",
     "BackendAuthSocialProviderConfigTypeDef",
     "BackendJobRespObjTypeDef",
-    "BackendStoragePermissionsOutputTypeDef",
     "BackendStoragePermissionsTypeDef",
     "CloneBackendRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EmailSettingsTypeDef",
     "SmsSettingsTypeDef",
     "CreateBackendAuthIdentityPoolConfigTypeDef",
-    "SettingsOutputTypeDef",
     "SettingsTypeDef",
-    "CreateBackendAuthPasswordPolicyConfigOutputTypeDef",
     "CreateBackendAuthPasswordPolicyConfigTypeDef",
     "CreateBackendConfigRequestRequestTypeDef",
     "CreateBackendRequestRequestTypeDef",
     "CreateTokenRequestRequestTypeDef",
     "DeleteBackendAuthRequestRequestTypeDef",
     "DeleteBackendRequestRequestTypeDef",
     "DeleteBackendStorageRequestRequestTypeDef",
@@ -82,16 +79,16 @@
     "RemoveAllBackendsRequestRequestTypeDef",
     "RemoveBackendConfigRequestRequestTypeDef",
     "UpdateBackendAuthIdentityPoolConfigTypeDef",
     "UpdateBackendAuthPasswordPolicyConfigTypeDef",
     "UpdateBackendJobRequestRequestTypeDef",
     "BackendAPIAuthTypeTypeDef",
     "SocialProviderSettingsTypeDef",
-    "GetBackendStorageResourceConfigTypeDef",
     "CreateBackendStorageResourceConfigTypeDef",
+    "GetBackendStorageResourceConfigTypeDef",
     "UpdateBackendStorageResourceConfigTypeDef",
     "CloneBackendResponseTypeDef",
     "CreateBackendAPIResponseTypeDef",
     "CreateBackendAuthResponseTypeDef",
     "CreateBackendConfigResponseTypeDef",
     "CreateBackendResponseTypeDef",
     "CreateBackendStorageResponseTypeDef",
@@ -115,44 +112,37 @@
     "UpdateBackendAuthResponseTypeDef",
     "UpdateBackendJobResponseTypeDef",
     "UpdateBackendStorageResponseTypeDef",
     "CreateBackendAuthForgotPasswordConfigTypeDef",
     "CreateBackendAuthVerificationMessageConfigTypeDef",
     "UpdateBackendAuthForgotPasswordConfigTypeDef",
     "UpdateBackendAuthVerificationMessageConfigTypeDef",
-    "CreateBackendAuthMFAConfigOutputTypeDef",
     "CreateBackendAuthMFAConfigTypeDef",
     "UpdateBackendAuthMFAConfigTypeDef",
     "ListBackendJobsRequestListBackendJobsPaginateTypeDef",
     "ListS3BucketsResponseTypeDef",
     "UpdateBackendConfigRequestRequestTypeDef",
     "UpdateBackendConfigResponseTypeDef",
-    "BackendAPIResourceConfigOutputTypeDef",
     "BackendAPIResourceConfigTypeDef",
-    "CreateBackendAuthOAuthConfigOutputTypeDef",
     "CreateBackendAuthOAuthConfigTypeDef",
     "UpdateBackendAuthOAuthConfigTypeDef",
-    "GetBackendStorageResponseTypeDef",
     "CreateBackendStorageRequestRequestTypeDef",
+    "GetBackendStorageResponseTypeDef",
     "UpdateBackendStorageRequestRequestTypeDef",
-    "GetBackendAPIResponseTypeDef",
-    "BackendAPIResourceConfigUnionTypeDef",
     "CreateBackendAPIRequestRequestTypeDef",
     "DeleteBackendAPIRequestRequestTypeDef",
     "GetBackendAPIRequestRequestTypeDef",
+    "GetBackendAPIResponseTypeDef",
     "UpdateBackendAPIRequestRequestTypeDef",
-    "CreateBackendAuthUserPoolConfigOutputTypeDef",
     "CreateBackendAuthUserPoolConfigTypeDef",
     "UpdateBackendAuthUserPoolConfigTypeDef",
-    "CreateBackendAuthResourceConfigOutputTypeDef",
     "CreateBackendAuthResourceConfigTypeDef",
     "UpdateBackendAuthResourceConfigTypeDef",
-    "GetBackendAuthResponseTypeDef",
     "CreateBackendAuthRequestRequestTypeDef",
-    "CreateBackendAuthResourceConfigUnionTypeDef",
+    "GetBackendAuthResponseTypeDef",
     "UpdateBackendAuthRequestRequestTypeDef",
 )
 
 BackendAPIAppSyncAuthSettingsTypeDef = TypedDict(
     "BackendAPIAppSyncAuthSettingsTypeDef",
     {
         "CognitoUserPoolId": str,
@@ -218,35 +208,14 @@
 
 class BackendJobRespObjTypeDef(
     _RequiredBackendJobRespObjTypeDef, _OptionalBackendJobRespObjTypeDef
 ):
     pass
 
 
-_RequiredBackendStoragePermissionsOutputTypeDef = TypedDict(
-    "_RequiredBackendStoragePermissionsOutputTypeDef",
-    {
-        "Authenticated": List[AuthenticatedElementType],
-    },
-)
-_OptionalBackendStoragePermissionsOutputTypeDef = TypedDict(
-    "_OptionalBackendStoragePermissionsOutputTypeDef",
-    {
-        "UnAuthenticated": List[UnAuthenticatedElementType],
-    },
-    total=False,
-)
-
-
-class BackendStoragePermissionsOutputTypeDef(
-    _RequiredBackendStoragePermissionsOutputTypeDef, _OptionalBackendStoragePermissionsOutputTypeDef
-):
-    pass
-
-
 _RequiredBackendStoragePermissionsTypeDef = TypedDict(
     "_RequiredBackendStoragePermissionsTypeDef",
     {
         "Authenticated": Sequence[AuthenticatedElementType],
     },
 )
 _OptionalBackendStoragePermissionsTypeDef = TypedDict(
@@ -305,54 +274,23 @@
     "CreateBackendAuthIdentityPoolConfigTypeDef",
     {
         "IdentityPoolName": str,
         "UnauthenticatedLogin": bool,
     },
 )
 
-SettingsOutputTypeDef = TypedDict(
-    "SettingsOutputTypeDef",
-    {
-        "MfaTypes": List[MfaTypesElementType],
-        "SmsMessage": str,
-    },
-    total=False,
-)
-
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "MfaTypes": Sequence[MfaTypesElementType],
         "SmsMessage": str,
     },
     total=False,
 )
 
-_RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef",
-    {
-        "MinimumLength": float,
-    },
-)
-_OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef",
-    {
-        "AdditionalConstraints": List[AdditionalConstraintsElementType],
-    },
-    total=False,
-)
-
-
-class CreateBackendAuthPasswordPolicyConfigOutputTypeDef(
-    _RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef,
-    _OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredCreateBackendAuthPasswordPolicyConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthPasswordPolicyConfigTypeDef",
     {
         "MinimumLength": float,
     },
 )
 _OptionalCreateBackendAuthPasswordPolicyConfigTypeDef = TypedDict(
@@ -731,56 +669,56 @@
         "Google": BackendAuthSocialProviderConfigTypeDef,
         "LoginWithAmazon": BackendAuthSocialProviderConfigTypeDef,
         "SignInWithApple": BackendAuthAppleProviderConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredGetBackendStorageResourceConfigTypeDef = TypedDict(
-    "_RequiredGetBackendStorageResourceConfigTypeDef",
+_RequiredCreateBackendStorageResourceConfigTypeDef = TypedDict(
+    "_RequiredCreateBackendStorageResourceConfigTypeDef",
     {
-        "Imported": bool,
+        "Permissions": BackendStoragePermissionsTypeDef,
         "ServiceName": Literal["S3"],
     },
 )
-_OptionalGetBackendStorageResourceConfigTypeDef = TypedDict(
-    "_OptionalGetBackendStorageResourceConfigTypeDef",
+_OptionalCreateBackendStorageResourceConfigTypeDef = TypedDict(
+    "_OptionalCreateBackendStorageResourceConfigTypeDef",
     {
         "BucketName": str,
-        "Permissions": BackendStoragePermissionsOutputTypeDef,
     },
     total=False,
 )
 
 
-class GetBackendStorageResourceConfigTypeDef(
-    _RequiredGetBackendStorageResourceConfigTypeDef, _OptionalGetBackendStorageResourceConfigTypeDef
+class CreateBackendStorageResourceConfigTypeDef(
+    _RequiredCreateBackendStorageResourceConfigTypeDef,
+    _OptionalCreateBackendStorageResourceConfigTypeDef,
 ):
     pass
 
 
-_RequiredCreateBackendStorageResourceConfigTypeDef = TypedDict(
-    "_RequiredCreateBackendStorageResourceConfigTypeDef",
+_RequiredGetBackendStorageResourceConfigTypeDef = TypedDict(
+    "_RequiredGetBackendStorageResourceConfigTypeDef",
     {
-        "Permissions": BackendStoragePermissionsTypeDef,
+        "Imported": bool,
         "ServiceName": Literal["S3"],
     },
 )
-_OptionalCreateBackendStorageResourceConfigTypeDef = TypedDict(
-    "_OptionalCreateBackendStorageResourceConfigTypeDef",
+_OptionalGetBackendStorageResourceConfigTypeDef = TypedDict(
+    "_OptionalGetBackendStorageResourceConfigTypeDef",
     {
         "BucketName": str,
+        "Permissions": BackendStoragePermissionsTypeDef,
     },
     total=False,
 )
 
 
-class CreateBackendStorageResourceConfigTypeDef(
-    _RequiredCreateBackendStorageResourceConfigTypeDef,
-    _OptionalCreateBackendStorageResourceConfigTypeDef,
+class GetBackendStorageResourceConfigTypeDef(
+    _RequiredGetBackendStorageResourceConfigTypeDef, _OptionalGetBackendStorageResourceConfigTypeDef
 ):
     pass
 
 
 UpdateBackendStorageResourceConfigTypeDef = TypedDict(
     "UpdateBackendStorageResourceConfigTypeDef",
     {
@@ -1175,36 +1113,14 @@
 class UpdateBackendAuthVerificationMessageConfigTypeDef(
     _RequiredUpdateBackendAuthVerificationMessageConfigTypeDef,
     _OptionalUpdateBackendAuthVerificationMessageConfigTypeDef,
 ):
     pass
 
 
-_RequiredCreateBackendAuthMFAConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthMFAConfigOutputTypeDef",
-    {
-        "MFAMode": MFAModeType,
-    },
-)
-_OptionalCreateBackendAuthMFAConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthMFAConfigOutputTypeDef",
-    {
-        "Settings": SettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateBackendAuthMFAConfigOutputTypeDef(
-    _RequiredCreateBackendAuthMFAConfigOutputTypeDef,
-    _OptionalCreateBackendAuthMFAConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredCreateBackendAuthMFAConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthMFAConfigTypeDef",
     {
         "MFAMode": MFAModeType,
     },
 )
 _OptionalCreateBackendAuthMFAConfigTypeDef = TypedDict(
@@ -1295,66 +1211,27 @@
         "BackendManagerAppId": str,
         "Error": str,
         "LoginAuthConfig": LoginAuthConfigReqObjTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BackendAPIResourceConfigOutputTypeDef = TypedDict(
-    "BackendAPIResourceConfigOutputTypeDef",
-    {
-        "AdditionalAuthTypes": List[BackendAPIAuthTypeTypeDef],
-        "ApiName": str,
-        "ConflictResolution": BackendAPIConflictResolutionTypeDef,
-        "DefaultAuthType": BackendAPIAuthTypeTypeDef,
-        "Service": str,
-        "TransformSchema": str,
-    },
-    total=False,
-)
-
 BackendAPIResourceConfigTypeDef = TypedDict(
     "BackendAPIResourceConfigTypeDef",
     {
         "AdditionalAuthTypes": Sequence[BackendAPIAuthTypeTypeDef],
         "ApiName": str,
         "ConflictResolution": BackendAPIConflictResolutionTypeDef,
         "DefaultAuthType": BackendAPIAuthTypeTypeDef,
         "Service": str,
         "TransformSchema": str,
     },
     total=False,
 )
 
-_RequiredCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthOAuthConfigOutputTypeDef",
-    {
-        "OAuthGrantType": OAuthGrantTypeType,
-        "OAuthScopes": List[OAuthScopesElementType],
-        "RedirectSignInURIs": List[str],
-        "RedirectSignOutURIs": List[str],
-    },
-)
-_OptionalCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthOAuthConfigOutputTypeDef",
-    {
-        "DomainPrefix": str,
-        "SocialProviderSettings": SocialProviderSettingsTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateBackendAuthOAuthConfigOutputTypeDef(
-    _RequiredCreateBackendAuthOAuthConfigOutputTypeDef,
-    _OptionalCreateBackendAuthOAuthConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredCreateBackendAuthOAuthConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthOAuthConfigTypeDef",
     {
         "OAuthGrantType": OAuthGrantTypeType,
         "OAuthScopes": Sequence[OAuthScopesElementType],
         "RedirectSignInURIs": Sequence[str],
         "RedirectSignOutURIs": Sequence[str],
@@ -1385,60 +1262,45 @@
         "RedirectSignInURIs": Sequence[str],
         "RedirectSignOutURIs": Sequence[str],
         "SocialProviderSettings": SocialProviderSettingsTypeDef,
     },
     total=False,
 )
 
-GetBackendStorageResponseTypeDef = TypedDict(
-    "GetBackendStorageResponseTypeDef",
-    {
-        "AppId": str,
-        "BackendEnvironmentName": str,
-        "ResourceConfig": GetBackendStorageResourceConfigTypeDef,
-        "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateBackendStorageRequestRequestTypeDef = TypedDict(
     "CreateBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": CreateBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
     },
 )
 
-UpdateBackendStorageRequestRequestTypeDef = TypedDict(
-    "UpdateBackendStorageRequestRequestTypeDef",
+GetBackendStorageResponseTypeDef = TypedDict(
+    "GetBackendStorageResponseTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": UpdateBackendStorageResourceConfigTypeDef,
+        "ResourceConfig": GetBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBackendAPIResponseTypeDef = TypedDict(
-    "GetBackendAPIResponseTypeDef",
+UpdateBackendStorageRequestRequestTypeDef = TypedDict(
+    "UpdateBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "Error": str,
-        "ResourceConfig": BackendAPIResourceConfigOutputTypeDef,
+        "ResourceConfig": UpdateBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BackendAPIResourceConfigUnionTypeDef = Union[
-    BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
-]
 CreateBackendAPIRequestRequestTypeDef = TypedDict(
     "CreateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
         "ResourceName": str,
@@ -1487,14 +1349,26 @@
 
 class GetBackendAPIRequestRequestTypeDef(
     _RequiredGetBackendAPIRequestRequestTypeDef, _OptionalGetBackendAPIRequestRequestTypeDef
 ):
     pass
 
 
+GetBackendAPIResponseTypeDef = TypedDict(
+    "GetBackendAPIResponseTypeDef",
+    {
+        "AppId": str,
+        "BackendEnvironmentName": str,
+        "Error": str,
+        "ResourceConfig": BackendAPIResourceConfigTypeDef,
+        "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateBackendAPIRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceName": str,
     },
@@ -1510,42 +1384,14 @@
 
 class UpdateBackendAPIRequestRequestTypeDef(
     _RequiredUpdateBackendAPIRequestRequestTypeDef, _OptionalUpdateBackendAPIRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthUserPoolConfigOutputTypeDef",
-    {
-        "RequiredSignUpAttributes": List[RequiredSignUpAttributesElementType],
-        "SignInMethod": SignInMethodType,
-        "UserPoolName": str,
-    },
-)
-_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef",
-    {
-        "ForgotPassword": CreateBackendAuthForgotPasswordConfigTypeDef,
-        "Mfa": CreateBackendAuthMFAConfigOutputTypeDef,
-        "OAuth": CreateBackendAuthOAuthConfigOutputTypeDef,
-        "PasswordPolicy": CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
-        "VerificationMessage": CreateBackendAuthVerificationMessageConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateBackendAuthUserPoolConfigOutputTypeDef(
-    _RequiredCreateBackendAuthUserPoolConfigOutputTypeDef,
-    _OptionalCreateBackendAuthUserPoolConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredCreateBackendAuthUserPoolConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthUserPoolConfigTypeDef",
     {
         "RequiredSignUpAttributes": Sequence[RequiredSignUpAttributesElementType],
         "SignInMethod": SignInMethodType,
         "UserPoolName": str,
     },
@@ -1577,38 +1423,14 @@
         "OAuth": UpdateBackendAuthOAuthConfigTypeDef,
         "PasswordPolicy": UpdateBackendAuthPasswordPolicyConfigTypeDef,
         "VerificationMessage": UpdateBackendAuthVerificationMessageConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthResourceConfigOutputTypeDef",
-    {
-        "AuthResources": AuthResourcesType,
-        "Service": Literal["COGNITO"],
-        "UserPoolConfigs": CreateBackendAuthUserPoolConfigOutputTypeDef,
-    },
-)
-_OptionalCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthResourceConfigOutputTypeDef",
-    {
-        "IdentityPoolConfigs": CreateBackendAuthIdentityPoolConfigTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateBackendAuthResourceConfigOutputTypeDef(
-    _RequiredCreateBackendAuthResourceConfigOutputTypeDef,
-    _OptionalCreateBackendAuthResourceConfigOutputTypeDef,
-):
-    pass
-
-
 _RequiredCreateBackendAuthResourceConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthResourceConfigTypeDef",
     {
         "AuthResources": AuthResourcesType,
         "Service": Literal["COGNITO"],
         "UserPoolConfigs": CreateBackendAuthUserPoolConfigTypeDef,
     },
@@ -1647,39 +1469,36 @@
 
 class UpdateBackendAuthResourceConfigTypeDef(
     _RequiredUpdateBackendAuthResourceConfigTypeDef, _OptionalUpdateBackendAuthResourceConfigTypeDef
 ):
     pass
 
 
-GetBackendAuthResponseTypeDef = TypedDict(
-    "GetBackendAuthResponseTypeDef",
+CreateBackendAuthRequestRequestTypeDef = TypedDict(
+    "CreateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "Error": str,
-        "ResourceConfig": CreateBackendAuthResourceConfigOutputTypeDef,
+        "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateBackendAuthRequestRequestTypeDef = TypedDict(
-    "CreateBackendAuthRequestRequestTypeDef",
+GetBackendAuthResponseTypeDef = TypedDict(
+    "GetBackendAuthResponseTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
+        "Error": str,
         "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateBackendAuthResourceConfigUnionTypeDef = Union[
-    CreateBackendAuthResourceConfigTypeDef, CreateBackendAuthResourceConfigOutputTypeDef
-]
 UpdateBackendAuthRequestRequestTypeDef = TypedDict(
     "UpdateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": UpdateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend/type_defs.pyi` & `types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     ```python
     from types_aiobotocore_amplifybackend.type_defs import BackendAPIAppSyncAuthSettingsTypeDef
 
     data: BackendAPIAppSyncAuthSettingsTypeDef = ...
     ```
 """
 import sys
-from typing import Any, Dict, List, Mapping, Sequence, Union
+from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import (
     AdditionalConstraintsElementType,
     AuthenticatedElementType,
     AuthResourcesType,
     DeliveryMethodType,
     MFAModeType,
@@ -42,24 +42,21 @@
 
 __all__ = (
     "BackendAPIAppSyncAuthSettingsTypeDef",
     "BackendAPIConflictResolutionTypeDef",
     "BackendAuthAppleProviderConfigTypeDef",
     "BackendAuthSocialProviderConfigTypeDef",
     "BackendJobRespObjTypeDef",
-    "BackendStoragePermissionsOutputTypeDef",
     "BackendStoragePermissionsTypeDef",
     "CloneBackendRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "EmailSettingsTypeDef",
     "SmsSettingsTypeDef",
     "CreateBackendAuthIdentityPoolConfigTypeDef",
-    "SettingsOutputTypeDef",
     "SettingsTypeDef",
-    "CreateBackendAuthPasswordPolicyConfigOutputTypeDef",
     "CreateBackendAuthPasswordPolicyConfigTypeDef",
     "CreateBackendConfigRequestRequestTypeDef",
     "CreateBackendRequestRequestTypeDef",
     "CreateTokenRequestRequestTypeDef",
     "DeleteBackendAuthRequestRequestTypeDef",
     "DeleteBackendRequestRequestTypeDef",
     "DeleteBackendStorageRequestRequestTypeDef",
@@ -81,16 +78,16 @@
     "RemoveAllBackendsRequestRequestTypeDef",
     "RemoveBackendConfigRequestRequestTypeDef",
     "UpdateBackendAuthIdentityPoolConfigTypeDef",
     "UpdateBackendAuthPasswordPolicyConfigTypeDef",
     "UpdateBackendJobRequestRequestTypeDef",
     "BackendAPIAuthTypeTypeDef",
     "SocialProviderSettingsTypeDef",
-    "GetBackendStorageResourceConfigTypeDef",
     "CreateBackendStorageResourceConfigTypeDef",
+    "GetBackendStorageResourceConfigTypeDef",
     "UpdateBackendStorageResourceConfigTypeDef",
     "CloneBackendResponseTypeDef",
     "CreateBackendAPIResponseTypeDef",
     "CreateBackendAuthResponseTypeDef",
     "CreateBackendConfigResponseTypeDef",
     "CreateBackendResponseTypeDef",
     "CreateBackendStorageResponseTypeDef",
@@ -114,44 +111,37 @@
     "UpdateBackendAuthResponseTypeDef",
     "UpdateBackendJobResponseTypeDef",
     "UpdateBackendStorageResponseTypeDef",
     "CreateBackendAuthForgotPasswordConfigTypeDef",
     "CreateBackendAuthVerificationMessageConfigTypeDef",
     "UpdateBackendAuthForgotPasswordConfigTypeDef",
     "UpdateBackendAuthVerificationMessageConfigTypeDef",
-    "CreateBackendAuthMFAConfigOutputTypeDef",
     "CreateBackendAuthMFAConfigTypeDef",
     "UpdateBackendAuthMFAConfigTypeDef",
     "ListBackendJobsRequestListBackendJobsPaginateTypeDef",
     "ListS3BucketsResponseTypeDef",
     "UpdateBackendConfigRequestRequestTypeDef",
     "UpdateBackendConfigResponseTypeDef",
-    "BackendAPIResourceConfigOutputTypeDef",
     "BackendAPIResourceConfigTypeDef",
-    "CreateBackendAuthOAuthConfigOutputTypeDef",
     "CreateBackendAuthOAuthConfigTypeDef",
     "UpdateBackendAuthOAuthConfigTypeDef",
-    "GetBackendStorageResponseTypeDef",
     "CreateBackendStorageRequestRequestTypeDef",
+    "GetBackendStorageResponseTypeDef",
     "UpdateBackendStorageRequestRequestTypeDef",
-    "GetBackendAPIResponseTypeDef",
-    "BackendAPIResourceConfigUnionTypeDef",
     "CreateBackendAPIRequestRequestTypeDef",
     "DeleteBackendAPIRequestRequestTypeDef",
     "GetBackendAPIRequestRequestTypeDef",
+    "GetBackendAPIResponseTypeDef",
     "UpdateBackendAPIRequestRequestTypeDef",
-    "CreateBackendAuthUserPoolConfigOutputTypeDef",
     "CreateBackendAuthUserPoolConfigTypeDef",
     "UpdateBackendAuthUserPoolConfigTypeDef",
-    "CreateBackendAuthResourceConfigOutputTypeDef",
     "CreateBackendAuthResourceConfigTypeDef",
     "UpdateBackendAuthResourceConfigTypeDef",
-    "GetBackendAuthResponseTypeDef",
     "CreateBackendAuthRequestRequestTypeDef",
-    "CreateBackendAuthResourceConfigUnionTypeDef",
+    "GetBackendAuthResponseTypeDef",
     "UpdateBackendAuthRequestRequestTypeDef",
 )
 
 BackendAPIAppSyncAuthSettingsTypeDef = TypedDict(
     "BackendAPIAppSyncAuthSettingsTypeDef",
     {
         "CognitoUserPoolId": str,
@@ -215,33 +205,14 @@
 )
 
 class BackendJobRespObjTypeDef(
     _RequiredBackendJobRespObjTypeDef, _OptionalBackendJobRespObjTypeDef
 ):
     pass
 
-_RequiredBackendStoragePermissionsOutputTypeDef = TypedDict(
-    "_RequiredBackendStoragePermissionsOutputTypeDef",
-    {
-        "Authenticated": List[AuthenticatedElementType],
-    },
-)
-_OptionalBackendStoragePermissionsOutputTypeDef = TypedDict(
-    "_OptionalBackendStoragePermissionsOutputTypeDef",
-    {
-        "UnAuthenticated": List[UnAuthenticatedElementType],
-    },
-    total=False,
-)
-
-class BackendStoragePermissionsOutputTypeDef(
-    _RequiredBackendStoragePermissionsOutputTypeDef, _OptionalBackendStoragePermissionsOutputTypeDef
-):
-    pass
-
 _RequiredBackendStoragePermissionsTypeDef = TypedDict(
     "_RequiredBackendStoragePermissionsTypeDef",
     {
         "Authenticated": Sequence[AuthenticatedElementType],
     },
 )
 _OptionalBackendStoragePermissionsTypeDef = TypedDict(
@@ -298,52 +269,23 @@
     "CreateBackendAuthIdentityPoolConfigTypeDef",
     {
         "IdentityPoolName": str,
         "UnauthenticatedLogin": bool,
     },
 )
 
-SettingsOutputTypeDef = TypedDict(
-    "SettingsOutputTypeDef",
-    {
-        "MfaTypes": List[MfaTypesElementType],
-        "SmsMessage": str,
-    },
-    total=False,
-)
-
 SettingsTypeDef = TypedDict(
     "SettingsTypeDef",
     {
         "MfaTypes": Sequence[MfaTypesElementType],
         "SmsMessage": str,
     },
     total=False,
 )
 
-_RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef",
-    {
-        "MinimumLength": float,
-    },
-)
-_OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef",
-    {
-        "AdditionalConstraints": List[AdditionalConstraintsElementType],
-    },
-    total=False,
-)
-
-class CreateBackendAuthPasswordPolicyConfigOutputTypeDef(
-    _RequiredCreateBackendAuthPasswordPolicyConfigOutputTypeDef,
-    _OptionalCreateBackendAuthPasswordPolicyConfigOutputTypeDef,
-):
-    pass
-
 _RequiredCreateBackendAuthPasswordPolicyConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthPasswordPolicyConfigTypeDef",
     {
         "MinimumLength": float,
     },
 )
 _OptionalCreateBackendAuthPasswordPolicyConfigTypeDef = TypedDict(
@@ -704,53 +646,53 @@
         "Google": BackendAuthSocialProviderConfigTypeDef,
         "LoginWithAmazon": BackendAuthSocialProviderConfigTypeDef,
         "SignInWithApple": BackendAuthAppleProviderConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredGetBackendStorageResourceConfigTypeDef = TypedDict(
-    "_RequiredGetBackendStorageResourceConfigTypeDef",
+_RequiredCreateBackendStorageResourceConfigTypeDef = TypedDict(
+    "_RequiredCreateBackendStorageResourceConfigTypeDef",
     {
-        "Imported": bool,
+        "Permissions": BackendStoragePermissionsTypeDef,
         "ServiceName": Literal["S3"],
     },
 )
-_OptionalGetBackendStorageResourceConfigTypeDef = TypedDict(
-    "_OptionalGetBackendStorageResourceConfigTypeDef",
+_OptionalCreateBackendStorageResourceConfigTypeDef = TypedDict(
+    "_OptionalCreateBackendStorageResourceConfigTypeDef",
     {
         "BucketName": str,
-        "Permissions": BackendStoragePermissionsOutputTypeDef,
     },
     total=False,
 )
 
-class GetBackendStorageResourceConfigTypeDef(
-    _RequiredGetBackendStorageResourceConfigTypeDef, _OptionalGetBackendStorageResourceConfigTypeDef
+class CreateBackendStorageResourceConfigTypeDef(
+    _RequiredCreateBackendStorageResourceConfigTypeDef,
+    _OptionalCreateBackendStorageResourceConfigTypeDef,
 ):
     pass
 
-_RequiredCreateBackendStorageResourceConfigTypeDef = TypedDict(
-    "_RequiredCreateBackendStorageResourceConfigTypeDef",
+_RequiredGetBackendStorageResourceConfigTypeDef = TypedDict(
+    "_RequiredGetBackendStorageResourceConfigTypeDef",
     {
-        "Permissions": BackendStoragePermissionsTypeDef,
+        "Imported": bool,
         "ServiceName": Literal["S3"],
     },
 )
-_OptionalCreateBackendStorageResourceConfigTypeDef = TypedDict(
-    "_OptionalCreateBackendStorageResourceConfigTypeDef",
+_OptionalGetBackendStorageResourceConfigTypeDef = TypedDict(
+    "_OptionalGetBackendStorageResourceConfigTypeDef",
     {
         "BucketName": str,
+        "Permissions": BackendStoragePermissionsTypeDef,
     },
     total=False,
 )
 
-class CreateBackendStorageResourceConfigTypeDef(
-    _RequiredCreateBackendStorageResourceConfigTypeDef,
-    _OptionalCreateBackendStorageResourceConfigTypeDef,
+class GetBackendStorageResourceConfigTypeDef(
+    _RequiredGetBackendStorageResourceConfigTypeDef, _OptionalGetBackendStorageResourceConfigTypeDef
 ):
     pass
 
 UpdateBackendStorageResourceConfigTypeDef = TypedDict(
     "UpdateBackendStorageResourceConfigTypeDef",
     {
         "Permissions": BackendStoragePermissionsTypeDef,
@@ -1138,34 +1080,14 @@
 
 class UpdateBackendAuthVerificationMessageConfigTypeDef(
     _RequiredUpdateBackendAuthVerificationMessageConfigTypeDef,
     _OptionalUpdateBackendAuthVerificationMessageConfigTypeDef,
 ):
     pass
 
-_RequiredCreateBackendAuthMFAConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthMFAConfigOutputTypeDef",
-    {
-        "MFAMode": MFAModeType,
-    },
-)
-_OptionalCreateBackendAuthMFAConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthMFAConfigOutputTypeDef",
-    {
-        "Settings": SettingsOutputTypeDef,
-    },
-    total=False,
-)
-
-class CreateBackendAuthMFAConfigOutputTypeDef(
-    _RequiredCreateBackendAuthMFAConfigOutputTypeDef,
-    _OptionalCreateBackendAuthMFAConfigOutputTypeDef,
-):
-    pass
-
 _RequiredCreateBackendAuthMFAConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthMFAConfigTypeDef",
     {
         "MFAMode": MFAModeType,
     },
 )
 _OptionalCreateBackendAuthMFAConfigTypeDef = TypedDict(
@@ -1250,64 +1172,27 @@
         "BackendManagerAppId": str,
         "Error": str,
         "LoginAuthConfig": LoginAuthConfigReqObjTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BackendAPIResourceConfigOutputTypeDef = TypedDict(
-    "BackendAPIResourceConfigOutputTypeDef",
-    {
-        "AdditionalAuthTypes": List[BackendAPIAuthTypeTypeDef],
-        "ApiName": str,
-        "ConflictResolution": BackendAPIConflictResolutionTypeDef,
-        "DefaultAuthType": BackendAPIAuthTypeTypeDef,
-        "Service": str,
-        "TransformSchema": str,
-    },
-    total=False,
-)
-
 BackendAPIResourceConfigTypeDef = TypedDict(
     "BackendAPIResourceConfigTypeDef",
     {
         "AdditionalAuthTypes": Sequence[BackendAPIAuthTypeTypeDef],
         "ApiName": str,
         "ConflictResolution": BackendAPIConflictResolutionTypeDef,
         "DefaultAuthType": BackendAPIAuthTypeTypeDef,
         "Service": str,
         "TransformSchema": str,
     },
     total=False,
 )
 
-_RequiredCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthOAuthConfigOutputTypeDef",
-    {
-        "OAuthGrantType": OAuthGrantTypeType,
-        "OAuthScopes": List[OAuthScopesElementType],
-        "RedirectSignInURIs": List[str],
-        "RedirectSignOutURIs": List[str],
-    },
-)
-_OptionalCreateBackendAuthOAuthConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthOAuthConfigOutputTypeDef",
-    {
-        "DomainPrefix": str,
-        "SocialProviderSettings": SocialProviderSettingsTypeDef,
-    },
-    total=False,
-)
-
-class CreateBackendAuthOAuthConfigOutputTypeDef(
-    _RequiredCreateBackendAuthOAuthConfigOutputTypeDef,
-    _OptionalCreateBackendAuthOAuthConfigOutputTypeDef,
-):
-    pass
-
 _RequiredCreateBackendAuthOAuthConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthOAuthConfigTypeDef",
     {
         "OAuthGrantType": OAuthGrantTypeType,
         "OAuthScopes": Sequence[OAuthScopesElementType],
         "RedirectSignInURIs": Sequence[str],
         "RedirectSignOutURIs": Sequence[str],
@@ -1336,60 +1221,45 @@
         "RedirectSignInURIs": Sequence[str],
         "RedirectSignOutURIs": Sequence[str],
         "SocialProviderSettings": SocialProviderSettingsTypeDef,
     },
     total=False,
 )
 
-GetBackendStorageResponseTypeDef = TypedDict(
-    "GetBackendStorageResponseTypeDef",
-    {
-        "AppId": str,
-        "BackendEnvironmentName": str,
-        "ResourceConfig": GetBackendStorageResourceConfigTypeDef,
-        "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateBackendStorageRequestRequestTypeDef = TypedDict(
     "CreateBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": CreateBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
     },
 )
 
-UpdateBackendStorageRequestRequestTypeDef = TypedDict(
-    "UpdateBackendStorageRequestRequestTypeDef",
+GetBackendStorageResponseTypeDef = TypedDict(
+    "GetBackendStorageResponseTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "ResourceConfig": UpdateBackendStorageResourceConfigTypeDef,
+        "ResourceConfig": GetBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetBackendAPIResponseTypeDef = TypedDict(
-    "GetBackendAPIResponseTypeDef",
+UpdateBackendStorageRequestRequestTypeDef = TypedDict(
+    "UpdateBackendStorageRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "Error": str,
-        "ResourceConfig": BackendAPIResourceConfigOutputTypeDef,
+        "ResourceConfig": UpdateBackendStorageResourceConfigTypeDef,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BackendAPIResourceConfigUnionTypeDef = Union[
-    BackendAPIResourceConfigTypeDef, BackendAPIResourceConfigOutputTypeDef
-]
 CreateBackendAPIRequestRequestTypeDef = TypedDict(
     "CreateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": BackendAPIResourceConfigTypeDef,
         "ResourceName": str,
@@ -1434,14 +1304,26 @@
 )
 
 class GetBackendAPIRequestRequestTypeDef(
     _RequiredGetBackendAPIRequestRequestTypeDef, _OptionalGetBackendAPIRequestRequestTypeDef
 ):
     pass
 
+GetBackendAPIResponseTypeDef = TypedDict(
+    "GetBackendAPIResponseTypeDef",
+    {
+        "AppId": str,
+        "BackendEnvironmentName": str,
+        "Error": str,
+        "ResourceConfig": BackendAPIResourceConfigTypeDef,
+        "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateBackendAPIRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateBackendAPIRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceName": str,
     },
@@ -1455,40 +1337,14 @@
 )
 
 class UpdateBackendAPIRequestRequestTypeDef(
     _RequiredUpdateBackendAPIRequestRequestTypeDef, _OptionalUpdateBackendAPIRequestRequestTypeDef
 ):
     pass
 
-_RequiredCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthUserPoolConfigOutputTypeDef",
-    {
-        "RequiredSignUpAttributes": List[RequiredSignUpAttributesElementType],
-        "SignInMethod": SignInMethodType,
-        "UserPoolName": str,
-    },
-)
-_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthUserPoolConfigOutputTypeDef",
-    {
-        "ForgotPassword": CreateBackendAuthForgotPasswordConfigTypeDef,
-        "Mfa": CreateBackendAuthMFAConfigOutputTypeDef,
-        "OAuth": CreateBackendAuthOAuthConfigOutputTypeDef,
-        "PasswordPolicy": CreateBackendAuthPasswordPolicyConfigOutputTypeDef,
-        "VerificationMessage": CreateBackendAuthVerificationMessageConfigTypeDef,
-    },
-    total=False,
-)
-
-class CreateBackendAuthUserPoolConfigOutputTypeDef(
-    _RequiredCreateBackendAuthUserPoolConfigOutputTypeDef,
-    _OptionalCreateBackendAuthUserPoolConfigOutputTypeDef,
-):
-    pass
-
 _RequiredCreateBackendAuthUserPoolConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthUserPoolConfigTypeDef",
     {
         "RequiredSignUpAttributes": Sequence[RequiredSignUpAttributesElementType],
         "SignInMethod": SignInMethodType,
         "UserPoolName": str,
     },
@@ -1518,36 +1374,14 @@
         "OAuth": UpdateBackendAuthOAuthConfigTypeDef,
         "PasswordPolicy": UpdateBackendAuthPasswordPolicyConfigTypeDef,
         "VerificationMessage": UpdateBackendAuthVerificationMessageConfigTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
-    "_RequiredCreateBackendAuthResourceConfigOutputTypeDef",
-    {
-        "AuthResources": AuthResourcesType,
-        "Service": Literal["COGNITO"],
-        "UserPoolConfigs": CreateBackendAuthUserPoolConfigOutputTypeDef,
-    },
-)
-_OptionalCreateBackendAuthResourceConfigOutputTypeDef = TypedDict(
-    "_OptionalCreateBackendAuthResourceConfigOutputTypeDef",
-    {
-        "IdentityPoolConfigs": CreateBackendAuthIdentityPoolConfigTypeDef,
-    },
-    total=False,
-)
-
-class CreateBackendAuthResourceConfigOutputTypeDef(
-    _RequiredCreateBackendAuthResourceConfigOutputTypeDef,
-    _OptionalCreateBackendAuthResourceConfigOutputTypeDef,
-):
-    pass
-
 _RequiredCreateBackendAuthResourceConfigTypeDef = TypedDict(
     "_RequiredCreateBackendAuthResourceConfigTypeDef",
     {
         "AuthResources": AuthResourcesType,
         "Service": Literal["COGNITO"],
         "UserPoolConfigs": CreateBackendAuthUserPoolConfigTypeDef,
     },
@@ -1582,39 +1416,36 @@
 )
 
 class UpdateBackendAuthResourceConfigTypeDef(
     _RequiredUpdateBackendAuthResourceConfigTypeDef, _OptionalUpdateBackendAuthResourceConfigTypeDef
 ):
     pass
 
-GetBackendAuthResponseTypeDef = TypedDict(
-    "GetBackendAuthResponseTypeDef",
+CreateBackendAuthRequestRequestTypeDef = TypedDict(
+    "CreateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
-        "Error": str,
-        "ResourceConfig": CreateBackendAuthResourceConfigOutputTypeDef,
+        "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateBackendAuthRequestRequestTypeDef = TypedDict(
-    "CreateBackendAuthRequestRequestTypeDef",
+GetBackendAuthResponseTypeDef = TypedDict(
+    "GetBackendAuthResponseTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
+        "Error": str,
         "ResourceConfig": CreateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateBackendAuthResourceConfigUnionTypeDef = Union[
-    CreateBackendAuthResourceConfigTypeDef, CreateBackendAuthResourceConfigOutputTypeDef
-]
 UpdateBackendAuthRequestRequestTypeDef = TypedDict(
     "UpdateBackendAuthRequestRequestTypeDef",
     {
         "AppId": str,
         "BackendEnvironmentName": str,
         "ResourceConfig": UpdateBackendAuthResourceConfigTypeDef,
         "ResourceName": str,
```

### Comparing `types-aiobotocore-amplifybackend-2.5.2.post1/types_aiobotocore_amplifybackend.egg-info/SOURCES.txt` & `types-aiobotocore-amplifybackend-2.5.2.post2/types_aiobotocore_amplifybackend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

