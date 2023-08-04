# Comparing `tmp/types-aiobotocore-managedblockchain-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-managedblockchain-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-managedblockchain-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:37 2023, max compression
+gzip compressed data, was "types-aiobotocore-managedblockchain-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:16 2023, max compression
```

## Comparing `types-aiobotocore-managedblockchain-2.5.2.post1.tar` & `types-aiobotocore-managedblockchain-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:37.977527 types-aiobotocore-managedblockchain-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-08-02 14:52:37.977527 types-aiobotocore-managedblockchain-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14906 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:37.977527 types-aiobotocore-managedblockchain-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:37.977527 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22343 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22306 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26824 2023-08-02 14:42:49.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26795 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:48.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:37.977527 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16464 2023-08-02 14:52:37.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:52:37.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:37.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:37.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:37.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:37.000000 types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.706643 types-aiobotocore-managedblockchain-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13487 2023-08-04 13:59:16.706643 types-aiobotocore-managedblockchain-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11929 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:16.706643 types-aiobotocore-managedblockchain-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2142 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.706643 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      721 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      720 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      983 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22333 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    22296 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9280 2023-08-04 13:43:49.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9278 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2093 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2090 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26442 2023-08-04 13:43:49.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    26413 2023-08-04 13:43:49.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:48.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:16.706643 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13487 2023-08-04 13:59:16.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1003 2023-08-04 13:59:16.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:16.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:16.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       36 2023-08-04 13:59:16.000000 types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/LICENSE` & `types-aiobotocore-managedblockchain-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/README.md` & `types-aiobotocore-managedblockchain-2.5.2.post2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,39 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-managedblockchain
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.ManagedBlockchain 2.5.2 service generated with mypy-boto3-builder 7.17.2
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore managedblockchain type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-managedblockchain"></a>
 
 # types-aiobotocore-managedblockchain
 
 [![PyPI - types-aiobotocore-managedblockchain](https://img.shields.io/pypi/v/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-managedblockchain.svg?color=blue)](https://pypi.org/project/types-aiobotocore-managedblockchain)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/)
@@ -15,15 +47,15 @@
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
 [types-aiobotocore-managedblockchain docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/).
 
 See how it helps to find and fix potential bugs:
 
@@ -257,138 +289,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_managedblockchain.literals` module contains literals
 extracted from shapes that can be used in user code for type checking.
 
+Full list of `ManagedBlockchain` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/literals/).
+
 ```python
-from types_aiobotocore_managedblockchain.literals import (
-    AccessorStatusType,
-    AccessorTypeType,
-    EditionType,
-    FrameworkType,
-    InvitationStatusType,
-    ListAccessorsPaginatorName,
-    MemberStatusType,
-    NetworkStatusType,
-    NodeStatusType,
-    ProposalStatusType,
-    StateDBTypeType,
-    ThresholdComparatorType,
-    VoteValueType,
-    ManagedBlockchainServiceName,
-    ServiceName,
-    ResourceServiceName,
-    PaginatorName,
-    RegionName,
-)
+from types_aiobotocore_managedblockchain.literals import AccessorStatusType
 
 
 def check_value(value: AccessorStatusType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_managedblockchain.type_defs` module contains structures and
 shapes assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `ManagedBlockchain` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain/type_defs/).
+
 ```python
-from types_aiobotocore_managedblockchain.type_defs import (
-    AccessorSummaryTypeDef,
-    AccessorTypeDef,
-    ApprovalThresholdPolicyTypeDef,
-    CreateAccessorInputRequestTypeDef,
-    ResponseMetadataTypeDef,
-    DeleteAccessorInputRequestTypeDef,
-    DeleteMemberInputRequestTypeDef,
-    DeleteNodeInputRequestTypeDef,
-    GetAccessorInputRequestTypeDef,
-    GetMemberInputRequestTypeDef,
-    GetNetworkInputRequestTypeDef,
-    GetNodeInputRequestTypeDef,
-    GetProposalInputRequestTypeDef,
-    NetworkSummaryTypeDef,
-    InviteActionTypeDef,
-    PaginatorConfigTypeDef,
-    ListAccessorsInputRequestTypeDef,
-    ListInvitationsInputRequestTypeDef,
-    ListMembersInputRequestTypeDef,
-    MemberSummaryTypeDef,
-    ListNetworksInputRequestTypeDef,
-    ListNodesInputRequestTypeDef,
-    NodeSummaryTypeDef,
-    ListProposalVotesInputRequestTypeDef,
-    VoteSummaryTypeDef,
-    ListProposalsInputRequestTypeDef,
-    ProposalSummaryTypeDef,
-    ListTagsForResourceRequestRequestTypeDef,
-    LogConfigurationTypeDef,
-    MemberFabricAttributesTypeDef,
-    MemberFabricConfigurationTypeDef,
-    NetworkEthereumAttributesTypeDef,
-    NetworkFabricAttributesTypeDef,
-    NetworkFabricConfigurationTypeDef,
-    NodeEthereumAttributesTypeDef,
-    NodeFabricAttributesTypeDef,
-    RemoveActionTypeDef,
-    RejectInvitationInputRequestTypeDef,
-    TagResourceRequestRequestTypeDef,
-    UntagResourceRequestRequestTypeDef,
-    VoteOnProposalInputRequestTypeDef,
-    VotingPolicyTypeDef,
-    CreateAccessorOutputTypeDef,
-    CreateMemberOutputTypeDef,
-    CreateNetworkOutputTypeDef,
-    CreateNodeOutputTypeDef,
-    CreateProposalOutputTypeDef,
-    GetAccessorOutputTypeDef,
-    ListAccessorsOutputTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    InvitationTypeDef,
-    ListNetworksOutputTypeDef,
-    ListAccessorsInputListAccessorsPaginateTypeDef,
-    ListMembersOutputTypeDef,
-    ListNodesOutputTypeDef,
-    ListProposalVotesOutputTypeDef,
-    ListProposalsOutputTypeDef,
-    LogConfigurationsTypeDef,
-    MemberFrameworkAttributesTypeDef,
-    MemberFrameworkConfigurationTypeDef,
-    NetworkFrameworkAttributesTypeDef,
-    NetworkFrameworkConfigurationTypeDef,
-    NodeFrameworkAttributesTypeDef,
-    ProposalActionsOutputTypeDef,
-    ProposalActionsTypeDef,
-    ListInvitationsOutputTypeDef,
-    MemberFabricLogPublishingConfigurationTypeDef,
-    NodeFabricLogPublishingConfigurationTypeDef,
-    NetworkTypeDef,
-    ProposalTypeDef,
-    CreateProposalInputRequestTypeDef,
-    ProposalActionsUnionTypeDef,
-    MemberLogPublishingConfigurationTypeDef,
-    NodeLogPublishingConfigurationTypeDef,
-    GetNetworkOutputTypeDef,
-    GetProposalOutputTypeDef,
-    MemberConfigurationTypeDef,
-    MemberTypeDef,
-    UpdateMemberInputRequestTypeDef,
-    NodeConfigurationTypeDef,
-    NodeTypeDef,
-    UpdateNodeInputRequestTypeDef,
-    CreateMemberInputRequestTypeDef,
-    CreateNetworkInputRequestTypeDef,
-    GetMemberOutputTypeDef,
-    CreateNodeInputRequestTypeDef,
-    GetNodeOutputTypeDef,
-)
+from types_aiobotocore_managedblockchain.type_defs import AccessorSummaryTypeDef
 
 
 def get_value() -> AccessorSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/setup.py` & `types-aiobotocore-managedblockchain-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-managedblockchain",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_managedblockchain"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ManagedBlockchain 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/__init__.py` & `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/__init__.pyi` & `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/__main__.py` & `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ManagedBlockchain 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_managedblockchain//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/managedblockchain.html#ManagedBlockchain\nOther"
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

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/client.py` & `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     ListProposalVotesOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     MemberConfigurationTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
-    ProposalActionsUnionTypeDef,
+    ProposalActionsTypeDef,
     VotingPolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -187,15 +187,15 @@
 
     async def create_proposal(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         MemberId: str,
-        Actions: ProposalActionsUnionTypeDef,
+        Actions: ProposalActionsTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateProposalOutputTypeDef:
         """
         Creates a proposal for a change to the network that other members of the network
         can vote on, for example, a proposal to add a new member to the network.
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/client.pyi` & `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     ListProposalVotesOutputTypeDef,
     ListTagsForResourceResponseTypeDef,
     MemberConfigurationTypeDef,
     MemberLogPublishingConfigurationTypeDef,
     NetworkFrameworkConfigurationTypeDef,
     NodeConfigurationTypeDef,
     NodeLogPublishingConfigurationTypeDef,
-    ProposalActionsUnionTypeDef,
+    ProposalActionsTypeDef,
     VotingPolicyTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -176,15 +176,15 @@
         """
     async def create_proposal(
         self,
         *,
         ClientRequestToken: str,
         NetworkId: str,
         MemberId: str,
-        Actions: ProposalActionsUnionTypeDef,
+        Actions: ProposalActionsTypeDef,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateProposalOutputTypeDef:
         """
         Creates a proposal for a change to the network that other members of the network
         can vote on, for example, a proposal to add a new member to the network.
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/literals.py` & `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
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
@@ -187,14 +188,15 @@
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
@@ -273,26 +275,28 @@
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

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/literals.pyi` & `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,15 @@
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
@@ -185,14 +186,15 @@
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
@@ -271,26 +273,28 @@
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

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/paginator.py` & `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/paginator.pyi` & `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/type_defs.py` & `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_managedblockchain.type_defs import AccessorSummaryTypeDef
 
     data: AccessorSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AccessorStatusType,
     EditionType,
     FrameworkType,
     InvitationStatusType,
     MemberStatusType,
@@ -34,15 +34,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteAccessorInputRequestTypeDef",
@@ -99,23 +98,21 @@
     "ListProposalsOutputTypeDef",
     "LogConfigurationsTypeDef",
     "MemberFrameworkAttributesTypeDef",
     "MemberFrameworkConfigurationTypeDef",
     "NetworkFrameworkAttributesTypeDef",
     "NetworkFrameworkConfigurationTypeDef",
     "NodeFrameworkAttributesTypeDef",
-    "ProposalActionsOutputTypeDef",
     "ProposalActionsTypeDef",
     "ListInvitationsOutputTypeDef",
     "MemberFabricLogPublishingConfigurationTypeDef",
     "NodeFabricLogPublishingConfigurationTypeDef",
     "NetworkTypeDef",
-    "ProposalTypeDef",
     "CreateProposalInputRequestTypeDef",
-    "ProposalActionsUnionTypeDef",
+    "ProposalTypeDef",
     "MemberLogPublishingConfigurationTypeDef",
     "NodeLogPublishingConfigurationTypeDef",
     "GetNetworkOutputTypeDef",
     "GetProposalOutputTypeDef",
     "MemberConfigurationTypeDef",
     "MemberTypeDef",
     "UpdateMemberInputRequestTypeDef",
@@ -176,21 +173,19 @@
     "_OptionalCreateAccessorInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateAccessorInputRequestTypeDef(
     _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
 ):
     pass
 
-
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -224,21 +219,19 @@
     "_OptionalDeleteNodeInputRequestTypeDef",
     {
         "MemberId": str,
     },
     total=False,
 )
 
-
 class DeleteNodeInputRequestTypeDef(
     _RequiredDeleteNodeInputRequestTypeDef, _OptionalDeleteNodeInputRequestTypeDef
 ):
     pass
 
-
 GetAccessorInputRequestTypeDef = TypedDict(
     "GetAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
     },
 )
 
@@ -268,21 +261,19 @@
     "_OptionalGetNodeInputRequestTypeDef",
     {
         "MemberId": str,
     },
     total=False,
 )
 
-
 class GetNodeInputRequestTypeDef(
     _RequiredGetNodeInputRequestTypeDef, _OptionalGetNodeInputRequestTypeDef
 ):
     pass
 
-
 GetProposalInputRequestTypeDef = TypedDict(
     "GetProposalInputRequestTypeDef",
     {
         "NetworkId": str,
         "ProposalId": str,
     },
 )
@@ -351,21 +342,19 @@
         "IsOwned": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListMembersInputRequestTypeDef(
     _RequiredListMembersInputRequestTypeDef, _OptionalListMembersInputRequestTypeDef
 ):
     pass
 
-
 MemberSummaryTypeDef = TypedDict(
     "MemberSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "Status": MemberStatusType,
@@ -401,21 +390,19 @@
         "Status": NodeStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListNodesInputRequestTypeDef(
     _RequiredListNodesInputRequestTypeDef, _OptionalListNodesInputRequestTypeDef
 ):
     pass
 
-
 NodeSummaryTypeDef = TypedDict(
     "NodeSummaryTypeDef",
     {
         "Id": str,
         "Status": NodeStatusType,
         "CreationDate": datetime,
         "AvailabilityZone": str,
@@ -437,21 +424,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListProposalVotesInputRequestTypeDef(
     _RequiredListProposalVotesInputRequestTypeDef, _OptionalListProposalVotesInputRequestTypeDef
 ):
     pass
 
-
 VoteSummaryTypeDef = TypedDict(
     "VoteSummaryTypeDef",
     {
         "Vote": VoteValueType,
         "MemberName": str,
         "MemberId": str,
     },
@@ -469,21 +454,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListProposalsInputRequestTypeDef(
     _RequiredListProposalsInputRequestTypeDef, _OptionalListProposalsInputRequestTypeDef
 ):
     pass
 
-
 ProposalSummaryTypeDef = TypedDict(
     "ProposalSummaryTypeDef",
     {
         "ProposalId": str,
         "Description": str,
         "ProposedByMemberId": str,
         "ProposedByMemberName": str,
@@ -796,23 +779,14 @@
     {
         "Fabric": NodeFabricAttributesTypeDef,
         "Ethereum": NodeEthereumAttributesTypeDef,
     },
     total=False,
 )
 
-ProposalActionsOutputTypeDef = TypedDict(
-    "ProposalActionsOutputTypeDef",
-    {
-        "Invitations": List[InviteActionTypeDef],
-        "Removals": List[RemoveActionTypeDef],
-    },
-    total=False,
-)
-
 ProposalActionsTypeDef = TypedDict(
     "ProposalActionsTypeDef",
     {
         "Invitations": Sequence[InviteActionTypeDef],
         "Removals": Sequence[RemoveActionTypeDef],
     },
     total=False,
@@ -859,35 +833,14 @@
         "CreationDate": datetime,
         "Tags": Dict[str, str],
         "Arn": str,
     },
     total=False,
 )
 
-ProposalTypeDef = TypedDict(
-    "ProposalTypeDef",
-    {
-        "ProposalId": str,
-        "NetworkId": str,
-        "Description": str,
-        "Actions": ProposalActionsOutputTypeDef,
-        "ProposedByMemberId": str,
-        "ProposedByMemberName": str,
-        "Status": ProposalStatusType,
-        "CreationDate": datetime,
-        "ExpirationDate": datetime,
-        "YesVoteCount": int,
-        "NoVoteCount": int,
-        "OutstandingVoteCount": int,
-        "Tags": Dict[str, str],
-        "Arn": str,
-    },
-    total=False,
-)
-
 _RequiredCreateProposalInputRequestTypeDef = TypedDict(
     "_RequiredCreateProposalInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "NetworkId": str,
         "MemberId": str,
         "Actions": ProposalActionsTypeDef,
@@ -898,22 +851,40 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateProposalInputRequestTypeDef(
     _RequiredCreateProposalInputRequestTypeDef, _OptionalCreateProposalInputRequestTypeDef
 ):
     pass
 
+ProposalTypeDef = TypedDict(
+    "ProposalTypeDef",
+    {
+        "ProposalId": str,
+        "NetworkId": str,
+        "Description": str,
+        "Actions": ProposalActionsTypeDef,
+        "ProposedByMemberId": str,
+        "ProposedByMemberName": str,
+        "Status": ProposalStatusType,
+        "CreationDate": datetime,
+        "ExpirationDate": datetime,
+        "YesVoteCount": int,
+        "NoVoteCount": int,
+        "OutstandingVoteCount": int,
+        "Tags": Dict[str, str],
+        "Arn": str,
+    },
+    total=False,
+)
 
-ProposalActionsUnionTypeDef = Union[ProposalActionsTypeDef, ProposalActionsOutputTypeDef]
 MemberLogPublishingConfigurationTypeDef = TypedDict(
     "MemberLogPublishingConfigurationTypeDef",
     {
         "Fabric": MemberFabricLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
@@ -956,21 +927,19 @@
         "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
         "Tags": Mapping[str, str],
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-
 class MemberConfigurationTypeDef(
     _RequiredMemberConfigurationTypeDef, _OptionalMemberConfigurationTypeDef
 ):
     pass
 
-
 MemberTypeDef = TypedDict(
     "MemberTypeDef",
     {
         "NetworkId": str,
         "Id": str,
         "Name": str,
         "Description": str,
@@ -996,21 +965,19 @@
     "_OptionalUpdateMemberInputRequestTypeDef",
     {
         "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMemberInputRequestTypeDef(
     _RequiredUpdateMemberInputRequestTypeDef, _OptionalUpdateMemberInputRequestTypeDef
 ):
     pass
 
-
 _RequiredNodeConfigurationTypeDef = TypedDict(
     "_RequiredNodeConfigurationTypeDef",
     {
         "InstanceType": str,
     },
 )
 _OptionalNodeConfigurationTypeDef = TypedDict(
@@ -1019,21 +986,19 @@
         "AvailabilityZone": str,
         "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
         "StateDB": StateDBTypeType,
     },
     total=False,
 )
 
-
 class NodeConfigurationTypeDef(
     _RequiredNodeConfigurationTypeDef, _OptionalNodeConfigurationTypeDef
 ):
     pass
 
-
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "NetworkId": str,
         "MemberId": str,
         "Id": str,
         "InstanceType": str,
@@ -1062,21 +1027,19 @@
     {
         "MemberId": str,
         "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateNodeInputRequestTypeDef(
     _RequiredUpdateNodeInputRequestTypeDef, _OptionalUpdateNodeInputRequestTypeDef
 ):
     pass
 
-
 CreateMemberInputRequestTypeDef = TypedDict(
     "CreateMemberInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "InvitationId": str,
         "NetworkId": str,
         "MemberConfiguration": MemberConfigurationTypeDef,
@@ -1100,21 +1063,19 @@
         "Description": str,
         "FrameworkConfiguration": NetworkFrameworkConfigurationTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateNetworkInputRequestTypeDef(
     _RequiredCreateNetworkInputRequestTypeDef, _OptionalCreateNetworkInputRequestTypeDef
 ):
     pass
 
-
 GetMemberOutputTypeDef = TypedDict(
     "GetMemberOutputTypeDef",
     {
         "Member": MemberTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1132,21 +1093,19 @@
     {
         "MemberId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateNodeInputRequestTypeDef(
     _RequiredCreateNodeInputRequestTypeDef, _OptionalCreateNodeInputRequestTypeDef
 ):
     pass
 
-
 GetNodeOutputTypeDef = TypedDict(
     "GetNodeOutputTypeDef",
     {
         "Node": NodeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain/type_defs.pyi` & `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_managedblockchain.type_defs import AccessorSummaryTypeDef
 
     data: AccessorSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AccessorStatusType,
     EditionType,
     FrameworkType,
     InvitationStatusType,
     MemberStatusType,
@@ -34,14 +34,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccessorSummaryTypeDef",
     "AccessorTypeDef",
     "ApprovalThresholdPolicyTypeDef",
     "CreateAccessorInputRequestTypeDef",
     "ResponseMetadataTypeDef",
     "DeleteAccessorInputRequestTypeDef",
@@ -98,23 +99,21 @@
     "ListProposalsOutputTypeDef",
     "LogConfigurationsTypeDef",
     "MemberFrameworkAttributesTypeDef",
     "MemberFrameworkConfigurationTypeDef",
     "NetworkFrameworkAttributesTypeDef",
     "NetworkFrameworkConfigurationTypeDef",
     "NodeFrameworkAttributesTypeDef",
-    "ProposalActionsOutputTypeDef",
     "ProposalActionsTypeDef",
     "ListInvitationsOutputTypeDef",
     "MemberFabricLogPublishingConfigurationTypeDef",
     "NodeFabricLogPublishingConfigurationTypeDef",
     "NetworkTypeDef",
-    "ProposalTypeDef",
     "CreateProposalInputRequestTypeDef",
-    "ProposalActionsUnionTypeDef",
+    "ProposalTypeDef",
     "MemberLogPublishingConfigurationTypeDef",
     "NodeLogPublishingConfigurationTypeDef",
     "GetNetworkOutputTypeDef",
     "GetProposalOutputTypeDef",
     "MemberConfigurationTypeDef",
     "MemberTypeDef",
     "UpdateMemberInputRequestTypeDef",
@@ -175,19 +174,21 @@
     "_OptionalCreateAccessorInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateAccessorInputRequestTypeDef(
     _RequiredCreateAccessorInputRequestTypeDef, _OptionalCreateAccessorInputRequestTypeDef
 ):
     pass
 
+
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
         "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
@@ -221,19 +222,21 @@
     "_OptionalDeleteNodeInputRequestTypeDef",
     {
         "MemberId": str,
     },
     total=False,
 )
 
+
 class DeleteNodeInputRequestTypeDef(
     _RequiredDeleteNodeInputRequestTypeDef, _OptionalDeleteNodeInputRequestTypeDef
 ):
     pass
 
+
 GetAccessorInputRequestTypeDef = TypedDict(
     "GetAccessorInputRequestTypeDef",
     {
         "AccessorId": str,
     },
 )
 
@@ -263,19 +266,21 @@
     "_OptionalGetNodeInputRequestTypeDef",
     {
         "MemberId": str,
     },
     total=False,
 )
 
+
 class GetNodeInputRequestTypeDef(
     _RequiredGetNodeInputRequestTypeDef, _OptionalGetNodeInputRequestTypeDef
 ):
     pass
 
+
 GetProposalInputRequestTypeDef = TypedDict(
     "GetProposalInputRequestTypeDef",
     {
         "NetworkId": str,
         "ProposalId": str,
     },
 )
@@ -344,19 +349,21 @@
         "IsOwned": bool,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListMembersInputRequestTypeDef(
     _RequiredListMembersInputRequestTypeDef, _OptionalListMembersInputRequestTypeDef
 ):
     pass
 
+
 MemberSummaryTypeDef = TypedDict(
     "MemberSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Description": str,
         "Status": MemberStatusType,
@@ -392,19 +399,21 @@
         "Status": NodeStatusType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListNodesInputRequestTypeDef(
     _RequiredListNodesInputRequestTypeDef, _OptionalListNodesInputRequestTypeDef
 ):
     pass
 
+
 NodeSummaryTypeDef = TypedDict(
     "NodeSummaryTypeDef",
     {
         "Id": str,
         "Status": NodeStatusType,
         "CreationDate": datetime,
         "AvailabilityZone": str,
@@ -426,19 +435,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListProposalVotesInputRequestTypeDef(
     _RequiredListProposalVotesInputRequestTypeDef, _OptionalListProposalVotesInputRequestTypeDef
 ):
     pass
 
+
 VoteSummaryTypeDef = TypedDict(
     "VoteSummaryTypeDef",
     {
         "Vote": VoteValueType,
         "MemberName": str,
         "MemberId": str,
     },
@@ -456,19 +467,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListProposalsInputRequestTypeDef(
     _RequiredListProposalsInputRequestTypeDef, _OptionalListProposalsInputRequestTypeDef
 ):
     pass
 
+
 ProposalSummaryTypeDef = TypedDict(
     "ProposalSummaryTypeDef",
     {
         "ProposalId": str,
         "Description": str,
         "ProposedByMemberId": str,
         "ProposedByMemberName": str,
@@ -781,23 +794,14 @@
     {
         "Fabric": NodeFabricAttributesTypeDef,
         "Ethereum": NodeEthereumAttributesTypeDef,
     },
     total=False,
 )
 
-ProposalActionsOutputTypeDef = TypedDict(
-    "ProposalActionsOutputTypeDef",
-    {
-        "Invitations": List[InviteActionTypeDef],
-        "Removals": List[RemoveActionTypeDef],
-    },
-    total=False,
-)
-
 ProposalActionsTypeDef = TypedDict(
     "ProposalActionsTypeDef",
     {
         "Invitations": Sequence[InviteActionTypeDef],
         "Removals": Sequence[RemoveActionTypeDef],
     },
     total=False,
@@ -844,35 +848,14 @@
         "CreationDate": datetime,
         "Tags": Dict[str, str],
         "Arn": str,
     },
     total=False,
 )
 
-ProposalTypeDef = TypedDict(
-    "ProposalTypeDef",
-    {
-        "ProposalId": str,
-        "NetworkId": str,
-        "Description": str,
-        "Actions": ProposalActionsOutputTypeDef,
-        "ProposedByMemberId": str,
-        "ProposedByMemberName": str,
-        "Status": ProposalStatusType,
-        "CreationDate": datetime,
-        "ExpirationDate": datetime,
-        "YesVoteCount": int,
-        "NoVoteCount": int,
-        "OutstandingVoteCount": int,
-        "Tags": Dict[str, str],
-        "Arn": str,
-    },
-    total=False,
-)
-
 _RequiredCreateProposalInputRequestTypeDef = TypedDict(
     "_RequiredCreateProposalInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "NetworkId": str,
         "MemberId": str,
         "Actions": ProposalActionsTypeDef,
@@ -883,20 +866,42 @@
     {
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateProposalInputRequestTypeDef(
     _RequiredCreateProposalInputRequestTypeDef, _OptionalCreateProposalInputRequestTypeDef
 ):
     pass
 
-ProposalActionsUnionTypeDef = Union[ProposalActionsTypeDef, ProposalActionsOutputTypeDef]
+
+ProposalTypeDef = TypedDict(
+    "ProposalTypeDef",
+    {
+        "ProposalId": str,
+        "NetworkId": str,
+        "Description": str,
+        "Actions": ProposalActionsTypeDef,
+        "ProposedByMemberId": str,
+        "ProposedByMemberName": str,
+        "Status": ProposalStatusType,
+        "CreationDate": datetime,
+        "ExpirationDate": datetime,
+        "YesVoteCount": int,
+        "NoVoteCount": int,
+        "OutstandingVoteCount": int,
+        "Tags": Dict[str, str],
+        "Arn": str,
+    },
+    total=False,
+)
+
 MemberLogPublishingConfigurationTypeDef = TypedDict(
     "MemberLogPublishingConfigurationTypeDef",
     {
         "Fabric": MemberFabricLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
@@ -939,19 +944,21 @@
         "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
         "Tags": Mapping[str, str],
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+
 class MemberConfigurationTypeDef(
     _RequiredMemberConfigurationTypeDef, _OptionalMemberConfigurationTypeDef
 ):
     pass
 
+
 MemberTypeDef = TypedDict(
     "MemberTypeDef",
     {
         "NetworkId": str,
         "Id": str,
         "Name": str,
         "Description": str,
@@ -977,19 +984,21 @@
     "_OptionalUpdateMemberInputRequestTypeDef",
     {
         "LogPublishingConfiguration": MemberLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMemberInputRequestTypeDef(
     _RequiredUpdateMemberInputRequestTypeDef, _OptionalUpdateMemberInputRequestTypeDef
 ):
     pass
 
+
 _RequiredNodeConfigurationTypeDef = TypedDict(
     "_RequiredNodeConfigurationTypeDef",
     {
         "InstanceType": str,
     },
 )
 _OptionalNodeConfigurationTypeDef = TypedDict(
@@ -998,19 +1007,21 @@
         "AvailabilityZone": str,
         "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
         "StateDB": StateDBTypeType,
     },
     total=False,
 )
 
+
 class NodeConfigurationTypeDef(
     _RequiredNodeConfigurationTypeDef, _OptionalNodeConfigurationTypeDef
 ):
     pass
 
+
 NodeTypeDef = TypedDict(
     "NodeTypeDef",
     {
         "NetworkId": str,
         "MemberId": str,
         "Id": str,
         "InstanceType": str,
@@ -1039,19 +1050,21 @@
     {
         "MemberId": str,
         "LogPublishingConfiguration": NodeLogPublishingConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateNodeInputRequestTypeDef(
     _RequiredUpdateNodeInputRequestTypeDef, _OptionalUpdateNodeInputRequestTypeDef
 ):
     pass
 
+
 CreateMemberInputRequestTypeDef = TypedDict(
     "CreateMemberInputRequestTypeDef",
     {
         "ClientRequestToken": str,
         "InvitationId": str,
         "NetworkId": str,
         "MemberConfiguration": MemberConfigurationTypeDef,
@@ -1075,19 +1088,21 @@
         "Description": str,
         "FrameworkConfiguration": NetworkFrameworkConfigurationTypeDef,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateNetworkInputRequestTypeDef(
     _RequiredCreateNetworkInputRequestTypeDef, _OptionalCreateNetworkInputRequestTypeDef
 ):
     pass
 
+
 GetMemberOutputTypeDef = TypedDict(
     "GetMemberOutputTypeDef",
     {
         "Member": MemberTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1105,19 +1120,21 @@
     {
         "MemberId": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateNodeInputRequestTypeDef(
     _RequiredCreateNodeInputRequestTypeDef, _OptionalCreateNodeInputRequestTypeDef
 ):
     pass
 
+
 GetNodeOutputTypeDef = TypedDict(
     "GetNodeOutputTypeDef",
     {
         "Node": NodeTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-managedblockchain-2.5.2.post1/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt` & `types-aiobotocore-managedblockchain-2.5.2.post2/types_aiobotocore_managedblockchain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

