# Comparing `tmp/types-aiobotocore-sts-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sts-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sts-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:05 2023, max compression
+gzip compressed data, was "types-aiobotocore-sts-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:28 2023, max compression
```

## Comparing `types-aiobotocore-sts-2.5.2.post1.tar` & `types-aiobotocore-sts-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.789443 types-aiobotocore-sts-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-08-02 14:53:05.781443 types-aiobotocore-sts-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11034 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:05.789443 types-aiobotocore-sts-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.777443 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7799 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:24.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:05.781443 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-08-02 14:53:05.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-02 14:53:05.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:05.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:05.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:05.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:05.000000 types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.346643 types-aiobotocore-sts-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:46.000000 types-aiobotocore-sts-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11978 2023-08-04 13:59:28.346643 types-aiobotocore-sts-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10476 2023-08-04 13:54:46.000000 types-aiobotocore-sts-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:28.346643 types-aiobotocore-sts-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:54:46.000000 types-aiobotocore-sts-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.346643 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      410 2023-08-04 13:54:46.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      409 2023-08-04 13:54:46.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:54:46.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10185 2023-08-04 13:54:46.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10169 2023-08-04 13:54:46.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8135 2023-08-04 13:54:46.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8133 2023-08-04 13:54:46.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:46.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8060 2023-08-04 13:54:47.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8051 2023-08-04 13:54:47.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:46.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:28.346643 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11978 2023-08-04 13:59:28.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      666 2023-08-04 13:59:28.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:28.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:28.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:28.000000 types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sts-2.5.2.post1/LICENSE` & `types-aiobotocore-sts-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sts-2.5.2.post1/PKG-INFO` & `types-aiobotocore-sts-2.5.2.post2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sts
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.STS 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.STS 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/
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
 [types-aiobotocore-sts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,58 +264,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sts.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `STS` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/literals/).
+
 ```python
-from types_aiobotocore_sts.literals import (
-    STSServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_sts.literals import STSServiceName
 
 
 def check_value(value: STSServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sts.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `STS` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/type_defs/).
+
 ```python
-from types_aiobotocore_sts.type_defs import (
-    PolicyDescriptorTypeTypeDef,
-    TagTypeDef,
-    AssumedRoleUserTypeDef,
-    CredentialsTypeDef,
-    ResponseMetadataTypeDef,
-    DecodeAuthorizationMessageRequestRequestTypeDef,
-    FederatedUserTypeDef,
-    GetAccessKeyInfoRequestRequestTypeDef,
-    GetSessionTokenRequestRequestTypeDef,
-    AssumeRoleWithSAMLRequestRequestTypeDef,
-    AssumeRoleWithWebIdentityRequestRequestTypeDef,
-    AssumeRoleRequestRequestTypeDef,
-    GetFederationTokenRequestRequestTypeDef,
-    AssumeRoleResponseTypeDef,
-    AssumeRoleWithSAMLResponseTypeDef,
-    AssumeRoleWithWebIdentityResponseTypeDef,
-    DecodeAuthorizationMessageResponseTypeDef,
-    GetAccessKeyInfoResponseTypeDef,
-    GetCallerIdentityResponseTypeDef,
-    GetSessionTokenResponseTypeDef,
-    GetFederationTokenResponseTypeDef,
-)
+from types_aiobotocore_sts.type_defs import PolicyDescriptorTypeTypeDef
 
 
 def get_value() -> PolicyDescriptorTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sts-2.5.2.post1/README.md` & `types-aiobotocore-sts-2.5.2.post2/README.md`

 * *Files 6% similar despite different names*

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
 [types-aiobotocore-sts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -232,58 +232,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sts.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `STS` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/literals/).
+
 ```python
-from types_aiobotocore_sts.literals import (
-    STSServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_sts.literals import STSServiceName
 
 
 def check_value(value: STSServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sts.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `STS` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/type_defs/).
+
 ```python
-from types_aiobotocore_sts.type_defs import (
-    PolicyDescriptorTypeTypeDef,
-    TagTypeDef,
-    AssumedRoleUserTypeDef,
-    CredentialsTypeDef,
-    ResponseMetadataTypeDef,
-    DecodeAuthorizationMessageRequestRequestTypeDef,
-    FederatedUserTypeDef,
-    GetAccessKeyInfoRequestRequestTypeDef,
-    GetSessionTokenRequestRequestTypeDef,
-    AssumeRoleWithSAMLRequestRequestTypeDef,
-    AssumeRoleWithWebIdentityRequestRequestTypeDef,
-    AssumeRoleRequestRequestTypeDef,
-    GetFederationTokenRequestRequestTypeDef,
-    AssumeRoleResponseTypeDef,
-    AssumeRoleWithSAMLResponseTypeDef,
-    AssumeRoleWithWebIdentityResponseTypeDef,
-    DecodeAuthorizationMessageResponseTypeDef,
-    GetAccessKeyInfoResponseTypeDef,
-    GetCallerIdentityResponseTypeDef,
-    GetSessionTokenResponseTypeDef,
-    GetFederationTokenResponseTypeDef,
-)
+from types_aiobotocore_sts.type_defs import PolicyDescriptorTypeTypeDef
 
 
 def get_value() -> PolicyDescriptorTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sts-2.5.2.post1/setup.py` & `types-aiobotocore-sts-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sts",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sts"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.STS 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/__main__.py` & `types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.STS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.STS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS\nOther"
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

### Comparing `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/client.py` & `types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     AssumeRoleWithWebIdentityResponseTypeDef,
     DecodeAuthorizationMessageResponseTypeDef,
     GetAccessKeyInfoResponseTypeDef,
     GetCallerIdentityResponseTypeDef,
     GetFederationTokenResponseTypeDef,
     GetSessionTokenResponseTypeDef,
     PolicyDescriptorTypeTypeDef,
+    ProvidedContextTypeDef,
     TagTypeDef,
 )
 
 __all__ = ("STSClient",)
 
 
 class BotocoreClientError(BaseException):
@@ -81,15 +82,16 @@
         Policy: str = ...,
         DurationSeconds: int = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TransitiveTagKeys: Sequence[str] = ...,
         ExternalId: str = ...,
         SerialNumber: str = ...,
         TokenCode: str = ...,
-        SourceIdentity: str = ...
+        SourceIdentity: str = ...,
+        ProvidedContexts: Sequence[ProvidedContextTypeDef] = ...
     ) -> AssumeRoleResponseTypeDef:
         """
         Returns a set of temporary security credentials that you can use to access
         Amazon Web Services resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.assume_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/client/#assume_role)
```

### Comparing `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/client.pyi` & `types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     AssumeRoleWithWebIdentityResponseTypeDef,
     DecodeAuthorizationMessageResponseTypeDef,
     GetAccessKeyInfoResponseTypeDef,
     GetCallerIdentityResponseTypeDef,
     GetFederationTokenResponseTypeDef,
     GetSessionTokenResponseTypeDef,
     PolicyDescriptorTypeTypeDef,
+    ProvidedContextTypeDef,
     TagTypeDef,
 )
 
 __all__ = ("STSClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -77,15 +78,16 @@
         Policy: str = ...,
         DurationSeconds: int = ...,
         Tags: Sequence[TagTypeDef] = ...,
         TransitiveTagKeys: Sequence[str] = ...,
         ExternalId: str = ...,
         SerialNumber: str = ...,
         TokenCode: str = ...,
-        SourceIdentity: str = ...
+        SourceIdentity: str = ...,
+        ProvidedContexts: Sequence[ProvidedContextTypeDef] = ...
     ) -> AssumeRoleResponseTypeDef:
         """
         Returns a set of temporary security credentials that you can use to access
         Amazon Web Services resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sts.html#STS.Client.assume_role)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/client/#assume_role)
```

### Comparing `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/literals.py` & `types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/literals.py`

 * *Files 1% similar despite different names*

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
@@ -403,14 +407,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/literals.pyi` & `types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/literals.pyi`

 * *Files 2% similar despite different names*

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
@@ -401,14 +405,15 @@
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
+    "il-central-1",
     "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
```

### Comparing `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/type_defs.py` & `types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 from typing import Dict, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "PolicyDescriptorTypeTypeDef",
+    "ProvidedContextTypeDef",
     "TagTypeDef",
     "AssumedRoleUserTypeDef",
     "CredentialsTypeDef",
     "ResponseMetadataTypeDef",
     "DecodeAuthorizationMessageRequestRequestTypeDef",
     "FederatedUserTypeDef",
     "GetAccessKeyInfoRequestRequestTypeDef",
@@ -49,14 +49,23 @@
     "PolicyDescriptorTypeTypeDef",
     {
         "arn": str,
     },
     total=False,
 )
 
+ProvidedContextTypeDef = TypedDict(
+    "ProvidedContextTypeDef",
+    {
+        "ProviderArn": str,
+        "ContextAssertion": str,
+    },
+    total=False,
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -136,22 +145,20 @@
         "PolicyArns": Sequence[PolicyDescriptorTypeTypeDef],
         "Policy": str,
         "DurationSeconds": int,
     },
     total=False,
 )
 
-
 class AssumeRoleWithSAMLRequestRequestTypeDef(
     _RequiredAssumeRoleWithSAMLRequestRequestTypeDef,
     _OptionalAssumeRoleWithSAMLRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredAssumeRoleWithWebIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredAssumeRoleWithWebIdentityRequestRequestTypeDef",
     {
         "RoleArn": str,
         "RoleSessionName": str,
         "WebIdentityToken": str,
     },
@@ -163,22 +170,20 @@
         "PolicyArns": Sequence[PolicyDescriptorTypeTypeDef],
         "Policy": str,
         "DurationSeconds": int,
     },
     total=False,
 )
 
-
 class AssumeRoleWithWebIdentityRequestRequestTypeDef(
     _RequiredAssumeRoleWithWebIdentityRequestRequestTypeDef,
     _OptionalAssumeRoleWithWebIdentityRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredAssumeRoleRequestRequestTypeDef = TypedDict(
     "_RequiredAssumeRoleRequestRequestTypeDef",
     {
         "RoleArn": str,
         "RoleSessionName": str,
     },
 )
@@ -190,25 +195,24 @@
         "DurationSeconds": int,
         "Tags": Sequence[TagTypeDef],
         "TransitiveTagKeys": Sequence[str],
         "ExternalId": str,
         "SerialNumber": str,
         "TokenCode": str,
         "SourceIdentity": str,
+        "ProvidedContexts": Sequence[ProvidedContextTypeDef],
     },
     total=False,
 )
 
-
 class AssumeRoleRequestRequestTypeDef(
     _RequiredAssumeRoleRequestRequestTypeDef, _OptionalAssumeRoleRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetFederationTokenRequestRequestTypeDef = TypedDict(
     "_RequiredGetFederationTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetFederationTokenRequestRequestTypeDef = TypedDict(
@@ -218,22 +222,20 @@
         "PolicyArns": Sequence[PolicyDescriptorTypeTypeDef],
         "DurationSeconds": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class GetFederationTokenRequestRequestTypeDef(
     _RequiredGetFederationTokenRequestRequestTypeDef,
     _OptionalGetFederationTokenRequestRequestTypeDef,
 ):
     pass
 
-
 AssumeRoleResponseTypeDef = TypedDict(
     "AssumeRoleResponseTypeDef",
     {
         "Credentials": CredentialsTypeDef,
         "AssumedRoleUser": AssumedRoleUserTypeDef,
         "PackedPolicySize": int,
         "SourceIdentity": str,
```

### Comparing `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts/type_defs.pyi` & `types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,18 @@
 from typing import Dict, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "PolicyDescriptorTypeTypeDef",
+    "ProvidedContextTypeDef",
     "TagTypeDef",
     "AssumedRoleUserTypeDef",
     "CredentialsTypeDef",
     "ResponseMetadataTypeDef",
     "DecodeAuthorizationMessageRequestRequestTypeDef",
     "FederatedUserTypeDef",
     "GetAccessKeyInfoRequestRequestTypeDef",
@@ -48,14 +50,23 @@
     "PolicyDescriptorTypeTypeDef",
     {
         "arn": str,
     },
     total=False,
 )
 
+ProvidedContextTypeDef = TypedDict(
+    "ProvidedContextTypeDef",
+    {
+        "ProviderArn": str,
+        "ContextAssertion": str,
+    },
+    total=False,
+)
+
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -135,20 +146,22 @@
         "PolicyArns": Sequence[PolicyDescriptorTypeTypeDef],
         "Policy": str,
         "DurationSeconds": int,
     },
     total=False,
 )
 
+
 class AssumeRoleWithSAMLRequestRequestTypeDef(
     _RequiredAssumeRoleWithSAMLRequestRequestTypeDef,
     _OptionalAssumeRoleWithSAMLRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredAssumeRoleWithWebIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredAssumeRoleWithWebIdentityRequestRequestTypeDef",
     {
         "RoleArn": str,
         "RoleSessionName": str,
         "WebIdentityToken": str,
     },
@@ -160,20 +173,22 @@
         "PolicyArns": Sequence[PolicyDescriptorTypeTypeDef],
         "Policy": str,
         "DurationSeconds": int,
     },
     total=False,
 )
 
+
 class AssumeRoleWithWebIdentityRequestRequestTypeDef(
     _RequiredAssumeRoleWithWebIdentityRequestRequestTypeDef,
     _OptionalAssumeRoleWithWebIdentityRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredAssumeRoleRequestRequestTypeDef = TypedDict(
     "_RequiredAssumeRoleRequestRequestTypeDef",
     {
         "RoleArn": str,
         "RoleSessionName": str,
     },
 )
@@ -185,23 +200,26 @@
         "DurationSeconds": int,
         "Tags": Sequence[TagTypeDef],
         "TransitiveTagKeys": Sequence[str],
         "ExternalId": str,
         "SerialNumber": str,
         "TokenCode": str,
         "SourceIdentity": str,
+        "ProvidedContexts": Sequence[ProvidedContextTypeDef],
     },
     total=False,
 )
 
+
 class AssumeRoleRequestRequestTypeDef(
     _RequiredAssumeRoleRequestRequestTypeDef, _OptionalAssumeRoleRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetFederationTokenRequestRequestTypeDef = TypedDict(
     "_RequiredGetFederationTokenRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalGetFederationTokenRequestRequestTypeDef = TypedDict(
@@ -211,20 +229,22 @@
         "PolicyArns": Sequence[PolicyDescriptorTypeTypeDef],
         "DurationSeconds": int,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class GetFederationTokenRequestRequestTypeDef(
     _RequiredGetFederationTokenRequestRequestTypeDef,
     _OptionalGetFederationTokenRequestRequestTypeDef,
 ):
     pass
 
+
 AssumeRoleResponseTypeDef = TypedDict(
     "AssumeRoleResponseTypeDef",
     {
         "Credentials": CredentialsTypeDef,
         "AssumedRoleUser": AssumedRoleUserTypeDef,
         "PackedPolicySize": int,
         "SourceIdentity": str,
```

### Comparing `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/PKG-INFO` & `types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sts
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.STS 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.STS 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/
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
 [types-aiobotocore-sts docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/).
 
 See how it helps to find and fix potential bugs:
 
@@ -264,58 +264,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sts.literals` module contains literals extracted from shapes
 that can be used in user code for type checking.
 
+Full list of `STS` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/literals/).
+
 ```python
-from types_aiobotocore_sts.literals import (
-    STSServiceName,
-    ServiceName,
-    ResourceServiceName,
-    RegionName,
-)
+from types_aiobotocore_sts.literals import STSServiceName
 
 
 def check_value(value: STSServiceName) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sts.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `STS` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sts/type_defs/).
+
 ```python
-from types_aiobotocore_sts.type_defs import (
-    PolicyDescriptorTypeTypeDef,
-    TagTypeDef,
-    AssumedRoleUserTypeDef,
-    CredentialsTypeDef,
-    ResponseMetadataTypeDef,
-    DecodeAuthorizationMessageRequestRequestTypeDef,
-    FederatedUserTypeDef,
-    GetAccessKeyInfoRequestRequestTypeDef,
-    GetSessionTokenRequestRequestTypeDef,
-    AssumeRoleWithSAMLRequestRequestTypeDef,
-    AssumeRoleWithWebIdentityRequestRequestTypeDef,
-    AssumeRoleRequestRequestTypeDef,
-    GetFederationTokenRequestRequestTypeDef,
-    AssumeRoleResponseTypeDef,
-    AssumeRoleWithSAMLResponseTypeDef,
-    AssumeRoleWithWebIdentityResponseTypeDef,
-    DecodeAuthorizationMessageResponseTypeDef,
-    GetAccessKeyInfoResponseTypeDef,
-    GetCallerIdentityResponseTypeDef,
-    GetSessionTokenResponseTypeDef,
-    GetFederationTokenResponseTypeDef,
-)
+from types_aiobotocore_sts.type_defs import PolicyDescriptorTypeTypeDef
 
 
 def get_value() -> PolicyDescriptorTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sts-2.5.2.post1/types_aiobotocore_sts.egg-info/SOURCES.txt` & `types-aiobotocore-sts-2.5.2.post2/types_aiobotocore_sts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

