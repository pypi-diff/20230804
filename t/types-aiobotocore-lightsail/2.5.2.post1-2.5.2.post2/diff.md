# Comparing `tmp/types-aiobotocore-lightsail-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-lightsail-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lightsail-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-lightsail-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
```

## Comparing `types-aiobotocore-lightsail-2.5.2.post1.tar` & `types-aiobotocore-lightsail-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.397535 types-aiobotocore-lightsail-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:18.000000 types-aiobotocore-lightsail-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37239 2023-08-02 14:52:35.397535 types-aiobotocore-lightsail-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35713 2023-08-02 14:42:18.000000 types-aiobotocore-lightsail-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:35.397535 types-aiobotocore-lightsail-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:42:18.000000 types-aiobotocore-lightsail-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.397535 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-08-02 14:42:18.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-08-02 14:42:18.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:42:18.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   119308 2023-08-02 14:42:19.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   119120 2023-08-02 14:42:19.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    25240 2023-08-02 14:42:20.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    25238 2023-08-02 14:42:20.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23981 2023-08-02 14:42:19.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    23958 2023-08-02 14:42:19.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:18.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   148323 2023-08-02 14:42:25.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   148224 2023-08-02 14:42:21.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:18.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.397535 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37239 2023-08-02 14:52:35.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:35.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:35.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:35.000000 types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.606643 types-aiobotocore-lightsail-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:06.000000 types-aiobotocore-lightsail-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16026 2023-08-04 13:59:15.606643 types-aiobotocore-lightsail-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14500 2023-08-04 13:43:06.000000 types-aiobotocore-lightsail-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.606643 types-aiobotocore-lightsail-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:43:06.000000 types-aiobotocore-lightsail-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.606643 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4923 2023-08-04 13:43:06.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     4922 2023-08-04 13:43:06.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:43:06.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   119263 2023-08-04 13:43:08.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   119075 2023-08-04 13:43:08.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25335 2023-08-04 13:43:09.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    25333 2023-08-04 13:43:08.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    23981 2023-08-04 13:43:08.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    23958 2023-08-04 13:43:08.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:06.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   146290 2023-08-04 13:43:13.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   146191 2023-08-04 13:43:11.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:06.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.606643 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    16026 2023-08-04 13:59:15.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-08-04 13:59:15.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:15.000000 types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/LICENSE` & `types-aiobotocore-lightsail-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/setup.py` & `types-aiobotocore-lightsail-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lightsail",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_lightsail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Lightsail 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/__init__.py` & `types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/__init__.pyi` & `types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/__main__.py` & `types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Lightsail 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Lightsail 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail\nOther"
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

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/client.py` & `types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,19 +78,19 @@
     AttachDiskResultTypeDef,
     AttachInstancesToLoadBalancerResultTypeDef,
     AttachLoadBalancerTlsCertificateResultTypeDef,
     AttachStaticIpResultTypeDef,
     BucketAccessLogConfigTypeDef,
     CacheBehaviorPerPathTypeDef,
     CacheBehaviorTypeDef,
-    CacheSettingsUnionTypeDef,
+    CacheSettingsTypeDef,
     CloseInstancePublicPortsResultTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     ContainerServicesListResultTypeDef,
-    ContainerUnionTypeDef,
+    ContainerTypeDef,
     CopySnapshotResultTypeDef,
     CreateBucketAccessKeyResultTypeDef,
     CreateBucketResultTypeDef,
     CreateCertificateResultTypeDef,
     CreateCloudFormationStackResultTypeDef,
     CreateContactMethodResultTypeDef,
     CreateContainerServiceDeploymentResultTypeDef,
@@ -133,15 +133,15 @@
     DeleteRelationalDatabaseSnapshotResultTypeDef,
     DetachCertificateFromDistributionResultTypeDef,
     DetachDiskResultTypeDef,
     DetachInstancesFromLoadBalancerResultTypeDef,
     DetachStaticIpResultTypeDef,
     DisableAddOnResultTypeDef,
     DiskMapTypeDef,
-    DomainEntryUnionTypeDef,
+    DomainEntryTypeDef,
     DownloadDefaultKeyPairResultTypeDef,
     EnableAddOnResultTypeDef,
     EndpointRequestTypeDef,
     ExportSnapshotResultTypeDef,
     GetActiveNamesResultTypeDef,
     GetAlarmsResultTypeDef,
     GetAutoSnapshotsResultTypeDef,
@@ -477,15 +477,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_container_service)
         """
 
     async def create_container_service_deployment(
         self,
         *,
         serviceName: str,
-        containers: Mapping[str, ContainerUnionTypeDef] = ...,
+        containers: Mapping[str, ContainerTypeDef] = ...,
         publicEndpoint: EndpointRequestTypeDef = ...
     ) -> CreateContainerServiceDeploymentResultTypeDef:
         """
         Creates a deployment for your Amazon Lightsail container service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_container_service_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_container_service_deployment)
@@ -557,15 +557,15 @@
     async def create_distribution(
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef,
         defaultCacheBehavior: CacheBehaviorTypeDef,
         bundleId: str,
-        cacheBehaviorSettings: CacheSettingsUnionTypeDef = ...,
+        cacheBehaviorSettings: CacheSettingsTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDistributionResultTypeDef:
         """
         Creates an Amazon Lightsail content delivery network (CDN) distribution.
 
@@ -580,15 +580,15 @@
         Creates a domain resource for the specified domain (e.g., example.com).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_domain)
         """
 
     async def create_domain_entry(
-        self, *, domainName: str, domainEntry: DomainEntryUnionTypeDef
+        self, *, domainName: str, domainEntry: DomainEntryTypeDef
     ) -> CreateDomainEntryResultTypeDef:
         """
         Creates one of the following domain name system (DNS) records in a domain DNS
         zone: Address (A), canonical name (CNAME), mail exchanger (MX), name server
         (NS), start of authority (SOA), service locator (SRV), or text (TXT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain_entry)
@@ -874,15 +874,15 @@
         Deletes the specified domain recordset and all of its domain records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#delete_domain)
         """
 
     async def delete_domain_entry(
-        self, *, domainName: str, domainEntry: DomainEntryUnionTypeDef
+        self, *, domainName: str, domainEntry: DomainEntryTypeDef
     ) -> DeleteDomainEntryResultTypeDef:
         """
         Deletes a specific domain entry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_domain_entry)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#delete_domain_entry)
         """
@@ -2053,15 +2053,15 @@
 
     async def update_distribution(
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef = ...,
         defaultCacheBehavior: CacheBehaviorTypeDef = ...,
-        cacheBehaviorSettings: CacheSettingsUnionTypeDef = ...,
+        cacheBehaviorSettings: CacheSettingsTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         isEnabled: bool = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates an existing Amazon Lightsail content delivery network (CDN)
         distribution.
 
@@ -2077,15 +2077,15 @@
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_distribution_bundle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_distribution_bundle)
         """
 
     async def update_domain_entry(
-        self, *, domainName: str, domainEntry: DomainEntryUnionTypeDef
+        self, *, domainName: str, domainEntry: DomainEntryTypeDef
     ) -> UpdateDomainEntryResultTypeDef:
         """
         Updates a domain recordset after it is created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_domain_entry)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_domain_entry)
         """
```

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/client.pyi` & `types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -78,19 +78,19 @@
     AttachDiskResultTypeDef,
     AttachInstancesToLoadBalancerResultTypeDef,
     AttachLoadBalancerTlsCertificateResultTypeDef,
     AttachStaticIpResultTypeDef,
     BucketAccessLogConfigTypeDef,
     CacheBehaviorPerPathTypeDef,
     CacheBehaviorTypeDef,
-    CacheSettingsUnionTypeDef,
+    CacheSettingsTypeDef,
     CloseInstancePublicPortsResultTypeDef,
     ContainerServiceDeploymentRequestTypeDef,
     ContainerServicesListResultTypeDef,
-    ContainerUnionTypeDef,
+    ContainerTypeDef,
     CopySnapshotResultTypeDef,
     CreateBucketAccessKeyResultTypeDef,
     CreateBucketResultTypeDef,
     CreateCertificateResultTypeDef,
     CreateCloudFormationStackResultTypeDef,
     CreateContactMethodResultTypeDef,
     CreateContainerServiceDeploymentResultTypeDef,
@@ -133,15 +133,15 @@
     DeleteRelationalDatabaseSnapshotResultTypeDef,
     DetachCertificateFromDistributionResultTypeDef,
     DetachDiskResultTypeDef,
     DetachInstancesFromLoadBalancerResultTypeDef,
     DetachStaticIpResultTypeDef,
     DisableAddOnResultTypeDef,
     DiskMapTypeDef,
-    DomainEntryUnionTypeDef,
+    DomainEntryTypeDef,
     DownloadDefaultKeyPairResultTypeDef,
     EnableAddOnResultTypeDef,
     EndpointRequestTypeDef,
     ExportSnapshotResultTypeDef,
     GetActiveNamesResultTypeDef,
     GetAlarmsResultTypeDef,
     GetAutoSnapshotsResultTypeDef,
@@ -456,15 +456,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_container_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_container_service)
         """
     async def create_container_service_deployment(
         self,
         *,
         serviceName: str,
-        containers: Mapping[str, ContainerUnionTypeDef] = ...,
+        containers: Mapping[str, ContainerTypeDef] = ...,
         publicEndpoint: EndpointRequestTypeDef = ...
     ) -> CreateContainerServiceDeploymentResultTypeDef:
         """
         Creates a deployment for your Amazon Lightsail container service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_container_service_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_container_service_deployment)
@@ -531,15 +531,15 @@
     async def create_distribution(
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef,
         defaultCacheBehavior: CacheBehaviorTypeDef,
         bundleId: str,
-        cacheBehaviorSettings: CacheSettingsUnionTypeDef = ...,
+        cacheBehaviorSettings: CacheSettingsTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         ipAddressType: IpAddressTypeType = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateDistributionResultTypeDef:
         """
         Creates an Amazon Lightsail content delivery network (CDN) distribution.
 
@@ -552,15 +552,15 @@
         """
         Creates a domain resource for the specified domain (e.g., example.com).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#create_domain)
         """
     async def create_domain_entry(
-        self, *, domainName: str, domainEntry: DomainEntryUnionTypeDef
+        self, *, domainName: str, domainEntry: DomainEntryTypeDef
     ) -> CreateDomainEntryResultTypeDef:
         """
         Creates one of the following domain name system (DNS) records in a domain DNS
         zone: Address (A), canonical name (CNAME), mail exchanger (MX), name server
         (NS), start of authority (SOA), service locator (SRV), or text (TXT).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.create_domain_entry)
@@ -823,15 +823,15 @@
         """
         Deletes the specified domain recordset and all of its domain records.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#delete_domain)
         """
     async def delete_domain_entry(
-        self, *, domainName: str, domainEntry: DomainEntryUnionTypeDef
+        self, *, domainName: str, domainEntry: DomainEntryTypeDef
     ) -> DeleteDomainEntryResultTypeDef:
         """
         Deletes a specific domain entry.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.delete_domain_entry)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#delete_domain_entry)
         """
@@ -1893,15 +1893,15 @@
         """
     async def update_distribution(
         self,
         *,
         distributionName: str,
         origin: InputOriginTypeDef = ...,
         defaultCacheBehavior: CacheBehaviorTypeDef = ...,
-        cacheBehaviorSettings: CacheSettingsUnionTypeDef = ...,
+        cacheBehaviorSettings: CacheSettingsTypeDef = ...,
         cacheBehaviors: Sequence[CacheBehaviorPerPathTypeDef] = ...,
         isEnabled: bool = ...
     ) -> UpdateDistributionResultTypeDef:
         """
         Updates an existing Amazon Lightsail content delivery network (CDN)
         distribution.
 
@@ -1915,15 +1915,15 @@
         Updates the bundle of your Amazon Lightsail content delivery network (CDN)
         distribution.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_distribution_bundle)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_distribution_bundle)
         """
     async def update_domain_entry(
-        self, *, domainName: str, domainEntry: DomainEntryUnionTypeDef
+        self, *, domainName: str, domainEntry: DomainEntryTypeDef
     ) -> UpdateDomainEntryResultTypeDef:
         """
         Updates a domain recordset after it is created.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lightsail.html#Lightsail.Client.update_domain_entry)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lightsail/client/#update_domain_entry)
         """
```

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/literals.py` & `types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -549,14 +549,15 @@
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
@@ -652,14 +653,15 @@
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
@@ -738,26 +740,28 @@
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

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/literals.pyi` & `types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -547,14 +547,15 @@
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
@@ -650,14 +651,15 @@
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
@@ -736,26 +738,28 @@
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

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/paginator.py` & `types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/paginator.pyi` & `types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/type_defs.py` & `types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,25 +124,21 @@
     "BucketBundleTypeDef",
     "BucketStateTypeDef",
     "ResourceReceivingAccessTypeDef",
     "TagTypeDef",
     "BundleTypeDef",
     "CacheBehaviorPerPathTypeDef",
     "CacheBehaviorTypeDef",
-    "CookieObjectOutputTypeDef",
-    "HeaderObjectOutputTypeDef",
-    "QueryStringObjectOutputTypeDef",
     "CookieObjectTypeDef",
     "HeaderObjectTypeDef",
     "QueryStringObjectTypeDef",
     "PortInfoTypeDef",
     "CloudFormationStackRecordSourceInfoTypeDef",
     "DestinationInfoTypeDef",
     "ContainerImageTypeDef",
-    "ContainerOutputTypeDef",
     "ContainerTypeDef",
     "ContainerServiceECRImagePullerRoleRequestTypeDef",
     "ContainerServiceECRImagePullerRoleTypeDef",
     "ContainerServiceHealthCheckConfigTypeDef",
     "ContainerServiceLogEventTypeDef",
     "ContainerServicePowerTypeDef",
     "ContainerServiceRegistryLoginTypeDef",
@@ -182,15 +178,14 @@
     "DetachInstancesFromLoadBalancerRequestRequestTypeDef",
     "DetachStaticIpRequestRequestTypeDef",
     "DisableAddOnRequestRequestTypeDef",
     "DiskInfoTypeDef",
     "DiskSnapshotInfoTypeDef",
     "DistributionBundleTypeDef",
     "DnsRecordCreationStateTypeDef",
-    "DomainEntryOutputTypeDef",
     "ResourceRecordTypeDef",
     "TimePeriodTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetActiveNamesRequestRequestTypeDef",
     "GetAlarmsRequestRequestTypeDef",
     "GetAutoSnapshotsRequestRequestTypeDef",
@@ -322,23 +317,21 @@
     "CreateRelationalDatabaseSnapshotRequestRequestTypeDef",
     "DiskSnapshotTypeDef",
     "DiskTypeDef",
     "KeyPairTypeDef",
     "RelationalDatabaseSnapshotTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetBundlesResultTypeDef",
-    "CacheSettingsOutputTypeDef",
     "CacheSettingsTypeDef",
     "CloseInstancePublicPortsRequestRequestTypeDef",
     "OpenInstancePublicPortsRequestRequestTypeDef",
     "PutInstancePublicPortsRequestRequestTypeDef",
     "CloudFormationStackRecordTypeDef",
     "GetContainerImagesResultTypeDef",
     "RegisterContainerImageResultTypeDef",
-    "ContainerUnionTypeDef",
     "PrivateRegistryAccessRequestTypeDef",
     "PrivateRegistryAccessTypeDef",
     "ContainerServiceEndpointTypeDef",
     "EndpointRequestTypeDef",
     "GetContainerLogResultTypeDef",
     "GetContainerServicePowersResultTypeDef",
     "CreateContainerServiceRegistryLoginResultTypeDef",
@@ -355,15 +348,14 @@
     "GetDistributionMetricDataRequestRequestTypeDef",
     "GetInstanceMetricDataRequestRequestTypeDef",
     "GetLoadBalancerMetricDataRequestRequestTypeDef",
     "GetRelationalDatabaseLogEventsRequestRequestTypeDef",
     "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
     "InstanceSnapshotInfoTypeDef",
     "GetDistributionBundlesResultTypeDef",
-    "DomainEntryUnionTypeDef",
     "DomainValidationRecordTypeDef",
     "EstimateByTimeTypeDef",
     "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
     "GetBundlesRequestGetBundlesPaginateTypeDef",
     "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
     "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
@@ -509,17 +501,16 @@
     "InstanceHardwareTypeDef",
     "InstanceSnapshotTypeDef",
     "CreateKeyPairResultTypeDef",
     "GetKeyPairResultTypeDef",
     "GetKeyPairsResultTypeDef",
     "GetRelationalDatabaseSnapshotResultTypeDef",
     "GetRelationalDatabaseSnapshotsResultTypeDef",
-    "LightsailDistributionTypeDef",
-    "CacheSettingsUnionTypeDef",
     "CreateDistributionRequestRequestTypeDef",
+    "LightsailDistributionTypeDef",
     "UpdateDistributionRequestRequestTypeDef",
     "GetCloudFormationStackRecordsResultTypeDef",
     "UpdateContainerServiceRequestRequestTypeDef",
     "ContainerServiceDeploymentTypeDef",
     "ContainerServiceDeploymentRequestTypeDef",
     "CreateContainerServiceDeploymentRequestRequestTypeDef",
     "ExportSnapshotRecordSourceInfoTypeDef",
@@ -843,41 +834,14 @@
     "CacheBehaviorTypeDef",
     {
         "behavior": BehaviorEnumType,
     },
     total=False,
 )
 
-CookieObjectOutputTypeDef = TypedDict(
-    "CookieObjectOutputTypeDef",
-    {
-        "option": ForwardValuesType,
-        "cookiesAllowList": List[str],
-    },
-    total=False,
-)
-
-HeaderObjectOutputTypeDef = TypedDict(
-    "HeaderObjectOutputTypeDef",
-    {
-        "option": ForwardValuesType,
-        "headersAllowList": List[HeaderEnumType],
-    },
-    total=False,
-)
-
-QueryStringObjectOutputTypeDef = TypedDict(
-    "QueryStringObjectOutputTypeDef",
-    {
-        "option": bool,
-        "queryStringsAllowList": List[str],
-    },
-    total=False,
-)
-
 CookieObjectTypeDef = TypedDict(
     "CookieObjectTypeDef",
     {
         "option": ForwardValuesType,
         "cookiesAllowList": Sequence[str],
     },
     total=False,
@@ -939,25 +903,14 @@
         "image": str,
         "digest": str,
         "createdAt": datetime,
     },
     total=False,
 )
 
-ContainerOutputTypeDef = TypedDict(
-    "ContainerOutputTypeDef",
-    {
-        "image": str,
-        "command": List[str],
-        "environment": Dict[str, str],
-        "ports": Dict[str, ContainerServiceProtocolType],
-    },
-    total=False,
-)
-
 ContainerTypeDef = TypedDict(
     "ContainerTypeDef",
     {
         "image": str,
         "command": Sequence[str],
         "environment": Mapping[str, str],
         "ports": Mapping[str, ContainerServiceProtocolType],
@@ -1454,27 +1407,14 @@
     {
         "code": DnsRecordCreationStateCodeType,
         "message": str,
     },
     total=False,
 )
 
-DomainEntryOutputTypeDef = TypedDict(
-    "DomainEntryOutputTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "target": str,
-        "isAlias": bool,
-        "type": str,
-        "options": Dict[str, str],
-    },
-    total=False,
-)
-
 ResourceRecordTypeDef = TypedDict(
     "ResourceRecordTypeDef",
     {
         "name": str,
         "type": str,
         "value": str,
     },
@@ -3164,29 +3104,14 @@
     {
         "bundles": List[BundleTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CacheSettingsOutputTypeDef = TypedDict(
-    "CacheSettingsOutputTypeDef",
-    {
-        "defaultTTL": int,
-        "minimumTTL": int,
-        "maximumTTL": int,
-        "allowedHTTPMethods": str,
-        "cachedHTTPMethods": str,
-        "forwardedCookies": CookieObjectOutputTypeDef,
-        "forwardedHeaders": HeaderObjectOutputTypeDef,
-        "forwardedQueryStrings": QueryStringObjectOutputTypeDef,
-    },
-    total=False,
-)
-
 CacheSettingsTypeDef = TypedDict(
     "CacheSettingsTypeDef",
     {
         "defaultTTL": int,
         "minimumTTL": int,
         "maximumTTL": int,
         "allowedHTTPMethods": str,
@@ -3249,15 +3174,14 @@
     "RegisterContainerImageResultTypeDef",
     {
         "containerImage": ContainerImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ContainerUnionTypeDef = Union[ContainerTypeDef, ContainerOutputTypeDef]
 PrivateRegistryAccessRequestTypeDef = TypedDict(
     "PrivateRegistryAccessRequestTypeDef",
     {
         "ecrImagePullerRole": ContainerServiceECRImagePullerRoleRequestTypeDef,
     },
     total=False,
 )
@@ -3548,15 +3472,14 @@
     "GetDistributionBundlesResultTypeDef",
     {
         "bundles": List[DistributionBundleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DomainEntryUnionTypeDef = Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
 DomainValidationRecordTypeDef = TypedDict(
     "DomainValidationRecordTypeDef",
     {
         "domainName": str,
         "resourceRecord": ResourceRecordTypeDef,
         "dnsRecordCreationState": DnsRecordCreationStateTypeDef,
         "validationStatus": CertificateDomainValidationStatusType,
@@ -5009,42 +4932,14 @@
     {
         "relationalDatabaseSnapshots": List[RelationalDatabaseSnapshotTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LightsailDistributionTypeDef = TypedDict(
-    "LightsailDistributionTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "alternativeDomainNames": List[str],
-        "status": str,
-        "isEnabled": bool,
-        "domainName": str,
-        "bundleId": str,
-        "certificateName": str,
-        "origin": OriginTypeDef,
-        "originPublicDNS": str,
-        "defaultCacheBehavior": CacheBehaviorTypeDef,
-        "cacheBehaviorSettings": CacheSettingsOutputTypeDef,
-        "cacheBehaviors": List[CacheBehaviorPerPathTypeDef],
-        "ableToUpdateBundle": bool,
-        "ipAddressType": IpAddressTypeType,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-CacheSettingsUnionTypeDef = Union[CacheSettingsTypeDef, CacheSettingsOutputTypeDef]
 _RequiredCreateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "origin": InputOriginTypeDef,
         "defaultCacheBehavior": CacheBehaviorTypeDef,
         "bundleId": str,
@@ -5065,14 +4960,41 @@
 class CreateDistributionRequestRequestTypeDef(
     _RequiredCreateDistributionRequestRequestTypeDef,
     _OptionalCreateDistributionRequestRequestTypeDef,
 ):
     pass
 
 
+LightsailDistributionTypeDef = TypedDict(
+    "LightsailDistributionTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "alternativeDomainNames": List[str],
+        "status": str,
+        "isEnabled": bool,
+        "domainName": str,
+        "bundleId": str,
+        "certificateName": str,
+        "origin": OriginTypeDef,
+        "originPublicDNS": str,
+        "defaultCacheBehavior": CacheBehaviorTypeDef,
+        "cacheBehaviorSettings": CacheSettingsTypeDef,
+        "cacheBehaviors": List[CacheBehaviorPerPathTypeDef],
+        "ableToUpdateBundle": bool,
+        "ipAddressType": IpAddressTypeType,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
     },
 )
 _OptionalUpdateDistributionRequestRequestTypeDef = TypedDict(
@@ -5131,15 +5053,15 @@
 
 
 ContainerServiceDeploymentTypeDef = TypedDict(
     "ContainerServiceDeploymentTypeDef",
     {
         "version": int,
         "state": ContainerServiceDeploymentStateType,
-        "containers": Dict[str, ContainerOutputTypeDef],
+        "containers": Dict[str, ContainerTypeDef],
         "publicEndpoint": ContainerServiceEndpointTypeDef,
         "createdAt": datetime,
     },
     total=False,
 )
 
 ContainerServiceDeploymentRequestTypeDef = TypedDict(
@@ -5156,15 +5078,15 @@
     {
         "serviceName": str,
     },
 )
 _OptionalCreateContainerServiceDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerServiceDeploymentRequestRequestTypeDef",
     {
-        "containers": Mapping[str, ContainerUnionTypeDef],
+        "containers": Mapping[str, ContainerTypeDef],
         "publicEndpoint": EndpointRequestTypeDef,
     },
     total=False,
 )
 
 
 class CreateContainerServiceDeploymentRequestRequestTypeDef(
@@ -5272,15 +5194,15 @@
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
         "tags": List[TagTypeDef],
-        "domainEntries": List[DomainEntryOutputTypeDef],
+        "domainEntries": List[DomainEntryTypeDef],
         "registeredDomainDelegationInfo": RegisteredDomainDelegationInfoTypeDef,
     },
     total=False,
 )
 
 GetRelationalDatabaseResultTypeDef = TypedDict(
     "GetRelationalDatabaseResultTypeDef",
```

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail/type_defs.pyi` & `types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -123,25 +123,21 @@
     "BucketBundleTypeDef",
     "BucketStateTypeDef",
     "ResourceReceivingAccessTypeDef",
     "TagTypeDef",
     "BundleTypeDef",
     "CacheBehaviorPerPathTypeDef",
     "CacheBehaviorTypeDef",
-    "CookieObjectOutputTypeDef",
-    "HeaderObjectOutputTypeDef",
-    "QueryStringObjectOutputTypeDef",
     "CookieObjectTypeDef",
     "HeaderObjectTypeDef",
     "QueryStringObjectTypeDef",
     "PortInfoTypeDef",
     "CloudFormationStackRecordSourceInfoTypeDef",
     "DestinationInfoTypeDef",
     "ContainerImageTypeDef",
-    "ContainerOutputTypeDef",
     "ContainerTypeDef",
     "ContainerServiceECRImagePullerRoleRequestTypeDef",
     "ContainerServiceECRImagePullerRoleTypeDef",
     "ContainerServiceHealthCheckConfigTypeDef",
     "ContainerServiceLogEventTypeDef",
     "ContainerServicePowerTypeDef",
     "ContainerServiceRegistryLoginTypeDef",
@@ -181,15 +177,14 @@
     "DetachInstancesFromLoadBalancerRequestRequestTypeDef",
     "DetachStaticIpRequestRequestTypeDef",
     "DisableAddOnRequestRequestTypeDef",
     "DiskInfoTypeDef",
     "DiskSnapshotInfoTypeDef",
     "DistributionBundleTypeDef",
     "DnsRecordCreationStateTypeDef",
-    "DomainEntryOutputTypeDef",
     "ResourceRecordTypeDef",
     "TimePeriodTypeDef",
     "ExportSnapshotRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetActiveNamesRequestRequestTypeDef",
     "GetAlarmsRequestRequestTypeDef",
     "GetAutoSnapshotsRequestRequestTypeDef",
@@ -321,23 +316,21 @@
     "CreateRelationalDatabaseSnapshotRequestRequestTypeDef",
     "DiskSnapshotTypeDef",
     "DiskTypeDef",
     "KeyPairTypeDef",
     "RelationalDatabaseSnapshotTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetBundlesResultTypeDef",
-    "CacheSettingsOutputTypeDef",
     "CacheSettingsTypeDef",
     "CloseInstancePublicPortsRequestRequestTypeDef",
     "OpenInstancePublicPortsRequestRequestTypeDef",
     "PutInstancePublicPortsRequestRequestTypeDef",
     "CloudFormationStackRecordTypeDef",
     "GetContainerImagesResultTypeDef",
     "RegisterContainerImageResultTypeDef",
-    "ContainerUnionTypeDef",
     "PrivateRegistryAccessRequestTypeDef",
     "PrivateRegistryAccessTypeDef",
     "ContainerServiceEndpointTypeDef",
     "EndpointRequestTypeDef",
     "GetContainerLogResultTypeDef",
     "GetContainerServicePowersResultTypeDef",
     "CreateContainerServiceRegistryLoginResultTypeDef",
@@ -354,15 +347,14 @@
     "GetDistributionMetricDataRequestRequestTypeDef",
     "GetInstanceMetricDataRequestRequestTypeDef",
     "GetLoadBalancerMetricDataRequestRequestTypeDef",
     "GetRelationalDatabaseLogEventsRequestRequestTypeDef",
     "GetRelationalDatabaseMetricDataRequestRequestTypeDef",
     "InstanceSnapshotInfoTypeDef",
     "GetDistributionBundlesResultTypeDef",
-    "DomainEntryUnionTypeDef",
     "DomainValidationRecordTypeDef",
     "EstimateByTimeTypeDef",
     "GetActiveNamesRequestGetActiveNamesPaginateTypeDef",
     "GetBlueprintsRequestGetBlueprintsPaginateTypeDef",
     "GetBundlesRequestGetBundlesPaginateTypeDef",
     "GetCloudFormationStackRecordsRequestGetCloudFormationStackRecordsPaginateTypeDef",
     "GetDiskSnapshotsRequestGetDiskSnapshotsPaginateTypeDef",
@@ -508,17 +500,16 @@
     "InstanceHardwareTypeDef",
     "InstanceSnapshotTypeDef",
     "CreateKeyPairResultTypeDef",
     "GetKeyPairResultTypeDef",
     "GetKeyPairsResultTypeDef",
     "GetRelationalDatabaseSnapshotResultTypeDef",
     "GetRelationalDatabaseSnapshotsResultTypeDef",
-    "LightsailDistributionTypeDef",
-    "CacheSettingsUnionTypeDef",
     "CreateDistributionRequestRequestTypeDef",
+    "LightsailDistributionTypeDef",
     "UpdateDistributionRequestRequestTypeDef",
     "GetCloudFormationStackRecordsResultTypeDef",
     "UpdateContainerServiceRequestRequestTypeDef",
     "ContainerServiceDeploymentTypeDef",
     "ContainerServiceDeploymentRequestTypeDef",
     "CreateContainerServiceDeploymentRequestRequestTypeDef",
     "ExportSnapshotRecordSourceInfoTypeDef",
@@ -838,41 +829,14 @@
     "CacheBehaviorTypeDef",
     {
         "behavior": BehaviorEnumType,
     },
     total=False,
 )
 
-CookieObjectOutputTypeDef = TypedDict(
-    "CookieObjectOutputTypeDef",
-    {
-        "option": ForwardValuesType,
-        "cookiesAllowList": List[str],
-    },
-    total=False,
-)
-
-HeaderObjectOutputTypeDef = TypedDict(
-    "HeaderObjectOutputTypeDef",
-    {
-        "option": ForwardValuesType,
-        "headersAllowList": List[HeaderEnumType],
-    },
-    total=False,
-)
-
-QueryStringObjectOutputTypeDef = TypedDict(
-    "QueryStringObjectOutputTypeDef",
-    {
-        "option": bool,
-        "queryStringsAllowList": List[str],
-    },
-    total=False,
-)
-
 CookieObjectTypeDef = TypedDict(
     "CookieObjectTypeDef",
     {
         "option": ForwardValuesType,
         "cookiesAllowList": Sequence[str],
     },
     total=False,
@@ -934,25 +898,14 @@
         "image": str,
         "digest": str,
         "createdAt": datetime,
     },
     total=False,
 )
 
-ContainerOutputTypeDef = TypedDict(
-    "ContainerOutputTypeDef",
-    {
-        "image": str,
-        "command": List[str],
-        "environment": Dict[str, str],
-        "ports": Dict[str, ContainerServiceProtocolType],
-    },
-    total=False,
-)
-
 ContainerTypeDef = TypedDict(
     "ContainerTypeDef",
     {
         "image": str,
         "command": Sequence[str],
         "environment": Mapping[str, str],
         "ports": Mapping[str, ContainerServiceProtocolType],
@@ -1433,27 +1386,14 @@
     {
         "code": DnsRecordCreationStateCodeType,
         "message": str,
     },
     total=False,
 )
 
-DomainEntryOutputTypeDef = TypedDict(
-    "DomainEntryOutputTypeDef",
-    {
-        "id": str,
-        "name": str,
-        "target": str,
-        "isAlias": bool,
-        "type": str,
-        "options": Dict[str, str],
-    },
-    total=False,
-)
-
 ResourceRecordTypeDef = TypedDict(
     "ResourceRecordTypeDef",
     {
         "name": str,
         "type": str,
         "value": str,
     },
@@ -3095,29 +3035,14 @@
     {
         "bundles": List[BundleTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CacheSettingsOutputTypeDef = TypedDict(
-    "CacheSettingsOutputTypeDef",
-    {
-        "defaultTTL": int,
-        "minimumTTL": int,
-        "maximumTTL": int,
-        "allowedHTTPMethods": str,
-        "cachedHTTPMethods": str,
-        "forwardedCookies": CookieObjectOutputTypeDef,
-        "forwardedHeaders": HeaderObjectOutputTypeDef,
-        "forwardedQueryStrings": QueryStringObjectOutputTypeDef,
-    },
-    total=False,
-)
-
 CacheSettingsTypeDef = TypedDict(
     "CacheSettingsTypeDef",
     {
         "defaultTTL": int,
         "minimumTTL": int,
         "maximumTTL": int,
         "allowedHTTPMethods": str,
@@ -3180,15 +3105,14 @@
     "RegisterContainerImageResultTypeDef",
     {
         "containerImage": ContainerImageTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ContainerUnionTypeDef = Union[ContainerTypeDef, ContainerOutputTypeDef]
 PrivateRegistryAccessRequestTypeDef = TypedDict(
     "PrivateRegistryAccessRequestTypeDef",
     {
         "ecrImagePullerRole": ContainerServiceECRImagePullerRoleRequestTypeDef,
     },
     total=False,
 )
@@ -3471,15 +3395,14 @@
     "GetDistributionBundlesResultTypeDef",
     {
         "bundles": List[DistributionBundleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DomainEntryUnionTypeDef = Union[DomainEntryTypeDef, DomainEntryOutputTypeDef]
 DomainValidationRecordTypeDef = TypedDict(
     "DomainValidationRecordTypeDef",
     {
         "domainName": str,
         "resourceRecord": ResourceRecordTypeDef,
         "dnsRecordCreationState": DnsRecordCreationStateTypeDef,
         "validationStatus": CertificateDomainValidationStatusType,
@@ -4920,42 +4843,14 @@
     {
         "relationalDatabaseSnapshots": List[RelationalDatabaseSnapshotTypeDef],
         "nextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LightsailDistributionTypeDef = TypedDict(
-    "LightsailDistributionTypeDef",
-    {
-        "name": str,
-        "arn": str,
-        "supportCode": str,
-        "createdAt": datetime,
-        "location": ResourceLocationTypeDef,
-        "resourceType": ResourceTypeType,
-        "alternativeDomainNames": List[str],
-        "status": str,
-        "isEnabled": bool,
-        "domainName": str,
-        "bundleId": str,
-        "certificateName": str,
-        "origin": OriginTypeDef,
-        "originPublicDNS": str,
-        "defaultCacheBehavior": CacheBehaviorTypeDef,
-        "cacheBehaviorSettings": CacheSettingsOutputTypeDef,
-        "cacheBehaviors": List[CacheBehaviorPerPathTypeDef],
-        "ableToUpdateBundle": bool,
-        "ipAddressType": IpAddressTypeType,
-        "tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-CacheSettingsUnionTypeDef = Union[CacheSettingsTypeDef, CacheSettingsOutputTypeDef]
 _RequiredCreateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
         "origin": InputOriginTypeDef,
         "defaultCacheBehavior": CacheBehaviorTypeDef,
         "bundleId": str,
@@ -4974,14 +4869,41 @@
 
 class CreateDistributionRequestRequestTypeDef(
     _RequiredCreateDistributionRequestRequestTypeDef,
     _OptionalCreateDistributionRequestRequestTypeDef,
 ):
     pass
 
+LightsailDistributionTypeDef = TypedDict(
+    "LightsailDistributionTypeDef",
+    {
+        "name": str,
+        "arn": str,
+        "supportCode": str,
+        "createdAt": datetime,
+        "location": ResourceLocationTypeDef,
+        "resourceType": ResourceTypeType,
+        "alternativeDomainNames": List[str],
+        "status": str,
+        "isEnabled": bool,
+        "domainName": str,
+        "bundleId": str,
+        "certificateName": str,
+        "origin": OriginTypeDef,
+        "originPublicDNS": str,
+        "defaultCacheBehavior": CacheBehaviorTypeDef,
+        "cacheBehaviorSettings": CacheSettingsTypeDef,
+        "cacheBehaviors": List[CacheBehaviorPerPathTypeDef],
+        "ableToUpdateBundle": bool,
+        "ipAddressType": IpAddressTypeType,
+        "tags": List[TagTypeDef],
+    },
+    total=False,
+)
+
 _RequiredUpdateDistributionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDistributionRequestRequestTypeDef",
     {
         "distributionName": str,
     },
 )
 _OptionalUpdateDistributionRequestRequestTypeDef = TypedDict(
@@ -5036,15 +4958,15 @@
     pass
 
 ContainerServiceDeploymentTypeDef = TypedDict(
     "ContainerServiceDeploymentTypeDef",
     {
         "version": int,
         "state": ContainerServiceDeploymentStateType,
-        "containers": Dict[str, ContainerOutputTypeDef],
+        "containers": Dict[str, ContainerTypeDef],
         "publicEndpoint": ContainerServiceEndpointTypeDef,
         "createdAt": datetime,
     },
     total=False,
 )
 
 ContainerServiceDeploymentRequestTypeDef = TypedDict(
@@ -5061,15 +4983,15 @@
     {
         "serviceName": str,
     },
 )
 _OptionalCreateContainerServiceDeploymentRequestRequestTypeDef = TypedDict(
     "_OptionalCreateContainerServiceDeploymentRequestRequestTypeDef",
     {
-        "containers": Mapping[str, ContainerUnionTypeDef],
+        "containers": Mapping[str, ContainerTypeDef],
         "publicEndpoint": EndpointRequestTypeDef,
     },
     total=False,
 )
 
 class CreateContainerServiceDeploymentRequestRequestTypeDef(
     _RequiredCreateContainerServiceDeploymentRequestRequestTypeDef,
@@ -5175,15 +5097,15 @@
         "name": str,
         "arn": str,
         "supportCode": str,
         "createdAt": datetime,
         "location": ResourceLocationTypeDef,
         "resourceType": ResourceTypeType,
         "tags": List[TagTypeDef],
-        "domainEntries": List[DomainEntryOutputTypeDef],
+        "domainEntries": List[DomainEntryTypeDef],
         "registeredDomainDelegationInfo": RegisteredDomainDelegationInfoTypeDef,
     },
     total=False,
 )
 
 GetRelationalDatabaseResultTypeDef = TypedDict(
     "GetRelationalDatabaseResultTypeDef",
```

### Comparing `types-aiobotocore-lightsail-2.5.2.post1/types_aiobotocore_lightsail.egg-info/SOURCES.txt` & `types-aiobotocore-lightsail-2.5.2.post2/types_aiobotocore_lightsail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

