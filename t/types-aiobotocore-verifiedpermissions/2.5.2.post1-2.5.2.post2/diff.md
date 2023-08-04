# Comparing `tmp/types-aiobotocore-verifiedpermissions-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-verifiedpermissions-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-verifiedpermissions-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:08 2023, max compression
+gzip compressed data, was "types-aiobotocore-verifiedpermissions-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
```

## Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1.tar` & `types-aiobotocore-verifiedpermissions-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.885432 types-aiobotocore-verifiedpermissions-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-08-02 14:53:08.885432 types-aiobotocore-verifiedpermissions-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:08.885432 types-aiobotocore-verifiedpermissions-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.881432 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22783 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22746 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8944 2023-08-02 14:50:47.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5935 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31216 2023-08-02 14:50:47.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31165 2023-08-02 14:50:47.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:46.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.885432 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-08-02 14:53:08.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 14:53:08.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:08.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:08.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:08.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:08.000000 types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.266643 types-aiobotocore-verifiedpermissions-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14074 2023-08-04 13:59:29.266643 types-aiobotocore-verifiedpermissions-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12508 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.266643 types-aiobotocore-verifiedpermissions-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2132 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.266643 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1403 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1402 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      991 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22783 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22746 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9039 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9037 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5935 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     5929 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31216 2023-08-04 13:55:24.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    31165 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:23.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.266643 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14074 2023-08-04 13:59:29.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1041 2023-08-04 13:59:29.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.000000 types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/LICENSE` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/README.md` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/README.md`

 * *Files 24% similar despite different names*

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
 [types-aiobotocore-verifiedpermissions docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/).
 
 See how it helps to find and fix potential bugs:
 
@@ -271,131 +271,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_verifiedpermissions.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `VerifiedPermissions` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/literals/).
+
 ```python
-from types_aiobotocore_verifiedpermissions.literals import (
-    DecisionType,
-    ListIdentitySourcesPaginatorName,
-    ListPoliciesPaginatorName,
-    ListPolicyStoresPaginatorName,
-    ListPolicyTemplatesPaginatorName,
-    OpenIdIssuerType,
-    PolicyTypeType,
-    ValidationModeType,
-    VerifiedPermissionsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_verifiedpermissions.literals import DecisionType
 
 
 def check_value(value: DecisionType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_verifiedpermissions.type_defs` module contains structures
 and shapes assembled to typed dictionaries and unions for additional type
 checking.
 
+Full list of `VerifiedPermissions` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions/type_defs/).
+
 ```python
-from types_aiobotocore_verifiedpermissions.type_defs import (
-    ActionIdentifierTypeDef,
-    EntityIdentifierTypeDef,
-    CognitoUserPoolConfigurationTypeDef,
-    ContextDefinitionTypeDef,
-    ResponseMetadataTypeDef,
-    ValidationSettingsTypeDef,
-    CreatePolicyTemplateInputRequestTypeDef,
-    DeleteIdentitySourceInputRequestTypeDef,
-    DeletePolicyInputRequestTypeDef,
-    DeletePolicyStoreInputRequestTypeDef,
-    DeletePolicyTemplateInputRequestTypeDef,
-    DeterminingPolicyItemTypeDef,
-    EvaluationErrorItemTypeDef,
-    GetIdentitySourceInputRequestTypeDef,
-    IdentitySourceDetailsTypeDef,
-    GetPolicyInputRequestTypeDef,
-    GetPolicyStoreInputRequestTypeDef,
-    GetPolicyTemplateInputRequestTypeDef,
-    GetSchemaInputRequestTypeDef,
-    IdentitySourceFilterTypeDef,
-    IdentitySourceItemDetailsTypeDef,
-    PaginatorConfigTypeDef,
-    ListPolicyStoresInputRequestTypeDef,
-    PolicyStoreItemTypeDef,
-    ListPolicyTemplatesInputRequestTypeDef,
-    PolicyTemplateItemTypeDef,
-    StaticPolicyDefinitionDetailTypeDef,
-    StaticPolicyDefinitionItemTypeDef,
-    StaticPolicyDefinitionTypeDef,
-    SchemaDefinitionTypeDef,
-    UpdateCognitoUserPoolConfigurationTypeDef,
-    UpdateStaticPolicyDefinitionTypeDef,
-    UpdatePolicyTemplateInputRequestTypeDef,
-    AttributeValueTypeDef,
-    EntityItemTypeDef,
-    EntityReferenceTypeDef,
-    TemplateLinkedPolicyDefinitionDetailTypeDef,
-    TemplateLinkedPolicyDefinitionItemTypeDef,
-    TemplateLinkedPolicyDefinitionTypeDef,
-    ConfigurationTypeDef,
-    CreateIdentitySourceOutputTypeDef,
-    CreatePolicyOutputTypeDef,
-    CreatePolicyStoreOutputTypeDef,
-    CreatePolicyTemplateOutputTypeDef,
-    GetPolicyTemplateOutputTypeDef,
-    GetSchemaOutputTypeDef,
-    PutSchemaOutputTypeDef,
-    UpdateIdentitySourceOutputTypeDef,
-    UpdatePolicyOutputTypeDef,
-    UpdatePolicyStoreOutputTypeDef,
-    UpdatePolicyTemplateOutputTypeDef,
-    CreatePolicyStoreInputRequestTypeDef,
-    GetPolicyStoreOutputTypeDef,
-    UpdatePolicyStoreInputRequestTypeDef,
-    IsAuthorizedOutputTypeDef,
-    IsAuthorizedWithTokenOutputTypeDef,
-    GetIdentitySourceOutputTypeDef,
-    ListIdentitySourcesInputRequestTypeDef,
-    IdentitySourceItemTypeDef,
-    ListIdentitySourcesInputListIdentitySourcesPaginateTypeDef,
-    ListPolicyStoresInputListPolicyStoresPaginateTypeDef,
-    ListPolicyTemplatesInputListPolicyTemplatesPaginateTypeDef,
-    ListPolicyStoresOutputTypeDef,
-    ListPolicyTemplatesOutputTypeDef,
-    PutSchemaInputRequestTypeDef,
-    UpdateConfigurationTypeDef,
-    UpdatePolicyDefinitionTypeDef,
-    EntitiesDefinitionTypeDef,
-    PolicyFilterTypeDef,
-    PolicyDefinitionDetailTypeDef,
-    PolicyDefinitionItemTypeDef,
-    PolicyDefinitionTypeDef,
-    CreateIdentitySourceInputRequestTypeDef,
-    ListIdentitySourcesOutputTypeDef,
-    UpdateIdentitySourceInputRequestTypeDef,
-    UpdatePolicyInputRequestTypeDef,
-    IsAuthorizedInputRequestTypeDef,
-    IsAuthorizedWithTokenInputRequestTypeDef,
-    ListPoliciesInputListPoliciesPaginateTypeDef,
-    ListPoliciesInputRequestTypeDef,
-    GetPolicyOutputTypeDef,
-    PolicyItemTypeDef,
-    CreatePolicyInputRequestTypeDef,
-    ListPoliciesOutputTypeDef,
-)
+from types_aiobotocore_verifiedpermissions.type_defs import ActionIdentifierTypeDef
 
 
 def get_value() -> ActionIdentifierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/setup.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-verifiedpermissions",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_verifiedpermissions"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.VerifiedPermissions 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/__init__.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/__init__.pyi` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/__main__.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.VerifiedPermissions 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_verifiedpermissions//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/verifiedpermissions.html#VerifiedPermissions\nOther"
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

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/client.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/client.pyi` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/literals.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "DecisionType",
     "ListIdentitySourcesPaginatorName",
     "ListPoliciesPaginatorName",
     "ListPolicyStoresPaginatorName",
     "ListPolicyTemplatesPaginatorName",
     "OpenIdIssuerType",
@@ -31,15 +30,14 @@
     "VerifiedPermissionsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 DecisionType = Literal["ALLOW", "DENY"]
 ListIdentitySourcesPaginatorName = Literal["list_identity_sources"]
 ListPoliciesPaginatorName = Literal["list_policies"]
 ListPolicyStoresPaginatorName = Literal["list_policy_stores"]
 ListPolicyTemplatesPaginatorName = Literal["list_policy_templates"]
 OpenIdIssuerType = Literal["COGNITO"]
 PolicyTypeType = Literal["STATIC", "TEMPLATE_LINKED"]
@@ -56,14 +54,15 @@
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
@@ -159,14 +158,15 @@
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
@@ -245,26 +245,28 @@
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

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/literals.pyi` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/literals.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "DecisionType",
     "ListIdentitySourcesPaginatorName",
     "ListPoliciesPaginatorName",
     "ListPolicyStoresPaginatorName",
     "ListPolicyTemplatesPaginatorName",
     "OpenIdIssuerType",
@@ -30,14 +31,15 @@
     "VerifiedPermissionsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 DecisionType = Literal["ALLOW", "DENY"]
 ListIdentitySourcesPaginatorName = Literal["list_identity_sources"]
 ListPoliciesPaginatorName = Literal["list_policies"]
 ListPolicyStoresPaginatorName = Literal["list_policy_stores"]
 ListPolicyTemplatesPaginatorName = Literal["list_policy_templates"]
 OpenIdIssuerType = Literal["COGNITO"]
 PolicyTypeType = Literal["STATIC", "TEMPLATE_LINKED"]
@@ -54,14 +56,15 @@
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
@@ -157,14 +160,15 @@
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
@@ -243,26 +247,28 @@
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

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/paginator.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/paginator.pyi` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/type_defs.py` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions/type_defs.pyi` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-verifiedpermissions-2.5.2.post1/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt` & `types-aiobotocore-verifiedpermissions-2.5.2.post2/types_aiobotocore_verifiedpermissions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

