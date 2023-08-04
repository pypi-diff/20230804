# Comparing `tmp/types-aiobotocore-appintegrations-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-appintegrations-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appintegrations-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-appintegrations-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:22 2023, max compression
```

## Comparing `types-aiobotocore-appintegrations-2.5.2.post1.tar` & `types-aiobotocore-appintegrations-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.565660 types-aiobotocore-appintegrations-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-08-02 14:51:50.565660 types-aiobotocore-appintegrations-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.565660 types-aiobotocore-appintegrations-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.565660 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14082 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:12.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.565660 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-08-02 14:51:50.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:51:50.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:51:50.000000 types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.787006 types-aiobotocore-appintegrations-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:19.000000 types-aiobotocore-appintegrations-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-08-04 12:00:22.787006 types-aiobotocore-appintegrations-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-08-04 11:40:19.000000 types-aiobotocore-appintegrations-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:22.787006 types-aiobotocore-appintegrations-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-04 11:40:19.000000 types-aiobotocore-appintegrations-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.779005 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-04 11:40:19.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-04 11:40:19.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-04 11:40:19.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-08-04 11:40:19.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-08-04 11:40:19.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-08-04 11:40:19.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7838 2023-08-04 11:40:19.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:19.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-08-04 11:40:20.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12450 2023-08-04 11:40:20.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:19.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.787006 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12711 2023-08-04 12:00:22.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:00:22.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:22.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-04 12:00:22.000000 types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/LICENSE` & `types-aiobotocore-appintegrations-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/PKG-INFO` & `types-aiobotocore-appintegrations-2.5.2.post2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appintegrations
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.AppIntegrationsService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.AppIntegrationsService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/
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
 [types-aiobotocore-appintegrations docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,71 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_appintegrations.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `AppIntegrationsService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/literals/).
+
 ```python
-from types_aiobotocore_appintegrations.literals import (
-    AppIntegrationsServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_appintegrations.literals import AppIntegrationsServiceServiceName
 
 
 def check_value(value: AppIntegrationsServiceServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_appintegrations.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `AppIntegrationsService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/type_defs/).
+
 ```python
-from types_aiobotocore_appintegrations.type_defs import (
-    FileConfigurationTypeDef,
-    ScheduleConfigurationTypeDef,
-    FileConfigurationOutputTypeDef,
-    ResponseMetadataTypeDef,
-    EventFilterTypeDef,
-    DataIntegrationAssociationSummaryTypeDef,
-    DataIntegrationSummaryTypeDef,
-    DeleteDataIntegrationRequestRequestTypeDef,
-    DeleteEventIntegrationRequestRequestTypeDef,
-    EventIntegrationAssociationTypeDef,
-    GetDataIntegrationRequestRequestTypeDef,
-    GetEventIntegrationRequestRequestTypeDef,
-    ListDataIntegrationAssociationsRequestRequestTypeDef,
-    ListDataIntegrationsRequestRequestTypeDef,
-    ListEventIntegrationAssociationsRequestRequestTypeDef,
-    ListEventIntegrationsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateDataIntegrationRequestRequestTypeDef,
-    UpdateEventIntegrationRequestRequestTypeDef,
-    CreateDataIntegrationRequestRequestTypeDef,
-    FileConfigurationUnionTypeDef,
-    CreateDataIntegrationResponseTypeDef,
-    CreateEventIntegrationResponseTypeDef,
-    GetDataIntegrationResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    CreateEventIntegrationRequestRequestTypeDef,
-    EventIntegrationTypeDef,
-    GetEventIntegrationResponseTypeDef,
-    ListDataIntegrationAssociationsResponseTypeDef,
-    ListDataIntegrationsResponseTypeDef,
-    ListEventIntegrationAssociationsResponseTypeDef,
-    ListEventIntegrationsResponseTypeDef,
-)
+from types_aiobotocore_appintegrations.type_defs import FileConfigurationTypeDef
 
 
 def get_value() -> FileConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/setup.py` & `types-aiobotocore-appintegrations-2.5.2.post2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appintegrations",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_appintegrations"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AppIntegrationsService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/__init__.py` & `types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/__init__.pyi` & `types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/__main__.py` & `types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.AppIntegrationsService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService\nOther"
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

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/client.py` & `types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
     CreateDataIntegrationResponseTypeDef,
     CreateEventIntegrationResponseTypeDef,
     EventFilterTypeDef,
-    FileConfigurationUnionTypeDef,
+    FileConfigurationTypeDef,
     GetDataIntegrationResponseTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -95,15 +95,15 @@
         Name: str,
         KmsKey: str,
         SourceURI: str,
         ScheduleConfig: ScheduleConfigurationTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...,
-        FileConfiguration: FileConfigurationUnionTypeDef = ...,
+        FileConfiguration: FileConfigurationTypeDef = ...,
         ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...
     ) -> CreateDataIntegrationResponseTypeDef:
         """
         Creates and persists a DataIntegration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.create_data_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/client/#create_data_integration)
```

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/client.pyi` & `types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
     CreateDataIntegrationResponseTypeDef,
     CreateEventIntegrationResponseTypeDef,
     EventFilterTypeDef,
-    FileConfigurationUnionTypeDef,
+    FileConfigurationTypeDef,
     GetDataIntegrationResponseTypeDef,
     GetEventIntegrationResponseTypeDef,
     ListDataIntegrationAssociationsResponseTypeDef,
     ListDataIntegrationsResponseTypeDef,
     ListEventIntegrationAssociationsResponseTypeDef,
     ListEventIntegrationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
@@ -89,15 +89,15 @@
         Name: str,
         KmsKey: str,
         SourceURI: str,
         ScheduleConfig: ScheduleConfigurationTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...,
         ClientToken: str = ...,
-        FileConfiguration: FileConfigurationUnionTypeDef = ...,
+        FileConfiguration: FileConfigurationTypeDef = ...,
         ObjectConfiguration: Mapping[str, Mapping[str, Sequence[str]]] = ...
     ) -> CreateDataIntegrationResponseTypeDef:
         """
         Creates and persists a DataIntegration resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appintegrations.html#AppIntegrationsService.Client.create_data_integration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/client/#create_data_integration)
```

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/literals.py` & `types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/literals.pyi` & `types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/type_defs.py` & `types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -8,26 +8,24 @@
     ```python
     from types_aiobotocore_appintegrations.type_defs import FileConfigurationTypeDef
 
     data: FileConfigurationTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "FileConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
-    "FileConfigurationOutputTypeDef",
     "ResponseMetadataTypeDef",
     "EventFilterTypeDef",
     "DataIntegrationAssociationSummaryTypeDef",
     "DataIntegrationSummaryTypeDef",
     "DeleteDataIntegrationRequestRequestTypeDef",
     "DeleteEventIntegrationRequestRequestTypeDef",
     "EventIntegrationAssociationTypeDef",
@@ -39,15 +37,14 @@
     "ListEventIntegrationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataIntegrationRequestRequestTypeDef",
     "UpdateEventIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationRequestRequestTypeDef",
-    "FileConfigurationUnionTypeDef",
     "CreateDataIntegrationResponseTypeDef",
     "CreateEventIntegrationResponseTypeDef",
     "GetDataIntegrationResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "CreateEventIntegrationRequestRequestTypeDef",
     "EventIntegrationTypeDef",
     "GetEventIntegrationResponseTypeDef",
@@ -67,21 +64,19 @@
     "_OptionalFileConfigurationTypeDef",
     {
         "Filters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class FileConfigurationTypeDef(
     _RequiredFileConfigurationTypeDef, _OptionalFileConfigurationTypeDef
 ):
     pass
 
-
 _RequiredScheduleConfigurationTypeDef = TypedDict(
     "_RequiredScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 _OptionalScheduleConfigurationTypeDef = TypedDict(
@@ -89,42 +84,19 @@
     {
         "FirstExecutionFrom": str,
         "Object": str,
     },
     total=False,
 )
 
-
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
-
-_RequiredFileConfigurationOutputTypeDef = TypedDict(
-    "_RequiredFileConfigurationOutputTypeDef",
-    {
-        "Folders": List[str],
-    },
-)
-_OptionalFileConfigurationOutputTypeDef = TypedDict(
-    "_OptionalFileConfigurationOutputTypeDef",
-    {
-        "Filters": Dict[str, List[str]],
-    },
-    total=False,
-)
-
-
-class FileConfigurationOutputTypeDef(
-    _RequiredFileConfigurationOutputTypeDef, _OptionalFileConfigurationOutputTypeDef
-):
-    pass
-
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -211,22 +183,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListDataIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListDataIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListDataIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListDataIntegrationsRequestRequestTypeDef = TypedDict(
     "ListDataIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -243,22 +213,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListEventIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListEventIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListEventIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 ListEventIntegrationsRequestRequestTypeDef = TypedDict(
     "ListEventIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -298,44 +266,40 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateDataIntegrationRequestRequestTypeDef(
     _RequiredUpdateDataIntegrationRequestRequestTypeDef,
     _OptionalUpdateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateEventIntegrationRequestRequestTypeDef(
     _RequiredUpdateEventIntegrationRequestRequestTypeDef,
     _OptionalUpdateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDataIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataIntegrationRequestRequestTypeDef",
     {
         "Name": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfig": ScheduleConfigurationTypeDef,
@@ -349,36 +313,33 @@
         "ClientToken": str,
         "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Mapping[str, Mapping[str, Sequence[str]]],
     },
     total=False,
 )
 
-
 class CreateDataIntegrationRequestRequestTypeDef(
     _RequiredCreateDataIntegrationRequestRequestTypeDef,
     _OptionalCreateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
-FileConfigurationUnionTypeDef = Union[FileConfigurationTypeDef, FileConfigurationOutputTypeDef]
 CreateDataIntegrationResponseTypeDef = TypedDict(
     "CreateDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
         "ClientToken": str,
-        "FileConfiguration": FileConfigurationOutputTypeDef,
+        "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEventIntegrationResponseTypeDef = TypedDict(
     "CreateEventIntegrationResponseTypeDef",
@@ -395,15 +356,15 @@
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
-        "FileConfiguration": FileConfigurationOutputTypeDef,
+        "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
@@ -427,22 +388,20 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateEventIntegrationRequestRequestTypeDef(
     _RequiredCreateEventIntegrationRequestRequestTypeDef,
     _OptionalCreateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
-
 EventIntegrationTypeDef = TypedDict(
     "EventIntegrationTypeDef",
     {
         "EventIntegrationArn": str,
         "Name": str,
         "Description": str,
         "EventFilter": EventFilterTypeDef,
```

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations/type_defs.pyi` & `types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,25 +8,25 @@
     ```python
     from types_aiobotocore_appintegrations.type_defs import FileConfigurationTypeDef
 
     data: FileConfigurationTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "FileConfigurationTypeDef",
     "ScheduleConfigurationTypeDef",
-    "FileConfigurationOutputTypeDef",
     "ResponseMetadataTypeDef",
     "EventFilterTypeDef",
     "DataIntegrationAssociationSummaryTypeDef",
     "DataIntegrationSummaryTypeDef",
     "DeleteDataIntegrationRequestRequestTypeDef",
     "DeleteEventIntegrationRequestRequestTypeDef",
     "EventIntegrationAssociationTypeDef",
@@ -38,15 +38,14 @@
     "ListEventIntegrationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDataIntegrationRequestRequestTypeDef",
     "UpdateEventIntegrationRequestRequestTypeDef",
     "CreateDataIntegrationRequestRequestTypeDef",
-    "FileConfigurationUnionTypeDef",
     "CreateDataIntegrationResponseTypeDef",
     "CreateEventIntegrationResponseTypeDef",
     "GetDataIntegrationResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "CreateEventIntegrationRequestRequestTypeDef",
     "EventIntegrationTypeDef",
     "GetEventIntegrationResponseTypeDef",
@@ -66,19 +65,21 @@
     "_OptionalFileConfigurationTypeDef",
     {
         "Filters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class FileConfigurationTypeDef(
     _RequiredFileConfigurationTypeDef, _OptionalFileConfigurationTypeDef
 ):
     pass
 
+
 _RequiredScheduleConfigurationTypeDef = TypedDict(
     "_RequiredScheduleConfigurationTypeDef",
     {
         "ScheduleExpression": str,
     },
 )
 _OptionalScheduleConfigurationTypeDef = TypedDict(
@@ -86,37 +87,20 @@
     {
         "FirstExecutionFrom": str,
         "Object": str,
     },
     total=False,
 )
 
+
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
-_RequiredFileConfigurationOutputTypeDef = TypedDict(
-    "_RequiredFileConfigurationOutputTypeDef",
-    {
-        "Folders": List[str],
-    },
-)
-_OptionalFileConfigurationOutputTypeDef = TypedDict(
-    "_OptionalFileConfigurationOutputTypeDef",
-    {
-        "Filters": Dict[str, List[str]],
-    },
-    total=False,
-)
-
-class FileConfigurationOutputTypeDef(
-    _RequiredFileConfigurationOutputTypeDef, _OptionalFileConfigurationOutputTypeDef
-):
-    pass
 
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
@@ -204,20 +188,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListDataIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListDataIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListDataIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListDataIntegrationsRequestRequestTypeDef = TypedDict(
     "ListDataIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -234,20 +220,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListEventIntegrationAssociationsRequestRequestTypeDef(
     _RequiredListEventIntegrationAssociationsRequestRequestTypeDef,
     _OptionalListEventIntegrationAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 ListEventIntegrationsRequestRequestTypeDef = TypedDict(
     "ListEventIntegrationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -287,40 +275,44 @@
     {
         "Name": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateDataIntegrationRequestRequestTypeDef(
     _RequiredUpdateDataIntegrationRequestRequestTypeDef,
     _OptionalUpdateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateEventIntegrationRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateEventIntegrationRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateEventIntegrationRequestRequestTypeDef(
     _RequiredUpdateEventIntegrationRequestRequestTypeDef,
     _OptionalUpdateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDataIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataIntegrationRequestRequestTypeDef",
     {
         "Name": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfig": ScheduleConfigurationTypeDef,
@@ -334,34 +326,35 @@
         "ClientToken": str,
         "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Mapping[str, Mapping[str, Sequence[str]]],
     },
     total=False,
 )
 
+
 class CreateDataIntegrationRequestRequestTypeDef(
     _RequiredCreateDataIntegrationRequestRequestTypeDef,
     _OptionalCreateDataIntegrationRequestRequestTypeDef,
 ):
     pass
 
-FileConfigurationUnionTypeDef = Union[FileConfigurationTypeDef, FileConfigurationOutputTypeDef]
+
 CreateDataIntegrationResponseTypeDef = TypedDict(
     "CreateDataIntegrationResponseTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
         "ClientToken": str,
-        "FileConfiguration": FileConfigurationOutputTypeDef,
+        "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateEventIntegrationResponseTypeDef = TypedDict(
     "CreateEventIntegrationResponseTypeDef",
@@ -378,15 +371,15 @@
         "Id": str,
         "Name": str,
         "Description": str,
         "KmsKey": str,
         "SourceURI": str,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "Tags": Dict[str, str],
-        "FileConfiguration": FileConfigurationOutputTypeDef,
+        "FileConfiguration": FileConfigurationTypeDef,
         "ObjectConfiguration": Dict[str, Dict[str, List[str]]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
@@ -410,20 +403,22 @@
         "Description": str,
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateEventIntegrationRequestRequestTypeDef(
     _RequiredCreateEventIntegrationRequestRequestTypeDef,
     _OptionalCreateEventIntegrationRequestRequestTypeDef,
 ):
     pass
 
+
 EventIntegrationTypeDef = TypedDict(
     "EventIntegrationTypeDef",
     {
         "EventIntegrationArn": str,
         "Name": str,
         "Description": str,
         "EventFilter": EventFilterTypeDef,
```

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/PKG-INFO` & `types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appintegrations
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.AppIntegrationsService 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.AppIntegrationsService 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/
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
 [types-aiobotocore-appintegrations docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,71 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_appintegrations.literals` module contains literals extracted
 from shapes that can be used in user code for type checking.
 
+Full list of `AppIntegrationsService` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/literals/).
+
 ```python
-from types_aiobotocore_appintegrations.literals import (
-    AppIntegrationsServiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_appintegrations.literals import AppIntegrationsServiceServiceName
 
 
 def check_value(value: AppIntegrationsServiceServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_appintegrations.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `AppIntegrationsService` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appintegrations/type_defs/).
+
 ```python
-from types_aiobotocore_appintegrations.type_defs import (
-    FileConfigurationTypeDef,
-    ScheduleConfigurationTypeDef,
-    FileConfigurationOutputTypeDef,
-    ResponseMetadataTypeDef,
-    EventFilterTypeDef,
-    DataIntegrationAssociationSummaryTypeDef,
-    DataIntegrationSummaryTypeDef,
-    DeleteDataIntegrationRequestRequestTypeDef,
-    DeleteEventIntegrationRequestRequestTypeDef,
-    EventIntegrationAssociationTypeDef,
-    GetDataIntegrationRequestRequestTypeDef,
-    GetEventIntegrationRequestRequestTypeDef,
-    ListDataIntegrationAssociationsRequestRequestTypeDef,
-    ListDataIntegrationsRequestRequestTypeDef,
-    ListEventIntegrationAssociationsRequestRequestTypeDef,
-    ListEventIntegrationsRequestRequestTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdateDataIntegrationRequestRequestTypeDef,
-    UpdateEventIntegrationRequestRequestTypeDef,
-    CreateDataIntegrationRequestRequestTypeDef,
-    FileConfigurationUnionTypeDef,
-    CreateDataIntegrationResponseTypeDef,
-    CreateEventIntegrationResponseTypeDef,
-    GetDataIntegrationResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    CreateEventIntegrationRequestRequestTypeDef,
-    EventIntegrationTypeDef,
-    GetEventIntegrationResponseTypeDef,
-    ListDataIntegrationAssociationsResponseTypeDef,
-    ListDataIntegrationsResponseTypeDef,
-    ListEventIntegrationAssociationsResponseTypeDef,
-    ListEventIntegrationsResponseTypeDef,
-)
+from types_aiobotocore_appintegrations.type_defs import FileConfigurationTypeDef
 
 
 def get_value() -> FileConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-appintegrations-2.5.2.post1/types_aiobotocore_appintegrations.egg-info/SOURCES.txt` & `types-aiobotocore-appintegrations-2.5.2.post2/types_aiobotocore_appintegrations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

