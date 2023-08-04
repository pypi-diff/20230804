# Comparing `tmp/types-aiobotocore-serverlessrepo-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-serverlessrepo-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-serverlessrepo-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:59 2023, max compression
+gzip compressed data, was "types-aiobotocore-serverlessrepo-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:25 2023, max compression
```

## Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1.tar` & `types-aiobotocore-serverlessrepo-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.685461 types-aiobotocore-serverlessrepo-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15692 2023-08-02 14:52:59.677461 types-aiobotocore-serverlessrepo-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14129 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:59.685461 types-aiobotocore-serverlessrepo-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.677461 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16568 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20134 2023-08-02 14:49:30.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-08-02 14:49:30.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:29.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.677461 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15692 2023-08-02 14:52:59.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:59.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:59.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:59.000000 types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.906643 types-aiobotocore-serverlessrepo-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13924 2023-08-04 13:59:25.906643 types-aiobotocore-serverlessrepo-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12361 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:25.906643 types-aiobotocore-serverlessrepo-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2138 2023-08-04 13:53:09.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.906643 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1340 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1339 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1005 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16558 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16532 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8783 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8781 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4817 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4812 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19293 2023-08-04 13:53:14.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    19263 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:10.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:25.906643 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13924 2023-08-04 13:59:25.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:25.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:25.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:25.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:25.000000 types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/LICENSE` & `types-aiobotocore-serverlessrepo-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/PKG-INFO` & `types-aiobotocore-serverlessrepo-2.5.2.post2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-serverlessrepo
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/
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
 [types-aiobotocore-serverlessrepo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,87 +301,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_serverlessrepo.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ServerlessApplicationRepository` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/literals/).
+
 ```python
-from types_aiobotocore_serverlessrepo.literals import (
-    CapabilityType,
-    ListApplicationDependenciesPaginatorName,
-    ListApplicationVersionsPaginatorName,
-    ListApplicationsPaginatorName,
-    StatusType,
-    ServerlessApplicationRepositoryServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_serverlessrepo.literals import CapabilityType
 
 
 def check_value(value: CapabilityType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_serverlessrepo.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ServerlessApplicationRepository` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/type_defs/).
+
 ```python
-from types_aiobotocore_serverlessrepo.type_defs import (
-    ApplicationDependencySummaryTypeDef,
-    ApplicationPolicyStatementOutputTypeDef,
-    ApplicationPolicyStatementTypeDef,
-    ApplicationSummaryTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateApplicationVersionRequestRequestTypeDef,
-    ParameterDefinitionTypeDef,
-    ParameterValueTypeDef,
-    TagTypeDef,
-    CreateCloudFormationTemplateRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    GetApplicationPolicyRequestRequestTypeDef,
-    GetApplicationRequestRequestTypeDef,
-    GetCloudFormationTemplateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationDependenciesRequestRequestTypeDef,
-    ListApplicationVersionsRequestRequestTypeDef,
-    VersionSummaryTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    RollbackTriggerTypeDef,
-    UnshareApplicationRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    ApplicationPolicyStatementUnionTypeDef,
-    CreateCloudFormationChangeSetResponseTypeDef,
-    CreateCloudFormationTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetApplicationPolicyResponseTypeDef,
-    GetCloudFormationTemplateResponseTypeDef,
-    ListApplicationDependenciesResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    PutApplicationPolicyResponseTypeDef,
-    CreateApplicationVersionResponseTypeDef,
-    VersionTypeDef,
-    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListApplicationVersionsResponseTypeDef,
-    RollbackConfigurationTypeDef,
-    PutApplicationPolicyRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    GetApplicationResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    CreateCloudFormationChangeSetRequestRequestTypeDef,
-)
+from types_aiobotocore_serverlessrepo.type_defs import ApplicationDependencySummaryTypeDef
 
 
 def get_value() -> ApplicationDependencySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/README.md` & `types-aiobotocore-serverlessrepo-2.5.2.post2/README.md`

 * *Files 13% similar despite different names*

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
 [types-aiobotocore-serverlessrepo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -269,87 +269,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_serverlessrepo.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ServerlessApplicationRepository` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/literals/).
+
 ```python
-from types_aiobotocore_serverlessrepo.literals import (
-    CapabilityType,
-    ListApplicationDependenciesPaginatorName,
-    ListApplicationVersionsPaginatorName,
-    ListApplicationsPaginatorName,
-    StatusType,
-    ServerlessApplicationRepositoryServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_serverlessrepo.literals import CapabilityType
 
 
 def check_value(value: CapabilityType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_serverlessrepo.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ServerlessApplicationRepository` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/type_defs/).
+
 ```python
-from types_aiobotocore_serverlessrepo.type_defs import (
-    ApplicationDependencySummaryTypeDef,
-    ApplicationPolicyStatementOutputTypeDef,
-    ApplicationPolicyStatementTypeDef,
-    ApplicationSummaryTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateApplicationVersionRequestRequestTypeDef,
-    ParameterDefinitionTypeDef,
-    ParameterValueTypeDef,
-    TagTypeDef,
-    CreateCloudFormationTemplateRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    GetApplicationPolicyRequestRequestTypeDef,
-    GetApplicationRequestRequestTypeDef,
-    GetCloudFormationTemplateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationDependenciesRequestRequestTypeDef,
-    ListApplicationVersionsRequestRequestTypeDef,
-    VersionSummaryTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    RollbackTriggerTypeDef,
-    UnshareApplicationRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    ApplicationPolicyStatementUnionTypeDef,
-    CreateCloudFormationChangeSetResponseTypeDef,
-    CreateCloudFormationTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetApplicationPolicyResponseTypeDef,
-    GetCloudFormationTemplateResponseTypeDef,
-    ListApplicationDependenciesResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    PutApplicationPolicyResponseTypeDef,
-    CreateApplicationVersionResponseTypeDef,
-    VersionTypeDef,
-    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListApplicationVersionsResponseTypeDef,
-    RollbackConfigurationTypeDef,
-    PutApplicationPolicyRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    GetApplicationResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    CreateCloudFormationChangeSetRequestRequestTypeDef,
-)
+from types_aiobotocore_serverlessrepo.type_defs import ApplicationDependencySummaryTypeDef
 
 
 def get_value() -> ApplicationDependencySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/setup.py` & `types-aiobotocore-serverlessrepo-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-serverlessrepo",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_serverlessrepo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2 service generated"
-        " with mypy-boto3-builder 7.17.1"
+        " with mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/__init__.py` & `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/__init__.pyi` & `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/__main__.py` & `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository\nOther"
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

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/client.py` & `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from .paginator import (
     ListApplicationDependenciesPaginator,
     ListApplicationsPaginator,
     ListApplicationVersionsPaginator,
 )
 from .type_defs import (
-    ApplicationPolicyStatementUnionTypeDef,
+    ApplicationPolicyStatementTypeDef,
     CreateApplicationResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
     GetApplicationResponseTypeDef,
@@ -267,15 +267,15 @@
         Lists applications owned by the requester.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#list_applications)
         """
 
     async def put_application_policy(
-        self, *, ApplicationId: str, Statements: Sequence[ApplicationPolicyStatementUnionTypeDef]
+        self, *, ApplicationId: str, Statements: Sequence[ApplicationPolicyStatementTypeDef]
     ) -> PutApplicationPolicyResponseTypeDef:
         """
         Sets the permission policy for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.put_application_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#put_application_policy)
         """
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/client.pyi` & `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 from .paginator import (
     ListApplicationDependenciesPaginator,
     ListApplicationsPaginator,
     ListApplicationVersionsPaginator,
 )
 from .type_defs import (
-    ApplicationPolicyStatementUnionTypeDef,
+    ApplicationPolicyStatementTypeDef,
     CreateApplicationResponseTypeDef,
     CreateApplicationVersionResponseTypeDef,
     CreateCloudFormationChangeSetResponseTypeDef,
     CreateCloudFormationTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetApplicationPolicyResponseTypeDef,
     GetApplicationResponseTypeDef,
@@ -248,15 +248,15 @@
         """
         Lists applications owned by the requester.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.list_applications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#list_applications)
         """
     async def put_application_policy(
-        self, *, ApplicationId: str, Statements: Sequence[ApplicationPolicyStatementUnionTypeDef]
+        self, *, ApplicationId: str, Statements: Sequence[ApplicationPolicyStatementTypeDef]
     ) -> PutApplicationPolicyResponseTypeDef:
         """
         Sets the permission policy for an application.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/serverlessrepo.html#ServerlessApplicationRepository.Client.put_application_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/client/#put_application_policy)
         """
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/literals.py` & `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
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
@@ -155,14 +156,15 @@
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
@@ -241,26 +243,28 @@
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

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/literals.pyi` & `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
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
@@ -153,14 +154,15 @@
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
@@ -239,26 +241,28 @@
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

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/paginator.py` & `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/paginator.pyi` & `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/type_defs.py` & `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,27 +8,26 @@
     ```python
     from types_aiobotocore_serverlessrepo.type_defs import ApplicationDependencySummaryTypeDef
 
     data: ApplicationDependencySummaryTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import CapabilityType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApplicationDependencySummaryTypeDef",
-    "ApplicationPolicyStatementOutputTypeDef",
     "ApplicationPolicyStatementTypeDef",
     "ApplicationSummaryTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateApplicationVersionRequestRequestTypeDef",
     "ParameterDefinitionTypeDef",
     "ParameterValueTypeDef",
@@ -42,15 +41,15 @@
     "ListApplicationDependenciesRequestRequestTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "VersionSummaryTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "RollbackTriggerTypeDef",
     "UnshareApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "ApplicationPolicyStatementUnionTypeDef",
+    "PutApplicationPolicyRequestRequestTypeDef",
     "CreateCloudFormationChangeSetResponseTypeDef",
     "CreateCloudFormationTemplateResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetApplicationPolicyResponseTypeDef",
     "GetCloudFormationTemplateResponseTypeDef",
     "ListApplicationDependenciesResponseTypeDef",
     "ListApplicationsResponseTypeDef",
@@ -58,64 +57,39 @@
     "CreateApplicationVersionResponseTypeDef",
     "VersionTypeDef",
     "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
     "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "RollbackConfigurationTypeDef",
-    "PutApplicationPolicyRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "CreateCloudFormationChangeSetRequestRequestTypeDef",
 )
 
 ApplicationDependencySummaryTypeDef = TypedDict(
     "ApplicationDependencySummaryTypeDef",
     {
         "ApplicationId": str,
         "SemanticVersion": str,
     },
 )
 
-_RequiredApplicationPolicyStatementOutputTypeDef = TypedDict(
-    "_RequiredApplicationPolicyStatementOutputTypeDef",
-    {
-        "Actions": List[str],
-        "Principals": List[str],
-    },
-)
-_OptionalApplicationPolicyStatementOutputTypeDef = TypedDict(
-    "_OptionalApplicationPolicyStatementOutputTypeDef",
-    {
-        "PrincipalOrgIDs": List[str],
-        "StatementId": str,
-    },
-    total=False,
-)
-
-
-class ApplicationPolicyStatementOutputTypeDef(
-    _RequiredApplicationPolicyStatementOutputTypeDef,
-    _OptionalApplicationPolicyStatementOutputTypeDef,
-):
-    pass
-
-
 _RequiredApplicationPolicyStatementTypeDef = TypedDict(
     "_RequiredApplicationPolicyStatementTypeDef",
     {
-        "Actions": Sequence[str],
-        "Principals": Sequence[str],
+        "Actions": List[str],
+        "Principals": List[str],
     },
 )
 _OptionalApplicationPolicyStatementTypeDef = TypedDict(
     "_OptionalApplicationPolicyStatementTypeDef",
     {
-        "PrincipalOrgIDs": Sequence[str],
+        "PrincipalOrgIDs": List[str],
         "StatementId": str,
     },
     total=False,
 )
 
 
 class ApplicationPolicyStatementTypeDef(
@@ -460,17 +434,22 @@
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
 
-ApplicationPolicyStatementUnionTypeDef = Union[
-    ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef
-]
+PutApplicationPolicyRequestRequestTypeDef = TypedDict(
+    "PutApplicationPolicyRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
+    },
+)
+
 CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
     "CreateCloudFormationChangeSetResponseTypeDef",
     {
         "ApplicationId": str,
         "ChangeSetId": str,
         "SemanticVersion": str,
         "StackId": str,
@@ -498,15 +477,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationPolicyResponseTypeDef = TypedDict(
     "GetApplicationPolicyResponseTypeDef",
     {
-        "Statements": List[ApplicationPolicyStatementOutputTypeDef],
+        "Statements": List[ApplicationPolicyStatementTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCloudFormationTemplateResponseTypeDef = TypedDict(
     "GetCloudFormationTemplateResponseTypeDef",
     {
@@ -538,15 +517,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutApplicationPolicyResponseTypeDef = TypedDict(
     "PutApplicationPolicyResponseTypeDef",
     {
-        "Statements": List[ApplicationPolicyStatementOutputTypeDef],
+        "Statements": List[ApplicationPolicyStatementTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApplicationVersionResponseTypeDef = TypedDict(
     "CreateApplicationVersionResponseTypeDef",
     {
@@ -656,22 +635,14 @@
     {
         "MonitoringTimeInMinutes": int,
         "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
     },
     total=False,
 )
 
-PutApplicationPolicyRequestRequestTypeDef = TypedDict(
-    "PutApplicationPolicyRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "Statements": Sequence[ApplicationPolicyStatementUnionTypeDef],
-    },
-)
-
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationId": str,
         "Author": str,
         "CreationTime": str,
         "Description": str,
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo/type_defs.pyi` & `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -8,26 +8,25 @@
     ```python
     from types_aiobotocore_serverlessrepo.type_defs import ApplicationDependencySummaryTypeDef
 
     data: ApplicationDependencySummaryTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import CapabilityType, StatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApplicationDependencySummaryTypeDef",
-    "ApplicationPolicyStatementOutputTypeDef",
     "ApplicationPolicyStatementTypeDef",
     "ApplicationSummaryTypeDef",
     "CreateApplicationRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CreateApplicationVersionRequestRequestTypeDef",
     "ParameterDefinitionTypeDef",
     "ParameterValueTypeDef",
@@ -41,15 +40,15 @@
     "ListApplicationDependenciesRequestRequestTypeDef",
     "ListApplicationVersionsRequestRequestTypeDef",
     "VersionSummaryTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "RollbackTriggerTypeDef",
     "UnshareApplicationRequestRequestTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
-    "ApplicationPolicyStatementUnionTypeDef",
+    "PutApplicationPolicyRequestRequestTypeDef",
     "CreateCloudFormationChangeSetResponseTypeDef",
     "CreateCloudFormationTemplateResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetApplicationPolicyResponseTypeDef",
     "GetCloudFormationTemplateResponseTypeDef",
     "ListApplicationDependenciesResponseTypeDef",
     "ListApplicationsResponseTypeDef",
@@ -57,62 +56,39 @@
     "CreateApplicationVersionResponseTypeDef",
     "VersionTypeDef",
     "ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef",
     "ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef",
     "ListApplicationsRequestListApplicationsPaginateTypeDef",
     "ListApplicationVersionsResponseTypeDef",
     "RollbackConfigurationTypeDef",
-    "PutApplicationPolicyRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "GetApplicationResponseTypeDef",
     "UpdateApplicationResponseTypeDef",
     "CreateCloudFormationChangeSetRequestRequestTypeDef",
 )
 
 ApplicationDependencySummaryTypeDef = TypedDict(
     "ApplicationDependencySummaryTypeDef",
     {
         "ApplicationId": str,
         "SemanticVersion": str,
     },
 )
 
-_RequiredApplicationPolicyStatementOutputTypeDef = TypedDict(
-    "_RequiredApplicationPolicyStatementOutputTypeDef",
-    {
-        "Actions": List[str],
-        "Principals": List[str],
-    },
-)
-_OptionalApplicationPolicyStatementOutputTypeDef = TypedDict(
-    "_OptionalApplicationPolicyStatementOutputTypeDef",
-    {
-        "PrincipalOrgIDs": List[str],
-        "StatementId": str,
-    },
-    total=False,
-)
-
-class ApplicationPolicyStatementOutputTypeDef(
-    _RequiredApplicationPolicyStatementOutputTypeDef,
-    _OptionalApplicationPolicyStatementOutputTypeDef,
-):
-    pass
-
 _RequiredApplicationPolicyStatementTypeDef = TypedDict(
     "_RequiredApplicationPolicyStatementTypeDef",
     {
-        "Actions": Sequence[str],
-        "Principals": Sequence[str],
+        "Actions": List[str],
+        "Principals": List[str],
     },
 )
 _OptionalApplicationPolicyStatementTypeDef = TypedDict(
     "_OptionalApplicationPolicyStatementTypeDef",
     {
-        "PrincipalOrgIDs": Sequence[str],
+        "PrincipalOrgIDs": List[str],
         "StatementId": str,
     },
     total=False,
 )
 
 class ApplicationPolicyStatementTypeDef(
     _RequiredApplicationPolicyStatementTypeDef, _OptionalApplicationPolicyStatementTypeDef
@@ -435,17 +411,22 @@
 )
 
 class UpdateApplicationRequestRequestTypeDef(
     _RequiredUpdateApplicationRequestRequestTypeDef, _OptionalUpdateApplicationRequestRequestTypeDef
 ):
     pass
 
-ApplicationPolicyStatementUnionTypeDef = Union[
-    ApplicationPolicyStatementTypeDef, ApplicationPolicyStatementOutputTypeDef
-]
+PutApplicationPolicyRequestRequestTypeDef = TypedDict(
+    "PutApplicationPolicyRequestRequestTypeDef",
+    {
+        "ApplicationId": str,
+        "Statements": Sequence[ApplicationPolicyStatementTypeDef],
+    },
+)
+
 CreateCloudFormationChangeSetResponseTypeDef = TypedDict(
     "CreateCloudFormationChangeSetResponseTypeDef",
     {
         "ApplicationId": str,
         "ChangeSetId": str,
         "SemanticVersion": str,
         "StackId": str,
@@ -473,15 +454,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApplicationPolicyResponseTypeDef = TypedDict(
     "GetApplicationPolicyResponseTypeDef",
     {
-        "Statements": List[ApplicationPolicyStatementOutputTypeDef],
+        "Statements": List[ApplicationPolicyStatementTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCloudFormationTemplateResponseTypeDef = TypedDict(
     "GetCloudFormationTemplateResponseTypeDef",
     {
@@ -513,15 +494,15 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutApplicationPolicyResponseTypeDef = TypedDict(
     "PutApplicationPolicyResponseTypeDef",
     {
-        "Statements": List[ApplicationPolicyStatementOutputTypeDef],
+        "Statements": List[ApplicationPolicyStatementTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApplicationVersionResponseTypeDef = TypedDict(
     "CreateApplicationVersionResponseTypeDef",
     {
@@ -625,22 +606,14 @@
     {
         "MonitoringTimeInMinutes": int,
         "RollbackTriggers": Sequence[RollbackTriggerTypeDef],
     },
     total=False,
 )
 
-PutApplicationPolicyRequestRequestTypeDef = TypedDict(
-    "PutApplicationPolicyRequestRequestTypeDef",
-    {
-        "ApplicationId": str,
-        "Statements": Sequence[ApplicationPolicyStatementUnionTypeDef],
-    },
-)
-
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationId": str,
         "Author": str,
         "CreationTime": str,
         "Description": str,
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO` & `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-serverlessrepo
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ServerlessApplicationRepository 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/
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
 [types-aiobotocore-serverlessrepo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/).
 
 See how it helps to find and fix potential bugs:
 
@@ -301,87 +301,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_serverlessrepo.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `ServerlessApplicationRepository` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/literals/).
+
 ```python
-from types_aiobotocore_serverlessrepo.literals import (
-    CapabilityType,
-    ListApplicationDependenciesPaginatorName,
-    ListApplicationVersionsPaginatorName,
-    ListApplicationsPaginatorName,
-    StatusType,
-    ServerlessApplicationRepositoryServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_serverlessrepo.literals import CapabilityType
 
 
 def check_value(value: CapabilityType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_serverlessrepo.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ServerlessApplicationRepository` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_serverlessrepo/type_defs/).
+
 ```python
-from types_aiobotocore_serverlessrepo.type_defs import (
-    ApplicationDependencySummaryTypeDef,
-    ApplicationPolicyStatementOutputTypeDef,
-    ApplicationPolicyStatementTypeDef,
-    ApplicationSummaryTypeDef,
-    CreateApplicationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    CreateApplicationVersionRequestRequestTypeDef,
-    ParameterDefinitionTypeDef,
-    ParameterValueTypeDef,
-    TagTypeDef,
-    CreateCloudFormationTemplateRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
-    GetApplicationPolicyRequestRequestTypeDef,
-    GetApplicationRequestRequestTypeDef,
-    GetCloudFormationTemplateRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListApplicationDependenciesRequestRequestTypeDef,
-    ListApplicationVersionsRequestRequestTypeDef,
-    VersionSummaryTypeDef,
-    ListApplicationsRequestRequestTypeDef,
-    RollbackTriggerTypeDef,
-    UnshareApplicationRequestRequestTypeDef,
-    UpdateApplicationRequestRequestTypeDef,
-    ApplicationPolicyStatementUnionTypeDef,
-    CreateCloudFormationChangeSetResponseTypeDef,
-    CreateCloudFormationTemplateResponseTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetApplicationPolicyResponseTypeDef,
-    GetCloudFormationTemplateResponseTypeDef,
-    ListApplicationDependenciesResponseTypeDef,
-    ListApplicationsResponseTypeDef,
-    PutApplicationPolicyResponseTypeDef,
-    CreateApplicationVersionResponseTypeDef,
-    VersionTypeDef,
-    ListApplicationDependenciesRequestListApplicationDependenciesPaginateTypeDef,
-    ListApplicationVersionsRequestListApplicationVersionsPaginateTypeDef,
-    ListApplicationsRequestListApplicationsPaginateTypeDef,
-    ListApplicationVersionsResponseTypeDef,
-    RollbackConfigurationTypeDef,
-    PutApplicationPolicyRequestRequestTypeDef,
-    CreateApplicationResponseTypeDef,
-    GetApplicationResponseTypeDef,
-    UpdateApplicationResponseTypeDef,
-    CreateCloudFormationChangeSetRequestRequestTypeDef,
-)
+from types_aiobotocore_serverlessrepo.type_defs import ApplicationDependencySummaryTypeDef
 
 
 def get_value() -> ApplicationDependencySummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-serverlessrepo-2.5.2.post1/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt` & `types-aiobotocore-serverlessrepo-2.5.2.post2/types_aiobotocore_serverlessrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

