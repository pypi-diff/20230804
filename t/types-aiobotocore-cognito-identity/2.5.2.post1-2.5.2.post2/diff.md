# Comparing `tmp/types-aiobotocore-cognito-identity-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cognito-identity-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cognito-identity-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-cognito-identity-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:39 2023, max compression
```

## Comparing `types-aiobotocore-cognito-identity-2.5.2.post1.tar` & `types-aiobotocore-cognito-identity-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.989618 types-aiobotocore-cognito-identity-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15475 2023-08-02 14:52:04.981618 types-aiobotocore-cognito-identity-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13922 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:04.989618 types-aiobotocore-cognito-identity-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.981618 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21116 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21083 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19132 2023-08-02 14:35:19.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19106 2023-08-02 14:35:19.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:17.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:04.981618 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15475 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:04.000000 types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.375645 types-aiobotocore-cognito-identity-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-08-04 12:00:39.367644 types-aiobotocore-cognito-identity-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11938 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:39.375645 types-aiobotocore-cognito-identity-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.363644 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21106 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21073 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-08-04 11:42:36.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18235 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:42:35.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:39.367644 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13491 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:00:39.000000 types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/LICENSE` & `types-aiobotocore-cognito-identity-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/PKG-INFO` & `types-aiobotocore-cognito-identity-2.5.2.post2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cognito-identity
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.CognitoIdentity 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CognitoIdentity 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/
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
 [types-aiobotocore-cognito-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -291,96 +291,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cognito_identity.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CognitoIdentity` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/literals/).
+
 ```python
-from types_aiobotocore_cognito_identity.literals import (
-    AmbiguousRoleResolutionTypeType,
-    ErrorCodeType,
-    ListIdentityPoolsPaginatorName,
-    MappingRuleMatchTypeType,
-    RoleMappingTypeType,
-    CognitoIdentityServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_cognito_identity.literals import AmbiguousRoleResolutionTypeType
 
 
 def check_value(value: AmbiguousRoleResolutionTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cognito_identity.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CognitoIdentity` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/type_defs/).
+
 ```python
-from types_aiobotocore_cognito_identity.type_defs import (
-    CognitoIdentityProviderTypeDef,
-    CredentialsTypeDef,
-    DeleteIdentitiesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    UnprocessedIdentityIdTypeDef,
-    DeleteIdentityPoolInputRequestTypeDef,
-    DescribeIdentityInputRequestTypeDef,
-    DescribeIdentityPoolInputRequestTypeDef,
-    GetCredentialsForIdentityInputRequestTypeDef,
-    GetIdInputRequestTypeDef,
-    GetIdentityPoolRolesInputRequestTypeDef,
-    GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
-    GetOpenIdTokenInputRequestTypeDef,
-    GetPrincipalTagAttributeMapInputRequestTypeDef,
-    IdentityDescriptionTypeDef,
-    IdentityPoolShortDescriptionTypeDef,
-    ListIdentitiesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListIdentityPoolsInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    LookupDeveloperIdentityInputRequestTypeDef,
-    MappingRuleTypeDef,
-    MergeDeveloperIdentitiesInputRequestTypeDef,
-    SetPrincipalTagAttributeMapInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    UnlinkDeveloperIdentityInputRequestTypeDef,
-    UnlinkIdentityInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CreateIdentityPoolInputRequestTypeDef,
-    IdentityPoolRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCredentialsForIdentityResponseTypeDef,
-    GetIdResponseTypeDef,
-    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
-    GetOpenIdTokenResponseTypeDef,
-    GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseTypeDef,
-    IdentityPoolTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LookupDeveloperIdentityResponseTypeDef,
-    MergeDeveloperIdentitiesResponseTypeDef,
-    SetPrincipalTagAttributeMapResponseTypeDef,
-    DeleteIdentitiesResponseTypeDef,
-    ListIdentitiesResponseTypeDef,
-    ListIdentityPoolsResponseTypeDef,
-    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
-    RulesConfigurationTypeOutputTypeDef,
-    RulesConfigurationTypeTypeDef,
-    RoleMappingOutputTypeDef,
-    RoleMappingTypeDef,
-    GetIdentityPoolRolesResponseTypeDef,
-    RoleMappingUnionTypeDef,
-    SetIdentityPoolRolesInputRequestTypeDef,
-)
+from types_aiobotocore_cognito_identity.type_defs import CognitoIdentityProviderTypeDef
 
 
 def get_value() -> CognitoIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/README.md` & `types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-cognito-identity
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.CognitoIdentity 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore cognito-identity type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cognito-identity"></a>
 
 # types-aiobotocore-cognito-identity
 
 [![PyPI - types-aiobotocore-cognito-identity](https://img.shields.io/pypi/v/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cognito-identity.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cognito-identity)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/)
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
 [types-aiobotocore-cognito-identity docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/).
 
 See how it helps to find and fix potential bugs:
 
@@ -259,96 +291,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_cognito_identity.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `CognitoIdentity` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/literals/).
+
 ```python
-from types_aiobotocore_cognito_identity.literals import (
-    AmbiguousRoleResolutionTypeType,
-    ErrorCodeType,
-    ListIdentityPoolsPaginatorName,
-    MappingRuleMatchTypeType,
-    RoleMappingTypeType,
-    CognitoIdentityServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_cognito_identity.literals import AmbiguousRoleResolutionTypeType
 
 
 def check_value(value: AmbiguousRoleResolutionTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_cognito_identity.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `CognitoIdentity` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/type_defs/).
+
 ```python
-from types_aiobotocore_cognito_identity.type_defs import (
-    CognitoIdentityProviderTypeDef,
-    CredentialsTypeDef,
-    DeleteIdentitiesInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    UnprocessedIdentityIdTypeDef,
-    DeleteIdentityPoolInputRequestTypeDef,
-    DescribeIdentityInputRequestTypeDef,
-    DescribeIdentityPoolInputRequestTypeDef,
-    GetCredentialsForIdentityInputRequestTypeDef,
-    GetIdInputRequestTypeDef,
-    GetIdentityPoolRolesInputRequestTypeDef,
-    GetOpenIdTokenForDeveloperIdentityInputRequestTypeDef,
-    GetOpenIdTokenInputRequestTypeDef,
-    GetPrincipalTagAttributeMapInputRequestTypeDef,
-    IdentityDescriptionTypeDef,
-    IdentityPoolShortDescriptionTypeDef,
-    ListIdentitiesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListIdentityPoolsInputRequestTypeDef,
-    ListTagsForResourceInputRequestTypeDef,
-    LookupDeveloperIdentityInputRequestTypeDef,
-    MappingRuleTypeDef,
-    MergeDeveloperIdentitiesInputRequestTypeDef,
-    SetPrincipalTagAttributeMapInputRequestTypeDef,
-    TagResourceInputRequestTypeDef,
-    UnlinkDeveloperIdentityInputRequestTypeDef,
-    UnlinkIdentityInputRequestTypeDef,
-    UntagResourceInputRequestTypeDef,
-    CreateIdentityPoolInputRequestTypeDef,
-    IdentityPoolRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetCredentialsForIdentityResponseTypeDef,
-    GetIdResponseTypeDef,
-    GetOpenIdTokenForDeveloperIdentityResponseTypeDef,
-    GetOpenIdTokenResponseTypeDef,
-    GetPrincipalTagAttributeMapResponseTypeDef,
-    IdentityDescriptionResponseTypeDef,
-    IdentityPoolTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    LookupDeveloperIdentityResponseTypeDef,
-    MergeDeveloperIdentitiesResponseTypeDef,
-    SetPrincipalTagAttributeMapResponseTypeDef,
-    DeleteIdentitiesResponseTypeDef,
-    ListIdentitiesResponseTypeDef,
-    ListIdentityPoolsResponseTypeDef,
-    ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef,
-    RulesConfigurationTypeOutputTypeDef,
-    RulesConfigurationTypeTypeDef,
-    RoleMappingOutputTypeDef,
-    RoleMappingTypeDef,
-    GetIdentityPoolRolesResponseTypeDef,
-    RoleMappingUnionTypeDef,
-    SetIdentityPoolRolesInputRequestTypeDef,
-)
+from types_aiobotocore_cognito_identity.type_defs import CognitoIdentityProviderTypeDef
 
 
 def get_value() -> CognitoIdentityProviderTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/setup.py` & `types-aiobotocore-cognito-identity-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cognito-identity",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cognito_identity"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CognitoIdentity 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/__init__.py` & `types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/__init__.pyi` & `types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/client.py` & `types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     IdentityDescriptionResponseTypeDef,
     IdentityPoolTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityResponseTypeDef,
     MergeDeveloperIdentitiesResponseTypeDef,
-    RoleMappingUnionTypeDef,
+    RoleMappingTypeDef,
     SetPrincipalTagAttributeMapResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -315,15 +315,15 @@
         """
 
     async def set_identity_pool_roles(
         self,
         *,
         IdentityPoolId: str,
         Roles: Mapping[str, str],
-        RoleMappings: Mapping[str, RoleMappingUnionTypeDef] = ...
+        RoleMappings: Mapping[str, RoleMappingTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the roles for an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.set_identity_pool_roles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#set_identity_pool_roles)
         """
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/client.pyi` & `types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     IdentityDescriptionResponseTypeDef,
     IdentityPoolTypeDef,
     ListIdentitiesResponseTypeDef,
     ListIdentityPoolsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     LookupDeveloperIdentityResponseTypeDef,
     MergeDeveloperIdentitiesResponseTypeDef,
-    RoleMappingUnionTypeDef,
+    RoleMappingTypeDef,
     SetPrincipalTagAttributeMapResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -291,15 +291,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#merge_developer_identities)
         """
     async def set_identity_pool_roles(
         self,
         *,
         IdentityPoolId: str,
         Roles: Mapping[str, str],
-        RoleMappings: Mapping[str, RoleMappingUnionTypeDef] = ...
+        RoleMappings: Mapping[str, RoleMappingTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets the roles for an identity pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-identity.html#CognitoIdentity.Client.set_identity_pool_roles)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cognito_identity/client/#set_identity_pool_roles)
         """
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/literals.py` & `types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/literals.pyi` & `types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/paginator.py` & `types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/paginator.pyi` & `types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/type_defs.py` & `types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_cognito_identity.type_defs import CognitoIdentityProviderTypeDef
 
     data: CognitoIdentityProviderTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AmbiguousRoleResolutionTypeType,
     ErrorCodeType,
     MappingRuleMatchTypeType,
     RoleMappingTypeType,
 )
@@ -71,20 +71,17 @@
     "LookupDeveloperIdentityResponseTypeDef",
     "MergeDeveloperIdentitiesResponseTypeDef",
     "SetPrincipalTagAttributeMapResponseTypeDef",
     "DeleteIdentitiesResponseTypeDef",
     "ListIdentitiesResponseTypeDef",
     "ListIdentityPoolsResponseTypeDef",
     "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
-    "RulesConfigurationTypeOutputTypeDef",
     "RulesConfigurationTypeTypeDef",
-    "RoleMappingOutputTypeDef",
     "RoleMappingTypeDef",
     "GetIdentityPoolRolesResponseTypeDef",
-    "RoleMappingUnionTypeDef",
     "SetIdentityPoolRolesInputRequestTypeDef",
 )
 
 CognitoIdentityProviderTypeDef = TypedDict(
     "CognitoIdentityProviderTypeDef",
     {
         "ProviderName": str,
@@ -650,50 +647,21 @@
     "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-RulesConfigurationTypeOutputTypeDef = TypedDict(
-    "RulesConfigurationTypeOutputTypeDef",
-    {
-        "Rules": List[MappingRuleTypeDef],
-    },
-)
-
 RulesConfigurationTypeTypeDef = TypedDict(
     "RulesConfigurationTypeTypeDef",
     {
-        "Rules": Sequence[MappingRuleTypeDef],
-    },
-)
-
-_RequiredRoleMappingOutputTypeDef = TypedDict(
-    "_RequiredRoleMappingOutputTypeDef",
-    {
-        "Type": RoleMappingTypeType,
-    },
-)
-_OptionalRoleMappingOutputTypeDef = TypedDict(
-    "_OptionalRoleMappingOutputTypeDef",
-    {
-        "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
-        "RulesConfiguration": RulesConfigurationTypeOutputTypeDef,
+        "Rules": List[MappingRuleTypeDef],
     },
-    total=False,
 )
 
-
-class RoleMappingOutputTypeDef(
-    _RequiredRoleMappingOutputTypeDef, _OptionalRoleMappingOutputTypeDef
-):
-    pass
-
-
 _RequiredRoleMappingTypeDef = TypedDict(
     "_RequiredRoleMappingTypeDef",
     {
         "Type": RoleMappingTypeType,
     },
 )
 _OptionalRoleMappingTypeDef = TypedDict(
@@ -711,31 +679,30 @@
 
 
 GetIdentityPoolRolesResponseTypeDef = TypedDict(
     "GetIdentityPoolRolesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Dict[str, str],
-        "RoleMappings": Dict[str, RoleMappingOutputTypeDef],
+        "RoleMappings": Dict[str, RoleMappingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RoleMappingUnionTypeDef = Union[RoleMappingTypeDef, RoleMappingOutputTypeDef]
 _RequiredSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Mapping[str, str],
     },
 )
 _OptionalSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_OptionalSetIdentityPoolRolesInputRequestTypeDef",
     {
-        "RoleMappings": Mapping[str, RoleMappingUnionTypeDef],
+        "RoleMappings": Mapping[str, RoleMappingTypeDef],
     },
     total=False,
 )
 
 
 class SetIdentityPoolRolesInputRequestTypeDef(
     _RequiredSetIdentityPoolRolesInputRequestTypeDef,
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity/type_defs.pyi` & `types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_cognito_identity.type_defs import CognitoIdentityProviderTypeDef
 
     data: CognitoIdentityProviderTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AmbiguousRoleResolutionTypeType,
     ErrorCodeType,
     MappingRuleMatchTypeType,
     RoleMappingTypeType,
 )
@@ -70,20 +70,17 @@
     "LookupDeveloperIdentityResponseTypeDef",
     "MergeDeveloperIdentitiesResponseTypeDef",
     "SetPrincipalTagAttributeMapResponseTypeDef",
     "DeleteIdentitiesResponseTypeDef",
     "ListIdentitiesResponseTypeDef",
     "ListIdentityPoolsResponseTypeDef",
     "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
-    "RulesConfigurationTypeOutputTypeDef",
     "RulesConfigurationTypeTypeDef",
-    "RoleMappingOutputTypeDef",
     "RoleMappingTypeDef",
     "GetIdentityPoolRolesResponseTypeDef",
-    "RoleMappingUnionTypeDef",
     "SetIdentityPoolRolesInputRequestTypeDef",
 )
 
 CognitoIdentityProviderTypeDef = TypedDict(
     "CognitoIdentityProviderTypeDef",
     {
         "ProviderName": str,
@@ -629,47 +626,20 @@
     "ListIdentityPoolsInputListIdentityPoolsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-RulesConfigurationTypeOutputTypeDef = TypedDict(
-    "RulesConfigurationTypeOutputTypeDef",
-    {
-        "Rules": List[MappingRuleTypeDef],
-    },
-)
-
 RulesConfigurationTypeTypeDef = TypedDict(
     "RulesConfigurationTypeTypeDef",
     {
-        "Rules": Sequence[MappingRuleTypeDef],
-    },
-)
-
-_RequiredRoleMappingOutputTypeDef = TypedDict(
-    "_RequiredRoleMappingOutputTypeDef",
-    {
-        "Type": RoleMappingTypeType,
+        "Rules": List[MappingRuleTypeDef],
     },
 )
-_OptionalRoleMappingOutputTypeDef = TypedDict(
-    "_OptionalRoleMappingOutputTypeDef",
-    {
-        "AmbiguousRoleResolution": AmbiguousRoleResolutionTypeType,
-        "RulesConfiguration": RulesConfigurationTypeOutputTypeDef,
-    },
-    total=False,
-)
-
-class RoleMappingOutputTypeDef(
-    _RequiredRoleMappingOutputTypeDef, _OptionalRoleMappingOutputTypeDef
-):
-    pass
 
 _RequiredRoleMappingTypeDef = TypedDict(
     "_RequiredRoleMappingTypeDef",
     {
         "Type": RoleMappingTypeType,
     },
 )
@@ -686,31 +656,30 @@
     pass
 
 GetIdentityPoolRolesResponseTypeDef = TypedDict(
     "GetIdentityPoolRolesResponseTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Dict[str, str],
-        "RoleMappings": Dict[str, RoleMappingOutputTypeDef],
+        "RoleMappings": Dict[str, RoleMappingTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RoleMappingUnionTypeDef = Union[RoleMappingTypeDef, RoleMappingOutputTypeDef]
 _RequiredSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_RequiredSetIdentityPoolRolesInputRequestTypeDef",
     {
         "IdentityPoolId": str,
         "Roles": Mapping[str, str],
     },
 )
 _OptionalSetIdentityPoolRolesInputRequestTypeDef = TypedDict(
     "_OptionalSetIdentityPoolRolesInputRequestTypeDef",
     {
-        "RoleMappings": Mapping[str, RoleMappingUnionTypeDef],
+        "RoleMappings": Mapping[str, RoleMappingTypeDef],
     },
     total=False,
 )
 
 class SetIdentityPoolRolesInputRequestTypeDef(
     _RequiredSetIdentityPoolRolesInputRequestTypeDef,
     _OptionalSetIdentityPoolRolesInputRequestTypeDef,
```

### Comparing `types-aiobotocore-cognito-identity-2.5.2.post1/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt` & `types-aiobotocore-cognito-identity-2.5.2.post2/types_aiobotocore_cognito_identity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

