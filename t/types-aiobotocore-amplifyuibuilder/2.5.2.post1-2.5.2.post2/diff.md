# Comparing `tmp/types-aiobotocore-amplifyuibuilder-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-amplifyuibuilder-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-amplifyuibuilder-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
+gzip compressed data, was "types-aiobotocore-amplifyuibuilder-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:22 2023, max compression
```

## Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1.tar` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.433660 types-aiobotocore-amplifyuibuilder-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-08-02 14:51:50.425660 types-aiobotocore-amplifyuibuilder-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17998 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.433660 types-aiobotocore-amplifyuibuilder-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.425660 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-08-02 14:32:55.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23755 2023-08-02 14:32:55.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-08-02 14:32:55.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-08-02 14:32:55.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-08-02 14:32:55.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-08-02 14:32:55.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58612 2023-08-02 14:32:56.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58502 2023-08-02 14:32:56.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:54.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.425660 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19552 2023-08-02 14:51:50.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:51:50.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:51:50.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.755005 types-aiobotocore-amplifyuibuilder-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:01.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-08-04 12:00:22.755005 types-aiobotocore-amplifyuibuilder-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-08-04 11:40:01.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:22.755005 types-aiobotocore-amplifyuibuilder-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-04 11:40:00.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.751004 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-08-04 11:40:01.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-08-04 11:40:01.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-04 11:40:01.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23796 2023-08-04 11:40:01.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23755 2023-08-04 11:40:01.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-08-04 11:40:01.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10286 2023-08-04 11:40:01.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8895 2023-08-04 11:40:01.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8886 2023-08-04 11:40:01.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:01.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47815 2023-08-04 11:40:03.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47723 2023-08-04 11:40:02.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:01.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:22.755005 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-08-04 12:00:22.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-04 12:00:22.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:22.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:22.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:00:22.000000 types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/LICENSE` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/setup.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-amplifyuibuilder",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_amplifyuibuilder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AmplifyUIBuilder 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/__init__.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/__init__.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/__main__.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.AmplifyUIBuilder 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_amplifyuibuilder//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/amplifyuibuilder.html#AmplifyUIBuilder\nOther"
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

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/client.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/client.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/literals.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/literals.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/paginator.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/paginator.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/type_defs.py` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,80 +39,66 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "MutationActionSetStateParameterTypeDef",
     "CodegenFeatureFlagsTypeDef",
-    "CodegenGenericDataEnumOutputTypeDef",
     "CodegenGenericDataEnumTypeDef",
-    "CodegenGenericDataRelationshipTypeOutputTypeDef",
     "CodegenGenericDataRelationshipTypeTypeDef",
     "CodegenJobAssetTypeDef",
     "ReactStartCodegenJobDataTypeDef",
     "CodegenJobSummaryTypeDef",
-    "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     "ComponentConditionPropertyTypeDef",
     "SortPropertyTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
     "FormBindingElementTypeDef",
     "ComponentSummaryTypeDef",
-    "ComponentVariantOutputTypeDef",
     "ComponentVariantTypeDef",
     "ResponseMetadataTypeDef",
     "FormDataTypeConfigTypeDef",
     "CreateThemeDataTypeDef",
     "ThemeTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteFormRequestRequestTypeDef",
     "DeleteThemeRequestRequestTypeDef",
     "ExchangeCodeForTokenRequestBodyTypeDef",
     "PaginatorConfigTypeDef",
     "ExportComponentsRequestRequestTypeDef",
     "ExportFormsRequestRequestTypeDef",
     "ExportThemesRequestRequestTypeDef",
     "FieldPositionTypeDef",
-    "FieldValidationConfigurationOutputTypeDef",
     "FieldValidationConfigurationTypeDef",
-    "FileUploaderFieldConfigOutputTypeDef",
     "FileUploaderFieldConfigTypeDef",
     "FormInputBindingPropertiesValuePropertiesTypeDef",
     "FormInputValuePropertyBindingPropertiesTypeDef",
     "FormStyleConfigTypeDef",
     "GetCodegenJobRequestRequestTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetFormRequestRequestTypeDef",
     "GetMetadataRequestRequestTypeDef",
     "GetThemeRequestRequestTypeDef",
     "ListCodegenJobsRequestRequestTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListFormsRequestRequestTypeDef",
     "ListThemesRequestRequestTypeDef",
     "ThemeSummaryTypeDef",
-    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "PutMetadataFlagBodyTypeDef",
     "RefreshTokenRequestBodyTypeDef",
-    "ThemeValueOutputTypeDef",
     "ThemeValueTypeDef",
-    "ThemeValuesOutputTypeDef",
     "ThemeValuesTypeDef",
     "UpdateThemeDataTypeDef",
     "ValueMappingTypeDef",
-    "ActionParametersOutputTypeDef",
     "ActionParametersTypeDef",
-    "CodegenGenericDataFieldOutputTypeDef",
     "CodegenGenericDataFieldTypeDef",
     "CodegenJobRenderConfigTypeDef",
-    "ComponentBindingPropertiesValueOutputTypeDef",
     "ComponentBindingPropertiesValueTypeDef",
-    "ComponentDataConfigurationOutputTypeDef",
     "ComponentDataConfigurationTypeDef",
-    "ComponentPropertyOutputTypeDef",
     "ComponentPropertyTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExchangeCodeForTokenResponseTypeDef",
     "GetMetadataResponseTypeDef",
     "ListCodegenJobsResponseTypeDef",
     "ListComponentsResponseTypeDef",
     "RefreshTokenResponseTypeDef",
@@ -135,54 +121,46 @@
     "FormInputBindingPropertiesValueTypeDef",
     "FormInputValuePropertyTypeDef",
     "FormStyleTypeDef",
     "ListThemesResponseTypeDef",
     "PutMetadataFlagRequestRequestTypeDef",
     "RefreshTokenRequestRequestTypeDef",
     "UpdateThemeRequestRequestTypeDef",
-    "ComponentEventOutputTypeDef",
     "ComponentEventTypeDef",
-    "CodegenGenericDataModelOutputTypeDef",
-    "CodegenGenericDataNonModelOutputTypeDef",
     "CodegenGenericDataModelTypeDef",
     "CodegenGenericDataNonModelTypeDef",
     "ListFormsResponseTypeDef",
     "FormCTATypeDef",
-    "ValueMappingsOutputTypeDef",
     "ValueMappingsTypeDef",
-    "ComponentChildOutputTypeDef",
-    "ComponentTypeDef",
     "ComponentChildTypeDef",
+    "ComponentTypeDef",
     "CreateComponentDataTypeDef",
     "UpdateComponentDataTypeDef",
-    "CodegenJobGenericDataSchemaOutputTypeDef",
     "CodegenJobGenericDataSchemaTypeDef",
-    "FieldInputConfigOutputTypeDef",
     "FieldInputConfigTypeDef",
     "CreateComponentResponseTypeDef",
     "ExportComponentsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "UpdateComponentResponseTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "CodegenJobTypeDef",
     "StartCodegenJobDataTypeDef",
-    "FieldConfigOutputTypeDef",
     "FieldConfigTypeDef",
     "GetCodegenJobResponseTypeDef",
     "StartCodegenJobResponseTypeDef",
     "StartCodegenJobRequestRequestTypeDef",
-    "FormTypeDef",
     "CreateFormDataTypeDef",
+    "FormTypeDef",
     "UpdateFormDataTypeDef",
+    "CreateFormRequestRequestTypeDef",
     "CreateFormResponseTypeDef",
     "ExportFormsResponseTypeDef",
     "GetFormResponseTypeDef",
     "UpdateFormResponseTypeDef",
-    "CreateFormRequestRequestTypeDef",
     "UpdateFormRequestRequestTypeDef",
 )
 
 MutationActionSetStateParameterTypeDef = TypedDict(
     "MutationActionSetStateParameterTypeDef",
     {
         "componentName": str,
@@ -196,73 +174,37 @@
     {
         "isRelationshipSupported": bool,
         "isNonModelSupported": bool,
     },
     total=False,
 )
 
-CodegenGenericDataEnumOutputTypeDef = TypedDict(
-    "CodegenGenericDataEnumOutputTypeDef",
-    {
-        "values": List[str],
-    },
-)
-
 CodegenGenericDataEnumTypeDef = TypedDict(
     "CodegenGenericDataEnumTypeDef",
     {
-        "values": Sequence[str],
-    },
-)
-
-_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef",
-    {
-        "type": GenericDataRelationshipTypeType,
-        "relatedModelName": str,
-    },
-)
-_OptionalCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataRelationshipTypeOutputTypeDef",
-    {
-        "relatedModelFields": List[str],
-        "canUnlinkAssociatedModel": bool,
-        "relatedJoinFieldName": str,
-        "relatedJoinTableName": str,
-        "belongsToFieldOnRelatedModel": str,
-        "associatedFields": List[str],
-        "isHasManyIndex": bool,
+        "values": List[str],
     },
-    total=False,
 )
 
-
-class CodegenGenericDataRelationshipTypeOutputTypeDef(
-    _RequiredCodegenGenericDataRelationshipTypeOutputTypeDef,
-    _OptionalCodegenGenericDataRelationshipTypeOutputTypeDef,
-):
-    pass
-
-
 _RequiredCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
     "_RequiredCodegenGenericDataRelationshipTypeTypeDef",
     {
         "type": GenericDataRelationshipTypeType,
         "relatedModelName": str,
     },
 )
 _OptionalCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
     "_OptionalCodegenGenericDataRelationshipTypeTypeDef",
     {
-        "relatedModelFields": Sequence[str],
+        "relatedModelFields": List[str],
         "canUnlinkAssociatedModel": bool,
         "relatedJoinFieldName": str,
         "relatedJoinTableName": str,
         "belongsToFieldOnRelatedModel": str,
-        "associatedFields": Sequence[str],
+        "associatedFields": List[str],
         "isHasManyIndex": bool,
     },
     total=False,
 )
 
 
 class CodegenGenericDataRelationshipTypeTypeDef(
@@ -312,29 +254,14 @@
 
 class CodegenJobSummaryTypeDef(
     _RequiredCodegenJobSummaryTypeDef, _OptionalCodegenJobSummaryTypeDef
 ):
     pass
 
 
-ComponentBindingPropertiesValuePropertiesOutputTypeDef = TypedDict(
-    "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
-    {
-        "model": str,
-        "field": str,
-        "predicates": List["PredicateOutputTypeDef"],
-        "userAttribute": str,
-        "bucket": str,
-        "key": str,
-        "defaultValue": str,
-        "slotName": str,
-    },
-    total=False,
-)
-
 ComponentBindingPropertiesValuePropertiesTypeDef = TypedDict(
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     {
         "model": str,
         "field": str,
         "predicates": Sequence["PredicateTypeDef"],
         "userAttribute": str,
@@ -405,23 +332,14 @@
         "environmentName": str,
         "id": str,
         "name": str,
         "componentType": str,
     },
 )
 
-ComponentVariantOutputTypeDef = TypedDict(
-    "ComponentVariantOutputTypeDef",
-    {
-        "variantValues": Dict[str, str],
-        "overrides": Dict[str, Dict[str, str]],
-    },
-    total=False,
-)
-
 ComponentVariantTypeDef = TypedDict(
     "ComponentVariantTypeDef",
     {
         "variantValues": Mapping[str, str],
         "overrides": Mapping[str, Mapping[str, str]],
     },
     total=False,
@@ -471,22 +389,22 @@
     "_RequiredThemeTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
         "createdAt": datetime,
-        "values": List["ThemeValuesOutputTypeDef"],
+        "values": List["ThemeValuesTypeDef"],
     },
 )
 _OptionalThemeTypeDef = TypedDict(
     "_OptionalThemeTypeDef",
     {
         "modifiedAt": datetime,
-        "overrides": List["ThemeValuesOutputTypeDef"],
+        "overrides": List["ThemeValuesTypeDef"],
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 
 class ThemeTypeDef(_RequiredThemeTypeDef, _OptionalThemeTypeDef):
@@ -624,38 +542,14 @@
         "fixed": Literal["first"],
         "rightOf": str,
         "below": str,
     },
     total=False,
 )
 
-_RequiredFieldValidationConfigurationOutputTypeDef = TypedDict(
-    "_RequiredFieldValidationConfigurationOutputTypeDef",
-    {
-        "type": str,
-    },
-)
-_OptionalFieldValidationConfigurationOutputTypeDef = TypedDict(
-    "_OptionalFieldValidationConfigurationOutputTypeDef",
-    {
-        "strValues": List[str],
-        "numValues": List[int],
-        "validationMessage": str,
-    },
-    total=False,
-)
-
-
-class FieldValidationConfigurationOutputTypeDef(
-    _RequiredFieldValidationConfigurationOutputTypeDef,
-    _OptionalFieldValidationConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredFieldValidationConfigurationTypeDef = TypedDict(
     "_RequiredFieldValidationConfigurationTypeDef",
     {
         "type": str,
     },
 )
 _OptionalFieldValidationConfigurationTypeDef = TypedDict(
@@ -671,39 +565,14 @@
 
 class FieldValidationConfigurationTypeDef(
     _RequiredFieldValidationConfigurationTypeDef, _OptionalFieldValidationConfigurationTypeDef
 ):
     pass
 
 
-_RequiredFileUploaderFieldConfigOutputTypeDef = TypedDict(
-    "_RequiredFileUploaderFieldConfigOutputTypeDef",
-    {
-        "accessLevel": StorageAccessLevelType,
-        "acceptedFileTypes": List[str],
-    },
-)
-_OptionalFileUploaderFieldConfigOutputTypeDef = TypedDict(
-    "_OptionalFileUploaderFieldConfigOutputTypeDef",
-    {
-        "showThumbnails": bool,
-        "isResumable": bool,
-        "maxFileCount": int,
-        "maxSize": int,
-    },
-    total=False,
-)
-
-
-class FileUploaderFieldConfigOutputTypeDef(
-    _RequiredFileUploaderFieldConfigOutputTypeDef, _OptionalFileUploaderFieldConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredFileUploaderFieldConfigTypeDef = TypedDict(
     "_RequiredFileUploaderFieldConfigTypeDef",
     {
         "accessLevel": StorageAccessLevelType,
         "acceptedFileTypes": Sequence[str],
     },
 )
@@ -906,27 +775,14 @@
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
     },
 )
 
-PredicateOutputTypeDef = TypedDict(
-    "PredicateOutputTypeDef",
-    {
-        "or": List[Dict[str, Any]],
-        "and": List[Dict[str, Any]],
-        "field": str,
-        "operator": str,
-        "operand": str,
-        "operandType": str,
-    },
-    total=False,
-)
-
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "or": Sequence[Dict[str, Any]],
         "and": Sequence[Dict[str, Any]],
         "field": str,
         "operator": str,
@@ -960,41 +816,23 @@
 
 class RefreshTokenRequestBodyTypeDef(
     _RequiredRefreshTokenRequestBodyTypeDef, _OptionalRefreshTokenRequestBodyTypeDef
 ):
     pass
 
 
-ThemeValueOutputTypeDef = TypedDict(
-    "ThemeValueOutputTypeDef",
-    {
-        "value": str,
-        "children": List[Dict[str, Any]],
-    },
-    total=False,
-)
-
 ThemeValueTypeDef = TypedDict(
     "ThemeValueTypeDef",
     {
         "value": str,
         "children": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-ThemeValuesOutputTypeDef = TypedDict(
-    "ThemeValuesOutputTypeDef",
-    {
-        "key": str,
-        "value": Dict[str, Any],
-    },
-    total=False,
-)
-
 ThemeValuesTypeDef = TypedDict(
     "ThemeValuesTypeDef",
     {
         "key": str,
         "value": Dict[str, Any],
     },
     total=False,
@@ -1036,30 +874,14 @@
 )
 
 
 class ValueMappingTypeDef(_RequiredValueMappingTypeDef, _OptionalValueMappingTypeDef):
     pass
 
 
-ActionParametersOutputTypeDef = TypedDict(
-    "ActionParametersOutputTypeDef",
-    {
-        "type": "ComponentPropertyOutputTypeDef",
-        "url": "ComponentPropertyOutputTypeDef",
-        "anchor": "ComponentPropertyOutputTypeDef",
-        "target": "ComponentPropertyOutputTypeDef",
-        "global": "ComponentPropertyOutputTypeDef",
-        "model": str,
-        "id": "ComponentPropertyOutputTypeDef",
-        "fields": Dict[str, "ComponentPropertyOutputTypeDef"],
-        "state": MutationActionSetStateParameterTypeDef,
-    },
-    total=False,
-)
-
 ActionParametersTypeDef = TypedDict(
     "ActionParametersTypeDef",
     {
         "type": "ComponentPropertyTypeDef",
         "url": "ComponentPropertyTypeDef",
         "anchor": "ComponentPropertyTypeDef",
         "target": "ComponentPropertyTypeDef",
@@ -1068,39 +890,14 @@
         "id": "ComponentPropertyTypeDef",
         "fields": Mapping[str, "ComponentPropertyTypeDef"],
         "state": MutationActionSetStateParameterTypeDef,
     },
     total=False,
 )
 
-_RequiredCodegenGenericDataFieldOutputTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataFieldOutputTypeDef",
-    {
-        "dataType": CodegenGenericDataFieldDataTypeType,
-        "dataTypeValue": str,
-        "required": bool,
-        "readOnly": bool,
-        "isArray": bool,
-    },
-)
-_OptionalCodegenGenericDataFieldOutputTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataFieldOutputTypeDef",
-    {
-        "relationship": CodegenGenericDataRelationshipTypeOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class CodegenGenericDataFieldOutputTypeDef(
-    _RequiredCodegenGenericDataFieldOutputTypeDef, _OptionalCodegenGenericDataFieldOutputTypeDef
-):
-    pass
-
-
 _RequiredCodegenGenericDataFieldTypeDef = TypedDict(
     "_RequiredCodegenGenericDataFieldTypeDef",
     {
         "dataType": CodegenGenericDataFieldDataTypeType,
         "dataTypeValue": str,
         "required": bool,
         "readOnly": bool,
@@ -1126,58 +923,24 @@
     "CodegenJobRenderConfigTypeDef",
     {
         "react": ReactStartCodegenJobDataTypeDef,
     },
     total=False,
 )
 
-ComponentBindingPropertiesValueOutputTypeDef = TypedDict(
-    "ComponentBindingPropertiesValueOutputTypeDef",
-    {
-        "type": str,
-        "bindingProperties": ComponentBindingPropertiesValuePropertiesOutputTypeDef,
-        "defaultValue": str,
-    },
-    total=False,
-)
-
 ComponentBindingPropertiesValueTypeDef = TypedDict(
     "ComponentBindingPropertiesValueTypeDef",
     {
         "type": str,
         "bindingProperties": ComponentBindingPropertiesValuePropertiesTypeDef,
         "defaultValue": str,
     },
     total=False,
 )
 
-_RequiredComponentDataConfigurationOutputTypeDef = TypedDict(
-    "_RequiredComponentDataConfigurationOutputTypeDef",
-    {
-        "model": str,
-    },
-)
-_OptionalComponentDataConfigurationOutputTypeDef = TypedDict(
-    "_OptionalComponentDataConfigurationOutputTypeDef",
-    {
-        "sort": List[SortPropertyTypeDef],
-        "predicate": "PredicateOutputTypeDef",
-        "identifiers": List[str],
-    },
-    total=False,
-)
-
-
-class ComponentDataConfigurationOutputTypeDef(
-    _RequiredComponentDataConfigurationOutputTypeDef,
-    _OptionalComponentDataConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredComponentDataConfigurationTypeDef = TypedDict(
     "_RequiredComponentDataConfigurationTypeDef",
     {
         "model": str,
     },
 )
 _OptionalComponentDataConfigurationTypeDef = TypedDict(
@@ -1193,36 +956,14 @@
 
 class ComponentDataConfigurationTypeDef(
     _RequiredComponentDataConfigurationTypeDef, _OptionalComponentDataConfigurationTypeDef
 ):
     pass
 
 
-ComponentPropertyOutputTypeDef = TypedDict(
-    "ComponentPropertyOutputTypeDef",
-    {
-        "value": str,
-        "bindingProperties": ComponentPropertyBindingPropertiesTypeDef,
-        "collectionBindingProperties": ComponentPropertyBindingPropertiesTypeDef,
-        "defaultValue": str,
-        "model": str,
-        "bindings": Dict[str, FormBindingElementTypeDef],
-        "event": str,
-        "userAttribute": str,
-        "concat": List[Dict[str, Any]],
-        "condition": "ComponentConditionPropertyTypeDef",
-        "configured": bool,
-        "type": str,
-        "importedValue": str,
-        "componentName": str,
-        "property": str,
-    },
-    total=False,
-)
-
 ComponentPropertyTypeDef = TypedDict(
     "ComponentPropertyTypeDef",
     {
         "value": str,
         "bindingProperties": ComponentPropertyBindingPropertiesTypeDef,
         "collectionBindingProperties": ComponentPropertyBindingPropertiesTypeDef,
         "defaultValue": str,
@@ -1639,68 +1380,29 @@
 
 class UpdateThemeRequestRequestTypeDef(
     _RequiredUpdateThemeRequestRequestTypeDef, _OptionalUpdateThemeRequestRequestTypeDef
 ):
     pass
 
 
-ComponentEventOutputTypeDef = TypedDict(
-    "ComponentEventOutputTypeDef",
-    {
-        "action": str,
-        "parameters": ActionParametersOutputTypeDef,
-        "bindingEvent": str,
-    },
-    total=False,
-)
-
 ComponentEventTypeDef = TypedDict(
     "ComponentEventTypeDef",
     {
         "action": str,
         "parameters": ActionParametersTypeDef,
         "bindingEvent": str,
     },
     total=False,
 )
 
-_RequiredCodegenGenericDataModelOutputTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataModelOutputTypeDef",
-    {
-        "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
-        "primaryKeys": List[str],
-    },
-)
-_OptionalCodegenGenericDataModelOutputTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataModelOutputTypeDef",
-    {
-        "isJoinTable": bool,
-    },
-    total=False,
-)
-
-
-class CodegenGenericDataModelOutputTypeDef(
-    _RequiredCodegenGenericDataModelOutputTypeDef, _OptionalCodegenGenericDataModelOutputTypeDef
-):
-    pass
-
-
-CodegenGenericDataNonModelOutputTypeDef = TypedDict(
-    "CodegenGenericDataNonModelOutputTypeDef",
-    {
-        "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
-    },
-)
-
 _RequiredCodegenGenericDataModelTypeDef = TypedDict(
     "_RequiredCodegenGenericDataModelTypeDef",
     {
-        "fields": Mapping[str, CodegenGenericDataFieldTypeDef],
-        "primaryKeys": Sequence[str],
+        "fields": Dict[str, CodegenGenericDataFieldTypeDef],
+        "primaryKeys": List[str],
     },
 )
 _OptionalCodegenGenericDataModelTypeDef = TypedDict(
     "_OptionalCodegenGenericDataModelTypeDef",
     {
         "isJoinTable": bool,
     },
@@ -1713,15 +1415,15 @@
 ):
     pass
 
 
 CodegenGenericDataNonModelTypeDef = TypedDict(
     "CodegenGenericDataNonModelTypeDef",
     {
-        "fields": Mapping[str, CodegenGenericDataFieldTypeDef],
+        "fields": Dict[str, CodegenGenericDataFieldTypeDef],
     },
 )
 
 ListFormsResponseTypeDef = TypedDict(
     "ListFormsResponseTypeDef",
     {
         "entities": List[FormSummaryTypeDef],
@@ -1737,35 +1439,14 @@
         "clear": FormButtonTypeDef,
         "cancel": FormButtonTypeDef,
         "submit": FormButtonTypeDef,
     },
     total=False,
 )
 
-_RequiredValueMappingsOutputTypeDef = TypedDict(
-    "_RequiredValueMappingsOutputTypeDef",
-    {
-        "values": List[ValueMappingTypeDef],
-    },
-)
-_OptionalValueMappingsOutputTypeDef = TypedDict(
-    "_OptionalValueMappingsOutputTypeDef",
-    {
-        "bindingProperties": Dict[str, FormInputBindingPropertiesValueTypeDef],
-    },
-    total=False,
-)
-
-
-class ValueMappingsOutputTypeDef(
-    _RequiredValueMappingsOutputTypeDef, _OptionalValueMappingsOutputTypeDef
-):
-    pass
-
-
 _RequiredValueMappingsTypeDef = TypedDict(
     "_RequiredValueMappingsTypeDef",
     {
         "values": Sequence[ValueMappingTypeDef],
     },
 )
 _OptionalValueMappingsTypeDef = TypedDict(
@@ -1777,96 +1458,71 @@
 )
 
 
 class ValueMappingsTypeDef(_RequiredValueMappingsTypeDef, _OptionalValueMappingsTypeDef):
     pass
 
 
-_RequiredComponentChildOutputTypeDef = TypedDict(
-    "_RequiredComponentChildOutputTypeDef",
+_RequiredComponentChildTypeDef = TypedDict(
+    "_RequiredComponentChildTypeDef",
     {
         "componentType": str,
         "name": str,
-        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "properties": Mapping[str, "ComponentPropertyTypeDef"],
     },
 )
-_OptionalComponentChildOutputTypeDef = TypedDict(
-    "_OptionalComponentChildOutputTypeDef",
+_OptionalComponentChildTypeDef = TypedDict(
+    "_OptionalComponentChildTypeDef",
     {
-        "children": List[Dict[str, Any]],
-        "events": Dict[str, ComponentEventOutputTypeDef],
+        "children": Sequence[Dict[str, Any]],
+        "events": Mapping[str, ComponentEventTypeDef],
         "sourceId": str,
     },
     total=False,
 )
 
 
-class ComponentChildOutputTypeDef(
-    _RequiredComponentChildOutputTypeDef, _OptionalComponentChildOutputTypeDef
-):
+class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
     pass
 
 
 _RequiredComponentTypeDef = TypedDict(
     "_RequiredComponentTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
         "componentType": str,
-        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
-        "variants": List[ComponentVariantOutputTypeDef],
+        "properties": Dict[str, "ComponentPropertyTypeDef"],
+        "variants": List[ComponentVariantTypeDef],
         "overrides": Dict[str, Dict[str, str]],
-        "bindingProperties": Dict[str, ComponentBindingPropertiesValueOutputTypeDef],
+        "bindingProperties": Dict[str, ComponentBindingPropertiesValueTypeDef],
         "createdAt": datetime,
     },
 )
 _OptionalComponentTypeDef = TypedDict(
     "_OptionalComponentTypeDef",
     {
         "sourceId": str,
-        "children": List["ComponentChildOutputTypeDef"],
-        "collectionProperties": Dict[str, ComponentDataConfigurationOutputTypeDef],
+        "children": List["ComponentChildTypeDef"],
+        "collectionProperties": Dict[str, ComponentDataConfigurationTypeDef],
         "modifiedAt": datetime,
         "tags": Dict[str, str],
-        "events": Dict[str, ComponentEventOutputTypeDef],
+        "events": Dict[str, ComponentEventTypeDef],
         "schemaVersion": str,
     },
     total=False,
 )
 
 
 class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
     pass
 
 
-_RequiredComponentChildTypeDef = TypedDict(
-    "_RequiredComponentChildTypeDef",
-    {
-        "componentType": str,
-        "name": str,
-        "properties": Mapping[str, "ComponentPropertyTypeDef"],
-    },
-)
-_OptionalComponentChildTypeDef = TypedDict(
-    "_OptionalComponentChildTypeDef",
-    {
-        "children": Sequence[Dict[str, Any]],
-        "events": Mapping[str, ComponentEventTypeDef],
-        "sourceId": str,
-    },
-    total=False,
-)
-
-
-class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
-    pass
-
-
 _RequiredCreateComponentDataTypeDef = TypedDict(
     "_RequiredCreateComponentDataTypeDef",
     {
         "name": str,
         "componentType": str,
         "properties": Mapping[str, "ComponentPropertyTypeDef"],
         "variants": Sequence[ComponentVariantTypeDef],
@@ -1909,69 +1565,24 @@
         "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
         "events": Mapping[str, ComponentEventTypeDef],
         "schemaVersion": str,
     },
     total=False,
 )
 
-CodegenJobGenericDataSchemaOutputTypeDef = TypedDict(
-    "CodegenJobGenericDataSchemaOutputTypeDef",
-    {
-        "dataSourceType": Literal["DataStore"],
-        "models": Dict[str, CodegenGenericDataModelOutputTypeDef],
-        "enums": Dict[str, CodegenGenericDataEnumOutputTypeDef],
-        "nonModels": Dict[str, CodegenGenericDataNonModelOutputTypeDef],
-    },
-)
-
 CodegenJobGenericDataSchemaTypeDef = TypedDict(
     "CodegenJobGenericDataSchemaTypeDef",
     {
         "dataSourceType": Literal["DataStore"],
-        "models": Mapping[str, CodegenGenericDataModelTypeDef],
-        "enums": Mapping[str, CodegenGenericDataEnumTypeDef],
-        "nonModels": Mapping[str, CodegenGenericDataNonModelTypeDef],
-    },
-)
-
-_RequiredFieldInputConfigOutputTypeDef = TypedDict(
-    "_RequiredFieldInputConfigOutputTypeDef",
-    {
-        "type": str,
-    },
-)
-_OptionalFieldInputConfigOutputTypeDef = TypedDict(
-    "_OptionalFieldInputConfigOutputTypeDef",
-    {
-        "required": bool,
-        "readOnly": bool,
-        "placeholder": str,
-        "defaultValue": str,
-        "descriptiveText": str,
-        "defaultChecked": bool,
-        "defaultCountryCode": str,
-        "valueMappings": ValueMappingsOutputTypeDef,
-        "name": str,
-        "minValue": float,
-        "maxValue": float,
-        "step": float,
-        "value": str,
-        "isArray": bool,
-        "fileUploaderConfig": FileUploaderFieldConfigOutputTypeDef,
+        "models": Dict[str, CodegenGenericDataModelTypeDef],
+        "enums": Dict[str, CodegenGenericDataEnumTypeDef],
+        "nonModels": Dict[str, CodegenGenericDataNonModelTypeDef],
     },
-    total=False,
 )
 
-
-class FieldInputConfigOutputTypeDef(
-    _RequiredFieldInputConfigOutputTypeDef, _OptionalFieldInputConfigOutputTypeDef
-):
-    pass
-
-
 _RequiredFieldInputConfigTypeDef = TypedDict(
     "_RequiredFieldInputConfigTypeDef",
     {
         "type": str,
     },
 )
 _OptionalFieldInputConfigTypeDef = TypedDict(
@@ -2089,15 +1700,15 @@
         "environmentName": str,
     },
 )
 _OptionalCodegenJobTypeDef = TypedDict(
     "_OptionalCodegenJobTypeDef",
     {
         "renderConfig": CodegenJobRenderConfigTypeDef,
-        "genericDataSchema": CodegenJobGenericDataSchemaOutputTypeDef,
+        "genericDataSchema": CodegenJobGenericDataSchemaTypeDef,
         "autoGenerateForms": bool,
         "features": CodegenFeatureFlagsTypeDef,
         "status": CodegenJobStatusType,
         "statusMessage": str,
         "asset": CodegenJobAssetTypeDef,
         "tags": Dict[str, str],
         "createdAt": datetime,
@@ -2131,26 +1742,14 @@
 
 class StartCodegenJobDataTypeDef(
     _RequiredStartCodegenJobDataTypeDef, _OptionalStartCodegenJobDataTypeDef
 ):
     pass
 
 
-FieldConfigOutputTypeDef = TypedDict(
-    "FieldConfigOutputTypeDef",
-    {
-        "label": str,
-        "position": FieldPositionTypeDef,
-        "excluded": bool,
-        "inputType": FieldInputConfigOutputTypeDef,
-        "validations": List[FieldValidationConfigurationOutputTypeDef],
-    },
-    total=False,
-)
-
 FieldConfigTypeDef = TypedDict(
     "FieldConfigTypeDef",
     {
         "label": str,
         "position": FieldPositionTypeDef,
         "excluded": bool,
         "inputType": FieldInputConfigTypeDef,
@@ -2194,68 +1793,68 @@
 
 class StartCodegenJobRequestRequestTypeDef(
     _RequiredStartCodegenJobRequestRequestTypeDef, _OptionalStartCodegenJobRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredFormTypeDef = TypedDict(
-    "_RequiredFormTypeDef",
+_RequiredCreateFormDataTypeDef = TypedDict(
+    "_RequiredCreateFormDataTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
         "name": str,
+        "dataType": FormDataTypeConfigTypeDef,
         "formActionType": FormActionTypeType,
+        "fields": Mapping[str, FieldConfigTypeDef],
         "style": FormStyleTypeDef,
-        "dataType": FormDataTypeConfigTypeDef,
-        "fields": Dict[str, FieldConfigOutputTypeDef],
-        "sectionalElements": Dict[str, SectionalElementTypeDef],
+        "sectionalElements": Mapping[str, SectionalElementTypeDef],
         "schemaVersion": str,
     },
 )
-_OptionalFormTypeDef = TypedDict(
-    "_OptionalFormTypeDef",
+_OptionalCreateFormDataTypeDef = TypedDict(
+    "_OptionalCreateFormDataTypeDef",
     {
-        "tags": Dict[str, str],
         "cta": FormCTATypeDef,
+        "tags": Mapping[str, str],
         "labelDecorator": LabelDecoratorType,
     },
     total=False,
 )
 
 
-class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
+class CreateFormDataTypeDef(_RequiredCreateFormDataTypeDef, _OptionalCreateFormDataTypeDef):
     pass
 
 
-_RequiredCreateFormDataTypeDef = TypedDict(
-    "_RequiredCreateFormDataTypeDef",
+_RequiredFormTypeDef = TypedDict(
+    "_RequiredFormTypeDef",
     {
+        "appId": str,
+        "environmentName": str,
+        "id": str,
         "name": str,
-        "dataType": FormDataTypeConfigTypeDef,
         "formActionType": FormActionTypeType,
-        "fields": Mapping[str, FieldConfigTypeDef],
         "style": FormStyleTypeDef,
-        "sectionalElements": Mapping[str, SectionalElementTypeDef],
+        "dataType": FormDataTypeConfigTypeDef,
+        "fields": Dict[str, FieldConfigTypeDef],
+        "sectionalElements": Dict[str, SectionalElementTypeDef],
         "schemaVersion": str,
     },
 )
-_OptionalCreateFormDataTypeDef = TypedDict(
-    "_OptionalCreateFormDataTypeDef",
+_OptionalFormTypeDef = TypedDict(
+    "_OptionalFormTypeDef",
     {
+        "tags": Dict[str, str],
         "cta": FormCTATypeDef,
-        "tags": Mapping[str, str],
         "labelDecorator": LabelDecoratorType,
     },
     total=False,
 )
 
 
-class CreateFormDataTypeDef(_RequiredCreateFormDataTypeDef, _OptionalCreateFormDataTypeDef):
+class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
     pass
 
 
 UpdateFormDataTypeDef = TypedDict(
     "UpdateFormDataTypeDef",
     {
         "name": str,
@@ -2267,14 +1866,37 @@
         "schemaVersion": str,
         "cta": FormCTATypeDef,
         "labelDecorator": LabelDecoratorType,
     },
     total=False,
 )
 
+_RequiredCreateFormRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFormRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "formToCreate": CreateFormDataTypeDef,
+    },
+)
+_OptionalCreateFormRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFormRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateFormRequestRequestTypeDef(
+    _RequiredCreateFormRequestRequestTypeDef, _OptionalCreateFormRequestRequestTypeDef
+):
+    pass
+
+
 CreateFormResponseTypeDef = TypedDict(
     "CreateFormResponseTypeDef",
     {
         "entity": FormTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2300,37 +1922,14 @@
     "UpdateFormResponseTypeDef",
     {
         "entity": FormTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateFormRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFormRequestRequestTypeDef",
-    {
-        "appId": str,
-        "environmentName": str,
-        "formToCreate": CreateFormDataTypeDef,
-    },
-)
-_OptionalCreateFormRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFormRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateFormRequestRequestTypeDef(
-    _RequiredCreateFormRequestRequestTypeDef, _OptionalCreateFormRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateFormRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFormRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "updatedForm": UpdateFormDataTypeDef,
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder/type_defs.pyi` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -38,80 +38,66 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "MutationActionSetStateParameterTypeDef",
     "CodegenFeatureFlagsTypeDef",
-    "CodegenGenericDataEnumOutputTypeDef",
     "CodegenGenericDataEnumTypeDef",
-    "CodegenGenericDataRelationshipTypeOutputTypeDef",
     "CodegenGenericDataRelationshipTypeTypeDef",
     "CodegenJobAssetTypeDef",
     "ReactStartCodegenJobDataTypeDef",
     "CodegenJobSummaryTypeDef",
-    "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     "ComponentConditionPropertyTypeDef",
     "SortPropertyTypeDef",
     "ComponentPropertyBindingPropertiesTypeDef",
     "FormBindingElementTypeDef",
     "ComponentSummaryTypeDef",
-    "ComponentVariantOutputTypeDef",
     "ComponentVariantTypeDef",
     "ResponseMetadataTypeDef",
     "FormDataTypeConfigTypeDef",
     "CreateThemeDataTypeDef",
     "ThemeTypeDef",
     "DeleteComponentRequestRequestTypeDef",
     "DeleteFormRequestRequestTypeDef",
     "DeleteThemeRequestRequestTypeDef",
     "ExchangeCodeForTokenRequestBodyTypeDef",
     "PaginatorConfigTypeDef",
     "ExportComponentsRequestRequestTypeDef",
     "ExportFormsRequestRequestTypeDef",
     "ExportThemesRequestRequestTypeDef",
     "FieldPositionTypeDef",
-    "FieldValidationConfigurationOutputTypeDef",
     "FieldValidationConfigurationTypeDef",
-    "FileUploaderFieldConfigOutputTypeDef",
     "FileUploaderFieldConfigTypeDef",
     "FormInputBindingPropertiesValuePropertiesTypeDef",
     "FormInputValuePropertyBindingPropertiesTypeDef",
     "FormStyleConfigTypeDef",
     "GetCodegenJobRequestRequestTypeDef",
     "GetComponentRequestRequestTypeDef",
     "GetFormRequestRequestTypeDef",
     "GetMetadataRequestRequestTypeDef",
     "GetThemeRequestRequestTypeDef",
     "ListCodegenJobsRequestRequestTypeDef",
     "ListComponentsRequestRequestTypeDef",
     "ListFormsRequestRequestTypeDef",
     "ListThemesRequestRequestTypeDef",
     "ThemeSummaryTypeDef",
-    "PredicateOutputTypeDef",
     "PredicateTypeDef",
     "PutMetadataFlagBodyTypeDef",
     "RefreshTokenRequestBodyTypeDef",
-    "ThemeValueOutputTypeDef",
     "ThemeValueTypeDef",
-    "ThemeValuesOutputTypeDef",
     "ThemeValuesTypeDef",
     "UpdateThemeDataTypeDef",
     "ValueMappingTypeDef",
-    "ActionParametersOutputTypeDef",
     "ActionParametersTypeDef",
-    "CodegenGenericDataFieldOutputTypeDef",
     "CodegenGenericDataFieldTypeDef",
     "CodegenJobRenderConfigTypeDef",
-    "ComponentBindingPropertiesValueOutputTypeDef",
     "ComponentBindingPropertiesValueTypeDef",
-    "ComponentDataConfigurationOutputTypeDef",
     "ComponentDataConfigurationTypeDef",
-    "ComponentPropertyOutputTypeDef",
     "ComponentPropertyTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ExchangeCodeForTokenResponseTypeDef",
     "GetMetadataResponseTypeDef",
     "ListCodegenJobsResponseTypeDef",
     "ListComponentsResponseTypeDef",
     "RefreshTokenResponseTypeDef",
@@ -134,54 +120,46 @@
     "FormInputBindingPropertiesValueTypeDef",
     "FormInputValuePropertyTypeDef",
     "FormStyleTypeDef",
     "ListThemesResponseTypeDef",
     "PutMetadataFlagRequestRequestTypeDef",
     "RefreshTokenRequestRequestTypeDef",
     "UpdateThemeRequestRequestTypeDef",
-    "ComponentEventOutputTypeDef",
     "ComponentEventTypeDef",
-    "CodegenGenericDataModelOutputTypeDef",
-    "CodegenGenericDataNonModelOutputTypeDef",
     "CodegenGenericDataModelTypeDef",
     "CodegenGenericDataNonModelTypeDef",
     "ListFormsResponseTypeDef",
     "FormCTATypeDef",
-    "ValueMappingsOutputTypeDef",
     "ValueMappingsTypeDef",
-    "ComponentChildOutputTypeDef",
-    "ComponentTypeDef",
     "ComponentChildTypeDef",
+    "ComponentTypeDef",
     "CreateComponentDataTypeDef",
     "UpdateComponentDataTypeDef",
-    "CodegenJobGenericDataSchemaOutputTypeDef",
     "CodegenJobGenericDataSchemaTypeDef",
-    "FieldInputConfigOutputTypeDef",
     "FieldInputConfigTypeDef",
     "CreateComponentResponseTypeDef",
     "ExportComponentsResponseTypeDef",
     "GetComponentResponseTypeDef",
     "UpdateComponentResponseTypeDef",
     "CreateComponentRequestRequestTypeDef",
     "UpdateComponentRequestRequestTypeDef",
     "CodegenJobTypeDef",
     "StartCodegenJobDataTypeDef",
-    "FieldConfigOutputTypeDef",
     "FieldConfigTypeDef",
     "GetCodegenJobResponseTypeDef",
     "StartCodegenJobResponseTypeDef",
     "StartCodegenJobRequestRequestTypeDef",
-    "FormTypeDef",
     "CreateFormDataTypeDef",
+    "FormTypeDef",
     "UpdateFormDataTypeDef",
+    "CreateFormRequestRequestTypeDef",
     "CreateFormResponseTypeDef",
     "ExportFormsResponseTypeDef",
     "GetFormResponseTypeDef",
     "UpdateFormResponseTypeDef",
-    "CreateFormRequestRequestTypeDef",
     "UpdateFormRequestRequestTypeDef",
 )
 
 MutationActionSetStateParameterTypeDef = TypedDict(
     "MutationActionSetStateParameterTypeDef",
     {
         "componentName": str,
@@ -195,71 +173,37 @@
     {
         "isRelationshipSupported": bool,
         "isNonModelSupported": bool,
     },
     total=False,
 )
 
-CodegenGenericDataEnumOutputTypeDef = TypedDict(
-    "CodegenGenericDataEnumOutputTypeDef",
-    {
-        "values": List[str],
-    },
-)
-
 CodegenGenericDataEnumTypeDef = TypedDict(
     "CodegenGenericDataEnumTypeDef",
     {
-        "values": Sequence[str],
-    },
-)
-
-_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataRelationshipTypeOutputTypeDef",
-    {
-        "type": GenericDataRelationshipTypeType,
-        "relatedModelName": str,
-    },
-)
-_OptionalCodegenGenericDataRelationshipTypeOutputTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataRelationshipTypeOutputTypeDef",
-    {
-        "relatedModelFields": List[str],
-        "canUnlinkAssociatedModel": bool,
-        "relatedJoinFieldName": str,
-        "relatedJoinTableName": str,
-        "belongsToFieldOnRelatedModel": str,
-        "associatedFields": List[str],
-        "isHasManyIndex": bool,
+        "values": List[str],
     },
-    total=False,
 )
 
-class CodegenGenericDataRelationshipTypeOutputTypeDef(
-    _RequiredCodegenGenericDataRelationshipTypeOutputTypeDef,
-    _OptionalCodegenGenericDataRelationshipTypeOutputTypeDef,
-):
-    pass
-
 _RequiredCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
     "_RequiredCodegenGenericDataRelationshipTypeTypeDef",
     {
         "type": GenericDataRelationshipTypeType,
         "relatedModelName": str,
     },
 )
 _OptionalCodegenGenericDataRelationshipTypeTypeDef = TypedDict(
     "_OptionalCodegenGenericDataRelationshipTypeTypeDef",
     {
-        "relatedModelFields": Sequence[str],
+        "relatedModelFields": List[str],
         "canUnlinkAssociatedModel": bool,
         "relatedJoinFieldName": str,
         "relatedJoinTableName": str,
         "belongsToFieldOnRelatedModel": str,
-        "associatedFields": Sequence[str],
+        "associatedFields": List[str],
         "isHasManyIndex": bool,
     },
     total=False,
 )
 
 class CodegenGenericDataRelationshipTypeTypeDef(
     _RequiredCodegenGenericDataRelationshipTypeTypeDef,
@@ -305,29 +249,14 @@
 )
 
 class CodegenJobSummaryTypeDef(
     _RequiredCodegenJobSummaryTypeDef, _OptionalCodegenJobSummaryTypeDef
 ):
     pass
 
-ComponentBindingPropertiesValuePropertiesOutputTypeDef = TypedDict(
-    "ComponentBindingPropertiesValuePropertiesOutputTypeDef",
-    {
-        "model": str,
-        "field": str,
-        "predicates": List["PredicateOutputTypeDef"],
-        "userAttribute": str,
-        "bucket": str,
-        "key": str,
-        "defaultValue": str,
-        "slotName": str,
-    },
-    total=False,
-)
-
 ComponentBindingPropertiesValuePropertiesTypeDef = TypedDict(
     "ComponentBindingPropertiesValuePropertiesTypeDef",
     {
         "model": str,
         "field": str,
         "predicates": Sequence["PredicateTypeDef"],
         "userAttribute": str,
@@ -396,23 +325,14 @@
         "environmentName": str,
         "id": str,
         "name": str,
         "componentType": str,
     },
 )
 
-ComponentVariantOutputTypeDef = TypedDict(
-    "ComponentVariantOutputTypeDef",
-    {
-        "variantValues": Dict[str, str],
-        "overrides": Dict[str, Dict[str, str]],
-    },
-    total=False,
-)
-
 ComponentVariantTypeDef = TypedDict(
     "ComponentVariantTypeDef",
     {
         "variantValues": Mapping[str, str],
         "overrides": Mapping[str, Mapping[str, str]],
     },
     total=False,
@@ -460,22 +380,22 @@
     "_RequiredThemeTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
         "createdAt": datetime,
-        "values": List["ThemeValuesOutputTypeDef"],
+        "values": List["ThemeValuesTypeDef"],
     },
 )
 _OptionalThemeTypeDef = TypedDict(
     "_OptionalThemeTypeDef",
     {
         "modifiedAt": datetime,
-        "overrides": List["ThemeValuesOutputTypeDef"],
+        "overrides": List["ThemeValuesTypeDef"],
         "tags": Dict[str, str],
     },
     total=False,
 )
 
 class ThemeTypeDef(_RequiredThemeTypeDef, _OptionalThemeTypeDef):
     pass
@@ -603,36 +523,14 @@
         "fixed": Literal["first"],
         "rightOf": str,
         "below": str,
     },
     total=False,
 )
 
-_RequiredFieldValidationConfigurationOutputTypeDef = TypedDict(
-    "_RequiredFieldValidationConfigurationOutputTypeDef",
-    {
-        "type": str,
-    },
-)
-_OptionalFieldValidationConfigurationOutputTypeDef = TypedDict(
-    "_OptionalFieldValidationConfigurationOutputTypeDef",
-    {
-        "strValues": List[str],
-        "numValues": List[int],
-        "validationMessage": str,
-    },
-    total=False,
-)
-
-class FieldValidationConfigurationOutputTypeDef(
-    _RequiredFieldValidationConfigurationOutputTypeDef,
-    _OptionalFieldValidationConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredFieldValidationConfigurationTypeDef = TypedDict(
     "_RequiredFieldValidationConfigurationTypeDef",
     {
         "type": str,
     },
 )
 _OptionalFieldValidationConfigurationTypeDef = TypedDict(
@@ -646,37 +544,14 @@
 )
 
 class FieldValidationConfigurationTypeDef(
     _RequiredFieldValidationConfigurationTypeDef, _OptionalFieldValidationConfigurationTypeDef
 ):
     pass
 
-_RequiredFileUploaderFieldConfigOutputTypeDef = TypedDict(
-    "_RequiredFileUploaderFieldConfigOutputTypeDef",
-    {
-        "accessLevel": StorageAccessLevelType,
-        "acceptedFileTypes": List[str],
-    },
-)
-_OptionalFileUploaderFieldConfigOutputTypeDef = TypedDict(
-    "_OptionalFileUploaderFieldConfigOutputTypeDef",
-    {
-        "showThumbnails": bool,
-        "isResumable": bool,
-        "maxFileCount": int,
-        "maxSize": int,
-    },
-    total=False,
-)
-
-class FileUploaderFieldConfigOutputTypeDef(
-    _RequiredFileUploaderFieldConfigOutputTypeDef, _OptionalFileUploaderFieldConfigOutputTypeDef
-):
-    pass
-
 _RequiredFileUploaderFieldConfigTypeDef = TypedDict(
     "_RequiredFileUploaderFieldConfigTypeDef",
     {
         "accessLevel": StorageAccessLevelType,
         "acceptedFileTypes": Sequence[str],
     },
 )
@@ -867,27 +742,14 @@
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
     },
 )
 
-PredicateOutputTypeDef = TypedDict(
-    "PredicateOutputTypeDef",
-    {
-        "or": List[Dict[str, Any]],
-        "and": List[Dict[str, Any]],
-        "field": str,
-        "operator": str,
-        "operand": str,
-        "operandType": str,
-    },
-    total=False,
-)
-
 PredicateTypeDef = TypedDict(
     "PredicateTypeDef",
     {
         "or": Sequence[Dict[str, Any]],
         "and": Sequence[Dict[str, Any]],
         "field": str,
         "operator": str,
@@ -919,41 +781,23 @@
 )
 
 class RefreshTokenRequestBodyTypeDef(
     _RequiredRefreshTokenRequestBodyTypeDef, _OptionalRefreshTokenRequestBodyTypeDef
 ):
     pass
 
-ThemeValueOutputTypeDef = TypedDict(
-    "ThemeValueOutputTypeDef",
-    {
-        "value": str,
-        "children": List[Dict[str, Any]],
-    },
-    total=False,
-)
-
 ThemeValueTypeDef = TypedDict(
     "ThemeValueTypeDef",
     {
         "value": str,
         "children": Sequence[Dict[str, Any]],
     },
     total=False,
 )
 
-ThemeValuesOutputTypeDef = TypedDict(
-    "ThemeValuesOutputTypeDef",
-    {
-        "key": str,
-        "value": Dict[str, Any],
-    },
-    total=False,
-)
-
 ThemeValuesTypeDef = TypedDict(
     "ThemeValuesTypeDef",
     {
         "key": str,
         "value": Dict[str, Any],
     },
     total=False,
@@ -991,30 +835,14 @@
     },
     total=False,
 )
 
 class ValueMappingTypeDef(_RequiredValueMappingTypeDef, _OptionalValueMappingTypeDef):
     pass
 
-ActionParametersOutputTypeDef = TypedDict(
-    "ActionParametersOutputTypeDef",
-    {
-        "type": "ComponentPropertyOutputTypeDef",
-        "url": "ComponentPropertyOutputTypeDef",
-        "anchor": "ComponentPropertyOutputTypeDef",
-        "target": "ComponentPropertyOutputTypeDef",
-        "global": "ComponentPropertyOutputTypeDef",
-        "model": str,
-        "id": "ComponentPropertyOutputTypeDef",
-        "fields": Dict[str, "ComponentPropertyOutputTypeDef"],
-        "state": MutationActionSetStateParameterTypeDef,
-    },
-    total=False,
-)
-
 ActionParametersTypeDef = TypedDict(
     "ActionParametersTypeDef",
     {
         "type": "ComponentPropertyTypeDef",
         "url": "ComponentPropertyTypeDef",
         "anchor": "ComponentPropertyTypeDef",
         "target": "ComponentPropertyTypeDef",
@@ -1023,37 +851,14 @@
         "id": "ComponentPropertyTypeDef",
         "fields": Mapping[str, "ComponentPropertyTypeDef"],
         "state": MutationActionSetStateParameterTypeDef,
     },
     total=False,
 )
 
-_RequiredCodegenGenericDataFieldOutputTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataFieldOutputTypeDef",
-    {
-        "dataType": CodegenGenericDataFieldDataTypeType,
-        "dataTypeValue": str,
-        "required": bool,
-        "readOnly": bool,
-        "isArray": bool,
-    },
-)
-_OptionalCodegenGenericDataFieldOutputTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataFieldOutputTypeDef",
-    {
-        "relationship": CodegenGenericDataRelationshipTypeOutputTypeDef,
-    },
-    total=False,
-)
-
-class CodegenGenericDataFieldOutputTypeDef(
-    _RequiredCodegenGenericDataFieldOutputTypeDef, _OptionalCodegenGenericDataFieldOutputTypeDef
-):
-    pass
-
 _RequiredCodegenGenericDataFieldTypeDef = TypedDict(
     "_RequiredCodegenGenericDataFieldTypeDef",
     {
         "dataType": CodegenGenericDataFieldDataTypeType,
         "dataTypeValue": str,
         "required": bool,
         "readOnly": bool,
@@ -1077,56 +882,24 @@
     "CodegenJobRenderConfigTypeDef",
     {
         "react": ReactStartCodegenJobDataTypeDef,
     },
     total=False,
 )
 
-ComponentBindingPropertiesValueOutputTypeDef = TypedDict(
-    "ComponentBindingPropertiesValueOutputTypeDef",
-    {
-        "type": str,
-        "bindingProperties": ComponentBindingPropertiesValuePropertiesOutputTypeDef,
-        "defaultValue": str,
-    },
-    total=False,
-)
-
 ComponentBindingPropertiesValueTypeDef = TypedDict(
     "ComponentBindingPropertiesValueTypeDef",
     {
         "type": str,
         "bindingProperties": ComponentBindingPropertiesValuePropertiesTypeDef,
         "defaultValue": str,
     },
     total=False,
 )
 
-_RequiredComponentDataConfigurationOutputTypeDef = TypedDict(
-    "_RequiredComponentDataConfigurationOutputTypeDef",
-    {
-        "model": str,
-    },
-)
-_OptionalComponentDataConfigurationOutputTypeDef = TypedDict(
-    "_OptionalComponentDataConfigurationOutputTypeDef",
-    {
-        "sort": List[SortPropertyTypeDef],
-        "predicate": "PredicateOutputTypeDef",
-        "identifiers": List[str],
-    },
-    total=False,
-)
-
-class ComponentDataConfigurationOutputTypeDef(
-    _RequiredComponentDataConfigurationOutputTypeDef,
-    _OptionalComponentDataConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredComponentDataConfigurationTypeDef = TypedDict(
     "_RequiredComponentDataConfigurationTypeDef",
     {
         "model": str,
     },
 )
 _OptionalComponentDataConfigurationTypeDef = TypedDict(
@@ -1140,36 +913,14 @@
 )
 
 class ComponentDataConfigurationTypeDef(
     _RequiredComponentDataConfigurationTypeDef, _OptionalComponentDataConfigurationTypeDef
 ):
     pass
 
-ComponentPropertyOutputTypeDef = TypedDict(
-    "ComponentPropertyOutputTypeDef",
-    {
-        "value": str,
-        "bindingProperties": ComponentPropertyBindingPropertiesTypeDef,
-        "collectionBindingProperties": ComponentPropertyBindingPropertiesTypeDef,
-        "defaultValue": str,
-        "model": str,
-        "bindings": Dict[str, FormBindingElementTypeDef],
-        "event": str,
-        "userAttribute": str,
-        "concat": List[Dict[str, Any]],
-        "condition": "ComponentConditionPropertyTypeDef",
-        "configured": bool,
-        "type": str,
-        "importedValue": str,
-        "componentName": str,
-        "property": str,
-    },
-    total=False,
-)
-
 ComponentPropertyTypeDef = TypedDict(
     "ComponentPropertyTypeDef",
     {
         "value": str,
         "bindingProperties": ComponentPropertyBindingPropertiesTypeDef,
         "collectionBindingProperties": ComponentPropertyBindingPropertiesTypeDef,
         "defaultValue": str,
@@ -1566,66 +1317,29 @@
 )
 
 class UpdateThemeRequestRequestTypeDef(
     _RequiredUpdateThemeRequestRequestTypeDef, _OptionalUpdateThemeRequestRequestTypeDef
 ):
     pass
 
-ComponentEventOutputTypeDef = TypedDict(
-    "ComponentEventOutputTypeDef",
-    {
-        "action": str,
-        "parameters": ActionParametersOutputTypeDef,
-        "bindingEvent": str,
-    },
-    total=False,
-)
-
 ComponentEventTypeDef = TypedDict(
     "ComponentEventTypeDef",
     {
         "action": str,
         "parameters": ActionParametersTypeDef,
         "bindingEvent": str,
     },
     total=False,
 )
 
-_RequiredCodegenGenericDataModelOutputTypeDef = TypedDict(
-    "_RequiredCodegenGenericDataModelOutputTypeDef",
-    {
-        "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
-        "primaryKeys": List[str],
-    },
-)
-_OptionalCodegenGenericDataModelOutputTypeDef = TypedDict(
-    "_OptionalCodegenGenericDataModelOutputTypeDef",
-    {
-        "isJoinTable": bool,
-    },
-    total=False,
-)
-
-class CodegenGenericDataModelOutputTypeDef(
-    _RequiredCodegenGenericDataModelOutputTypeDef, _OptionalCodegenGenericDataModelOutputTypeDef
-):
-    pass
-
-CodegenGenericDataNonModelOutputTypeDef = TypedDict(
-    "CodegenGenericDataNonModelOutputTypeDef",
-    {
-        "fields": Dict[str, CodegenGenericDataFieldOutputTypeDef],
-    },
-)
-
 _RequiredCodegenGenericDataModelTypeDef = TypedDict(
     "_RequiredCodegenGenericDataModelTypeDef",
     {
-        "fields": Mapping[str, CodegenGenericDataFieldTypeDef],
-        "primaryKeys": Sequence[str],
+        "fields": Dict[str, CodegenGenericDataFieldTypeDef],
+        "primaryKeys": List[str],
     },
 )
 _OptionalCodegenGenericDataModelTypeDef = TypedDict(
     "_OptionalCodegenGenericDataModelTypeDef",
     {
         "isJoinTable": bool,
     },
@@ -1636,15 +1350,15 @@
     _RequiredCodegenGenericDataModelTypeDef, _OptionalCodegenGenericDataModelTypeDef
 ):
     pass
 
 CodegenGenericDataNonModelTypeDef = TypedDict(
     "CodegenGenericDataNonModelTypeDef",
     {
-        "fields": Mapping[str, CodegenGenericDataFieldTypeDef],
+        "fields": Dict[str, CodegenGenericDataFieldTypeDef],
     },
 )
 
 ListFormsResponseTypeDef = TypedDict(
     "ListFormsResponseTypeDef",
     {
         "entities": List[FormSummaryTypeDef],
@@ -1660,33 +1374,14 @@
         "clear": FormButtonTypeDef,
         "cancel": FormButtonTypeDef,
         "submit": FormButtonTypeDef,
     },
     total=False,
 )
 
-_RequiredValueMappingsOutputTypeDef = TypedDict(
-    "_RequiredValueMappingsOutputTypeDef",
-    {
-        "values": List[ValueMappingTypeDef],
-    },
-)
-_OptionalValueMappingsOutputTypeDef = TypedDict(
-    "_OptionalValueMappingsOutputTypeDef",
-    {
-        "bindingProperties": Dict[str, FormInputBindingPropertiesValueTypeDef],
-    },
-    total=False,
-)
-
-class ValueMappingsOutputTypeDef(
-    _RequiredValueMappingsOutputTypeDef, _OptionalValueMappingsOutputTypeDef
-):
-    pass
-
 _RequiredValueMappingsTypeDef = TypedDict(
     "_RequiredValueMappingsTypeDef",
     {
         "values": Sequence[ValueMappingTypeDef],
     },
 )
 _OptionalValueMappingsTypeDef = TypedDict(
@@ -1696,90 +1391,67 @@
     },
     total=False,
 )
 
 class ValueMappingsTypeDef(_RequiredValueMappingsTypeDef, _OptionalValueMappingsTypeDef):
     pass
 
-_RequiredComponentChildOutputTypeDef = TypedDict(
-    "_RequiredComponentChildOutputTypeDef",
+_RequiredComponentChildTypeDef = TypedDict(
+    "_RequiredComponentChildTypeDef",
     {
         "componentType": str,
         "name": str,
-        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
+        "properties": Mapping[str, "ComponentPropertyTypeDef"],
     },
 )
-_OptionalComponentChildOutputTypeDef = TypedDict(
-    "_OptionalComponentChildOutputTypeDef",
+_OptionalComponentChildTypeDef = TypedDict(
+    "_OptionalComponentChildTypeDef",
     {
-        "children": List[Dict[str, Any]],
-        "events": Dict[str, ComponentEventOutputTypeDef],
+        "children": Sequence[Dict[str, Any]],
+        "events": Mapping[str, ComponentEventTypeDef],
         "sourceId": str,
     },
     total=False,
 )
 
-class ComponentChildOutputTypeDef(
-    _RequiredComponentChildOutputTypeDef, _OptionalComponentChildOutputTypeDef
-):
+class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
     pass
 
 _RequiredComponentTypeDef = TypedDict(
     "_RequiredComponentTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "name": str,
         "componentType": str,
-        "properties": Dict[str, "ComponentPropertyOutputTypeDef"],
-        "variants": List[ComponentVariantOutputTypeDef],
+        "properties": Dict[str, "ComponentPropertyTypeDef"],
+        "variants": List[ComponentVariantTypeDef],
         "overrides": Dict[str, Dict[str, str]],
-        "bindingProperties": Dict[str, ComponentBindingPropertiesValueOutputTypeDef],
+        "bindingProperties": Dict[str, ComponentBindingPropertiesValueTypeDef],
         "createdAt": datetime,
     },
 )
 _OptionalComponentTypeDef = TypedDict(
     "_OptionalComponentTypeDef",
     {
         "sourceId": str,
-        "children": List["ComponentChildOutputTypeDef"],
-        "collectionProperties": Dict[str, ComponentDataConfigurationOutputTypeDef],
+        "children": List["ComponentChildTypeDef"],
+        "collectionProperties": Dict[str, ComponentDataConfigurationTypeDef],
         "modifiedAt": datetime,
         "tags": Dict[str, str],
-        "events": Dict[str, ComponentEventOutputTypeDef],
+        "events": Dict[str, ComponentEventTypeDef],
         "schemaVersion": str,
     },
     total=False,
 )
 
 class ComponentTypeDef(_RequiredComponentTypeDef, _OptionalComponentTypeDef):
     pass
 
-_RequiredComponentChildTypeDef = TypedDict(
-    "_RequiredComponentChildTypeDef",
-    {
-        "componentType": str,
-        "name": str,
-        "properties": Mapping[str, "ComponentPropertyTypeDef"],
-    },
-)
-_OptionalComponentChildTypeDef = TypedDict(
-    "_OptionalComponentChildTypeDef",
-    {
-        "children": Sequence[Dict[str, Any]],
-        "events": Mapping[str, ComponentEventTypeDef],
-        "sourceId": str,
-    },
-    total=False,
-)
-
-class ComponentChildTypeDef(_RequiredComponentChildTypeDef, _OptionalComponentChildTypeDef):
-    pass
-
 _RequiredCreateComponentDataTypeDef = TypedDict(
     "_RequiredCreateComponentDataTypeDef",
     {
         "name": str,
         "componentType": str,
         "properties": Mapping[str, "ComponentPropertyTypeDef"],
         "variants": Sequence[ComponentVariantTypeDef],
@@ -1820,67 +1492,24 @@
         "collectionProperties": Mapping[str, ComponentDataConfigurationTypeDef],
         "events": Mapping[str, ComponentEventTypeDef],
         "schemaVersion": str,
     },
     total=False,
 )
 
-CodegenJobGenericDataSchemaOutputTypeDef = TypedDict(
-    "CodegenJobGenericDataSchemaOutputTypeDef",
-    {
-        "dataSourceType": Literal["DataStore"],
-        "models": Dict[str, CodegenGenericDataModelOutputTypeDef],
-        "enums": Dict[str, CodegenGenericDataEnumOutputTypeDef],
-        "nonModels": Dict[str, CodegenGenericDataNonModelOutputTypeDef],
-    },
-)
-
 CodegenJobGenericDataSchemaTypeDef = TypedDict(
     "CodegenJobGenericDataSchemaTypeDef",
     {
         "dataSourceType": Literal["DataStore"],
-        "models": Mapping[str, CodegenGenericDataModelTypeDef],
-        "enums": Mapping[str, CodegenGenericDataEnumTypeDef],
-        "nonModels": Mapping[str, CodegenGenericDataNonModelTypeDef],
+        "models": Dict[str, CodegenGenericDataModelTypeDef],
+        "enums": Dict[str, CodegenGenericDataEnumTypeDef],
+        "nonModels": Dict[str, CodegenGenericDataNonModelTypeDef],
     },
 )
 
-_RequiredFieldInputConfigOutputTypeDef = TypedDict(
-    "_RequiredFieldInputConfigOutputTypeDef",
-    {
-        "type": str,
-    },
-)
-_OptionalFieldInputConfigOutputTypeDef = TypedDict(
-    "_OptionalFieldInputConfigOutputTypeDef",
-    {
-        "required": bool,
-        "readOnly": bool,
-        "placeholder": str,
-        "defaultValue": str,
-        "descriptiveText": str,
-        "defaultChecked": bool,
-        "defaultCountryCode": str,
-        "valueMappings": ValueMappingsOutputTypeDef,
-        "name": str,
-        "minValue": float,
-        "maxValue": float,
-        "step": float,
-        "value": str,
-        "isArray": bool,
-        "fileUploaderConfig": FileUploaderFieldConfigOutputTypeDef,
-    },
-    total=False,
-)
-
-class FieldInputConfigOutputTypeDef(
-    _RequiredFieldInputConfigOutputTypeDef, _OptionalFieldInputConfigOutputTypeDef
-):
-    pass
-
 _RequiredFieldInputConfigTypeDef = TypedDict(
     "_RequiredFieldInputConfigTypeDef",
     {
         "type": str,
     },
 )
 _OptionalFieldInputConfigTypeDef = TypedDict(
@@ -1992,15 +1621,15 @@
         "environmentName": str,
     },
 )
 _OptionalCodegenJobTypeDef = TypedDict(
     "_OptionalCodegenJobTypeDef",
     {
         "renderConfig": CodegenJobRenderConfigTypeDef,
-        "genericDataSchema": CodegenJobGenericDataSchemaOutputTypeDef,
+        "genericDataSchema": CodegenJobGenericDataSchemaTypeDef,
         "autoGenerateForms": bool,
         "features": CodegenFeatureFlagsTypeDef,
         "status": CodegenJobStatusType,
         "statusMessage": str,
         "asset": CodegenJobAssetTypeDef,
         "tags": Dict[str, str],
         "createdAt": datetime,
@@ -2030,26 +1659,14 @@
 )
 
 class StartCodegenJobDataTypeDef(
     _RequiredStartCodegenJobDataTypeDef, _OptionalStartCodegenJobDataTypeDef
 ):
     pass
 
-FieldConfigOutputTypeDef = TypedDict(
-    "FieldConfigOutputTypeDef",
-    {
-        "label": str,
-        "position": FieldPositionTypeDef,
-        "excluded": bool,
-        "inputType": FieldInputConfigOutputTypeDef,
-        "validations": List[FieldValidationConfigurationOutputTypeDef],
-    },
-    total=False,
-)
-
 FieldConfigTypeDef = TypedDict(
     "FieldConfigTypeDef",
     {
         "label": str,
         "position": FieldPositionTypeDef,
         "excluded": bool,
         "inputType": FieldInputConfigTypeDef,
@@ -2091,65 +1708,65 @@
 )
 
 class StartCodegenJobRequestRequestTypeDef(
     _RequiredStartCodegenJobRequestRequestTypeDef, _OptionalStartCodegenJobRequestRequestTypeDef
 ):
     pass
 
-_RequiredFormTypeDef = TypedDict(
-    "_RequiredFormTypeDef",
+_RequiredCreateFormDataTypeDef = TypedDict(
+    "_RequiredCreateFormDataTypeDef",
     {
-        "appId": str,
-        "environmentName": str,
-        "id": str,
         "name": str,
+        "dataType": FormDataTypeConfigTypeDef,
         "formActionType": FormActionTypeType,
+        "fields": Mapping[str, FieldConfigTypeDef],
         "style": FormStyleTypeDef,
-        "dataType": FormDataTypeConfigTypeDef,
-        "fields": Dict[str, FieldConfigOutputTypeDef],
-        "sectionalElements": Dict[str, SectionalElementTypeDef],
+        "sectionalElements": Mapping[str, SectionalElementTypeDef],
         "schemaVersion": str,
     },
 )
-_OptionalFormTypeDef = TypedDict(
-    "_OptionalFormTypeDef",
+_OptionalCreateFormDataTypeDef = TypedDict(
+    "_OptionalCreateFormDataTypeDef",
     {
-        "tags": Dict[str, str],
         "cta": FormCTATypeDef,
+        "tags": Mapping[str, str],
         "labelDecorator": LabelDecoratorType,
     },
     total=False,
 )
 
-class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
+class CreateFormDataTypeDef(_RequiredCreateFormDataTypeDef, _OptionalCreateFormDataTypeDef):
     pass
 
-_RequiredCreateFormDataTypeDef = TypedDict(
-    "_RequiredCreateFormDataTypeDef",
+_RequiredFormTypeDef = TypedDict(
+    "_RequiredFormTypeDef",
     {
+        "appId": str,
+        "environmentName": str,
+        "id": str,
         "name": str,
-        "dataType": FormDataTypeConfigTypeDef,
         "formActionType": FormActionTypeType,
-        "fields": Mapping[str, FieldConfigTypeDef],
         "style": FormStyleTypeDef,
-        "sectionalElements": Mapping[str, SectionalElementTypeDef],
+        "dataType": FormDataTypeConfigTypeDef,
+        "fields": Dict[str, FieldConfigTypeDef],
+        "sectionalElements": Dict[str, SectionalElementTypeDef],
         "schemaVersion": str,
     },
 )
-_OptionalCreateFormDataTypeDef = TypedDict(
-    "_OptionalCreateFormDataTypeDef",
+_OptionalFormTypeDef = TypedDict(
+    "_OptionalFormTypeDef",
     {
+        "tags": Dict[str, str],
         "cta": FormCTATypeDef,
-        "tags": Mapping[str, str],
         "labelDecorator": LabelDecoratorType,
     },
     total=False,
 )
 
-class CreateFormDataTypeDef(_RequiredCreateFormDataTypeDef, _OptionalCreateFormDataTypeDef):
+class FormTypeDef(_RequiredFormTypeDef, _OptionalFormTypeDef):
     pass
 
 UpdateFormDataTypeDef = TypedDict(
     "UpdateFormDataTypeDef",
     {
         "name": str,
         "dataType": FormDataTypeConfigTypeDef,
@@ -2160,14 +1777,35 @@
         "schemaVersion": str,
         "cta": FormCTATypeDef,
         "labelDecorator": LabelDecoratorType,
     },
     total=False,
 )
 
+_RequiredCreateFormRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFormRequestRequestTypeDef",
+    {
+        "appId": str,
+        "environmentName": str,
+        "formToCreate": CreateFormDataTypeDef,
+    },
+)
+_OptionalCreateFormRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFormRequestRequestTypeDef",
+    {
+        "clientToken": str,
+    },
+    total=False,
+)
+
+class CreateFormRequestRequestTypeDef(
+    _RequiredCreateFormRequestRequestTypeDef, _OptionalCreateFormRequestRequestTypeDef
+):
+    pass
+
 CreateFormResponseTypeDef = TypedDict(
     "CreateFormResponseTypeDef",
     {
         "entity": FormTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2193,35 +1831,14 @@
     "UpdateFormResponseTypeDef",
     {
         "entity": FormTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateFormRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFormRequestRequestTypeDef",
-    {
-        "appId": str,
-        "environmentName": str,
-        "formToCreate": CreateFormDataTypeDef,
-    },
-)
-_OptionalCreateFormRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFormRequestRequestTypeDef",
-    {
-        "clientToken": str,
-    },
-    total=False,
-)
-
-class CreateFormRequestRequestTypeDef(
-    _RequiredCreateFormRequestRequestTypeDef, _OptionalCreateFormRequestRequestTypeDef
-):
-    pass
-
 _RequiredUpdateFormRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFormRequestRequestTypeDef",
     {
         "appId": str,
         "environmentName": str,
         "id": str,
         "updatedForm": UpdateFormDataTypeDef,
```

### Comparing `types-aiobotocore-amplifyuibuilder-2.5.2.post1/types_aiobotocore_amplifyuibuilder.egg-info/SOURCES.txt` & `types-aiobotocore-amplifyuibuilder-2.5.2.post2/types_aiobotocore_amplifyuibuilder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

