# Comparing `tmp/types-aiobotocore-sso-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sso-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sso-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-sso-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
```

## Comparing `types-aiobotocore-sso-2.5.2.post1.tar` & `types-aiobotocore-sso-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.741447 types-aiobotocore-sso-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-08-02 14:53:04.741447 types-aiobotocore-sso-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:04.741447 types-aiobotocore-sso-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.741447 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-08-02 14:50:17.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-08-02 14:50:17.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-08-02 14:50:17.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-08-02 14:50:17.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.741447 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-08-02 14:53:04.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:53:04.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:04.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:04.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:04.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:04.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.876643 types-aiobotocore-sso-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12815 2023-08-04 13:59:27.876643 types-aiobotocore-sso-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11313 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.876643 types-aiobotocore-sso-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:54:29.000000 types-aiobotocore-sso-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.876643 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      799 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      798 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7370 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7355 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8350 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8348 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3023 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3019 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5373 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5364 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:30.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.876643 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12815 2023-08-04 13:59:27.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:27.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:27.000000 types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sso-2.5.2.post1/LICENSE` & `types-aiobotocore-sso-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post1/PKG-INFO` & `types-aiobotocore-sso-2.5.2.post2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SSO 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SSO 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/
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
 [types-aiobotocore-sso docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,55 +290,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sso.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `SSO` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/literals/).
+
 ```python
-from types_aiobotocore_sso.literals import (
-    ListAccountRolesPaginatorName,
-    ListAccountsPaginatorName,
-    SSOServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_sso.literals import ListAccountRolesPaginatorName
 
 
 def check_value(value: ListAccountRolesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sso.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SSO` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/type_defs/).
+
 ```python
-from types_aiobotocore_sso.type_defs import (
-    AccountInfoTypeDef,
-    ResponseMetadataTypeDef,
-    GetRoleCredentialsRequestRequestTypeDef,
-    RoleCredentialsTypeDef,
-    PaginatorConfigTypeDef,
-    ListAccountRolesRequestRequestTypeDef,
-    RoleInfoTypeDef,
-    ListAccountsRequestRequestTypeDef,
-    LogoutRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAccountsResponseTypeDef,
-    GetRoleCredentialsResponseTypeDef,
-    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
-    ListAccountRolesResponseTypeDef,
-)
+from types_aiobotocore_sso.type_defs import AccountInfoTypeDef
 
 
 def get_value() -> AccountInfoTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sso-2.5.2.post1/README.md` & `types-aiobotocore-sso-2.5.2.post2/README.md`

 * *Files 5% similar despite different names*

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
 [types-aiobotocore-sso docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/).
 
 See how it helps to find and fix potential bugs:
 
@@ -258,55 +258,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sso.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `SSO` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/literals/).
+
 ```python
-from types_aiobotocore_sso.literals import (
-    ListAccountRolesPaginatorName,
-    ListAccountsPaginatorName,
-    SSOServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_sso.literals import ListAccountRolesPaginatorName
 
 
 def check_value(value: ListAccountRolesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sso.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SSO` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/type_defs/).
+
 ```python
-from types_aiobotocore_sso.type_defs import (
-    AccountInfoTypeDef,
-    ResponseMetadataTypeDef,
-    GetRoleCredentialsRequestRequestTypeDef,
-    RoleCredentialsTypeDef,
-    PaginatorConfigTypeDef,
-    ListAccountRolesRequestRequestTypeDef,
-    RoleInfoTypeDef,
-    ListAccountsRequestRequestTypeDef,
-    LogoutRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAccountsResponseTypeDef,
-    GetRoleCredentialsResponseTypeDef,
-    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
-    ListAccountRolesResponseTypeDef,
-)
+from types_aiobotocore_sso.type_defs import AccountInfoTypeDef
 
 
 def get_value() -> AccountInfoTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sso-2.5.2.post1/setup.py` & `types-aiobotocore-sso-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sso",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sso"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SSO 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/__init__.py` & `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/__init__.pyi` & `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/__main__.py` & `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSO 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SSO 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO\nOther"
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

### Comparing `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/client.py` & `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/client.pyi` & `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/literals.py` & `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
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
@@ -147,14 +148,15 @@
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
@@ -233,26 +235,28 @@
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

### Comparing `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/literals.pyi` & `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
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
@@ -145,14 +146,15 @@
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
@@ -231,26 +233,28 @@
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

### Comparing `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/paginator.py` & `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/paginator.pyi` & `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/type_defs.py` & `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/type_defs.pyi` & `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/PKG-INFO` & `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.SSO 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.SSO 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/
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
 [types-aiobotocore-sso docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/).
 
 See how it helps to find and fix potential bugs:
 
@@ -290,55 +290,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sso.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `SSO` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/literals/).
+
 ```python
-from types_aiobotocore_sso.literals import (
-    ListAccountRolesPaginatorName,
-    ListAccountsPaginatorName,
-    SSOServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_sso.literals import ListAccountRolesPaginatorName
 
 
 def check_value(value: ListAccountRolesPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sso.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `SSO` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/type_defs/).
+
 ```python
-from types_aiobotocore_sso.type_defs import (
-    AccountInfoTypeDef,
-    ResponseMetadataTypeDef,
-    GetRoleCredentialsRequestRequestTypeDef,
-    RoleCredentialsTypeDef,
-    PaginatorConfigTypeDef,
-    ListAccountRolesRequestRequestTypeDef,
-    RoleInfoTypeDef,
-    ListAccountsRequestRequestTypeDef,
-    LogoutRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListAccountsResponseTypeDef,
-    GetRoleCredentialsResponseTypeDef,
-    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
-    ListAccountRolesResponseTypeDef,
-)
+from types_aiobotocore_sso.type_defs import AccountInfoTypeDef
 
 
 def get_value() -> AccountInfoTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/SOURCES.txt` & `types-aiobotocore-sso-2.5.2.post2/types_aiobotocore_sso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

