# Comparing `tmp/types-aiobotocore-license-manager-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-license-manager-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-license-manager-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-license-manager-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
```

## Comparing `types-aiobotocore-license-manager-2.5.2.post1.tar` & `types-aiobotocore-license-manager-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.893541 types-aiobotocore-license-manager-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-08-02 14:52:33.889541 types-aiobotocore-license-manager-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19197 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.893541 types-aiobotocore-license-manager-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.889541 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    43096 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43032 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12392 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    56419 2023-08-02 14:42:13.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    56347 2023-08-02 14:42:12.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:11.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.889541 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20746 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:33.000000 types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.256643 types-aiobotocore-license-manager-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14347 2023-08-04 13:59:15.256643 types-aiobotocore-license-manager-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12798 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.256643 types-aiobotocore-license-manager-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2127 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.256643 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2010 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2009 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      973 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43066 2023-08-04 13:42:58.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43002 2023-08-04 13:42:58.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12487 2023-08-04 13:42:58.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12485 2023-08-04 13:42:58.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7931 2023-08-04 13:42:58.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7924 2023-08-04 13:42:58.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    55079 2023-08-04 13:42:59.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    55008 2023-08-04 13:42:59.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:57.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.256643 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14347 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       34 2023-08-04 13:59:15.000000 types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/LICENSE` & `types-aiobotocore-license-manager-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/setup.py` & `types-aiobotocore-license-manager-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-license-manager",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_license_manager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LicenseManager 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/__init__.py` & `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/__init__.pyi` & `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/__main__.py` & `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.LicenseManager 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager\nOther"
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

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/client.py` & `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -84,38 +84,35 @@
     ListResourceInventoryResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTokensResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     MetadataTypeDef,
     OptionsTypeDef,
     OrganizationConfigurationTypeDef,
-    ProductInformationUnionTypeDef,
+    ProductInformationTypeDef,
     RejectGrantResponseTypeDef,
-    ReportContextUnionTypeDef,
+    ReportContextTypeDef,
     ReportFrequencyTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("LicenseManagerClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     AuthorizationException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     EntitlementNotAllowedException: Type[BotocoreClientError]
     FailedDependencyException: Type[BotocoreClientError]
@@ -128,15 +125,14 @@
     RedirectException: Type[BotocoreClientError]
     ResourceLimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServerInternalException: Type[BotocoreClientError]
     UnsupportedDigitalSignatureMethodException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class LicenseManagerClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/)
     """
 
     meta: ClientMeta
@@ -145,41 +141,37 @@
     def exceptions(self) -> Exceptions:
         """
         LicenseManagerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#exceptions)
         """
-
     async def accept_grant(self, *, GrantArn: str) -> AcceptGrantResponseTypeDef:
         """
         Accepts the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.accept_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#accept_grant)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#can_paginate)
         """
-
     async def check_in_license(
         self, *, LicenseConsumptionToken: str, Beneficiary: str = ...
     ) -> Dict[str, Any]:
         """
         Checks in the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.check_in_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#check_in_license)
         """
-
     async def checkout_borrow_license(
         self,
         *,
         LicenseArn: str,
         Entitlements: Sequence[EntitlementDataTypeDef],
         DigitalSignatureMethod: Literal["JWT_PS384"],
         ClientToken: str,
@@ -188,15 +180,14 @@
     ) -> CheckoutBorrowLicenseResponseTypeDef:
         """
         Checks out the specified license for offline use.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.checkout_borrow_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#checkout_borrow_license)
         """
-
     async def checkout_license(
         self,
         *,
         ProductSKU: str,
         CheckoutType: CheckoutTypeType,
         KeyFingerprint: str,
         Entitlements: Sequence[EntitlementDataTypeDef],
@@ -206,23 +197,21 @@
     ) -> CheckoutLicenseResponseTypeDef:
         """
         Checks out the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.checkout_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#checkout_license)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#close)
         """
-
     async def create_grant(
         self,
         *,
         ClientToken: str,
         GrantName: str,
         LicenseArn: str,
         Principals: Sequence[str],
@@ -231,15 +220,14 @@
     ) -> CreateGrantResponseTypeDef:
         """
         Creates a grant for the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_grant)
         """
-
     async def create_grant_version(
         self,
         *,
         ClientToken: str,
         GrantArn: str,
         GrantName: str = ...,
         AllowedOperations: Sequence[AllowedOperationType] = ...,
@@ -250,15 +238,14 @@
     ) -> CreateGrantVersionResponseTypeDef:
         """
         Creates a new version of the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_grant_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_grant_version)
         """
-
     async def create_license(
         self,
         *,
         LicenseName: str,
         ProductName: str,
         ProductSKU: str,
         Issuer: IssuerTypeDef,
@@ -272,67 +259,63 @@
     ) -> CreateLicenseResponseTypeDef:
         """
         Creates a license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license)
         """
-
     async def create_license_configuration(
         self,
         *,
         Name: str,
         LicenseCountingType: LicenseCountingTypeType,
         Description: str = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         LicenseRules: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...,
-        ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...
+        ProductInformationList: Sequence[ProductInformationTypeDef] = ...
     ) -> CreateLicenseConfigurationResponseTypeDef:
         """
         Creates a license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_configuration)
         """
-
     async def create_license_conversion_task_for_resource(
         self,
         *,
         ResourceArn: str,
         SourceLicenseContext: LicenseConversionContextTypeDef,
         DestinationLicenseContext: LicenseConversionContextTypeDef
     ) -> CreateLicenseConversionTaskForResourceResponseTypeDef:
         """
         Creates a new license conversion task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_conversion_task_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_conversion_task_for_resource)
         """
-
     async def create_license_manager_report_generator(
         self,
         *,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: ReportContextUnionTypeDef,
+        ReportContext: ReportContextTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateLicenseManagerReportGeneratorResponseTypeDef:
         """
         Creates a report generator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_manager_report_generator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_manager_report_generator)
         """
-
     async def create_license_version(
         self,
         *,
         LicenseArn: str,
         LicenseName: str,
         ProductName: str,
         Issuer: IssuerTypeDef,
@@ -347,15 +330,14 @@
     ) -> CreateLicenseVersionResponseTypeDef:
         """
         Creates a new version of the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_version)
         """
-
     async def create_token(
         self,
         *,
         LicenseArn: str,
         ClientToken: str,
         RoleArns: Sequence[str] = ...,
         ExpirationInDays: int = ...,
@@ -363,358 +345,326 @@
     ) -> CreateTokenResponseTypeDef:
         """
         Creates a long-lived token.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_token)
         """
-
     async def delete_grant(
         self, *, GrantArn: str, Version: str, StatusReason: str = ...
     ) -> DeleteGrantResponseTypeDef:
         """
         Deletes the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.delete_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#delete_grant)
         """
-
     async def delete_license(
         self, *, LicenseArn: str, SourceVersion: str
     ) -> DeleteLicenseResponseTypeDef:
         """
         Deletes the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.delete_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#delete_license)
         """
-
     async def delete_license_configuration(self, *, LicenseConfigurationArn: str) -> Dict[str, Any]:
         """
         Deletes the specified license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.delete_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#delete_license_configuration)
         """
-
     async def delete_license_manager_report_generator(
         self, *, LicenseManagerReportGeneratorArn: str
     ) -> Dict[str, Any]:
         """
         Deletes the specified report generator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.delete_license_manager_report_generator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#delete_license_manager_report_generator)
         """
-
     async def delete_token(self, *, TokenId: str) -> Dict[str, Any]:
         """
         Deletes the specified token.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.delete_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#delete_token)
         """
-
     async def extend_license_consumption(
         self, *, LicenseConsumptionToken: str, DryRun: bool = ...
     ) -> ExtendLicenseConsumptionResponseTypeDef:
         """
         Extends the expiration date for license consumption.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.extend_license_consumption)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#extend_license_consumption)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#generate_presigned_url)
         """
-
     async def get_access_token(
         self, *, Token: str, TokenProperties: Sequence[str] = ...
     ) -> GetAccessTokenResponseTypeDef:
         """
         Gets a temporary access token to use with AssumeRoleWithWebIdentity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_access_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_access_token)
         """
-
     async def get_grant(self, *, GrantArn: str, Version: str = ...) -> GetGrantResponseTypeDef:
         """
         Gets detailed information about the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_grant)
         """
-
     async def get_license(
         self, *, LicenseArn: str, Version: str = ...
     ) -> GetLicenseResponseTypeDef:
         """
         Gets detailed information about the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_license)
         """
-
     async def get_license_configuration(
         self, *, LicenseConfigurationArn: str
     ) -> GetLicenseConfigurationResponseTypeDef:
         """
         Gets detailed information about the specified license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_license_configuration)
         """
-
     async def get_license_conversion_task(
         self, *, LicenseConversionTaskId: str
     ) -> GetLicenseConversionTaskResponseTypeDef:
         """
         Gets information about the specified license type conversion task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_license_conversion_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_license_conversion_task)
         """
-
     async def get_license_manager_report_generator(
         self, *, LicenseManagerReportGeneratorArn: str
     ) -> GetLicenseManagerReportGeneratorResponseTypeDef:
         """
         Gets information about the specified report generator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_license_manager_report_generator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_license_manager_report_generator)
         """
-
     async def get_license_usage(self, *, LicenseArn: str) -> GetLicenseUsageResponseTypeDef:
         """
         Gets detailed information about the usage of the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_license_usage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_license_usage)
         """
-
     async def get_service_settings(self) -> GetServiceSettingsResponseTypeDef:
         """
         Gets the License Manager settings for the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_service_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_service_settings)
         """
-
     async def list_associations_for_license_configuration(
         self, *, LicenseConfigurationArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAssociationsForLicenseConfigurationResponseTypeDef:
         """
         Lists the resource associations for the specified license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_associations_for_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_associations_for_license_configuration)
         """
-
     async def list_distributed_grants(
         self,
         *,
         GrantArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDistributedGrantsResponseTypeDef:
         """
         Lists the grants distributed for the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_distributed_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_distributed_grants)
         """
-
     async def list_failures_for_license_configuration_operations(
         self, *, LicenseConfigurationArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListFailuresForLicenseConfigurationOperationsResponseTypeDef:
         """
         Lists the license configuration operations that failed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_failures_for_license_configuration_operations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_failures_for_license_configuration_operations)
         """
-
     async def list_license_configurations(
         self,
         *,
         LicenseConfigurationArns: Sequence[str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...
     ) -> ListLicenseConfigurationsResponseTypeDef:
         """
         Lists the license configurations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_license_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_license_configurations)
         """
-
     async def list_license_conversion_tasks(
         self, *, NextToken: str = ..., MaxResults: int = ..., Filters: Sequence[FilterTypeDef] = ...
     ) -> ListLicenseConversionTasksResponseTypeDef:
         """
         Lists the license type conversion tasks for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_license_conversion_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_license_conversion_tasks)
         """
-
     async def list_license_manager_report_generators(
         self, *, Filters: Sequence[FilterTypeDef] = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListLicenseManagerReportGeneratorsResponseTypeDef:
         """
         Lists the report generators for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_license_manager_report_generators)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_license_manager_report_generators)
         """
-
     async def list_license_specifications_for_resource(
         self, *, ResourceArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListLicenseSpecificationsForResourceResponseTypeDef:
         """
         Describes the license configurations for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_license_specifications_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_license_specifications_for_resource)
         """
-
     async def list_license_versions(
         self, *, LicenseArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListLicenseVersionsResponseTypeDef:
         """
         Lists all versions of the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_license_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_license_versions)
         """
-
     async def list_licenses(
         self,
         *,
         LicenseArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListLicensesResponseTypeDef:
         """
         Lists the licenses for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_licenses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_licenses)
         """
-
     async def list_received_grants(
         self,
         *,
         GrantArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListReceivedGrantsResponseTypeDef:
         """
         Lists grants that are received.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_grants)
         """
-
     async def list_received_grants_for_organization(
         self,
         *,
         LicenseArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListReceivedGrantsForOrganizationResponseTypeDef:
         """
         Lists the grants received for all accounts in the organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_grants_for_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_grants_for_organization)
         """
-
     async def list_received_licenses(
         self,
         *,
         LicenseArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListReceivedLicensesResponseTypeDef:
         """
         Lists received licenses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_licenses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_licenses)
         """
-
     async def list_received_licenses_for_organization(
         self, *, Filters: Sequence[FilterTypeDef] = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListReceivedLicensesForOrganizationResponseTypeDef:
         """
         Lists the licenses received for all accounts in the organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_licenses_for_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_licenses_for_organization)
         """
-
     async def list_resource_inventory(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[InventoryFilterTypeDef] = ...
     ) -> ListResourceInventoryResponseTypeDef:
         """
         Lists resources managed using Systems Manager inventory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_resource_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_resource_inventory)
         """
-
     async def list_tags_for_resource(
         self, *, ResourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for the specified license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_tags_for_resource)
         """
-
     async def list_tokens(
         self,
         *,
         TokenIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListTokensResponseTypeDef:
         """
         Lists your tokens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_tokens)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_tokens)
         """
-
     async def list_usage_for_license_configuration(
         self,
         *,
         LicenseConfigurationArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...
@@ -722,156 +672,142 @@
         """
         Lists all license usage records for a license configuration, displaying license
         consumption details by resource at a selected point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_usage_for_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_usage_for_license_configuration)
         """
-
     async def reject_grant(self, *, GrantArn: str) -> RejectGrantResponseTypeDef:
         """
         Rejects the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.reject_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#reject_grant)
         """
-
     async def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds the specified tags to the specified license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#tag_resource)
         """
-
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the specified tags from the specified license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#untag_resource)
         """
-
     async def update_license_configuration(
         self,
         *,
         LicenseConfigurationArn: str,
         LicenseConfigurationStatus: LicenseConfigurationStatusType = ...,
         LicenseRules: Sequence[str] = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         Name: str = ...,
         Description: str = ...,
-        ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...,
+        ProductInformationList: Sequence[ProductInformationTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...
     ) -> Dict[str, Any]:
         """
         Modifies the attributes of an existing license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_license_configuration)
         """
-
     async def update_license_manager_report_generator(
         self,
         *,
         LicenseManagerReportGeneratorArn: str,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: ReportContextUnionTypeDef,
+        ReportContext: ReportContextTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a report generator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_manager_report_generator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_license_manager_report_generator)
         """
-
     async def update_license_specifications_for_resource(
         self,
         *,
         ResourceArn: str,
         AddLicenseSpecifications: Sequence[LicenseSpecificationTypeDef] = ...,
         RemoveLicenseSpecifications: Sequence[LicenseSpecificationTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Adds or removes the specified license configurations for the specified Amazon
         Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_specifications_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_license_specifications_for_resource)
         """
-
     async def update_service_settings(
         self,
         *,
         S3BucketArn: str = ...,
         SnsTopicArn: str = ...,
         OrganizationConfiguration: OrganizationConfigurationTypeDef = ...,
         EnableCrossAccountsDiscovery: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates License Manager settings for the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_service_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_service_settings)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_associations_for_license_configuration"]
     ) -> ListAssociationsForLicenseConfigurationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_license_configurations"]
     ) -> ListLicenseConfigurationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_license_specifications_for_resource"]
     ) -> ListLicenseSpecificationsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_inventory"]
     ) -> ListResourceInventoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_usage_for_license_configuration"]
     ) -> ListUsageForLicenseConfigurationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "LicenseManagerClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/)
         """
```

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/client.pyi` & `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,35 +84,38 @@
     ListResourceInventoryResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTokensResponseTypeDef,
     ListUsageForLicenseConfigurationResponseTypeDef,
     MetadataTypeDef,
     OptionsTypeDef,
     OrganizationConfigurationTypeDef,
-    ProductInformationUnionTypeDef,
+    ProductInformationTypeDef,
     RejectGrantResponseTypeDef,
-    ReportContextUnionTypeDef,
+    ReportContextTypeDef,
     ReportFrequencyTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("LicenseManagerClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     AuthorizationException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     EntitlementNotAllowedException: Type[BotocoreClientError]
     FailedDependencyException: Type[BotocoreClientError]
@@ -125,14 +128,15 @@
     RedirectException: Type[BotocoreClientError]
     ResourceLimitExceededException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServerInternalException: Type[BotocoreClientError]
     UnsupportedDigitalSignatureMethodException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class LicenseManagerClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/)
     """
 
     meta: ClientMeta
@@ -141,37 +145,41 @@
     def exceptions(self) -> Exceptions:
         """
         LicenseManagerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#exceptions)
         """
+
     async def accept_grant(self, *, GrantArn: str) -> AcceptGrantResponseTypeDef:
         """
         Accepts the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.accept_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#accept_grant)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#can_paginate)
         """
+
     async def check_in_license(
         self, *, LicenseConsumptionToken: str, Beneficiary: str = ...
     ) -> Dict[str, Any]:
         """
         Checks in the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.check_in_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#check_in_license)
         """
+
     async def checkout_borrow_license(
         self,
         *,
         LicenseArn: str,
         Entitlements: Sequence[EntitlementDataTypeDef],
         DigitalSignatureMethod: Literal["JWT_PS384"],
         ClientToken: str,
@@ -180,14 +188,15 @@
     ) -> CheckoutBorrowLicenseResponseTypeDef:
         """
         Checks out the specified license for offline use.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.checkout_borrow_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#checkout_borrow_license)
         """
+
     async def checkout_license(
         self,
         *,
         ProductSKU: str,
         CheckoutType: CheckoutTypeType,
         KeyFingerprint: str,
         Entitlements: Sequence[EntitlementDataTypeDef],
@@ -197,21 +206,23 @@
     ) -> CheckoutLicenseResponseTypeDef:
         """
         Checks out the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.checkout_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#checkout_license)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#close)
         """
+
     async def create_grant(
         self,
         *,
         ClientToken: str,
         GrantName: str,
         LicenseArn: str,
         Principals: Sequence[str],
@@ -220,14 +231,15 @@
     ) -> CreateGrantResponseTypeDef:
         """
         Creates a grant for the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_grant)
         """
+
     async def create_grant_version(
         self,
         *,
         ClientToken: str,
         GrantArn: str,
         GrantName: str = ...,
         AllowedOperations: Sequence[AllowedOperationType] = ...,
@@ -238,14 +250,15 @@
     ) -> CreateGrantVersionResponseTypeDef:
         """
         Creates a new version of the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_grant_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_grant_version)
         """
+
     async def create_license(
         self,
         *,
         LicenseName: str,
         ProductName: str,
         ProductSKU: str,
         Issuer: IssuerTypeDef,
@@ -259,63 +272,67 @@
     ) -> CreateLicenseResponseTypeDef:
         """
         Creates a license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license)
         """
+
     async def create_license_configuration(
         self,
         *,
         Name: str,
         LicenseCountingType: LicenseCountingTypeType,
         Description: str = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         LicenseRules: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...,
-        ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...
+        ProductInformationList: Sequence[ProductInformationTypeDef] = ...
     ) -> CreateLicenseConfigurationResponseTypeDef:
         """
         Creates a license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_configuration)
         """
+
     async def create_license_conversion_task_for_resource(
         self,
         *,
         ResourceArn: str,
         SourceLicenseContext: LicenseConversionContextTypeDef,
         DestinationLicenseContext: LicenseConversionContextTypeDef
     ) -> CreateLicenseConversionTaskForResourceResponseTypeDef:
         """
         Creates a new license conversion task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_conversion_task_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_conversion_task_for_resource)
         """
+
     async def create_license_manager_report_generator(
         self,
         *,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: ReportContextUnionTypeDef,
+        ReportContext: ReportContextTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateLicenseManagerReportGeneratorResponseTypeDef:
         """
         Creates a report generator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_manager_report_generator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_manager_report_generator)
         """
+
     async def create_license_version(
         self,
         *,
         LicenseArn: str,
         LicenseName: str,
         ProductName: str,
         Issuer: IssuerTypeDef,
@@ -330,14 +347,15 @@
     ) -> CreateLicenseVersionResponseTypeDef:
         """
         Creates a new version of the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_license_version)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_license_version)
         """
+
     async def create_token(
         self,
         *,
         LicenseArn: str,
         ClientToken: str,
         RoleArns: Sequence[str] = ...,
         ExpirationInDays: int = ...,
@@ -345,326 +363,358 @@
     ) -> CreateTokenResponseTypeDef:
         """
         Creates a long-lived token.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.create_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#create_token)
         """
+
     async def delete_grant(
         self, *, GrantArn: str, Version: str, StatusReason: str = ...
     ) -> DeleteGrantResponseTypeDef:
         """
         Deletes the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.delete_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#delete_grant)
         """
+
     async def delete_license(
         self, *, LicenseArn: str, SourceVersion: str
     ) -> DeleteLicenseResponseTypeDef:
         """
         Deletes the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.delete_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#delete_license)
         """
+
     async def delete_license_configuration(self, *, LicenseConfigurationArn: str) -> Dict[str, Any]:
         """
         Deletes the specified license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.delete_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#delete_license_configuration)
         """
+
     async def delete_license_manager_report_generator(
         self, *, LicenseManagerReportGeneratorArn: str
     ) -> Dict[str, Any]:
         """
         Deletes the specified report generator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.delete_license_manager_report_generator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#delete_license_manager_report_generator)
         """
+
     async def delete_token(self, *, TokenId: str) -> Dict[str, Any]:
         """
         Deletes the specified token.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.delete_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#delete_token)
         """
+
     async def extend_license_consumption(
         self, *, LicenseConsumptionToken: str, DryRun: bool = ...
     ) -> ExtendLicenseConsumptionResponseTypeDef:
         """
         Extends the expiration date for license consumption.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.extend_license_consumption)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#extend_license_consumption)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#generate_presigned_url)
         """
+
     async def get_access_token(
         self, *, Token: str, TokenProperties: Sequence[str] = ...
     ) -> GetAccessTokenResponseTypeDef:
         """
         Gets a temporary access token to use with AssumeRoleWithWebIdentity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_access_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_access_token)
         """
+
     async def get_grant(self, *, GrantArn: str, Version: str = ...) -> GetGrantResponseTypeDef:
         """
         Gets detailed information about the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_grant)
         """
+
     async def get_license(
         self, *, LicenseArn: str, Version: str = ...
     ) -> GetLicenseResponseTypeDef:
         """
         Gets detailed information about the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_license)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_license)
         """
+
     async def get_license_configuration(
         self, *, LicenseConfigurationArn: str
     ) -> GetLicenseConfigurationResponseTypeDef:
         """
         Gets detailed information about the specified license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_license_configuration)
         """
+
     async def get_license_conversion_task(
         self, *, LicenseConversionTaskId: str
     ) -> GetLicenseConversionTaskResponseTypeDef:
         """
         Gets information about the specified license type conversion task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_license_conversion_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_license_conversion_task)
         """
+
     async def get_license_manager_report_generator(
         self, *, LicenseManagerReportGeneratorArn: str
     ) -> GetLicenseManagerReportGeneratorResponseTypeDef:
         """
         Gets information about the specified report generator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_license_manager_report_generator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_license_manager_report_generator)
         """
+
     async def get_license_usage(self, *, LicenseArn: str) -> GetLicenseUsageResponseTypeDef:
         """
         Gets detailed information about the usage of the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_license_usage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_license_usage)
         """
+
     async def get_service_settings(self) -> GetServiceSettingsResponseTypeDef:
         """
         Gets the License Manager settings for the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_service_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_service_settings)
         """
+
     async def list_associations_for_license_configuration(
         self, *, LicenseConfigurationArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListAssociationsForLicenseConfigurationResponseTypeDef:
         """
         Lists the resource associations for the specified license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_associations_for_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_associations_for_license_configuration)
         """
+
     async def list_distributed_grants(
         self,
         *,
         GrantArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListDistributedGrantsResponseTypeDef:
         """
         Lists the grants distributed for the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_distributed_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_distributed_grants)
         """
+
     async def list_failures_for_license_configuration_operations(
         self, *, LicenseConfigurationArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListFailuresForLicenseConfigurationOperationsResponseTypeDef:
         """
         Lists the license configuration operations that failed.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_failures_for_license_configuration_operations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_failures_for_license_configuration_operations)
         """
+
     async def list_license_configurations(
         self,
         *,
         LicenseConfigurationArns: Sequence[str] = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...
     ) -> ListLicenseConfigurationsResponseTypeDef:
         """
         Lists the license configurations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_license_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_license_configurations)
         """
+
     async def list_license_conversion_tasks(
         self, *, NextToken: str = ..., MaxResults: int = ..., Filters: Sequence[FilterTypeDef] = ...
     ) -> ListLicenseConversionTasksResponseTypeDef:
         """
         Lists the license type conversion tasks for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_license_conversion_tasks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_license_conversion_tasks)
         """
+
     async def list_license_manager_report_generators(
         self, *, Filters: Sequence[FilterTypeDef] = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListLicenseManagerReportGeneratorsResponseTypeDef:
         """
         Lists the report generators for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_license_manager_report_generators)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_license_manager_report_generators)
         """
+
     async def list_license_specifications_for_resource(
         self, *, ResourceArn: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListLicenseSpecificationsForResourceResponseTypeDef:
         """
         Describes the license configurations for the specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_license_specifications_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_license_specifications_for_resource)
         """
+
     async def list_license_versions(
         self, *, LicenseArn: str, NextToken: str = ..., MaxResults: int = ...
     ) -> ListLicenseVersionsResponseTypeDef:
         """
         Lists all versions of the specified license.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_license_versions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_license_versions)
         """
+
     async def list_licenses(
         self,
         *,
         LicenseArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListLicensesResponseTypeDef:
         """
         Lists the licenses for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_licenses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_licenses)
         """
+
     async def list_received_grants(
         self,
         *,
         GrantArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListReceivedGrantsResponseTypeDef:
         """
         Lists grants that are received.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_grants)
         """
+
     async def list_received_grants_for_organization(
         self,
         *,
         LicenseArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListReceivedGrantsForOrganizationResponseTypeDef:
         """
         Lists the grants received for all accounts in the organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_grants_for_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_grants_for_organization)
         """
+
     async def list_received_licenses(
         self,
         *,
         LicenseArns: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListReceivedLicensesResponseTypeDef:
         """
         Lists received licenses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_licenses)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_licenses)
         """
+
     async def list_received_licenses_for_organization(
         self, *, Filters: Sequence[FilterTypeDef] = ..., NextToken: str = ..., MaxResults: int = ...
     ) -> ListReceivedLicensesForOrganizationResponseTypeDef:
         """
         Lists the licenses received for all accounts in the organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_received_licenses_for_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_received_licenses_for_organization)
         """
+
     async def list_resource_inventory(
         self,
         *,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[InventoryFilterTypeDef] = ...
     ) -> ListResourceInventoryResponseTypeDef:
         """
         Lists resources managed using Systems Manager inventory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_resource_inventory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_resource_inventory)
         """
+
     async def list_tags_for_resource(
         self, *, ResourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Lists the tags for the specified license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_tags_for_resource)
         """
+
     async def list_tokens(
         self,
         *,
         TokenIds: Sequence[str] = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListTokensResponseTypeDef:
         """
         Lists your tokens.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_tokens)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_tokens)
         """
+
     async def list_usage_for_license_configuration(
         self,
         *,
         LicenseConfigurationArn: str,
         MaxResults: int = ...,
         NextToken: str = ...,
         Filters: Sequence[FilterTypeDef] = ...
@@ -672,142 +722,156 @@
         """
         Lists all license usage records for a license configuration, displaying license
         consumption details by resource at a selected point in time.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.list_usage_for_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#list_usage_for_license_configuration)
         """
+
     async def reject_grant(self, *, GrantArn: str) -> RejectGrantResponseTypeDef:
         """
         Rejects the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.reject_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#reject_grant)
         """
+
     async def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds the specified tags to the specified license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#tag_resource)
         """
+
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes the specified tags from the specified license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#untag_resource)
         """
+
     async def update_license_configuration(
         self,
         *,
         LicenseConfigurationArn: str,
         LicenseConfigurationStatus: LicenseConfigurationStatusType = ...,
         LicenseRules: Sequence[str] = ...,
         LicenseCount: int = ...,
         LicenseCountHardLimit: bool = ...,
         Name: str = ...,
         Description: str = ...,
-        ProductInformationList: Sequence[ProductInformationUnionTypeDef] = ...,
+        ProductInformationList: Sequence[ProductInformationTypeDef] = ...,
         DisassociateWhenNotFound: bool = ...
     ) -> Dict[str, Any]:
         """
         Modifies the attributes of an existing license configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_license_configuration)
         """
+
     async def update_license_manager_report_generator(
         self,
         *,
         LicenseManagerReportGeneratorArn: str,
         ReportGeneratorName: str,
         Type: Sequence[ReportTypeType],
-        ReportContext: ReportContextUnionTypeDef,
+        ReportContext: ReportContextTypeDef,
         ReportFrequency: ReportFrequencyTypeDef,
         ClientToken: str,
         Description: str = ...
     ) -> Dict[str, Any]:
         """
         Updates a report generator.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_manager_report_generator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_license_manager_report_generator)
         """
+
     async def update_license_specifications_for_resource(
         self,
         *,
         ResourceArn: str,
         AddLicenseSpecifications: Sequence[LicenseSpecificationTypeDef] = ...,
         RemoveLicenseSpecifications: Sequence[LicenseSpecificationTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Adds or removes the specified license configurations for the specified Amazon
         Web Services resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_license_specifications_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_license_specifications_for_resource)
         """
+
     async def update_service_settings(
         self,
         *,
         S3BucketArn: str = ...,
         SnsTopicArn: str = ...,
         OrganizationConfiguration: OrganizationConfigurationTypeDef = ...,
         EnableCrossAccountsDiscovery: bool = ...
     ) -> Dict[str, Any]:
         """
         Updates License Manager settings for the current Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.update_service_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#update_service_settings)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_associations_for_license_configuration"]
     ) -> ListAssociationsForLicenseConfigurationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_license_configurations"]
     ) -> ListLicenseConfigurationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_license_specifications_for_resource"]
     ) -> ListLicenseSpecificationsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_inventory"]
     ) -> ListResourceInventoryPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_usage_for_license_configuration"]
     ) -> ListUsageForLicenseConfigurationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "LicenseManagerClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/license-manager.html#LicenseManager.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_license_manager/client/)
         """
```

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/literals.py` & `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,14 +187,15 @@
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
@@ -290,14 +291,15 @@
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
@@ -376,26 +378,28 @@
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

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/literals.pyi` & `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,15 @@
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
@@ -288,14 +289,15 @@
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
@@ -374,26 +376,28 @@
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

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/paginator.py` & `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/paginator.pyi` & `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/type_defs.py` & `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_license_manager.type_defs import AcceptGrantRequestRequestTypeDef
 
     data: AcceptGrantRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     ActivationOverrideBehaviorType,
     AllowedOperationType,
     CheckoutTypeType,
     EntitlementDataUnitType,
     EntitlementUnitType,
@@ -40,15 +40,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcceptGrantRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AutomatedDiscoveryInformationTypeDef",
     "BorrowConfigurationTypeDef",
     "CheckInLicenseRequestRequestTypeDef",
     "EntitlementDataTypeDef",
@@ -92,18 +91,16 @@
     "ListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     "ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
     "ListLicenseSpecificationsForResourceRequestRequestTypeDef",
     "ListLicenseVersionsRequestRequestTypeDef",
     "ResourceInventoryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TokenDataTypeDef",
-    "ProductInformationFilterOutputTypeDef",
     "ProductInformationFilterTypeDef",
     "RejectGrantRequestRequestTypeDef",
-    "ReportContextOutputTypeDef",
     "S3LocationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AcceptGrantResponseTypeDef",
     "CreateGrantResponseTypeDef",
     "CreateGrantVersionResponseTypeDef",
     "CreateLicenseConfigurationResponseTypeDef",
     "CreateLicenseConversionTaskForResourceResponseTypeDef",
@@ -153,42 +150,39 @@
     "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
     "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
     "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListResourceInventoryResponseTypeDef",
     "ListTokensResponseTypeDef",
-    "ProductInformationOutputTypeDef",
     "ProductInformationTypeDef",
-    "ReportContextUnionTypeDef",
     "ReportGeneratorTypeDef",
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     "CreateLicenseRequestRequestTypeDef",
     "CreateLicenseVersionRequestRequestTypeDef",
     "GrantedLicenseTypeDef",
     "LicenseTypeDef",
     "GetGrantResponseTypeDef",
     "ListDistributedGrantsResponseTypeDef",
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     "ListReceivedGrantsResponseTypeDef",
     "ListLicenseConversionTasksResponseTypeDef",
     "GetLicenseUsageResponseTypeDef",
+    "CreateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseConfigurationResponseTypeDef",
     "LicenseConfigurationTypeDef",
-    "ProductInformationUnionTypeDef",
+    "UpdateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     "ListReceivedLicensesResponseTypeDef",
     "GetLicenseResponseTypeDef",
     "ListLicenseVersionsResponseTypeDef",
     "ListLicensesResponseTypeDef",
     "ListLicenseConfigurationsResponseTypeDef",
-    "CreateLicenseConfigurationRequestRequestTypeDef",
-    "UpdateLicenseConfigurationRequestRequestTypeDef",
 )
 
 AcceptGrantRequestRequestTypeDef = TypedDict(
     "AcceptGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
@@ -231,21 +225,19 @@
     "_OptionalCheckInLicenseRequestRequestTypeDef",
     {
         "Beneficiary": str,
     },
     total=False,
 )
 
-
 class CheckInLicenseRequestRequestTypeDef(
     _RequiredCheckInLicenseRequestRequestTypeDef, _OptionalCheckInLicenseRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredEntitlementDataTypeDef = TypedDict(
     "_RequiredEntitlementDataTypeDef",
     {
         "Name": str,
         "Unit": EntitlementDataUnitType,
     },
 )
@@ -253,19 +245,17 @@
     "_OptionalEntitlementDataTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class EntitlementDataTypeDef(_RequiredEntitlementDataTypeDef, _OptionalEntitlementDataTypeDef):
     pass
 
-
 MetadataTypeDef = TypedDict(
     "MetadataTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -350,19 +340,17 @@
     "_OptionalDatetimeRangeTypeDef",
     {
         "End": str,
     },
     total=False,
 )
 
-
 class DatetimeRangeTypeDef(_RequiredDatetimeRangeTypeDef, _OptionalDatetimeRangeTypeDef):
     pass
 
-
 _RequiredEntitlementTypeDef = TypedDict(
     "_RequiredEntitlementTypeDef",
     {
         "Name": str,
         "Unit": EntitlementUnitType,
     },
 )
@@ -373,38 +361,34 @@
         "MaxCount": int,
         "Overage": bool,
         "AllowCheckIn": bool,
     },
     total=False,
 )
 
-
 class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
     pass
 
-
 _RequiredIssuerTypeDef = TypedDict(
     "_RequiredIssuerTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalIssuerTypeDef = TypedDict(
     "_OptionalIssuerTypeDef",
     {
         "SignKey": str,
     },
     total=False,
 )
 
-
 class IssuerTypeDef(_RequiredIssuerTypeDef, _OptionalIssuerTypeDef):
     pass
 
-
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "ClientToken": str,
     },
 )
@@ -414,21 +398,19 @@
         "RoleArns": Sequence[str],
         "ExpirationInDays": int,
         "TokenProperties": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteGrantRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
         "Version": str,
     },
 )
@@ -436,21 +418,19 @@
     "_OptionalDeleteGrantRequestRequestTypeDef",
     {
         "StatusReason": str,
     },
     total=False,
 )
 
-
 class DeleteGrantRequestRequestTypeDef(
     _RequiredDeleteGrantRequestRequestTypeDef, _OptionalDeleteGrantRequestRequestTypeDef
 ):
     pass
 
-
 DeleteLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 
@@ -488,41 +468,37 @@
     "_OptionalEntitlementUsageTypeDef",
     {
         "MaxCount": str,
     },
     total=False,
 )
 
-
 class EntitlementUsageTypeDef(_RequiredEntitlementUsageTypeDef, _OptionalEntitlementUsageTypeDef):
     pass
 
-
 _RequiredExtendLicenseConsumptionRequestRequestTypeDef = TypedDict(
     "_RequiredExtendLicenseConsumptionRequestRequestTypeDef",
     {
         "LicenseConsumptionToken": str,
     },
 )
 _OptionalExtendLicenseConsumptionRequestRequestTypeDef = TypedDict(
     "_OptionalExtendLicenseConsumptionRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
-
 class ExtendLicenseConsumptionRequestRequestTypeDef(
     _RequiredExtendLicenseConsumptionRequestRequestTypeDef,
     _OptionalExtendLicenseConsumptionRequestRequestTypeDef,
 ):
     pass
 
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -538,42 +514,38 @@
     "_OptionalGetAccessTokenRequestRequestTypeDef",
     {
         "TokenProperties": Sequence[str],
     },
     total=False,
 )
 
-
 class GetAccessTokenRequestRequestTypeDef(
     _RequiredGetAccessTokenRequestRequestTypeDef, _OptionalGetAccessTokenRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetGrantRequestRequestTypeDef = TypedDict(
     "_RequiredGetGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 _OptionalGetGrantRequestRequestTypeDef = TypedDict(
     "_OptionalGetGrantRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetGrantRequestRequestTypeDef(
     _RequiredGetGrantRequestRequestTypeDef, _OptionalGetGrantRequestRequestTypeDef
 ):
     pass
 
-
 GetLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "GetLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 
@@ -610,21 +582,19 @@
     "_OptionalGetLicenseRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
-
 class GetLicenseRequestRequestTypeDef(
     _RequiredGetLicenseRequestRequestTypeDef, _OptionalGetLicenseRequestRequestTypeDef
 ):
     pass
 
-
 GetLicenseUsageRequestRequestTypeDef = TypedDict(
     "GetLicenseUsageRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 
@@ -666,19 +636,17 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
-
 LicenseConfigurationAssociationTypeDef = TypedDict(
     "LicenseConfigurationAssociationTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": ResourceTypeType,
         "ResourceOwnerId": str,
         "AssociationTime": datetime,
@@ -710,21 +678,19 @@
     "_OptionalLicenseSpecificationTypeDef",
     {
         "AmiAssociationScope": str,
     },
     total=False,
 )
 
-
 class LicenseSpecificationTypeDef(
     _RequiredLicenseSpecificationTypeDef, _OptionalLicenseSpecificationTypeDef
 ):
     pass
 
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -742,22 +708,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAssociationsForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListAssociationsForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef = TypedDict(
@@ -765,22 +729,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef(
     _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
     _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
@@ -788,22 +750,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalListLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListLicenseVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseVersionsRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 _OptionalListLicenseVersionsRequestRequestTypeDef = TypedDict(
@@ -811,22 +771,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListLicenseVersionsRequestRequestTypeDef(
     _RequiredListLicenseVersionsRequestRequestTypeDef,
     _OptionalListLicenseVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ResourceInventoryTypeDef = TypedDict(
     "ResourceInventoryTypeDef",
     {
         "ResourceId": str,
         "ResourceType": ResourceTypeType,
         "ResourceArn": str,
         "Platform": str,
@@ -853,36 +811,14 @@
         "TokenProperties": List[str],
         "RoleArns": List[str],
         "Status": str,
     },
     total=False,
 )
 
-_RequiredProductInformationFilterOutputTypeDef = TypedDict(
-    "_RequiredProductInformationFilterOutputTypeDef",
-    {
-        "ProductInformationFilterName": str,
-        "ProductInformationFilterComparator": str,
-    },
-)
-_OptionalProductInformationFilterOutputTypeDef = TypedDict(
-    "_OptionalProductInformationFilterOutputTypeDef",
-    {
-        "ProductInformationFilterValue": List[str],
-    },
-    total=False,
-)
-
-
-class ProductInformationFilterOutputTypeDef(
-    _RequiredProductInformationFilterOutputTypeDef, _OptionalProductInformationFilterOutputTypeDef
-):
-    pass
-
-
 _RequiredProductInformationFilterTypeDef = TypedDict(
     "_RequiredProductInformationFilterTypeDef",
     {
         "ProductInformationFilterName": str,
         "ProductInformationFilterComparator": str,
     },
 )
@@ -890,35 +826,26 @@
     "_OptionalProductInformationFilterTypeDef",
     {
         "ProductInformationFilterValue": Sequence[str],
     },
     total=False,
 )
 
-
 class ProductInformationFilterTypeDef(
     _RequiredProductInformationFilterTypeDef, _OptionalProductInformationFilterTypeDef
 ):
     pass
 
-
 RejectGrantRequestRequestTypeDef = TypedDict(
     "RejectGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-ReportContextOutputTypeDef = TypedDict(
-    "ReportContextOutputTypeDef",
-    {
-        "licenseConfigurationArns": List[str],
-    },
-)
-
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
     },
     total=False,
@@ -1077,21 +1004,19 @@
     {
         "Beneficiary": str,
         "NodeId": str,
     },
     total=False,
 )
 
-
 class CheckoutLicenseRequestRequestTypeDef(
     _RequiredCheckoutLicenseRequestRequestTypeDef, _OptionalCheckoutLicenseRequestRequestTypeDef
 ):
     pass
 
-
 CheckoutLicenseResponseTypeDef = TypedDict(
     "CheckoutLicenseResponseTypeDef",
     {
         "CheckoutType": CheckoutTypeType,
         "LicenseConsumptionToken": str,
         "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "SignedToken": str,
@@ -1117,22 +1042,20 @@
     {
         "NodeId": str,
         "CheckoutMetadata": Sequence[MetadataTypeDef],
     },
     total=False,
 )
 
-
 class CheckoutBorrowLicenseRequestRequestTypeDef(
     _RequiredCheckoutBorrowLicenseRequestRequestTypeDef,
     _OptionalCheckoutBorrowLicenseRequestRequestTypeDef,
 ):
     pass
 
-
 CheckoutBorrowLicenseResponseTypeDef = TypedDict(
     "CheckoutBorrowLicenseResponseTypeDef",
     {
         "LicenseArn": str,
         "LicenseConsumptionToken": str,
         "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "NodeId": str,
@@ -1185,22 +1108,20 @@
         "StatusReason": str,
         "SourceVersion": str,
         "Options": OptionsTypeDef,
     },
     total=False,
 )
 
-
 class CreateGrantVersionRequestRequestTypeDef(
     _RequiredCreateGrantVersionRequestRequestTypeDef,
     _OptionalCreateGrantVersionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGrantTypeDef = TypedDict(
     "_RequiredGrantTypeDef",
     {
         "GrantArn": str,
         "GrantName": str,
         "ParentArn": str,
         "LicenseArn": str,
@@ -1216,19 +1137,17 @@
     {
         "StatusReason": str,
         "Options": OptionsTypeDef,
     },
     total=False,
 )
 
-
 class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1297,22 +1216,20 @@
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateLicenseManagerReportGeneratorRequestRequestTypeDef(
     _RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     _OptionalCreateLicenseManagerReportGeneratorRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "LicenseManagerReportGeneratorArn": str,
         "ReportGeneratorName": str,
         "Type": Sequence[ReportTypeType],
         "ReportContext": ReportContextTypeDef,
@@ -1324,22 +1241,20 @@
     "_OptionalUpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateLicenseManagerReportGeneratorRequestRequestTypeDef(
     _RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     _OptionalUpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
 ):
     pass
 
-
 LicenseUsageTypeDef = TypedDict(
     "LicenseUsageTypeDef",
     {
         "EntitlementUsages": List[EntitlementUsageTypeDef],
     },
     total=False,
 )
@@ -1409,22 +1324,20 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListReceivedGrantsForOrganizationRequestRequestTypeDef(
     _RequiredListReceivedGrantsForOrganizationRequestRequestTypeDef,
     _OptionalListReceivedGrantsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
-
 ListReceivedGrantsRequestRequestTypeDef = TypedDict(
     "ListReceivedGrantsRequestRequestTypeDef",
     {
         "GrantArns": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
@@ -1476,22 +1389,20 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-
 class ListUsageForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
         "OrganizationConfiguration": OrganizationConfigurationTypeDef,
         "EnableCrossAccountsDiscovery": bool,
@@ -1559,44 +1470,40 @@
     {
         "AddLicenseSpecifications": Sequence[LicenseSpecificationTypeDef],
         "RemoveLicenseSpecifications": Sequence[LicenseSpecificationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
     "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
     "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
     _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
     _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
 ):
     pass
 
-
 ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
     "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
     {
         "LicenseConfigurationArns": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1613,22 +1520,20 @@
     "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
     _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
 ):
     pass
 
-
 ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
     "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1645,22 +1550,20 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
     _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
 ):
     pass
 
-
 ListResourceInventoryResponseTypeDef = TypedDict(
     "ListResourceInventoryResponseTypeDef",
     {
         "ResourceInventoryList": List[ResourceInventoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1671,37 +1574,28 @@
     {
         "Tokens": List[TokenDataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProductInformationOutputTypeDef = TypedDict(
-    "ProductInformationOutputTypeDef",
-    {
-        "ResourceType": str,
-        "ProductInformationFilterList": List[ProductInformationFilterOutputTypeDef],
-    },
-)
-
 ProductInformationTypeDef = TypedDict(
     "ProductInformationTypeDef",
     {
         "ResourceType": str,
         "ProductInformationFilterList": Sequence[ProductInformationFilterTypeDef],
     },
 )
 
-ReportContextUnionTypeDef = Union[ReportContextTypeDef, ReportContextOutputTypeDef]
 ReportGeneratorTypeDef = TypedDict(
     "ReportGeneratorTypeDef",
     {
         "ReportGeneratorName": str,
         "ReportType": List[ReportTypeType],
-        "ReportContext": ReportContextOutputTypeDef,
+        "ReportContext": ReportContextTypeDef,
         "ReportFrequency": ReportFrequencyTypeDef,
         "LicenseManagerReportGeneratorArn": str,
         "LastRunStatus": str,
         "LastRunFailureReason": str,
         "LastReportGenerationTime": str,
         "ReportCreatorAccount": str,
         "Description": str,
@@ -1740,21 +1634,19 @@
     "_OptionalCreateLicenseRequestRequestTypeDef",
     {
         "LicenseMetadata": Sequence[MetadataTypeDef],
     },
     total=False,
 )
 
-
 class CreateLicenseRequestRequestTypeDef(
     _RequiredCreateLicenseRequestRequestTypeDef, _OptionalCreateLicenseRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateLicenseVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseVersionRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "LicenseName": str,
         "ProductName": str,
         "Issuer": IssuerTypeDef,
@@ -1771,22 +1663,20 @@
     {
         "LicenseMetadata": Sequence[MetadataTypeDef],
         "SourceVersion": str,
     },
     total=False,
 )
 
-
 class CreateLicenseVersionRequestRequestTypeDef(
     _RequiredCreateLicenseVersionRequestRequestTypeDef,
     _OptionalCreateLicenseVersionRequestRequestTypeDef,
 ):
     pass
 
-
 GrantedLicenseTypeDef = TypedDict(
     "GrantedLicenseTypeDef",
     {
         "LicenseArn": str,
         "LicenseName": str,
         "ProductName": str,
         "ProductSKU": str,
@@ -1874,14 +1764,41 @@
     "GetLicenseUsageResponseTypeDef",
     {
         "LicenseUsage": LicenseUsageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "LicenseCountingType": LicenseCountingTypeType,
+    },
+)
+_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "LicenseRules": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "DisassociateWhenNotFound": bool,
+        "ProductInformationList": Sequence[ProductInformationTypeDef],
+    },
+    total=False,
+)
+
+class CreateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
+
 GetLicenseConfigurationResponseTypeDef = TypedDict(
     "GetLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationId": str,
         "LicenseConfigurationArn": str,
         "Name": str,
         "Description": str,
@@ -1891,15 +1808,15 @@
         "LicenseCountHardLimit": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
         "Tags": List[TagTypeDef],
-        "ProductInformationList": List[ProductInformationOutputTypeDef],
+        "ProductInformationList": List[ProductInformationTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
         "DisassociateWhenNotFound": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LicenseConfigurationTypeDef = TypedDict(
@@ -1915,21 +1832,47 @@
         "LicenseCountHardLimit": bool,
         "DisassociateWhenNotFound": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
-        "ProductInformationList": List[ProductInformationOutputTypeDef],
+        "ProductInformationList": List[ProductInformationTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
     },
     total=False,
 )
 
-ProductInformationUnionTypeDef = Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
+_RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "LicenseConfigurationStatus": LicenseConfigurationStatusType,
+        "LicenseRules": Sequence[str],
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "Name": str,
+        "Description": str,
+        "ProductInformationList": Sequence[ProductInformationTypeDef],
+        "DisassociateWhenNotFound": bool,
+    },
+    total=False,
+)
+
+class UpdateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
+
 GetLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     {
         "ReportGenerator": ReportGeneratorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1991,64 +1934,7 @@
     "ListLicenseConfigurationsResponseTypeDef",
     {
         "LicenseConfigurations": List[LicenseConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "LicenseCountingType": LicenseCountingTypeType,
-    },
-)
-_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "LicenseRules": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "DisassociateWhenNotFound": bool,
-        "ProductInformationList": Sequence[ProductInformationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "LicenseConfigurationStatus": LicenseConfigurationStatusType,
-        "LicenseRules": Sequence[str],
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "Name": str,
-        "Description": str,
-        "ProductInformationList": Sequence[ProductInformationUnionTypeDef],
-        "DisassociateWhenNotFound": bool,
-    },
-    total=False,
-)
-
-
-class UpdateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager/type_defs.pyi` & `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_license_manager.type_defs import AcceptGrantRequestRequestTypeDef
 
     data: AcceptGrantRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     ActivationOverrideBehaviorType,
     AllowedOperationType,
     CheckoutTypeType,
     EntitlementDataUnitType,
     EntitlementUnitType,
@@ -40,14 +40,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcceptGrantRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "AutomatedDiscoveryInformationTypeDef",
     "BorrowConfigurationTypeDef",
     "CheckInLicenseRequestRequestTypeDef",
     "EntitlementDataTypeDef",
@@ -91,18 +92,16 @@
     "ListAssociationsForLicenseConfigurationRequestRequestTypeDef",
     "ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
     "ListLicenseSpecificationsForResourceRequestRequestTypeDef",
     "ListLicenseVersionsRequestRequestTypeDef",
     "ResourceInventoryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TokenDataTypeDef",
-    "ProductInformationFilterOutputTypeDef",
     "ProductInformationFilterTypeDef",
     "RejectGrantRequestRequestTypeDef",
-    "ReportContextOutputTypeDef",
     "S3LocationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AcceptGrantResponseTypeDef",
     "CreateGrantResponseTypeDef",
     "CreateGrantVersionResponseTypeDef",
     "CreateLicenseConfigurationResponseTypeDef",
     "CreateLicenseConversionTaskForResourceResponseTypeDef",
@@ -152,42 +151,39 @@
     "ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
     "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
     "ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     "ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef",
     "ListResourceInventoryResponseTypeDef",
     "ListTokensResponseTypeDef",
-    "ProductInformationOutputTypeDef",
     "ProductInformationTypeDef",
-    "ReportContextUnionTypeDef",
     "ReportGeneratorTypeDef",
     "ListFailuresForLicenseConfigurationOperationsResponseTypeDef",
     "CreateLicenseRequestRequestTypeDef",
     "CreateLicenseVersionRequestRequestTypeDef",
     "GrantedLicenseTypeDef",
     "LicenseTypeDef",
     "GetGrantResponseTypeDef",
     "ListDistributedGrantsResponseTypeDef",
     "ListReceivedGrantsForOrganizationResponseTypeDef",
     "ListReceivedGrantsResponseTypeDef",
     "ListLicenseConversionTasksResponseTypeDef",
     "GetLicenseUsageResponseTypeDef",
+    "CreateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseConfigurationResponseTypeDef",
     "LicenseConfigurationTypeDef",
-    "ProductInformationUnionTypeDef",
+    "UpdateLicenseConfigurationRequestRequestTypeDef",
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     "ListLicenseManagerReportGeneratorsResponseTypeDef",
     "ListReceivedLicensesForOrganizationResponseTypeDef",
     "ListReceivedLicensesResponseTypeDef",
     "GetLicenseResponseTypeDef",
     "ListLicenseVersionsResponseTypeDef",
     "ListLicensesResponseTypeDef",
     "ListLicenseConfigurationsResponseTypeDef",
-    "CreateLicenseConfigurationRequestRequestTypeDef",
-    "UpdateLicenseConfigurationRequestRequestTypeDef",
 )
 
 AcceptGrantRequestRequestTypeDef = TypedDict(
     "AcceptGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
@@ -230,19 +226,21 @@
     "_OptionalCheckInLicenseRequestRequestTypeDef",
     {
         "Beneficiary": str,
     },
     total=False,
 )
 
+
 class CheckInLicenseRequestRequestTypeDef(
     _RequiredCheckInLicenseRequestRequestTypeDef, _OptionalCheckInLicenseRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredEntitlementDataTypeDef = TypedDict(
     "_RequiredEntitlementDataTypeDef",
     {
         "Name": str,
         "Unit": EntitlementDataUnitType,
     },
 )
@@ -250,17 +248,19 @@
     "_OptionalEntitlementDataTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class EntitlementDataTypeDef(_RequiredEntitlementDataTypeDef, _OptionalEntitlementDataTypeDef):
     pass
 
+
 MetadataTypeDef = TypedDict(
     "MetadataTypeDef",
     {
         "Name": str,
         "Value": str,
     },
     total=False,
@@ -345,17 +345,19 @@
     "_OptionalDatetimeRangeTypeDef",
     {
         "End": str,
     },
     total=False,
 )
 
+
 class DatetimeRangeTypeDef(_RequiredDatetimeRangeTypeDef, _OptionalDatetimeRangeTypeDef):
     pass
 
+
 _RequiredEntitlementTypeDef = TypedDict(
     "_RequiredEntitlementTypeDef",
     {
         "Name": str,
         "Unit": EntitlementUnitType,
     },
 )
@@ -366,34 +368,38 @@
         "MaxCount": int,
         "Overage": bool,
         "AllowCheckIn": bool,
     },
     total=False,
 )
 
+
 class EntitlementTypeDef(_RequiredEntitlementTypeDef, _OptionalEntitlementTypeDef):
     pass
 
+
 _RequiredIssuerTypeDef = TypedDict(
     "_RequiredIssuerTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalIssuerTypeDef = TypedDict(
     "_OptionalIssuerTypeDef",
     {
         "SignKey": str,
     },
     total=False,
 )
 
+
 class IssuerTypeDef(_RequiredIssuerTypeDef, _OptionalIssuerTypeDef):
     pass
 
+
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "ClientToken": str,
     },
 )
@@ -403,19 +409,21 @@
         "RoleArns": Sequence[str],
         "ExpirationInDays": int,
         "TokenProperties": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteGrantRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
         "Version": str,
     },
 )
@@ -423,19 +431,21 @@
     "_OptionalDeleteGrantRequestRequestTypeDef",
     {
         "StatusReason": str,
     },
     total=False,
 )
 
+
 class DeleteGrantRequestRequestTypeDef(
     _RequiredDeleteGrantRequestRequestTypeDef, _OptionalDeleteGrantRequestRequestTypeDef
 ):
     pass
 
+
 DeleteLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "DeleteLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 
@@ -473,37 +483,41 @@
     "_OptionalEntitlementUsageTypeDef",
     {
         "MaxCount": str,
     },
     total=False,
 )
 
+
 class EntitlementUsageTypeDef(_RequiredEntitlementUsageTypeDef, _OptionalEntitlementUsageTypeDef):
     pass
 
+
 _RequiredExtendLicenseConsumptionRequestRequestTypeDef = TypedDict(
     "_RequiredExtendLicenseConsumptionRequestRequestTypeDef",
     {
         "LicenseConsumptionToken": str,
     },
 )
 _OptionalExtendLicenseConsumptionRequestRequestTypeDef = TypedDict(
     "_OptionalExtendLicenseConsumptionRequestRequestTypeDef",
     {
         "DryRun": bool,
     },
     total=False,
 )
 
+
 class ExtendLicenseConsumptionRequestRequestTypeDef(
     _RequiredExtendLicenseConsumptionRequestRequestTypeDef,
     _OptionalExtendLicenseConsumptionRequestRequestTypeDef,
 ):
     pass
 
+
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
     total=False,
@@ -519,38 +533,42 @@
     "_OptionalGetAccessTokenRequestRequestTypeDef",
     {
         "TokenProperties": Sequence[str],
     },
     total=False,
 )
 
+
 class GetAccessTokenRequestRequestTypeDef(
     _RequiredGetAccessTokenRequestRequestTypeDef, _OptionalGetAccessTokenRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetGrantRequestRequestTypeDef = TypedDict(
     "_RequiredGetGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 _OptionalGetGrantRequestRequestTypeDef = TypedDict(
     "_OptionalGetGrantRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetGrantRequestRequestTypeDef(
     _RequiredGetGrantRequestRequestTypeDef, _OptionalGetGrantRequestRequestTypeDef
 ):
     pass
 
+
 GetLicenseConfigurationRequestRequestTypeDef = TypedDict(
     "GetLicenseConfigurationRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 
@@ -587,19 +605,21 @@
     "_OptionalGetLicenseRequestRequestTypeDef",
     {
         "Version": str,
     },
     total=False,
 )
 
+
 class GetLicenseRequestRequestTypeDef(
     _RequiredGetLicenseRequestRequestTypeDef, _OptionalGetLicenseRequestRequestTypeDef
 ):
     pass
 
+
 GetLicenseUsageRequestRequestTypeDef = TypedDict(
     "GetLicenseUsageRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 
@@ -641,17 +661,19 @@
     "_OptionalInventoryFilterTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class InventoryFilterTypeDef(_RequiredInventoryFilterTypeDef, _OptionalInventoryFilterTypeDef):
     pass
 
+
 LicenseConfigurationAssociationTypeDef = TypedDict(
     "LicenseConfigurationAssociationTypeDef",
     {
         "ResourceArn": str,
         "ResourceType": ResourceTypeType,
         "ResourceOwnerId": str,
         "AssociationTime": datetime,
@@ -683,19 +705,21 @@
     "_OptionalLicenseSpecificationTypeDef",
     {
         "AmiAssociationScope": str,
     },
     total=False,
 )
 
+
 class LicenseSpecificationTypeDef(
     _RequiredLicenseSpecificationTypeDef, _OptionalLicenseSpecificationTypeDef
 ):
     pass
 
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -713,20 +737,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAssociationsForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListAssociationsForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListAssociationsForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef = TypedDict(
     "_RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef = TypedDict(
@@ -734,20 +760,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef(
     _RequiredListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
     _OptionalListFailuresForLicenseConfigurationOperationsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListLicenseSpecificationsForResourceRequestRequestTypeDef = TypedDict(
@@ -755,20 +783,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredListLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalListLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListLicenseVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListLicenseVersionsRequestRequestTypeDef",
     {
         "LicenseArn": str,
     },
 )
 _OptionalListLicenseVersionsRequestRequestTypeDef = TypedDict(
@@ -776,20 +806,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListLicenseVersionsRequestRequestTypeDef(
     _RequiredListLicenseVersionsRequestRequestTypeDef,
     _OptionalListLicenseVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ResourceInventoryTypeDef = TypedDict(
     "ResourceInventoryTypeDef",
     {
         "ResourceId": str,
         "ResourceType": ResourceTypeType,
         "ResourceArn": str,
         "Platform": str,
@@ -816,34 +848,14 @@
         "TokenProperties": List[str],
         "RoleArns": List[str],
         "Status": str,
     },
     total=False,
 )
 
-_RequiredProductInformationFilterOutputTypeDef = TypedDict(
-    "_RequiredProductInformationFilterOutputTypeDef",
-    {
-        "ProductInformationFilterName": str,
-        "ProductInformationFilterComparator": str,
-    },
-)
-_OptionalProductInformationFilterOutputTypeDef = TypedDict(
-    "_OptionalProductInformationFilterOutputTypeDef",
-    {
-        "ProductInformationFilterValue": List[str],
-    },
-    total=False,
-)
-
-class ProductInformationFilterOutputTypeDef(
-    _RequiredProductInformationFilterOutputTypeDef, _OptionalProductInformationFilterOutputTypeDef
-):
-    pass
-
 _RequiredProductInformationFilterTypeDef = TypedDict(
     "_RequiredProductInformationFilterTypeDef",
     {
         "ProductInformationFilterName": str,
         "ProductInformationFilterComparator": str,
     },
 )
@@ -851,33 +863,28 @@
     "_OptionalProductInformationFilterTypeDef",
     {
         "ProductInformationFilterValue": Sequence[str],
     },
     total=False,
 )
 
+
 class ProductInformationFilterTypeDef(
     _RequiredProductInformationFilterTypeDef, _OptionalProductInformationFilterTypeDef
 ):
     pass
 
+
 RejectGrantRequestRequestTypeDef = TypedDict(
     "RejectGrantRequestRequestTypeDef",
     {
         "GrantArn": str,
     },
 )
 
-ReportContextOutputTypeDef = TypedDict(
-    "ReportContextOutputTypeDef",
-    {
-        "licenseConfigurationArns": List[str],
-    },
-)
-
 S3LocationTypeDef = TypedDict(
     "S3LocationTypeDef",
     {
         "bucket": str,
         "keyPrefix": str,
     },
     total=False,
@@ -1036,19 +1043,21 @@
     {
         "Beneficiary": str,
         "NodeId": str,
     },
     total=False,
 )
 
+
 class CheckoutLicenseRequestRequestTypeDef(
     _RequiredCheckoutLicenseRequestRequestTypeDef, _OptionalCheckoutLicenseRequestRequestTypeDef
 ):
     pass
 
+
 CheckoutLicenseResponseTypeDef = TypedDict(
     "CheckoutLicenseResponseTypeDef",
     {
         "CheckoutType": CheckoutTypeType,
         "LicenseConsumptionToken": str,
         "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "SignedToken": str,
@@ -1074,20 +1083,22 @@
     {
         "NodeId": str,
         "CheckoutMetadata": Sequence[MetadataTypeDef],
     },
     total=False,
 )
 
+
 class CheckoutBorrowLicenseRequestRequestTypeDef(
     _RequiredCheckoutBorrowLicenseRequestRequestTypeDef,
     _OptionalCheckoutBorrowLicenseRequestRequestTypeDef,
 ):
     pass
 
+
 CheckoutBorrowLicenseResponseTypeDef = TypedDict(
     "CheckoutBorrowLicenseResponseTypeDef",
     {
         "LicenseArn": str,
         "LicenseConsumptionToken": str,
         "EntitlementsAllowed": List[EntitlementDataTypeDef],
         "NodeId": str,
@@ -1140,20 +1151,22 @@
         "StatusReason": str,
         "SourceVersion": str,
         "Options": OptionsTypeDef,
     },
     total=False,
 )
 
+
 class CreateGrantVersionRequestRequestTypeDef(
     _RequiredCreateGrantVersionRequestRequestTypeDef,
     _OptionalCreateGrantVersionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGrantTypeDef = TypedDict(
     "_RequiredGrantTypeDef",
     {
         "GrantArn": str,
         "GrantName": str,
         "ParentArn": str,
         "LicenseArn": str,
@@ -1169,17 +1182,19 @@
     {
         "StatusReason": str,
         "Options": OptionsTypeDef,
     },
     total=False,
 )
 
+
 class GrantTypeDef(_RequiredGrantTypeDef, _OptionalGrantTypeDef):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1248,20 +1263,22 @@
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateLicenseManagerReportGeneratorRequestRequestTypeDef(
     _RequiredCreateLicenseManagerReportGeneratorRequestRequestTypeDef,
     _OptionalCreateLicenseManagerReportGeneratorRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "LicenseManagerReportGeneratorArn": str,
         "ReportGeneratorName": str,
         "Type": Sequence[ReportTypeType],
         "ReportContext": ReportContextTypeDef,
@@ -1273,20 +1290,22 @@
     "_OptionalUpdateLicenseManagerReportGeneratorRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateLicenseManagerReportGeneratorRequestRequestTypeDef(
     _RequiredUpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
     _OptionalUpdateLicenseManagerReportGeneratorRequestRequestTypeDef,
 ):
     pass
 
+
 LicenseUsageTypeDef = TypedDict(
     "LicenseUsageTypeDef",
     {
         "EntitlementUsages": List[EntitlementUsageTypeDef],
     },
     total=False,
 )
@@ -1356,20 +1375,22 @@
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListReceivedGrantsForOrganizationRequestRequestTypeDef(
     _RequiredListReceivedGrantsForOrganizationRequestRequestTypeDef,
     _OptionalListReceivedGrantsForOrganizationRequestRequestTypeDef,
 ):
     pass
 
+
 ListReceivedGrantsRequestRequestTypeDef = TypedDict(
     "ListReceivedGrantsRequestRequestTypeDef",
     {
         "GrantArns": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "NextToken": str,
         "MaxResults": int,
@@ -1421,20 +1442,22 @@
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
+
 class ListUsageForLicenseConfigurationRequestRequestTypeDef(
     _RequiredListUsageForLicenseConfigurationRequestRequestTypeDef,
     _OptionalListUsageForLicenseConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 GetServiceSettingsResponseTypeDef = TypedDict(
     "GetServiceSettingsResponseTypeDef",
     {
         "S3BucketArn": str,
         "SnsTopicArn": str,
         "OrganizationConfiguration": OrganizationConfigurationTypeDef,
         "EnableCrossAccountsDiscovery": bool,
@@ -1502,40 +1525,44 @@
     {
         "AddLicenseSpecifications": Sequence[LicenseSpecificationTypeDef],
         "RemoveLicenseSpecifications": Sequence[LicenseSpecificationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateLicenseSpecificationsForResourceRequestRequestTypeDef(
     _RequiredUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
     _OptionalUpdateLicenseSpecificationsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
     "_RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
     {
         "LicenseConfigurationArn": str,
     },
 )
 _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef = TypedDict(
     "_OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef(
     _RequiredListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
     _OptionalListAssociationsForLicenseConfigurationRequestListAssociationsForLicenseConfigurationPaginateTypeDef,
 ):
     pass
 
+
 ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef = TypedDict(
     "ListLicenseConfigurationsRequestListLicenseConfigurationsPaginateTypeDef",
     {
         "LicenseConfigurationArns": Sequence[str],
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -1552,20 +1579,22 @@
     "_OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef(
     _RequiredListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
     _OptionalListLicenseSpecificationsForResourceRequestListLicenseSpecificationsForResourcePaginateTypeDef,
 ):
     pass
 
+
 ListResourceInventoryRequestListResourceInventoryPaginateTypeDef = TypedDict(
     "ListResourceInventoryRequestListResourceInventoryPaginateTypeDef",
     {
         "Filters": Sequence[InventoryFilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1582,20 +1611,22 @@
     {
         "Filters": Sequence[FilterTypeDef],
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef(
     _RequiredListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
     _OptionalListUsageForLicenseConfigurationRequestListUsageForLicenseConfigurationPaginateTypeDef,
 ):
     pass
 
+
 ListResourceInventoryResponseTypeDef = TypedDict(
     "ListResourceInventoryResponseTypeDef",
     {
         "ResourceInventoryList": List[ResourceInventoryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1606,37 +1637,28 @@
     {
         "Tokens": List[TokenDataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ProductInformationOutputTypeDef = TypedDict(
-    "ProductInformationOutputTypeDef",
-    {
-        "ResourceType": str,
-        "ProductInformationFilterList": List[ProductInformationFilterOutputTypeDef],
-    },
-)
-
 ProductInformationTypeDef = TypedDict(
     "ProductInformationTypeDef",
     {
         "ResourceType": str,
         "ProductInformationFilterList": Sequence[ProductInformationFilterTypeDef],
     },
 )
 
-ReportContextUnionTypeDef = Union[ReportContextTypeDef, ReportContextOutputTypeDef]
 ReportGeneratorTypeDef = TypedDict(
     "ReportGeneratorTypeDef",
     {
         "ReportGeneratorName": str,
         "ReportType": List[ReportTypeType],
-        "ReportContext": ReportContextOutputTypeDef,
+        "ReportContext": ReportContextTypeDef,
         "ReportFrequency": ReportFrequencyTypeDef,
         "LicenseManagerReportGeneratorArn": str,
         "LastRunStatus": str,
         "LastRunFailureReason": str,
         "LastReportGenerationTime": str,
         "ReportCreatorAccount": str,
         "Description": str,
@@ -1675,19 +1697,21 @@
     "_OptionalCreateLicenseRequestRequestTypeDef",
     {
         "LicenseMetadata": Sequence[MetadataTypeDef],
     },
     total=False,
 )
 
+
 class CreateLicenseRequestRequestTypeDef(
     _RequiredCreateLicenseRequestRequestTypeDef, _OptionalCreateLicenseRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateLicenseVersionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLicenseVersionRequestRequestTypeDef",
     {
         "LicenseArn": str,
         "LicenseName": str,
         "ProductName": str,
         "Issuer": IssuerTypeDef,
@@ -1704,20 +1728,22 @@
     {
         "LicenseMetadata": Sequence[MetadataTypeDef],
         "SourceVersion": str,
     },
     total=False,
 )
 
+
 class CreateLicenseVersionRequestRequestTypeDef(
     _RequiredCreateLicenseVersionRequestRequestTypeDef,
     _OptionalCreateLicenseVersionRequestRequestTypeDef,
 ):
     pass
 
+
 GrantedLicenseTypeDef = TypedDict(
     "GrantedLicenseTypeDef",
     {
         "LicenseArn": str,
         "LicenseName": str,
         "ProductName": str,
         "ProductSKU": str,
@@ -1805,14 +1831,43 @@
     "GetLicenseUsageResponseTypeDef",
     {
         "LicenseUsage": LicenseUsageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Name": str,
+        "LicenseCountingType": LicenseCountingTypeType,
+    },
+)
+_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "LicenseRules": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+        "DisassociateWhenNotFound": bool,
+        "ProductInformationList": Sequence[ProductInformationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 GetLicenseConfigurationResponseTypeDef = TypedDict(
     "GetLicenseConfigurationResponseTypeDef",
     {
         "LicenseConfigurationId": str,
         "LicenseConfigurationArn": str,
         "Name": str,
         "Description": str,
@@ -1822,15 +1877,15 @@
         "LicenseCountHardLimit": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
         "Tags": List[TagTypeDef],
-        "ProductInformationList": List[ProductInformationOutputTypeDef],
+        "ProductInformationList": List[ProductInformationTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
         "DisassociateWhenNotFound": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LicenseConfigurationTypeDef = TypedDict(
@@ -1846,21 +1901,49 @@
         "LicenseCountHardLimit": bool,
         "DisassociateWhenNotFound": bool,
         "ConsumedLicenses": int,
         "Status": str,
         "OwnerAccountId": str,
         "ConsumedLicenseSummaryList": List[ConsumedLicenseSummaryTypeDef],
         "ManagedResourceSummaryList": List[ManagedResourceSummaryTypeDef],
-        "ProductInformationList": List[ProductInformationOutputTypeDef],
+        "ProductInformationList": List[ProductInformationTypeDef],
         "AutomatedDiscoveryInformation": AutomatedDiscoveryInformationTypeDef,
     },
     total=False,
 )
 
-ProductInformationUnionTypeDef = Union[ProductInformationTypeDef, ProductInformationOutputTypeDef]
+_RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "LicenseConfigurationArn": str,
+    },
+)
+_OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateLicenseConfigurationRequestRequestTypeDef",
+    {
+        "LicenseConfigurationStatus": LicenseConfigurationStatusType,
+        "LicenseRules": Sequence[str],
+        "LicenseCount": int,
+        "LicenseCountHardLimit": bool,
+        "Name": str,
+        "Description": str,
+        "ProductInformationList": Sequence[ProductInformationTypeDef],
+        "DisassociateWhenNotFound": bool,
+    },
+    total=False,
+)
+
+
+class UpdateLicenseConfigurationRequestRequestTypeDef(
+    _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
+    _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
+):
+    pass
+
+
 GetLicenseManagerReportGeneratorResponseTypeDef = TypedDict(
     "GetLicenseManagerReportGeneratorResponseTypeDef",
     {
         "ReportGenerator": ReportGeneratorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1922,61 +2005,7 @@
     "ListLicenseConfigurationsResponseTypeDef",
     {
         "LicenseConfigurations": List[LicenseConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Name": str,
-        "LicenseCountingType": LicenseCountingTypeType,
-    },
-)
-_OptionalCreateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "LicenseRules": Sequence[str],
-        "Tags": Sequence[TagTypeDef],
-        "DisassociateWhenNotFound": bool,
-        "ProductInformationList": Sequence[ProductInformationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredCreateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalCreateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "LicenseConfigurationArn": str,
-    },
-)
-_OptionalUpdateLicenseConfigurationRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateLicenseConfigurationRequestRequestTypeDef",
-    {
-        "LicenseConfigurationStatus": LicenseConfigurationStatusType,
-        "LicenseRules": Sequence[str],
-        "LicenseCount": int,
-        "LicenseCountHardLimit": bool,
-        "Name": str,
-        "Description": str,
-        "ProductInformationList": Sequence[ProductInformationUnionTypeDef],
-        "DisassociateWhenNotFound": bool,
-    },
-    total=False,
-)
-
-class UpdateLicenseConfigurationRequestRequestTypeDef(
-    _RequiredUpdateLicenseConfigurationRequestRequestTypeDef,
-    _OptionalUpdateLicenseConfigurationRequestRequestTypeDef,
-):
-    pass
```

### Comparing `types-aiobotocore-license-manager-2.5.2.post1/types_aiobotocore_license_manager.egg-info/SOURCES.txt` & `types-aiobotocore-license-manager-2.5.2.post2/types_aiobotocore_license_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

