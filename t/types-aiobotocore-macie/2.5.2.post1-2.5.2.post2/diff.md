# Comparing `tmp/types-aiobotocore-macie-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-macie-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-macie-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:36 2023, max compression
+gzip compressed data, was "types-aiobotocore-macie-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
```

## Comparing `types-aiobotocore-macie-2.5.2.post1.tar` & `types-aiobotocore-macie-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.781530 types-aiobotocore-macie-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13879 2023-08-02 14:52:36.773531 types-aiobotocore-macie-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:36.781530 types-aiobotocore-macie-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.773531 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-08-02 14:42:42.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-08-02 14:42:42.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-08-02 14:42:42.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.773531 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13879 2023-08-02 14:52:36.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 14:52:36.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:36.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:36.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:36.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:36.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.546643 types-aiobotocore-macie-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:39.000000 types-aiobotocore-macie-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13023 2023-08-04 13:59:16.546643 types-aiobotocore-macie-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11513 2023-08-04 13:43:39.000000 types-aiobotocore-macie-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.546643 types-aiobotocore-macie-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2058 2023-08-04 13:43:39.000000 types-aiobotocore-macie-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.536643 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      847 2023-08-04 13:43:39.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      846 2023-08-04 13:43:39.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      924 2023-08-04 13:43:39.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9616 2023-08-04 13:43:39.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9598 2023-08-04 13:43:39.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8190 2023-08-04 13:43:40.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8188 2023-08-04 13:43:39.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3091 2023-08-04 13:43:39.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3087 2023-08-04 13:43:39.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:39.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8365 2023-08-04 13:43:40.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8352 2023-08-04 13:43:40.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:39.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.546643 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13023 2023-08-04 13:59:16.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      775 2023-08-04 13:59:16.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:16.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       24 2023-08-04 13:59:16.000000 types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-macie-2.5.2.post1/LICENSE` & `types-aiobotocore-macie-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2.post1/PKG-INFO` & `types-aiobotocore-macie-2.5.2.post2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-macie
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Macie 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Macie 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/
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
 [types-aiobotocore-macie docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,66 +292,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_macie.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Macie` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/literals/).
+
 ```python
-from types_aiobotocore_macie.literals import (
-    ListMemberAccountsPaginatorName,
-    ListS3ResourcesPaginatorName,
-    S3ContinuousClassificationTypeType,
-    S3OneTimeClassificationTypeType,
-    MacieServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_macie.literals import ListMemberAccountsPaginatorName
 
 
 def check_value(value: ListMemberAccountsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_macie.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Macie` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/type_defs/).
+
 ```python
-from types_aiobotocore_macie.type_defs import (
-    AssociateMemberAccountRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ClassificationTypeTypeDef,
-    ClassificationTypeUpdateTypeDef,
-    DisassociateMemberAccountRequestRequestTypeDef,
-    S3ResourceTypeDef,
-    PaginatorConfigTypeDef,
-    ListMemberAccountsRequestRequestTypeDef,
-    MemberAccountTypeDef,
-    ListS3ResourcesRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    S3ResourceClassificationTypeDef,
-    S3ResourceClassificationUpdateTypeDef,
-    DisassociateS3ResourcesRequestRequestTypeDef,
-    FailedS3ResourceTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
-    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
-    ListMemberAccountsResultTypeDef,
-    AssociateS3ResourcesRequestRequestTypeDef,
-    ListS3ResourcesResultTypeDef,
-    UpdateS3ResourcesRequestRequestTypeDef,
-    AssociateS3ResourcesResultTypeDef,
-    DisassociateS3ResourcesResultTypeDef,
-    UpdateS3ResourcesResultTypeDef,
-)
+from types_aiobotocore_macie.type_defs import AssociateMemberAccountRequestRequestTypeDef
 
 
 def get_value() -> AssociateMemberAccountRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-macie-2.5.2.post1/README.md` & `types-aiobotocore-macie-2.5.2.post2/README.md`

 * *Files 25% similar despite different names*

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
 [types-aiobotocore-macie docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/).
 
 See how it helps to find and fix potential bugs:
 
@@ -260,66 +260,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_macie.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Macie` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/literals/).
+
 ```python
-from types_aiobotocore_macie.literals import (
-    ListMemberAccountsPaginatorName,
-    ListS3ResourcesPaginatorName,
-    S3ContinuousClassificationTypeType,
-    S3OneTimeClassificationTypeType,
-    MacieServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_macie.literals import ListMemberAccountsPaginatorName
 
 
 def check_value(value: ListMemberAccountsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_macie.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Macie` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/type_defs/).
+
 ```python
-from types_aiobotocore_macie.type_defs import (
-    AssociateMemberAccountRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ClassificationTypeTypeDef,
-    ClassificationTypeUpdateTypeDef,
-    DisassociateMemberAccountRequestRequestTypeDef,
-    S3ResourceTypeDef,
-    PaginatorConfigTypeDef,
-    ListMemberAccountsRequestRequestTypeDef,
-    MemberAccountTypeDef,
-    ListS3ResourcesRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    S3ResourceClassificationTypeDef,
-    S3ResourceClassificationUpdateTypeDef,
-    DisassociateS3ResourcesRequestRequestTypeDef,
-    FailedS3ResourceTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
-    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
-    ListMemberAccountsResultTypeDef,
-    AssociateS3ResourcesRequestRequestTypeDef,
-    ListS3ResourcesResultTypeDef,
-    UpdateS3ResourcesRequestRequestTypeDef,
-    AssociateS3ResourcesResultTypeDef,
-    DisassociateS3ResourcesResultTypeDef,
-    UpdateS3ResourcesResultTypeDef,
-)
+from types_aiobotocore_macie.type_defs import AssociateMemberAccountRequestRequestTypeDef
 
 
 def get_value() -> AssociateMemberAccountRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-macie-2.5.2.post1/setup.py` & `types-aiobotocore-macie-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-macie",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_macie"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Macie 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/__init__.py` & `types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/__init__.pyi` & `types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/__main__.py` & `types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Macie 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Macie 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie\nOther"
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

### Comparing `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/client.py` & `types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/client.pyi` & `types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/literals.py` & `types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
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
@@ -151,14 +152,15 @@
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
@@ -237,26 +239,28 @@
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

### Comparing `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/literals.pyi` & `types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
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
@@ -149,14 +150,15 @@
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
@@ -235,26 +237,28 @@
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

### Comparing `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/paginator.py` & `types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/paginator.pyi` & `types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/type_defs.py` & `types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/type_defs.pyi` & `types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/PKG-INFO` & `types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-macie
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.Macie 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.Macie 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/
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
 [types-aiobotocore-macie docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/).
 
 See how it helps to find and fix potential bugs:
 
@@ -292,66 +292,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_macie.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `Macie` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/literals/).
+
 ```python
-from types_aiobotocore_macie.literals import (
-    ListMemberAccountsPaginatorName,
-    ListS3ResourcesPaginatorName,
-    S3ContinuousClassificationTypeType,
-    S3OneTimeClassificationTypeType,
-    MacieServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_macie.literals import ListMemberAccountsPaginatorName
 
 
 def check_value(value: ListMemberAccountsPaginatorName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_macie.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `Macie` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/type_defs/).
+
 ```python
-from types_aiobotocore_macie.type_defs import (
-    AssociateMemberAccountRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ClassificationTypeTypeDef,
-    ClassificationTypeUpdateTypeDef,
-    DisassociateMemberAccountRequestRequestTypeDef,
-    S3ResourceTypeDef,
-    PaginatorConfigTypeDef,
-    ListMemberAccountsRequestRequestTypeDef,
-    MemberAccountTypeDef,
-    ListS3ResourcesRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
-    S3ResourceClassificationTypeDef,
-    S3ResourceClassificationUpdateTypeDef,
-    DisassociateS3ResourcesRequestRequestTypeDef,
-    FailedS3ResourceTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
-    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
-    ListMemberAccountsResultTypeDef,
-    AssociateS3ResourcesRequestRequestTypeDef,
-    ListS3ResourcesResultTypeDef,
-    UpdateS3ResourcesRequestRequestTypeDef,
-    AssociateS3ResourcesResultTypeDef,
-    DisassociateS3ResourcesResultTypeDef,
-    UpdateS3ResourcesResultTypeDef,
-)
+from types_aiobotocore_macie.type_defs import AssociateMemberAccountRequestRequestTypeDef
 
 
 def get_value() -> AssociateMemberAccountRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/SOURCES.txt` & `types-aiobotocore-macie-2.5.2.post2/types_aiobotocore_macie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

