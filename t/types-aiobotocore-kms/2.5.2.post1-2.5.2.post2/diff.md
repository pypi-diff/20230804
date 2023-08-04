# Comparing `tmp/types-aiobotocore-kms-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-kms-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kms-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-kms-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:14 2023, max compression
```

## Comparing `types-aiobotocore-kms-2.5.2.post1.tar` & `types-aiobotocore-kms-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.097545 types-aiobotocore-kms-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-08-02 14:52:33.097545 types-aiobotocore-kms-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16722 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.097545 types-aiobotocore-kms-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.097545 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42763 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    42697 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40489 2023-08-02 14:41:40.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40430 2023-08-02 14:41:40.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:39.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.097545 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18224 2023-08-02 14:52:32.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:32.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:32.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:32.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:32.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:32.000000 types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.816643 types-aiobotocore-kms-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:42:15.000000 types-aiobotocore-kms-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13506 2023-08-04 13:59:14.816643 types-aiobotocore-kms-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12004 2023-08-04 13:42:15.000000 types-aiobotocore-kms-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:14.816643 types-aiobotocore-kms-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:42:15.000000 types-aiobotocore-kms-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.816643 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1813 2023-08-04 13:42:15.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1812 2023-08-04 13:42:15.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:42:15.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43199 2023-08-04 13:42:16.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    43133 2023-08-04 13:42:16.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13061 2023-08-04 13:42:17.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13059 2023-08-04 13:42:17.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8418 2023-08-04 13:42:17.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8409 2023-08-04 13:42:17.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:42:15.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    40736 2023-08-04 13:42:18.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    40675 2023-08-04 13:42:17.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:42:15.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:14.816643 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13506 2023-08-04 13:59:14.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      737 2023-08-04 13:59:14.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:14.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:14.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:14.000000 types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kms-2.5.2.post1/LICENSE` & `types-aiobotocore-kms-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kms-2.5.2.post1/setup.py` & `types-aiobotocore-kms-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kms",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_kms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KMS 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/__init__.py` & `types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/__init__.pyi` & `types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/__main__.py` & `types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KMS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.KMS 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS\nOther"
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

### Comparing `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/client.py` & `types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     GenerateDataKeyWithoutPlaintextResponseTypeDef,
     GenerateMacResponseTypeDef,
     GenerateRandomResponseTypeDef,
     GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportResponseTypeDef,
     GetPublicKeyResponseTypeDef,
-    GrantConstraintsUnionTypeDef,
+    GrantConstraintsTypeDef,
     ListAliasesResponseTypeDef,
     ListGrantsResponseTypeDef,
     ListKeyPoliciesResponseTypeDef,
     ListKeysResponseTypeDef,
     ListResourceTagsResponseTypeDef,
     RecipientInfoTypeDef,
     ReEncryptResponseTypeDef,
@@ -87,40 +87,38 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("KMSClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     CloudHsmClusterInUseException: Type[BotocoreClientError]
     CloudHsmClusterInvalidConfigurationException: Type[BotocoreClientError]
     CloudHsmClusterNotActiveException: Type[BotocoreClientError]
     CloudHsmClusterNotFoundException: Type[BotocoreClientError]
     CloudHsmClusterNotRelatedException: Type[BotocoreClientError]
     CustomKeyStoreHasCMKsException: Type[BotocoreClientError]
     CustomKeyStoreInvalidStateException: Type[BotocoreClientError]
     CustomKeyStoreNameInUseException: Type[BotocoreClientError]
     CustomKeyStoreNotFoundException: Type[BotocoreClientError]
     DependencyTimeoutException: Type[BotocoreClientError]
     DisabledException: Type[BotocoreClientError]
+    DryRunOperationException: Type[BotocoreClientError]
     ExpiredImportTokenException: Type[BotocoreClientError]
     IncorrectKeyException: Type[BotocoreClientError]
     IncorrectKeyMaterialException: Type[BotocoreClientError]
     IncorrectTrustAnchorException: Type[BotocoreClientError]
     InvalidAliasNameException: Type[BotocoreClientError]
     InvalidArnException: Type[BotocoreClientError]
     InvalidCiphertextException: Type[BotocoreClientError]
@@ -148,15 +146,14 @@
     XksProxyUriEndpointInUseException: Type[BotocoreClientError]
     XksProxyUriInUseException: Type[BotocoreClientError]
     XksProxyUriUnreachableException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInUseException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInvalidConfigurationException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceNotFoundException: Type[BotocoreClientError]
 
-
 class KMSClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/)
     """
 
     meta: ClientMeta
@@ -165,59 +162,53 @@
     def exceptions(self) -> Exceptions:
         """
         KMSClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#can_paginate)
         """
-
     async def cancel_key_deletion(self, *, KeyId: str) -> CancelKeyDeletionResponseTypeDef:
         """
         Cancels the deletion of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.cancel_key_deletion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#cancel_key_deletion)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#close)
         """
-
     async def connect_custom_key_store(self, *, CustomKeyStoreId: str) -> Dict[str, Any]:
         """
         Connects or reconnects a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ to its backing key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.connect_custom_key_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#connect_custom_key_store)
         """
-
     async def create_alias(
         self, *, AliasName: str, TargetKeyId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a friendly name for a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#create_alias)
         """
-
     async def create_custom_key_store(
         self,
         *,
         CustomKeyStoreName: str,
         CloudHsmClusterId: str = ...,
         TrustAnchorCertificate: str = ...,
         KeyStorePassword: str = ...,
@@ -232,33 +223,32 @@
         Creates a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ backed by a key store that you own and manage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_custom_key_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#create_custom_key_store)
         """
-
     async def create_grant(
         self,
         *,
         KeyId: str,
         GranteePrincipal: str,
         Operations: Sequence[GrantOperationType],
         RetiringPrincipal: str = ...,
-        Constraints: GrantConstraintsUnionTypeDef = ...,
+        Constraints: GrantConstraintsTypeDef = ...,
         GrantTokens: Sequence[str] = ...,
-        Name: str = ...
+        Name: str = ...,
+        DryRun: bool = ...
     ) -> CreateGrantResponseTypeDef:
         """
         Adds a grant to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#create_grant)
         """
-
     async def create_key(
         self,
         *,
         Policy: str = ...,
         Description: str = ...,
         KeyUsage: KeyUsageTypeType = ...,
         CustomerMasterKeySpec: CustomerMasterKeySpecType = ...,
@@ -274,61 +264,57 @@
         Creates a unique customer managed [KMS
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#kms-
         keys)_ in your Amazon Web Services account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#create_key)
         """
-
     async def decrypt(
         self,
         *,
         CiphertextBlob: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         KeyId: str = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
+        DryRun: bool = ...
     ) -> DecryptResponseTypeDef:
         """
         Decrypts ciphertext that was encrypted by a KMS key using any of the following
         operations: *  Encrypt *  GenerateDataKey *  GenerateDataKeyPair *
         GenerateDataKeyWithoutPlaintext *  GenerateDataKeyPairWithoutPlaintext You can
         use this operation to decrypt ciphertext that was enc...
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.decrypt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#decrypt)
         """
-
     async def delete_alias(self, *, AliasName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#delete_alias)
         """
-
     async def delete_custom_key_store(self, *, CustomKeyStoreId: str) -> Dict[str, Any]:
         """
         Deletes a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_custom_key_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#delete_custom_key_store)
         """
-
     async def delete_imported_key_material(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes key material that was previously imported.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_imported_key_material)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#delete_imported_key_material)
         """
-
     async def describe_custom_key_stores(
         self,
         *,
         CustomKeyStoreId: str = ...,
         CustomKeyStoreName: str = ...,
         Limit: int = ...,
         Marker: str = ...
@@ -337,238 +323,225 @@
         Gets information about [custom key
         stores](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.describe_custom_key_stores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#describe_custom_key_stores)
         """
-
     async def describe_key(
         self, *, KeyId: str, GrantTokens: Sequence[str] = ...
     ) -> DescribeKeyResponseTypeDef:
         """
         Provides detailed information about a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.describe_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#describe_key)
         """
-
     async def disable_key(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Sets the state of a KMS key to disabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disable_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#disable_key)
         """
-
     async def disable_key_rotation(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Disables [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-
         keys.html)_ of the specified symmetric encryption KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disable_key_rotation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#disable_key_rotation)
         """
-
     async def disconnect_custom_key_store(self, *, CustomKeyStoreId: str) -> Dict[str, Any]:
         """
         Disconnects the [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ from its backing key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disconnect_custom_key_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#disconnect_custom_key_store)
         """
-
     async def enable_key(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Sets the key state of a KMS key to enabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#enable_key)
         """
-
     async def enable_key_rotation(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Enables [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-
         keys.html)_ of the specified symmetric encryption KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key_rotation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#enable_key_rotation)
         """
-
     async def encrypt(
         self,
         *,
         KeyId: str,
         Plaintext: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
-        EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...
+        EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
+        DryRun: bool = ...
     ) -> EncryptResponseTypeDef:
         """
         Encrypts plaintext of up to 4,096 bytes using a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.encrypt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#encrypt)
         """
-
     async def generate_data_key(
         self,
         *,
         KeyId: str,
         EncryptionContext: Mapping[str, str] = ...,
         NumberOfBytes: int = ...,
         KeySpec: DataKeySpecType = ...,
         GrantTokens: Sequence[str] = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyResponseTypeDef:
         """
         Returns a unique symmetric data key for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key)
         """
-
     async def generate_data_key_pair(
         self,
         *,
         KeyId: str,
         KeyPairSpec: DataKeyPairSpecType,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyPairResponseTypeDef:
         """
         Returns a unique asymmetric data key pair for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_pair)
         """
-
     async def generate_data_key_pair_without_plaintext(
         self,
         *,
         KeyId: str,
         KeyPairSpec: DataKeyPairSpecType,
         EncryptionContext: Mapping[str, str] = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyPairWithoutPlaintextResponseTypeDef:
         """
         Returns a unique asymmetric data key pair for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair_without_plaintext)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_pair_without_plaintext)
         """
-
     async def generate_data_key_without_plaintext(
         self,
         *,
         KeyId: str,
         EncryptionContext: Mapping[str, str] = ...,
         KeySpec: DataKeySpecType = ...,
         NumberOfBytes: int = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyWithoutPlaintextResponseTypeDef:
         """
         Returns a unique symmetric data key for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_without_plaintext)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_without_plaintext)
         """
-
     async def generate_mac(
         self,
         *,
         Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> GenerateMacResponseTypeDef:
         """
         Generates a hash-based message authentication code (HMAC) for a message using an
         HMAC KMS key and a MAC algorithm that the key supports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_mac)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_mac)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_presigned_url)
         """
-
     async def generate_random(
         self,
         *,
         NumberOfBytes: int = ...,
         CustomKeyStoreId: str = ...,
         Recipient: RecipientInfoTypeDef = ...
     ) -> GenerateRandomResponseTypeDef:
         """
         Returns a random byte string that is cryptographically secure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_random)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_random)
         """
-
     async def get_key_policy(self, *, KeyId: str, PolicyName: str) -> GetKeyPolicyResponseTypeDef:
         """
         Gets a key policy attached to the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_key_policy)
         """
-
     async def get_key_rotation_status(self, *, KeyId: str) -> GetKeyRotationStatusResponseTypeDef:
         """
         Gets a Boolean value that indicates whether [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-
         keys.html)_ is enabled for the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_rotation_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_key_rotation_status)
         """
-
     async def get_parameters_for_import(
         self,
         *,
         KeyId: str,
         WrappingAlgorithm: AlgorithmSpecType,
         WrappingKeySpec: WrappingKeySpecType
     ) -> GetParametersForImportResponseTypeDef:
         """
         Returns the public key and an import token you need to import or reimport key
         material for a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_parameters_for_import)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_parameters_for_import)
         """
-
     async def get_public_key(
         self, *, KeyId: str, GrantTokens: Sequence[str] = ...
     ) -> GetPublicKeyResponseTypeDef:
         """
         Returns the public key of an asymmetric KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_public_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_public_key)
         """
-
     async def import_key_material(
         self,
         *,
         KeyId: str,
         ImportToken: BlobTypeDef,
         EncryptedKeyMaterial: BlobTypeDef,
         ValidTo: TimestampTypeDef = ...,
@@ -577,25 +550,23 @@
         """
         Imports or reimports key material into an existing KMS key that was created
         without key material.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.import_key_material)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#import_key_material)
         """
-
     async def list_aliases(
         self, *, KeyId: str = ..., Limit: int = ..., Marker: str = ...
     ) -> ListAliasesResponseTypeDef:
         """
         Gets a list of aliases in the caller's Amazon Web Services account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_aliases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_aliases)
         """
-
     async def list_grants(
         self,
         *,
         KeyId: str,
         Limit: int = ...,
         Marker: str = ...,
         GrantId: str = ...,
@@ -603,89 +574,83 @@
     ) -> ListGrantsResponseTypeDef:
         """
         Gets a list of all grants for the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_grants)
         """
-
     async def list_key_policies(
         self, *, KeyId: str, Limit: int = ..., Marker: str = ...
     ) -> ListKeyPoliciesResponseTypeDef:
         """
         Gets the names of the key policies that are attached to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_key_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_key_policies)
         """
-
     async def list_keys(self, *, Limit: int = ..., Marker: str = ...) -> ListKeysResponseTypeDef:
         """
         Gets a list of all KMS keys in the caller's Amazon Web Services account and
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_keys)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_keys)
         """
-
     async def list_resource_tags(
         self, *, KeyId: str, Limit: int = ..., Marker: str = ...
     ) -> ListResourceTagsResponseTypeDef:
         """
         Returns all tags on the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_resource_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_resource_tags)
         """
-
     async def list_retirable_grants(
         self, *, RetiringPrincipal: str, Limit: int = ..., Marker: str = ...
     ) -> ListGrantsResponseTypeDef:
         """
         Returns information about all grants in the Amazon Web Services account and
         Region that have the specified retiring principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_retirable_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_retirable_grants)
         """
-
     async def put_key_policy(
         self,
         *,
         KeyId: str,
         PolicyName: str,
         Policy: str,
         BypassPolicyLockoutSafetyCheck: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Attaches a key policy to the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.put_key_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#put_key_policy)
         """
-
     async def re_encrypt(
         self,
         *,
         CiphertextBlob: BlobTypeDef,
         DestinationKeyId: str,
         SourceEncryptionContext: Mapping[str, str] = ...,
         SourceKeyId: str = ...,
         DestinationEncryptionContext: Mapping[str, str] = ...,
         SourceEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         DestinationEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> ReEncryptResponseTypeDef:
         """
         Decrypts ciphertext and then reencrypts it entirely within KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.re_encrypt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#re_encrypt)
         """
-
     async def replicate_key(
         self,
         *,
         KeyId: str,
         ReplicaRegion: str,
         Policy: str = ...,
         BypassPolicyLockoutSafetyCheck: bool = ...,
@@ -694,95 +659,90 @@
     ) -> ReplicateKeyResponseTypeDef:
         """
         Replicates a multi-Region key into the specified Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.replicate_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#replicate_key)
         """
-
     async def retire_grant(
-        self, *, GrantToken: str = ..., KeyId: str = ..., GrantId: str = ...
+        self, *, GrantToken: str = ..., KeyId: str = ..., GrantId: str = ..., DryRun: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.retire_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#retire_grant)
         """
-
-    async def revoke_grant(self, *, KeyId: str, GrantId: str) -> EmptyResponseMetadataTypeDef:
+    async def revoke_grant(
+        self, *, KeyId: str, GrantId: str, DryRun: bool = ...
+    ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.revoke_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#revoke_grant)
         """
-
     async def schedule_key_deletion(
         self, *, KeyId: str, PendingWindowInDays: int = ...
     ) -> ScheduleKeyDeletionResponseTypeDef:
         """
         Schedules the deletion of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.schedule_key_deletion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#schedule_key_deletion)
         """
-
     async def sign(
         self,
         *,
         KeyId: str,
         Message: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> SignResponseTypeDef:
         """
         Creates a [digital signature](https://en.wikipedia.org/wiki/Digital_signature)_
         for a message or message digest by using the private key in an asymmetric
         signing KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.sign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#sign)
         """
-
     async def tag_resource(
         self, *, KeyId: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or edits tags on a [customer managed
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#customer-
         cmk)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#tag_resource)
         """
-
     async def untag_resource(
         self, *, KeyId: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes tags from a [customer managed
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#customer-
         cmk)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#untag_resource)
         """
-
     async def update_alias(
         self, *, AliasName: str, TargetKeyId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associates an existing KMS alias with a different KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#update_alias)
         """
-
     async def update_custom_key_store(
         self,
         *,
         CustomKeyStoreId: str,
         NewCustomKeyStoreName: str = ...,
         KeyStorePassword: str = ...,
         CloudHsmClusterId: str = ...,
@@ -794,130 +754,119 @@
     ) -> Dict[str, Any]:
         """
         Changes the properties of a custom key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_custom_key_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#update_custom_key_store)
         """
-
     async def update_key_description(
         self, *, KeyId: str, Description: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the description of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_key_description)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#update_key_description)
         """
-
     async def update_primary_region(
         self, *, KeyId: str, PrimaryRegion: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the primary key of a multi-Region key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_primary_region)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#update_primary_region)
         """
-
     async def verify(
         self,
         *,
         KeyId: str,
         Message: BlobTypeDef,
         Signature: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> VerifyResponseTypeDef:
         """
         Verifies a digital signature that was generated by the  Sign operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#verify)
         """
-
     async def verify_mac(
         self,
         *,
         Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
         Mac: BlobTypeDef,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> VerifyMacResponseTypeDef:
         """
         Verifies the hash-based message authentication code (HMAC) for a specified
         message, HMAC KMS key, and MAC algorithm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify_mac)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#verify_mac)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_custom_key_stores"]
     ) -> DescribeCustomKeyStoresPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_aliases"]) -> ListAliasesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_grants"]) -> ListGrantsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_key_policies"]
     ) -> ListKeyPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_keys"]) -> ListKeysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_tags"]
     ) -> ListResourceTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_retirable_grants"]
     ) -> ListRetirableGrantsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "KMSClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/)
         """
```

### Comparing `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/client.pyi` & `types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     GenerateDataKeyWithoutPlaintextResponseTypeDef,
     GenerateMacResponseTypeDef,
     GenerateRandomResponseTypeDef,
     GetKeyPolicyResponseTypeDef,
     GetKeyRotationStatusResponseTypeDef,
     GetParametersForImportResponseTypeDef,
     GetPublicKeyResponseTypeDef,
-    GrantConstraintsUnionTypeDef,
+    GrantConstraintsTypeDef,
     ListAliasesResponseTypeDef,
     ListGrantsResponseTypeDef,
     ListKeyPoliciesResponseTypeDef,
     ListKeysResponseTypeDef,
     ListResourceTagsResponseTypeDef,
     RecipientInfoTypeDef,
     ReEncryptResponseTypeDef,
@@ -87,37 +87,41 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("KMSClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AlreadyExistsException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     CloudHsmClusterInUseException: Type[BotocoreClientError]
     CloudHsmClusterInvalidConfigurationException: Type[BotocoreClientError]
     CloudHsmClusterNotActiveException: Type[BotocoreClientError]
     CloudHsmClusterNotFoundException: Type[BotocoreClientError]
     CloudHsmClusterNotRelatedException: Type[BotocoreClientError]
     CustomKeyStoreHasCMKsException: Type[BotocoreClientError]
     CustomKeyStoreInvalidStateException: Type[BotocoreClientError]
     CustomKeyStoreNameInUseException: Type[BotocoreClientError]
     CustomKeyStoreNotFoundException: Type[BotocoreClientError]
     DependencyTimeoutException: Type[BotocoreClientError]
     DisabledException: Type[BotocoreClientError]
+    DryRunOperationException: Type[BotocoreClientError]
     ExpiredImportTokenException: Type[BotocoreClientError]
     IncorrectKeyException: Type[BotocoreClientError]
     IncorrectKeyMaterialException: Type[BotocoreClientError]
     IncorrectTrustAnchorException: Type[BotocoreClientError]
     InvalidAliasNameException: Type[BotocoreClientError]
     InvalidArnException: Type[BotocoreClientError]
     InvalidCiphertextException: Type[BotocoreClientError]
@@ -145,14 +149,15 @@
     XksProxyUriEndpointInUseException: Type[BotocoreClientError]
     XksProxyUriInUseException: Type[BotocoreClientError]
     XksProxyUriUnreachableException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInUseException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceInvalidConfigurationException: Type[BotocoreClientError]
     XksProxyVpcEndpointServiceNotFoundException: Type[BotocoreClientError]
 
+
 class KMSClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/)
     """
 
     meta: ClientMeta
@@ -161,53 +166,59 @@
     def exceptions(self) -> Exceptions:
         """
         KMSClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#can_paginate)
         """
+
     async def cancel_key_deletion(self, *, KeyId: str) -> CancelKeyDeletionResponseTypeDef:
         """
         Cancels the deletion of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.cancel_key_deletion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#cancel_key_deletion)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#close)
         """
+
     async def connect_custom_key_store(self, *, CustomKeyStoreId: str) -> Dict[str, Any]:
         """
         Connects or reconnects a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ to its backing key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.connect_custom_key_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#connect_custom_key_store)
         """
+
     async def create_alias(
         self, *, AliasName: str, TargetKeyId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a friendly name for a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#create_alias)
         """
+
     async def create_custom_key_store(
         self,
         *,
         CustomKeyStoreName: str,
         CloudHsmClusterId: str = ...,
         TrustAnchorCertificate: str = ...,
         KeyStorePassword: str = ...,
@@ -222,31 +233,34 @@
         Creates a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ backed by a key store that you own and manage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_custom_key_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#create_custom_key_store)
         """
+
     async def create_grant(
         self,
         *,
         KeyId: str,
         GranteePrincipal: str,
         Operations: Sequence[GrantOperationType],
         RetiringPrincipal: str = ...,
-        Constraints: GrantConstraintsUnionTypeDef = ...,
+        Constraints: GrantConstraintsTypeDef = ...,
         GrantTokens: Sequence[str] = ...,
-        Name: str = ...
+        Name: str = ...,
+        DryRun: bool = ...
     ) -> CreateGrantResponseTypeDef:
         """
         Adds a grant to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#create_grant)
         """
+
     async def create_key(
         self,
         *,
         Policy: str = ...,
         Description: str = ...,
         KeyUsage: KeyUsageTypeType = ...,
         CustomerMasterKeySpec: CustomerMasterKeySpecType = ...,
@@ -262,56 +276,62 @@
         Creates a unique customer managed [KMS
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#kms-
         keys)_ in your Amazon Web Services account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.create_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#create_key)
         """
+
     async def decrypt(
         self,
         *,
         CiphertextBlob: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
         KeyId: str = ...,
         EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
+        DryRun: bool = ...
     ) -> DecryptResponseTypeDef:
         """
         Decrypts ciphertext that was encrypted by a KMS key using any of the following
         operations: *  Encrypt *  GenerateDataKey *  GenerateDataKeyPair *
         GenerateDataKeyWithoutPlaintext *  GenerateDataKeyPairWithoutPlaintext You can
         use this operation to decrypt ciphertext that was enc...
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.decrypt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#decrypt)
         """
+
     async def delete_alias(self, *, AliasName: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified alias.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#delete_alias)
         """
+
     async def delete_custom_key_store(self, *, CustomKeyStoreId: str) -> Dict[str, Any]:
         """
         Deletes a [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_custom_key_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#delete_custom_key_store)
         """
+
     async def delete_imported_key_material(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Deletes key material that was previously imported.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.delete_imported_key_material)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#delete_imported_key_material)
         """
+
     async def describe_custom_key_stores(
         self,
         *,
         CustomKeyStoreId: str = ...,
         CustomKeyStoreName: str = ...,
         Limit: int = ...,
         Marker: str = ...
@@ -320,219 +340,244 @@
         Gets information about [custom key
         stores](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ in the account and Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.describe_custom_key_stores)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#describe_custom_key_stores)
         """
+
     async def describe_key(
         self, *, KeyId: str, GrantTokens: Sequence[str] = ...
     ) -> DescribeKeyResponseTypeDef:
         """
         Provides detailed information about a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.describe_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#describe_key)
         """
+
     async def disable_key(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Sets the state of a KMS key to disabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disable_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#disable_key)
         """
+
     async def disable_key_rotation(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Disables [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-
         keys.html)_ of the specified symmetric encryption KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disable_key_rotation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#disable_key_rotation)
         """
+
     async def disconnect_custom_key_store(self, *, CustomKeyStoreId: str) -> Dict[str, Any]:
         """
         Disconnects the [custom key
         store](https://docs.aws.amazon.com/kms/latest/developerguide/custom-key-store-
         overview.html)_ from its backing key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.disconnect_custom_key_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#disconnect_custom_key_store)
         """
+
     async def enable_key(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Sets the key state of a KMS key to enabled.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#enable_key)
         """
+
     async def enable_key_rotation(self, *, KeyId: str) -> EmptyResponseMetadataTypeDef:
         """
         Enables [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-
         keys.html)_ of the specified symmetric encryption KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.enable_key_rotation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#enable_key_rotation)
         """
+
     async def encrypt(
         self,
         *,
         KeyId: str,
         Plaintext: BlobTypeDef,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
-        EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...
+        EncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
+        DryRun: bool = ...
     ) -> EncryptResponseTypeDef:
         """
         Encrypts plaintext of up to 4,096 bytes using a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.encrypt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#encrypt)
         """
+
     async def generate_data_key(
         self,
         *,
         KeyId: str,
         EncryptionContext: Mapping[str, str] = ...,
         NumberOfBytes: int = ...,
         KeySpec: DataKeySpecType = ...,
         GrantTokens: Sequence[str] = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyResponseTypeDef:
         """
         Returns a unique symmetric data key for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key)
         """
+
     async def generate_data_key_pair(
         self,
         *,
         KeyId: str,
         KeyPairSpec: DataKeyPairSpecType,
         EncryptionContext: Mapping[str, str] = ...,
         GrantTokens: Sequence[str] = ...,
-        Recipient: RecipientInfoTypeDef = ...
+        Recipient: RecipientInfoTypeDef = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyPairResponseTypeDef:
         """
         Returns a unique asymmetric data key pair for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_pair)
         """
+
     async def generate_data_key_pair_without_plaintext(
         self,
         *,
         KeyId: str,
         KeyPairSpec: DataKeyPairSpecType,
         EncryptionContext: Mapping[str, str] = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyPairWithoutPlaintextResponseTypeDef:
         """
         Returns a unique asymmetric data key pair for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_pair_without_plaintext)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_pair_without_plaintext)
         """
+
     async def generate_data_key_without_plaintext(
         self,
         *,
         KeyId: str,
         EncryptionContext: Mapping[str, str] = ...,
         KeySpec: DataKeySpecType = ...,
         NumberOfBytes: int = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> GenerateDataKeyWithoutPlaintextResponseTypeDef:
         """
         Returns a unique symmetric data key for use outside of KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_data_key_without_plaintext)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_data_key_without_plaintext)
         """
+
     async def generate_mac(
         self,
         *,
         Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> GenerateMacResponseTypeDef:
         """
         Generates a hash-based message authentication code (HMAC) for a message using an
         HMAC KMS key and a MAC algorithm that the key supports.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_mac)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_mac)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_presigned_url)
         """
+
     async def generate_random(
         self,
         *,
         NumberOfBytes: int = ...,
         CustomKeyStoreId: str = ...,
         Recipient: RecipientInfoTypeDef = ...
     ) -> GenerateRandomResponseTypeDef:
         """
         Returns a random byte string that is cryptographically secure.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.generate_random)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#generate_random)
         """
+
     async def get_key_policy(self, *, KeyId: str, PolicyName: str) -> GetKeyPolicyResponseTypeDef:
         """
         Gets a key policy attached to the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_key_policy)
         """
+
     async def get_key_rotation_status(self, *, KeyId: str) -> GetKeyRotationStatusResponseTypeDef:
         """
         Gets a Boolean value that indicates whether [automatic rotation of the key
         material](https://docs.aws.amazon.com/kms/latest/developerguide/rotate-
         keys.html)_ is enabled for the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_key_rotation_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_key_rotation_status)
         """
+
     async def get_parameters_for_import(
         self,
         *,
         KeyId: str,
         WrappingAlgorithm: AlgorithmSpecType,
         WrappingKeySpec: WrappingKeySpecType
     ) -> GetParametersForImportResponseTypeDef:
         """
         Returns the public key and an import token you need to import or reimport key
         material for a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_parameters_for_import)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_parameters_for_import)
         """
+
     async def get_public_key(
         self, *, KeyId: str, GrantTokens: Sequence[str] = ...
     ) -> GetPublicKeyResponseTypeDef:
         """
         Returns the public key of an asymmetric KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_public_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_public_key)
         """
+
     async def import_key_material(
         self,
         *,
         KeyId: str,
         ImportToken: BlobTypeDef,
         EncryptedKeyMaterial: BlobTypeDef,
         ValidTo: TimestampTypeDef = ...,
@@ -541,23 +586,25 @@
         """
         Imports or reimports key material into an existing KMS key that was created
         without key material.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.import_key_material)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#import_key_material)
         """
+
     async def list_aliases(
         self, *, KeyId: str = ..., Limit: int = ..., Marker: str = ...
     ) -> ListAliasesResponseTypeDef:
         """
         Gets a list of aliases in the caller's Amazon Web Services account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_aliases)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_aliases)
         """
+
     async def list_grants(
         self,
         *,
         KeyId: str,
         Limit: int = ...,
         Marker: str = ...,
         GrantId: str = ...,
@@ -565,82 +612,90 @@
     ) -> ListGrantsResponseTypeDef:
         """
         Gets a list of all grants for the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_grants)
         """
+
     async def list_key_policies(
         self, *, KeyId: str, Limit: int = ..., Marker: str = ...
     ) -> ListKeyPoliciesResponseTypeDef:
         """
         Gets the names of the key policies that are attached to a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_key_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_key_policies)
         """
+
     async def list_keys(self, *, Limit: int = ..., Marker: str = ...) -> ListKeysResponseTypeDef:
         """
         Gets a list of all KMS keys in the caller's Amazon Web Services account and
         Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_keys)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_keys)
         """
+
     async def list_resource_tags(
         self, *, KeyId: str, Limit: int = ..., Marker: str = ...
     ) -> ListResourceTagsResponseTypeDef:
         """
         Returns all tags on the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_resource_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_resource_tags)
         """
+
     async def list_retirable_grants(
         self, *, RetiringPrincipal: str, Limit: int = ..., Marker: str = ...
     ) -> ListGrantsResponseTypeDef:
         """
         Returns information about all grants in the Amazon Web Services account and
         Region that have the specified retiring principal.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.list_retirable_grants)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#list_retirable_grants)
         """
+
     async def put_key_policy(
         self,
         *,
         KeyId: str,
         PolicyName: str,
         Policy: str,
         BypassPolicyLockoutSafetyCheck: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Attaches a key policy to the specified KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.put_key_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#put_key_policy)
         """
+
     async def re_encrypt(
         self,
         *,
         CiphertextBlob: BlobTypeDef,
         DestinationKeyId: str,
         SourceEncryptionContext: Mapping[str, str] = ...,
         SourceKeyId: str = ...,
         DestinationEncryptionContext: Mapping[str, str] = ...,
         SourceEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
         DestinationEncryptionAlgorithm: EncryptionAlgorithmSpecType = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> ReEncryptResponseTypeDef:
         """
         Decrypts ciphertext and then reencrypts it entirely within KMS.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.re_encrypt)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#re_encrypt)
         """
+
     async def replicate_key(
         self,
         *,
         KeyId: str,
         ReplicaRegion: str,
         Policy: str = ...,
         BypassPolicyLockoutSafetyCheck: bool = ...,
@@ -649,87 +704,98 @@
     ) -> ReplicateKeyResponseTypeDef:
         """
         Replicates a multi-Region key into the specified Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.replicate_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#replicate_key)
         """
+
     async def retire_grant(
-        self, *, GrantToken: str = ..., KeyId: str = ..., GrantId: str = ...
+        self, *, GrantToken: str = ..., KeyId: str = ..., GrantId: str = ..., DryRun: bool = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes a grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.retire_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#retire_grant)
         """
-    async def revoke_grant(self, *, KeyId: str, GrantId: str) -> EmptyResponseMetadataTypeDef:
+
+    async def revoke_grant(
+        self, *, KeyId: str, GrantId: str, DryRun: bool = ...
+    ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes the specified grant.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.revoke_grant)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#revoke_grant)
         """
+
     async def schedule_key_deletion(
         self, *, KeyId: str, PendingWindowInDays: int = ...
     ) -> ScheduleKeyDeletionResponseTypeDef:
         """
         Schedules the deletion of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.schedule_key_deletion)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#schedule_key_deletion)
         """
+
     async def sign(
         self,
         *,
         KeyId: str,
         Message: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> SignResponseTypeDef:
         """
         Creates a [digital signature](https://en.wikipedia.org/wiki/Digital_signature)_
         for a message or message digest by using the private key in an asymmetric
         signing KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.sign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#sign)
         """
+
     async def tag_resource(
         self, *, KeyId: str, Tags: Sequence[TagTypeDef]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or edits tags on a [customer managed
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#customer-
         cmk)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#tag_resource)
         """
+
     async def untag_resource(
         self, *, KeyId: str, TagKeys: Sequence[str]
     ) -> EmptyResponseMetadataTypeDef:
         """
         Deletes tags from a [customer managed
         key](https://docs.aws.amazon.com/kms/latest/developerguide/concepts.html#customer-
         cmk)_.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#untag_resource)
         """
+
     async def update_alias(
         self, *, AliasName: str, TargetKeyId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Associates an existing KMS alias with a different KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_alias)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#update_alias)
         """
+
     async def update_custom_key_store(
         self,
         *,
         CustomKeyStoreId: str,
         NewCustomKeyStoreName: str = ...,
         KeyStorePassword: str = ...,
         CloudHsmClusterId: str = ...,
@@ -741,117 +807,132 @@
     ) -> Dict[str, Any]:
         """
         Changes the properties of a custom key store.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_custom_key_store)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#update_custom_key_store)
         """
+
     async def update_key_description(
         self, *, KeyId: str, Description: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Updates the description of a KMS key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_key_description)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#update_key_description)
         """
+
     async def update_primary_region(
         self, *, KeyId: str, PrimaryRegion: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Changes the primary key of a multi-Region key.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.update_primary_region)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#update_primary_region)
         """
+
     async def verify(
         self,
         *,
         KeyId: str,
         Message: BlobTypeDef,
         Signature: BlobTypeDef,
         SigningAlgorithm: SigningAlgorithmSpecType,
         MessageType: MessageTypeType = ...,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> VerifyResponseTypeDef:
         """
         Verifies a digital signature that was generated by the  Sign operation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#verify)
         """
+
     async def verify_mac(
         self,
         *,
         Message: BlobTypeDef,
         KeyId: str,
         MacAlgorithm: MacAlgorithmSpecType,
         Mac: BlobTypeDef,
-        GrantTokens: Sequence[str] = ...
+        GrantTokens: Sequence[str] = ...,
+        DryRun: bool = ...
     ) -> VerifyMacResponseTypeDef:
         """
         Verifies the hash-based message authentication code (HMAC) for a specified
         message, HMAC KMS key, and MAC algorithm.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.verify_mac)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#verify_mac)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_custom_key_stores"]
     ) -> DescribeCustomKeyStoresPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_aliases"]) -> ListAliasesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_grants"]) -> ListGrantsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_key_policies"]
     ) -> ListKeyPoliciesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_keys"]) -> ListKeysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_resource_tags"]
     ) -> ListResourceTagsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_retirable_grants"]
     ) -> ListRetirableGrantsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "KMSClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kms.html#KMS.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kms/client/)
         """
```

### Comparing `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/literals.py` & `types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -201,14 +201,15 @@
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
@@ -304,14 +305,15 @@
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
@@ -390,26 +392,28 @@
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
@@ -579,14 +583,15 @@
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

### Comparing `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/literals.pyi` & `types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -199,14 +199,15 @@
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
@@ -302,14 +303,15 @@
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
@@ -388,26 +390,28 @@
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
@@ -577,14 +581,15 @@
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

### Comparing `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/paginator.py` & `types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/paginator.pyi` & `types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/type_defs.py` & `types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,14 @@
     "EnableKeyRotationRequestRequestTypeDef",
     "GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     "GenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
     "GetKeyPolicyRequestRequestTypeDef",
     "GetKeyRotationStatusRequestRequestTypeDef",
     "GetParametersForImportRequestRequestTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
-    "GrantConstraintsOutputTypeDef",
     "TimestampTypeDef",
     "KeyListEntryTypeDef",
     "XksKeyConfigurationTypeTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListGrantsRequestRequestTypeDef",
     "ListKeyPoliciesRequestRequestTypeDef",
     "ListKeysRequestRequestTypeDef",
@@ -127,37 +126,36 @@
     "ScheduleKeyDeletionResponseTypeDef",
     "SignResponseTypeDef",
     "VerifyMacResponseTypeDef",
     "VerifyResponseTypeDef",
     "CreateCustomKeyStoreRequestRequestTypeDef",
     "UpdateCustomKeyStoreRequestRequestTypeDef",
     "CreateGrantRequestRequestTypeDef",
+    "GrantListEntryTypeDef",
     "CreateKeyRequestRequestTypeDef",
     "ListResourceTagsResponseTypeDef",
     "ReplicateKeyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomKeyStoresListEntryTypeDef",
     "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListGrantsRequestListGrantsPaginateTypeDef",
     "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     "ListKeysRequestListKeysPaginateTypeDef",
     "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
     "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
-    "GrantConstraintsUnionTypeDef",
-    "GrantListEntryTypeDef",
     "ImportKeyMaterialRequestRequestTypeDef",
     "ListKeysResponseTypeDef",
     "MultiRegionConfigurationTypeDef",
     "DecryptRequestRequestTypeDef",
     "GenerateDataKeyPairRequestRequestTypeDef",
     "GenerateDataKeyRequestRequestTypeDef",
     "GenerateRandomRequestRequestTypeDef",
-    "DescribeCustomKeyStoresResponseTypeDef",
     "ListGrantsResponseTypeDef",
+    "DescribeCustomKeyStoresResponseTypeDef",
     "KeyMetadataTypeDef",
     "CreateKeyResponseTypeDef",
     "DescribeKeyResponseTypeDef",
     "ReplicateKeyResponseTypeDef",
 )
 
 AliasListEntryTypeDef = TypedDict(
@@ -349,14 +347,15 @@
     },
 )
 _OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
@@ -374,14 +373,15 @@
 _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "KeySpec": DataKeySpecType,
         "NumberOfBytes": int,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class GenerateDataKeyWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
@@ -431,23 +431,14 @@
 
 class GetPublicKeyRequestRequestTypeDef(
     _RequiredGetPublicKeyRequestRequestTypeDef, _OptionalGetPublicKeyRequestRequestTypeDef
 ):
     pass
 
 
-GrantConstraintsOutputTypeDef = TypedDict(
-    "GrantConstraintsOutputTypeDef",
-    {
-        "EncryptionContextSubset": Dict[str, str],
-        "EncryptionContextEquals": Dict[str, str],
-    },
-    total=False,
-)
-
 TimestampTypeDef = Union[datetime, str]
 KeyListEntryTypeDef = TypedDict(
     "KeyListEntryTypeDef",
     {
         "KeyId": str,
         "KeyArn": str,
     },
@@ -606,25 +597,40 @@
 
 RetireGrantRequestRequestTypeDef = TypedDict(
     "RetireGrantRequestRequestTypeDef",
     {
         "GrantToken": str,
         "KeyId": str,
         "GrantId": str,
+        "DryRun": bool,
     },
     total=False,
 )
 
-RevokeGrantRequestRequestTypeDef = TypedDict(
-    "RevokeGrantRequestRequestTypeDef",
+_RequiredRevokeGrantRequestRequestTypeDef = TypedDict(
+    "_RequiredRevokeGrantRequestRequestTypeDef",
     {
         "KeyId": str,
         "GrantId": str,
     },
 )
+_OptionalRevokeGrantRequestRequestTypeDef = TypedDict(
+    "_OptionalRevokeGrantRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class RevokeGrantRequestRequestTypeDef(
+    _RequiredRevokeGrantRequestRequestTypeDef, _OptionalRevokeGrantRequestRequestTypeDef
+):
+    pass
+
 
 _RequiredScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "_RequiredScheduleKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
@@ -685,14 +691,15 @@
 )
 _OptionalEncryptRequestRequestTypeDef = TypedDict(
     "_OptionalEncryptRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class EncryptRequestRequestTypeDef(
     _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
@@ -708,14 +715,15 @@
         "MacAlgorithm": MacAlgorithmSpecType,
     },
 )
 _OptionalGenerateMacRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateMacRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class GenerateMacRequestRequestTypeDef(
     _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
@@ -735,14 +743,15 @@
     {
         "SourceEncryptionContext": Mapping[str, str],
         "SourceKeyId": str,
         "DestinationEncryptionContext": Mapping[str, str],
         "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class ReEncryptRequestRequestTypeDef(
     _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
@@ -768,14 +777,15 @@
     },
 )
 _OptionalSignRequestRequestTypeDef = TypedDict(
     "_OptionalSignRequestRequestTypeDef",
     {
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class SignRequestRequestTypeDef(
     _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
@@ -792,14 +802,15 @@
         "Mac": BlobTypeDef,
     },
 )
 _OptionalVerifyMacRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyMacRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class VerifyMacRequestRequestTypeDef(
     _RequiredVerifyMacRequestRequestTypeDef, _OptionalVerifyMacRequestRequestTypeDef
@@ -817,14 +828,15 @@
     },
 )
 _OptionalVerifyRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyRequestRequestTypeDef",
     {
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class VerifyRequestRequestTypeDef(
     _RequiredVerifyRequestRequestTypeDef, _OptionalVerifyRequestRequestTypeDef
@@ -1132,25 +1144,42 @@
 _OptionalCreateGrantRequestRequestTypeDef = TypedDict(
     "_OptionalCreateGrantRequestRequestTypeDef",
     {
         "RetiringPrincipal": str,
         "Constraints": GrantConstraintsTypeDef,
         "GrantTokens": Sequence[str],
         "Name": str,
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class CreateGrantRequestRequestTypeDef(
     _RequiredCreateGrantRequestRequestTypeDef, _OptionalCreateGrantRequestRequestTypeDef
 ):
     pass
 
 
+GrantListEntryTypeDef = TypedDict(
+    "GrantListEntryTypeDef",
+    {
+        "KeyId": str,
+        "GrantId": str,
+        "Name": str,
+        "CreationDate": datetime,
+        "GranteePrincipal": str,
+        "RetiringPrincipal": str,
+        "IssuingAccount": str,
+        "Operations": List[GrantOperationType],
+        "Constraints": GrantConstraintsTypeDef,
+    },
+    total=False,
+)
+
 CreateKeyRequestRequestTypeDef = TypedDict(
     "CreateKeyRequestRequestTypeDef",
     {
         "Policy": str,
         "Description": str,
         "KeyUsage": KeyUsageTypeType,
         "CustomerMasterKeySpec": CustomerMasterKeySpecType,
@@ -1337,31 +1366,14 @@
 class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
     _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
 ):
     pass
 
 
-GrantConstraintsUnionTypeDef = Union[GrantConstraintsTypeDef, GrantConstraintsOutputTypeDef]
-GrantListEntryTypeDef = TypedDict(
-    "GrantListEntryTypeDef",
-    {
-        "KeyId": str,
-        "GrantId": str,
-        "Name": str,
-        "CreationDate": datetime,
-        "GranteePrincipal": str,
-        "RetiringPrincipal": str,
-        "IssuingAccount": str,
-        "Operations": List[GrantOperationType],
-        "Constraints": GrantConstraintsOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredImportKeyMaterialRequestRequestTypeDef = TypedDict(
     "_RequiredImportKeyMaterialRequestRequestTypeDef",
     {
         "KeyId": str,
         "ImportToken": BlobTypeDef,
         "EncryptedKeyMaterial": BlobTypeDef,
     },
@@ -1412,14 +1424,15 @@
     "_OptionalDecryptRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "KeyId": str,
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class DecryptRequestRequestTypeDef(
     _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
@@ -1436,14 +1449,15 @@
 )
 _OptionalGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataKeyPairRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class GenerateDataKeyPairRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairRequestRequestTypeDef,
@@ -1462,14 +1476,15 @@
     "_OptionalGenerateDataKeyRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "NumberOfBytes": int,
         "KeySpec": DataKeySpecType,
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
     },
     total=False,
 )
 
 
 class GenerateDataKeyRequestRequestTypeDef(
     _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
@@ -1483,28 +1498,28 @@
         "NumberOfBytes": int,
         "CustomKeyStoreId": str,
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
-DescribeCustomKeyStoresResponseTypeDef = TypedDict(
-    "DescribeCustomKeyStoresResponseTypeDef",
+ListGrantsResponseTypeDef = TypedDict(
+    "ListGrantsResponseTypeDef",
     {
-        "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
+        "Grants": List[GrantListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListGrantsResponseTypeDef = TypedDict(
-    "ListGrantsResponseTypeDef",
+DescribeCustomKeyStoresResponseTypeDef = TypedDict(
+    "DescribeCustomKeyStoresResponseTypeDef",
     {
-        "Grants": List[GrantListEntryTypeDef],
+        "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredKeyMetadataTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms/type_defs.pyi` & `types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
     "EnableKeyRotationRequestRequestTypeDef",
     "GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     "GenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
     "GetKeyPolicyRequestRequestTypeDef",
     "GetKeyRotationStatusRequestRequestTypeDef",
     "GetParametersForImportRequestRequestTypeDef",
     "GetPublicKeyRequestRequestTypeDef",
-    "GrantConstraintsOutputTypeDef",
     "TimestampTypeDef",
     "KeyListEntryTypeDef",
     "XksKeyConfigurationTypeTypeDef",
     "ListAliasesRequestRequestTypeDef",
     "ListGrantsRequestRequestTypeDef",
     "ListKeyPoliciesRequestRequestTypeDef",
     "ListKeysRequestRequestTypeDef",
@@ -126,37 +125,36 @@
     "ScheduleKeyDeletionResponseTypeDef",
     "SignResponseTypeDef",
     "VerifyMacResponseTypeDef",
     "VerifyResponseTypeDef",
     "CreateCustomKeyStoreRequestRequestTypeDef",
     "UpdateCustomKeyStoreRequestRequestTypeDef",
     "CreateGrantRequestRequestTypeDef",
+    "GrantListEntryTypeDef",
     "CreateKeyRequestRequestTypeDef",
     "ListResourceTagsResponseTypeDef",
     "ReplicateKeyRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CustomKeyStoresListEntryTypeDef",
     "DescribeCustomKeyStoresRequestDescribeCustomKeyStoresPaginateTypeDef",
     "ListAliasesRequestListAliasesPaginateTypeDef",
     "ListGrantsRequestListGrantsPaginateTypeDef",
     "ListKeyPoliciesRequestListKeyPoliciesPaginateTypeDef",
     "ListKeysRequestListKeysPaginateTypeDef",
     "ListResourceTagsRequestListResourceTagsPaginateTypeDef",
     "ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef",
-    "GrantConstraintsUnionTypeDef",
-    "GrantListEntryTypeDef",
     "ImportKeyMaterialRequestRequestTypeDef",
     "ListKeysResponseTypeDef",
     "MultiRegionConfigurationTypeDef",
     "DecryptRequestRequestTypeDef",
     "GenerateDataKeyPairRequestRequestTypeDef",
     "GenerateDataKeyRequestRequestTypeDef",
     "GenerateRandomRequestRequestTypeDef",
-    "DescribeCustomKeyStoresResponseTypeDef",
     "ListGrantsResponseTypeDef",
+    "DescribeCustomKeyStoresResponseTypeDef",
     "KeyMetadataTypeDef",
     "CreateKeyResponseTypeDef",
     "DescribeKeyResponseTypeDef",
     "ReplicateKeyResponseTypeDef",
 )
 
 AliasListEntryTypeDef = TypedDict(
@@ -346,14 +344,15 @@
     },
 )
 _OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class GenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairWithoutPlaintextRequestRequestTypeDef,
@@ -369,14 +368,15 @@
 _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "KeySpec": DataKeySpecType,
         "NumberOfBytes": int,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class GenerateDataKeyWithoutPlaintextRequestRequestTypeDef(
     _RequiredGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
     _OptionalGenerateDataKeyWithoutPlaintextRequestRequestTypeDef,
@@ -422,23 +422,14 @@
 )
 
 class GetPublicKeyRequestRequestTypeDef(
     _RequiredGetPublicKeyRequestRequestTypeDef, _OptionalGetPublicKeyRequestRequestTypeDef
 ):
     pass
 
-GrantConstraintsOutputTypeDef = TypedDict(
-    "GrantConstraintsOutputTypeDef",
-    {
-        "EncryptionContextSubset": Dict[str, str],
-        "EncryptionContextEquals": Dict[str, str],
-    },
-    total=False,
-)
-
 TimestampTypeDef = Union[datetime, str]
 KeyListEntryTypeDef = TypedDict(
     "KeyListEntryTypeDef",
     {
         "KeyId": str,
         "KeyArn": str,
     },
@@ -587,25 +578,38 @@
 
 RetireGrantRequestRequestTypeDef = TypedDict(
     "RetireGrantRequestRequestTypeDef",
     {
         "GrantToken": str,
         "KeyId": str,
         "GrantId": str,
+        "DryRun": bool,
     },
     total=False,
 )
 
-RevokeGrantRequestRequestTypeDef = TypedDict(
-    "RevokeGrantRequestRequestTypeDef",
+_RequiredRevokeGrantRequestRequestTypeDef = TypedDict(
+    "_RequiredRevokeGrantRequestRequestTypeDef",
     {
         "KeyId": str,
         "GrantId": str,
     },
 )
+_OptionalRevokeGrantRequestRequestTypeDef = TypedDict(
+    "_OptionalRevokeGrantRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class RevokeGrantRequestRequestTypeDef(
+    _RequiredRevokeGrantRequestRequestTypeDef, _OptionalRevokeGrantRequestRequestTypeDef
+):
+    pass
 
 _RequiredScheduleKeyDeletionRequestRequestTypeDef = TypedDict(
     "_RequiredScheduleKeyDeletionRequestRequestTypeDef",
     {
         "KeyId": str,
     },
 )
@@ -664,14 +668,15 @@
 )
 _OptionalEncryptRequestRequestTypeDef = TypedDict(
     "_OptionalEncryptRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
+        "DryRun": bool,
     },
     total=False,
 )
 
 class EncryptRequestRequestTypeDef(
     _RequiredEncryptRequestRequestTypeDef, _OptionalEncryptRequestRequestTypeDef
 ):
@@ -685,14 +690,15 @@
         "MacAlgorithm": MacAlgorithmSpecType,
     },
 )
 _OptionalGenerateMacRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateMacRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class GenerateMacRequestRequestTypeDef(
     _RequiredGenerateMacRequestRequestTypeDef, _OptionalGenerateMacRequestRequestTypeDef
 ):
@@ -710,14 +716,15 @@
     {
         "SourceEncryptionContext": Mapping[str, str],
         "SourceKeyId": str,
         "DestinationEncryptionContext": Mapping[str, str],
         "SourceEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "DestinationEncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class ReEncryptRequestRequestTypeDef(
     _RequiredReEncryptRequestRequestTypeDef, _OptionalReEncryptRequestRequestTypeDef
 ):
@@ -741,14 +748,15 @@
     },
 )
 _OptionalSignRequestRequestTypeDef = TypedDict(
     "_OptionalSignRequestRequestTypeDef",
     {
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class SignRequestRequestTypeDef(
     _RequiredSignRequestRequestTypeDef, _OptionalSignRequestRequestTypeDef
 ):
@@ -763,14 +771,15 @@
         "Mac": BlobTypeDef,
     },
 )
 _OptionalVerifyMacRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyMacRequestRequestTypeDef",
     {
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class VerifyMacRequestRequestTypeDef(
     _RequiredVerifyMacRequestRequestTypeDef, _OptionalVerifyMacRequestRequestTypeDef
 ):
@@ -786,14 +795,15 @@
     },
 )
 _OptionalVerifyRequestRequestTypeDef = TypedDict(
     "_OptionalVerifyRequestRequestTypeDef",
     {
         "MessageType": MessageTypeType,
         "GrantTokens": Sequence[str],
+        "DryRun": bool,
     },
     total=False,
 )
 
 class VerifyRequestRequestTypeDef(
     _RequiredVerifyRequestRequestTypeDef, _OptionalVerifyRequestRequestTypeDef
 ):
@@ -1095,23 +1105,40 @@
 _OptionalCreateGrantRequestRequestTypeDef = TypedDict(
     "_OptionalCreateGrantRequestRequestTypeDef",
     {
         "RetiringPrincipal": str,
         "Constraints": GrantConstraintsTypeDef,
         "GrantTokens": Sequence[str],
         "Name": str,
+        "DryRun": bool,
     },
     total=False,
 )
 
 class CreateGrantRequestRequestTypeDef(
     _RequiredCreateGrantRequestRequestTypeDef, _OptionalCreateGrantRequestRequestTypeDef
 ):
     pass
 
+GrantListEntryTypeDef = TypedDict(
+    "GrantListEntryTypeDef",
+    {
+        "KeyId": str,
+        "GrantId": str,
+        "Name": str,
+        "CreationDate": datetime,
+        "GranteePrincipal": str,
+        "RetiringPrincipal": str,
+        "IssuingAccount": str,
+        "Operations": List[GrantOperationType],
+        "Constraints": GrantConstraintsTypeDef,
+    },
+    total=False,
+)
+
 CreateKeyRequestRequestTypeDef = TypedDict(
     "CreateKeyRequestRequestTypeDef",
     {
         "Policy": str,
         "Description": str,
         "KeyUsage": KeyUsageTypeType,
         "CustomerMasterKeySpec": CustomerMasterKeySpecType,
@@ -1288,31 +1315,14 @@
 
 class ListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef(
     _RequiredListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
     _OptionalListRetirableGrantsRequestListRetirableGrantsPaginateTypeDef,
 ):
     pass
 
-GrantConstraintsUnionTypeDef = Union[GrantConstraintsTypeDef, GrantConstraintsOutputTypeDef]
-GrantListEntryTypeDef = TypedDict(
-    "GrantListEntryTypeDef",
-    {
-        "KeyId": str,
-        "GrantId": str,
-        "Name": str,
-        "CreationDate": datetime,
-        "GranteePrincipal": str,
-        "RetiringPrincipal": str,
-        "IssuingAccount": str,
-        "Operations": List[GrantOperationType],
-        "Constraints": GrantConstraintsOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredImportKeyMaterialRequestRequestTypeDef = TypedDict(
     "_RequiredImportKeyMaterialRequestRequestTypeDef",
     {
         "KeyId": str,
         "ImportToken": BlobTypeDef,
         "EncryptedKeyMaterial": BlobTypeDef,
     },
@@ -1361,14 +1371,15 @@
     "_OptionalDecryptRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "KeyId": str,
         "EncryptionAlgorithm": EncryptionAlgorithmSpecType,
         "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
     },
     total=False,
 )
 
 class DecryptRequestRequestTypeDef(
     _RequiredDecryptRequestRequestTypeDef, _OptionalDecryptRequestRequestTypeDef
 ):
@@ -1383,14 +1394,15 @@
 )
 _OptionalGenerateDataKeyPairRequestRequestTypeDef = TypedDict(
     "_OptionalGenerateDataKeyPairRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
     },
     total=False,
 )
 
 class GenerateDataKeyPairRequestRequestTypeDef(
     _RequiredGenerateDataKeyPairRequestRequestTypeDef,
     _OptionalGenerateDataKeyPairRequestRequestTypeDef,
@@ -1407,14 +1419,15 @@
     "_OptionalGenerateDataKeyRequestRequestTypeDef",
     {
         "EncryptionContext": Mapping[str, str],
         "NumberOfBytes": int,
         "KeySpec": DataKeySpecType,
         "GrantTokens": Sequence[str],
         "Recipient": RecipientInfoTypeDef,
+        "DryRun": bool,
     },
     total=False,
 )
 
 class GenerateDataKeyRequestRequestTypeDef(
     _RequiredGenerateDataKeyRequestRequestTypeDef, _OptionalGenerateDataKeyRequestRequestTypeDef
 ):
@@ -1426,28 +1439,28 @@
         "NumberOfBytes": int,
         "CustomKeyStoreId": str,
         "Recipient": RecipientInfoTypeDef,
     },
     total=False,
 )
 
-DescribeCustomKeyStoresResponseTypeDef = TypedDict(
-    "DescribeCustomKeyStoresResponseTypeDef",
+ListGrantsResponseTypeDef = TypedDict(
+    "ListGrantsResponseTypeDef",
     {
-        "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
+        "Grants": List[GrantListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListGrantsResponseTypeDef = TypedDict(
-    "ListGrantsResponseTypeDef",
+DescribeCustomKeyStoresResponseTypeDef = TypedDict(
+    "DescribeCustomKeyStoresResponseTypeDef",
     {
-        "Grants": List[GrantListEntryTypeDef],
+        "CustomKeyStores": List[CustomKeyStoresListEntryTypeDef],
         "NextMarker": str,
         "Truncated": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredKeyMetadataTypeDef = TypedDict(
```

### Comparing `types-aiobotocore-kms-2.5.2.post1/types_aiobotocore_kms.egg-info/SOURCES.txt` & `types-aiobotocore-kms-2.5.2.post2/types_aiobotocore_kms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

