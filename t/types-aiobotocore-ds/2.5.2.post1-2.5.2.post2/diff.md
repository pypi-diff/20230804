# Comparing `tmp/types-aiobotocore-ds-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ds-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ds-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-ds-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:47 2023, max compression
```

## Comparing `types-aiobotocore-ds-2.5.2.post1.tar` & `types-aiobotocore-ds-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.089601 types-aiobotocore-ds-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22600 2023-08-02 14:52:12.085601 types-aiobotocore-ds-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.089601 types-aiobotocore-ds-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-02 14:36:43.000000 types-aiobotocore-ds-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.085601 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54586 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54496 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-08-02 14:36:45.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-08-02 14:36:45.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-08-02 14:36:45.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    58571 2023-08-02 14:36:46.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    58498 2023-08-02 14:36:45.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:44.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.085601 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22600 2023-08-02 14:52:11.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-02 14:52:11.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:11.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:11.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 14:52:11.000000 types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.447954 types-aiobotocore-ds-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:44:05.000000 types-aiobotocore-ds-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-08-04 12:00:47.435953 types-aiobotocore-ds-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13461 2023-08-04 11:44:05.000000 types-aiobotocore-ds-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:47.447954 types-aiobotocore-ds-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-04 11:44:05.000000 types-aiobotocore-ds-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.435953 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-08-04 11:44:05.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-08-04 11:44:05.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-04 11:44:05.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54551 2023-08-04 11:44:06.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54461 2023-08-04 11:44:06.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-08-04 11:44:07.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-08-04 11:44:07.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-08-04 11:44:07.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17731 2023-08-04 11:44:07.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:44:05.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    57645 2023-08-04 11:44:09.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57572 2023-08-04 11:44:08.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:44:05.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:47.435953 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14973 2023-08-04 12:00:47.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-04 12:00:47.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:47.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:47.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-04 12:00:47.000000 types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ds-2.5.2.post1/LICENSE` & `types-aiobotocore-ds-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post1/setup.py` & `types-aiobotocore-ds-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ds",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ds"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DirectoryService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/__init__.py` & `types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/__init__.pyi` & `types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/__main__.py` & `types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.DirectoryService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService\nOther"
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

### Comparing `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/client.py` & `types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,25 +71,25 @@
     DescribeRegionsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
     DirectoryConnectSettingsTypeDef,
-    DirectoryVpcSettingsUnionTypeDef,
+    DirectoryVpcSettingsTypeDef,
     GetDirectoryLimitsResultTypeDef,
     GetSnapshotLimitsResultTypeDef,
     IpRouteTypeDef,
     ListCertificatesResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     OSUpdateSettingsTypeDef,
-    RadiusSettingsUnionTypeDef,
+    RadiusSettingsTypeDef,
     RegisterCertificateResultTypeDef,
     RejectSharedDirectoryResultTypeDef,
     SettingTypeDef,
     ShareDirectoryResultTypeDef,
     ShareTargetTypeDef,
     StartSchemaExtensionResultTypeDef,
     TagTypeDef,
@@ -199,15 +199,15 @@
         from your Microsoft AD on Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_ip_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#add_ip_routes)
         """
 
     async def add_region(
-        self, *, DirectoryId: str, RegionName: str, VPCSettings: DirectoryVpcSettingsUnionTypeDef
+        self, *, DirectoryId: str, RegionName: str, VPCSettings: DirectoryVpcSettingsTypeDef
     ) -> Dict[str, Any]:
         """
         Adds two domain controllers in the specified Region for the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_region)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#add_region)
         """
@@ -305,15 +305,15 @@
         self,
         *,
         Name: str,
         Password: str,
         Size: DirectorySizeType,
         ShortName: str = ...,
         Description: str = ...,
-        VpcSettings: DirectoryVpcSettingsUnionTypeDef = ...,
+        VpcSettings: DirectoryVpcSettingsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDirectoryResultTypeDef:
         """
         Creates a Simple AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_directory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_directory)
@@ -332,15 +332,15 @@
         """
 
     async def create_microsoft_ad(
         self,
         *,
         Name: str,
         Password: str,
-        VpcSettings: DirectoryVpcSettingsUnionTypeDef,
+        VpcSettings: DirectoryVpcSettingsTypeDef,
         ShortName: str = ...,
         Description: str = ...,
         Edition: DirectoryEditionType = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMicrosoftADResultTypeDef:
         """
         Creates a Microsoft AD directory in the Amazon Web Services Cloud.
@@ -671,15 +671,15 @@
         Activates the switch for the specific directory to always use LDAP secure calls.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_ldaps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#enable_ldaps)
         """
 
     async def enable_radius(
-        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsUnionTypeDef
+        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsTypeDef
     ) -> Dict[str, Any]:
         """
         Enables multi-factor authentication (MFA) with the Remote Authentication Dial In
         User Service (RADIUS) server for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_radius)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#enable_radius)
@@ -931,15 +931,15 @@
         Adds or removes domain controllers to or from the directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_number_of_domain_controllers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#update_number_of_domain_controllers)
         """
 
     async def update_radius(
-        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsUnionTypeDef
+        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the Remote Authentication Dial In User Service (RADIUS) server
         information for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_radius)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#update_radius)
```

### Comparing `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/client.pyi` & `types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -71,25 +71,25 @@
     DescribeRegionsResultTypeDef,
     DescribeSettingsResultTypeDef,
     DescribeSharedDirectoriesResultTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeTrustsResultTypeDef,
     DescribeUpdateDirectoryResultTypeDef,
     DirectoryConnectSettingsTypeDef,
-    DirectoryVpcSettingsUnionTypeDef,
+    DirectoryVpcSettingsTypeDef,
     GetDirectoryLimitsResultTypeDef,
     GetSnapshotLimitsResultTypeDef,
     IpRouteTypeDef,
     ListCertificatesResultTypeDef,
     ListIpRoutesResultTypeDef,
     ListLogSubscriptionsResultTypeDef,
     ListSchemaExtensionsResultTypeDef,
     ListTagsForResourceResultTypeDef,
     OSUpdateSettingsTypeDef,
-    RadiusSettingsUnionTypeDef,
+    RadiusSettingsTypeDef,
     RegisterCertificateResultTypeDef,
     RejectSharedDirectoryResultTypeDef,
     SettingTypeDef,
     ShareDirectoryResultTypeDef,
     ShareTargetTypeDef,
     StartSchemaExtensionResultTypeDef,
     TagTypeDef,
@@ -192,15 +192,15 @@
         address, you must add a CIDR address block to correctly route traffic to and
         from your Microsoft AD on Amazon Web Services.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_ip_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#add_ip_routes)
         """
     async def add_region(
-        self, *, DirectoryId: str, RegionName: str, VPCSettings: DirectoryVpcSettingsUnionTypeDef
+        self, *, DirectoryId: str, RegionName: str, VPCSettings: DirectoryVpcSettingsTypeDef
     ) -> Dict[str, Any]:
         """
         Adds two domain controllers in the specified Region for the specified directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.add_region)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#add_region)
         """
@@ -289,15 +289,15 @@
         self,
         *,
         Name: str,
         Password: str,
         Size: DirectorySizeType,
         ShortName: str = ...,
         Description: str = ...,
-        VpcSettings: DirectoryVpcSettingsUnionTypeDef = ...,
+        VpcSettings: DirectoryVpcSettingsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDirectoryResultTypeDef:
         """
         Creates a Simple AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.create_directory)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_directory)
@@ -314,15 +314,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#create_log_subscription)
         """
     async def create_microsoft_ad(
         self,
         *,
         Name: str,
         Password: str,
-        VpcSettings: DirectoryVpcSettingsUnionTypeDef,
+        VpcSettings: DirectoryVpcSettingsTypeDef,
         ShortName: str = ...,
         Description: str = ...,
         Edition: DirectoryEditionType = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateMicrosoftADResultTypeDef:
         """
         Creates a Microsoft AD directory in the Amazon Web Services Cloud.
@@ -624,15 +624,15 @@
         """
         Activates the switch for the specific directory to always use LDAP secure calls.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_ldaps)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#enable_ldaps)
         """
     async def enable_radius(
-        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsUnionTypeDef
+        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsTypeDef
     ) -> Dict[str, Any]:
         """
         Enables multi-factor authentication (MFA) with the Remote Authentication Dial In
         User Service (RADIUS) server for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.enable_radius)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#enable_radius)
@@ -860,15 +860,15 @@
         """
         Adds or removes domain controllers to or from the directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_number_of_domain_controllers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#update_number_of_domain_controllers)
         """
     async def update_radius(
-        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsUnionTypeDef
+        self, *, DirectoryId: str, RadiusSettings: RadiusSettingsTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the Remote Authentication Dial In User Service (RADIUS) server
         information for an AD Connector or Microsoft AD directory.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ds.html#DirectoryService.Client.update_radius)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ds/client/#update_radius)
```

### Comparing `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/literals.py` & `types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/literals.pyi` & `types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/paginator.py` & `types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/paginator.pyi` & `types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/type_defs.py` & `types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_ds.type_defs import AcceptSharedDirectoryRequestRequestTypeDef
 
     data: AcceptSharedDirectoryRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     CertificateStateType,
     CertificateTypeType,
     ClientAuthenticationStatusType,
     ClientAuthenticationTypeType,
     DirectoryConfigurationStatusType,
@@ -99,25 +99,23 @@
     "DescribeSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
     "DescribeTrustsRequestRequestTypeDef",
     "TrustTypeDef",
     "DescribeUpdateDirectoryRequestRequestTypeDef",
     "DirectoryConnectSettingsDescriptionTypeDef",
     "DirectoryVpcSettingsDescriptionTypeDef",
-    "RadiusSettingsOutputTypeDef",
+    "RadiusSettingsTypeDef",
     "RegionsInfoTypeDef",
     "DirectoryLimitsTypeDef",
-    "DirectoryVpcSettingsOutputTypeDef",
     "DisableClientAuthenticationRequestRequestTypeDef",
     "DisableLDAPSRequestRequestTypeDef",
     "DisableRadiusRequestRequestTypeDef",
     "DisableSsoRequestRequestTypeDef",
     "EnableClientAuthenticationRequestRequestTypeDef",
     "EnableLDAPSRequestRequestTypeDef",
-    "RadiusSettingsTypeDef",
     "EnableSsoRequestRequestTypeDef",
     "GetSnapshotLimitsRequestRequestTypeDef",
     "SnapshotLimitsTypeDef",
     "IpRouteInfoTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListIpRoutesRequestRequestTypeDef",
     "ListLogSubscriptionsRequestRequestTypeDef",
@@ -158,14 +156,15 @@
     "UpdateSettingsResultTypeDef",
     "UpdateTrustResultTypeDef",
     "VerifyTrustResultTypeDef",
     "AcceptSharedDirectoryResultTypeDef",
     "DescribeSharedDirectoriesResultTypeDef",
     "AddIpRoutesRequestRequestTypeDef",
     "AddRegionRequestRequestTypeDef",
+    "RegionDescriptionTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
     "CreateMicrosoftADRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "ComputerTypeDef",
     "CreateComputerRequestRequestTypeDef",
     "ListCertificatesResultTypeDef",
@@ -190,34 +189,31 @@
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeDomainControllersResultTypeDef",
     "DescribeEventTopicsResultTypeDef",
     "DescribeLDAPSSettingsResultTypeDef",
     "DescribeSettingsResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "DescribeTrustsResultTypeDef",
-    "OwnerDirectoryDescriptionTypeDef",
-    "GetDirectoryLimitsResultTypeDef",
-    "DirectoryVpcSettingsUnionTypeDef",
-    "RegionDescriptionTypeDef",
     "EnableRadiusRequestRequestTypeDef",
-    "RadiusSettingsUnionTypeDef",
+    "OwnerDirectoryDescriptionTypeDef",
     "UpdateRadiusRequestRequestTypeDef",
+    "GetDirectoryLimitsResultTypeDef",
     "GetSnapshotLimitsResultTypeDef",
     "ListIpRoutesResultTypeDef",
     "ListLogSubscriptionsResultTypeDef",
     "ListSchemaExtensionsResultTypeDef",
     "UpdateDirectorySetupRequestRequestTypeDef",
     "UpdateValueTypeDef",
     "UpdateSettingsRequestRequestTypeDef",
     "ShareDirectoryRequestRequestTypeDef",
     "UnshareDirectoryRequestRequestTypeDef",
+    "DescribeRegionsResultTypeDef",
     "CreateComputerResultTypeDef",
     "DescribeCertificateResultTypeDef",
     "DirectoryDescriptionTypeDef",
-    "DescribeRegionsResultTypeDef",
     "UpdateInfoEntryTypeDef",
     "DescribeDirectoriesResultTypeDef",
     "DescribeUpdateDirectoryResultTypeDef",
 )
 
 AcceptSharedDirectoryRequestRequestTypeDef = TypedDict(
     "AcceptSharedDirectoryRequestRequestTypeDef",
@@ -836,16 +832,16 @@
         "SubnetIds": List[str],
         "SecurityGroupId": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
-RadiusSettingsOutputTypeDef = TypedDict(
-    "RadiusSettingsOutputTypeDef",
+RadiusSettingsTypeDef = TypedDict(
+    "RadiusSettingsTypeDef",
     {
         "RadiusServers": List[str],
         "RadiusPort": int,
         "RadiusTimeout": int,
         "RadiusRetries": int,
         "SharedSecret": str,
         "AuthenticationProtocol": RadiusAuthenticationProtocolType,
@@ -876,22 +872,14 @@
         "ConnectedDirectoriesLimit": int,
         "ConnectedDirectoriesCurrentCount": int,
         "ConnectedDirectoriesLimitReached": bool,
     },
     total=False,
 )
 
-DirectoryVpcSettingsOutputTypeDef = TypedDict(
-    "DirectoryVpcSettingsOutputTypeDef",
-    {
-        "VpcId": str,
-        "SubnetIds": List[str],
-    },
-)
-
 DisableClientAuthenticationRequestRequestTypeDef = TypedDict(
     "DisableClientAuthenticationRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": ClientAuthenticationTypeType,
     },
 )
@@ -945,29 +933,14 @@
     "EnableLDAPSRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": Literal["Client"],
     },
 )
 
-RadiusSettingsTypeDef = TypedDict(
-    "RadiusSettingsTypeDef",
-    {
-        "RadiusServers": Sequence[str],
-        "RadiusPort": int,
-        "RadiusTimeout": int,
-        "RadiusRetries": int,
-        "SharedSecret": str,
-        "AuthenticationProtocol": RadiusAuthenticationProtocolType,
-        "DisplayLabel": str,
-        "UseSameUsername": bool,
-    },
-    total=False,
-)
-
 _RequiredEnableSsoRequestRequestTypeDef = TypedDict(
     "_RequiredEnableSsoRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalEnableSsoRequestRequestTypeDef = TypedDict(
@@ -1463,14 +1436,30 @@
     {
         "DirectoryId": str,
         "RegionName": str,
         "VPCSettings": DirectoryVpcSettingsTypeDef,
     },
 )
 
+RegionDescriptionTypeDef = TypedDict(
+    "RegionDescriptionTypeDef",
+    {
+        "DirectoryId": str,
+        "RegionName": str,
+        "RegionType": RegionTypeType,
+        "Status": DirectoryStageType,
+        "VpcSettings": DirectoryVpcSettingsTypeDef,
+        "DesiredNumberOfDomainControllers": int,
+        "LaunchTime": datetime,
+        "StatusLastUpdatedDateTime": datetime,
+        "LastUpdatedDateTime": datetime,
+    },
+    total=False,
+)
+
 AddTagsToResourceRequestRequestTypeDef = TypedDict(
     "AddTagsToResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1976,68 +1965,48 @@
     {
         "Trusts": List[TrustTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EnableRadiusRequestRequestTypeDef = TypedDict(
+    "EnableRadiusRequestRequestTypeDef",
+    {
+        "DirectoryId": str,
+        "RadiusSettings": RadiusSettingsTypeDef,
+    },
+)
+
 OwnerDirectoryDescriptionTypeDef = TypedDict(
     "OwnerDirectoryDescriptionTypeDef",
     {
         "DirectoryId": str,
         "AccountId": str,
         "DnsIpAddrs": List[str],
         "VpcSettings": DirectoryVpcSettingsDescriptionTypeDef,
-        "RadiusSettings": RadiusSettingsOutputTypeDef,
+        "RadiusSettings": RadiusSettingsTypeDef,
         "RadiusStatus": RadiusStatusType,
     },
     total=False,
 )
 
-GetDirectoryLimitsResultTypeDef = TypedDict(
-    "GetDirectoryLimitsResultTypeDef",
-    {
-        "DirectoryLimits": DirectoryLimitsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DirectoryVpcSettingsUnionTypeDef = Union[
-    DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef
-]
-RegionDescriptionTypeDef = TypedDict(
-    "RegionDescriptionTypeDef",
-    {
-        "DirectoryId": str,
-        "RegionName": str,
-        "RegionType": RegionTypeType,
-        "Status": DirectoryStageType,
-        "VpcSettings": DirectoryVpcSettingsOutputTypeDef,
-        "DesiredNumberOfDomainControllers": int,
-        "LaunchTime": datetime,
-        "StatusLastUpdatedDateTime": datetime,
-        "LastUpdatedDateTime": datetime,
-    },
-    total=False,
-)
-
-EnableRadiusRequestRequestTypeDef = TypedDict(
-    "EnableRadiusRequestRequestTypeDef",
+UpdateRadiusRequestRequestTypeDef = TypedDict(
+    "UpdateRadiusRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
 
-RadiusSettingsUnionTypeDef = Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
-UpdateRadiusRequestRequestTypeDef = TypedDict(
-    "UpdateRadiusRequestRequestTypeDef",
+GetDirectoryLimitsResultTypeDef = TypedDict(
+    "GetDirectoryLimitsResultTypeDef",
     {
-        "DirectoryId": str,
-        "RadiusSettings": RadiusSettingsTypeDef,
+        "DirectoryLimits": DirectoryLimitsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotLimitsResultTypeDef = TypedDict(
     "GetSnapshotLimitsResultTypeDef",
     {
         "SnapshotLimits": SnapshotLimitsTypeDef,
@@ -2139,14 +2108,23 @@
     "UnshareDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UnshareTarget": UnshareTargetTypeDef,
     },
 )
 
+DescribeRegionsResultTypeDef = TypedDict(
+    "DescribeRegionsResultTypeDef",
+    {
+        "RegionsDescription": List[RegionDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateComputerResultTypeDef = TypedDict(
     "CreateComputerResultTypeDef",
     {
         "Computer": ComputerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2176,35 +2154,26 @@
         "ShareMethod": ShareMethodType,
         "ShareNotes": str,
         "LaunchTime": datetime,
         "StageLastUpdatedDateTime": datetime,
         "Type": DirectoryTypeType,
         "VpcSettings": DirectoryVpcSettingsDescriptionTypeDef,
         "ConnectSettings": DirectoryConnectSettingsDescriptionTypeDef,
-        "RadiusSettings": RadiusSettingsOutputTypeDef,
+        "RadiusSettings": RadiusSettingsTypeDef,
         "RadiusStatus": RadiusStatusType,
         "StageReason": str,
         "SsoEnabled": bool,
         "DesiredNumberOfDomainControllers": int,
         "OwnerDirectoryDescription": OwnerDirectoryDescriptionTypeDef,
         "RegionsInfo": RegionsInfoTypeDef,
         "OsVersion": OSVersionType,
     },
     total=False,
 )
 
-DescribeRegionsResultTypeDef = TypedDict(
-    "DescribeRegionsResultTypeDef",
-    {
-        "RegionsDescription": List[RegionDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateInfoEntryTypeDef = TypedDict(
     "UpdateInfoEntryTypeDef",
     {
         "Region": str,
         "Status": UpdateStatusType,
         "StatusReason": str,
         "InitiatedBy": str,
```

### Comparing `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds/type_defs.pyi` & `types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_ds.type_defs import AcceptSharedDirectoryRequestRequestTypeDef
 
     data: AcceptSharedDirectoryRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     CertificateStateType,
     CertificateTypeType,
     ClientAuthenticationStatusType,
     ClientAuthenticationTypeType,
     DirectoryConfigurationStatusType,
@@ -98,25 +98,23 @@
     "DescribeSnapshotsRequestRequestTypeDef",
     "SnapshotTypeDef",
     "DescribeTrustsRequestRequestTypeDef",
     "TrustTypeDef",
     "DescribeUpdateDirectoryRequestRequestTypeDef",
     "DirectoryConnectSettingsDescriptionTypeDef",
     "DirectoryVpcSettingsDescriptionTypeDef",
-    "RadiusSettingsOutputTypeDef",
+    "RadiusSettingsTypeDef",
     "RegionsInfoTypeDef",
     "DirectoryLimitsTypeDef",
-    "DirectoryVpcSettingsOutputTypeDef",
     "DisableClientAuthenticationRequestRequestTypeDef",
     "DisableLDAPSRequestRequestTypeDef",
     "DisableRadiusRequestRequestTypeDef",
     "DisableSsoRequestRequestTypeDef",
     "EnableClientAuthenticationRequestRequestTypeDef",
     "EnableLDAPSRequestRequestTypeDef",
-    "RadiusSettingsTypeDef",
     "EnableSsoRequestRequestTypeDef",
     "GetSnapshotLimitsRequestRequestTypeDef",
     "SnapshotLimitsTypeDef",
     "IpRouteInfoTypeDef",
     "ListCertificatesRequestRequestTypeDef",
     "ListIpRoutesRequestRequestTypeDef",
     "ListLogSubscriptionsRequestRequestTypeDef",
@@ -157,14 +155,15 @@
     "UpdateSettingsResultTypeDef",
     "UpdateTrustResultTypeDef",
     "VerifyTrustResultTypeDef",
     "AcceptSharedDirectoryResultTypeDef",
     "DescribeSharedDirectoriesResultTypeDef",
     "AddIpRoutesRequestRequestTypeDef",
     "AddRegionRequestRequestTypeDef",
+    "RegionDescriptionTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
     "CreateDirectoryRequestRequestTypeDef",
     "CreateMicrosoftADRequestRequestTypeDef",
     "ListTagsForResourceResultTypeDef",
     "ComputerTypeDef",
     "CreateComputerRequestRequestTypeDef",
     "ListCertificatesResultTypeDef",
@@ -189,34 +188,31 @@
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeDomainControllersResultTypeDef",
     "DescribeEventTopicsResultTypeDef",
     "DescribeLDAPSSettingsResultTypeDef",
     "DescribeSettingsResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "DescribeTrustsResultTypeDef",
-    "OwnerDirectoryDescriptionTypeDef",
-    "GetDirectoryLimitsResultTypeDef",
-    "DirectoryVpcSettingsUnionTypeDef",
-    "RegionDescriptionTypeDef",
     "EnableRadiusRequestRequestTypeDef",
-    "RadiusSettingsUnionTypeDef",
+    "OwnerDirectoryDescriptionTypeDef",
     "UpdateRadiusRequestRequestTypeDef",
+    "GetDirectoryLimitsResultTypeDef",
     "GetSnapshotLimitsResultTypeDef",
     "ListIpRoutesResultTypeDef",
     "ListLogSubscriptionsResultTypeDef",
     "ListSchemaExtensionsResultTypeDef",
     "UpdateDirectorySetupRequestRequestTypeDef",
     "UpdateValueTypeDef",
     "UpdateSettingsRequestRequestTypeDef",
     "ShareDirectoryRequestRequestTypeDef",
     "UnshareDirectoryRequestRequestTypeDef",
+    "DescribeRegionsResultTypeDef",
     "CreateComputerResultTypeDef",
     "DescribeCertificateResultTypeDef",
     "DirectoryDescriptionTypeDef",
-    "DescribeRegionsResultTypeDef",
     "UpdateInfoEntryTypeDef",
     "DescribeDirectoriesResultTypeDef",
     "DescribeUpdateDirectoryResultTypeDef",
 )
 
 AcceptSharedDirectoryRequestRequestTypeDef = TypedDict(
     "AcceptSharedDirectoryRequestRequestTypeDef",
@@ -813,16 +809,16 @@
         "SubnetIds": List[str],
         "SecurityGroupId": str,
         "AvailabilityZones": List[str],
     },
     total=False,
 )
 
-RadiusSettingsOutputTypeDef = TypedDict(
-    "RadiusSettingsOutputTypeDef",
+RadiusSettingsTypeDef = TypedDict(
+    "RadiusSettingsTypeDef",
     {
         "RadiusServers": List[str],
         "RadiusPort": int,
         "RadiusTimeout": int,
         "RadiusRetries": int,
         "SharedSecret": str,
         "AuthenticationProtocol": RadiusAuthenticationProtocolType,
@@ -853,22 +849,14 @@
         "ConnectedDirectoriesLimit": int,
         "ConnectedDirectoriesCurrentCount": int,
         "ConnectedDirectoriesLimitReached": bool,
     },
     total=False,
 )
 
-DirectoryVpcSettingsOutputTypeDef = TypedDict(
-    "DirectoryVpcSettingsOutputTypeDef",
-    {
-        "VpcId": str,
-        "SubnetIds": List[str],
-    },
-)
-
 DisableClientAuthenticationRequestRequestTypeDef = TypedDict(
     "DisableClientAuthenticationRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": ClientAuthenticationTypeType,
     },
 )
@@ -920,29 +908,14 @@
     "EnableLDAPSRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "Type": Literal["Client"],
     },
 )
 
-RadiusSettingsTypeDef = TypedDict(
-    "RadiusSettingsTypeDef",
-    {
-        "RadiusServers": Sequence[str],
-        "RadiusPort": int,
-        "RadiusTimeout": int,
-        "RadiusRetries": int,
-        "SharedSecret": str,
-        "AuthenticationProtocol": RadiusAuthenticationProtocolType,
-        "DisplayLabel": str,
-        "UseSameUsername": bool,
-    },
-    total=False,
-)
-
 _RequiredEnableSsoRequestRequestTypeDef = TypedDict(
     "_RequiredEnableSsoRequestRequestTypeDef",
     {
         "DirectoryId": str,
     },
 )
 _OptionalEnableSsoRequestRequestTypeDef = TypedDict(
@@ -1424,14 +1397,30 @@
     {
         "DirectoryId": str,
         "RegionName": str,
         "VPCSettings": DirectoryVpcSettingsTypeDef,
     },
 )
 
+RegionDescriptionTypeDef = TypedDict(
+    "RegionDescriptionTypeDef",
+    {
+        "DirectoryId": str,
+        "RegionName": str,
+        "RegionType": RegionTypeType,
+        "Status": DirectoryStageType,
+        "VpcSettings": DirectoryVpcSettingsTypeDef,
+        "DesiredNumberOfDomainControllers": int,
+        "LaunchTime": datetime,
+        "StatusLastUpdatedDateTime": datetime,
+        "LastUpdatedDateTime": datetime,
+    },
+    total=False,
+)
+
 AddTagsToResourceRequestRequestTypeDef = TypedDict(
     "AddTagsToResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1907,68 +1896,48 @@
     {
         "Trusts": List[TrustTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EnableRadiusRequestRequestTypeDef = TypedDict(
+    "EnableRadiusRequestRequestTypeDef",
+    {
+        "DirectoryId": str,
+        "RadiusSettings": RadiusSettingsTypeDef,
+    },
+)
+
 OwnerDirectoryDescriptionTypeDef = TypedDict(
     "OwnerDirectoryDescriptionTypeDef",
     {
         "DirectoryId": str,
         "AccountId": str,
         "DnsIpAddrs": List[str],
         "VpcSettings": DirectoryVpcSettingsDescriptionTypeDef,
-        "RadiusSettings": RadiusSettingsOutputTypeDef,
+        "RadiusSettings": RadiusSettingsTypeDef,
         "RadiusStatus": RadiusStatusType,
     },
     total=False,
 )
 
-GetDirectoryLimitsResultTypeDef = TypedDict(
-    "GetDirectoryLimitsResultTypeDef",
-    {
-        "DirectoryLimits": DirectoryLimitsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DirectoryVpcSettingsUnionTypeDef = Union[
-    DirectoryVpcSettingsTypeDef, DirectoryVpcSettingsOutputTypeDef
-]
-RegionDescriptionTypeDef = TypedDict(
-    "RegionDescriptionTypeDef",
-    {
-        "DirectoryId": str,
-        "RegionName": str,
-        "RegionType": RegionTypeType,
-        "Status": DirectoryStageType,
-        "VpcSettings": DirectoryVpcSettingsOutputTypeDef,
-        "DesiredNumberOfDomainControllers": int,
-        "LaunchTime": datetime,
-        "StatusLastUpdatedDateTime": datetime,
-        "LastUpdatedDateTime": datetime,
-    },
-    total=False,
-)
-
-EnableRadiusRequestRequestTypeDef = TypedDict(
-    "EnableRadiusRequestRequestTypeDef",
+UpdateRadiusRequestRequestTypeDef = TypedDict(
+    "UpdateRadiusRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "RadiusSettings": RadiusSettingsTypeDef,
     },
 )
 
-RadiusSettingsUnionTypeDef = Union[RadiusSettingsTypeDef, RadiusSettingsOutputTypeDef]
-UpdateRadiusRequestRequestTypeDef = TypedDict(
-    "UpdateRadiusRequestRequestTypeDef",
+GetDirectoryLimitsResultTypeDef = TypedDict(
+    "GetDirectoryLimitsResultTypeDef",
     {
-        "DirectoryId": str,
-        "RadiusSettings": RadiusSettingsTypeDef,
+        "DirectoryLimits": DirectoryLimitsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSnapshotLimitsResultTypeDef = TypedDict(
     "GetSnapshotLimitsResultTypeDef",
     {
         "SnapshotLimits": SnapshotLimitsTypeDef,
@@ -2066,14 +2035,23 @@
     "UnshareDirectoryRequestRequestTypeDef",
     {
         "DirectoryId": str,
         "UnshareTarget": UnshareTargetTypeDef,
     },
 )
 
+DescribeRegionsResultTypeDef = TypedDict(
+    "DescribeRegionsResultTypeDef",
+    {
+        "RegionsDescription": List[RegionDescriptionTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateComputerResultTypeDef = TypedDict(
     "CreateComputerResultTypeDef",
     {
         "Computer": ComputerTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -2103,35 +2081,26 @@
         "ShareMethod": ShareMethodType,
         "ShareNotes": str,
         "LaunchTime": datetime,
         "StageLastUpdatedDateTime": datetime,
         "Type": DirectoryTypeType,
         "VpcSettings": DirectoryVpcSettingsDescriptionTypeDef,
         "ConnectSettings": DirectoryConnectSettingsDescriptionTypeDef,
-        "RadiusSettings": RadiusSettingsOutputTypeDef,
+        "RadiusSettings": RadiusSettingsTypeDef,
         "RadiusStatus": RadiusStatusType,
         "StageReason": str,
         "SsoEnabled": bool,
         "DesiredNumberOfDomainControllers": int,
         "OwnerDirectoryDescription": OwnerDirectoryDescriptionTypeDef,
         "RegionsInfo": RegionsInfoTypeDef,
         "OsVersion": OSVersionType,
     },
     total=False,
 )
 
-DescribeRegionsResultTypeDef = TypedDict(
-    "DescribeRegionsResultTypeDef",
-    {
-        "RegionsDescription": List[RegionDescriptionTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 UpdateInfoEntryTypeDef = TypedDict(
     "UpdateInfoEntryTypeDef",
     {
         "Region": str,
         "Status": UpdateStatusType,
         "StatusReason": str,
         "InitiatedBy": str,
```

### Comparing `types-aiobotocore-ds-2.5.2.post1/types_aiobotocore_ds.egg-info/SOURCES.txt` & `types-aiobotocore-ds-2.5.2.post2/types_aiobotocore_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

