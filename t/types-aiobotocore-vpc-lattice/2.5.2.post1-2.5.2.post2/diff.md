# Comparing `tmp/types-aiobotocore-vpc-lattice-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-vpc-lattice-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-vpc-lattice-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-vpc-lattice-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:29 2023, max compression
```

## Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1.tar` & `types-aiobotocore-vpc-lattice-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.193431 types-aiobotocore-vpc-lattice-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20722 2023-08-02 14:53:09.189431 types-aiobotocore-vpc-lattice-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:09.193431 types-aiobotocore-vpc-lattice-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.185430 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41389 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41319 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-08-02 14:50:50.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-08-02 14:50:50.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    49704 2023-08-02 14:50:54.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49655 2023-08-02 14:50:53.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.189431 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20722 2023-08-02 14:53:09.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 14:53:09.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:09.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:53:09.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.446643 types-aiobotocore-vpc-lattice-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14465 2023-08-04 13:59:29.446643 types-aiobotocore-vpc-lattice-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12932 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:29.446643 types-aiobotocore-vpc-lattice-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2099 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.446643 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2538 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2537 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      957 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    41317 2023-08-04 13:55:32.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    41247 2023-08-04 13:55:32.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10660 2023-08-04 13:55:32.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10658 2023-08-04 13:55:32.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11903 2023-08-04 13:55:32.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    11892 2023-08-04 13:55:32.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    48595 2023-08-04 13:55:33.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    48546 2023-08-04 13:55:33.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:55:31.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:29.446643 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14465 2023-08-04 13:59:29.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      889 2023-08-04 13:59:29.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:29.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:29.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:29.000000 types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/LICENSE` & `types-aiobotocore-vpc-lattice-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/setup.py` & `types-aiobotocore-vpc-lattice-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-vpc-lattice",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_vpc_lattice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.VPCLattice 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/__init__.py` & `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/__init__.pyi` & `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/__main__.py` & `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.VPCLattice 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.VPCLattice 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice\nOther"
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

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/client.py` & `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PutAuthPolicyResponseTypeDef,
     RegisterTargetsResponseTypeDef,
-    RuleActionUnionTypeDef,
-    RuleMatchUnionTypeDef,
+    RuleActionTypeDef,
+    RuleMatchTypeDef,
     RuleUpdateTypeDef,
     TargetGroupConfigTypeDef,
     TargetTypeDef,
     UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateListenerResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateServiceNetworkResponseTypeDef,
@@ -170,15 +170,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_access_log_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_access_log_subscription)
         """
 
     async def create_listener(
         self,
         *,
-        defaultAction: RuleActionUnionTypeDef,
+        defaultAction: RuleActionTypeDef,
         name: str,
         protocol: ListenerProtocolType,
         serviceIdentifier: str,
         clientToken: str = ...,
         port: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateListenerResponseTypeDef:
@@ -188,17 +188,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_listener)
         """
 
     async def create_rule(
         self,
         *,
-        action: RuleActionUnionTypeDef,
+        action: RuleActionTypeDef,
         listenerIdentifier: str,
-        match: RuleMatchUnionTypeDef,
+        match: RuleMatchTypeDef,
         name: str,
         priority: int,
         serviceIdentifier: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleResponseTypeDef:
         """
@@ -678,35 +678,31 @@
         Updates the specified access log subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_access_log_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_access_log_subscription)
         """
 
     async def update_listener(
-        self,
-        *,
-        defaultAction: RuleActionUnionTypeDef,
-        listenerIdentifier: str,
-        serviceIdentifier: str
+        self, *, defaultAction: RuleActionTypeDef, listenerIdentifier: str, serviceIdentifier: str
     ) -> UpdateListenerResponseTypeDef:
         """
         Updates the specified listener for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_listener)
         """
 
     async def update_rule(
         self,
         *,
         listenerIdentifier: str,
         ruleIdentifier: str,
         serviceIdentifier: str,
-        action: RuleActionUnionTypeDef = ...,
-        match: RuleMatchUnionTypeDef = ...,
+        action: RuleActionTypeDef = ...,
+        match: RuleMatchTypeDef = ...,
         priority: int = ...
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates a rule for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_rule)
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/client.pyi` & `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PutAuthPolicyResponseTypeDef,
     RegisterTargetsResponseTypeDef,
-    RuleActionUnionTypeDef,
-    RuleMatchUnionTypeDef,
+    RuleActionTypeDef,
+    RuleMatchTypeDef,
     RuleUpdateTypeDef,
     TargetGroupConfigTypeDef,
     TargetTypeDef,
     UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateListenerResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateServiceNetworkResponseTypeDef,
@@ -161,15 +161,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_access_log_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_access_log_subscription)
         """
     async def create_listener(
         self,
         *,
-        defaultAction: RuleActionUnionTypeDef,
+        defaultAction: RuleActionTypeDef,
         name: str,
         protocol: ListenerProtocolType,
         serviceIdentifier: str,
         clientToken: str = ...,
         port: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateListenerResponseTypeDef:
@@ -178,17 +178,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_listener)
         """
     async def create_rule(
         self,
         *,
-        action: RuleActionUnionTypeDef,
+        action: RuleActionTypeDef,
         listenerIdentifier: str,
-        match: RuleMatchUnionTypeDef,
+        match: RuleMatchTypeDef,
         name: str,
         priority: int,
         serviceIdentifier: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleResponseTypeDef:
         """
@@ -624,34 +624,30 @@
         """
         Updates the specified access log subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_access_log_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_access_log_subscription)
         """
     async def update_listener(
-        self,
-        *,
-        defaultAction: RuleActionUnionTypeDef,
-        listenerIdentifier: str,
-        serviceIdentifier: str
+        self, *, defaultAction: RuleActionTypeDef, listenerIdentifier: str, serviceIdentifier: str
     ) -> UpdateListenerResponseTypeDef:
         """
         Updates the specified listener for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_listener)
         """
     async def update_rule(
         self,
         *,
         listenerIdentifier: str,
         ruleIdentifier: str,
         serviceIdentifier: str,
-        action: RuleActionUnionTypeDef = ...,
-        match: RuleMatchUnionTypeDef = ...,
+        action: RuleActionTypeDef = ...,
+        match: RuleMatchTypeDef = ...,
         priority: int = ...
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates a rule for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_rule)
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/literals.py` & `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,14 +100,15 @@
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
@@ -203,14 +204,15 @@
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
@@ -289,26 +291,28 @@
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

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/literals.pyi` & `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -98,14 +98,15 @@
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
@@ -201,14 +202,15 @@
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
@@ -287,26 +289,28 @@
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

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/paginator.py` & `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/paginator.pyi` & `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/type_defs.py` & `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_vpc_lattice.type_defs import AccessLogSubscriptionSummaryTypeDef
 
     data: AccessLogSubscriptionSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AuthPolicyStateType,
     AuthTypeType,
     HealthCheckProtocolVersionType,
     IpAddressTypeType,
     ListenerProtocolType,
@@ -124,15 +124,14 @@
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     "ServiceSummaryTypeDef",
     "DeregisterTargetsRequestRequestTypeDef",
     "ListTargetsRequestRequestTypeDef",
     "RegisterTargetsRequestRequestTypeDef",
     "DeregisterTargetsResponseTypeDef",
     "RegisterTargetsResponseTypeDef",
-    "ForwardActionOutputTypeDef",
     "ForwardActionTypeDef",
     "HeaderMatchTypeDef",
     "HealthCheckConfigTypeDef",
     "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
     "ListListenersRequestListListenersPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
@@ -146,40 +145,35 @@
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     "ListServiceNetworksResponseTypeDef",
     "ListTargetGroupsResponseTypeDef",
     "ListTargetsResponseTypeDef",
     "PathMatchTypeDef",
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     "ListServicesResponseTypeDef",
-    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
     "TargetGroupConfigTypeDef",
     "UpdateTargetGroupRequestRequestTypeDef",
-    "HttpMatchOutputTypeDef",
     "HttpMatchTypeDef",
+    "CreateListenerRequestRequestTypeDef",
     "CreateListenerResponseTypeDef",
     "GetListenerResponseTypeDef",
-    "UpdateListenerResponseTypeDef",
-    "CreateListenerRequestRequestTypeDef",
-    "RuleActionUnionTypeDef",
     "UpdateListenerRequestRequestTypeDef",
+    "UpdateListenerResponseTypeDef",
     "CreateTargetGroupRequestRequestTypeDef",
     "CreateTargetGroupResponseTypeDef",
     "GetTargetGroupResponseTypeDef",
     "UpdateTargetGroupResponseTypeDef",
-    "RuleMatchOutputTypeDef",
     "RuleMatchTypeDef",
+    "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "RuleUpdateSuccessTypeDef",
-    "UpdateRuleResponseTypeDef",
-    "CreateRuleRequestRequestTypeDef",
-    "RuleMatchUnionTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRuleRequestRequestTypeDef",
+    "UpdateRuleResponseTypeDef",
     "BatchUpdateRuleResponseTypeDef",
     "BatchUpdateRuleRequestRequestTypeDef",
 )
 
 AccessLogSubscriptionSummaryTypeDef = TypedDict(
     "AccessLogSubscriptionSummaryTypeDef",
     {
@@ -1254,21 +1248,14 @@
     {
         "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ForwardActionOutputTypeDef = TypedDict(
-    "ForwardActionOutputTypeDef",
-    {
-        "targetGroups": List[WeightedTargetGroupTypeDef],
-    },
-)
-
 ForwardActionTypeDef = TypedDict(
     "ForwardActionTypeDef",
     {
         "targetGroups": Sequence[WeightedTargetGroupTypeDef],
     },
 )
 
@@ -1534,23 +1521,14 @@
     {
         "items": List[ServiceSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RuleActionOutputTypeDef = TypedDict(
-    "RuleActionOutputTypeDef",
-    {
-        "fixedResponse": FixedResponseActionTypeDef,
-        "forward": ForwardActionOutputTypeDef,
-    },
-    total=False,
-)
-
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "fixedResponse": FixedResponseActionTypeDef,
         "forward": ForwardActionTypeDef,
     },
     total=False,
@@ -1585,39 +1563,55 @@
     "UpdateTargetGroupRequestRequestTypeDef",
     {
         "healthCheck": HealthCheckConfigTypeDef,
         "targetGroupIdentifier": str,
     },
 )
 
-HttpMatchOutputTypeDef = TypedDict(
-    "HttpMatchOutputTypeDef",
+HttpMatchTypeDef = TypedDict(
+    "HttpMatchTypeDef",
     {
-        "headerMatches": List[HeaderMatchTypeDef],
+        "headerMatches": Sequence[HeaderMatchTypeDef],
         "method": str,
         "pathMatch": PathMatchTypeDef,
     },
     total=False,
 )
 
-HttpMatchTypeDef = TypedDict(
-    "HttpMatchTypeDef",
+_RequiredCreateListenerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateListenerRequestRequestTypeDef",
     {
-        "headerMatches": Sequence[HeaderMatchTypeDef],
-        "method": str,
-        "pathMatch": PathMatchTypeDef,
+        "defaultAction": RuleActionTypeDef,
+        "name": str,
+        "protocol": ListenerProtocolType,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalCreateListenerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateListenerRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "port": int,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
+class CreateListenerRequestRequestTypeDef(
+    _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
+):
+    pass
+
+
 CreateListenerResponseTypeDef = TypedDict(
     "CreateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionOutputTypeDef,
+        "defaultAction": RuleActionTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1625,77 +1619,50 @@
 )
 
 GetListenerResponseTypeDef = TypedDict(
     "GetListenerResponseTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "defaultAction": RuleActionOutputTypeDef,
+        "defaultAction": RuleActionTypeDef,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateListenerRequestRequestTypeDef = TypedDict(
+    "UpdateListenerRequestRequestTypeDef",
+    {
+        "defaultAction": RuleActionTypeDef,
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
+    },
+)
+
 UpdateListenerResponseTypeDef = TypedDict(
     "UpdateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionOutputTypeDef,
+        "defaultAction": RuleActionTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateListenerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "name": str,
-        "protocol": ListenerProtocolType,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalCreateListenerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateListenerRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "port": int,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateListenerRequestRequestTypeDef(
-    _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
-):
-    pass
-
-
-RuleActionUnionTypeDef = Union[RuleActionTypeDef, RuleActionOutputTypeDef]
-UpdateListenerRequestRequestTypeDef = TypedDict(
-    "UpdateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
-    },
-)
-
 _RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTargetGroupRequestRequestTypeDef",
     {
         "name": str,
         "type": TargetGroupTypeType,
     },
 )
@@ -1756,115 +1723,92 @@
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RuleMatchOutputTypeDef = TypedDict(
-    "RuleMatchOutputTypeDef",
+RuleMatchTypeDef = TypedDict(
+    "RuleMatchTypeDef",
     {
-        "httpMatch": HttpMatchOutputTypeDef,
+        "httpMatch": HttpMatchTypeDef,
     },
     total=False,
 )
 
-RuleMatchTypeDef = TypedDict(
-    "RuleMatchTypeDef",
+_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleRequestRequestTypeDef",
     {
-        "httpMatch": HttpMatchTypeDef,
+        "action": RuleActionTypeDef,
+        "listenerIdentifier": str,
+        "match": RuleMatchTypeDef,
+        "name": str,
+        "priority": int,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
+class CreateRuleRequestRequestTypeDef(
+    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+):
+    pass
+
+
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
-        "action": RuleActionOutputTypeDef,
+        "action": RuleActionTypeDef,
         "arn": str,
         "id": str,
-        "match": RuleMatchOutputTypeDef,
+        "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
-        "action": RuleActionOutputTypeDef,
+        "action": RuleActionTypeDef,
         "arn": str,
         "createdAt": datetime,
         "id": str,
         "isDefault": bool,
         "lastUpdatedAt": datetime,
-        "match": RuleMatchOutputTypeDef,
+        "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleUpdateSuccessTypeDef = TypedDict(
     "RuleUpdateSuccessTypeDef",
     {
-        "action": RuleActionOutputTypeDef,
-        "arn": str,
-        "id": str,
-        "isDefault": bool,
-        "match": RuleMatchOutputTypeDef,
-        "name": str,
-        "priority": int,
-    },
-    total=False,
-)
-
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
-    {
-        "action": RuleActionOutputTypeDef,
+        "action": RuleActionTypeDef,
         "arn": str,
         "id": str,
         "isDefault": bool,
-        "match": RuleMatchOutputTypeDef,
-        "name": str,
-        "priority": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleRequestRequestTypeDef",
-    {
-        "action": RuleActionTypeDef,
-        "listenerIdentifier": str,
         "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-
-class CreateRuleRequestRequestTypeDef(
-    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
-):
-    pass
-
-
-RuleMatchUnionTypeDef = Union[RuleMatchTypeDef, RuleMatchOutputTypeDef]
 _RequiredRuleUpdateTypeDef = TypedDict(
     "_RequiredRuleUpdateTypeDef",
     {
         "ruleIdentifier": str,
     },
 )
 _OptionalRuleUpdateTypeDef = TypedDict(
@@ -1903,14 +1847,28 @@
 
 class UpdateRuleRequestRequestTypeDef(
     _RequiredUpdateRuleRequestRequestTypeDef, _OptionalUpdateRuleRequestRequestTypeDef
 ):
     pass
 
 
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
+    {
+        "action": RuleActionTypeDef,
+        "arn": str,
+        "id": str,
+        "isDefault": bool,
+        "match": RuleMatchTypeDef,
+        "name": str,
+        "priority": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchUpdateRuleResponseTypeDef = TypedDict(
     "BatchUpdateRuleResponseTypeDef",
     {
         "successful": List[RuleUpdateSuccessTypeDef],
         "unsuccessful": List[RuleUpdateFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/type_defs.pyi` & `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_vpc_lattice.type_defs import AccessLogSubscriptionSummaryTypeDef
 
     data: AccessLogSubscriptionSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AuthPolicyStateType,
     AuthTypeType,
     HealthCheckProtocolVersionType,
     IpAddressTypeType,
     ListenerProtocolType,
@@ -123,15 +123,14 @@
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     "ServiceSummaryTypeDef",
     "DeregisterTargetsRequestRequestTypeDef",
     "ListTargetsRequestRequestTypeDef",
     "RegisterTargetsRequestRequestTypeDef",
     "DeregisterTargetsResponseTypeDef",
     "RegisterTargetsResponseTypeDef",
-    "ForwardActionOutputTypeDef",
     "ForwardActionTypeDef",
     "HeaderMatchTypeDef",
     "HealthCheckConfigTypeDef",
     "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
     "ListListenersRequestListListenersPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
@@ -145,40 +144,35 @@
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     "ListServiceNetworksResponseTypeDef",
     "ListTargetGroupsResponseTypeDef",
     "ListTargetsResponseTypeDef",
     "PathMatchTypeDef",
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     "ListServicesResponseTypeDef",
-    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
     "TargetGroupConfigTypeDef",
     "UpdateTargetGroupRequestRequestTypeDef",
-    "HttpMatchOutputTypeDef",
     "HttpMatchTypeDef",
+    "CreateListenerRequestRequestTypeDef",
     "CreateListenerResponseTypeDef",
     "GetListenerResponseTypeDef",
-    "UpdateListenerResponseTypeDef",
-    "CreateListenerRequestRequestTypeDef",
-    "RuleActionUnionTypeDef",
     "UpdateListenerRequestRequestTypeDef",
+    "UpdateListenerResponseTypeDef",
     "CreateTargetGroupRequestRequestTypeDef",
     "CreateTargetGroupResponseTypeDef",
     "GetTargetGroupResponseTypeDef",
     "UpdateTargetGroupResponseTypeDef",
-    "RuleMatchOutputTypeDef",
     "RuleMatchTypeDef",
+    "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "RuleUpdateSuccessTypeDef",
-    "UpdateRuleResponseTypeDef",
-    "CreateRuleRequestRequestTypeDef",
-    "RuleMatchUnionTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRuleRequestRequestTypeDef",
+    "UpdateRuleResponseTypeDef",
     "BatchUpdateRuleResponseTypeDef",
     "BatchUpdateRuleRequestRequestTypeDef",
 )
 
 AccessLogSubscriptionSummaryTypeDef = TypedDict(
     "AccessLogSubscriptionSummaryTypeDef",
     {
@@ -1229,21 +1223,14 @@
     {
         "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ForwardActionOutputTypeDef = TypedDict(
-    "ForwardActionOutputTypeDef",
-    {
-        "targetGroups": List[WeightedTargetGroupTypeDef],
-    },
-)
-
 ForwardActionTypeDef = TypedDict(
     "ForwardActionTypeDef",
     {
         "targetGroups": Sequence[WeightedTargetGroupTypeDef],
     },
 )
 
@@ -1497,23 +1484,14 @@
     {
         "items": List[ServiceSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RuleActionOutputTypeDef = TypedDict(
-    "RuleActionOutputTypeDef",
-    {
-        "fixedResponse": FixedResponseActionTypeDef,
-        "forward": ForwardActionOutputTypeDef,
-    },
-    total=False,
-)
-
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "fixedResponse": FixedResponseActionTypeDef,
         "forward": ForwardActionTypeDef,
     },
     total=False,
@@ -1546,39 +1524,53 @@
     "UpdateTargetGroupRequestRequestTypeDef",
     {
         "healthCheck": HealthCheckConfigTypeDef,
         "targetGroupIdentifier": str,
     },
 )
 
-HttpMatchOutputTypeDef = TypedDict(
-    "HttpMatchOutputTypeDef",
+HttpMatchTypeDef = TypedDict(
+    "HttpMatchTypeDef",
     {
-        "headerMatches": List[HeaderMatchTypeDef],
+        "headerMatches": Sequence[HeaderMatchTypeDef],
         "method": str,
         "pathMatch": PathMatchTypeDef,
     },
     total=False,
 )
 
-HttpMatchTypeDef = TypedDict(
-    "HttpMatchTypeDef",
+_RequiredCreateListenerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateListenerRequestRequestTypeDef",
     {
-        "headerMatches": Sequence[HeaderMatchTypeDef],
-        "method": str,
-        "pathMatch": PathMatchTypeDef,
+        "defaultAction": RuleActionTypeDef,
+        "name": str,
+        "protocol": ListenerProtocolType,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalCreateListenerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateListenerRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "port": int,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+class CreateListenerRequestRequestTypeDef(
+    _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
+):
+    pass
+
 CreateListenerResponseTypeDef = TypedDict(
     "CreateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionOutputTypeDef,
+        "defaultAction": RuleActionTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1586,75 +1578,50 @@
 )
 
 GetListenerResponseTypeDef = TypedDict(
     "GetListenerResponseTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "defaultAction": RuleActionOutputTypeDef,
+        "defaultAction": RuleActionTypeDef,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+UpdateListenerRequestRequestTypeDef = TypedDict(
+    "UpdateListenerRequestRequestTypeDef",
+    {
+        "defaultAction": RuleActionTypeDef,
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
+    },
+)
+
 UpdateListenerResponseTypeDef = TypedDict(
     "UpdateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionOutputTypeDef,
+        "defaultAction": RuleActionTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateListenerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "name": str,
-        "protocol": ListenerProtocolType,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalCreateListenerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateListenerRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "port": int,
-        "tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateListenerRequestRequestTypeDef(
-    _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
-):
-    pass
-
-RuleActionUnionTypeDef = Union[RuleActionTypeDef, RuleActionOutputTypeDef]
-UpdateListenerRequestRequestTypeDef = TypedDict(
-    "UpdateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
-    },
-)
-
 _RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTargetGroupRequestRequestTypeDef",
     {
         "name": str,
         "type": TargetGroupTypeType,
     },
 )
@@ -1713,113 +1680,90 @@
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RuleMatchOutputTypeDef = TypedDict(
-    "RuleMatchOutputTypeDef",
+RuleMatchTypeDef = TypedDict(
+    "RuleMatchTypeDef",
     {
-        "httpMatch": HttpMatchOutputTypeDef,
+        "httpMatch": HttpMatchTypeDef,
     },
     total=False,
 )
 
-RuleMatchTypeDef = TypedDict(
-    "RuleMatchTypeDef",
+_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleRequestRequestTypeDef",
     {
-        "httpMatch": HttpMatchTypeDef,
+        "action": RuleActionTypeDef,
+        "listenerIdentifier": str,
+        "match": RuleMatchTypeDef,
+        "name": str,
+        "priority": int,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+class CreateRuleRequestRequestTypeDef(
+    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+):
+    pass
+
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
-        "action": RuleActionOutputTypeDef,
+        "action": RuleActionTypeDef,
         "arn": str,
         "id": str,
-        "match": RuleMatchOutputTypeDef,
+        "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
-        "action": RuleActionOutputTypeDef,
+        "action": RuleActionTypeDef,
         "arn": str,
         "createdAt": datetime,
         "id": str,
         "isDefault": bool,
         "lastUpdatedAt": datetime,
-        "match": RuleMatchOutputTypeDef,
+        "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleUpdateSuccessTypeDef = TypedDict(
     "RuleUpdateSuccessTypeDef",
     {
-        "action": RuleActionOutputTypeDef,
-        "arn": str,
-        "id": str,
-        "isDefault": bool,
-        "match": RuleMatchOutputTypeDef,
-        "name": str,
-        "priority": int,
-    },
-    total=False,
-)
-
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
-    {
-        "action": RuleActionOutputTypeDef,
+        "action": RuleActionTypeDef,
         "arn": str,
         "id": str,
         "isDefault": bool,
-        "match": RuleMatchOutputTypeDef,
-        "name": str,
-        "priority": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleRequestRequestTypeDef",
-    {
-        "action": RuleActionTypeDef,
-        "listenerIdentifier": str,
         "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleRequestRequestTypeDef",
-    {
-        "clientToken": str,
-        "tags": Mapping[str, str],
     },
     total=False,
 )
 
-class CreateRuleRequestRequestTypeDef(
-    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
-):
-    pass
-
-RuleMatchUnionTypeDef = Union[RuleMatchTypeDef, RuleMatchOutputTypeDef]
 _RequiredRuleUpdateTypeDef = TypedDict(
     "_RequiredRuleUpdateTypeDef",
     {
         "ruleIdentifier": str,
     },
 )
 _OptionalRuleUpdateTypeDef = TypedDict(
@@ -1854,14 +1798,28 @@
 )
 
 class UpdateRuleRequestRequestTypeDef(
     _RequiredUpdateRuleRequestRequestTypeDef, _OptionalUpdateRuleRequestRequestTypeDef
 ):
     pass
 
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
+    {
+        "action": RuleActionTypeDef,
+        "arn": str,
+        "id": str,
+        "isDefault": bool,
+        "match": RuleMatchTypeDef,
+        "name": str,
+        "priority": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchUpdateRuleResponseTypeDef = TypedDict(
     "BatchUpdateRuleResponseTypeDef",
     {
         "successful": List[RuleUpdateSuccessTypeDef],
         "unsuccessful": List[RuleUpdateFailureTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt` & `types-aiobotocore-vpc-lattice-2.5.2.post2/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

