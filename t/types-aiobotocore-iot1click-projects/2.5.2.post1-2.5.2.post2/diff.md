# Comparing `tmp/types-aiobotocore-iot1click-projects-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iot1click-projects-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iot1click-projects-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:24 2023, max compression
+gzip compressed data, was "types-aiobotocore-iot1click-projects-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:11 2023, max compression
```

## Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1.tar` & `types-aiobotocore-iot1click-projects-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.437569 types-aiobotocore-iot1click-projects-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-08-02 14:52:24.433569 types-aiobotocore-iot1click-projects-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13320 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:24.437569 types-aiobotocore-iot1click-projects-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.433569 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14763 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14736 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8038 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8036 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-08-02 14:40:39.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11492 2023-08-02 14:40:39.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:38.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.433569 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 14:52:24.000000 types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.236642 types-aiobotocore-iot1click-projects-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13747 2023-08-04 13:59:11.236642 types-aiobotocore-iot1click-projects-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12186 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:11.236642 types-aiobotocore-iot1click-projects-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2148 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.236642 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      900 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      899 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      985 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14748 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14721 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8133 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8131 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3242 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3238 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10882 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10865 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:51.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:11.236642 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13747 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1022 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       37 2023-08-04 13:59:11.000000 types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/LICENSE` & `types-aiobotocore-iot1click-projects-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/PKG-INFO` & `types-aiobotocore-iot1click-projects-2.5.2.post2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot1click-projects
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/
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
 [types-aiobotocore-iot1click-projects docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,74 +293,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot1click_projects.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `IoT1ClickProjects` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/literals/).
+
 ```python
-from types_aiobotocore_iot1click_projects.literals import (
-    ListPlacementsPaginatorName,
-    ListProjectsPaginatorName,
-    IoT1ClickProjectsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_iot1click_projects.literals import ListPlacementsPaginatorName
 
 
 def check_value(value: ListPlacementsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot1click_projects.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoT1ClickProjects` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/type_defs/).
+
 ```python
 from types_aiobotocore_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
-    CreatePlacementRequestRequestTypeDef,
-    DeletePlacementRequestRequestTypeDef,
-    DeleteProjectRequestRequestTypeDef,
-    DescribePlacementRequestRequestTypeDef,
-    PlacementDescriptionTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeProjectRequestRequestTypeDef,
-    DeviceTemplateOutputTypeDef,
-    DeviceTemplateTypeDef,
-    DisassociateDeviceFromPlacementRequestRequestTypeDef,
-    GetDevicesInPlacementRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListPlacementsRequestRequestTypeDef,
-    PlacementSummaryTypeDef,
-    ListProjectsRequestRequestTypeDef,
-    ProjectSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdatePlacementRequestRequestTypeDef,
-    DescribePlacementResponseTypeDef,
-    GetDevicesInPlacementResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PlacementTemplateOutputTypeDef,
-    PlacementTemplateTypeDef,
-    ListPlacementsRequestListPlacementsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListPlacementsResponseTypeDef,
-    ListProjectsResponseTypeDef,
-    ProjectDescriptionTypeDef,
-    CreateProjectRequestRequestTypeDef,
-    PlacementTemplateUnionTypeDef,
-    UpdateProjectRequestRequestTypeDef,
-    DescribeProjectResponseTypeDef,
 )
 
 
 def get_value() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/README.md` & `types-aiobotocore-iot1click-projects-2.5.2.post2/README.md`

 * *Files 14% similar despite different names*

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
 [types-aiobotocore-iot1click-projects docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
 
@@ -261,74 +261,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot1click_projects.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `IoT1ClickProjects` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/literals/).
+
 ```python
-from types_aiobotocore_iot1click_projects.literals import (
-    ListPlacementsPaginatorName,
-    ListProjectsPaginatorName,
-    IoT1ClickProjectsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_iot1click_projects.literals import ListPlacementsPaginatorName
 
 
 def check_value(value: ListPlacementsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot1click_projects.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoT1ClickProjects` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/type_defs/).
+
 ```python
 from types_aiobotocore_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
-    CreatePlacementRequestRequestTypeDef,
-    DeletePlacementRequestRequestTypeDef,
-    DeleteProjectRequestRequestTypeDef,
-    DescribePlacementRequestRequestTypeDef,
-    PlacementDescriptionTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeProjectRequestRequestTypeDef,
-    DeviceTemplateOutputTypeDef,
-    DeviceTemplateTypeDef,
-    DisassociateDeviceFromPlacementRequestRequestTypeDef,
-    GetDevicesInPlacementRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListPlacementsRequestRequestTypeDef,
-    PlacementSummaryTypeDef,
-    ListProjectsRequestRequestTypeDef,
-    ProjectSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdatePlacementRequestRequestTypeDef,
-    DescribePlacementResponseTypeDef,
-    GetDevicesInPlacementResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PlacementTemplateOutputTypeDef,
-    PlacementTemplateTypeDef,
-    ListPlacementsRequestListPlacementsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListPlacementsResponseTypeDef,
-    ListProjectsResponseTypeDef,
-    ProjectDescriptionTypeDef,
-    CreateProjectRequestRequestTypeDef,
-    PlacementTemplateUnionTypeDef,
-    UpdateProjectRequestRequestTypeDef,
-    DescribeProjectResponseTypeDef,
 )
 
 
 def get_value() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/setup.py` & `types-aiobotocore-iot1click-projects-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iot1click-projects",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iot1click_projects"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoT1ClickProjects 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/__init__.py` & `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/__init__.pyi` & `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/__main__.py` & `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.IoT1ClickProjects 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects\nOther"
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

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/client.py` & `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .type_defs import (
     DescribePlacementResponseTypeDef,
     DescribeProjectResponseTypeDef,
     GetDevicesInPlacementResponseTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PlacementTemplateUnionTypeDef,
+    PlacementTemplateTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -111,15 +111,15 @@
         """
 
     async def create_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: PlacementTemplateUnionTypeDef = ...,
+        placementTemplate: PlacementTemplateTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> Dict[str, Any]:
         """
         Creates an empty project with a placement template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#create_project)
@@ -252,15 +252,15 @@
         """
 
     async def update_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: PlacementTemplateUnionTypeDef = ...
+        placementTemplate: PlacementTemplateTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a project associated with your AWS account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#update_project)
         """
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/client.pyi` & `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .type_defs import (
     DescribePlacementResponseTypeDef,
     DescribeProjectResponseTypeDef,
     GetDevicesInPlacementResponseTypeDef,
     ListPlacementsResponseTypeDef,
     ListProjectsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PlacementTemplateUnionTypeDef,
+    PlacementTemplateTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -102,15 +102,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#create_placement)
         """
     async def create_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: PlacementTemplateUnionTypeDef = ...,
+        placementTemplate: PlacementTemplateTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> Dict[str, Any]:
         """
         Creates an empty project with a placement template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.create_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#create_project)
@@ -229,15 +229,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#update_placement)
         """
     async def update_project(
         self,
         *,
         projectName: str,
         description: str = ...,
-        placementTemplate: PlacementTemplateUnionTypeDef = ...
+        placementTemplate: PlacementTemplateTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates a project associated with your AWS account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iot1click-projects.html#IoT1ClickProjects.Client.update_project)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/client/#update_project)
         """
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/literals.py` & `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/literals.py`

 * *Files 0% similar despite different names*

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

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/literals.pyi` & `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/literals.pyi`

 * *Files 0% similar despite different names*

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

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/paginator.py` & `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/paginator.pyi` & `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/type_defs.py` & `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_iot1click_projects.type_defs import AssociateDeviceWithPlacementRequestRequestTypeDef
 
     data: AssociateDeviceWithPlacementRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
@@ -26,15 +26,14 @@
     "CreatePlacementRequestRequestTypeDef",
     "DeletePlacementRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DescribePlacementRequestRequestTypeDef",
     "PlacementDescriptionTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeProjectRequestRequestTypeDef",
-    "DeviceTemplateOutputTypeDef",
     "DeviceTemplateTypeDef",
     "DisassociateDeviceFromPlacementRequestRequestTypeDef",
     "GetDevicesInPlacementRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListPlacementsRequestRequestTypeDef",
     "PlacementSummaryTypeDef",
     "ListProjectsRequestRequestTypeDef",
@@ -42,23 +41,21 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePlacementRequestRequestTypeDef",
     "DescribePlacementResponseTypeDef",
     "GetDevicesInPlacementResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PlacementTemplateOutputTypeDef",
     "PlacementTemplateTypeDef",
     "ListPlacementsRequestListPlacementsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListPlacementsResponseTypeDef",
     "ListProjectsResponseTypeDef",
-    "ProjectDescriptionTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "PlacementTemplateUnionTypeDef",
+    "ProjectDescriptionTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
 )
 
 AssociateDeviceWithPlacementRequestRequestTypeDef = TypedDict(
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     {
@@ -139,23 +136,14 @@
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
-DeviceTemplateOutputTypeDef = TypedDict(
-    "DeviceTemplateOutputTypeDef",
-    {
-        "deviceType": str,
-        "callbackOverrides": Dict[str, str],
-    },
-    total=False,
-)
-
 DeviceTemplateTypeDef = TypedDict(
     "DeviceTemplateTypeDef",
     {
         "deviceType": str,
         "callbackOverrides": Mapping[str, str],
     },
     total=False,
@@ -316,23 +304,14 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PlacementTemplateOutputTypeDef = TypedDict(
-    "PlacementTemplateOutputTypeDef",
-    {
-        "defaultAttributes": Dict[str, str],
-        "deviceTemplates": Dict[str, DeviceTemplateOutputTypeDef],
-    },
-    total=False,
-)
-
 PlacementTemplateTypeDef = TypedDict(
     "PlacementTemplateTypeDef",
     {
         "defaultAttributes": Mapping[str, str],
         "deviceTemplates": Mapping[str, DeviceTemplateTypeDef],
     },
     total=False,
@@ -382,64 +361,63 @@
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredProjectDescriptionTypeDef = TypedDict(
-    "_RequiredProjectDescriptionTypeDef",
+_RequiredCreateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "projectName": str,
-        "createdDate": datetime,
-        "updatedDate": datetime,
     },
 )
-_OptionalProjectDescriptionTypeDef = TypedDict(
-    "_OptionalProjectDescriptionTypeDef",
+_OptionalCreateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectRequestRequestTypeDef",
     {
-        "arn": str,
         "description": str,
-        "placementTemplate": PlacementTemplateOutputTypeDef,
-        "tags": Dict[str, str],
+        "placementTemplate": PlacementTemplateTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
 
-class ProjectDescriptionTypeDef(
-    _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
+class CreateProjectRequestRequestTypeDef(
+    _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredCreateProjectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectRequestRequestTypeDef",
+_RequiredProjectDescriptionTypeDef = TypedDict(
+    "_RequiredProjectDescriptionTypeDef",
     {
         "projectName": str,
+        "createdDate": datetime,
+        "updatedDate": datetime,
     },
 )
-_OptionalCreateProjectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectRequestRequestTypeDef",
+_OptionalProjectDescriptionTypeDef = TypedDict(
+    "_OptionalProjectDescriptionTypeDef",
     {
+        "arn": str,
         "description": str,
         "placementTemplate": PlacementTemplateTypeDef,
-        "tags": Mapping[str, str],
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
 
-class CreateProjectRequestRequestTypeDef(
-    _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
+class ProjectDescriptionTypeDef(
+    _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
 ):
     pass
 
 
-PlacementTemplateUnionTypeDef = Union[PlacementTemplateTypeDef, PlacementTemplateOutputTypeDef]
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects/type_defs.pyi` & `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_iot1click_projects.type_defs import AssociateDeviceWithPlacementRequestRequestTypeDef
 
     data: AssociateDeviceWithPlacementRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
@@ -25,15 +25,14 @@
     "CreatePlacementRequestRequestTypeDef",
     "DeletePlacementRequestRequestTypeDef",
     "DeleteProjectRequestRequestTypeDef",
     "DescribePlacementRequestRequestTypeDef",
     "PlacementDescriptionTypeDef",
     "ResponseMetadataTypeDef",
     "DescribeProjectRequestRequestTypeDef",
-    "DeviceTemplateOutputTypeDef",
     "DeviceTemplateTypeDef",
     "DisassociateDeviceFromPlacementRequestRequestTypeDef",
     "GetDevicesInPlacementRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListPlacementsRequestRequestTypeDef",
     "PlacementSummaryTypeDef",
     "ListProjectsRequestRequestTypeDef",
@@ -41,23 +40,21 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePlacementRequestRequestTypeDef",
     "DescribePlacementResponseTypeDef",
     "GetDevicesInPlacementResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PlacementTemplateOutputTypeDef",
     "PlacementTemplateTypeDef",
     "ListPlacementsRequestListPlacementsPaginateTypeDef",
     "ListProjectsRequestListProjectsPaginateTypeDef",
     "ListPlacementsResponseTypeDef",
     "ListProjectsResponseTypeDef",
-    "ProjectDescriptionTypeDef",
     "CreateProjectRequestRequestTypeDef",
-    "PlacementTemplateUnionTypeDef",
+    "ProjectDescriptionTypeDef",
     "UpdateProjectRequestRequestTypeDef",
     "DescribeProjectResponseTypeDef",
 )
 
 AssociateDeviceWithPlacementRequestRequestTypeDef = TypedDict(
     "AssociateDeviceWithPlacementRequestRequestTypeDef",
     {
@@ -136,23 +133,14 @@
 DescribeProjectRequestRequestTypeDef = TypedDict(
     "DescribeProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 
-DeviceTemplateOutputTypeDef = TypedDict(
-    "DeviceTemplateOutputTypeDef",
-    {
-        "deviceType": str,
-        "callbackOverrides": Dict[str, str],
-    },
-    total=False,
-)
-
 DeviceTemplateTypeDef = TypedDict(
     "DeviceTemplateTypeDef",
     {
         "deviceType": str,
         "callbackOverrides": Mapping[str, str],
     },
     total=False,
@@ -307,23 +295,14 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PlacementTemplateOutputTypeDef = TypedDict(
-    "PlacementTemplateOutputTypeDef",
-    {
-        "defaultAttributes": Dict[str, str],
-        "deviceTemplates": Dict[str, DeviceTemplateOutputTypeDef],
-    },
-    total=False,
-)
-
 PlacementTemplateTypeDef = TypedDict(
     "PlacementTemplateTypeDef",
     {
         "defaultAttributes": Mapping[str, str],
         "deviceTemplates": Mapping[str, DeviceTemplateTypeDef],
     },
     total=False,
@@ -371,60 +350,59 @@
     {
         "projects": List[ProjectSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredProjectDescriptionTypeDef = TypedDict(
-    "_RequiredProjectDescriptionTypeDef",
+_RequiredCreateProjectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProjectRequestRequestTypeDef",
     {
         "projectName": str,
-        "createdDate": datetime,
-        "updatedDate": datetime,
     },
 )
-_OptionalProjectDescriptionTypeDef = TypedDict(
-    "_OptionalProjectDescriptionTypeDef",
+_OptionalCreateProjectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProjectRequestRequestTypeDef",
     {
-        "arn": str,
         "description": str,
-        "placementTemplate": PlacementTemplateOutputTypeDef,
-        "tags": Dict[str, str],
+        "placementTemplate": PlacementTemplateTypeDef,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class ProjectDescriptionTypeDef(
-    _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
+class CreateProjectRequestRequestTypeDef(
+    _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
 ):
     pass
 
-_RequiredCreateProjectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProjectRequestRequestTypeDef",
+_RequiredProjectDescriptionTypeDef = TypedDict(
+    "_RequiredProjectDescriptionTypeDef",
     {
         "projectName": str,
+        "createdDate": datetime,
+        "updatedDate": datetime,
     },
 )
-_OptionalCreateProjectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProjectRequestRequestTypeDef",
+_OptionalProjectDescriptionTypeDef = TypedDict(
+    "_OptionalProjectDescriptionTypeDef",
     {
+        "arn": str,
         "description": str,
         "placementTemplate": PlacementTemplateTypeDef,
-        "tags": Mapping[str, str],
+        "tags": Dict[str, str],
     },
     total=False,
 )
 
-class CreateProjectRequestRequestTypeDef(
-    _RequiredCreateProjectRequestRequestTypeDef, _OptionalCreateProjectRequestRequestTypeDef
+class ProjectDescriptionTypeDef(
+    _RequiredProjectDescriptionTypeDef, _OptionalProjectDescriptionTypeDef
 ):
     pass
 
-PlacementTemplateUnionTypeDef = Union[PlacementTemplateTypeDef, PlacementTemplateOutputTypeDef]
 _RequiredUpdateProjectRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProjectRequestRequestTypeDef",
     {
         "projectName": str,
     },
 )
 _OptionalUpdateProjectRequestRequestTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO` & `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iot1click-projects
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.IoT1ClickProjects 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/
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
 [types-aiobotocore-iot1click-projects docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/).
 
 See how it helps to find and fix potential bugs:
 
@@ -293,74 +293,38 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_iot1click_projects.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `IoT1ClickProjects` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/literals/).
+
 ```python
-from types_aiobotocore_iot1click_projects.literals import (
-    ListPlacementsPaginatorName,
-    ListProjectsPaginatorName,
-    IoT1ClickProjectsServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_iot1click_projects.literals import ListPlacementsPaginatorName
 
 
 def check_value(value: ListPlacementsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_iot1click_projects.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `IoT1ClickProjects` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iot1click_projects/type_defs/).
+
 ```python
 from types_aiobotocore_iot1click_projects.type_defs import (
     AssociateDeviceWithPlacementRequestRequestTypeDef,
-    CreatePlacementRequestRequestTypeDef,
-    DeletePlacementRequestRequestTypeDef,
-    DeleteProjectRequestRequestTypeDef,
-    DescribePlacementRequestRequestTypeDef,
-    PlacementDescriptionTypeDef,
-    ResponseMetadataTypeDef,
-    DescribeProjectRequestRequestTypeDef,
-    DeviceTemplateOutputTypeDef,
-    DeviceTemplateTypeDef,
-    DisassociateDeviceFromPlacementRequestRequestTypeDef,
-    GetDevicesInPlacementRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ListPlacementsRequestRequestTypeDef,
-    PlacementSummaryTypeDef,
-    ListProjectsRequestRequestTypeDef,
-    ProjectSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    UpdatePlacementRequestRequestTypeDef,
-    DescribePlacementResponseTypeDef,
-    GetDevicesInPlacementResponseTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PlacementTemplateOutputTypeDef,
-    PlacementTemplateTypeDef,
-    ListPlacementsRequestListPlacementsPaginateTypeDef,
-    ListProjectsRequestListProjectsPaginateTypeDef,
-    ListPlacementsResponseTypeDef,
-    ListProjectsResponseTypeDef,
-    ProjectDescriptionTypeDef,
-    CreateProjectRequestRequestTypeDef,
-    PlacementTemplateUnionTypeDef,
-    UpdateProjectRequestRequestTypeDef,
-    DescribeProjectResponseTypeDef,
 )
 
 
 def get_value() -> AssociateDeviceWithPlacementRequestRequestTypeDef:
     return {...}
 ```
```

### Comparing `types-aiobotocore-iot1click-projects-2.5.2.post1/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt` & `types-aiobotocore-iot1click-projects-2.5.2.post2/types_aiobotocore_iot1click_projects.egg-info/SOURCES.txt`

 * *Files identical despite different names*

