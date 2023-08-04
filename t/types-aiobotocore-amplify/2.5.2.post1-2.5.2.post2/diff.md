# Comparing `tmp/types-aiobotocore-amplify-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-amplify-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-amplify-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-amplify-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:19 2023, max compression
```

## Comparing `types-aiobotocore-amplify-2.5.2.post1.tar` & `types-aiobotocore-amplify-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.841667 types-aiobotocore-amplify-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-08-02 14:51:47.833667 types-aiobotocore-amplify-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:47.841667 types-aiobotocore-amplify-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.833667 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29912 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29862 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36050 2023-08-02 14:32:51.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    35991 2023-08-02 14:32:50.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:49.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.833667 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-08-02 14:51:47.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:51:47.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:47.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:47.000000 types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.742887 types-aiobotocore-amplify-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:39:54.000000 types-aiobotocore-amplify-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-08-04 12:00:19.738887 types-aiobotocore-amplify-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-08-04 11:39:54.000000 types-aiobotocore-amplify-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:19.742887 types-aiobotocore-amplify-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 11:39:54.000000 types-aiobotocore-amplify-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.734887 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-04 11:39:54.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-04 11:39:54.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 11:39:54.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29897 2023-08-04 11:39:55.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29847 2023-08-04 11:39:55.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-08-04 11:39:55.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9098 2023-08-04 11:39:55.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-08-04 11:39:55.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-08-04 11:39:55.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:39:54.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35336 2023-08-04 11:39:56.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35277 2023-08-04 11:39:56.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:39:54.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.738887 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-08-04 12:00:19.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 12:00:19.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:19.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:00:19.000000 types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-amplify-2.5.2.post1/LICENSE` & `types-aiobotocore-amplify-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2.post1/setup.py` & `types-aiobotocore-amplify-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-amplify",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_amplify"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Amplify 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/__init__.py` & `types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/__init__.pyi` & `types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/__main__.py` & `types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Amplify 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Amplify 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify\nOther"
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

### Comparing `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/client.py` & `types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .paginator import (
     ListAppsPaginator,
     ListBranchesPaginator,
     ListDomainAssociationsPaginator,
     ListJobsPaginator,
 )
 from .type_defs import (
-    AutoBranchCreationConfigUnionTypeDef,
+    AutoBranchCreationConfigTypeDef,
     CreateAppResultTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateDomainAssociationResultTypeDef,
     CreateWebhookResultTypeDef,
     CustomRuleTypeDef,
@@ -147,15 +147,15 @@
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...
+        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...
     ) -> CreateAppResultTypeDef:
         """
         Creates a new Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#create_app)
         """
@@ -537,15 +537,15 @@
         enableBasicAuth: bool = ...,
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...,
+        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
         repository: str = ...,
         oauthToken: str = ...,
         accessToken: str = ...
     ) -> UpdateAppResultTypeDef:
         """
         Updates an existing Amplify app.
```

### Comparing `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/client.pyi` & `types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .paginator import (
     ListAppsPaginator,
     ListBranchesPaginator,
     ListDomainAssociationsPaginator,
     ListJobsPaginator,
 )
 from .type_defs import (
-    AutoBranchCreationConfigUnionTypeDef,
+    AutoBranchCreationConfigTypeDef,
     CreateAppResultTypeDef,
     CreateBackendEnvironmentResultTypeDef,
     CreateBranchResultTypeDef,
     CreateDeploymentResultTypeDef,
     CreateDomainAssociationResultTypeDef,
     CreateWebhookResultTypeDef,
     CustomRuleTypeDef,
@@ -140,15 +140,15 @@
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         tags: Mapping[str, str] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...
+        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...
     ) -> CreateAppResultTypeDef:
         """
         Creates a new Amplify app.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplify.html#Amplify.Client.create_app)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/client/#create_app)
         """
@@ -496,15 +496,15 @@
         enableBasicAuth: bool = ...,
         basicAuthCredentials: str = ...,
         customRules: Sequence[CustomRuleTypeDef] = ...,
         buildSpec: str = ...,
         customHeaders: str = ...,
         enableAutoBranchCreation: bool = ...,
         autoBranchCreationPatterns: Sequence[str] = ...,
-        autoBranchCreationConfig: AutoBranchCreationConfigUnionTypeDef = ...,
+        autoBranchCreationConfig: AutoBranchCreationConfigTypeDef = ...,
         repository: str = ...,
         oauthToken: str = ...,
         accessToken: str = ...
     ) -> UpdateAppResultTypeDef:
         """
         Updates an existing Amplify app.
```

### Comparing `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/literals.py` & `types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/literals.pyi` & `types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/paginator.py` & `types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/paginator.pyi` & `types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/type_defs.py` & `types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplify service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_amplify.type_defs import AutoBranchCreationConfigOutputTypeDef
+    from types_aiobotocore_amplify.type_defs import AutoBranchCreationConfigTypeDef
 
-    data: AutoBranchCreationConfigOutputTypeDef = ...
+    data: AutoBranchCreationConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -27,19 +27,18 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AutoBranchCreationConfigOutputTypeDef",
+    "AutoBranchCreationConfigTypeDef",
     "CustomRuleTypeDef",
     "ProductionBranchTypeDef",
     "ArtifactTypeDef",
-    "AutoBranchCreationConfigTypeDef",
     "BackendEnvironmentTypeDef",
     "BranchTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackendEnvironmentRequestRequestTypeDef",
     "CreateBranchRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "SubDomainSettingTypeDef",
@@ -72,18 +71,17 @@
     "ListWebhooksRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBranchRequestRequestTypeDef",
     "UpdateWebhookRequestRequestTypeDef",
-    "AppTypeDef",
-    "AutoBranchCreationConfigUnionTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
+    "AppTypeDef",
     "CreateBackendEnvironmentResultTypeDef",
     "CreateBranchResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "DeleteBackendEnvironmentResultTypeDef",
     "DeleteBranchResultTypeDef",
     "GenerateAccessLogsResultTypeDef",
     "GetArtifactUrlResultTypeDef",
@@ -124,21 +122,21 @@
     "CreateDomainAssociationResultTypeDef",
     "DeleteDomainAssociationResultTypeDef",
     "GetDomainAssociationResultTypeDef",
     "ListDomainAssociationsResultTypeDef",
     "UpdateDomainAssociationResultTypeDef",
 )
 
-AutoBranchCreationConfigOutputTypeDef = TypedDict(
-    "AutoBranchCreationConfigOutputTypeDef",
+AutoBranchCreationConfigTypeDef = TypedDict(
+    "AutoBranchCreationConfigTypeDef",
     {
         "stage": StageType,
         "framework": str,
         "enableAutoBuild": bool,
-        "environmentVariables": Dict[str, str],
+        "environmentVariables": Mapping[str, str],
         "basicAuthCredentials": str,
         "enableBasicAuth": bool,
         "enablePerformanceMode": bool,
         "buildSpec": str,
         "enablePullRequestPreview": bool,
         "pullRequestEnvironmentName": str,
     },
@@ -181,31 +179,14 @@
     "ArtifactTypeDef",
     {
         "artifactFileName": str,
         "artifactId": str,
     },
 )
 
-AutoBranchCreationConfigTypeDef = TypedDict(
-    "AutoBranchCreationConfigTypeDef",
-    {
-        "stage": StageType,
-        "framework": str,
-        "enableAutoBuild": bool,
-        "environmentVariables": Mapping[str, str],
-        "basicAuthCredentials": str,
-        "enableBasicAuth": bool,
-        "enablePerformanceMode": bool,
-        "buildSpec": str,
-        "enablePullRequestPreview": bool,
-        "pullRequestEnvironmentName": str,
-    },
-    total=False,
-)
-
 _RequiredBackendEnvironmentTypeDef = TypedDict(
     "_RequiredBackendEnvironmentTypeDef",
     {
         "backendEnvironmentArn": str,
         "environmentName": str,
         "createTime": datetime,
         "updateTime": datetime,
@@ -830,58 +811,14 @@
 
 class UpdateWebhookRequestRequestTypeDef(
     _RequiredUpdateWebhookRequestRequestTypeDef, _OptionalUpdateWebhookRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredAppTypeDef = TypedDict(
-    "_RequiredAppTypeDef",
-    {
-        "appId": str,
-        "appArn": str,
-        "name": str,
-        "description": str,
-        "repository": str,
-        "platform": PlatformType,
-        "createTime": datetime,
-        "updateTime": datetime,
-        "environmentVariables": Dict[str, str],
-        "defaultDomain": str,
-        "enableBranchAutoBuild": bool,
-        "enableBasicAuth": bool,
-    },
-)
-_OptionalAppTypeDef = TypedDict(
-    "_OptionalAppTypeDef",
-    {
-        "tags": Dict[str, str],
-        "iamServiceRoleArn": str,
-        "enableBranchAutoDeletion": bool,
-        "basicAuthCredentials": str,
-        "customRules": List[CustomRuleTypeDef],
-        "productionBranch": ProductionBranchTypeDef,
-        "buildSpec": str,
-        "customHeaders": str,
-        "enableAutoBranchCreation": bool,
-        "autoBranchCreationPatterns": List[str],
-        "autoBranchCreationConfig": AutoBranchCreationConfigOutputTypeDef,
-        "repositoryCloneMethod": RepositoryCloneMethodType,
-    },
-    total=False,
-)
-
-
-class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
-    pass
-
-
-AutoBranchCreationConfigUnionTypeDef = Union[
-    AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
-]
 _RequiredCreateAppRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAppRequestRequestTypeDef = TypedDict(
@@ -950,14 +887,55 @@
 
 class UpdateAppRequestRequestTypeDef(
     _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredAppTypeDef = TypedDict(
+    "_RequiredAppTypeDef",
+    {
+        "appId": str,
+        "appArn": str,
+        "name": str,
+        "description": str,
+        "repository": str,
+        "platform": PlatformType,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "environmentVariables": Dict[str, str],
+        "defaultDomain": str,
+        "enableBranchAutoBuild": bool,
+        "enableBasicAuth": bool,
+    },
+)
+_OptionalAppTypeDef = TypedDict(
+    "_OptionalAppTypeDef",
+    {
+        "tags": Dict[str, str],
+        "iamServiceRoleArn": str,
+        "enableBranchAutoDeletion": bool,
+        "basicAuthCredentials": str,
+        "customRules": List[CustomRuleTypeDef],
+        "productionBranch": ProductionBranchTypeDef,
+        "buildSpec": str,
+        "customHeaders": str,
+        "enableAutoBranchCreation": bool,
+        "autoBranchCreationPatterns": List[str],
+        "autoBranchCreationConfig": AutoBranchCreationConfigTypeDef,
+        "repositoryCloneMethod": RepositoryCloneMethodType,
+    },
+    total=False,
+)
+
+
+class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+    pass
+
+
 CreateBackendEnvironmentResultTypeDef = TypedDict(
     "CreateBackendEnvironmentResultTypeDef",
     {
         "backendEnvironment": BackendEnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify/type_defs.pyi` & `types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for amplify service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplify/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_amplify.type_defs import AutoBranchCreationConfigOutputTypeDef
+    from types_aiobotocore_amplify.type_defs import AutoBranchCreationConfigTypeDef
 
-    data: AutoBranchCreationConfigOutputTypeDef = ...
+    data: AutoBranchCreationConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -26,19 +26,18 @@
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AutoBranchCreationConfigOutputTypeDef",
+    "AutoBranchCreationConfigTypeDef",
     "CustomRuleTypeDef",
     "ProductionBranchTypeDef",
     "ArtifactTypeDef",
-    "AutoBranchCreationConfigTypeDef",
     "BackendEnvironmentTypeDef",
     "BranchTypeDef",
     "ResponseMetadataTypeDef",
     "CreateBackendEnvironmentRequestRequestTypeDef",
     "CreateBranchRequestRequestTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
     "SubDomainSettingTypeDef",
@@ -71,18 +70,17 @@
     "ListWebhooksRequestRequestTypeDef",
     "StartDeploymentRequestRequestTypeDef",
     "StopJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBranchRequestRequestTypeDef",
     "UpdateWebhookRequestRequestTypeDef",
-    "AppTypeDef",
-    "AutoBranchCreationConfigUnionTypeDef",
     "CreateAppRequestRequestTypeDef",
     "UpdateAppRequestRequestTypeDef",
+    "AppTypeDef",
     "CreateBackendEnvironmentResultTypeDef",
     "CreateBranchResultTypeDef",
     "CreateDeploymentResultTypeDef",
     "DeleteBackendEnvironmentResultTypeDef",
     "DeleteBranchResultTypeDef",
     "GenerateAccessLogsResultTypeDef",
     "GetArtifactUrlResultTypeDef",
@@ -123,21 +121,21 @@
     "CreateDomainAssociationResultTypeDef",
     "DeleteDomainAssociationResultTypeDef",
     "GetDomainAssociationResultTypeDef",
     "ListDomainAssociationsResultTypeDef",
     "UpdateDomainAssociationResultTypeDef",
 )
 
-AutoBranchCreationConfigOutputTypeDef = TypedDict(
-    "AutoBranchCreationConfigOutputTypeDef",
+AutoBranchCreationConfigTypeDef = TypedDict(
+    "AutoBranchCreationConfigTypeDef",
     {
         "stage": StageType,
         "framework": str,
         "enableAutoBuild": bool,
-        "environmentVariables": Dict[str, str],
+        "environmentVariables": Mapping[str, str],
         "basicAuthCredentials": str,
         "enableBasicAuth": bool,
         "enablePerformanceMode": bool,
         "buildSpec": str,
         "enablePullRequestPreview": bool,
         "pullRequestEnvironmentName": str,
     },
@@ -178,31 +176,14 @@
     "ArtifactTypeDef",
     {
         "artifactFileName": str,
         "artifactId": str,
     },
 )
 
-AutoBranchCreationConfigTypeDef = TypedDict(
-    "AutoBranchCreationConfigTypeDef",
-    {
-        "stage": StageType,
-        "framework": str,
-        "enableAutoBuild": bool,
-        "environmentVariables": Mapping[str, str],
-        "basicAuthCredentials": str,
-        "enableBasicAuth": bool,
-        "enablePerformanceMode": bool,
-        "buildSpec": str,
-        "enablePullRequestPreview": bool,
-        "pullRequestEnvironmentName": str,
-    },
-    total=False,
-)
-
 _RequiredBackendEnvironmentTypeDef = TypedDict(
     "_RequiredBackendEnvironmentTypeDef",
     {
         "backendEnvironmentArn": str,
         "environmentName": str,
         "createTime": datetime,
         "updateTime": datetime,
@@ -793,56 +774,14 @@
 )
 
 class UpdateWebhookRequestRequestTypeDef(
     _RequiredUpdateWebhookRequestRequestTypeDef, _OptionalUpdateWebhookRequestRequestTypeDef
 ):
     pass
 
-_RequiredAppTypeDef = TypedDict(
-    "_RequiredAppTypeDef",
-    {
-        "appId": str,
-        "appArn": str,
-        "name": str,
-        "description": str,
-        "repository": str,
-        "platform": PlatformType,
-        "createTime": datetime,
-        "updateTime": datetime,
-        "environmentVariables": Dict[str, str],
-        "defaultDomain": str,
-        "enableBranchAutoBuild": bool,
-        "enableBasicAuth": bool,
-    },
-)
-_OptionalAppTypeDef = TypedDict(
-    "_OptionalAppTypeDef",
-    {
-        "tags": Dict[str, str],
-        "iamServiceRoleArn": str,
-        "enableBranchAutoDeletion": bool,
-        "basicAuthCredentials": str,
-        "customRules": List[CustomRuleTypeDef],
-        "productionBranch": ProductionBranchTypeDef,
-        "buildSpec": str,
-        "customHeaders": str,
-        "enableAutoBranchCreation": bool,
-        "autoBranchCreationPatterns": List[str],
-        "autoBranchCreationConfig": AutoBranchCreationConfigOutputTypeDef,
-        "repositoryCloneMethod": RepositoryCloneMethodType,
-    },
-    total=False,
-)
-
-class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
-    pass
-
-AutoBranchCreationConfigUnionTypeDef = Union[
-    AutoBranchCreationConfigTypeDef, AutoBranchCreationConfigOutputTypeDef
-]
 _RequiredCreateAppRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAppRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateAppRequestRequestTypeDef = TypedDict(
@@ -907,14 +846,53 @@
 )
 
 class UpdateAppRequestRequestTypeDef(
     _RequiredUpdateAppRequestRequestTypeDef, _OptionalUpdateAppRequestRequestTypeDef
 ):
     pass
 
+_RequiredAppTypeDef = TypedDict(
+    "_RequiredAppTypeDef",
+    {
+        "appId": str,
+        "appArn": str,
+        "name": str,
+        "description": str,
+        "repository": str,
+        "platform": PlatformType,
+        "createTime": datetime,
+        "updateTime": datetime,
+        "environmentVariables": Dict[str, str],
+        "defaultDomain": str,
+        "enableBranchAutoBuild": bool,
+        "enableBasicAuth": bool,
+    },
+)
+_OptionalAppTypeDef = TypedDict(
+    "_OptionalAppTypeDef",
+    {
+        "tags": Dict[str, str],
+        "iamServiceRoleArn": str,
+        "enableBranchAutoDeletion": bool,
+        "basicAuthCredentials": str,
+        "customRules": List[CustomRuleTypeDef],
+        "productionBranch": ProductionBranchTypeDef,
+        "buildSpec": str,
+        "customHeaders": str,
+        "enableAutoBranchCreation": bool,
+        "autoBranchCreationPatterns": List[str],
+        "autoBranchCreationConfig": AutoBranchCreationConfigTypeDef,
+        "repositoryCloneMethod": RepositoryCloneMethodType,
+    },
+    total=False,
+)
+
+class AppTypeDef(_RequiredAppTypeDef, _OptionalAppTypeDef):
+    pass
+
 CreateBackendEnvironmentResultTypeDef = TypedDict(
     "CreateBackendEnvironmentResultTypeDef",
     {
         "backendEnvironment": BackendEnvironmentTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-amplify-2.5.2.post1/types_aiobotocore_amplify.egg-info/SOURCES.txt` & `types-aiobotocore-amplify-2.5.2.post2/types_aiobotocore_amplify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

