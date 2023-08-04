# Comparing `tmp/types-aiobotocore-sso-oidc-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sso-oidc-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sso-oidc-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-sso-oidc-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
```

## Comparing `types-aiobotocore-sso-oidc-2.5.2.post1.tar` & `types-aiobotocore-sso-oidc-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.601447 types-aiobotocore-sso-oidc-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-08-02 14:53:04.601447 types-aiobotocore-sso-oidc-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:04.601447 types-aiobotocore-sso-oidc-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.601447 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-08-02 14:50:19.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-08-02 14:50:19.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-08-02 14:50:19.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-08-02 14:50:19.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-08-02 14:50:19.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-02 14:50:19.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.601447 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-08-02 14:53:04.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 14:53:04.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:04.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:04.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:04.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:04.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.726643 types-aiobotocore-sso-oidc-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12254 2023-08-04 13:59:27.726643 types-aiobotocore-sso-oidc-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10733 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.726643 types-aiobotocore-sso-oidc-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2078 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.726643 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      445 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      444 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      945 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6480 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6469 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8058 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8056 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3330 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3325 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:34.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.726643 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12254 2023-08-04 13:59:27.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      751 2023-08-04 13:59:27.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:27.000000 types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sso-oidc-2.5.2.post1/LICENSE` & `types-aiobotocore-sso-oidc-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-oidc-2.5.2.post1/PKG-INFO` & `types-aiobotocore-sso-oidc-2.5.2.post2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso-oidc
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SSOOIDC 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SSOOIDC 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/
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
 [types-aiobotocore-sso-oidc docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,44 +265,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sso_oidc.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `SSOOIDC` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/literals/).
+
 ```python
-from types_aiobotocore_sso_oidc.literals import (
-    SSOOIDCServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_sso_oidc.literals import SSOOIDCServiceName
 
 
 def check_value(value: SSOOIDCServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sso_oidc.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SSOOIDC` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/type_defs/).
+
 ```python
-from types_aiobotocore_sso_oidc.type_defs import (
-    CreateTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RegisterClientRequestRequestTypeDef,
-    StartDeviceAuthorizationRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
-    RegisterClientResponseTypeDef,
-    StartDeviceAuthorizationResponseTypeDef,
-)
+from types_aiobotocore_sso_oidc.type_defs import CreateTokenRequestRequestTypeDef
 
 
 def get_value() -> CreateTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sso-oidc-2.5.2.post1/README.md` & `types-aiobotocore-sso-oidc-2.5.2.post2/README.md`

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
 [types-aiobotocore-sso-oidc docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/).
 
 See how it helps to find and fix potential bugs:
 
@@ -233,44 +233,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sso_oidc.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `SSOOIDC` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/literals/).
+
 ```python
-from types_aiobotocore_sso_oidc.literals import (
-    SSOOIDCServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_sso_oidc.literals import SSOOIDCServiceName
 
 
 def check_value(value: SSOOIDCServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sso_oidc.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SSOOIDC` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/type_defs/).
+
 ```python
-from types_aiobotocore_sso_oidc.type_defs import (
-    CreateTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RegisterClientRequestRequestTypeDef,
-    StartDeviceAuthorizationRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
-    RegisterClientResponseTypeDef,
-    StartDeviceAuthorizationResponseTypeDef,
-)
+from types_aiobotocore_sso_oidc.type_defs import CreateTokenRequestRequestTypeDef
 
 
 def get_value() -> CreateTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sso-oidc-2.5.2.post1/setup.py` & `types-aiobotocore-sso-oidc-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sso-oidc",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sso_oidc"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SSOOIDC 2.5.2 service generated with mypy-boto3-builder"
-        " 7.17.1"
+        " 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/__main__.py` & `types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSOOIDC 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SSOOIDC 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC\nOther"
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

### Comparing `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/client.py` & `types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/client.pyi` & `types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/literals.py` & `types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/literals.py`

 * *Files 0% similar despite different names*

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

### Comparing `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/literals.pyi` & `types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/literals.pyi`

 * *Files 0% similar despite different names*

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

### Comparing `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/type_defs.py` & `types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/type_defs.pyi` & `types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/PKG-INFO` & `types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso-oidc
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SSOOIDC 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SSOOIDC 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/
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
 [types-aiobotocore-sso-oidc docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/).
 
 See how it helps to find and fix potential bugs:
 
@@ -265,44 +265,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sso_oidc.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `SSOOIDC` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/literals/).
+
 ```python
-from types_aiobotocore_sso_oidc.literals import (
-    SSOOIDCServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_sso_oidc.literals import SSOOIDCServiceName
 
 
 def check_value(value: SSOOIDCServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sso_oidc.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SSOOIDC` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/type_defs/).
+
 ```python
-from types_aiobotocore_sso_oidc.type_defs import (
-    CreateTokenRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    RegisterClientRequestRequestTypeDef,
-    StartDeviceAuthorizationRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
-    RegisterClientResponseTypeDef,
-    StartDeviceAuthorizationResponseTypeDef,
-)
+from types_aiobotocore_sso_oidc.type_defs import CreateTokenRequestRequestTypeDef
 
 
 def get_value() -> CreateTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/SOURCES.txt` & `types-aiobotocore-sso-oidc-2.5.2.post2/types_aiobotocore_sso_oidc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

