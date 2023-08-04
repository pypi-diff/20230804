# Comparing `tmp/types-aiobotocore-transfer-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-transfer-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-transfer-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:08 2023, max compression
+gzip compressed data, was "types-aiobotocore-transfer-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
```

## Comparing `types-aiobotocore-transfer-2.5.2.post1.tar` & `types-aiobotocore-transfer-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.097434 types-aiobotocore-transfer-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22452 2023-08-02 14:53:08.081435 types-aiobotocore-transfer-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20930 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:08.097434 types-aiobotocore-transfer-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.081435 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49024 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    48944 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-08-02 14:50:44.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    61839 2023-08-02 14:50:45.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    61749 2023-08-02 14:50:44.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-08-02 14:50:43.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:08.081435 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22452 2023-08-02 14:53:07.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-02 14:53:07.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:07.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:07.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:07.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:07.000000 types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.206643 types-aiobotocore-transfer-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15082 2023-08-04 13:59:29.206643 types-aiobotocore-transfer-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13560 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.206643 types-aiobotocore-transfer-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2079 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.206643 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2923 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2922 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      947 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    49822 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    49741 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12293 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12291 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12803 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12790 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    60425 2023-08-04 13:55:20.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    60334 2023-08-04 13:55:19.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:17.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2438 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2436 2023-08-04 13:55:18.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.206643 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15082 2023-08-04 13:59:29.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      907 2023-08-04 13:59:29.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:29.000000 types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-transfer-2.5.2.post1/LICENSE` & `types-aiobotocore-transfer-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post1/setup.py` & `types-aiobotocore-transfer-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-transfer",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_transfer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Transfer 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/__init__.py` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/__init__.pyi` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/__main__.py` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Transfer 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Transfer 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer\nOther"
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

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/client.py` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeWorkflowResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EndpointDetailsUnionTypeDef,
+    EndpointDetailsTypeDef,
     HomeDirectoryMapEntryTypeDef,
     IdentityProviderDetailsTypeDef,
     ImportCertificateResponseTypeDef,
     ImportHostKeyResponseTypeDef,
     ImportSshPublicKeyResponseTypeDef,
     ListAccessesResponseTypeDef,
     ListAgreementsResponseTypeDef,
@@ -79,30 +79,32 @@
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
     ListServersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
-    PosixProfileUnionTypeDef,
-    ProtocolDetailsUnionTypeDef,
+    PosixProfileTypeDef,
+    ProtocolDetailsTypeDef,
+    SftpConnectorConfigTypeDef,
     StartFileTransferResponseTypeDef,
     TagTypeDef,
+    TestConnectionResponseTypeDef,
     TestIdentityProviderResponseTypeDef,
     TimestampTypeDef,
     UpdateAccessResponseTypeDef,
     UpdateAgreementResponseTypeDef,
     UpdateCertificateResponseTypeDef,
     UpdateConnectorResponseTypeDef,
     UpdateHostKeyResponseTypeDef,
     UpdateProfileResponseTypeDef,
     UpdateServerResponseTypeDef,
     UpdateUserResponseTypeDef,
-    WorkflowDetailsUnionTypeDef,
-    WorkflowStepUnionTypeDef,
+    WorkflowDetailsTypeDef,
+    WorkflowStepTypeDef,
 )
 from .waiter import ServerOfflineWaiter, ServerOnlineWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -171,15 +173,15 @@
         Role: str,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileUnionTypeDef = ...
+        PosixProfile: PosixProfileTypeDef = ...
     ) -> CreateAccessResponseTypeDef:
         """
         Used by administrators to choose which groups in the directory should have
         access to upload and download files over the enabled protocols using Transfer
         Family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_access)
@@ -205,22 +207,23 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_agreement)
         """
 
     async def create_connector(
         self,
         *,
         Url: str,
-        As2Config: As2ConnectorConfigTypeDef,
         AccessRole: str,
+        As2Config: As2ConnectorConfigTypeDef = ...,
         LoggingRole: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
+        SftpConfig: SftpConnectorConfigTypeDef = ...
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates the connector, which captures the parameters for an outbound connection
-        for the AS2 protocol.
+        for the AS2 or SFTP protocol.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_connector)
         """
 
     async def create_profile(
         self,
@@ -238,27 +241,27 @@
         """
 
     async def create_server(
         self,
         *,
         Certificate: str = ...,
         Domain: DomainType = ...,
-        EndpointDetails: EndpointDetailsUnionTypeDef = ...,
+        EndpointDetails: EndpointDetailsTypeDef = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         IdentityProviderType: IdentityProviderTypeType = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
-        ProtocolDetails: ProtocolDetailsUnionTypeDef = ...,
+        ProtocolDetails: ProtocolDetailsTypeDef = ...,
         SecurityPolicyName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        WorkflowDetails: WorkflowDetailsUnionTypeDef = ...,
+        WorkflowDetails: WorkflowDetailsTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> CreateServerResponseTypeDef:
         """
         Instantiates an auto-scaling virtual server based on the selected file transfer
         protocol in Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_server)
@@ -271,32 +274,32 @@
         Role: str,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileUnionTypeDef = ...,
+        PosixProfile: PosixProfileTypeDef = ...,
         SshPublicKeyBody: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user and associates them with an existing file transfer protocol-
         enabled server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_user)
         """
 
     async def create_workflow(
         self,
         *,
-        Steps: Sequence[WorkflowStepUnionTypeDef],
+        Steps: Sequence[WorkflowStepTypeDef],
         Description: str = ...,
-        OnExceptionSteps: Sequence[WorkflowStepUnionTypeDef] = ...,
+        OnExceptionSteps: Sequence[WorkflowStepTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWorkflowResponseTypeDef:
         """
         Allows you to create a workflow with specified steps and step details the
         workflow invokes after file transfer completes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_workflow)
@@ -330,15 +333,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#delete_certificate)
         """
 
     async def delete_connector(self, *, ConnectorId: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the agreement that's specified in the provided `ConnectorId`.
+        Deletes the connector that's specified in the provided `ConnectorId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#delete_connector)
         """
 
     async def delete_host_key(
         self, *, ServerId: str, HostKeyId: str
@@ -697,18 +700,25 @@
         Sends a callback for asynchronous custom steps.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.send_workflow_step_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#send_workflow_step_state)
         """
 
     async def start_file_transfer(
-        self, *, ConnectorId: str, SendFilePaths: Sequence[str]
+        self,
+        *,
+        ConnectorId: str,
+        SendFilePaths: Sequence[str] = ...,
+        RetrieveFilePaths: Sequence[str] = ...,
+        LocalDirectoryPath: str = ...,
+        RemoteDirectoryPath: str = ...
     ) -> StartFileTransferResponseTypeDef:
         """
-        Begins an outbound file transfer to a remote AS2 server.
+        Begins a file transfer between local Amazon Web Services storage and a remote
+        AS2 or SFTP server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.start_file_transfer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#start_file_transfer)
         """
 
     async def start_server(self, *, ServerId: str) -> EmptyResponseMetadataTypeDef:
         """
@@ -735,14 +745,22 @@
         Attaches a key-value pair to a resource, as identified by its Amazon Resource
         Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#tag_resource)
         """
 
+    async def test_connection(self, *, ConnectorId: str) -> TestConnectionResponseTypeDef:
+        """
+        Tests whether your SFTP connector is set up successfully.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.test_connection)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#test_connection)
+        """
+
     async def test_identity_provider(
         self,
         *,
         ServerId: str,
         UserName: str,
         ServerProtocol: ProtocolType = ...,
         SourceIp: str = ...,
@@ -773,15 +791,15 @@
         *,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileUnionTypeDef = ...,
+        PosixProfile: PosixProfileTypeDef = ...,
         Role: str = ...
     ) -> UpdateAccessResponseTypeDef:
         """
         Allows you to update parameters for the access specified in the `ServerID` and
         `ExternalID` parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_access)
@@ -825,15 +843,16 @@
     async def update_connector(
         self,
         *,
         ConnectorId: str,
         Url: str = ...,
         As2Config: As2ConnectorConfigTypeDef = ...,
         AccessRole: str = ...,
-        LoggingRole: str = ...
+        LoggingRole: str = ...,
+        SftpConfig: SftpConnectorConfigTypeDef = ...
     ) -> UpdateConnectorResponseTypeDef:
         """
         Updates some of the parameters for an existing connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_connector)
         """
@@ -860,25 +879,25 @@
         """
 
     async def update_server(
         self,
         *,
         ServerId: str,
         Certificate: str = ...,
-        ProtocolDetails: ProtocolDetailsUnionTypeDef = ...,
-        EndpointDetails: EndpointDetailsUnionTypeDef = ...,
+        ProtocolDetails: ProtocolDetailsTypeDef = ...,
+        EndpointDetails: EndpointDetailsTypeDef = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
         SecurityPolicyName: str = ...,
-        WorkflowDetails: WorkflowDetailsUnionTypeDef = ...,
+        WorkflowDetails: WorkflowDetailsTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> UpdateServerResponseTypeDef:
         """
         Updates the file transfer protocol-enabled server's properties after that server
         has been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_server)
@@ -890,15 +909,15 @@
         *,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileUnionTypeDef = ...,
+        PosixProfile: PosixProfileTypeDef = ...,
         Role: str = ...
     ) -> UpdateUserResponseTypeDef:
         """
         Assigns new properties to a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_user)
```

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/client.pyi` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     DescribeHostKeyResponseTypeDef,
     DescribeProfileResponseTypeDef,
     DescribeSecurityPolicyResponseTypeDef,
     DescribeServerResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeWorkflowResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EndpointDetailsUnionTypeDef,
+    EndpointDetailsTypeDef,
     HomeDirectoryMapEntryTypeDef,
     IdentityProviderDetailsTypeDef,
     ImportCertificateResponseTypeDef,
     ImportHostKeyResponseTypeDef,
     ImportSshPublicKeyResponseTypeDef,
     ListAccessesResponseTypeDef,
     ListAgreementsResponseTypeDef,
@@ -79,30 +79,32 @@
     ListHostKeysResponseTypeDef,
     ListProfilesResponseTypeDef,
     ListSecurityPoliciesResponseTypeDef,
     ListServersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsersResponseTypeDef,
     ListWorkflowsResponseTypeDef,
-    PosixProfileUnionTypeDef,
-    ProtocolDetailsUnionTypeDef,
+    PosixProfileTypeDef,
+    ProtocolDetailsTypeDef,
+    SftpConnectorConfigTypeDef,
     StartFileTransferResponseTypeDef,
     TagTypeDef,
+    TestConnectionResponseTypeDef,
     TestIdentityProviderResponseTypeDef,
     TimestampTypeDef,
     UpdateAccessResponseTypeDef,
     UpdateAgreementResponseTypeDef,
     UpdateCertificateResponseTypeDef,
     UpdateConnectorResponseTypeDef,
     UpdateHostKeyResponseTypeDef,
     UpdateProfileResponseTypeDef,
     UpdateServerResponseTypeDef,
     UpdateUserResponseTypeDef,
-    WorkflowDetailsUnionTypeDef,
-    WorkflowStepUnionTypeDef,
+    WorkflowDetailsTypeDef,
+    WorkflowStepTypeDef,
 )
 from .waiter import ServerOfflineWaiter, ServerOnlineWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -164,15 +166,15 @@
         Role: str,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileUnionTypeDef = ...
+        PosixProfile: PosixProfileTypeDef = ...
     ) -> CreateAccessResponseTypeDef:
         """
         Used by administrators to choose which groups in the directory should have
         access to upload and download files over the enabled protocols using Transfer
         Family.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_access)
@@ -196,22 +198,23 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_agreement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_agreement)
         """
     async def create_connector(
         self,
         *,
         Url: str,
-        As2Config: As2ConnectorConfigTypeDef,
         AccessRole: str,
+        As2Config: As2ConnectorConfigTypeDef = ...,
         LoggingRole: str = ...,
-        Tags: Sequence[TagTypeDef] = ...
+        Tags: Sequence[TagTypeDef] = ...,
+        SftpConfig: SftpConnectorConfigTypeDef = ...
     ) -> CreateConnectorResponseTypeDef:
         """
         Creates the connector, which captures the parameters for an outbound connection
-        for the AS2 protocol.
+        for the AS2 or SFTP protocol.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_connector)
         """
     async def create_profile(
         self,
         *,
@@ -227,27 +230,27 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_profile)
         """
     async def create_server(
         self,
         *,
         Certificate: str = ...,
         Domain: DomainType = ...,
-        EndpointDetails: EndpointDetailsUnionTypeDef = ...,
+        EndpointDetails: EndpointDetailsTypeDef = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         IdentityProviderType: IdentityProviderTypeType = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
-        ProtocolDetails: ProtocolDetailsUnionTypeDef = ...,
+        ProtocolDetails: ProtocolDetailsTypeDef = ...,
         SecurityPolicyName: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        WorkflowDetails: WorkflowDetailsUnionTypeDef = ...,
+        WorkflowDetails: WorkflowDetailsTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> CreateServerResponseTypeDef:
         """
         Instantiates an auto-scaling virtual server based on the selected file transfer
         protocol in Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_server)
@@ -259,31 +262,31 @@
         Role: str,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileUnionTypeDef = ...,
+        PosixProfile: PosixProfileTypeDef = ...,
         SshPublicKeyBody: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateUserResponseTypeDef:
         """
         Creates a user and associates them with an existing file transfer protocol-
         enabled server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#create_user)
         """
     async def create_workflow(
         self,
         *,
-        Steps: Sequence[WorkflowStepUnionTypeDef],
+        Steps: Sequence[WorkflowStepTypeDef],
         Description: str = ...,
-        OnExceptionSteps: Sequence[WorkflowStepUnionTypeDef] = ...,
+        OnExceptionSteps: Sequence[WorkflowStepTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWorkflowResponseTypeDef:
         """
         Allows you to create a workflow with specified steps and step details the
         workflow invokes after file transfer completes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.create_workflow)
@@ -313,15 +316,15 @@
         Deletes the certificate that's specified in the `CertificateId` parameter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_certificate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#delete_certificate)
         """
     async def delete_connector(self, *, ConnectorId: str) -> EmptyResponseMetadataTypeDef:
         """
-        Deletes the agreement that's specified in the provided `ConnectorId`.
+        Deletes the connector that's specified in the provided `ConnectorId`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.delete_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#delete_connector)
         """
     async def delete_host_key(
         self, *, ServerId: str, HostKeyId: str
     ) -> EmptyResponseMetadataTypeDef:
@@ -645,18 +648,25 @@
         """
         Sends a callback for asynchronous custom steps.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.send_workflow_step_state)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#send_workflow_step_state)
         """
     async def start_file_transfer(
-        self, *, ConnectorId: str, SendFilePaths: Sequence[str]
+        self,
+        *,
+        ConnectorId: str,
+        SendFilePaths: Sequence[str] = ...,
+        RetrieveFilePaths: Sequence[str] = ...,
+        LocalDirectoryPath: str = ...,
+        RemoteDirectoryPath: str = ...
     ) -> StartFileTransferResponseTypeDef:
         """
-        Begins an outbound file transfer to a remote AS2 server.
+        Begins a file transfer between local Amazon Web Services storage and a remote
+        AS2 or SFTP server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.start_file_transfer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#start_file_transfer)
         """
     async def start_server(self, *, ServerId: str) -> EmptyResponseMetadataTypeDef:
         """
         Changes the state of a file transfer protocol-enabled server from `OFFLINE` to
@@ -679,14 +689,21 @@
         """
         Attaches a key-value pair to a resource, as identified by its Amazon Resource
         Name (ARN).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#tag_resource)
         """
+    async def test_connection(self, *, ConnectorId: str) -> TestConnectionResponseTypeDef:
+        """
+        Tests whether your SFTP connector is set up successfully.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.test_connection)
+        [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#test_connection)
+        """
     async def test_identity_provider(
         self,
         *,
         ServerId: str,
         UserName: str,
         ServerProtocol: ProtocolType = ...,
         SourceIp: str = ...,
@@ -715,15 +732,15 @@
         *,
         ServerId: str,
         ExternalId: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileUnionTypeDef = ...,
+        PosixProfile: PosixProfileTypeDef = ...,
         Role: str = ...
     ) -> UpdateAccessResponseTypeDef:
         """
         Allows you to update parameters for the access specified in the `ServerID` and
         `ExternalID` parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_access)
@@ -764,15 +781,16 @@
     async def update_connector(
         self,
         *,
         ConnectorId: str,
         Url: str = ...,
         As2Config: As2ConnectorConfigTypeDef = ...,
         AccessRole: str = ...,
-        LoggingRole: str = ...
+        LoggingRole: str = ...,
+        SftpConfig: SftpConnectorConfigTypeDef = ...
     ) -> UpdateConnectorResponseTypeDef:
         """
         Updates some of the parameters for an existing connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_connector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_connector)
         """
@@ -796,25 +814,25 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_profile)
         """
     async def update_server(
         self,
         *,
         ServerId: str,
         Certificate: str = ...,
-        ProtocolDetails: ProtocolDetailsUnionTypeDef = ...,
-        EndpointDetails: EndpointDetailsUnionTypeDef = ...,
+        ProtocolDetails: ProtocolDetailsTypeDef = ...,
+        EndpointDetails: EndpointDetailsTypeDef = ...,
         EndpointType: EndpointTypeType = ...,
         HostKey: str = ...,
         IdentityProviderDetails: IdentityProviderDetailsTypeDef = ...,
         LoggingRole: str = ...,
         PostAuthenticationLoginBanner: str = ...,
         PreAuthenticationLoginBanner: str = ...,
         Protocols: Sequence[ProtocolType] = ...,
         SecurityPolicyName: str = ...,
-        WorkflowDetails: WorkflowDetailsUnionTypeDef = ...,
+        WorkflowDetails: WorkflowDetailsTypeDef = ...,
         StructuredLogDestinations: Sequence[str] = ...
     ) -> UpdateServerResponseTypeDef:
         """
         Updates the file transfer protocol-enabled server's properties after that server
         has been created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_server)
@@ -825,15 +843,15 @@
         *,
         ServerId: str,
         UserName: str,
         HomeDirectory: str = ...,
         HomeDirectoryType: HomeDirectoryTypeType = ...,
         HomeDirectoryMappings: Sequence[HomeDirectoryMapEntryTypeDef] = ...,
         Policy: str = ...,
-        PosixProfile: PosixProfileUnionTypeDef = ...,
+        PosixProfile: PosixProfileTypeDef = ...,
         Role: str = ...
     ) -> UpdateUserResponseTypeDef:
         """
         Assigns new properties to a user.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/transfer.html#Transfer.Client.update_user)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_transfer/client/#update_user)
```

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/literals.py` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AgreementStatusTypeType",
     "As2TransportType",
     "CertificateStatusTypeType",
     "CertificateTypeType",
     "CertificateUsageTypeType",
     "CompressionEnumType",
@@ -63,15 +62,14 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
-
 AgreementStatusTypeType = Literal["ACTIVE", "INACTIVE"]
 As2TransportType = Literal["HTTP"]
 CertificateStatusTypeType = Literal["ACTIVE", "INACTIVE", "PENDING_ROTATION"]
 CertificateTypeType = Literal["CERTIFICATE", "CERTIFICATE_WITH_PRIVATE_KEY"]
 CertificateUsageTypeType = Literal["ENCRYPTION", "SIGNING"]
 CompressionEnumType = Literal["DISABLED", "ZLIB"]
 CustomStepStatusType = Literal["FAILURE", "SUCCESS"]
@@ -132,14 +130,15 @@
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
@@ -235,14 +234,15 @@
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
@@ -321,26 +321,28 @@
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
@@ -505,14 +507,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/literals.pyi` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AgreementStatusTypeType",
     "As2TransportType",
     "CertificateStatusTypeType",
     "CertificateTypeType",
     "CertificateUsageTypeType",
     "CompressionEnumType",
@@ -62,14 +63,15 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "WaiterName",
     "RegionName",
 )
 
+
 AgreementStatusTypeType = Literal["ACTIVE", "INACTIVE"]
 As2TransportType = Literal["HTTP"]
 CertificateStatusTypeType = Literal["ACTIVE", "INACTIVE", "PENDING_ROTATION"]
 CertificateTypeType = Literal["CERTIFICATE", "CERTIFICATE_WITH_PRIVATE_KEY"]
 CertificateUsageTypeType = Literal["ENCRYPTION", "SIGNING"]
 CompressionEnumType = Literal["DISABLED", "ZLIB"]
 CustomStepStatusType = Literal["FAILURE", "SUCCESS"]
@@ -130,14 +132,15 @@
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
@@ -233,14 +236,15 @@
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
@@ -319,26 +323,28 @@
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
@@ -503,14 +509,15 @@
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
+    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
```

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/paginator.py` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/paginator.pyi` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/type_defs.py` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 
 __all__ = (
     "As2ConnectorConfigTypeDef",
     "HomeDirectoryMapEntryTypeDef",
     "PosixProfileTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
+    "SftpConnectorConfigTypeDef",
     "EndpointDetailsTypeDef",
     "IdentityProviderDetailsTypeDef",
     "ProtocolDetailsTypeDef",
     "CustomStepDetailsTypeDef",
     "DeleteAccessRequestRequestTypeDef",
     "DeleteAgreementRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
@@ -82,18 +83,15 @@
     "DescribeProfileRequestRequestTypeDef",
     "DescribeSecurityPolicyRequestRequestTypeDef",
     "DescribedSecurityPolicyTypeDef",
     "DescribeServerRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "DescribeWorkflowRequestRequestTypeDef",
-    "PosixProfileOutputTypeDef",
     "LoggingConfigurationTypeDef",
-    "EndpointDetailsOutputTypeDef",
-    "ProtocolDetailsOutputTypeDef",
     "SshPublicKeyTypeDef",
     "EfsFileLocationTypeDef",
     "ExecutionErrorTypeDef",
     "S3FileLocationTypeDef",
     "TimestampTypeDef",
     "ImportSshPublicKeyRequestRequestTypeDef",
     "S3InputFileLocationTypeDef",
@@ -121,22 +119,23 @@
     "ListedWorkflowTypeDef",
     "S3TagTypeDef",
     "SendWorkflowStepStateRequestRequestTypeDef",
     "UserDetailsTypeDef",
     "StartFileTransferRequestRequestTypeDef",
     "StartServerRequestRequestTypeDef",
     "StopServerRequestRequestTypeDef",
+    "TestConnectionRequestRequestTypeDef",
     "TestIdentityProviderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgreementRequestRequestTypeDef",
     "UpdateHostKeyRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "WorkflowDetailTypeDef",
-    "UpdateConnectorRequestRequestTypeDef",
     "CreateAccessRequestRequestTypeDef",
+    "DescribedAccessTypeDef",
     "UpdateAccessRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateAccessResponseTypeDef",
     "CreateAgreementResponseTypeDef",
     "CreateConnectorResponseTypeDef",
     "CreateProfileResponseTypeDef",
     "CreateServerResponseTypeDef",
@@ -144,42 +143,40 @@
     "CreateWorkflowResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ImportCertificateResponseTypeDef",
     "ImportHostKeyResponseTypeDef",
     "ImportSshPublicKeyResponseTypeDef",
     "ListSecurityPoliciesResponseTypeDef",
     "StartFileTransferResponseTypeDef",
+    "TestConnectionResponseTypeDef",
     "TestIdentityProviderResponseTypeDef",
     "UpdateAccessResponseTypeDef",
     "UpdateAgreementResponseTypeDef",
     "UpdateCertificateResponseTypeDef",
     "UpdateConnectorResponseTypeDef",
     "UpdateHostKeyResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "UpdateServerResponseTypeDef",
     "UpdateUserResponseTypeDef",
     "CreateAgreementRequestRequestTypeDef",
-    "CreateConnectorRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DescribedAgreementTypeDef",
     "DescribedCertificateTypeDef",
-    "DescribedConnectorTypeDef",
     "DescribedHostKeyTypeDef",
     "DescribedProfileTypeDef",
     "ImportHostKeyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateConnectorRequestRequestTypeDef",
+    "DescribedConnectorTypeDef",
+    "UpdateConnectorRequestRequestTypeDef",
     "DescribeSecurityPolicyResponseTypeDef",
     "DescribeServerRequestServerOfflineWaitTypeDef",
     "DescribeServerRequestServerOnlineWaitTypeDef",
-    "DescribedAccessTypeDef",
-    "PosixProfileUnionTypeDef",
-    "EndpointDetailsUnionTypeDef",
-    "ProtocolDetailsUnionTypeDef",
     "DescribedUserTypeDef",
     "ExecutionStepResultTypeDef",
     "FileLocationTypeDef",
     "ImportCertificateRequestRequestTypeDef",
     "UpdateCertificateRequestRequestTypeDef",
     "InputFileLocationTypeDef",
     "ListAccessesRequestListAccessesPaginateTypeDef",
@@ -198,57 +195,53 @@
     "ListCertificatesResponseTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListHostKeysResponseTypeDef",
     "ListProfilesResponseTypeDef",
     "ListServersResponseTypeDef",
     "ListUsersResponseTypeDef",
     "ListWorkflowsResponseTypeDef",
-    "TagStepDetailsOutputTypeDef",
     "TagStepDetailsTypeDef",
     "ServiceMetadataTypeDef",
-    "WorkflowDetailsOutputTypeDef",
     "WorkflowDetailsTypeDef",
+    "DescribeAccessResponseTypeDef",
     "DescribeAgreementResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
-    "DescribeConnectorResponseTypeDef",
     "DescribeHostKeyResponseTypeDef",
     "DescribeProfileResponseTypeDef",
-    "DescribeAccessResponseTypeDef",
+    "DescribeConnectorResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "ExecutionResultsTypeDef",
     "CopyStepDetailsTypeDef",
     "DecryptStepDetailsTypeDef",
     "ListedExecutionTypeDef",
-    "DescribedServerTypeDef",
     "CreateServerRequestRequestTypeDef",
+    "DescribedServerTypeDef",
     "UpdateServerRequestRequestTypeDef",
-    "WorkflowDetailsUnionTypeDef",
     "DescribedExecutionTypeDef",
-    "WorkflowStepOutputTypeDef",
     "WorkflowStepTypeDef",
     "ListExecutionsResponseTypeDef",
     "DescribeServerResponseTypeDef",
     "DescribeExecutionResponseTypeDef",
+    "CreateWorkflowRequestRequestTypeDef",
     "DescribedWorkflowTypeDef",
-    "WorkflowStepUnionTypeDef",
     "DescribeWorkflowResponseTypeDef",
-    "CreateWorkflowRequestRequestTypeDef",
 )
 
 As2ConnectorConfigTypeDef = TypedDict(
     "As2ConnectorConfigTypeDef",
     {
         "LocalProfileId": str,
         "PartnerProfileId": str,
         "MessageSubject": str,
         "Compression": CompressionEnumType,
         "EncryptionAlgorithm": EncryptionAlgType,
         "SigningAlgorithm": SigningAlgType,
         "MdnSigningAlgorithm": MdnSigningAlgType,
         "MdnResponse": MdnResponseType,
+        "BasicAuthSecretId": str,
     },
     total=False,
 )
 
 HomeDirectoryMapEntryTypeDef = TypedDict(
     "HomeDirectoryMapEntryTypeDef",
     {
@@ -292,14 +285,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+SftpConnectorConfigTypeDef = TypedDict(
+    "SftpConnectorConfigTypeDef",
+    {
+        "UserSecretId": str,
+        "TrustedHostKeys": Sequence[str],
+    },
+    total=False,
+)
+
 EndpointDetailsTypeDef = TypedDict(
     "EndpointDetailsTypeDef",
     {
         "AddressAllocationIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "VpcEndpointId": str,
         "VpcId": str,
@@ -539,68 +541,23 @@
 DescribeWorkflowRequestRequestTypeDef = TypedDict(
     "DescribeWorkflowRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
 )
 
-_RequiredPosixProfileOutputTypeDef = TypedDict(
-    "_RequiredPosixProfileOutputTypeDef",
-    {
-        "Uid": int,
-        "Gid": int,
-    },
-)
-_OptionalPosixProfileOutputTypeDef = TypedDict(
-    "_OptionalPosixProfileOutputTypeDef",
-    {
-        "SecondaryGids": List[int],
-    },
-    total=False,
-)
-
-
-class PosixProfileOutputTypeDef(
-    _RequiredPosixProfileOutputTypeDef, _OptionalPosixProfileOutputTypeDef
-):
-    pass
-
-
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "LoggingRole": str,
         "LogGroupName": str,
     },
     total=False,
 )
 
-EndpointDetailsOutputTypeDef = TypedDict(
-    "EndpointDetailsOutputTypeDef",
-    {
-        "AddressAllocationIds": List[str],
-        "SubnetIds": List[str],
-        "VpcEndpointId": str,
-        "VpcId": str,
-        "SecurityGroupIds": List[str],
-    },
-    total=False,
-)
-
-ProtocolDetailsOutputTypeDef = TypedDict(
-    "ProtocolDetailsOutputTypeDef",
-    {
-        "PassiveIp": str,
-        "TlsSessionResumptionMode": TlsSessionResumptionModeType,
-        "SetStatOption": SetStatOptionType,
-        "As2Transports": List[Literal["HTTP"]],
-    },
-    total=False,
-)
-
 SshPublicKeyTypeDef = TypedDict(
     "SshPublicKeyTypeDef",
     {
         "DateImported": datetime,
         "SshPublicKeyBody": str,
         "SshPublicKeyId": str,
     },
@@ -1027,36 +984,59 @@
 )
 
 
 class UserDetailsTypeDef(_RequiredUserDetailsTypeDef, _OptionalUserDetailsTypeDef):
     pass
 
 
-StartFileTransferRequestRequestTypeDef = TypedDict(
-    "StartFileTransferRequestRequestTypeDef",
+_RequiredStartFileTransferRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFileTransferRequestRequestTypeDef",
     {
         "ConnectorId": str,
+    },
+)
+_OptionalStartFileTransferRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFileTransferRequestRequestTypeDef",
+    {
         "SendFilePaths": Sequence[str],
+        "RetrieveFilePaths": Sequence[str],
+        "LocalDirectoryPath": str,
+        "RemoteDirectoryPath": str,
     },
+    total=False,
 )
 
+
+class StartFileTransferRequestRequestTypeDef(
+    _RequiredStartFileTransferRequestRequestTypeDef, _OptionalStartFileTransferRequestRequestTypeDef
+):
+    pass
+
+
 StartServerRequestRequestTypeDef = TypedDict(
     "StartServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
 StopServerRequestRequestTypeDef = TypedDict(
     "StopServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
+TestConnectionRequestRequestTypeDef = TypedDict(
+    "TestConnectionRequestRequestTypeDef",
+    {
+        "ConnectorId": str,
+    },
+)
+
 _RequiredTestIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredTestIdentityProviderRequestRequestTypeDef",
     {
         "ServerId": str,
         "UserName": str,
     },
 )
@@ -1147,38 +1127,14 @@
     "WorkflowDetailTypeDef",
     {
         "WorkflowId": str,
         "ExecutionRole": str,
     },
 )
 
-_RequiredUpdateConnectorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConnectorRequestRequestTypeDef",
-    {
-        "ConnectorId": str,
-    },
-)
-_OptionalUpdateConnectorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConnectorRequestRequestTypeDef",
-    {
-        "Url": str,
-        "As2Config": As2ConnectorConfigTypeDef,
-        "AccessRole": str,
-        "LoggingRole": str,
-    },
-    total=False,
-)
-
-
-class UpdateConnectorRequestRequestTypeDef(
-    _RequiredUpdateConnectorRequestRequestTypeDef, _OptionalUpdateConnectorRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateAccessRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessRequestRequestTypeDef",
     {
         "Role": str,
         "ServerId": str,
         "ExternalId": str,
     },
@@ -1198,14 +1154,28 @@
 
 class CreateAccessRequestRequestTypeDef(
     _RequiredCreateAccessRequestRequestTypeDef, _OptionalCreateAccessRequestRequestTypeDef
 ):
     pass
 
 
+DescribedAccessTypeDef = TypedDict(
+    "DescribedAccessTypeDef",
+    {
+        "HomeDirectory": str,
+        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
+        "HomeDirectoryType": HomeDirectoryTypeType,
+        "Policy": str,
+        "PosixProfile": PosixProfileTypeDef,
+        "Role": str,
+        "ExternalId": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateAccessRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessRequestRequestTypeDef",
     {
         "ServerId": str,
         "ExternalId": str,
     },
 )
@@ -1361,14 +1331,24 @@
     "StartFileTransferResponseTypeDef",
     {
         "TransferId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TestConnectionResponseTypeDef = TypedDict(
+    "TestConnectionResponseTypeDef",
+    {
+        "ConnectorId": str,
+        "Status": str,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TestIdentityProviderResponseTypeDef = TypedDict(
     "TestIdentityProviderResponseTypeDef",
     {
         "Response": str,
         "StatusCode": int,
         "Message": str,
         "Url": str,
@@ -1466,38 +1446,14 @@
 
 class CreateAgreementRequestRequestTypeDef(
     _RequiredCreateAgreementRequestRequestTypeDef, _OptionalCreateAgreementRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredCreateConnectorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConnectorRequestRequestTypeDef",
-    {
-        "Url": str,
-        "As2Config": As2ConnectorConfigTypeDef,
-        "AccessRole": str,
-    },
-)
-_OptionalCreateConnectorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConnectorRequestRequestTypeDef",
-    {
-        "LoggingRole": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateConnectorRequestRequestTypeDef(
-    _RequiredCreateConnectorRequestRequestTypeDef, _OptionalCreateConnectorRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredCreateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfileRequestRequestTypeDef",
     {
         "As2Id": str,
         "ProfileType": ProfileTypeType,
     },
 )
@@ -1604,40 +1560,14 @@
 
 class DescribedCertificateTypeDef(
     _RequiredDescribedCertificateTypeDef, _OptionalDescribedCertificateTypeDef
 ):
     pass
 
 
-_RequiredDescribedConnectorTypeDef = TypedDict(
-    "_RequiredDescribedConnectorTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedConnectorTypeDef = TypedDict(
-    "_OptionalDescribedConnectorTypeDef",
-    {
-        "ConnectorId": str,
-        "Url": str,
-        "As2Config": As2ConnectorConfigTypeDef,
-        "AccessRole": str,
-        "LoggingRole": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class DescribedConnectorTypeDef(
-    _RequiredDescribedConnectorTypeDef, _OptionalDescribedConnectorTypeDef
-):
-    pass
-
-
 _RequiredDescribedHostKeyTypeDef = TypedDict(
     "_RequiredDescribedHostKeyTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedHostKeyTypeDef = TypedDict(
@@ -1718,14 +1648,91 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredCreateConnectorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConnectorRequestRequestTypeDef",
+    {
+        "Url": str,
+        "AccessRole": str,
+    },
+)
+_OptionalCreateConnectorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConnectorRequestRequestTypeDef",
+    {
+        "As2Config": As2ConnectorConfigTypeDef,
+        "LoggingRole": str,
+        "Tags": Sequence[TagTypeDef],
+        "SftpConfig": SftpConnectorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateConnectorRequestRequestTypeDef(
+    _RequiredCreateConnectorRequestRequestTypeDef, _OptionalCreateConnectorRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredDescribedConnectorTypeDef = TypedDict(
+    "_RequiredDescribedConnectorTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalDescribedConnectorTypeDef = TypedDict(
+    "_OptionalDescribedConnectorTypeDef",
+    {
+        "ConnectorId": str,
+        "Url": str,
+        "As2Config": As2ConnectorConfigTypeDef,
+        "AccessRole": str,
+        "LoggingRole": str,
+        "Tags": List[TagTypeDef],
+        "SftpConfig": SftpConnectorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribedConnectorTypeDef(
+    _RequiredDescribedConnectorTypeDef, _OptionalDescribedConnectorTypeDef
+):
+    pass
+
+
+_RequiredUpdateConnectorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConnectorRequestRequestTypeDef",
+    {
+        "ConnectorId": str,
+    },
+)
+_OptionalUpdateConnectorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConnectorRequestRequestTypeDef",
+    {
+        "Url": str,
+        "As2Config": As2ConnectorConfigTypeDef,
+        "AccessRole": str,
+        "LoggingRole": str,
+        "SftpConfig": SftpConnectorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateConnectorRequestRequestTypeDef(
+    _RequiredUpdateConnectorRequestRequestTypeDef, _OptionalUpdateConnectorRequestRequestTypeDef
+):
+    pass
+
+
 DescribeSecurityPolicyResponseTypeDef = TypedDict(
     "DescribeSecurityPolicyResponseTypeDef",
     {
         "SecurityPolicy": DescribedSecurityPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1770,45 +1777,28 @@
 class DescribeServerRequestServerOnlineWaitTypeDef(
     _RequiredDescribeServerRequestServerOnlineWaitTypeDef,
     _OptionalDescribeServerRequestServerOnlineWaitTypeDef,
 ):
     pass
 
 
-DescribedAccessTypeDef = TypedDict(
-    "DescribedAccessTypeDef",
-    {
-        "HomeDirectory": str,
-        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
-        "HomeDirectoryType": HomeDirectoryTypeType,
-        "Policy": str,
-        "PosixProfile": PosixProfileOutputTypeDef,
-        "Role": str,
-        "ExternalId": str,
-    },
-    total=False,
-)
-
-PosixProfileUnionTypeDef = Union[PosixProfileTypeDef, PosixProfileOutputTypeDef]
-EndpointDetailsUnionTypeDef = Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]
-ProtocolDetailsUnionTypeDef = Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef]
 _RequiredDescribedUserTypeDef = TypedDict(
     "_RequiredDescribedUserTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedUserTypeDef = TypedDict(
     "_OptionalDescribedUserTypeDef",
     {
         "HomeDirectory": str,
         "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
-        "PosixProfile": PosixProfileOutputTypeDef,
+        "PosixProfile": PosixProfileTypeDef,
         "Role": str,
         "SshPublicKeys": List[SshPublicKeyTypeDef],
         "Tags": List[TagTypeDef],
         "UserName": str,
     },
     total=False,
 )
@@ -2135,24 +2125,14 @@
     {
         "NextToken": str,
         "Workflows": List[ListedWorkflowTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagStepDetailsOutputTypeDef = TypedDict(
-    "TagStepDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Tags": List[S3TagTypeDef],
-        "SourceFileLocation": str,
-    },
-    total=False,
-)
-
 TagStepDetailsTypeDef = TypedDict(
     "TagStepDetailsTypeDef",
     {
         "Name": str,
         "Tags": Sequence[S3TagTypeDef],
         "SourceFileLocation": str,
     },
@@ -2162,32 +2142,32 @@
 ServiceMetadataTypeDef = TypedDict(
     "ServiceMetadataTypeDef",
     {
         "UserDetails": UserDetailsTypeDef,
     },
 )
 
-WorkflowDetailsOutputTypeDef = TypedDict(
-    "WorkflowDetailsOutputTypeDef",
-    {
-        "OnUpload": List[WorkflowDetailTypeDef],
-        "OnPartialUpload": List[WorkflowDetailTypeDef],
-    },
-    total=False,
-)
-
 WorkflowDetailsTypeDef = TypedDict(
     "WorkflowDetailsTypeDef",
     {
         "OnUpload": Sequence[WorkflowDetailTypeDef],
         "OnPartialUpload": Sequence[WorkflowDetailTypeDef],
     },
     total=False,
 )
 
+DescribeAccessResponseTypeDef = TypedDict(
+    "DescribeAccessResponseTypeDef",
+    {
+        "ServerId": str,
+        "Access": DescribedAccessTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeAgreementResponseTypeDef = TypedDict(
     "DescribeAgreementResponseTypeDef",
     {
         "Agreement": DescribedAgreementTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2196,22 +2176,14 @@
     "DescribeCertificateResponseTypeDef",
     {
         "Certificate": DescribedCertificateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeConnectorResponseTypeDef = TypedDict(
-    "DescribeConnectorResponseTypeDef",
-    {
-        "Connector": DescribedConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeHostKeyResponseTypeDef = TypedDict(
     "DescribeHostKeyResponseTypeDef",
     {
         "HostKey": DescribedHostKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2220,19 +2192,18 @@
     "DescribeProfileResponseTypeDef",
     {
         "Profile": DescribedProfileTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAccessResponseTypeDef = TypedDict(
-    "DescribeAccessResponseTypeDef",
+DescribeConnectorResponseTypeDef = TypedDict(
+    "DescribeConnectorResponseTypeDef",
     {
-        "ServerId": str,
-        "Access": DescribedAccessTypeDef,
+        "Connector": DescribedConnectorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
@@ -2293,74 +2264,74 @@
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "Status": ExecutionStatusType,
     },
     total=False,
 )
 
+CreateServerRequestRequestTypeDef = TypedDict(
+    "CreateServerRequestRequestTypeDef",
+    {
+        "Certificate": str,
+        "Domain": DomainType,
+        "EndpointDetails": EndpointDetailsTypeDef,
+        "EndpointType": EndpointTypeType,
+        "HostKey": str,
+        "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
+        "IdentityProviderType": IdentityProviderTypeType,
+        "LoggingRole": str,
+        "PostAuthenticationLoginBanner": str,
+        "PreAuthenticationLoginBanner": str,
+        "Protocols": Sequence[ProtocolType],
+        "ProtocolDetails": ProtocolDetailsTypeDef,
+        "SecurityPolicyName": str,
+        "Tags": Sequence[TagTypeDef],
+        "WorkflowDetails": WorkflowDetailsTypeDef,
+        "StructuredLogDestinations": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredDescribedServerTypeDef = TypedDict(
     "_RequiredDescribedServerTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedServerTypeDef = TypedDict(
     "_OptionalDescribedServerTypeDef",
     {
         "Certificate": str,
-        "ProtocolDetails": ProtocolDetailsOutputTypeDef,
+        "ProtocolDetails": ProtocolDetailsTypeDef,
         "Domain": DomainType,
-        "EndpointDetails": EndpointDetailsOutputTypeDef,
+        "EndpointDetails": EndpointDetailsTypeDef,
         "EndpointType": EndpointTypeType,
         "HostKeyFingerprint": str,
         "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
         "IdentityProviderType": IdentityProviderTypeType,
         "LoggingRole": str,
         "PostAuthenticationLoginBanner": str,
         "PreAuthenticationLoginBanner": str,
         "Protocols": List[ProtocolType],
         "SecurityPolicyName": str,
         "ServerId": str,
         "State": StateType,
         "Tags": List[TagTypeDef],
         "UserCount": int,
-        "WorkflowDetails": WorkflowDetailsOutputTypeDef,
+        "WorkflowDetails": WorkflowDetailsTypeDef,
         "StructuredLogDestinations": List[str],
     },
     total=False,
 )
 
 
 class DescribedServerTypeDef(_RequiredDescribedServerTypeDef, _OptionalDescribedServerTypeDef):
     pass
 
 
-CreateServerRequestRequestTypeDef = TypedDict(
-    "CreateServerRequestRequestTypeDef",
-    {
-        "Certificate": str,
-        "Domain": DomainType,
-        "EndpointDetails": EndpointDetailsTypeDef,
-        "EndpointType": EndpointTypeType,
-        "HostKey": str,
-        "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
-        "IdentityProviderType": IdentityProviderTypeType,
-        "LoggingRole": str,
-        "PostAuthenticationLoginBanner": str,
-        "PreAuthenticationLoginBanner": str,
-        "Protocols": Sequence[ProtocolType],
-        "ProtocolDetails": ProtocolDetailsTypeDef,
-        "SecurityPolicyName": str,
-        "Tags": Sequence[TagTypeDef],
-        "WorkflowDetails": WorkflowDetailsTypeDef,
-        "StructuredLogDestinations": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredUpdateServerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalUpdateServerRequestRequestTypeDef = TypedDict(
@@ -2386,43 +2357,29 @@
 
 class UpdateServerRequestRequestTypeDef(
     _RequiredUpdateServerRequestRequestTypeDef, _OptionalUpdateServerRequestRequestTypeDef
 ):
     pass
 
 
-WorkflowDetailsUnionTypeDef = Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef]
 DescribedExecutionTypeDef = TypedDict(
     "DescribedExecutionTypeDef",
     {
         "ExecutionId": str,
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "ExecutionRole": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "PosixProfile": PosixProfileOutputTypeDef,
+        "PosixProfile": PosixProfileTypeDef,
         "Status": ExecutionStatusType,
         "Results": ExecutionResultsTypeDef,
     },
     total=False,
 )
 
-WorkflowStepOutputTypeDef = TypedDict(
-    "WorkflowStepOutputTypeDef",
-    {
-        "Type": WorkflowStepTypeType,
-        "CopyStepDetails": CopyStepDetailsTypeDef,
-        "CustomStepDetails": CustomStepDetailsTypeDef,
-        "DeleteStepDetails": DeleteStepDetailsTypeDef,
-        "TagStepDetails": TagStepDetailsOutputTypeDef,
-        "DecryptStepDetails": DecryptStepDetailsTypeDef,
-    },
-    total=False,
-)
-
 WorkflowStepTypeDef = TypedDict(
     "WorkflowStepTypeDef",
     {
         "Type": WorkflowStepTypeType,
         "CopyStepDetails": CopyStepDetailsTypeDef,
         "CustomStepDetails": CustomStepDetailsTypeDef,
         "DeleteStepDetails": DeleteStepDetailsTypeDef,
@@ -2455,62 +2412,62 @@
     {
         "WorkflowId": str,
         "Execution": DescribedExecutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkflowRequestRequestTypeDef",
+    {
+        "Steps": Sequence[WorkflowStepTypeDef],
+    },
+)
+_OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkflowRequestRequestTypeDef",
+    {
+        "Description": str,
+        "OnExceptionSteps": Sequence[WorkflowStepTypeDef],
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateWorkflowRequestRequestTypeDef(
+    _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredDescribedWorkflowTypeDef = TypedDict(
     "_RequiredDescribedWorkflowTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedWorkflowTypeDef = TypedDict(
     "_OptionalDescribedWorkflowTypeDef",
     {
         "Description": str,
-        "Steps": List[WorkflowStepOutputTypeDef],
-        "OnExceptionSteps": List[WorkflowStepOutputTypeDef],
+        "Steps": List[WorkflowStepTypeDef],
+        "OnExceptionSteps": List[WorkflowStepTypeDef],
         "WorkflowId": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 
 class DescribedWorkflowTypeDef(
     _RequiredDescribedWorkflowTypeDef, _OptionalDescribedWorkflowTypeDef
 ):
     pass
 
 
-WorkflowStepUnionTypeDef = Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]
 DescribeWorkflowResponseTypeDef = TypedDict(
     "DescribeWorkflowResponseTypeDef",
     {
         "Workflow": DescribedWorkflowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkflowRequestRequestTypeDef",
-    {
-        "Steps": Sequence[WorkflowStepUnionTypeDef],
-    },
-)
-_OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkflowRequestRequestTypeDef",
-    {
-        "Description": str,
-        "OnExceptionSteps": Sequence[WorkflowStepUnionTypeDef],
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateWorkflowRequestRequestTypeDef(
-    _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/type_defs.pyi` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 
 __all__ = (
     "As2ConnectorConfigTypeDef",
     "HomeDirectoryMapEntryTypeDef",
     "PosixProfileTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
+    "SftpConnectorConfigTypeDef",
     "EndpointDetailsTypeDef",
     "IdentityProviderDetailsTypeDef",
     "ProtocolDetailsTypeDef",
     "CustomStepDetailsTypeDef",
     "DeleteAccessRequestRequestTypeDef",
     "DeleteAgreementRequestRequestTypeDef",
     "DeleteCertificateRequestRequestTypeDef",
@@ -81,18 +82,15 @@
     "DescribeProfileRequestRequestTypeDef",
     "DescribeSecurityPolicyRequestRequestTypeDef",
     "DescribedSecurityPolicyTypeDef",
     "DescribeServerRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "DescribeWorkflowRequestRequestTypeDef",
-    "PosixProfileOutputTypeDef",
     "LoggingConfigurationTypeDef",
-    "EndpointDetailsOutputTypeDef",
-    "ProtocolDetailsOutputTypeDef",
     "SshPublicKeyTypeDef",
     "EfsFileLocationTypeDef",
     "ExecutionErrorTypeDef",
     "S3FileLocationTypeDef",
     "TimestampTypeDef",
     "ImportSshPublicKeyRequestRequestTypeDef",
     "S3InputFileLocationTypeDef",
@@ -120,22 +118,23 @@
     "ListedWorkflowTypeDef",
     "S3TagTypeDef",
     "SendWorkflowStepStateRequestRequestTypeDef",
     "UserDetailsTypeDef",
     "StartFileTransferRequestRequestTypeDef",
     "StartServerRequestRequestTypeDef",
     "StopServerRequestRequestTypeDef",
+    "TestConnectionRequestRequestTypeDef",
     "TestIdentityProviderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAgreementRequestRequestTypeDef",
     "UpdateHostKeyRequestRequestTypeDef",
     "UpdateProfileRequestRequestTypeDef",
     "WorkflowDetailTypeDef",
-    "UpdateConnectorRequestRequestTypeDef",
     "CreateAccessRequestRequestTypeDef",
+    "DescribedAccessTypeDef",
     "UpdateAccessRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "CreateAccessResponseTypeDef",
     "CreateAgreementResponseTypeDef",
     "CreateConnectorResponseTypeDef",
     "CreateProfileResponseTypeDef",
     "CreateServerResponseTypeDef",
@@ -143,42 +142,40 @@
     "CreateWorkflowResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ImportCertificateResponseTypeDef",
     "ImportHostKeyResponseTypeDef",
     "ImportSshPublicKeyResponseTypeDef",
     "ListSecurityPoliciesResponseTypeDef",
     "StartFileTransferResponseTypeDef",
+    "TestConnectionResponseTypeDef",
     "TestIdentityProviderResponseTypeDef",
     "UpdateAccessResponseTypeDef",
     "UpdateAgreementResponseTypeDef",
     "UpdateCertificateResponseTypeDef",
     "UpdateConnectorResponseTypeDef",
     "UpdateHostKeyResponseTypeDef",
     "UpdateProfileResponseTypeDef",
     "UpdateServerResponseTypeDef",
     "UpdateUserResponseTypeDef",
     "CreateAgreementRequestRequestTypeDef",
-    "CreateConnectorRequestRequestTypeDef",
     "CreateProfileRequestRequestTypeDef",
     "CreateUserRequestRequestTypeDef",
     "DescribedAgreementTypeDef",
     "DescribedCertificateTypeDef",
-    "DescribedConnectorTypeDef",
     "DescribedHostKeyTypeDef",
     "DescribedProfileTypeDef",
     "ImportHostKeyRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateConnectorRequestRequestTypeDef",
+    "DescribedConnectorTypeDef",
+    "UpdateConnectorRequestRequestTypeDef",
     "DescribeSecurityPolicyResponseTypeDef",
     "DescribeServerRequestServerOfflineWaitTypeDef",
     "DescribeServerRequestServerOnlineWaitTypeDef",
-    "DescribedAccessTypeDef",
-    "PosixProfileUnionTypeDef",
-    "EndpointDetailsUnionTypeDef",
-    "ProtocolDetailsUnionTypeDef",
     "DescribedUserTypeDef",
     "ExecutionStepResultTypeDef",
     "FileLocationTypeDef",
     "ImportCertificateRequestRequestTypeDef",
     "UpdateCertificateRequestRequestTypeDef",
     "InputFileLocationTypeDef",
     "ListAccessesRequestListAccessesPaginateTypeDef",
@@ -197,57 +194,53 @@
     "ListCertificatesResponseTypeDef",
     "ListConnectorsResponseTypeDef",
     "ListHostKeysResponseTypeDef",
     "ListProfilesResponseTypeDef",
     "ListServersResponseTypeDef",
     "ListUsersResponseTypeDef",
     "ListWorkflowsResponseTypeDef",
-    "TagStepDetailsOutputTypeDef",
     "TagStepDetailsTypeDef",
     "ServiceMetadataTypeDef",
-    "WorkflowDetailsOutputTypeDef",
     "WorkflowDetailsTypeDef",
+    "DescribeAccessResponseTypeDef",
     "DescribeAgreementResponseTypeDef",
     "DescribeCertificateResponseTypeDef",
-    "DescribeConnectorResponseTypeDef",
     "DescribeHostKeyResponseTypeDef",
     "DescribeProfileResponseTypeDef",
-    "DescribeAccessResponseTypeDef",
+    "DescribeConnectorResponseTypeDef",
     "DescribeUserResponseTypeDef",
     "ExecutionResultsTypeDef",
     "CopyStepDetailsTypeDef",
     "DecryptStepDetailsTypeDef",
     "ListedExecutionTypeDef",
-    "DescribedServerTypeDef",
     "CreateServerRequestRequestTypeDef",
+    "DescribedServerTypeDef",
     "UpdateServerRequestRequestTypeDef",
-    "WorkflowDetailsUnionTypeDef",
     "DescribedExecutionTypeDef",
-    "WorkflowStepOutputTypeDef",
     "WorkflowStepTypeDef",
     "ListExecutionsResponseTypeDef",
     "DescribeServerResponseTypeDef",
     "DescribeExecutionResponseTypeDef",
+    "CreateWorkflowRequestRequestTypeDef",
     "DescribedWorkflowTypeDef",
-    "WorkflowStepUnionTypeDef",
     "DescribeWorkflowResponseTypeDef",
-    "CreateWorkflowRequestRequestTypeDef",
 )
 
 As2ConnectorConfigTypeDef = TypedDict(
     "As2ConnectorConfigTypeDef",
     {
         "LocalProfileId": str,
         "PartnerProfileId": str,
         "MessageSubject": str,
         "Compression": CompressionEnumType,
         "EncryptionAlgorithm": EncryptionAlgType,
         "SigningAlgorithm": SigningAlgType,
         "MdnSigningAlgorithm": MdnSigningAlgType,
         "MdnResponse": MdnResponseType,
+        "BasicAuthSecretId": str,
     },
     total=False,
 )
 
 HomeDirectoryMapEntryTypeDef = TypedDict(
     "HomeDirectoryMapEntryTypeDef",
     {
@@ -289,14 +282,23 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
+SftpConnectorConfigTypeDef = TypedDict(
+    "SftpConnectorConfigTypeDef",
+    {
+        "UserSecretId": str,
+        "TrustedHostKeys": Sequence[str],
+    },
+    total=False,
+)
+
 EndpointDetailsTypeDef = TypedDict(
     "EndpointDetailsTypeDef",
     {
         "AddressAllocationIds": Sequence[str],
         "SubnetIds": Sequence[str],
         "VpcEndpointId": str,
         "VpcId": str,
@@ -534,66 +536,23 @@
 DescribeWorkflowRequestRequestTypeDef = TypedDict(
     "DescribeWorkflowRequestRequestTypeDef",
     {
         "WorkflowId": str,
     },
 )
 
-_RequiredPosixProfileOutputTypeDef = TypedDict(
-    "_RequiredPosixProfileOutputTypeDef",
-    {
-        "Uid": int,
-        "Gid": int,
-    },
-)
-_OptionalPosixProfileOutputTypeDef = TypedDict(
-    "_OptionalPosixProfileOutputTypeDef",
-    {
-        "SecondaryGids": List[int],
-    },
-    total=False,
-)
-
-class PosixProfileOutputTypeDef(
-    _RequiredPosixProfileOutputTypeDef, _OptionalPosixProfileOutputTypeDef
-):
-    pass
-
 LoggingConfigurationTypeDef = TypedDict(
     "LoggingConfigurationTypeDef",
     {
         "LoggingRole": str,
         "LogGroupName": str,
     },
     total=False,
 )
 
-EndpointDetailsOutputTypeDef = TypedDict(
-    "EndpointDetailsOutputTypeDef",
-    {
-        "AddressAllocationIds": List[str],
-        "SubnetIds": List[str],
-        "VpcEndpointId": str,
-        "VpcId": str,
-        "SecurityGroupIds": List[str],
-    },
-    total=False,
-)
-
-ProtocolDetailsOutputTypeDef = TypedDict(
-    "ProtocolDetailsOutputTypeDef",
-    {
-        "PassiveIp": str,
-        "TlsSessionResumptionMode": TlsSessionResumptionModeType,
-        "SetStatOption": SetStatOptionType,
-        "As2Transports": List[Literal["HTTP"]],
-    },
-    total=False,
-)
-
 SshPublicKeyTypeDef = TypedDict(
     "SshPublicKeyTypeDef",
     {
         "DateImported": datetime,
         "SshPublicKeyBody": str,
         "SshPublicKeyId": str,
     },
@@ -1000,36 +959,57 @@
     },
     total=False,
 )
 
 class UserDetailsTypeDef(_RequiredUserDetailsTypeDef, _OptionalUserDetailsTypeDef):
     pass
 
-StartFileTransferRequestRequestTypeDef = TypedDict(
-    "StartFileTransferRequestRequestTypeDef",
+_RequiredStartFileTransferRequestRequestTypeDef = TypedDict(
+    "_RequiredStartFileTransferRequestRequestTypeDef",
     {
         "ConnectorId": str,
+    },
+)
+_OptionalStartFileTransferRequestRequestTypeDef = TypedDict(
+    "_OptionalStartFileTransferRequestRequestTypeDef",
+    {
         "SendFilePaths": Sequence[str],
+        "RetrieveFilePaths": Sequence[str],
+        "LocalDirectoryPath": str,
+        "RemoteDirectoryPath": str,
     },
+    total=False,
 )
 
+class StartFileTransferRequestRequestTypeDef(
+    _RequiredStartFileTransferRequestRequestTypeDef, _OptionalStartFileTransferRequestRequestTypeDef
+):
+    pass
+
 StartServerRequestRequestTypeDef = TypedDict(
     "StartServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
 StopServerRequestRequestTypeDef = TypedDict(
     "StopServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 
+TestConnectionRequestRequestTypeDef = TypedDict(
+    "TestConnectionRequestRequestTypeDef",
+    {
+        "ConnectorId": str,
+    },
+)
+
 _RequiredTestIdentityProviderRequestRequestTypeDef = TypedDict(
     "_RequiredTestIdentityProviderRequestRequestTypeDef",
     {
         "ServerId": str,
         "UserName": str,
     },
 )
@@ -1114,36 +1094,14 @@
     "WorkflowDetailTypeDef",
     {
         "WorkflowId": str,
         "ExecutionRole": str,
     },
 )
 
-_RequiredUpdateConnectorRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateConnectorRequestRequestTypeDef",
-    {
-        "ConnectorId": str,
-    },
-)
-_OptionalUpdateConnectorRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateConnectorRequestRequestTypeDef",
-    {
-        "Url": str,
-        "As2Config": As2ConnectorConfigTypeDef,
-        "AccessRole": str,
-        "LoggingRole": str,
-    },
-    total=False,
-)
-
-class UpdateConnectorRequestRequestTypeDef(
-    _RequiredUpdateConnectorRequestRequestTypeDef, _OptionalUpdateConnectorRequestRequestTypeDef
-):
-    pass
-
 _RequiredCreateAccessRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAccessRequestRequestTypeDef",
     {
         "Role": str,
         "ServerId": str,
         "ExternalId": str,
     },
@@ -1161,14 +1119,28 @@
 )
 
 class CreateAccessRequestRequestTypeDef(
     _RequiredCreateAccessRequestRequestTypeDef, _OptionalCreateAccessRequestRequestTypeDef
 ):
     pass
 
+DescribedAccessTypeDef = TypedDict(
+    "DescribedAccessTypeDef",
+    {
+        "HomeDirectory": str,
+        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
+        "HomeDirectoryType": HomeDirectoryTypeType,
+        "Policy": str,
+        "PosixProfile": PosixProfileTypeDef,
+        "Role": str,
+        "ExternalId": str,
+    },
+    total=False,
+)
+
 _RequiredUpdateAccessRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAccessRequestRequestTypeDef",
     {
         "ServerId": str,
         "ExternalId": str,
     },
 )
@@ -1320,14 +1292,24 @@
     "StartFileTransferResponseTypeDef",
     {
         "TransferId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TestConnectionResponseTypeDef = TypedDict(
+    "TestConnectionResponseTypeDef",
+    {
+        "ConnectorId": str,
+        "Status": str,
+        "StatusMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TestIdentityProviderResponseTypeDef = TypedDict(
     "TestIdentityProviderResponseTypeDef",
     {
         "Response": str,
         "StatusCode": int,
         "Message": str,
         "Url": str,
@@ -1423,36 +1405,14 @@
 )
 
 class CreateAgreementRequestRequestTypeDef(
     _RequiredCreateAgreementRequestRequestTypeDef, _OptionalCreateAgreementRequestRequestTypeDef
 ):
     pass
 
-_RequiredCreateConnectorRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateConnectorRequestRequestTypeDef",
-    {
-        "Url": str,
-        "As2Config": As2ConnectorConfigTypeDef,
-        "AccessRole": str,
-    },
-)
-_OptionalCreateConnectorRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateConnectorRequestRequestTypeDef",
-    {
-        "LoggingRole": str,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateConnectorRequestRequestTypeDef(
-    _RequiredCreateConnectorRequestRequestTypeDef, _OptionalCreateConnectorRequestRequestTypeDef
-):
-    pass
-
 _RequiredCreateProfileRequestRequestTypeDef = TypedDict(
     "_RequiredCreateProfileRequestRequestTypeDef",
     {
         "As2Id": str,
         "ProfileType": ProfileTypeType,
     },
 )
@@ -1551,38 +1511,14 @@
 )
 
 class DescribedCertificateTypeDef(
     _RequiredDescribedCertificateTypeDef, _OptionalDescribedCertificateTypeDef
 ):
     pass
 
-_RequiredDescribedConnectorTypeDef = TypedDict(
-    "_RequiredDescribedConnectorTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalDescribedConnectorTypeDef = TypedDict(
-    "_OptionalDescribedConnectorTypeDef",
-    {
-        "ConnectorId": str,
-        "Url": str,
-        "As2Config": As2ConnectorConfigTypeDef,
-        "AccessRole": str,
-        "LoggingRole": str,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-class DescribedConnectorTypeDef(
-    _RequiredDescribedConnectorTypeDef, _OptionalDescribedConnectorTypeDef
-):
-    pass
-
 _RequiredDescribedHostKeyTypeDef = TypedDict(
     "_RequiredDescribedHostKeyTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedHostKeyTypeDef = TypedDict(
@@ -1657,14 +1593,85 @@
     "TagResourceRequestRequestTypeDef",
     {
         "Arn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+_RequiredCreateConnectorRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateConnectorRequestRequestTypeDef",
+    {
+        "Url": str,
+        "AccessRole": str,
+    },
+)
+_OptionalCreateConnectorRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateConnectorRequestRequestTypeDef",
+    {
+        "As2Config": As2ConnectorConfigTypeDef,
+        "LoggingRole": str,
+        "Tags": Sequence[TagTypeDef],
+        "SftpConfig": SftpConnectorConfigTypeDef,
+    },
+    total=False,
+)
+
+class CreateConnectorRequestRequestTypeDef(
+    _RequiredCreateConnectorRequestRequestTypeDef, _OptionalCreateConnectorRequestRequestTypeDef
+):
+    pass
+
+_RequiredDescribedConnectorTypeDef = TypedDict(
+    "_RequiredDescribedConnectorTypeDef",
+    {
+        "Arn": str,
+    },
+)
+_OptionalDescribedConnectorTypeDef = TypedDict(
+    "_OptionalDescribedConnectorTypeDef",
+    {
+        "ConnectorId": str,
+        "Url": str,
+        "As2Config": As2ConnectorConfigTypeDef,
+        "AccessRole": str,
+        "LoggingRole": str,
+        "Tags": List[TagTypeDef],
+        "SftpConfig": SftpConnectorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribedConnectorTypeDef(
+    _RequiredDescribedConnectorTypeDef, _OptionalDescribedConnectorTypeDef
+):
+    pass
+
+_RequiredUpdateConnectorRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateConnectorRequestRequestTypeDef",
+    {
+        "ConnectorId": str,
+    },
+)
+_OptionalUpdateConnectorRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateConnectorRequestRequestTypeDef",
+    {
+        "Url": str,
+        "As2Config": As2ConnectorConfigTypeDef,
+        "AccessRole": str,
+        "LoggingRole": str,
+        "SftpConfig": SftpConnectorConfigTypeDef,
+    },
+    total=False,
+)
+
+class UpdateConnectorRequestRequestTypeDef(
+    _RequiredUpdateConnectorRequestRequestTypeDef, _OptionalUpdateConnectorRequestRequestTypeDef
+):
+    pass
+
 DescribeSecurityPolicyResponseTypeDef = TypedDict(
     "DescribeSecurityPolicyResponseTypeDef",
     {
         "SecurityPolicy": DescribedSecurityPolicyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1705,45 +1712,28 @@
 
 class DescribeServerRequestServerOnlineWaitTypeDef(
     _RequiredDescribeServerRequestServerOnlineWaitTypeDef,
     _OptionalDescribeServerRequestServerOnlineWaitTypeDef,
 ):
     pass
 
-DescribedAccessTypeDef = TypedDict(
-    "DescribedAccessTypeDef",
-    {
-        "HomeDirectory": str,
-        "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
-        "HomeDirectoryType": HomeDirectoryTypeType,
-        "Policy": str,
-        "PosixProfile": PosixProfileOutputTypeDef,
-        "Role": str,
-        "ExternalId": str,
-    },
-    total=False,
-)
-
-PosixProfileUnionTypeDef = Union[PosixProfileTypeDef, PosixProfileOutputTypeDef]
-EndpointDetailsUnionTypeDef = Union[EndpointDetailsTypeDef, EndpointDetailsOutputTypeDef]
-ProtocolDetailsUnionTypeDef = Union[ProtocolDetailsTypeDef, ProtocolDetailsOutputTypeDef]
 _RequiredDescribedUserTypeDef = TypedDict(
     "_RequiredDescribedUserTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedUserTypeDef = TypedDict(
     "_OptionalDescribedUserTypeDef",
     {
         "HomeDirectory": str,
         "HomeDirectoryMappings": List[HomeDirectoryMapEntryTypeDef],
         "HomeDirectoryType": HomeDirectoryTypeType,
         "Policy": str,
-        "PosixProfile": PosixProfileOutputTypeDef,
+        "PosixProfile": PosixProfileTypeDef,
         "Role": str,
         "SshPublicKeys": List[SshPublicKeyTypeDef],
         "Tags": List[TagTypeDef],
         "UserName": str,
     },
     total=False,
 )
@@ -2054,24 +2044,14 @@
     {
         "NextToken": str,
         "Workflows": List[ListedWorkflowTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagStepDetailsOutputTypeDef = TypedDict(
-    "TagStepDetailsOutputTypeDef",
-    {
-        "Name": str,
-        "Tags": List[S3TagTypeDef],
-        "SourceFileLocation": str,
-    },
-    total=False,
-)
-
 TagStepDetailsTypeDef = TypedDict(
     "TagStepDetailsTypeDef",
     {
         "Name": str,
         "Tags": Sequence[S3TagTypeDef],
         "SourceFileLocation": str,
     },
@@ -2081,32 +2061,32 @@
 ServiceMetadataTypeDef = TypedDict(
     "ServiceMetadataTypeDef",
     {
         "UserDetails": UserDetailsTypeDef,
     },
 )
 
-WorkflowDetailsOutputTypeDef = TypedDict(
-    "WorkflowDetailsOutputTypeDef",
-    {
-        "OnUpload": List[WorkflowDetailTypeDef],
-        "OnPartialUpload": List[WorkflowDetailTypeDef],
-    },
-    total=False,
-)
-
 WorkflowDetailsTypeDef = TypedDict(
     "WorkflowDetailsTypeDef",
     {
         "OnUpload": Sequence[WorkflowDetailTypeDef],
         "OnPartialUpload": Sequence[WorkflowDetailTypeDef],
     },
     total=False,
 )
 
+DescribeAccessResponseTypeDef = TypedDict(
+    "DescribeAccessResponseTypeDef",
+    {
+        "ServerId": str,
+        "Access": DescribedAccessTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeAgreementResponseTypeDef = TypedDict(
     "DescribeAgreementResponseTypeDef",
     {
         "Agreement": DescribedAgreementTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2115,22 +2095,14 @@
     "DescribeCertificateResponseTypeDef",
     {
         "Certificate": DescribedCertificateTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeConnectorResponseTypeDef = TypedDict(
-    "DescribeConnectorResponseTypeDef",
-    {
-        "Connector": DescribedConnectorTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeHostKeyResponseTypeDef = TypedDict(
     "DescribeHostKeyResponseTypeDef",
     {
         "HostKey": DescribedHostKeyTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2139,19 +2111,18 @@
     "DescribeProfileResponseTypeDef",
     {
         "Profile": DescribedProfileTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAccessResponseTypeDef = TypedDict(
-    "DescribeAccessResponseTypeDef",
+DescribeConnectorResponseTypeDef = TypedDict(
+    "DescribeConnectorResponseTypeDef",
     {
-        "ServerId": str,
-        "Access": DescribedAccessTypeDef,
+        "Connector": DescribedConnectorTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
@@ -2210,72 +2181,72 @@
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "Status": ExecutionStatusType,
     },
     total=False,
 )
 
+CreateServerRequestRequestTypeDef = TypedDict(
+    "CreateServerRequestRequestTypeDef",
+    {
+        "Certificate": str,
+        "Domain": DomainType,
+        "EndpointDetails": EndpointDetailsTypeDef,
+        "EndpointType": EndpointTypeType,
+        "HostKey": str,
+        "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
+        "IdentityProviderType": IdentityProviderTypeType,
+        "LoggingRole": str,
+        "PostAuthenticationLoginBanner": str,
+        "PreAuthenticationLoginBanner": str,
+        "Protocols": Sequence[ProtocolType],
+        "ProtocolDetails": ProtocolDetailsTypeDef,
+        "SecurityPolicyName": str,
+        "Tags": Sequence[TagTypeDef],
+        "WorkflowDetails": WorkflowDetailsTypeDef,
+        "StructuredLogDestinations": Sequence[str],
+    },
+    total=False,
+)
+
 _RequiredDescribedServerTypeDef = TypedDict(
     "_RequiredDescribedServerTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedServerTypeDef = TypedDict(
     "_OptionalDescribedServerTypeDef",
     {
         "Certificate": str,
-        "ProtocolDetails": ProtocolDetailsOutputTypeDef,
+        "ProtocolDetails": ProtocolDetailsTypeDef,
         "Domain": DomainType,
-        "EndpointDetails": EndpointDetailsOutputTypeDef,
+        "EndpointDetails": EndpointDetailsTypeDef,
         "EndpointType": EndpointTypeType,
         "HostKeyFingerprint": str,
         "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
         "IdentityProviderType": IdentityProviderTypeType,
         "LoggingRole": str,
         "PostAuthenticationLoginBanner": str,
         "PreAuthenticationLoginBanner": str,
         "Protocols": List[ProtocolType],
         "SecurityPolicyName": str,
         "ServerId": str,
         "State": StateType,
         "Tags": List[TagTypeDef],
         "UserCount": int,
-        "WorkflowDetails": WorkflowDetailsOutputTypeDef,
+        "WorkflowDetails": WorkflowDetailsTypeDef,
         "StructuredLogDestinations": List[str],
     },
     total=False,
 )
 
 class DescribedServerTypeDef(_RequiredDescribedServerTypeDef, _OptionalDescribedServerTypeDef):
     pass
 
-CreateServerRequestRequestTypeDef = TypedDict(
-    "CreateServerRequestRequestTypeDef",
-    {
-        "Certificate": str,
-        "Domain": DomainType,
-        "EndpointDetails": EndpointDetailsTypeDef,
-        "EndpointType": EndpointTypeType,
-        "HostKey": str,
-        "IdentityProviderDetails": IdentityProviderDetailsTypeDef,
-        "IdentityProviderType": IdentityProviderTypeType,
-        "LoggingRole": str,
-        "PostAuthenticationLoginBanner": str,
-        "PreAuthenticationLoginBanner": str,
-        "Protocols": Sequence[ProtocolType],
-        "ProtocolDetails": ProtocolDetailsTypeDef,
-        "SecurityPolicyName": str,
-        "Tags": Sequence[TagTypeDef],
-        "WorkflowDetails": WorkflowDetailsTypeDef,
-        "StructuredLogDestinations": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredUpdateServerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateServerRequestRequestTypeDef",
     {
         "ServerId": str,
     },
 )
 _OptionalUpdateServerRequestRequestTypeDef = TypedDict(
@@ -2299,43 +2270,29 @@
 )
 
 class UpdateServerRequestRequestTypeDef(
     _RequiredUpdateServerRequestRequestTypeDef, _OptionalUpdateServerRequestRequestTypeDef
 ):
     pass
 
-WorkflowDetailsUnionTypeDef = Union[WorkflowDetailsTypeDef, WorkflowDetailsOutputTypeDef]
 DescribedExecutionTypeDef = TypedDict(
     "DescribedExecutionTypeDef",
     {
         "ExecutionId": str,
         "InitialFileLocation": FileLocationTypeDef,
         "ServiceMetadata": ServiceMetadataTypeDef,
         "ExecutionRole": str,
         "LoggingConfiguration": LoggingConfigurationTypeDef,
-        "PosixProfile": PosixProfileOutputTypeDef,
+        "PosixProfile": PosixProfileTypeDef,
         "Status": ExecutionStatusType,
         "Results": ExecutionResultsTypeDef,
     },
     total=False,
 )
 
-WorkflowStepOutputTypeDef = TypedDict(
-    "WorkflowStepOutputTypeDef",
-    {
-        "Type": WorkflowStepTypeType,
-        "CopyStepDetails": CopyStepDetailsTypeDef,
-        "CustomStepDetails": CustomStepDetailsTypeDef,
-        "DeleteStepDetails": DeleteStepDetailsTypeDef,
-        "TagStepDetails": TagStepDetailsOutputTypeDef,
-        "DecryptStepDetails": DecryptStepDetailsTypeDef,
-    },
-    total=False,
-)
-
 WorkflowStepTypeDef = TypedDict(
     "WorkflowStepTypeDef",
     {
         "Type": WorkflowStepTypeType,
         "CopyStepDetails": CopyStepDetailsTypeDef,
         "CustomStepDetails": CustomStepDetailsTypeDef,
         "DeleteStepDetails": DeleteStepDetailsTypeDef,
@@ -2368,59 +2325,58 @@
     {
         "WorkflowId": str,
         "Execution": DescribedExecutionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateWorkflowRequestRequestTypeDef",
+    {
+        "Steps": Sequence[WorkflowStepTypeDef],
+    },
+)
+_OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateWorkflowRequestRequestTypeDef",
+    {
+        "Description": str,
+        "OnExceptionSteps": Sequence[WorkflowStepTypeDef],
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class CreateWorkflowRequestRequestTypeDef(
+    _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
+):
+    pass
+
 _RequiredDescribedWorkflowTypeDef = TypedDict(
     "_RequiredDescribedWorkflowTypeDef",
     {
         "Arn": str,
     },
 )
 _OptionalDescribedWorkflowTypeDef = TypedDict(
     "_OptionalDescribedWorkflowTypeDef",
     {
         "Description": str,
-        "Steps": List[WorkflowStepOutputTypeDef],
-        "OnExceptionSteps": List[WorkflowStepOutputTypeDef],
+        "Steps": List[WorkflowStepTypeDef],
+        "OnExceptionSteps": List[WorkflowStepTypeDef],
         "WorkflowId": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 class DescribedWorkflowTypeDef(
     _RequiredDescribedWorkflowTypeDef, _OptionalDescribedWorkflowTypeDef
 ):
     pass
 
-WorkflowStepUnionTypeDef = Union[WorkflowStepTypeDef, WorkflowStepOutputTypeDef]
 DescribeWorkflowResponseTypeDef = TypedDict(
     "DescribeWorkflowResponseTypeDef",
     {
         "Workflow": DescribedWorkflowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateWorkflowRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateWorkflowRequestRequestTypeDef",
-    {
-        "Steps": Sequence[WorkflowStepUnionTypeDef],
-    },
-)
-_OptionalCreateWorkflowRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateWorkflowRequestRequestTypeDef",
-    {
-        "Description": str,
-        "OnExceptionSteps": Sequence[WorkflowStepUnionTypeDef],
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class CreateWorkflowRequestRequestTypeDef(
-    _RequiredCreateWorkflowRequestRequestTypeDef, _OptionalCreateWorkflowRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/waiter.py` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer/waiter.pyi` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-transfer-2.5.2.post1/types_aiobotocore_transfer.egg-info/SOURCES.txt` & `types-aiobotocore-transfer-2.5.2.post2/types_aiobotocore_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

