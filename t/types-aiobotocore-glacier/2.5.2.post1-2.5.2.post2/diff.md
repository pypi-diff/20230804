# Comparing `tmp/types-aiobotocore-glacier-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-glacier-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-glacier-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-glacier-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:56 2023, max compression
```

## Comparing `types-aiobotocore-glacier-2.5.2.post1.tar` & `types-aiobotocore-glacier-2.5.2.post2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:20.633579 types-aiobotocore-glacier-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:15.000000 types-aiobotocore-glacier-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-08-02 14:52:20.633579 types-aiobotocore-glacier-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19083 2023-08-02 14:39:15.000000 types-aiobotocore-glacier-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:20.633579 types-aiobotocore-glacier-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:39:15.000000 types-aiobotocore-glacier-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:20.629579 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-02 14:39:15.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-08-02 14:39:15.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:39:15.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28415 2023-08-02 14:39:16.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    28367 2023-08-02 14:39:15.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-08-02 14:39:17.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-08-02 14:39:17.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-08-02 14:39:17.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-08-02 14:39:17.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:15.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42723 2023-08-02 14:39:17.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    42605 2023-08-02 14:39:17.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39668 2023-08-02 14:39:18.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    39596 2023-08-02 14:39:17.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:15.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-02 14:39:17.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-02 14:39:17.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:20.633579 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-08-02 14:52:20.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:52:20.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:20.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:20.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:20.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:52:20.000000 types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:56.380288 types-aiobotocore-glacier-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:46.000000 types-aiobotocore-glacier-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-08-04 12:00:56.380288 types-aiobotocore-glacier-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-08-04 11:46:46.000000 types-aiobotocore-glacier-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:56.380288 types-aiobotocore-glacier-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-04 11:46:46.000000 types-aiobotocore-glacier-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:56.380288 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-04 11:46:46.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-08-04 11:46:46.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-04 11:46:46.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28395 2023-08-04 11:46:46.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28347 2023-08-04 11:46:46.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-08-04 11:46:47.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9645 2023-08-04 11:46:47.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-08-04 11:46:47.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-08-04 11:46:47.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:46.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42777 2023-08-04 11:46:47.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42659 2023-08-04 11:46:47.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    38711 2023-08-04 11:46:49.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38639 2023-08-04 11:46:49.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:46.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-08-04 11:46:47.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-04 11:46:47.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:56.380288 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16428 2023-08-04 12:00:56.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-04 12:00:56.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:56.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:56.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:56.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:00:56.000000 types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-glacier-2.5.2.post1/LICENSE` & `types-aiobotocore-glacier-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post1/setup.py` & `types-aiobotocore-glacier-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-glacier",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_glacier"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Glacier 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/__init__.py` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/__init__.pyi` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/__main__.py` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Glacier 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Glacier 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier\nOther"
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

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/client.py` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     ListPartsPaginator,
     ListVaultsPaginator,
 )
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
     BlobTypeDef,
     CreateVaultOutputTypeDef,
-    DataRetrievalPolicyUnionTypeDef,
+    DataRetrievalPolicyTypeDef,
     DescribeVaultResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
     GetVaultLockOutputTypeDef,
     GetVaultNotificationsOutputTypeDef,
@@ -49,15 +49,15 @@
     ListProvisionedCapacityOutputTypeDef,
     ListTagsForVaultOutputTypeDef,
     ListVaultsOutputTypeDef,
     PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
     VaultAccessPolicyTypeDef,
     VaultLockPolicyTypeDef,
-    VaultNotificationConfigUnionTypeDef,
+    VaultNotificationConfigTypeDef,
 )
 from .waiter import VaultExistsWaiter, VaultNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -457,15 +457,15 @@
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.remove_tags_from_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/client/#remove_tags_from_vault)
         """
 
     async def set_data_retrieval_policy(
-        self, *, accountId: str = "-", Policy: DataRetrievalPolicyUnionTypeDef = ...
+        self, *, accountId: str = "-", Policy: DataRetrievalPolicyTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation sets and then enacts a data retrieval policy in the region
         specified in the PUT request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_data_retrieval_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/client/#set_data_retrieval_policy)
@@ -483,15 +483,15 @@
         """
 
     async def set_vault_notifications(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
-        vaultNotificationConfig: VaultNotificationConfigUnionTypeDef = ...
+        vaultNotificationConfig: VaultNotificationConfigTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation configures notifications that will be sent when specific events
         happen to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_vault_notifications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/client/#set_vault_notifications)
```

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/client.pyi` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     ListPartsPaginator,
     ListVaultsPaginator,
 )
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
     BlobTypeDef,
     CreateVaultOutputTypeDef,
-    DataRetrievalPolicyUnionTypeDef,
+    DataRetrievalPolicyTypeDef,
     DescribeVaultResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDataRetrievalPolicyOutputTypeDef,
     GetJobOutputOutputTypeDef,
     GetVaultAccessPolicyOutputTypeDef,
     GetVaultLockOutputTypeDef,
     GetVaultNotificationsOutputTypeDef,
@@ -49,15 +49,15 @@
     ListProvisionedCapacityOutputTypeDef,
     ListTagsForVaultOutputTypeDef,
     ListVaultsOutputTypeDef,
     PurchaseProvisionedCapacityOutputTypeDef,
     UploadMultipartPartOutputTypeDef,
     VaultAccessPolicyTypeDef,
     VaultLockPolicyTypeDef,
-    VaultNotificationConfigUnionTypeDef,
+    VaultNotificationConfigTypeDef,
 )
 from .waiter import VaultExistsWaiter, VaultNotExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -421,15 +421,15 @@
         This operation removes one or more tags from the set of tags attached to a
         vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.remove_tags_from_vault)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/client/#remove_tags_from_vault)
         """
     async def set_data_retrieval_policy(
-        self, *, accountId: str = "-", Policy: DataRetrievalPolicyUnionTypeDef = ...
+        self, *, accountId: str = "-", Policy: DataRetrievalPolicyTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation sets and then enacts a data retrieval policy in the region
         specified in the PUT request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_data_retrieval_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/client/#set_data_retrieval_policy)
@@ -445,15 +445,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/client/#set_vault_access_policy)
         """
     async def set_vault_notifications(
         self,
         *,
         vaultName: str,
         accountId: str = "-",
-        vaultNotificationConfig: VaultNotificationConfigUnionTypeDef = ...
+        vaultNotificationConfig: VaultNotificationConfigTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         This operation configures notifications that will be sent when specific events
         happen to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Client.set_vault_notifications)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/client/#set_vault_notifications)
```

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/literals.py` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/literals.pyi` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/paginator.py` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/paginator.pyi` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/service_resource.py` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/service_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
     BlobTypeDef,
     CreateVaultOutputTypeDef,
     GetJobOutputOutputTypeDef,
     InventoryRetrievalJobDescriptionResponseTypeDef,
     ListPartsOutputTypeDef,
-    OutputLocationTypeDef,
+    OutputLocationResponseTypeDef,
     SelectParametersResponseTypeDef,
     UploadMultipartPartOutputTypeDef,
-    VaultNotificationConfigTypeDef,
+    VaultNotificationConfigNotificationTypeDef,
 )
 
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOBoto3ServiceResource
 try:
@@ -473,15 +473,15 @@
     sha256_tree_hash: Awaitable[str]
     archive_sha256_tree_hash: Awaitable[str]
     retrieval_byte_range: Awaitable[str]
     tier: Awaitable[str]
     inventory_retrieval_parameters: Awaitable[InventoryRetrievalJobDescriptionResponseTypeDef]
     job_output_path: Awaitable[str]
     select_parameters: Awaitable[SelectParametersResponseTypeDef]
-    output_location: Awaitable[OutputLocationTypeDef]
+    output_location: Awaitable[OutputLocationResponseTypeDef]
     account_id: str
     vault_name: str
     id: str
 
     async def Vault(self) -> "_Vault":
         """
         Creates a Vault resource.
@@ -651,15 +651,17 @@
         Calls :py:meth:`Glacier.Client.get_vault_notifications` to update the attributes
         of the Notification resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Notification.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#notificationreload-method)
         """
 
-    async def set(self, *, vaultNotificationConfig: VaultNotificationConfigTypeDef = ...) -> None:
+    async def set(
+        self, *, vaultNotificationConfig: VaultNotificationConfigNotificationTypeDef = ...
+    ) -> None:
         """
         This operation configures notifications that will be sent when specific events
         happen to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Notification.set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#notificationset-method)
         """
```

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/service_resource.pyi` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -30,18 +30,18 @@
 from .type_defs import (
     ArchiveCreationOutputTypeDef,
     BlobTypeDef,
     CreateVaultOutputTypeDef,
     GetJobOutputOutputTypeDef,
     InventoryRetrievalJobDescriptionResponseTypeDef,
     ListPartsOutputTypeDef,
-    OutputLocationTypeDef,
+    OutputLocationResponseTypeDef,
     SelectParametersResponseTypeDef,
     UploadMultipartPartOutputTypeDef,
-    VaultNotificationConfigTypeDef,
+    VaultNotificationConfigNotificationTypeDef,
 )
 
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOBoto3ServiceResource
 try:
@@ -441,15 +441,15 @@
     sha256_tree_hash: Awaitable[str]
     archive_sha256_tree_hash: Awaitable[str]
     retrieval_byte_range: Awaitable[str]
     tier: Awaitable[str]
     inventory_retrieval_parameters: Awaitable[InventoryRetrievalJobDescriptionResponseTypeDef]
     job_output_path: Awaitable[str]
     select_parameters: Awaitable[SelectParametersResponseTypeDef]
-    output_location: Awaitable[OutputLocationTypeDef]
+    output_location: Awaitable[OutputLocationResponseTypeDef]
     account_id: str
     vault_name: str
     id: str
 
     async def Vault(self) -> "_Vault":
         """
         Creates a Vault resource.
@@ -601,15 +601,17 @@
         """
         Calls :py:meth:`Glacier.Client.get_vault_notifications` to update the attributes
         of the Notification resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Notification.reload)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#notificationreload-method)
         """
-    async def set(self, *, vaultNotificationConfig: VaultNotificationConfigTypeDef = ...) -> None:
+    async def set(
+        self, *, vaultNotificationConfig: VaultNotificationConfigNotificationTypeDef = ...
+    ) -> None:
         """
         This operation configures notifications that will be sent when specific events
         happen to a vault.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/glacier.html#Glacier.Notification.set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_glacier/service_resource/#notificationset-method)
         """
```

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/type_defs.py` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     "GetDataRetrievalPolicyInputRequestTypeDef",
     "GetJobOutputInputJobGetOutputTypeDef",
     "GetJobOutputInputRequestTypeDef",
     "GetVaultAccessPolicyInputRequestTypeDef",
     "VaultAccessPolicyTypeDef",
     "GetVaultLockInputRequestTypeDef",
     "GetVaultNotificationsInputRequestTypeDef",
-    "VaultNotificationConfigOutputTypeDef",
+    "VaultNotificationConfigTypeDef",
     "InventoryRetrievalJobDescriptionTypeDef",
     "GranteeTypeDef",
     "InitiateMultipartUploadInputRequestTypeDef",
     "InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef",
     "VaultLockPolicyTypeDef",
     "InventoryRetrievalJobInputTypeDef",
     "PaginatorConfigTypeDef",
@@ -85,15 +85,15 @@
     "PartListElementTypeDef",
     "ListProvisionedCapacityInputRequestTypeDef",
     "ProvisionedCapacityDescriptionTypeDef",
     "ListTagsForVaultInputRequestTypeDef",
     "ListVaultsInputRequestTypeDef",
     "PurchaseProvisionedCapacityInputRequestTypeDef",
     "RemoveTagsFromVaultInputRequestTypeDef",
-    "VaultNotificationConfigTypeDef",
+    "VaultNotificationConfigNotificationTypeDef",
     "ArchiveCreationOutputTypeDef",
     "CreateVaultOutputTypeDef",
     "DescribeVaultResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetJobOutputOutputTypeDef",
     "GetVaultLockOutputTypeDef",
     "InitiateJobOutputTypeDef",
@@ -105,42 +105,38 @@
     "UploadMultipartPartOutputTypeDef",
     "UploadArchiveInputRequestTypeDef",
     "UploadArchiveInputVaultUploadArchiveTypeDef",
     "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
     "UploadMultipartPartInputRequestTypeDef",
     "InputSerializationTypeDef",
     "OutputSerializationTypeDef",
-    "DataRetrievalPolicyOutputTypeDef",
     "DataRetrievalPolicyTypeDef",
     "DescribeVaultInputVaultExistsWaitTypeDef",
     "DescribeVaultInputVaultNotExistsWaitTypeDef",
     "ListVaultsOutputTypeDef",
     "GetVaultAccessPolicyOutputTypeDef",
     "SetVaultAccessPolicyInputRequestTypeDef",
     "GetVaultNotificationsOutputTypeDef",
+    "SetVaultNotificationsInputRequestTypeDef",
     "GrantTypeDef",
     "InitiateVaultLockInputRequestTypeDef",
     "ListJobsInputListJobsPaginateTypeDef",
     "ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
     "ListPartsInputListPartsPaginateTypeDef",
     "ListVaultsInputListVaultsPaginateTypeDef",
     "ListMultipartUploadsOutputTypeDef",
     "ListPartsOutputTypeDef",
     "ListProvisionedCapacityOutputTypeDef",
     "SetVaultNotificationsInputNotificationSetTypeDef",
-    "SetVaultNotificationsInputRequestTypeDef",
-    "VaultNotificationConfigUnionTypeDef",
     "SelectParametersResponseTypeDef",
     "SelectParametersTypeDef",
     "GetDataRetrievalPolicyOutputTypeDef",
-    "DataRetrievalPolicyUnionTypeDef",
     "SetDataRetrievalPolicyInputRequestTypeDef",
-    "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
-    "OutputLocationOutputTypeDef",
+    "OutputLocationResponseTypeDef",
     "OutputLocationTypeDef",
     "GlacierJobDescriptionResponseTypeDef",
     "GlacierJobDescriptionTypeDef",
     "JobParametersTypeDef",
     "ListJobsOutputTypeDef",
     "InitiateJobInputRequestTypeDef",
 )
@@ -633,16 +629,16 @@
 class GetVaultNotificationsInputRequestTypeDef(
     _RequiredGetVaultNotificationsInputRequestTypeDef,
     _OptionalGetVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
 
-VaultNotificationConfigOutputTypeDef = TypedDict(
-    "VaultNotificationConfigOutputTypeDef",
+VaultNotificationConfigTypeDef = TypedDict(
+    "VaultNotificationConfigTypeDef",
     {
         "SNSTopic": str,
         "Events": List[str],
     },
     total=False,
 )
 
@@ -920,16 +916,16 @@
 
 class RemoveTagsFromVaultInputRequestTypeDef(
     _RequiredRemoveTagsFromVaultInputRequestTypeDef, _OptionalRemoveTagsFromVaultInputRequestTypeDef
 ):
     pass
 
 
-VaultNotificationConfigTypeDef = TypedDict(
-    "VaultNotificationConfigTypeDef",
+VaultNotificationConfigNotificationTypeDef = TypedDict(
+    "VaultNotificationConfigNotificationTypeDef",
     {
         "SNSTopic": str,
         "Events": Sequence[str],
     },
     total=False,
 )
 
@@ -1140,26 +1136,18 @@
     "OutputSerializationTypeDef",
     {
         "csv": CSVOutputTypeDef,
     },
     total=False,
 )
 
-DataRetrievalPolicyOutputTypeDef = TypedDict(
-    "DataRetrievalPolicyOutputTypeDef",
-    {
-        "Rules": List[DataRetrievalRuleTypeDef],
-    },
-    total=False,
-)
-
 DataRetrievalPolicyTypeDef = TypedDict(
     "DataRetrievalPolicyTypeDef",
     {
-        "Rules": Sequence[DataRetrievalRuleTypeDef],
+        "Rules": List[DataRetrievalRuleTypeDef],
     },
     total=False,
 )
 
 _RequiredDescribeVaultInputVaultExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeVaultInputVaultExistsWaitTypeDef",
     {
@@ -1245,19 +1233,42 @@
 ):
     pass
 
 
 GetVaultNotificationsOutputTypeDef = TypedDict(
     "GetVaultNotificationsOutputTypeDef",
     {
-        "vaultNotificationConfig": VaultNotificationConfigOutputTypeDef,
+        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredSetVaultNotificationsInputRequestTypeDef = TypedDict(
+    "_RequiredSetVaultNotificationsInputRequestTypeDef",
+    {
+        "vaultName": str,
+    },
+)
+_OptionalSetVaultNotificationsInputRequestTypeDef = TypedDict(
+    "_OptionalSetVaultNotificationsInputRequestTypeDef",
+    {
+        "accountId": str,
+        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SetVaultNotificationsInputRequestTypeDef(
+    _RequiredSetVaultNotificationsInputRequestTypeDef,
+    _OptionalSetVaultNotificationsInputRequestTypeDef,
+):
+    pass
+
+
 GrantTypeDef = TypedDict(
     "GrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": PermissionType,
     },
     total=False,
@@ -1407,45 +1418,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetVaultNotificationsInputNotificationSetTypeDef = TypedDict(
     "SetVaultNotificationsInputNotificationSetTypeDef",
     {
-        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredSetVaultNotificationsInputRequestTypeDef = TypedDict(
-    "_RequiredSetVaultNotificationsInputRequestTypeDef",
-    {
-        "vaultName": str,
-    },
-)
-_OptionalSetVaultNotificationsInputRequestTypeDef = TypedDict(
-    "_OptionalSetVaultNotificationsInputRequestTypeDef",
-    {
-        "accountId": str,
-        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
+        "vaultNotificationConfig": VaultNotificationConfigNotificationTypeDef,
     },
     total=False,
 )
 
-
-class SetVaultNotificationsInputRequestTypeDef(
-    _RequiredSetVaultNotificationsInputRequestTypeDef,
-    _OptionalSetVaultNotificationsInputRequestTypeDef,
-):
-    pass
-
-
-VaultNotificationConfigUnionTypeDef = Union[
-    VaultNotificationConfigTypeDef, VaultNotificationConfigOutputTypeDef
-]
 SelectParametersResponseTypeDef = TypedDict(
     "SelectParametersResponseTypeDef",
     {
         "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
@@ -1463,75 +1448,57 @@
     },
     total=False,
 )
 
 GetDataRetrievalPolicyOutputTypeDef = TypedDict(
     "GetDataRetrievalPolicyOutputTypeDef",
     {
-        "Policy": DataRetrievalPolicyOutputTypeDef,
+        "Policy": DataRetrievalPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataRetrievalPolicyUnionTypeDef = Union[
-    DataRetrievalPolicyTypeDef, DataRetrievalPolicyOutputTypeDef
-]
 SetDataRetrievalPolicyInputRequestTypeDef = TypedDict(
     "SetDataRetrievalPolicyInputRequestTypeDef",
     {
         "accountId": str,
         "Policy": DataRetrievalPolicyTypeDef,
     },
     total=False,
 )
 
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
         "BucketName": str,
         "Prefix": str,
         "Encryption": EncryptionTypeDef,
         "CannedACL": CannedACLType,
         "AccessControlList": List[GrantTypeDef],
         "Tagging": Dict[str, str],
         "UserMetadata": Dict[str, str],
         "StorageClass": StorageClassType,
     },
     total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
-    {
-        "BucketName": str,
-        "Prefix": str,
-        "Encryption": EncryptionTypeDef,
-        "CannedACL": CannedACLType,
-        "AccessControlList": Sequence[GrantTypeDef],
-        "Tagging": Mapping[str, str],
-        "UserMetadata": Mapping[str, str],
-        "StorageClass": StorageClassType,
-    },
-    total=False,
-)
-
-OutputLocationOutputTypeDef = TypedDict(
-    "OutputLocationOutputTypeDef",
+OutputLocationResponseTypeDef = TypedDict(
+    "OutputLocationResponseTypeDef",
     {
-        "S3": S3LocationOutputTypeDef,
+        "S3": S3LocationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 OutputLocationTypeDef = TypedDict(
     "OutputLocationTypeDef",
     {
-        "S3": S3LocationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "S3": S3LocationTypeDef,
     },
+    total=False,
 )
 
 GlacierJobDescriptionResponseTypeDef = TypedDict(
     "GlacierJobDescriptionResponseTypeDef",
     {
         "JobId": str,
         "JobDescription": str,
@@ -1549,15 +1516,15 @@
         "SHA256TreeHash": str,
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
         "SelectParameters": SelectParametersTypeDef,
-        "OutputLocation": OutputLocationOutputTypeDef,
+        "OutputLocation": OutputLocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlacierJobDescriptionTypeDef = TypedDict(
     "GlacierJobDescriptionTypeDef",
     {
@@ -1577,15 +1544,15 @@
         "SHA256TreeHash": str,
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
         "SelectParameters": SelectParametersTypeDef,
-        "OutputLocation": OutputLocationOutputTypeDef,
+        "OutputLocation": OutputLocationTypeDef,
     },
     total=False,
 )
 
 JobParametersTypeDef = TypedDict(
     "JobParametersTypeDef",
     {
```

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/type_defs.pyi` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     "GetDataRetrievalPolicyInputRequestTypeDef",
     "GetJobOutputInputJobGetOutputTypeDef",
     "GetJobOutputInputRequestTypeDef",
     "GetVaultAccessPolicyInputRequestTypeDef",
     "VaultAccessPolicyTypeDef",
     "GetVaultLockInputRequestTypeDef",
     "GetVaultNotificationsInputRequestTypeDef",
-    "VaultNotificationConfigOutputTypeDef",
+    "VaultNotificationConfigTypeDef",
     "InventoryRetrievalJobDescriptionTypeDef",
     "GranteeTypeDef",
     "InitiateMultipartUploadInputRequestTypeDef",
     "InitiateMultipartUploadInputVaultInitiateMultipartUploadTypeDef",
     "VaultLockPolicyTypeDef",
     "InventoryRetrievalJobInputTypeDef",
     "PaginatorConfigTypeDef",
@@ -84,15 +84,15 @@
     "PartListElementTypeDef",
     "ListProvisionedCapacityInputRequestTypeDef",
     "ProvisionedCapacityDescriptionTypeDef",
     "ListTagsForVaultInputRequestTypeDef",
     "ListVaultsInputRequestTypeDef",
     "PurchaseProvisionedCapacityInputRequestTypeDef",
     "RemoveTagsFromVaultInputRequestTypeDef",
-    "VaultNotificationConfigTypeDef",
+    "VaultNotificationConfigNotificationTypeDef",
     "ArchiveCreationOutputTypeDef",
     "CreateVaultOutputTypeDef",
     "DescribeVaultResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetJobOutputOutputTypeDef",
     "GetVaultLockOutputTypeDef",
     "InitiateJobOutputTypeDef",
@@ -104,42 +104,38 @@
     "UploadMultipartPartOutputTypeDef",
     "UploadArchiveInputRequestTypeDef",
     "UploadArchiveInputVaultUploadArchiveTypeDef",
     "UploadMultipartPartInputMultipartUploadUploadPartTypeDef",
     "UploadMultipartPartInputRequestTypeDef",
     "InputSerializationTypeDef",
     "OutputSerializationTypeDef",
-    "DataRetrievalPolicyOutputTypeDef",
     "DataRetrievalPolicyTypeDef",
     "DescribeVaultInputVaultExistsWaitTypeDef",
     "DescribeVaultInputVaultNotExistsWaitTypeDef",
     "ListVaultsOutputTypeDef",
     "GetVaultAccessPolicyOutputTypeDef",
     "SetVaultAccessPolicyInputRequestTypeDef",
     "GetVaultNotificationsOutputTypeDef",
+    "SetVaultNotificationsInputRequestTypeDef",
     "GrantTypeDef",
     "InitiateVaultLockInputRequestTypeDef",
     "ListJobsInputListJobsPaginateTypeDef",
     "ListMultipartUploadsInputListMultipartUploadsPaginateTypeDef",
     "ListPartsInputListPartsPaginateTypeDef",
     "ListVaultsInputListVaultsPaginateTypeDef",
     "ListMultipartUploadsOutputTypeDef",
     "ListPartsOutputTypeDef",
     "ListProvisionedCapacityOutputTypeDef",
     "SetVaultNotificationsInputNotificationSetTypeDef",
-    "SetVaultNotificationsInputRequestTypeDef",
-    "VaultNotificationConfigUnionTypeDef",
     "SelectParametersResponseTypeDef",
     "SelectParametersTypeDef",
     "GetDataRetrievalPolicyOutputTypeDef",
-    "DataRetrievalPolicyUnionTypeDef",
     "SetDataRetrievalPolicyInputRequestTypeDef",
-    "S3LocationOutputTypeDef",
     "S3LocationTypeDef",
-    "OutputLocationOutputTypeDef",
+    "OutputLocationResponseTypeDef",
     "OutputLocationTypeDef",
     "GlacierJobDescriptionResponseTypeDef",
     "GlacierJobDescriptionTypeDef",
     "JobParametersTypeDef",
     "ListJobsOutputTypeDef",
     "InitiateJobInputRequestTypeDef",
 )
@@ -598,16 +594,16 @@
 
 class GetVaultNotificationsInputRequestTypeDef(
     _RequiredGetVaultNotificationsInputRequestTypeDef,
     _OptionalGetVaultNotificationsInputRequestTypeDef,
 ):
     pass
 
-VaultNotificationConfigOutputTypeDef = TypedDict(
-    "VaultNotificationConfigOutputTypeDef",
+VaultNotificationConfigTypeDef = TypedDict(
+    "VaultNotificationConfigTypeDef",
     {
         "SNSTopic": str,
         "Events": List[str],
     },
     total=False,
 )
 
@@ -871,16 +867,16 @@
 )
 
 class RemoveTagsFromVaultInputRequestTypeDef(
     _RequiredRemoveTagsFromVaultInputRequestTypeDef, _OptionalRemoveTagsFromVaultInputRequestTypeDef
 ):
     pass
 
-VaultNotificationConfigTypeDef = TypedDict(
-    "VaultNotificationConfigTypeDef",
+VaultNotificationConfigNotificationTypeDef = TypedDict(
+    "VaultNotificationConfigNotificationTypeDef",
     {
         "SNSTopic": str,
         "Events": Sequence[str],
     },
     total=False,
 )
 
@@ -1087,26 +1083,18 @@
     "OutputSerializationTypeDef",
     {
         "csv": CSVOutputTypeDef,
     },
     total=False,
 )
 
-DataRetrievalPolicyOutputTypeDef = TypedDict(
-    "DataRetrievalPolicyOutputTypeDef",
-    {
-        "Rules": List[DataRetrievalRuleTypeDef],
-    },
-    total=False,
-)
-
 DataRetrievalPolicyTypeDef = TypedDict(
     "DataRetrievalPolicyTypeDef",
     {
-        "Rules": Sequence[DataRetrievalRuleTypeDef],
+        "Rules": List[DataRetrievalRuleTypeDef],
     },
     total=False,
 )
 
 _RequiredDescribeVaultInputVaultExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeVaultInputVaultExistsWaitTypeDef",
     {
@@ -1186,19 +1174,40 @@
     _OptionalSetVaultAccessPolicyInputRequestTypeDef,
 ):
     pass
 
 GetVaultNotificationsOutputTypeDef = TypedDict(
     "GetVaultNotificationsOutputTypeDef",
     {
-        "vaultNotificationConfig": VaultNotificationConfigOutputTypeDef,
+        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredSetVaultNotificationsInputRequestTypeDef = TypedDict(
+    "_RequiredSetVaultNotificationsInputRequestTypeDef",
+    {
+        "vaultName": str,
+    },
+)
+_OptionalSetVaultNotificationsInputRequestTypeDef = TypedDict(
+    "_OptionalSetVaultNotificationsInputRequestTypeDef",
+    {
+        "accountId": str,
+        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
+    },
+    total=False,
+)
+
+class SetVaultNotificationsInputRequestTypeDef(
+    _RequiredSetVaultNotificationsInputRequestTypeDef,
+    _OptionalSetVaultNotificationsInputRequestTypeDef,
+):
+    pass
+
 GrantTypeDef = TypedDict(
     "GrantTypeDef",
     {
         "Grantee": GranteeTypeDef,
         "Permission": PermissionType,
     },
     total=False,
@@ -1338,43 +1347,19 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetVaultNotificationsInputNotificationSetTypeDef = TypedDict(
     "SetVaultNotificationsInputNotificationSetTypeDef",
     {
-        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
-    },
-    total=False,
-)
-
-_RequiredSetVaultNotificationsInputRequestTypeDef = TypedDict(
-    "_RequiredSetVaultNotificationsInputRequestTypeDef",
-    {
-        "vaultName": str,
-    },
-)
-_OptionalSetVaultNotificationsInputRequestTypeDef = TypedDict(
-    "_OptionalSetVaultNotificationsInputRequestTypeDef",
-    {
-        "accountId": str,
-        "vaultNotificationConfig": VaultNotificationConfigTypeDef,
+        "vaultNotificationConfig": VaultNotificationConfigNotificationTypeDef,
     },
     total=False,
 )
 
-class SetVaultNotificationsInputRequestTypeDef(
-    _RequiredSetVaultNotificationsInputRequestTypeDef,
-    _OptionalSetVaultNotificationsInputRequestTypeDef,
-):
-    pass
-
-VaultNotificationConfigUnionTypeDef = Union[
-    VaultNotificationConfigTypeDef, VaultNotificationConfigOutputTypeDef
-]
 SelectParametersResponseTypeDef = TypedDict(
     "SelectParametersResponseTypeDef",
     {
         "InputSerialization": InputSerializationTypeDef,
         "ExpressionType": Literal["SQL"],
         "Expression": str,
         "OutputSerialization": OutputSerializationTypeDef,
@@ -1392,75 +1377,57 @@
     },
     total=False,
 )
 
 GetDataRetrievalPolicyOutputTypeDef = TypedDict(
     "GetDataRetrievalPolicyOutputTypeDef",
     {
-        "Policy": DataRetrievalPolicyOutputTypeDef,
+        "Policy": DataRetrievalPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DataRetrievalPolicyUnionTypeDef = Union[
-    DataRetrievalPolicyTypeDef, DataRetrievalPolicyOutputTypeDef
-]
 SetDataRetrievalPolicyInputRequestTypeDef = TypedDict(
     "SetDataRetrievalPolicyInputRequestTypeDef",
     {
         "accountId": str,
         "Policy": DataRetrievalPolicyTypeDef,
     },
     total=False,
 )
 
-S3LocationOutputTypeDef = TypedDict(
-    "S3LocationOutputTypeDef",
+S3LocationTypeDef = TypedDict(
+    "S3LocationTypeDef",
     {
         "BucketName": str,
         "Prefix": str,
         "Encryption": EncryptionTypeDef,
         "CannedACL": CannedACLType,
         "AccessControlList": List[GrantTypeDef],
         "Tagging": Dict[str, str],
         "UserMetadata": Dict[str, str],
         "StorageClass": StorageClassType,
     },
     total=False,
 )
 
-S3LocationTypeDef = TypedDict(
-    "S3LocationTypeDef",
+OutputLocationResponseTypeDef = TypedDict(
+    "OutputLocationResponseTypeDef",
     {
-        "BucketName": str,
-        "Prefix": str,
-        "Encryption": EncryptionTypeDef,
-        "CannedACL": CannedACLType,
-        "AccessControlList": Sequence[GrantTypeDef],
-        "Tagging": Mapping[str, str],
-        "UserMetadata": Mapping[str, str],
-        "StorageClass": StorageClassType,
-    },
-    total=False,
-)
-
-OutputLocationOutputTypeDef = TypedDict(
-    "OutputLocationOutputTypeDef",
-    {
-        "S3": S3LocationOutputTypeDef,
+        "S3": S3LocationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 OutputLocationTypeDef = TypedDict(
     "OutputLocationTypeDef",
     {
-        "S3": S3LocationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "S3": S3LocationTypeDef,
     },
+    total=False,
 )
 
 GlacierJobDescriptionResponseTypeDef = TypedDict(
     "GlacierJobDescriptionResponseTypeDef",
     {
         "JobId": str,
         "JobDescription": str,
@@ -1478,15 +1445,15 @@
         "SHA256TreeHash": str,
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
         "SelectParameters": SelectParametersTypeDef,
-        "OutputLocation": OutputLocationOutputTypeDef,
+        "OutputLocation": OutputLocationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GlacierJobDescriptionTypeDef = TypedDict(
     "GlacierJobDescriptionTypeDef",
     {
@@ -1506,15 +1473,15 @@
         "SHA256TreeHash": str,
         "ArchiveSHA256TreeHash": str,
         "RetrievalByteRange": str,
         "Tier": str,
         "InventoryRetrievalParameters": InventoryRetrievalJobDescriptionTypeDef,
         "JobOutputPath": str,
         "SelectParameters": SelectParametersTypeDef,
-        "OutputLocation": OutputLocationOutputTypeDef,
+        "OutputLocation": OutputLocationTypeDef,
     },
     total=False,
 )
 
 JobParametersTypeDef = TypedDict(
     "JobParametersTypeDef",
     {
```

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/waiter.py` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier/waiter.pyi` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-glacier-2.5.2.post1/types_aiobotocore_glacier.egg-info/SOURCES.txt` & `types-aiobotocore-glacier-2.5.2.post2/types_aiobotocore_glacier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

