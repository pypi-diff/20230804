# Comparing `tmp/types-aiobotocore-ec2-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ec2-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ec2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-ec2-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:49 2023, max compression
```

## Comparing `types-aiobotocore-ec2-2.5.2.post1.tar` & `types-aiobotocore-ec2-2.5.2.post2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.117595 types-aiobotocore-ec2-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:37:11.000000 types-aiobotocore-ec2-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)   173228 2023-08-02 14:52:14.113595 types-aiobotocore-ec2-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)   171726 2023-08-02 14:37:11.000000 types-aiobotocore-ec2-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.117595 types-aiobotocore-ec2-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:37:10.000000 types-aiobotocore-ec2-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.109595 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/
--rw-r--r--   0 runner    (1001) docker     (123)    46244 2023-08-02 14:37:11.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    46242 2023-08-02 14:37:11.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:37:11.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   539314 2023-08-02 14:37:17.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   538538 2023-08-02 14:37:14.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    89586 2023-08-02 14:37:25.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    89584 2023-08-02 14:37:23.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   188526 2023-08-02 14:37:22.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)   188385 2023-08-02 14:37:21.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:37:11.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   293471 2023-08-02 14:37:19.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)   292974 2023-08-02 14:37:18.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)   962122 2023-08-02 14:37:48.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   961113 2023-08-02 14:37:36.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:37:11.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)    40394 2023-08-02 14:37:22.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    40359 2023-08-02 14:37:22.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.113595 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)   173228 2023-08-02 14:52:13.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 14:52:13.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:13.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:13.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:13.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:13.000000 types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:49.216021 types-aiobotocore-ec2-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:44:35.000000 types-aiobotocore-ec2-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    51729 2023-08-04 12:00:49.216021 types-aiobotocore-ec2-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    50227 2023-08-04 11:44:35.000000 types-aiobotocore-ec2-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:49.216021 types-aiobotocore-ec2-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-04 11:44:34.000000 types-aiobotocore-ec2-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:49.216021 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/
+-rw-r--r--   0 runner    (1001) docker     (123)    46244 2023-08-04 11:44:35.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46242 2023-08-04 11:44:35.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-04 11:44:35.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   538805 2023-08-04 11:44:41.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   538029 2023-08-04 11:44:37.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    89586 2023-08-04 11:44:49.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89584 2023-08-04 11:44:48.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   188566 2023-08-04 11:44:47.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188425 2023-08-04 11:44:45.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:44:35.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   293373 2023-08-04 11:44:44.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)   292876 2023-08-04 11:44:43.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)   958695 2023-08-04 11:45:16.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   957686 2023-08-04 11:45:03.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:44:35.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40394 2023-08-04 11:44:47.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40359 2023-08-04 11:44:47.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:49.216021 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    51729 2023-08-04 12:00:49.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-04 12:00:49.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:49.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:49.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:49.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 12:00:49.000000 types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ec2-2.5.2.post1/LICENSE` & `types-aiobotocore-ec2-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-2.5.2.post1/setup.py` & `types-aiobotocore-ec2-2.5.2.post2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ec2",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ec2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EC2 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/__init__.py` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/__init__.pyi` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/__main__.py` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EC2 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.EC2 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2\nOther"
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

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/client.py` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -718,26 +718,26 @@
     InstanceEventWindowAssociationRequestTypeDef,
     InstanceEventWindowDisassociationRequestTypeDef,
     InstanceEventWindowTimeRangeRequestTypeDef,
     InstanceIpv6AddressTypeDef,
     InstanceMaintenanceOptionsRequestTypeDef,
     InstanceMarketOptionsRequestTypeDef,
     InstanceMetadataOptionsRequestTypeDef,
-    InstanceNetworkInterfaceSpecificationUnionTypeDef,
+    InstanceNetworkInterfaceSpecificationTypeDef,
     InstanceRequirementsRequestTypeDef,
     InstanceRequirementsWithMetadataRequestTypeDef,
     InstanceSpecificationTypeDef,
     IntegrateServicesTypeDef,
     IpamCidrAuthorizationContextTypeDef,
-    IpPermissionUnionTypeDef,
+    IpPermissionTypeDef,
     Ipv4PrefixSpecificationRequestTypeDef,
     Ipv6PrefixSpecificationRequestTypeDef,
     KeyPairTypeDef,
     LaunchPermissionModificationsTypeDef,
-    LaunchTemplateConfigUnionTypeDef,
+    LaunchTemplateConfigTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LicenseConfigurationRequestTypeDef,
     ListImagesInRecycleBinResultTypeDef,
     ListSnapshotsInRecycleBinResultTypeDef,
     LoadPermissionModificationsTypeDef,
     ModifyAddressAttributeResultTypeDef,
     ModifyAvailabilityZoneGroupResultTypeDef,
@@ -869,24 +869,24 @@
     SearchTransitGatewayRoutesResultTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     SecurityGroupRuleUpdateTypeDef,
     SlotDateTimeRangeRequestTypeDef,
     SlotStartTimeRangeRequestTypeDef,
     SnapshotDiskContainerTypeDef,
     SnapshotResponseTypeDef,
-    SpotFleetRequestConfigDataUnionTypeDef,
+    SpotFleetRequestConfigDataTypeDef,
     SpotOptionsRequestTypeDef,
     StartInstancesResultTypeDef,
     StartNetworkInsightsAccessScopeAnalysisResultTypeDef,
     StartNetworkInsightsAnalysisResultTypeDef,
     StartVpcEndpointServicePrivateDnsVerificationResultTypeDef,
     StopInstancesResultTypeDef,
     StorageLocationTypeDef,
-    StorageUnionTypeDef,
-    TagSpecificationUnionTypeDef,
+    StorageTypeDef,
+    TagSpecificationTypeDef,
     TagTypeDef,
     TargetCapacitySpecificationRequestTypeDef,
     TargetConfigurationRequestTypeDef,
     TerminateClientVpnConnectionsResultTypeDef,
     TerminateInstancesResultTypeDef,
     TimestampTypeDef,
     TrafficMirrorPortRangeRequestTypeDef,
@@ -894,15 +894,15 @@
     TransitGatewayRequestOptionsTypeDef,
     UnassignIpv6AddressesResultTypeDef,
     UnassignPrivateNatGatewayAddressResultTypeDef,
     UnmonitorInstancesResultTypeDef,
     UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef,
     UpdateSecurityGroupRuleDescriptionsIngressResultTypeDef,
     VerifiedAccessLogOptionsTypeDef,
-    VolumeAttachmentResponseTypeDef,
+    VolumeAttachmentTypeDef,
     VolumeDetailTypeDef,
     VolumeResponseTypeDef,
     VpnConnectionOptionsSpecificationTypeDef,
     WithdrawByoipCidrResultTypeDef,
 )
 from .waiter import (
     BundleTaskCompleteWaiter,
@@ -980,15 +980,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#exceptions)
         """
 
     async def accept_address_transfer(
         self,
         *,
         Address: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> AcceptAddressTransferResultTypeDef:
         """
         Accepts an Elastic IP address transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.accept_address_transfer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#accept_address_transfer)
@@ -1080,15 +1080,15 @@
         *,
         Domain: DomainTypeType = ...,
         Address: str = ...,
         PublicIpv4Pool: str = ...,
         NetworkBorderGroup: str = ...,
         CustomerOwnedIpv4Pool: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> AllocateAddressResultTypeDef:
         """
         Allocates an Elastic IP address to your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.allocate_address)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#allocate_address)
         """
@@ -1098,15 +1098,15 @@
         *,
         AvailabilityZone: str,
         AutoPlacement: AutoPlacementType = ...,
         ClientToken: str = ...,
         InstanceType: str = ...,
         InstanceFamily: str = ...,
         Quantity: int = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         HostRecovery: HostRecoveryType = ...,
         OutpostArn: str = ...,
         HostMaintenance: HostMaintenanceType = ...,
         AssetIds: Sequence[str] = ...
     ) -> AllocateHostsResultTypeDef:
         """
         Allocates a Dedicated Host to your account.
@@ -1276,15 +1276,15 @@
 
     async def associate_ipam_resource_discovery(
         self,
         *,
         IpamId: str,
         IpamResourceDiscoveryId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> AssociateIpamResourceDiscoveryResultTypeDef:
         """
         Associates an IPAM resource discovery with an Amazon VPC IPAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.associate_ipam_resource_discovery)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#associate_ipam_resource_discovery)
@@ -1463,15 +1463,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.attach_verified_access_trust_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#attach_verified_access_trust_provider)
         """
 
     async def attach_volume(
         self, *, Device: str, InstanceId: str, VolumeId: str, DryRun: bool = ...
-    ) -> VolumeAttachmentResponseTypeDef:
+    ) -> VolumeAttachmentTypeDef:
         """
         Attaches an EBS volume to a running or stopped instance and exposes it to the
         instance with the specified device name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.attach_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#attach_volume)
         """
@@ -1505,16 +1505,16 @@
         """
 
     async def authorize_security_group_egress(
         self,
         *,
         GroupId: str,
         DryRun: bool = ...,
-        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         CidrIp: str = ...,
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...
     ) -> AuthorizeSecurityGroupEgressResultTypeDef:
@@ -1529,31 +1529,31 @@
     async def authorize_security_group_ingress(
         self,
         *,
         CidrIp: str = ...,
         FromPort: int = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
         IpProtocol: str = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...,
         ToPort: int = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> AuthorizeSecurityGroupIngressResultTypeDef:
         """
         Adds the specified inbound (ingress) rules to a security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.authorize_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#authorize_security_group_ingress)
         """
 
     async def bundle_instance(
-        self, *, InstanceId: str, Storage: StorageUnionTypeDef, DryRun: bool = ...
+        self, *, InstanceId: str, Storage: StorageTypeDef, DryRun: bool = ...
     ) -> BundleInstanceResultTypeDef:
         """
         Bundles an Amazon instance store-backed Windows instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.bundle_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#bundle_instance)
         """
@@ -1730,15 +1730,15 @@
         SourceSnapshotId: str,
         Description: str = ...,
         DestinationOutpostArn: str = ...,
         DestinationRegion: str = ...,
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         PresignedUrl: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CopySnapshotResultTypeDef:
         """
         Copies a point-in-time snapshot of an EBS volume and stores it in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.copy_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#copy_snapshot)
@@ -1755,15 +1755,15 @@
         AvailabilityZoneId: str = ...,
         Tenancy: CapacityReservationTenancyType = ...,
         EbsOptimized: bool = ...,
         EphemeralStorage: bool = ...,
         EndDate: TimestampTypeDef = ...,
         EndDateType: EndDateTypeType = ...,
         InstanceMatchCriteria: InstanceMatchCriteriaType = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         OutpostArn: str = ...,
         PlacementGroupArn: str = ...
     ) -> CreateCapacityReservationResultTypeDef:
         """
         Creates a new Capacity Reservation with the specified attributes.
 
@@ -1777,29 +1777,29 @@
         InstanceTypeSpecifications: Sequence[ReservationFleetInstanceSpecificationTypeDef],
         TotalTargetCapacity: int,
         AllocationStrategy: str = ...,
         ClientToken: str = ...,
         Tenancy: Literal["default"] = ...,
         EndDate: TimestampTypeDef = ...,
         InstanceMatchCriteria: Literal["open"] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateCapacityReservationFleetResultTypeDef:
         """
         Creates a Capacity Reservation Fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_capacity_reservation_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_capacity_reservation_fleet)
         """
 
     async def create_carrier_gateway(
         self,
         *,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...
     ) -> CreateCarrierGatewayResultTypeDef:
         """
         Creates a carrier gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_carrier_gateway)
@@ -1816,15 +1816,15 @@
         DnsServers: Sequence[str] = ...,
         TransportProtocol: TransportProtocolType = ...,
         VpnPort: int = ...,
         Description: str = ...,
         SplitTunnel: bool = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         SecurityGroupIds: Sequence[str] = ...,
         VpcId: str = ...,
         SelfServicePortal: SelfServicePortalType = ...,
         ClientConnectOptions: ClientConnectOptionsTypeDef = ...,
         SessionTimeoutHours: int = ...,
         ClientLoginBannerOptions: ClientLoginBannerOptionsTypeDef = ...
     ) -> CreateClientVpnEndpointResultTypeDef:
@@ -1862,15 +1862,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_coip_cidr)
         """
 
     async def create_coip_pool(
         self,
         *,
         LocalGatewayRouteTableId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateCoipPoolResultTypeDef:
         """
         Creates a pool of customer-owned IP (CoIP) addresses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_coip_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_coip_pool)
@@ -1879,15 +1879,15 @@
     async def create_customer_gateway(
         self,
         *,
         Type: Literal["ipsec.1"],
         BgpAsn: int = ...,
         PublicIp: str = ...,
         CertificateArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DeviceName: str = ...,
         IpAddress: str = ...,
         DryRun: bool = ...
     ) -> CreateCustomerGatewayResultTypeDef:
         """
         Provides information to Amazon Web Services about your customer gateway device.
 
@@ -1915,15 +1915,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_default_vpc)
         """
 
     async def create_dhcp_options(
         self,
         *,
         DhcpConfigurations: Sequence[NewDhcpConfigurationTypeDef],
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateDhcpOptionsResultTypeDef:
         """
         Creates a set of DHCP options for your VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_dhcp_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_dhcp_options)
@@ -1931,15 +1931,15 @@
 
     async def create_egress_only_internet_gateway(
         self,
         *,
         VpcId: str,
         ClientToken: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateEgressOnlyInternetGatewayResultTypeDef:
         """
         [IPv6 only] Creates an egress-only internet gateway for your VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_egress_only_internet_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_egress_only_internet_gateway)
         """
@@ -1955,15 +1955,15 @@
         OnDemandOptions: OnDemandOptionsRequestTypeDef = ...,
         ExcessCapacityTerminationPolicy: FleetExcessCapacityTerminationPolicyType = ...,
         TerminateInstancesWithExpiration: bool = ...,
         Type: FleetTypeType = ...,
         ValidFrom: TimestampTypeDef = ...,
         ValidUntil: TimestampTypeDef = ...,
         ReplaceUnhealthyInstances: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         Context: str = ...
     ) -> CreateFleetResultTypeDef:
         """
         Creates an EC2 Fleet that contains the configuration information for On-Demand
         Instances and Spot Instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_fleet)
@@ -1980,15 +1980,15 @@
         DeliverLogsPermissionArn: str = ...,
         DeliverCrossAccountRole: str = ...,
         LogGroupName: str = ...,
         TrafficType: TrafficTypeType = ...,
         LogDestinationType: LogDestinationTypeType = ...,
         LogDestination: str = ...,
         LogFormat: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         MaxAggregationInterval: int = ...,
         DestinationOptions: DestinationOptionsRequestTypeDef = ...
     ) -> CreateFlowLogsResultTypeDef:
         """
         Creates one or more flow logs to capture information about IP traffic for a
         specific network interface, subnet, or VPC.
 
@@ -2001,15 +2001,15 @@
         *,
         InputStorageLocation: StorageLocationTypeDef,
         DryRun: bool = ...,
         LogsStorageLocation: StorageLocationTypeDef = ...,
         Description: str = ...,
         Name: str = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateFpgaImageResultTypeDef:
         """
         Creates an Amazon FPGA Image (AFI) from the specified design checkpoint (DCP).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_fpga_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_fpga_image)
         """
@@ -2019,15 +2019,15 @@
         *,
         InstanceId: str,
         Name: str,
         BlockDeviceMappings: Sequence[BlockDeviceMappingTypeDef] = ...,
         Description: str = ...,
         DryRun: bool = ...,
         NoReboot: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateImageResultTypeDef:
         """
         Creates an Amazon EBS-backed AMI from an Amazon EBS-backed instance that is
         either running or stopped.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_image)
@@ -2037,15 +2037,15 @@
         self,
         *,
         SubnetId: str,
         DryRun: bool = ...,
         SecurityGroupIds: Sequence[str] = ...,
         PreserveClientIp: bool = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateInstanceConnectEndpointResultTypeDef:
         """
         Creates an EC2 Instance Connect Endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_instance_connect_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_instance_connect_endpoint)
         """
@@ -2053,15 +2053,15 @@
     async def create_instance_event_window(
         self,
         *,
         DryRun: bool = ...,
         Name: str = ...,
         TimeRanges: Sequence[InstanceEventWindowTimeRangeRequestTypeDef] = ...,
         CronExpression: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateInstanceEventWindowResultTypeDef:
         """
         Creates an event window in which scheduled events for the associated Amazon EC2
         instances can run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_instance_event_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_instance_event_window)
@@ -2070,40 +2070,40 @@
     async def create_instance_export_task(
         self,
         *,
         ExportToS3Task: ExportToS3TaskSpecificationTypeDef,
         InstanceId: str,
         TargetEnvironment: ExportEnvironmentType,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateInstanceExportTaskResultTypeDef:
         """
         Exports a running or stopped instance to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_instance_export_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_instance_export_task)
         """
 
     async def create_internet_gateway(
-        self, *, TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ..., DryRun: bool = ...
+        self, *, TagSpecifications: Sequence[TagSpecificationTypeDef] = ..., DryRun: bool = ...
     ) -> CreateInternetGatewayResultTypeDef:
         """
         Creates an internet gateway for use with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_internet_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_internet_gateway)
         """
 
     async def create_ipam(
         self,
         *,
         DryRun: bool = ...,
         Description: str = ...,
         OperatingRegions: Sequence[AddIpamOperatingRegionTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateIpamResultTypeDef:
         """
         Create an IPAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_ipam)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_ipam)
@@ -2120,15 +2120,15 @@
         Description: str = ...,
         AutoImport: bool = ...,
         PubliclyAdvertisable: bool = ...,
         AllocationMinNetmaskLength: int = ...,
         AllocationMaxNetmaskLength: int = ...,
         AllocationDefaultNetmaskLength: int = ...,
         AllocationResourceTags: Sequence[RequestIpamResourceTagTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...,
         AwsService: Literal["ec2"] = ...,
         PublicIpSource: IpamPoolPublicIpSourceType = ...
     ) -> CreateIpamPoolResultTypeDef:
         """
         Create an IP address pool for Amazon VPC IP Address Manager (IPAM).
 
@@ -2138,15 +2138,15 @@
 
     async def create_ipam_resource_discovery(
         self,
         *,
         DryRun: bool = ...,
         Description: str = ...,
         OperatingRegions: Sequence[AddIpamOperatingRegionTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateIpamResourceDiscoveryResultTypeDef:
         """
         Creates an IPAM resource discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_ipam_resource_discovery)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_ipam_resource_discovery)
@@ -2154,15 +2154,15 @@
 
     async def create_ipam_scope(
         self,
         *,
         IpamId: str,
         DryRun: bool = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateIpamScopeResultTypeDef:
         """
         Create an IPAM scope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_ipam_scope)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_ipam_scope)
@@ -2170,15 +2170,15 @@
 
     async def create_key_pair(
         self,
         *,
         KeyName: str,
         DryRun: bool = ...,
         KeyType: KeyTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         KeyFormat: KeyFormatType = ...
     ) -> KeyPairTypeDef:
         """
         Creates an ED25519 or 2048-bit RSA key pair with the specified name and in the
         specified PEM or PPK format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_key_pair)
@@ -2189,15 +2189,15 @@
         self,
         *,
         LaunchTemplateName: str,
         LaunchTemplateData: RequestLaunchTemplateDataTypeDef,
         DryRun: bool = ...,
         ClientToken: str = ...,
         VersionDescription: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateLaunchTemplateResultTypeDef:
         """
         Creates a launch template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_launch_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_launch_template)
         """
@@ -2239,45 +2239,45 @@
         """
 
     async def create_local_gateway_route_table(
         self,
         *,
         LocalGatewayId: str,
         Mode: LocalGatewayRouteTableModeType = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateLocalGatewayRouteTableResultTypeDef:
         """
         Creates a local gateway route table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_local_gateway_route_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_local_gateway_route_table)
         """
 
     async def create_local_gateway_route_table_virtual_interface_group_association(
         self,
         *,
         LocalGatewayRouteTableId: str,
         LocalGatewayVirtualInterfaceGroupId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationResultTypeDef:
         """
         Creates a local gateway route table virtual interface group association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_local_gateway_route_table_virtual_interface_group_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_local_gateway_route_table_virtual_interface_group_association)
         """
 
     async def create_local_gateway_route_table_vpc_association(
         self,
         *,
         LocalGatewayRouteTableId: str,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateLocalGatewayRouteTableVpcAssociationResultTypeDef:
         """
         Associates the specified VPC with the specified local gateway route table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_local_gateway_route_table_vpc_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_local_gateway_route_table_vpc_association)
@@ -2287,15 +2287,15 @@
         self,
         *,
         PrefixListName: str,
         MaxEntries: int,
         AddressFamily: str,
         DryRun: bool = ...,
         Entries: Sequence[AddPrefixListEntryTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateManagedPrefixListResultTypeDef:
         """
         Creates a managed prefix list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_managed_prefix_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_managed_prefix_list)
@@ -2304,15 +2304,15 @@
     async def create_nat_gateway(
         self,
         *,
         SubnetId: str,
         AllocationId: str = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ConnectivityType: ConnectivityTypeType = ...,
         PrivateIpAddress: str = ...,
         SecondaryAllocationIds: Sequence[str] = ...,
         SecondaryPrivateIpAddresses: Sequence[str] = ...,
         SecondaryPrivateIpAddressCount: int = ...
     ) -> CreateNatGatewayResultTypeDef:
         """
@@ -2323,15 +2323,15 @@
         """
 
     async def create_network_acl(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateNetworkAclResultTypeDef:
         """
         Creates a network ACL in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_network_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_network_acl)
         """
@@ -2359,15 +2359,15 @@
 
     async def create_network_insights_access_scope(
         self,
         *,
         ClientToken: str,
         MatchPaths: Sequence[AccessScopePathRequestTypeDef] = ...,
         ExcludePaths: Sequence[AccessScopePathRequestTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateNetworkInsightsAccessScopeResultTypeDef:
         """
         Creates a Network Access Scope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_network_insights_access_scope)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_network_insights_access_scope)
@@ -2379,15 +2379,15 @@
         Source: str,
         Protocol: ProtocolType,
         ClientToken: str,
         SourceIp: str = ...,
         DestinationIp: str = ...,
         Destination: str = ...,
         DestinationPort: int = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         FilterAtSource: PathRequestFilterTypeDef = ...,
         FilterAtDestination: PathRequestFilterTypeDef = ...
     ) -> CreateNetworkInsightsPathResultTypeDef:
         """
         Creates a path to analyze for reachability.
 
@@ -2408,15 +2408,15 @@
         PrivateIpAddresses: Sequence[PrivateIpAddressSpecificationTypeDef] = ...,
         SecondaryPrivateIpAddressCount: int = ...,
         Ipv4Prefixes: Sequence[Ipv4PrefixSpecificationRequestTypeDef] = ...,
         Ipv4PrefixCount: int = ...,
         Ipv6Prefixes: Sequence[Ipv6PrefixSpecificationRequestTypeDef] = ...,
         Ipv6PrefixCount: int = ...,
         InterfaceType: NetworkInterfaceCreationTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateNetworkInterfaceResultTypeDef:
         """
         Creates a network interface in the specified subnet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_network_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_network_interface)
@@ -2442,26 +2442,26 @@
     async def create_placement_group(
         self,
         *,
         DryRun: bool = ...,
         GroupName: str = ...,
         Strategy: PlacementStrategyType = ...,
         PartitionCount: int = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         SpreadLevel: SpreadLevelType = ...
     ) -> CreatePlacementGroupResultTypeDef:
         """
         Creates a placement group in which to launch instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_placement_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_placement_group)
         """
 
     async def create_public_ipv4_pool(
-        self, *, DryRun: bool = ..., TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        self, *, DryRun: bool = ..., TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreatePublicIpv4PoolResultTypeDef:
         """
         Creates a public IPv4 address pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_public_ipv4_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_public_ipv4_pool)
         """
@@ -2469,15 +2469,15 @@
     async def create_replace_root_volume_task(
         self,
         *,
         InstanceId: str,
         SnapshotId: str = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ImageId: str = ...,
         DeleteReplacedRootVolume: bool = ...
     ) -> CreateReplaceRootVolumeTaskResultTypeDef:
         """
         Replaces the EBS-backed root volume for a `running` instance with a new volume
         that is restored to the original root volume's launch state, that is restored to
         a specific snapshot taken from the original root volume, or that is restored
@@ -2505,15 +2505,15 @@
 
     async def create_restore_image_task(
         self,
         *,
         Bucket: str,
         ObjectKey: str,
         Name: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateRestoreImageTaskResultTypeDef:
         """
         Starts a task that restores an AMI from an Amazon S3 object that was previously
         created by using
         [CreateStoreImageTask](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateStoreImageTask.html)_.
 
@@ -2549,30 +2549,30 @@
         """
 
     async def create_route_table(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateRouteTableResultTypeDef:
         """
         Creates a route table for the specified VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_route_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_route_table)
         """
 
     async def create_security_group(
         self,
         *,
         Description: str,
         GroupName: str,
         VpcId: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateSecurityGroupResultTypeDef:
         """
         Creates a security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_security_group)
@@ -2580,15 +2580,15 @@
 
     async def create_snapshot(
         self,
         *,
         VolumeId: str,
         Description: str = ...,
         OutpostArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> SnapshotResponseTypeDef:
         """
         Creates a snapshot of an EBS volume and stores it in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_snapshot)
@@ -2596,15 +2596,15 @@
 
     async def create_snapshots(
         self,
         *,
         InstanceSpecification: InstanceSpecificationTypeDef,
         Description: str = ...,
         OutpostArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         CopyTagsFromSource: Literal["volume"] = ...
     ) -> CreateSnapshotsResultTypeDef:
         """
         Creates crash-consistent snapshots of multiple EBS volumes and stores the data
         in S3.
 
@@ -2638,15 +2638,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_store_image_task)
         """
 
     async def create_subnet(
         self,
         *,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         AvailabilityZone: str = ...,
         AvailabilityZoneId: str = ...,
         CidrBlock: str = ...,
         Ipv6CidrBlock: str = ...,
         OutpostArn: str = ...,
         DryRun: bool = ...,
         Ipv6Native: bool = ...
@@ -2662,15 +2662,15 @@
         self,
         *,
         SubnetId: str,
         Cidr: str,
         ReservationType: SubnetCidrReservationTypeType,
         Description: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateSubnetCidrReservationResultTypeDef:
         """
         Creates a subnet CIDR reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_subnet_cidr_reservation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_subnet_cidr_reservation)
         """
@@ -2686,15 +2686,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_tags)
         """
 
     async def create_traffic_mirror_filter(
         self,
         *,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...
     ) -> CreateTrafficMirrorFilterResultTypeDef:
         """
         Creates a Traffic Mirror filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_traffic_mirror_filter)
@@ -2730,15 +2730,15 @@
         NetworkInterfaceId: str,
         TrafficMirrorTargetId: str,
         TrafficMirrorFilterId: str,
         SessionNumber: int,
         PacketLength: int = ...,
         VirtualNetworkId: int = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...
     ) -> CreateTrafficMirrorSessionResultTypeDef:
         """
         Creates a Traffic Mirror session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_traffic_mirror_session)
@@ -2747,15 +2747,15 @@
 
     async def create_traffic_mirror_target(
         self,
         *,
         NetworkInterfaceId: str = ...,
         NetworkLoadBalancerArn: str = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
         GatewayLoadBalancerEndpointId: str = ...
     ) -> CreateTrafficMirrorTargetResultTypeDef:
         """
         Creates a target for your Traffic Mirror session.
 
@@ -2764,30 +2764,30 @@
         """
 
     async def create_transit_gateway(
         self,
         *,
         Description: str = ...,
         Options: TransitGatewayRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayResultTypeDef:
         """
         Creates a transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway)
         """
 
     async def create_transit_gateway_connect(
         self,
         *,
         TransportTransitGatewayAttachmentId: str,
         Options: CreateTransitGatewayConnectRequestOptionsTypeDef,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayConnectResultTypeDef:
         """
         Creates a Connect attachment from a specified transit gateway attachment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_connect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_connect)
@@ -2797,15 +2797,15 @@
         self,
         *,
         TransitGatewayAttachmentId: str,
         PeerAddress: str,
         InsideCidrBlocks: Sequence[str],
         TransitGatewayAddress: str = ...,
         BgpOptions: TransitGatewayConnectRequestBgpOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayConnectPeerResultTypeDef:
         """
         Creates a Connect peer for a specified transit gateway Connect attachment
         between a transit gateway and an appliance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_connect_peer)
@@ -2813,15 +2813,15 @@
         """
 
     async def create_transit_gateway_multicast_domain(
         self,
         *,
         TransitGatewayId: str,
         Options: CreateTransitGatewayMulticastDomainRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayMulticastDomainResultTypeDef:
         """
         Creates a multicast domain using the specified transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_multicast_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_multicast_domain)
@@ -2831,30 +2831,30 @@
         self,
         *,
         TransitGatewayId: str,
         PeerTransitGatewayId: str,
         PeerAccountId: str,
         PeerRegion: str,
         Options: CreateTransitGatewayPeeringAttachmentRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayPeeringAttachmentResultTypeDef:
         """
         Requests a transit gateway peering attachment between the specified transit
         gateway (requester) and a peer transit gateway (accepter).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_peering_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_peering_attachment)
         """
 
     async def create_transit_gateway_policy_table(
         self,
         *,
         TransitGatewayId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayPolicyTableResultTypeDef:
         """
         Creates a transit gateway policy table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_policy_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_policy_table)
@@ -2893,30 +2893,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_route)
         """
 
     async def create_transit_gateway_route_table(
         self,
         *,
         TransitGatewayId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayRouteTableResultTypeDef:
         """
         Creates a route table for the specified transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_route_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_route_table)
         """
 
     async def create_transit_gateway_route_table_announcement(
         self,
         *,
         TransitGatewayRouteTableId: str,
         PeeringAttachmentId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayRouteTableAnnouncementResultTypeDef:
         """
         Advertises a new transit gateway route table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_route_table_announcement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_route_table_announcement)
@@ -2925,15 +2925,15 @@
     async def create_transit_gateway_vpc_attachment(
         self,
         *,
         TransitGatewayId: str,
         VpcId: str,
         SubnetIds: Sequence[str],
         Options: CreateTransitGatewayVpcAttachmentRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayVpcAttachmentResultTypeDef:
         """
         Attaches the specified VPC to the specified transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_vpc_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_vpc_attachment)
@@ -2949,15 +2949,15 @@
         ApplicationDomain: str,
         EndpointDomainPrefix: str,
         SecurityGroupIds: Sequence[str] = ...,
         LoadBalancerOptions: CreateVerifiedAccessEndpointLoadBalancerOptionsTypeDef = ...,
         NetworkInterfaceOptions: CreateVerifiedAccessEndpointEniOptionsTypeDef = ...,
         Description: str = ...,
         PolicyDocument: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...
     ) -> CreateVerifiedAccessEndpointResultTypeDef:
         """
         An Amazon Web Services Verified Access endpoint is where you define your
         application along with an optional endpoint-level access policy.
 
@@ -2967,15 +2967,15 @@
 
     async def create_verified_access_group(
         self,
         *,
         VerifiedAccessInstanceId: str,
         Description: str = ...,
         PolicyDocument: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...
     ) -> CreateVerifiedAccessGroupResultTypeDef:
         """
         An Amazon Web Services Verified Access group is a collection of Amazon Web
         Services Verified Access endpoints who's associated applications have similar
         security requirements.
@@ -2984,15 +2984,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_verified_access_group)
         """
 
     async def create_verified_access_instance(
         self,
         *,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...
     ) -> CreateVerifiedAccessInstanceResultTypeDef:
         """
         An Amazon Web Services Verified Access instance is a regional entity that
         evaluates application requests and grants access only when your security
         requirements are met.
@@ -3007,15 +3007,15 @@
         TrustProviderType: TrustProviderTypeType,
         PolicyReferenceName: str,
         UserTrustProviderType: UserTrustProviderTypeType = ...,
         DeviceTrustProviderType: DeviceTrustProviderTypeType = ...,
         OidcOptions: CreateVerifiedAccessTrustProviderOidcOptionsTypeDef = ...,
         DeviceOptions: CreateVerifiedAccessTrustProviderDeviceOptionsTypeDef = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...
     ) -> CreateVerifiedAccessTrustProviderResultTypeDef:
         """
         A trust provider is a third-party entity that creates, maintains, and manages
         identity information for users and devices.
 
@@ -3031,15 +3031,15 @@
         Iops: int = ...,
         KmsKeyId: str = ...,
         OutpostArn: str = ...,
         Size: int = ...,
         SnapshotId: str = ...,
         VolumeType: VolumeTypeType = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         MultiAttachEnabled: bool = ...,
         Throughput: int = ...,
         ClientToken: str = ...
     ) -> VolumeResponseTypeDef:
         """
         Creates an EBS volume that can be attached to an instance in the same
         Availability Zone.
@@ -3058,15 +3058,15 @@
         Ipv4IpamPoolId: str = ...,
         Ipv4NetmaskLength: int = ...,
         Ipv6IpamPoolId: str = ...,
         Ipv6NetmaskLength: int = ...,
         DryRun: bool = ...,
         InstanceTenancy: TenancyType = ...,
         Ipv6CidrBlockNetworkBorderGroup: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateVpcResultTypeDef:
         """
         Creates a VPC with the specified CIDR blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_vpc)
         """
@@ -3082,15 +3082,15 @@
         RouteTableIds: Sequence[str] = ...,
         SubnetIds: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
         IpAddressType: IpAddressTypeType = ...,
         DnsOptions: DnsOptionsSpecificationTypeDef = ...,
         ClientToken: str = ...,
         PrivateDnsEnabled: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateVpcEndpointResultTypeDef:
         """
         Creates a VPC endpoint for a specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_vpc_endpoint)
         """
@@ -3119,15 +3119,15 @@
         DryRun: bool = ...,
         AcceptanceRequired: bool = ...,
         PrivateDnsName: str = ...,
         NetworkLoadBalancerArns: Sequence[str] = ...,
         GatewayLoadBalancerArns: Sequence[str] = ...,
         SupportedIpAddressTypes: Sequence[str] = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateVpcEndpointServiceConfigurationResultTypeDef:
         """
         Creates a VPC endpoint service to which service consumers (Amazon Web Services
         accounts, users, and IAM roles) can connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_endpoint_service_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_vpc_endpoint_service_configuration)
@@ -3137,15 +3137,15 @@
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
         PeerOwnerId: str = ...,
         PeerVpcId: str = ...,
         PeerRegion: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateVpcPeeringConnectionResultTypeDef:
         """
         Requests a VPC peering connection between two VPCs: a requester VPC that you own
         and an accepter VPC with which to create the connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_peering_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_vpc_peering_connection)
@@ -3156,15 +3156,15 @@
         *,
         CustomerGatewayId: str,
         Type: str,
         VpnGatewayId: str = ...,
         TransitGatewayId: str = ...,
         DryRun: bool = ...,
         Options: VpnConnectionOptionsSpecificationTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateVpnConnectionResultTypeDef:
         """
         Creates a VPN connection between an existing virtual private gateway or transit
         gateway and a customer gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpn_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_vpn_connection)
@@ -3182,15 +3182,15 @@
         """
 
     async def create_vpn_gateway(
         self,
         *,
         Type: Literal["ipsec.1"],
         AvailabilityZone: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         AmazonSideAsn: int = ...,
         DryRun: bool = ...
     ) -> CreateVpnGatewayResultTypeDef:
         """
         Creates a virtual private gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpn_gateway)
@@ -6350,15 +6350,15 @@
         self,
         *,
         VolumeId: str,
         Device: str = ...,
         Force: bool = ...,
         InstanceId: str = ...,
         DryRun: bool = ...
-    ) -> VolumeAttachmentResponseTypeDef:
+    ) -> VolumeAttachmentTypeDef:
         """
         Detaches an EBS volume from an instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.detach_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#detach_volume)
         """
 
@@ -6870,15 +6870,15 @@
         DiskImageFormat: DiskImageFormatType,
         ImageId: str,
         S3ExportLocation: ExportTaskS3LocationRequestTypeDef,
         ClientToken: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
         RoleName: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> ExportImageResultTypeDef:
         """
         Exports an Amazon Machine Image (AMI) to a VM file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.export_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#export_image)
         """
@@ -7545,15 +7545,15 @@
         Encrypted: bool = ...,
         Hypervisor: str = ...,
         KmsKeyId: str = ...,
         LicenseType: str = ...,
         Platform: str = ...,
         RoleName: str = ...,
         LicenseSpecifications: Sequence[ImportImageLicenseConfigurationRequestTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         UsageOperation: str = ...,
         BootMode: BootModeValuesType = ...
     ) -> ImportImageResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_image)
@@ -7578,15 +7578,15 @@
 
     async def import_key_pair(
         self,
         *,
         KeyName: str,
         PublicKeyMaterial: BlobTypeDef,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> ImportKeyPairResultTypeDef:
         """
         Imports the public key from an RSA or ED25519 key pair that you created with a
         third-party tool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_key_pair)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#import_key_pair)
@@ -7599,15 +7599,15 @@
         ClientToken: str = ...,
         Description: str = ...,
         DiskContainer: SnapshotDiskContainerTypeDef = ...,
         DryRun: bool = ...,
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         RoleName: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> ImportSnapshotResultTypeDef:
         """
         Imports a disk into an EBS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#import_snapshot)
         """
@@ -8234,15 +8234,15 @@
         """
 
     async def modify_spot_fleet_request(
         self,
         *,
         SpotFleetRequestId: str,
         ExcessCapacityTerminationPolicy: ExcessCapacityTerminationPolicyType = ...,
-        LaunchTemplateConfigs: Sequence[LaunchTemplateConfigUnionTypeDef] = ...,
+        LaunchTemplateConfigs: Sequence[LaunchTemplateConfigTypeDef] = ...,
         TargetCapacity: int = ...,
         OnDemandTargetCapacity: int = ...,
         Context: str = ...
     ) -> ModifySpotFleetRequestResponseTypeDef:
         """
         Modifies the specified Spot Fleet request.
 
@@ -8744,15 +8744,15 @@
         self,
         *,
         Cidr: str,
         CidrAuthorizationContext: CidrAuthorizationContextTypeDef = ...,
         PubliclyAdvertisable: bool = ...,
         Description: str = ...,
         DryRun: bool = ...,
-        PoolTagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        PoolTagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         MultiRegion: bool = ...
     ) -> ProvisionByoipCidrResultTypeDef:
         """
         Provisions an IPv4 or IPv6 address range for use with your Amazon Web Services
         resources through bring your own IP addresses (BYOIP) and creates a
         corresponding address pool.
 
@@ -8791,15 +8791,15 @@
         self,
         *,
         HostIdSet: Sequence[str],
         OfferingId: str,
         ClientToken: str = ...,
         CurrencyCode: Literal["USD"] = ...,
         LimitPrice: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> PurchaseHostReservationResultTypeDef:
         """
         Purchase a reservation with configurations that match those of your Dedicated
         Host.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.purchase_host_reservation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#purchase_host_reservation)
@@ -9133,15 +9133,15 @@
         Submits feedback about the status of an instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.report_instance_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#report_instance_status)
         """
 
     async def request_spot_fleet(
-        self, *, SpotFleetRequestConfig: SpotFleetRequestConfigDataUnionTypeDef, DryRun: bool = ...
+        self, *, SpotFleetRequestConfig: SpotFleetRequestConfigDataTypeDef, DryRun: bool = ...
     ) -> RequestSpotFleetResponseTypeDef:
         """
         Creates a Spot Fleet request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.request_spot_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#request_spot_fleet)
         """
@@ -9156,15 +9156,15 @@
         InstanceCount: int = ...,
         LaunchGroup: str = ...,
         LaunchSpecification: RequestSpotLaunchSpecificationTypeDef = ...,
         SpotPrice: str = ...,
         Type: SpotInstanceTypeType = ...,
         ValidFrom: TimestampTypeDef = ...,
         ValidUntil: TimestampTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         InstanceInterruptionBehavior: InstanceInterruptionBehaviorType = ...
     ) -> RequestSpotInstancesResultTypeDef:
         """
         Creates a Spot Instance request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.request_spot_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#request_spot_instances)
@@ -9317,15 +9317,15 @@
         """
 
     async def revoke_security_group_egress(
         self,
         *,
         GroupId: str,
         DryRun: bool = ...,
-        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
         SecurityGroupRuleIds: Sequence[str] = ...,
         CidrIp: str = ...,
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...
@@ -9341,15 +9341,15 @@
     async def revoke_security_group_ingress(
         self,
         *,
         CidrIp: str = ...,
         FromPort: int = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
         IpProtocol: str = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...,
         ToPort: int = ...,
         DryRun: bool = ...,
         SecurityGroupRuleIds: Sequence[str] = ...
     ) -> RevokeSecurityGroupIngressResultTypeDef:
@@ -9382,19 +9382,19 @@
         AdditionalInfo: str = ...,
         ClientToken: str = ...,
         DisableApiTermination: bool = ...,
         DryRun: bool = ...,
         EbsOptimized: bool = ...,
         IamInstanceProfile: IamInstanceProfileSpecificationTypeDef = ...,
         InstanceInitiatedShutdownBehavior: ShutdownBehaviorType = ...,
-        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef] = ...,
+        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationTypeDef] = ...,
         PrivateIpAddress: str = ...,
         ElasticGpuSpecification: Sequence[ElasticGpuSpecificationTypeDef] = ...,
         ElasticInferenceAccelerators: Sequence[ElasticInferenceAcceleratorTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         InstanceMarketOptions: InstanceMarketOptionsRequestTypeDef = ...,
         CreditSpecification: CreditSpecificationRequestTypeDef = ...,
         CpuOptions: CpuOptionsRequestTypeDef = ...,
         CapacityReservationSpecification: CapacityReservationSpecificationTypeDef = ...,
         HibernationOptions: HibernationOptionsRequestTypeDef = ...,
         LicenseSpecifications: Sequence[LicenseConfigurationRequestTypeDef] = ...,
@@ -9500,15 +9500,15 @@
 
     async def start_network_insights_access_scope_analysis(
         self,
         *,
         NetworkInsightsAccessScopeId: str,
         ClientToken: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> StartNetworkInsightsAccessScopeAnalysisResultTypeDef:
         """
         Starts analyzing the specified Network Access Scope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.start_network_insights_access_scope_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#start_network_insights_access_scope_analysis)
         """
@@ -9517,15 +9517,15 @@
         self,
         *,
         NetworkInsightsPathId: str,
         ClientToken: str,
         AdditionalAccounts: Sequence[str] = ...,
         FilterInArns: Sequence[str] = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> StartNetworkInsightsAnalysisResultTypeDef:
         """
         Starts analyzing the specified path.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.start_network_insights_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#start_network_insights_analysis)
         """
@@ -9638,15 +9638,15 @@
 
     async def update_security_group_rule_descriptions_egress(
         self,
         *,
         DryRun: bool = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
         SecurityGroupRuleDescriptions: Sequence[SecurityGroupRuleDescriptionTypeDef] = ...
     ) -> UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef:
         """
         [VPC only] Updates the description of an egress (outbound) security group rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.update_security_group_rule_descriptions_egress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#update_security_group_rule_descriptions_egress)
@@ -9654,15 +9654,15 @@
 
     async def update_security_group_rule_descriptions_ingress(
         self,
         *,
         DryRun: bool = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
         SecurityGroupRuleDescriptions: Sequence[SecurityGroupRuleDescriptionTypeDef] = ...
     ) -> UpdateSecurityGroupRuleDescriptionsIngressResultTypeDef:
         """
         Updates the description of an ingress (inbound) security group rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.update_security_group_rule_descriptions_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#update_security_group_rule_descriptions_ingress)
```

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/client.pyi` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -718,26 +718,26 @@
     InstanceEventWindowAssociationRequestTypeDef,
     InstanceEventWindowDisassociationRequestTypeDef,
     InstanceEventWindowTimeRangeRequestTypeDef,
     InstanceIpv6AddressTypeDef,
     InstanceMaintenanceOptionsRequestTypeDef,
     InstanceMarketOptionsRequestTypeDef,
     InstanceMetadataOptionsRequestTypeDef,
-    InstanceNetworkInterfaceSpecificationUnionTypeDef,
+    InstanceNetworkInterfaceSpecificationTypeDef,
     InstanceRequirementsRequestTypeDef,
     InstanceRequirementsWithMetadataRequestTypeDef,
     InstanceSpecificationTypeDef,
     IntegrateServicesTypeDef,
     IpamCidrAuthorizationContextTypeDef,
-    IpPermissionUnionTypeDef,
+    IpPermissionTypeDef,
     Ipv4PrefixSpecificationRequestTypeDef,
     Ipv6PrefixSpecificationRequestTypeDef,
     KeyPairTypeDef,
     LaunchPermissionModificationsTypeDef,
-    LaunchTemplateConfigUnionTypeDef,
+    LaunchTemplateConfigTypeDef,
     LaunchTemplateSpecificationTypeDef,
     LicenseConfigurationRequestTypeDef,
     ListImagesInRecycleBinResultTypeDef,
     ListSnapshotsInRecycleBinResultTypeDef,
     LoadPermissionModificationsTypeDef,
     ModifyAddressAttributeResultTypeDef,
     ModifyAvailabilityZoneGroupResultTypeDef,
@@ -869,24 +869,24 @@
     SearchTransitGatewayRoutesResultTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     SecurityGroupRuleUpdateTypeDef,
     SlotDateTimeRangeRequestTypeDef,
     SlotStartTimeRangeRequestTypeDef,
     SnapshotDiskContainerTypeDef,
     SnapshotResponseTypeDef,
-    SpotFleetRequestConfigDataUnionTypeDef,
+    SpotFleetRequestConfigDataTypeDef,
     SpotOptionsRequestTypeDef,
     StartInstancesResultTypeDef,
     StartNetworkInsightsAccessScopeAnalysisResultTypeDef,
     StartNetworkInsightsAnalysisResultTypeDef,
     StartVpcEndpointServicePrivateDnsVerificationResultTypeDef,
     StopInstancesResultTypeDef,
     StorageLocationTypeDef,
-    StorageUnionTypeDef,
-    TagSpecificationUnionTypeDef,
+    StorageTypeDef,
+    TagSpecificationTypeDef,
     TagTypeDef,
     TargetCapacitySpecificationRequestTypeDef,
     TargetConfigurationRequestTypeDef,
     TerminateClientVpnConnectionsResultTypeDef,
     TerminateInstancesResultTypeDef,
     TimestampTypeDef,
     TrafficMirrorPortRangeRequestTypeDef,
@@ -894,15 +894,15 @@
     TransitGatewayRequestOptionsTypeDef,
     UnassignIpv6AddressesResultTypeDef,
     UnassignPrivateNatGatewayAddressResultTypeDef,
     UnmonitorInstancesResultTypeDef,
     UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef,
     UpdateSecurityGroupRuleDescriptionsIngressResultTypeDef,
     VerifiedAccessLogOptionsTypeDef,
-    VolumeAttachmentResponseTypeDef,
+    VolumeAttachmentTypeDef,
     VolumeDetailTypeDef,
     VolumeResponseTypeDef,
     VpnConnectionOptionsSpecificationTypeDef,
     WithdrawByoipCidrResultTypeDef,
 )
 from .waiter import (
     BundleTaskCompleteWaiter,
@@ -975,15 +975,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#exceptions)
         """
     async def accept_address_transfer(
         self,
         *,
         Address: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> AcceptAddressTransferResultTypeDef:
         """
         Accepts an Elastic IP address transfer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.accept_address_transfer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#accept_address_transfer)
@@ -1067,15 +1067,15 @@
         *,
         Domain: DomainTypeType = ...,
         Address: str = ...,
         PublicIpv4Pool: str = ...,
         NetworkBorderGroup: str = ...,
         CustomerOwnedIpv4Pool: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> AllocateAddressResultTypeDef:
         """
         Allocates an Elastic IP address to your Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.allocate_address)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#allocate_address)
         """
@@ -1084,15 +1084,15 @@
         *,
         AvailabilityZone: str,
         AutoPlacement: AutoPlacementType = ...,
         ClientToken: str = ...,
         InstanceType: str = ...,
         InstanceFamily: str = ...,
         Quantity: int = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         HostRecovery: HostRecoveryType = ...,
         OutpostArn: str = ...,
         HostMaintenance: HostMaintenanceType = ...,
         AssetIds: Sequence[str] = ...
     ) -> AllocateHostsResultTypeDef:
         """
         Allocates a Dedicated Host to your account.
@@ -1250,15 +1250,15 @@
         """
     async def associate_ipam_resource_discovery(
         self,
         *,
         IpamId: str,
         IpamResourceDiscoveryId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> AssociateIpamResourceDiscoveryResultTypeDef:
         """
         Associates an IPAM resource discovery with an Amazon VPC IPAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.associate_ipam_resource_discovery)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#associate_ipam_resource_discovery)
@@ -1424,15 +1424,15 @@
         specified Amazon Web Services Verified Access instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.attach_verified_access_trust_provider)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#attach_verified_access_trust_provider)
         """
     async def attach_volume(
         self, *, Device: str, InstanceId: str, VolumeId: str, DryRun: bool = ...
-    ) -> VolumeAttachmentResponseTypeDef:
+    ) -> VolumeAttachmentTypeDef:
         """
         Attaches an EBS volume to a running or stopped instance and exposes it to the
         instance with the specified device name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.attach_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#attach_volume)
         """
@@ -1463,16 +1463,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#authorize_client_vpn_ingress)
         """
     async def authorize_security_group_egress(
         self,
         *,
         GroupId: str,
         DryRun: bool = ...,
-        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         CidrIp: str = ...,
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...
     ) -> AuthorizeSecurityGroupEgressResultTypeDef:
@@ -1486,30 +1486,30 @@
     async def authorize_security_group_ingress(
         self,
         *,
         CidrIp: str = ...,
         FromPort: int = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
         IpProtocol: str = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...,
         ToPort: int = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> AuthorizeSecurityGroupIngressResultTypeDef:
         """
         Adds the specified inbound (ingress) rules to a security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.authorize_security_group_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#authorize_security_group_ingress)
         """
     async def bundle_instance(
-        self, *, InstanceId: str, Storage: StorageUnionTypeDef, DryRun: bool = ...
+        self, *, InstanceId: str, Storage: StorageTypeDef, DryRun: bool = ...
     ) -> BundleInstanceResultTypeDef:
         """
         Bundles an Amazon instance store-backed Windows instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.bundle_instance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#bundle_instance)
         """
@@ -1670,15 +1670,15 @@
         SourceSnapshotId: str,
         Description: str = ...,
         DestinationOutpostArn: str = ...,
         DestinationRegion: str = ...,
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         PresignedUrl: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CopySnapshotResultTypeDef:
         """
         Copies a point-in-time snapshot of an EBS volume and stores it in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.copy_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#copy_snapshot)
@@ -1694,15 +1694,15 @@
         AvailabilityZoneId: str = ...,
         Tenancy: CapacityReservationTenancyType = ...,
         EbsOptimized: bool = ...,
         EphemeralStorage: bool = ...,
         EndDate: TimestampTypeDef = ...,
         EndDateType: EndDateTypeType = ...,
         InstanceMatchCriteria: InstanceMatchCriteriaType = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         OutpostArn: str = ...,
         PlacementGroupArn: str = ...
     ) -> CreateCapacityReservationResultTypeDef:
         """
         Creates a new Capacity Reservation with the specified attributes.
 
@@ -1715,28 +1715,28 @@
         InstanceTypeSpecifications: Sequence[ReservationFleetInstanceSpecificationTypeDef],
         TotalTargetCapacity: int,
         AllocationStrategy: str = ...,
         ClientToken: str = ...,
         Tenancy: Literal["default"] = ...,
         EndDate: TimestampTypeDef = ...,
         InstanceMatchCriteria: Literal["open"] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateCapacityReservationFleetResultTypeDef:
         """
         Creates a Capacity Reservation Fleet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_capacity_reservation_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_capacity_reservation_fleet)
         """
     async def create_carrier_gateway(
         self,
         *,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...
     ) -> CreateCarrierGatewayResultTypeDef:
         """
         Creates a carrier gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_carrier_gateway)
@@ -1752,15 +1752,15 @@
         DnsServers: Sequence[str] = ...,
         TransportProtocol: TransportProtocolType = ...,
         VpnPort: int = ...,
         Description: str = ...,
         SplitTunnel: bool = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         SecurityGroupIds: Sequence[str] = ...,
         VpcId: str = ...,
         SelfServicePortal: SelfServicePortalType = ...,
         ClientConnectOptions: ClientConnectOptionsTypeDef = ...,
         SessionTimeoutHours: int = ...,
         ClientLoginBannerOptions: ClientLoginBannerOptionsTypeDef = ...
     ) -> CreateClientVpnEndpointResultTypeDef:
@@ -1795,15 +1795,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_coip_cidr)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_coip_cidr)
         """
     async def create_coip_pool(
         self,
         *,
         LocalGatewayRouteTableId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateCoipPoolResultTypeDef:
         """
         Creates a pool of customer-owned IP (CoIP) addresses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_coip_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_coip_pool)
@@ -1811,15 +1811,15 @@
     async def create_customer_gateway(
         self,
         *,
         Type: Literal["ipsec.1"],
         BgpAsn: int = ...,
         PublicIp: str = ...,
         CertificateArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DeviceName: str = ...,
         IpAddress: str = ...,
         DryRun: bool = ...
     ) -> CreateCustomerGatewayResultTypeDef:
         """
         Provides information to Amazon Web Services about your customer gateway device.
 
@@ -1844,30 +1844,30 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_default_vpc)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_default_vpc)
         """
     async def create_dhcp_options(
         self,
         *,
         DhcpConfigurations: Sequence[NewDhcpConfigurationTypeDef],
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateDhcpOptionsResultTypeDef:
         """
         Creates a set of DHCP options for your VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_dhcp_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_dhcp_options)
         """
     async def create_egress_only_internet_gateway(
         self,
         *,
         VpcId: str,
         ClientToken: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateEgressOnlyInternetGatewayResultTypeDef:
         """
         [IPv6 only] Creates an egress-only internet gateway for your VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_egress_only_internet_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_egress_only_internet_gateway)
         """
@@ -1882,15 +1882,15 @@
         OnDemandOptions: OnDemandOptionsRequestTypeDef = ...,
         ExcessCapacityTerminationPolicy: FleetExcessCapacityTerminationPolicyType = ...,
         TerminateInstancesWithExpiration: bool = ...,
         Type: FleetTypeType = ...,
         ValidFrom: TimestampTypeDef = ...,
         ValidUntil: TimestampTypeDef = ...,
         ReplaceUnhealthyInstances: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         Context: str = ...
     ) -> CreateFleetResultTypeDef:
         """
         Creates an EC2 Fleet that contains the configuration information for On-Demand
         Instances and Spot Instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_fleet)
@@ -1906,15 +1906,15 @@
         DeliverLogsPermissionArn: str = ...,
         DeliverCrossAccountRole: str = ...,
         LogGroupName: str = ...,
         TrafficType: TrafficTypeType = ...,
         LogDestinationType: LogDestinationTypeType = ...,
         LogDestination: str = ...,
         LogFormat: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         MaxAggregationInterval: int = ...,
         DestinationOptions: DestinationOptionsRequestTypeDef = ...
     ) -> CreateFlowLogsResultTypeDef:
         """
         Creates one or more flow logs to capture information about IP traffic for a
         specific network interface, subnet, or VPC.
 
@@ -1926,15 +1926,15 @@
         *,
         InputStorageLocation: StorageLocationTypeDef,
         DryRun: bool = ...,
         LogsStorageLocation: StorageLocationTypeDef = ...,
         Description: str = ...,
         Name: str = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateFpgaImageResultTypeDef:
         """
         Creates an Amazon FPGA Image (AFI) from the specified design checkpoint (DCP).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_fpga_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_fpga_image)
         """
@@ -1943,15 +1943,15 @@
         *,
         InstanceId: str,
         Name: str,
         BlockDeviceMappings: Sequence[BlockDeviceMappingTypeDef] = ...,
         Description: str = ...,
         DryRun: bool = ...,
         NoReboot: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateImageResultTypeDef:
         """
         Creates an Amazon EBS-backed AMI from an Amazon EBS-backed instance that is
         either running or stopped.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_image)
@@ -1960,30 +1960,30 @@
         self,
         *,
         SubnetId: str,
         DryRun: bool = ...,
         SecurityGroupIds: Sequence[str] = ...,
         PreserveClientIp: bool = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateInstanceConnectEndpointResultTypeDef:
         """
         Creates an EC2 Instance Connect Endpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_instance_connect_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_instance_connect_endpoint)
         """
     async def create_instance_event_window(
         self,
         *,
         DryRun: bool = ...,
         Name: str = ...,
         TimeRanges: Sequence[InstanceEventWindowTimeRangeRequestTypeDef] = ...,
         CronExpression: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateInstanceEventWindowResultTypeDef:
         """
         Creates an event window in which scheduled events for the associated Amazon EC2
         instances can run.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_instance_event_window)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_instance_event_window)
@@ -1991,38 +1991,38 @@
     async def create_instance_export_task(
         self,
         *,
         ExportToS3Task: ExportToS3TaskSpecificationTypeDef,
         InstanceId: str,
         TargetEnvironment: ExportEnvironmentType,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateInstanceExportTaskResultTypeDef:
         """
         Exports a running or stopped instance to an Amazon S3 bucket.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_instance_export_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_instance_export_task)
         """
     async def create_internet_gateway(
-        self, *, TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ..., DryRun: bool = ...
+        self, *, TagSpecifications: Sequence[TagSpecificationTypeDef] = ..., DryRun: bool = ...
     ) -> CreateInternetGatewayResultTypeDef:
         """
         Creates an internet gateway for use with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_internet_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_internet_gateway)
         """
     async def create_ipam(
         self,
         *,
         DryRun: bool = ...,
         Description: str = ...,
         OperatingRegions: Sequence[AddIpamOperatingRegionTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateIpamResultTypeDef:
         """
         Create an IPAM.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_ipam)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_ipam)
@@ -2038,15 +2038,15 @@
         Description: str = ...,
         AutoImport: bool = ...,
         PubliclyAdvertisable: bool = ...,
         AllocationMinNetmaskLength: int = ...,
         AllocationMaxNetmaskLength: int = ...,
         AllocationDefaultNetmaskLength: int = ...,
         AllocationResourceTags: Sequence[RequestIpamResourceTagTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...,
         AwsService: Literal["ec2"] = ...,
         PublicIpSource: IpamPoolPublicIpSourceType = ...
     ) -> CreateIpamPoolResultTypeDef:
         """
         Create an IP address pool for Amazon VPC IP Address Manager (IPAM).
 
@@ -2055,45 +2055,45 @@
         """
     async def create_ipam_resource_discovery(
         self,
         *,
         DryRun: bool = ...,
         Description: str = ...,
         OperatingRegions: Sequence[AddIpamOperatingRegionTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateIpamResourceDiscoveryResultTypeDef:
         """
         Creates an IPAM resource discovery.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_ipam_resource_discovery)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_ipam_resource_discovery)
         """
     async def create_ipam_scope(
         self,
         *,
         IpamId: str,
         DryRun: bool = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateIpamScopeResultTypeDef:
         """
         Create an IPAM scope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_ipam_scope)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_ipam_scope)
         """
     async def create_key_pair(
         self,
         *,
         KeyName: str,
         DryRun: bool = ...,
         KeyType: KeyTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         KeyFormat: KeyFormatType = ...
     ) -> KeyPairTypeDef:
         """
         Creates an ED25519 or 2048-bit RSA key pair with the specified name and in the
         specified PEM or PPK format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_key_pair)
@@ -2103,15 +2103,15 @@
         self,
         *,
         LaunchTemplateName: str,
         LaunchTemplateData: RequestLaunchTemplateDataTypeDef,
         DryRun: bool = ...,
         ClientToken: str = ...,
         VersionDescription: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateLaunchTemplateResultTypeDef:
         """
         Creates a launch template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_launch_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_launch_template)
         """
@@ -2150,43 +2150,43 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_local_gateway_route)
         """
     async def create_local_gateway_route_table(
         self,
         *,
         LocalGatewayId: str,
         Mode: LocalGatewayRouteTableModeType = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateLocalGatewayRouteTableResultTypeDef:
         """
         Creates a local gateway route table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_local_gateway_route_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_local_gateway_route_table)
         """
     async def create_local_gateway_route_table_virtual_interface_group_association(
         self,
         *,
         LocalGatewayRouteTableId: str,
         LocalGatewayVirtualInterfaceGroupId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationResultTypeDef:
         """
         Creates a local gateway route table virtual interface group association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_local_gateway_route_table_virtual_interface_group_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_local_gateway_route_table_virtual_interface_group_association)
         """
     async def create_local_gateway_route_table_vpc_association(
         self,
         *,
         LocalGatewayRouteTableId: str,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateLocalGatewayRouteTableVpcAssociationResultTypeDef:
         """
         Associates the specified VPC with the specified local gateway route table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_local_gateway_route_table_vpc_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_local_gateway_route_table_vpc_association)
@@ -2195,15 +2195,15 @@
         self,
         *,
         PrefixListName: str,
         MaxEntries: int,
         AddressFamily: str,
         DryRun: bool = ...,
         Entries: Sequence[AddPrefixListEntryTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateManagedPrefixListResultTypeDef:
         """
         Creates a managed prefix list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_managed_prefix_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_managed_prefix_list)
@@ -2211,15 +2211,15 @@
     async def create_nat_gateway(
         self,
         *,
         SubnetId: str,
         AllocationId: str = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ConnectivityType: ConnectivityTypeType = ...,
         PrivateIpAddress: str = ...,
         SecondaryAllocationIds: Sequence[str] = ...,
         SecondaryPrivateIpAddresses: Sequence[str] = ...,
         SecondaryPrivateIpAddressCount: int = ...
     ) -> CreateNatGatewayResultTypeDef:
         """
@@ -2229,15 +2229,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_nat_gateway)
         """
     async def create_network_acl(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateNetworkAclResultTypeDef:
         """
         Creates a network ACL in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_network_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_network_acl)
         """
@@ -2263,15 +2263,15 @@
         """
     async def create_network_insights_access_scope(
         self,
         *,
         ClientToken: str,
         MatchPaths: Sequence[AccessScopePathRequestTypeDef] = ...,
         ExcludePaths: Sequence[AccessScopePathRequestTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateNetworkInsightsAccessScopeResultTypeDef:
         """
         Creates a Network Access Scope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_network_insights_access_scope)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_network_insights_access_scope)
@@ -2282,15 +2282,15 @@
         Source: str,
         Protocol: ProtocolType,
         ClientToken: str,
         SourceIp: str = ...,
         DestinationIp: str = ...,
         Destination: str = ...,
         DestinationPort: int = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         FilterAtSource: PathRequestFilterTypeDef = ...,
         FilterAtDestination: PathRequestFilterTypeDef = ...
     ) -> CreateNetworkInsightsPathResultTypeDef:
         """
         Creates a path to analyze for reachability.
 
@@ -2310,15 +2310,15 @@
         PrivateIpAddresses: Sequence[PrivateIpAddressSpecificationTypeDef] = ...,
         SecondaryPrivateIpAddressCount: int = ...,
         Ipv4Prefixes: Sequence[Ipv4PrefixSpecificationRequestTypeDef] = ...,
         Ipv4PrefixCount: int = ...,
         Ipv6Prefixes: Sequence[Ipv6PrefixSpecificationRequestTypeDef] = ...,
         Ipv6PrefixCount: int = ...,
         InterfaceType: NetworkInterfaceCreationTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> CreateNetworkInterfaceResultTypeDef:
         """
         Creates a network interface in the specified subnet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_network_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_network_interface)
@@ -2342,40 +2342,40 @@
     async def create_placement_group(
         self,
         *,
         DryRun: bool = ...,
         GroupName: str = ...,
         Strategy: PlacementStrategyType = ...,
         PartitionCount: int = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         SpreadLevel: SpreadLevelType = ...
     ) -> CreatePlacementGroupResultTypeDef:
         """
         Creates a placement group in which to launch instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_placement_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_placement_group)
         """
     async def create_public_ipv4_pool(
-        self, *, DryRun: bool = ..., TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        self, *, DryRun: bool = ..., TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreatePublicIpv4PoolResultTypeDef:
         """
         Creates a public IPv4 address pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_public_ipv4_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_public_ipv4_pool)
         """
     async def create_replace_root_volume_task(
         self,
         *,
         InstanceId: str,
         SnapshotId: str = ...,
         ClientToken: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ImageId: str = ...,
         DeleteReplacedRootVolume: bool = ...
     ) -> CreateReplaceRootVolumeTaskResultTypeDef:
         """
         Replaces the EBS-backed root volume for a `running` instance with a new volume
         that is restored to the original root volume's launch state, that is restored to
         a specific snapshot taken from the original root volume, or that is restored
@@ -2401,15 +2401,15 @@
         """
     async def create_restore_image_task(
         self,
         *,
         Bucket: str,
         ObjectKey: str,
         Name: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateRestoreImageTaskResultTypeDef:
         """
         Starts a task that restores an AMI from an Amazon S3 object that was previously
         created by using
         [CreateStoreImageTask](https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_CreateStoreImageTask.html)_.
 
@@ -2443,59 +2443,59 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_route)
         """
     async def create_route_table(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateRouteTableResultTypeDef:
         """
         Creates a route table for the specified VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_route_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_route_table)
         """
     async def create_security_group(
         self,
         *,
         Description: str,
         GroupName: str,
         VpcId: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateSecurityGroupResultTypeDef:
         """
         Creates a security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_security_group)
         """
     async def create_snapshot(
         self,
         *,
         VolumeId: str,
         Description: str = ...,
         OutpostArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> SnapshotResponseTypeDef:
         """
         Creates a snapshot of an EBS volume and stores it in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_snapshot)
         """
     async def create_snapshots(
         self,
         *,
         InstanceSpecification: InstanceSpecificationTypeDef,
         Description: str = ...,
         OutpostArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         CopyTagsFromSource: Literal["volume"] = ...
     ) -> CreateSnapshotsResultTypeDef:
         """
         Creates crash-consistent snapshots of multiple EBS volumes and stores the data
         in S3.
 
@@ -2526,15 +2526,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_store_image_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_store_image_task)
         """
     async def create_subnet(
         self,
         *,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         AvailabilityZone: str = ...,
         AvailabilityZoneId: str = ...,
         CidrBlock: str = ...,
         Ipv6CidrBlock: str = ...,
         OutpostArn: str = ...,
         DryRun: bool = ...,
         Ipv6Native: bool = ...
@@ -2549,15 +2549,15 @@
         self,
         *,
         SubnetId: str,
         Cidr: str,
         ReservationType: SubnetCidrReservationTypeType,
         Description: str = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateSubnetCidrReservationResultTypeDef:
         """
         Creates a subnet CIDR reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_subnet_cidr_reservation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_subnet_cidr_reservation)
         """
@@ -2571,15 +2571,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_tags)
         """
     async def create_traffic_mirror_filter(
         self,
         *,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...
     ) -> CreateTrafficMirrorFilterResultTypeDef:
         """
         Creates a Traffic Mirror filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_traffic_mirror_filter)
@@ -2613,15 +2613,15 @@
         NetworkInterfaceId: str,
         TrafficMirrorTargetId: str,
         TrafficMirrorFilterId: str,
         SessionNumber: int,
         PacketLength: int = ...,
         VirtualNetworkId: int = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...
     ) -> CreateTrafficMirrorSessionResultTypeDef:
         """
         Creates a Traffic Mirror session.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_traffic_mirror_session)
@@ -2629,15 +2629,15 @@
         """
     async def create_traffic_mirror_target(
         self,
         *,
         NetworkInterfaceId: str = ...,
         NetworkLoadBalancerArn: str = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...,
         ClientToken: str = ...,
         GatewayLoadBalancerEndpointId: str = ...
     ) -> CreateTrafficMirrorTargetResultTypeDef:
         """
         Creates a target for your Traffic Mirror session.
 
@@ -2645,29 +2645,29 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_traffic_mirror_target)
         """
     async def create_transit_gateway(
         self,
         *,
         Description: str = ...,
         Options: TransitGatewayRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayResultTypeDef:
         """
         Creates a transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway)
         """
     async def create_transit_gateway_connect(
         self,
         *,
         TransportTransitGatewayAttachmentId: str,
         Options: CreateTransitGatewayConnectRequestOptionsTypeDef,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayConnectResultTypeDef:
         """
         Creates a Connect attachment from a specified transit gateway attachment.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_connect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_connect)
@@ -2676,30 +2676,30 @@
         self,
         *,
         TransitGatewayAttachmentId: str,
         PeerAddress: str,
         InsideCidrBlocks: Sequence[str],
         TransitGatewayAddress: str = ...,
         BgpOptions: TransitGatewayConnectRequestBgpOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayConnectPeerResultTypeDef:
         """
         Creates a Connect peer for a specified transit gateway Connect attachment
         between a transit gateway and an appliance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_connect_peer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_connect_peer)
         """
     async def create_transit_gateway_multicast_domain(
         self,
         *,
         TransitGatewayId: str,
         Options: CreateTransitGatewayMulticastDomainRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayMulticastDomainResultTypeDef:
         """
         Creates a multicast domain using the specified transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_multicast_domain)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_multicast_domain)
@@ -2708,29 +2708,29 @@
         self,
         *,
         TransitGatewayId: str,
         PeerTransitGatewayId: str,
         PeerAccountId: str,
         PeerRegion: str,
         Options: CreateTransitGatewayPeeringAttachmentRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayPeeringAttachmentResultTypeDef:
         """
         Requests a transit gateway peering attachment between the specified transit
         gateway (requester) and a peer transit gateway (accepter).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_peering_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_peering_attachment)
         """
     async def create_transit_gateway_policy_table(
         self,
         *,
         TransitGatewayId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayPolicyTableResultTypeDef:
         """
         Creates a transit gateway policy table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_policy_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_policy_table)
@@ -2766,29 +2766,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_route)
         """
     async def create_transit_gateway_route_table(
         self,
         *,
         TransitGatewayId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayRouteTableResultTypeDef:
         """
         Creates a route table for the specified transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_route_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_route_table)
         """
     async def create_transit_gateway_route_table_announcement(
         self,
         *,
         TransitGatewayRouteTableId: str,
         PeeringAttachmentId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayRouteTableAnnouncementResultTypeDef:
         """
         Advertises a new transit gateway route table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_route_table_announcement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_route_table_announcement)
@@ -2796,15 +2796,15 @@
     async def create_transit_gateway_vpc_attachment(
         self,
         *,
         TransitGatewayId: str,
         VpcId: str,
         SubnetIds: Sequence[str],
         Options: CreateTransitGatewayVpcAttachmentRequestOptionsTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> CreateTransitGatewayVpcAttachmentResultTypeDef:
         """
         Attaches the specified VPC to the specified transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_transit_gateway_vpc_attachment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_transit_gateway_vpc_attachment)
@@ -2819,15 +2819,15 @@
         ApplicationDomain: str,
         EndpointDomainPrefix: str,
         SecurityGroupIds: Sequence[str] = ...,
         LoadBalancerOptions: CreateVerifiedAccessEndpointLoadBalancerOptionsTypeDef = ...,
         NetworkInterfaceOptions: CreateVerifiedAccessEndpointEniOptionsTypeDef = ...,
         Description: str = ...,
         PolicyDocument: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...
     ) -> CreateVerifiedAccessEndpointResultTypeDef:
         """
         An Amazon Web Services Verified Access endpoint is where you define your
         application along with an optional endpoint-level access policy.
 
@@ -2836,15 +2836,15 @@
         """
     async def create_verified_access_group(
         self,
         *,
         VerifiedAccessInstanceId: str,
         Description: str = ...,
         PolicyDocument: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...
     ) -> CreateVerifiedAccessGroupResultTypeDef:
         """
         An Amazon Web Services Verified Access group is a collection of Amazon Web
         Services Verified Access endpoints who's associated applications have similar
         security requirements.
@@ -2852,15 +2852,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_verified_access_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_verified_access_group)
         """
     async def create_verified_access_instance(
         self,
         *,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...
     ) -> CreateVerifiedAccessInstanceResultTypeDef:
         """
         An Amazon Web Services Verified Access instance is a regional entity that
         evaluates application requests and grants access only when your security
         requirements are met.
@@ -2874,15 +2874,15 @@
         TrustProviderType: TrustProviderTypeType,
         PolicyReferenceName: str,
         UserTrustProviderType: UserTrustProviderTypeType = ...,
         DeviceTrustProviderType: DeviceTrustProviderTypeType = ...,
         OidcOptions: CreateVerifiedAccessTrustProviderOidcOptionsTypeDef = ...,
         DeviceOptions: CreateVerifiedAccessTrustProviderDeviceOptionsTypeDef = ...,
         Description: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...,
         DryRun: bool = ...
     ) -> CreateVerifiedAccessTrustProviderResultTypeDef:
         """
         A trust provider is a third-party entity that creates, maintains, and manages
         identity information for users and devices.
 
@@ -2897,15 +2897,15 @@
         Iops: int = ...,
         KmsKeyId: str = ...,
         OutpostArn: str = ...,
         Size: int = ...,
         SnapshotId: str = ...,
         VolumeType: VolumeTypeType = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         MultiAttachEnabled: bool = ...,
         Throughput: int = ...,
         ClientToken: str = ...
     ) -> VolumeResponseTypeDef:
         """
         Creates an EBS volume that can be attached to an instance in the same
         Availability Zone.
@@ -2923,15 +2923,15 @@
         Ipv4IpamPoolId: str = ...,
         Ipv4NetmaskLength: int = ...,
         Ipv6IpamPoolId: str = ...,
         Ipv6NetmaskLength: int = ...,
         DryRun: bool = ...,
         InstanceTenancy: TenancyType = ...,
         Ipv6CidrBlockNetworkBorderGroup: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateVpcResultTypeDef:
         """
         Creates a VPC with the specified CIDR blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_vpc)
         """
@@ -2946,15 +2946,15 @@
         RouteTableIds: Sequence[str] = ...,
         SubnetIds: Sequence[str] = ...,
         SecurityGroupIds: Sequence[str] = ...,
         IpAddressType: IpAddressTypeType = ...,
         DnsOptions: DnsOptionsSpecificationTypeDef = ...,
         ClientToken: str = ...,
         PrivateDnsEnabled: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateVpcEndpointResultTypeDef:
         """
         Creates a VPC endpoint for a specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_endpoint)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_vpc_endpoint)
         """
@@ -2981,15 +2981,15 @@
         DryRun: bool = ...,
         AcceptanceRequired: bool = ...,
         PrivateDnsName: str = ...,
         NetworkLoadBalancerArns: Sequence[str] = ...,
         GatewayLoadBalancerArns: Sequence[str] = ...,
         SupportedIpAddressTypes: Sequence[str] = ...,
         ClientToken: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateVpcEndpointServiceConfigurationResultTypeDef:
         """
         Creates a VPC endpoint service to which service consumers (Amazon Web Services
         accounts, users, and IAM roles) can connect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_endpoint_service_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_vpc_endpoint_service_configuration)
@@ -2998,15 +2998,15 @@
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
         PeerOwnerId: str = ...,
         PeerVpcId: str = ...,
         PeerRegion: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateVpcPeeringConnectionResultTypeDef:
         """
         Requests a VPC peering connection between two VPCs: a requester VPC that you own
         and an accepter VPC with which to create the connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpc_peering_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_vpc_peering_connection)
@@ -3016,15 +3016,15 @@
         *,
         CustomerGatewayId: str,
         Type: str,
         VpnGatewayId: str = ...,
         TransitGatewayId: str = ...,
         DryRun: bool = ...,
         Options: VpnConnectionOptionsSpecificationTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> CreateVpnConnectionResultTypeDef:
         """
         Creates a VPN connection between an existing virtual private gateway or transit
         gateway and a customer gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpn_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_vpn_connection)
@@ -3040,15 +3040,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#create_vpn_connection_route)
         """
     async def create_vpn_gateway(
         self,
         *,
         Type: Literal["ipsec.1"],
         AvailabilityZone: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         AmazonSideAsn: int = ...,
         DryRun: bool = ...
     ) -> CreateVpnGatewayResultTypeDef:
         """
         Creates a virtual private gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.create_vpn_gateway)
@@ -5977,15 +5977,15 @@
         self,
         *,
         VolumeId: str,
         Device: str = ...,
         Force: bool = ...,
         InstanceId: str = ...,
         DryRun: bool = ...
-    ) -> VolumeAttachmentResponseTypeDef:
+    ) -> VolumeAttachmentTypeDef:
         """
         Detaches an EBS volume from an instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.detach_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#detach_volume)
         """
     async def detach_vpn_gateway(
@@ -6453,15 +6453,15 @@
         DiskImageFormat: DiskImageFormatType,
         ImageId: str,
         S3ExportLocation: ExportTaskS3LocationRequestTypeDef,
         ClientToken: str = ...,
         Description: str = ...,
         DryRun: bool = ...,
         RoleName: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> ExportImageResultTypeDef:
         """
         Exports an Amazon Machine Image (AMI) to a VM file.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.export_image)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#export_image)
         """
@@ -7081,15 +7081,15 @@
         Encrypted: bool = ...,
         Hypervisor: str = ...,
         KmsKeyId: str = ...,
         LicenseType: str = ...,
         Platform: str = ...,
         RoleName: str = ...,
         LicenseSpecifications: Sequence[ImportImageLicenseConfigurationRequestTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         UsageOperation: str = ...,
         BootMode: BootModeValuesType = ...
     ) -> ImportImageResultTypeDef:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_image)
@@ -7112,15 +7112,15 @@
         """
     async def import_key_pair(
         self,
         *,
         KeyName: str,
         PublicKeyMaterial: BlobTypeDef,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> ImportKeyPairResultTypeDef:
         """
         Imports the public key from an RSA or ED25519 key pair that you created with a
         third-party tool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_key_pair)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#import_key_pair)
@@ -7132,15 +7132,15 @@
         ClientToken: str = ...,
         Description: str = ...,
         DiskContainer: SnapshotDiskContainerTypeDef = ...,
         DryRun: bool = ...,
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         RoleName: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> ImportSnapshotResultTypeDef:
         """
         Imports a disk into an EBS snapshot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.import_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#import_snapshot)
         """
@@ -7728,15 +7728,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#modify_snapshot_tier)
         """
     async def modify_spot_fleet_request(
         self,
         *,
         SpotFleetRequestId: str,
         ExcessCapacityTerminationPolicy: ExcessCapacityTerminationPolicyType = ...,
-        LaunchTemplateConfigs: Sequence[LaunchTemplateConfigUnionTypeDef] = ...,
+        LaunchTemplateConfigs: Sequence[LaunchTemplateConfigTypeDef] = ...,
         TargetCapacity: int = ...,
         OnDemandTargetCapacity: int = ...,
         Context: str = ...
     ) -> ModifySpotFleetRequestResponseTypeDef:
         """
         Modifies the specified Spot Fleet request.
 
@@ -8206,15 +8206,15 @@
         self,
         *,
         Cidr: str,
         CidrAuthorizationContext: CidrAuthorizationContextTypeDef = ...,
         PubliclyAdvertisable: bool = ...,
         Description: str = ...,
         DryRun: bool = ...,
-        PoolTagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        PoolTagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         MultiRegion: bool = ...
     ) -> ProvisionByoipCidrResultTypeDef:
         """
         Provisions an IPv4 or IPv6 address range for use with your Amazon Web Services
         resources through bring your own IP addresses (BYOIP) and creates a
         corresponding address pool.
 
@@ -8250,15 +8250,15 @@
         self,
         *,
         HostIdSet: Sequence[str],
         OfferingId: str,
         ClientToken: str = ...,
         CurrencyCode: Literal["USD"] = ...,
         LimitPrice: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> PurchaseHostReservationResultTypeDef:
         """
         Purchase a reservation with configurations that match those of your Dedicated
         Host.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.purchase_host_reservation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#purchase_host_reservation)
@@ -8568,15 +8568,15 @@
         """
         Submits feedback about the status of an instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.report_instance_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#report_instance_status)
         """
     async def request_spot_fleet(
-        self, *, SpotFleetRequestConfig: SpotFleetRequestConfigDataUnionTypeDef, DryRun: bool = ...
+        self, *, SpotFleetRequestConfig: SpotFleetRequestConfigDataTypeDef, DryRun: bool = ...
     ) -> RequestSpotFleetResponseTypeDef:
         """
         Creates a Spot Fleet request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.request_spot_fleet)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#request_spot_fleet)
         """
@@ -8590,15 +8590,15 @@
         InstanceCount: int = ...,
         LaunchGroup: str = ...,
         LaunchSpecification: RequestSpotLaunchSpecificationTypeDef = ...,
         SpotPrice: str = ...,
         Type: SpotInstanceTypeType = ...,
         ValidFrom: TimestampTypeDef = ...,
         ValidUntil: TimestampTypeDef = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         InstanceInterruptionBehavior: InstanceInterruptionBehaviorType = ...
     ) -> RequestSpotInstancesResultTypeDef:
         """
         Creates a Spot Instance request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.request_spot_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#request_spot_instances)
@@ -8737,15 +8737,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#revoke_client_vpn_ingress)
         """
     async def revoke_security_group_egress(
         self,
         *,
         GroupId: str,
         DryRun: bool = ...,
-        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
         SecurityGroupRuleIds: Sequence[str] = ...,
         CidrIp: str = ...,
         FromPort: int = ...,
         IpProtocol: str = ...,
         ToPort: int = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...
@@ -8760,15 +8760,15 @@
     async def revoke_security_group_ingress(
         self,
         *,
         CidrIp: str = ...,
         FromPort: int = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
         IpProtocol: str = ...,
         SourceSecurityGroupName: str = ...,
         SourceSecurityGroupOwnerId: str = ...,
         ToPort: int = ...,
         DryRun: bool = ...,
         SecurityGroupRuleIds: Sequence[str] = ...
     ) -> RevokeSecurityGroupIngressResultTypeDef:
@@ -8800,19 +8800,19 @@
         AdditionalInfo: str = ...,
         ClientToken: str = ...,
         DisableApiTermination: bool = ...,
         DryRun: bool = ...,
         EbsOptimized: bool = ...,
         IamInstanceProfile: IamInstanceProfileSpecificationTypeDef = ...,
         InstanceInitiatedShutdownBehavior: ShutdownBehaviorType = ...,
-        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef] = ...,
+        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationTypeDef] = ...,
         PrivateIpAddress: str = ...,
         ElasticGpuSpecification: Sequence[ElasticGpuSpecificationTypeDef] = ...,
         ElasticInferenceAccelerators: Sequence[ElasticInferenceAcceleratorTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         InstanceMarketOptions: InstanceMarketOptionsRequestTypeDef = ...,
         CreditSpecification: CreditSpecificationRequestTypeDef = ...,
         CpuOptions: CpuOptionsRequestTypeDef = ...,
         CapacityReservationSpecification: CapacityReservationSpecificationTypeDef = ...,
         HibernationOptions: HibernationOptionsRequestTypeDef = ...,
         LicenseSpecifications: Sequence[LicenseConfigurationRequestTypeDef] = ...,
@@ -8911,15 +8911,15 @@
         """
     async def start_network_insights_access_scope_analysis(
         self,
         *,
         NetworkInsightsAccessScopeId: str,
         ClientToken: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> StartNetworkInsightsAccessScopeAnalysisResultTypeDef:
         """
         Starts analyzing the specified Network Access Scope.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.start_network_insights_access_scope_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#start_network_insights_access_scope_analysis)
         """
@@ -8927,15 +8927,15 @@
         self,
         *,
         NetworkInsightsPathId: str,
         ClientToken: str,
         AdditionalAccounts: Sequence[str] = ...,
         FilterInArns: Sequence[str] = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> StartNetworkInsightsAnalysisResultTypeDef:
         """
         Starts analyzing the specified path.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.start_network_insights_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#start_network_insights_analysis)
         """
@@ -9039,30 +9039,30 @@
         """
     async def update_security_group_rule_descriptions_egress(
         self,
         *,
         DryRun: bool = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
         SecurityGroupRuleDescriptions: Sequence[SecurityGroupRuleDescriptionTypeDef] = ...
     ) -> UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef:
         """
         [VPC only] Updates the description of an egress (outbound) security group rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.update_security_group_rule_descriptions_egress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#update_security_group_rule_descriptions_egress)
         """
     async def update_security_group_rule_descriptions_ingress(
         self,
         *,
         DryRun: bool = ...,
         GroupId: str = ...,
         GroupName: str = ...,
-        IpPermissions: Sequence[IpPermissionUnionTypeDef] = ...,
+        IpPermissions: Sequence[IpPermissionTypeDef] = ...,
         SecurityGroupRuleDescriptions: Sequence[SecurityGroupRuleDescriptionTypeDef] = ...
     ) -> UpdateSecurityGroupRuleDescriptionsIngressResultTypeDef:
         """
         Updates the description of an ingress (inbound) security group rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Client.update_security_group_rule_descriptions_ingress)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/client/#update_security_group_rule_descriptions_ingress)
```

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/literals.py` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/literals.pyi` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/paginator.py` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -381,19 +381,19 @@
     DescribeReplaceRootVolumeTasksResultTypeDef,
     DescribeReservedInstancesModificationsResultTypeDef,
     DescribeReservedInstancesOfferingsResultTypeDef,
     DescribeRouteTablesResultTypeDef,
     DescribeScheduledInstanceAvailabilityResultTypeDef,
     DescribeScheduledInstancesResultTypeDef,
     DescribeSecurityGroupRulesResultTypeDef,
-    DescribeSecurityGroupsResultTypeDef,
+    DescribeSecurityGroupsResultVpcAddressTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeSnapshotTierStatusResultTypeDef,
     DescribeSpotFleetInstancesResponseTypeDef,
-    DescribeSpotFleetRequestsResponseTypeDef,
+    DescribeSpotFleetRequestsResponseVpcAddressTypeDef,
     DescribeSpotInstanceRequestsResultTypeDef,
     DescribeSpotPriceHistoryResultTypeDef,
     DescribeStaleSecurityGroupsResultTypeDef,
     DescribeStoreImageTasksResultTypeDef,
     DescribeSubnetsResultTypeDef,
     DescribeTagsResultTypeDef,
     DescribeTrafficMirrorFiltersResultTypeDef,
@@ -2071,15 +2071,15 @@
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         GroupIds: Sequence[str] = ...,
         GroupNames: Sequence[str] = ...,
         DryRun: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[DescribeSecurityGroupsResultTypeDef]:
+    ) -> AsyncIterator[DescribeSecurityGroupsResultVpcAddressTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSecurityGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/paginators/#describesecuritygroupspaginator)
         """
 
 
 class DescribeSnapshotTierStatusPaginator(AioPaginator):
@@ -2150,15 +2150,15 @@
 
     def paginate(
         self,
         *,
         DryRun: bool = ...,
         SpotFleetRequestIds: Sequence[str] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[DescribeSpotFleetRequestsResponseTypeDef]:
+    ) -> AsyncIterator[DescribeSpotFleetRequestsResponseVpcAddressTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSpotFleetRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/paginators/#describespotfleetrequestspaginator)
         """
 
 
 class DescribeSpotInstanceRequestsPaginator(AioPaginator):
```

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/paginator.pyi` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -381,19 +381,19 @@
     DescribeReplaceRootVolumeTasksResultTypeDef,
     DescribeReservedInstancesModificationsResultTypeDef,
     DescribeReservedInstancesOfferingsResultTypeDef,
     DescribeRouteTablesResultTypeDef,
     DescribeScheduledInstanceAvailabilityResultTypeDef,
     DescribeScheduledInstancesResultTypeDef,
     DescribeSecurityGroupRulesResultTypeDef,
-    DescribeSecurityGroupsResultTypeDef,
+    DescribeSecurityGroupsResultVpcAddressTypeDef,
     DescribeSnapshotsResultTypeDef,
     DescribeSnapshotTierStatusResultTypeDef,
     DescribeSpotFleetInstancesResponseTypeDef,
-    DescribeSpotFleetRequestsResponseTypeDef,
+    DescribeSpotFleetRequestsResponseVpcAddressTypeDef,
     DescribeSpotInstanceRequestsResultTypeDef,
     DescribeSpotPriceHistoryResultTypeDef,
     DescribeStaleSecurityGroupsResultTypeDef,
     DescribeStoreImageTasksResultTypeDef,
     DescribeSubnetsResultTypeDef,
     DescribeTagsResultTypeDef,
     DescribeTrafficMirrorFiltersResultTypeDef,
@@ -1996,15 +1996,15 @@
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
         GroupIds: Sequence[str] = ...,
         GroupNames: Sequence[str] = ...,
         DryRun: bool = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[DescribeSecurityGroupsResultTypeDef]:
+    ) -> AsyncIterator[DescribeSecurityGroupsResultVpcAddressTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSecurityGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/paginators/#describesecuritygroupspaginator)
         """
 
 class DescribeSnapshotTierStatusPaginator(AioPaginator):
     """
@@ -2071,15 +2071,15 @@
 
     def paginate(
         self,
         *,
         DryRun: bool = ...,
         SpotFleetRequestIds: Sequence[str] = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> AsyncIterator[DescribeSpotFleetRequestsResponseTypeDef]:
+    ) -> AsyncIterator[DescribeSpotFleetRequestsResponseVpcAddressTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Paginator.DescribeSpotFleetRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/paginators/#describespotfleetrequestspaginator)
         """
 
 class DescribeSpotInstanceRequestsPaginator(AioPaginator):
     """
```

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/service_resource.py` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,20 +138,19 @@
     InstanceBlockDeviceMappingTypeDef,
     InstanceIpv6AddressTypeDef,
     InstanceMaintenanceOptionsRequestTypeDef,
     InstanceMaintenanceOptionsResponseTypeDef,
     InstanceMarketOptionsRequestTypeDef,
     InstanceMetadataOptionsRequestTypeDef,
     InstanceMetadataOptionsResponseResponseTypeDef,
-    InstanceNetworkInterfaceSpecificationTypeDef,
-    InstanceNetworkInterfaceSpecificationUnionTypeDef,
+    InstanceNetworkInterfaceSpecificationServiceResourceTypeDef,
+    InstanceNetworkInterfaceSpecificationSubnetTypeDef,
     InstanceNetworkInterfaceTypeDef,
     InstanceStateResponseTypeDef,
     InternetGatewayAttachmentTypeDef,
-    IpPermissionOutputTypeDef,
     IpPermissionTypeDef,
     Ipv4PrefixSpecificationRequestTypeDef,
     Ipv4PrefixSpecificationTypeDef,
     Ipv6PrefixSpecificationRequestTypeDef,
     Ipv6PrefixSpecificationTypeDef,
     LaunchPermissionModificationsTypeDef,
     LaunchTemplateSpecificationTypeDef,
@@ -182,18 +181,18 @@
     RevokeSecurityGroupIngressResultTypeDef,
     RouteTableAssociationStateResponseTypeDef,
     RouteTableAssociationTypeDef,
     RouteTypeDef,
     RunInstancesMonitoringEnabledTypeDef,
     StartInstancesResultTypeDef,
     StateReasonResponseTypeDef,
+    StateReasonTypeDef,
     StopInstancesResultTypeDef,
     SubnetIpv6CidrBlockAssociationTypeDef,
     TagSpecificationTypeDef,
-    TagSpecificationUnionTypeDef,
     TagTypeDef,
     TerminateInstancesResultTypeDef,
     TimestampTypeDef,
     UnmonitorInstancesResultTypeDef,
     VolumeAttachmentResponseTypeDef,
     VolumeAttachmentTypeDef,
     VpcCidrBlockAssociationTypeDef,
@@ -2561,15 +2560,15 @@
     ena_support: Awaitable[bool]
     hypervisor: Awaitable[HypervisorTypeType]
     image_owner_alias: Awaitable[str]
     name: Awaitable[str]
     root_device_name: Awaitable[str]
     root_device_type: Awaitable[DeviceTypeType]
     sriov_net_support: Awaitable[str]
-    state_reason: Awaitable[StateReasonResponseTypeDef]
+    state_reason: Awaitable[StateReasonTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     virtualization_type: Awaitable[VirtualizationTypeType]
     boot_mode: Awaitable[BootModeValuesType]
     tpm_support: Awaitable[Literal["v2.0"]]
     deprecation_time: Awaitable[str]
     imds_support: Awaitable[Literal["v2.0"]]
     id: str
@@ -3360,18 +3359,18 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.SecurityGroup)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#securitygroup)
     """
 
     description: Awaitable[str]
     group_name: Awaitable[str]
-    ip_permissions: Awaitable[List[IpPermissionOutputTypeDef]]
+    ip_permissions: Awaitable[List[IpPermissionTypeDef]]
     owner_id: Awaitable[str]
     group_id: Awaitable[str]
-    ip_permissions_egress: Awaitable[List[IpPermissionOutputTypeDef]]
+    ip_permissions_egress: Awaitable[List[IpPermissionTypeDef]]
     tags: Awaitable[List[TagTypeDef]]
     vpc_id: Awaitable[str]
     id: str
 
     async def authorize_egress(
         self,
         *,
@@ -3999,15 +3998,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Instance.attach_classic_link_vpc)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#instanceattach_classic_link_vpc-method)
         """
 
     async def attach_volume(
         self, *, Device: str, VolumeId: str, DryRun: bool = ...
-    ) -> VolumeAttachmentResponseTypeDef:
+    ) -> VolumeAttachmentTypeDef:
         """
         Attaches an EBS volume to a running or stopped instance and exposes it to the
         instance with the specified device name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Instance.attach_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#instanceattach_volume-method)
         """
@@ -4075,15 +4074,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Instance.detach_classic_link_vpc)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#instancedetach_classic_link_vpc-method)
         """
 
     async def detach_volume(
         self, *, VolumeId: str, Device: str = ..., Force: bool = ..., DryRun: bool = ...
-    ) -> VolumeAttachmentResponseTypeDef:
+    ) -> VolumeAttachmentTypeDef:
         """
         Detaches an EBS volume from an instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Instance.detach_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#instancedetach_volume-method)
         """
 
@@ -4791,15 +4790,15 @@
         AdditionalInfo: str = ...,
         ClientToken: str = ...,
         DisableApiTermination: bool = ...,
         DryRun: bool = ...,
         EbsOptimized: bool = ...,
         IamInstanceProfile: IamInstanceProfileSpecificationTypeDef = ...,
         InstanceInitiatedShutdownBehavior: ShutdownBehaviorType = ...,
-        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationTypeDef] = ...,
+        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationSubnetTypeDef] = ...,
         PrivateIpAddress: str = ...,
         ElasticGpuSpecification: Sequence[ElasticGpuSpecificationTypeDef] = ...,
         ElasticInferenceAccelerators: Sequence[ElasticInferenceAcceleratorTypeDef] = ...,
         TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         InstanceMarketOptions: InstanceMarketOptionsRequestTypeDef = ...,
         CreditSpecification: CreditSpecificationRequestTypeDef = ...,
@@ -5402,15 +5401,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcevpcpeeringconnection-method)
         """
 
     async def create_dhcp_options(
         self,
         *,
         DhcpConfigurations: Sequence[NewDhcpConfigurationTypeDef],
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> _DhcpOptions:
         """
         Creates a set of DHCP options for your VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_dhcp_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_dhcp_options-method)
@@ -5438,19 +5437,21 @@
         AdditionalInfo: str = ...,
         ClientToken: str = ...,
         DisableApiTermination: bool = ...,
         DryRun: bool = ...,
         EbsOptimized: bool = ...,
         IamInstanceProfile: IamInstanceProfileSpecificationTypeDef = ...,
         InstanceInitiatedShutdownBehavior: ShutdownBehaviorType = ...,
-        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef] = ...,
+        NetworkInterfaces: Sequence[
+            InstanceNetworkInterfaceSpecificationServiceResourceTypeDef
+        ] = ...,
         PrivateIpAddress: str = ...,
         ElasticGpuSpecification: Sequence[ElasticGpuSpecificationTypeDef] = ...,
         ElasticInferenceAccelerators: Sequence[ElasticInferenceAcceleratorTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         InstanceMarketOptions: InstanceMarketOptionsRequestTypeDef = ...,
         CreditSpecification: CreditSpecificationRequestTypeDef = ...,
         CpuOptions: CpuOptionsRequestTypeDef = ...,
         CapacityReservationSpecification: CapacityReservationSpecificationTypeDef = ...,
         HibernationOptions: HibernationOptionsRequestTypeDef = ...,
         LicenseSpecifications: Sequence[LicenseConfigurationRequestTypeDef] = ...,
@@ -5465,30 +5466,30 @@
         permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_instances-method)
         """
 
     async def create_internet_gateway(
-        self, *, TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ..., DryRun: bool = ...
+        self, *, TagSpecifications: Sequence[TagSpecificationTypeDef] = ..., DryRun: bool = ...
     ) -> _InternetGateway:
         """
         Creates an internet gateway for use with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_internet_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_internet_gateway-method)
         """
 
     async def create_key_pair(
         self,
         *,
         KeyName: str,
         DryRun: bool = ...,
         KeyType: KeyTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         KeyFormat: KeyFormatType = ...
     ) -> _KeyPair:
         """
         Creates an ED25519 or 2048-bit RSA key pair with the specified name and in the
         specified PEM or PPK format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_key_pair)
@@ -5496,15 +5497,15 @@
         """
 
     async def create_network_acl(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> _NetworkAcl:
         """
         Creates a network ACL in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_network_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_network_acl-method)
         """
@@ -5522,15 +5523,15 @@
         PrivateIpAddresses: Sequence[PrivateIpAddressSpecificationTypeDef] = ...,
         SecondaryPrivateIpAddressCount: int = ...,
         Ipv4Prefixes: Sequence[Ipv4PrefixSpecificationRequestTypeDef] = ...,
         Ipv4PrefixCount: int = ...,
         Ipv6Prefixes: Sequence[Ipv6PrefixSpecificationRequestTypeDef] = ...,
         Ipv6PrefixCount: int = ...,
         InterfaceType: NetworkInterfaceCreationTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> _NetworkInterface:
         """
         Creates a network interface in the specified subnet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_network_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_network_interface-method)
@@ -5539,45 +5540,45 @@
     async def create_placement_group(
         self,
         *,
         DryRun: bool = ...,
         GroupName: str = ...,
         Strategy: PlacementStrategyType = ...,
         PartitionCount: int = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         SpreadLevel: SpreadLevelType = ...
     ) -> _PlacementGroup:
         """
         Creates a placement group in which to launch instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_placement_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_placement_group-method)
         """
 
     async def create_route_table(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> _RouteTable:
         """
         Creates a route table for the specified VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_route_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_route_table-method)
         """
 
     async def create_security_group(
         self,
         *,
         Description: str,
         GroupName: str,
         VpcId: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> _SecurityGroup:
         """
         Creates a security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_security_group-method)
@@ -5585,29 +5586,29 @@
 
     async def create_snapshot(
         self,
         *,
         VolumeId: str,
         Description: str = ...,
         OutpostArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> _Snapshot:
         """
         Creates a snapshot of an EBS volume and stores it in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_snapshot-method)
         """
 
     async def create_subnet(
         self,
         *,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         AvailabilityZone: str = ...,
         AvailabilityZoneId: str = ...,
         CidrBlock: str = ...,
         Ipv6CidrBlock: str = ...,
         OutpostArn: str = ...,
         DryRun: bool = ...,
         Ipv6Native: bool = ...
@@ -5635,15 +5636,15 @@
         Iops: int = ...,
         KmsKeyId: str = ...,
         OutpostArn: str = ...,
         Size: int = ...,
         SnapshotId: str = ...,
         VolumeType: VolumeTypeType = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         MultiAttachEnabled: bool = ...,
         Throughput: int = ...,
         ClientToken: str = ...
     ) -> _Volume:
         """
         Creates an EBS volume that can be attached to an instance in the same
         Availability Zone.
@@ -5662,15 +5663,15 @@
         Ipv4IpamPoolId: str = ...,
         Ipv4NetmaskLength: int = ...,
         Ipv6IpamPoolId: str = ...,
         Ipv6NetmaskLength: int = ...,
         DryRun: bool = ...,
         InstanceTenancy: TenancyType = ...,
         Ipv6CidrBlockNetworkBorderGroup: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> _Vpc:
         """
         Creates a VPC with the specified CIDR blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_vpc)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_vpc-method)
         """
@@ -5679,15 +5680,15 @@
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
         PeerOwnerId: str = ...,
         PeerVpcId: str = ...,
         PeerRegion: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> _VpcPeeringConnection:
         """
         Requests a VPC peering connection between two VPCs: a requester VPC that you own
         and an accepter VPC with which to create the connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_vpc_peering_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_vpc_peering_connection-method)
@@ -5711,15 +5712,15 @@
 
     async def import_key_pair(
         self,
         *,
         KeyName: str,
         PublicKeyMaterial: BlobTypeDef,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> _KeyPairInfo:
         """
         Imports the public key from an RSA or ED25519 key pair that you created with a
         third-party tool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.import_key_pair)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourceimport_key_pair-method)
```

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/service_resource.pyi` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -138,20 +138,19 @@
     InstanceBlockDeviceMappingTypeDef,
     InstanceIpv6AddressTypeDef,
     InstanceMaintenanceOptionsRequestTypeDef,
     InstanceMaintenanceOptionsResponseTypeDef,
     InstanceMarketOptionsRequestTypeDef,
     InstanceMetadataOptionsRequestTypeDef,
     InstanceMetadataOptionsResponseResponseTypeDef,
-    InstanceNetworkInterfaceSpecificationTypeDef,
-    InstanceNetworkInterfaceSpecificationUnionTypeDef,
+    InstanceNetworkInterfaceSpecificationServiceResourceTypeDef,
+    InstanceNetworkInterfaceSpecificationSubnetTypeDef,
     InstanceNetworkInterfaceTypeDef,
     InstanceStateResponseTypeDef,
     InternetGatewayAttachmentTypeDef,
-    IpPermissionOutputTypeDef,
     IpPermissionTypeDef,
     Ipv4PrefixSpecificationRequestTypeDef,
     Ipv4PrefixSpecificationTypeDef,
     Ipv6PrefixSpecificationRequestTypeDef,
     Ipv6PrefixSpecificationTypeDef,
     LaunchPermissionModificationsTypeDef,
     LaunchTemplateSpecificationTypeDef,
@@ -182,18 +181,18 @@
     RevokeSecurityGroupIngressResultTypeDef,
     RouteTableAssociationStateResponseTypeDef,
     RouteTableAssociationTypeDef,
     RouteTypeDef,
     RunInstancesMonitoringEnabledTypeDef,
     StartInstancesResultTypeDef,
     StateReasonResponseTypeDef,
+    StateReasonTypeDef,
     StopInstancesResultTypeDef,
     SubnetIpv6CidrBlockAssociationTypeDef,
     TagSpecificationTypeDef,
-    TagSpecificationUnionTypeDef,
     TagTypeDef,
     TerminateInstancesResultTypeDef,
     TimestampTypeDef,
     UnmonitorInstancesResultTypeDef,
     VolumeAttachmentResponseTypeDef,
     VolumeAttachmentTypeDef,
     VpcCidrBlockAssociationTypeDef,
@@ -2293,15 +2292,15 @@
     ena_support: Awaitable[bool]
     hypervisor: Awaitable[HypervisorTypeType]
     image_owner_alias: Awaitable[str]
     name: Awaitable[str]
     root_device_name: Awaitable[str]
     root_device_type: Awaitable[DeviceTypeType]
     sriov_net_support: Awaitable[str]
-    state_reason: Awaitable[StateReasonResponseTypeDef]
+    state_reason: Awaitable[StateReasonTypeDef]
     tags: Awaitable[List[TagTypeDef]]
     virtualization_type: Awaitable[VirtualizationTypeType]
     boot_mode: Awaitable[BootModeValuesType]
     tpm_support: Awaitable[Literal["v2.0"]]
     deprecation_time: Awaitable[str]
     imds_support: Awaitable[Literal["v2.0"]]
     id: str
@@ -3033,18 +3032,18 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.SecurityGroup)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#securitygroup)
     """
 
     description: Awaitable[str]
     group_name: Awaitable[str]
-    ip_permissions: Awaitable[List[IpPermissionOutputTypeDef]]
+    ip_permissions: Awaitable[List[IpPermissionTypeDef]]
     owner_id: Awaitable[str]
     group_id: Awaitable[str]
-    ip_permissions_egress: Awaitable[List[IpPermissionOutputTypeDef]]
+    ip_permissions_egress: Awaitable[List[IpPermissionTypeDef]]
     tags: Awaitable[List[TagTypeDef]]
     vpc_id: Awaitable[str]
     id: str
 
     async def authorize_egress(
         self,
         *,
@@ -3631,15 +3630,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Instance.attach_classic_link_vpc)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#instanceattach_classic_link_vpc-method)
         """
     async def attach_volume(
         self, *, Device: str, VolumeId: str, DryRun: bool = ...
-    ) -> VolumeAttachmentResponseTypeDef:
+    ) -> VolumeAttachmentTypeDef:
         """
         Attaches an EBS volume to a running or stopped instance and exposes it to the
         instance with the specified device name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Instance.attach_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#instanceattach_volume-method)
         """
@@ -3700,15 +3699,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Instance.detach_classic_link_vpc)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#instancedetach_classic_link_vpc-method)
         """
     async def detach_volume(
         self, *, VolumeId: str, Device: str = ..., Force: bool = ..., DryRun: bool = ...
-    ) -> VolumeAttachmentResponseTypeDef:
+    ) -> VolumeAttachmentTypeDef:
         """
         Detaches an EBS volume from an instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.Instance.detach_volume)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#instancedetach_volume-method)
         """
     async def get_available_subresources(self) -> Sequence[str]:
@@ -4364,15 +4363,15 @@
         AdditionalInfo: str = ...,
         ClientToken: str = ...,
         DisableApiTermination: bool = ...,
         DryRun: bool = ...,
         EbsOptimized: bool = ...,
         IamInstanceProfile: IamInstanceProfileSpecificationTypeDef = ...,
         InstanceInitiatedShutdownBehavior: ShutdownBehaviorType = ...,
-        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationTypeDef] = ...,
+        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationSubnetTypeDef] = ...,
         PrivateIpAddress: str = ...,
         ElasticGpuSpecification: Sequence[ElasticGpuSpecificationTypeDef] = ...,
         ElasticInferenceAccelerators: Sequence[ElasticInferenceAcceleratorTypeDef] = ...,
         TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         InstanceMarketOptions: InstanceMarketOptionsRequestTypeDef = ...,
         CreditSpecification: CreditSpecificationRequestTypeDef = ...,
@@ -4923,15 +4922,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.VpcPeeringConnection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcevpcpeeringconnection-method)
         """
     async def create_dhcp_options(
         self,
         *,
         DhcpConfigurations: Sequence[NewDhcpConfigurationTypeDef],
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> _DhcpOptions:
         """
         Creates a set of DHCP options for your VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_dhcp_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_dhcp_options-method)
@@ -4958,19 +4957,21 @@
         AdditionalInfo: str = ...,
         ClientToken: str = ...,
         DisableApiTermination: bool = ...,
         DryRun: bool = ...,
         EbsOptimized: bool = ...,
         IamInstanceProfile: IamInstanceProfileSpecificationTypeDef = ...,
         InstanceInitiatedShutdownBehavior: ShutdownBehaviorType = ...,
-        NetworkInterfaces: Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef] = ...,
+        NetworkInterfaces: Sequence[
+            InstanceNetworkInterfaceSpecificationServiceResourceTypeDef
+        ] = ...,
         PrivateIpAddress: str = ...,
         ElasticGpuSpecification: Sequence[ElasticGpuSpecificationTypeDef] = ...,
         ElasticInferenceAccelerators: Sequence[ElasticInferenceAcceleratorTypeDef] = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         LaunchTemplate: LaunchTemplateSpecificationTypeDef = ...,
         InstanceMarketOptions: InstanceMarketOptionsRequestTypeDef = ...,
         CreditSpecification: CreditSpecificationRequestTypeDef = ...,
         CpuOptions: CpuOptionsRequestTypeDef = ...,
         CapacityReservationSpecification: CapacityReservationSpecificationTypeDef = ...,
         HibernationOptions: HibernationOptionsRequestTypeDef = ...,
         LicenseSpecifications: Sequence[LicenseConfigurationRequestTypeDef] = ...,
@@ -4984,44 +4985,44 @@
         Launches the specified number of instances using an AMI for which you have
         permissions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_instances)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_instances-method)
         """
     async def create_internet_gateway(
-        self, *, TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ..., DryRun: bool = ...
+        self, *, TagSpecifications: Sequence[TagSpecificationTypeDef] = ..., DryRun: bool = ...
     ) -> _InternetGateway:
         """
         Creates an internet gateway for use with a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_internet_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_internet_gateway-method)
         """
     async def create_key_pair(
         self,
         *,
         KeyName: str,
         DryRun: bool = ...,
         KeyType: KeyTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         KeyFormat: KeyFormatType = ...
     ) -> _KeyPair:
         """
         Creates an ED25519 or 2048-bit RSA key pair with the specified name and in the
         specified PEM or PPK format.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_key_pair)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_key_pair-method)
         """
     async def create_network_acl(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> _NetworkAcl:
         """
         Creates a network ACL in a VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_network_acl)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_network_acl-method)
         """
@@ -5038,15 +5039,15 @@
         PrivateIpAddresses: Sequence[PrivateIpAddressSpecificationTypeDef] = ...,
         SecondaryPrivateIpAddressCount: int = ...,
         Ipv4Prefixes: Sequence[Ipv4PrefixSpecificationRequestTypeDef] = ...,
         Ipv4PrefixCount: int = ...,
         Ipv6Prefixes: Sequence[Ipv6PrefixSpecificationRequestTypeDef] = ...,
         Ipv6PrefixCount: int = ...,
         InterfaceType: NetworkInterfaceCreationTypeType = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         ClientToken: str = ...
     ) -> _NetworkInterface:
         """
         Creates a network interface in the specified subnet.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_network_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_network_interface-method)
@@ -5054,71 +5055,71 @@
     async def create_placement_group(
         self,
         *,
         DryRun: bool = ...,
         GroupName: str = ...,
         Strategy: PlacementStrategyType = ...,
         PartitionCount: int = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         SpreadLevel: SpreadLevelType = ...
     ) -> _PlacementGroup:
         """
         Creates a placement group in which to launch instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_placement_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_placement_group-method)
         """
     async def create_route_table(
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> _RouteTable:
         """
         Creates a route table for the specified VPC.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_route_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_route_table-method)
         """
     async def create_security_group(
         self,
         *,
         Description: str,
         GroupName: str,
         VpcId: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> _SecurityGroup:
         """
         Creates a security group.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_security_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_security_group-method)
         """
     async def create_snapshot(
         self,
         *,
         VolumeId: str,
         Description: str = ...,
         OutpostArn: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         DryRun: bool = ...
     ) -> _Snapshot:
         """
         Creates a snapshot of an EBS volume and stores it in Amazon S3.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_snapshot)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_snapshot-method)
         """
     async def create_subnet(
         self,
         *,
         VpcId: str,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         AvailabilityZone: str = ...,
         AvailabilityZoneId: str = ...,
         CidrBlock: str = ...,
         Ipv6CidrBlock: str = ...,
         OutpostArn: str = ...,
         DryRun: bool = ...,
         Ipv6Native: bool = ...
@@ -5144,15 +5145,15 @@
         Iops: int = ...,
         KmsKeyId: str = ...,
         OutpostArn: str = ...,
         Size: int = ...,
         SnapshotId: str = ...,
         VolumeType: VolumeTypeType = ...,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...,
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...,
         MultiAttachEnabled: bool = ...,
         Throughput: int = ...,
         ClientToken: str = ...
     ) -> _Volume:
         """
         Creates an EBS volume that can be attached to an instance in the same
         Availability Zone.
@@ -5170,15 +5171,15 @@
         Ipv4IpamPoolId: str = ...,
         Ipv4NetmaskLength: int = ...,
         Ipv6IpamPoolId: str = ...,
         Ipv6NetmaskLength: int = ...,
         DryRun: bool = ...,
         InstanceTenancy: TenancyType = ...,
         Ipv6CidrBlockNetworkBorderGroup: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> _Vpc:
         """
         Creates a VPC with the specified CIDR blocks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_vpc)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_vpc-method)
         """
@@ -5186,15 +5187,15 @@
         self,
         *,
         VpcId: str,
         DryRun: bool = ...,
         PeerOwnerId: str = ...,
         PeerVpcId: str = ...,
         PeerRegion: str = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> _VpcPeeringConnection:
         """
         Requests a VPC peering connection between two VPCs: a requester VPC that you own
         and an accepter VPC with which to create the connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.create_vpc_peering_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourcecreate_vpc_peering_connection-method)
@@ -5215,15 +5216,15 @@
         """
     async def import_key_pair(
         self,
         *,
         KeyName: str,
         PublicKeyMaterial: BlobTypeDef,
         DryRun: bool = ...,
-        TagSpecifications: Sequence[TagSpecificationUnionTypeDef] = ...
+        TagSpecifications: Sequence[TagSpecificationTypeDef] = ...
     ) -> _KeyPairInfo:
         """
         Imports the public key from an RSA or ED25519 key pair that you created with a
         third-party tool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2.ServiceResource.import_key_pair)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ec2/service_resource/#ec2serviceresourceimport_key_pair-method)
```

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/type_defs.py` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -806,15 +806,14 @@
     "HostPropertiesTypeDef",
     "IKEVersionsListValueTypeDef",
     "IKEVersionsRequestListValueTypeDef",
     "IamInstanceProfileTypeDef",
     "LaunchPermissionTypeDef",
     "UserBucketTypeDef",
     "ImageRecycleBinInfoTypeDef",
-    "StateReasonTypeDef",
     "ImportClientVpnClientCertificateRevocationListRequestRequestTypeDef",
     "ImportImageLicenseConfigurationRequestTypeDef",
     "ImportImageLicenseConfigurationResponseTypeDef",
     "UserDataTypeDef",
     "InferenceDeviceInfoTypeDef",
     "InstanceCountTypeDef",
     "InstanceCreditSpecificationRequestTypeDef",
@@ -825,26 +824,26 @@
     "InstanceMaintenanceOptionsRequestTypeDef",
     "InstanceMaintenanceOptionsTypeDef",
     "InstanceMetadataOptionsRequestTypeDef",
     "InstanceMetadataOptionsResponseTypeDef",
     "MonitoringTypeDef",
     "InstanceNetworkInterfaceAssociationTypeDef",
     "InstanceNetworkInterfaceAttachmentTypeDef",
-    "MemoryGiBPerVCpuTypeDef",
-    "MemoryMiBTypeDef",
-    "NetworkBandwidthGbpsTypeDef",
-    "NetworkInterfaceCountTypeDef",
-    "TotalLocalStorageGBTypeDef",
-    "VCpuCountRangeTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRangeRequestTypeDef",
+    "MemoryGiBPerVCpuTypeDef",
+    "MemoryMiBTypeDef",
+    "NetworkBandwidthGbpsTypeDef",
+    "NetworkInterfaceCountTypeDef",
+    "TotalLocalStorageGBTypeDef",
+    "VCpuCountRangeTypeDef",
     "InstanceStateTypeDef",
     "InstanceStatusDetailsTypeDef",
     "InstanceStatusEventTypeDef",
     "LicenseConfigurationTypeDef",
     "PrivateDnsNameOptionsResponseTypeDef",
     "MemoryInfoTypeDef",
     "PlacementGroupInfoTypeDef",
@@ -1029,15 +1028,14 @@
     "RestoreAddressToClassicRequestRequestTypeDef",
     "RestoreImageFromRecycleBinRequestRequestTypeDef",
     "RestoreManagedPrefixListVersionRequestRequestTypeDef",
     "RestoreSnapshotFromRecycleBinRequestRequestTypeDef",
     "RestoreSnapshotTierRequestRequestTypeDef",
     "RevokeClientVpnIngressRequestRequestTypeDef",
     "RouteTypeDef",
-    "S3StorageOutputTypeDef",
     "ScheduledInstanceRecurrenceTypeDef",
     "ScheduledInstancesEbsTypeDef",
     "ScheduledInstancesIamInstanceProfileTypeDef",
     "ScheduledInstancesIpv6AddressTypeDef",
     "ScheduledInstancesMonitoringTypeDef",
     "ScheduledInstancesPlacementTypeDef",
     "ScheduledInstancesPrivateIpAddressConfigTypeDef",
@@ -1223,14 +1221,15 @@
     "RestoreImageFromRecycleBinResultTypeDef",
     "RestoreSnapshotFromRecycleBinResultTypeDef",
     "RestoreSnapshotTierResultTypeDef",
     "RouteTableAssociationStateResponseTypeDef",
     "RunScheduledInstancesResultTypeDef",
     "StartVpcEndpointServicePrivateDnsVerificationResultTypeDef",
     "StateReasonResponseTypeDef",
+    "StateReasonTypeDef",
     "UnassignIpv6AddressesResultTypeDef",
     "UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef",
     "UpdateSecurityGroupRuleDescriptionsIngressResultTypeDef",
     "VolumeAttachmentResponseTypeDef",
     "VpcPeeringConnectionStateReasonResponseTypeDef",
     "AcceptReservedInstancesExchangeQuoteRequestRequestTypeDef",
     "GetReservedInstancesExchangeQuoteRequestRequestTypeDef",
@@ -1276,19 +1275,18 @@
     "NetworkInsightsAccessScopeTypeDef",
     "PlacementGroupTypeDef",
     "ReplaceRootVolumeTaskTypeDef",
     "SnapshotInfoTypeDef",
     "SnapshotResponseTypeDef",
     "SnapshotTierStatusTypeDef",
     "SnapshotTypeDef",
-    "SpotFleetTagSpecificationOutputTypeDef",
     "SpotFleetTagSpecificationTypeDef",
     "SubnetCidrReservationTypeDef",
-    "TagSpecificationOutputTypeDef",
     "TagSpecificationTypeDef",
+    "TagSpecificationVpcAddressTypeDef",
     "TrafficMirrorSessionTypeDef",
     "TrafficMirrorTargetTypeDef",
     "TransitGatewayPolicyTableTypeDef",
     "TransitGatewayRouteTableAnnouncementTypeDef",
     "TransitGatewayRouteTableTypeDef",
     "TrunkInterfaceAssociationTypeDef",
     "VerifiedAccessGroupTypeDef",
@@ -1371,15 +1369,14 @@
     "CapacityReservationSpecificationResponseResponseTypeDef",
     "CapacityReservationSpecificationResponseTypeDef",
     "LaunchTemplateCapacityReservationSpecificationResponseTypeDef",
     "CapacityReservationSpecificationTypeDef",
     "LaunchTemplateCapacityReservationSpecificationRequestTypeDef",
     "DescribeVpcClassicLinkDnsSupportResultTypeDef",
     "ClassicLinkInstanceTypeDef",
-    "ClassicLoadBalancersConfigOutputTypeDef",
     "ClassicLoadBalancersConfigTypeDef",
     "ExportClientVpnClientCertificateRevocationListResultTypeDef",
     "ClientConnectResponseOptionsTypeDef",
     "ClientVpnAuthenticationRequestTypeDef",
     "ClientVpnAuthenticationTypeDef",
     "ClientVpnConnectionTypeDef",
     "TerminateConnectionStatusTypeDef",
@@ -1402,15 +1399,16 @@
     "ModifyLocalGatewayRouteResultTypeDef",
     "SearchLocalGatewayRoutesResultTypeDef",
     "CreateNetworkAclEntryRequestNetworkAclCreateEntryTypeDef",
     "CreateNetworkAclEntryRequestRequestTypeDef",
     "NetworkAclEntryTypeDef",
     "ReplaceNetworkAclEntryRequestNetworkAclReplaceEntryTypeDef",
     "ReplaceNetworkAclEntryRequestRequestTypeDef",
-    "InstanceNetworkInterfaceSpecificationOutputTypeDef",
+    "InstanceNetworkInterfaceSpecificationServiceResourceTypeDef",
+    "InstanceNetworkInterfaceSpecificationSubnetTypeDef",
     "InstanceNetworkInterfaceSpecificationTypeDef",
     "CreateReservedInstancesListingRequestRequestTypeDef",
     "CreateStoreImageTaskRequestRequestTypeDef",
     "CreateTrafficMirrorFilterRuleRequestRequestTypeDef",
     "ModifyTrafficMirrorFilterRuleRequestRequestTypeDef",
     "CreateVolumePermissionModificationsTypeDef",
     "ModifyVpcEndpointRequestRequestTypeDef",
@@ -1805,30 +1803,28 @@
     "GetVpnTunnelReplacementStatusResultTypeDef",
     "GpuDeviceInfoTypeDef",
     "IamInstanceProfileAssociationTypeDef",
     "LaunchPermissionModificationsTypeDef",
     "ImageDiskContainerTypeDef",
     "SnapshotDiskContainerTypeDef",
     "ListImagesInRecycleBinResultTypeDef",
-    "LocalGatewayRouteTableTypeDef",
     "ImportInstanceLaunchSpecificationTypeDef",
     "InferenceAcceleratorInfoTypeDef",
     "ModifyInstanceCreditSpecificationRequestRequestTypeDef",
     "LaunchTemplateInstanceNetworkInterfaceSpecificationRequestTypeDef",
     "ModifyInstanceMetadataOptionsResultTypeDef",
     "InstanceMonitoringTypeDef",
     "InstancePrivateIpAddressTypeDef",
-    "InstanceRequirementsOutputTypeDef",
-    "InstanceRequirementsTypeDef",
     "InstanceRequirementsRequestTypeDef",
+    "InstanceRequirementsTypeDef",
     "InstanceStateChangeTypeDef",
     "InstanceStatusSummaryTypeDef",
     "ModifyInstanceEventStartTimeResultTypeDef",
-    "IpPermissionOutputTypeDef",
     "IpPermissionTypeDef",
+    "IpPermissionVpcAddressTypeDef",
     "StaleIpPermissionTypeDef",
     "ProvisionIpamPoolCidrRequestRequestTypeDef",
     "IpamDiscoveredAccountTypeDef",
     "IpamDiscoveredResourceCidrTypeDef",
     "IpamPoolTypeDef",
     "IpamResourceCidrTypeDef",
     "IpamResourceDiscoveryTypeDef",
@@ -1869,15 +1865,14 @@
     "PurchaseReservedInstancesOfferingRequestRequestTypeDef",
     "ReservedInstancesOfferingTypeDef",
     "ReservedInstancesTypeDef",
     "SecurityGroupRuleTypeDef",
     "RegisterInstanceEventNotificationAttributesRequestRequestTypeDef",
     "RegisterTransitGatewayMulticastGroupMembersResultTypeDef",
     "RegisterTransitGatewayMulticastGroupSourcesResultTypeDef",
-    "StorageOutputTypeDef",
     "ScheduledInstanceAvailabilityTypeDef",
     "ScheduledInstanceTypeDef",
     "ScheduledInstancesBlockDeviceMappingTypeDef",
     "ScheduledInstancesNetworkInterfaceTypeDef",
     "SearchTransitGatewayMulticastGroupsResultTypeDef",
     "VpcEndpointTypeDef",
     "SecurityGroupRuleUpdateTypeDef",
@@ -1887,15 +1882,14 @@
     "SnapshotTaskDetailTypeDef",
     "SpotMaintenanceStrategiesTypeDef",
     "SpotDatafeedSubscriptionTypeDef",
     "TransitGatewayMulticastDomainAssociationTypeDef",
     "TransitGatewayMulticastDomainAssociationsTypeDef",
     "SubnetIpv6CidrBlockAssociationTypeDef",
     "TargetReservationValueTypeDef",
-    "TargetGroupsConfigOutputTypeDef",
     "TargetGroupsConfigTypeDef",
     "TrafficMirrorFilterRuleTypeDef",
     "TransitGatewayAttachmentTypeDef",
     "TransitGatewayConnectPeerConfigurationTypeDef",
     "TransitGatewayConnectTypeDef",
     "TransitGatewayMulticastDomainTypeDef",
     "TransitGatewayTypeDef",
@@ -1916,14 +1910,15 @@
     "VolumeResponseTypeDef",
     "VolumeTypeDef",
     "VolumeStatusInfoTypeDef",
     "VpcCidrBlockAssociationTypeDef",
     "VpcIpv6CidrBlockAssociationTypeDef",
     "VpcPeeringConnectionVpcInfoResponseTypeDef",
     "VpcPeeringConnectionVpcInfoTypeDef",
+    "LocalGatewayRouteTableTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "AdditionalDetailTypeDef",
     "DescribeAddressesAttributeResultTypeDef",
     "ModifyAddressAttributeResultTypeDef",
     "ResetAddressAttributeResultTypeDef",
     "DescribeAddressesResultTypeDef",
     "DescribeVpcEndpointServicePermissionsResultTypeDef",
@@ -1976,23 +1971,104 @@
     "DescribeReplaceRootVolumeTasksResultTypeDef",
     "CreateSnapshotsResultTypeDef",
     "DescribeSnapshotTierStatusResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "CreateSubnetCidrReservationResultTypeDef",
     "DeleteSubnetCidrReservationResultTypeDef",
     "GetSubnetCidrReservationsResultTypeDef",
+    "AcceptAddressTransferRequestRequestTypeDef",
+    "AllocateAddressRequestRequestTypeDef",
+    "AllocateHostsRequestRequestTypeDef",
+    "AssociateIpamResourceDiscoveryRequestRequestTypeDef",
+    "CopySnapshotRequestRequestTypeDef",
     "CopySnapshotRequestSnapshotCopyTypeDef",
+    "CreateCapacityReservationFleetRequestRequestTypeDef",
+    "CreateCapacityReservationRequestRequestTypeDef",
+    "CreateCarrierGatewayRequestRequestTypeDef",
+    "CreateCoipPoolRequestRequestTypeDef",
+    "CreateCustomerGatewayRequestRequestTypeDef",
+    "CreateDhcpOptionsRequestRequestTypeDef",
+    "CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
+    "CreateEgressOnlyInternetGatewayRequestRequestTypeDef",
+    "CreateFlowLogsRequestRequestTypeDef",
+    "CreateFpgaImageRequestRequestTypeDef",
+    "CreateInstanceConnectEndpointRequestRequestTypeDef",
+    "CreateInstanceEventWindowRequestRequestTypeDef",
+    "CreateInstanceExportTaskRequestRequestTypeDef",
+    "CreateInternetGatewayRequestRequestTypeDef",
+    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
+    "CreateIpamPoolRequestRequestTypeDef",
+    "CreateIpamRequestRequestTypeDef",
+    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
+    "CreateIpamScopeRequestRequestTypeDef",
+    "CreateKeyPairRequestRequestTypeDef",
+    "CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
+    "CreateLocalGatewayRouteTableRequestRequestTypeDef",
+    "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
+    "CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
+    "CreateManagedPrefixListRequestRequestTypeDef",
+    "CreateNatGatewayRequestRequestTypeDef",
+    "CreateNetworkAclRequestRequestTypeDef",
+    "CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
     "CreateNetworkAclRequestVpcCreateNetworkAclTypeDef",
+    "CreateNetworkInterfaceRequestRequestTypeDef",
+    "CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
     "CreateNetworkInterfaceRequestSubnetCreateNetworkInterfaceTypeDef",
+    "CreatePlacementGroupRequestRequestTypeDef",
+    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
+    "CreatePublicIpv4PoolRequestRequestTypeDef",
+    "CreateReplaceRootVolumeTaskRequestRequestTypeDef",
+    "CreateRestoreImageTaskRequestRequestTypeDef",
+    "CreateRouteTableRequestRequestTypeDef",
+    "CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
     "CreateRouteTableRequestVpcCreateRouteTableTypeDef",
+    "CreateSecurityGroupRequestRequestTypeDef",
+    "CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
     "CreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef",
+    "CreateSnapshotRequestRequestTypeDef",
+    "CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
     "CreateSnapshotRequestVolumeCreateSnapshotTypeDef",
+    "CreateSnapshotsRequestRequestTypeDef",
+    "CreateSubnetCidrReservationRequestRequestTypeDef",
+    "CreateSubnetRequestRequestTypeDef",
+    "CreateSubnetRequestServiceResourceCreateSubnetTypeDef",
     "CreateSubnetRequestVpcCreateSubnetTypeDef",
+    "CreateTrafficMirrorFilterRequestRequestTypeDef",
+    "CreateTrafficMirrorSessionRequestRequestTypeDef",
+    "CreateTrafficMirrorTargetRequestRequestTypeDef",
+    "CreateTransitGatewayConnectPeerRequestRequestTypeDef",
+    "CreateTransitGatewayConnectRequestRequestTypeDef",
+    "CreateTransitGatewayMulticastDomainRequestRequestTypeDef",
+    "CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
+    "CreateTransitGatewayPolicyTableRequestRequestTypeDef",
+    "CreateTransitGatewayRequestRequestTypeDef",
+    "CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
+    "CreateTransitGatewayRouteTableRequestRequestTypeDef",
+    "CreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
+    "CreateVerifiedAccessEndpointRequestRequestTypeDef",
+    "CreateVerifiedAccessGroupRequestRequestTypeDef",
+    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
+    "CreateVerifiedAccessTrustProviderRequestRequestTypeDef",
+    "CreateVolumeRequestRequestTypeDef",
+    "CreateVolumeRequestServiceResourceCreateVolumeTypeDef",
+    "CreateVpcEndpointRequestRequestTypeDef",
+    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
+    "CreateVpcPeeringConnectionRequestRequestTypeDef",
+    "CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
     "CreateVpcPeeringConnectionRequestVpcRequestVpcPeeringConnectionTypeDef",
-    "TagSpecificationUnionTypeDef",
+    "CreateVpcRequestRequestTypeDef",
+    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
+    "CreateVpnGatewayRequestRequestTypeDef",
+    "ExportImageRequestRequestTypeDef",
+    "ImportKeyPairRequestRequestTypeDef",
+    "ImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
+    "ProvisionByoipCidrRequestRequestTypeDef",
+    "PurchaseHostReservationRequestRequestTypeDef",
+    "StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
+    "StartNetworkInsightsAnalysisRequestRequestTypeDef",
     "CreateTrafficMirrorSessionResultTypeDef",
     "DescribeTrafficMirrorSessionsResultTypeDef",
     "ModifyTrafficMirrorSessionResultTypeDef",
     "CreateTrafficMirrorTargetResultTypeDef",
     "DescribeTrafficMirrorTargetsResultTypeDef",
     "CreateTransitGatewayPolicyTableResultTypeDef",
     "DeleteTransitGatewayPolicyTableResultTypeDef",
@@ -2026,35 +2102,36 @@
     "NetworkInterfaceAttachmentTypeDef",
     "DhcpOptionsTypeDef",
     "DescribeClientVpnAuthorizationRulesResultTypeDef",
     "DescribeAvailabilityZonesResultTypeDef",
     "HostTypeDef",
     "StorageTypeDef",
     "CreateImageRequestInstanceCreateImageTypeDef",
+    "CreateImageRequestRequestTypeDef",
     "ImageAttributeTypeDef",
     "ImageTypeDef",
     "RegisterImageRequestRequestTypeDef",
     "RegisterImageRequestServiceResourceRegisterImageTypeDef",
     "CancelCapacityReservationFleetsResultTypeDef",
     "CancelSpotFleetRequestsResponseTypeDef",
     "CreateCapacityReservationResultTypeDef",
     "DescribeCapacityReservationsResultTypeDef",
     "DescribeCapacityReservationFleetsResultTypeDef",
     "ModifyInstanceCapacityReservationAttributesRequestRequestTypeDef",
     "DescribeClassicLinkInstancesResultTypeDef",
+    "CreateClientVpnEndpointRequestRequestTypeDef",
     "ClientVpnEndpointTypeDef",
     "DescribeClientVpnConnectionsResultTypeDef",
     "TerminateClientVpnConnectionsResultTypeDef",
     "DescribeClientVpnRoutesResultTypeDef",
     "ModifyVpnTunnelOptionsSpecificationTypeDef",
     "VpnTunnelOptionsSpecificationTypeDef",
     "TunnelOptionTypeDef",
     "NetworkAclTypeDef",
     "LaunchSpecificationTypeDef",
-    "InstanceNetworkInterfaceSpecificationUnionTypeDef",
     "RequestSpotLaunchSpecificationTypeDef",
     "ModifySnapshotAttributeRequestRequestTypeDef",
     "ModifySnapshotAttributeRequestSnapshotModifyAttributeTypeDef",
     "GetAwsNetworkPerformanceDataResultTypeDef",
     "DeleteFleetsResultTypeDef",
     "DeleteLaunchTemplateVersionsResultTypeDef",
     "DeleteQueuedReservedInstancesResultTypeDef",
@@ -2092,42 +2169,45 @@
     "GpuInfoTypeDef",
     "AssociateIamInstanceProfileResultTypeDef",
     "DescribeIamInstanceProfileAssociationsResultTypeDef",
     "DisassociateIamInstanceProfileResultTypeDef",
     "ReplaceIamInstanceProfileAssociationResultTypeDef",
     "ModifyImageAttributeRequestImageModifyAttributeTypeDef",
     "ModifyImageAttributeRequestRequestTypeDef",
-    "CreateLocalGatewayRouteTableResultTypeDef",
-    "DeleteLocalGatewayRouteTableResultTypeDef",
-    "DescribeLocalGatewayRouteTablesResultTypeDef",
+    "ImportImageRequestRequestTypeDef",
+    "ImportSnapshotRequestRequestTypeDef",
     "ImportInstanceRequestRequestTypeDef",
     "MonitorInstancesResultTypeDef",
     "UnmonitorInstancesResultTypeDef",
     "InstanceNetworkInterfaceTypeDef",
-    "FleetLaunchTemplateOverridesTypeDef",
-    "LaunchTemplateOverridesOutputTypeDef",
-    "SpotFleetLaunchSpecificationOutputTypeDef",
-    "LaunchTemplateOverridesTypeDef",
-    "SpotFleetLaunchSpecificationTypeDef",
     "FleetLaunchTemplateOverridesRequestTypeDef",
     "GetInstanceTypesFromInstanceRequirementsRequestGetInstanceTypesFromInstanceRequirementsPaginateTypeDef",
     "GetInstanceTypesFromInstanceRequirementsRequestRequestTypeDef",
     "InstanceRequirementsWithMetadataRequestTypeDef",
+    "FleetLaunchTemplateOverridesTypeDef",
+    "LaunchTemplateOverridesTypeDef",
+    "SpotFleetLaunchSpecificationTypeDef",
     "StartInstancesResultTypeDef",
     "StopInstancesResultTypeDef",
     "TerminateInstancesResultTypeDef",
     "InstanceStatusTypeDef",
-    "RevokeSecurityGroupEgressResultTypeDef",
-    "RevokeSecurityGroupIngressResultTypeDef",
-    "SecurityGroupTypeDef",
+    "AuthorizeSecurityGroupEgressRequestRequestTypeDef",
     "AuthorizeSecurityGroupEgressRequestSecurityGroupAuthorizeEgressTypeDef",
+    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
     "AuthorizeSecurityGroupIngressRequestSecurityGroupAuthorizeIngressTypeDef",
-    "IpPermissionUnionTypeDef",
+    "RevokeSecurityGroupEgressRequestRequestTypeDef",
     "RevokeSecurityGroupEgressRequestSecurityGroupRevokeEgressTypeDef",
+    "RevokeSecurityGroupEgressResultTypeDef",
+    "RevokeSecurityGroupIngressRequestRequestTypeDef",
     "RevokeSecurityGroupIngressRequestSecurityGroupRevokeIngressTypeDef",
+    "RevokeSecurityGroupIngressResultTypeDef",
+    "SecurityGroupTypeDef",
+    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
+    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
+    "SecurityGroupVpcAddressTypeDef",
     "StaleSecurityGroupTypeDef",
     "GetIpamDiscoveredAccountsResultTypeDef",
     "GetIpamDiscoveredResourceCidrsResultTypeDef",
     "CreateIpamPoolResultTypeDef",
     "DeleteIpamPoolResultTypeDef",
     "DescribeIpamPoolsResultTypeDef",
     "ModifyIpamPoolResultTypeDef",
@@ -2152,26 +2232,26 @@
     "DescribeNatGatewaysResultTypeDef",
     "CreateNetworkInterfacePermissionResultTypeDef",
     "DescribeNetworkInterfacePermissionsResultTypeDef",
     "CreateVerifiedAccessTrustProviderResultTypeDef",
     "DeleteVerifiedAccessTrustProviderResultTypeDef",
     "DescribeVerifiedAccessTrustProvidersResultTypeDef",
     "ModifyVerifiedAccessTrustProviderResultTypeDef",
+    "CreateNetworkInsightsPathRequestRequestTypeDef",
     "AccessScopePathRequestTypeDef",
     "AccessScopePathTypeDef",
     "CancelReservedInstancesListingResultTypeDef",
     "CreateReservedInstancesListingResultTypeDef",
     "DescribeReservedInstancesListingsResultTypeDef",
     "DescribePublicIpv4PoolsResultTypeDef",
     "DescribeReservedInstancesOfferingsResultTypeDef",
     "DescribeReservedInstancesResultTypeDef",
     "AuthorizeSecurityGroupEgressResultTypeDef",
     "AuthorizeSecurityGroupIngressResultTypeDef",
     "DescribeSecurityGroupRulesResultTypeDef",
-    "BundleTaskTypeDef",
     "DescribeScheduledInstanceAvailabilityResultTypeDef",
     "DescribeScheduledInstancesResultTypeDef",
     "PurchaseScheduledInstancesResultTypeDef",
     "ScheduledInstancesLaunchSpecificationTypeDef",
     "CreateVpcEndpointResultTypeDef",
     "DescribeVpcEndpointsResultTypeDef",
     "ModifySecurityGroupRulesRequestRequestTypeDef",
@@ -2189,15 +2269,14 @@
     "AssociateTransitGatewayMulticastDomainResultTypeDef",
     "DisassociateTransitGatewayMulticastDomainResultTypeDef",
     "RejectTransitGatewayMulticastDomainAssociationsResultTypeDef",
     "AssociateSubnetCidrBlockResultTypeDef",
     "DisassociateSubnetCidrBlockResultTypeDef",
     "SubnetTypeDef",
     "GetReservedInstancesExchangeQuoteResultTypeDef",
-    "LoadBalancersConfigOutputTypeDef",
     "LoadBalancersConfigTypeDef",
     "CreateTrafficMirrorFilterRuleResultTypeDef",
     "ModifyTrafficMirrorFilterRuleResultTypeDef",
     "TrafficMirrorFilterTypeDef",
     "DescribeTransitGatewayAttachmentsResultTypeDef",
     "TransitGatewayConnectPeerTypeDef",
     "CreateTransitGatewayConnectResultTypeDef",
@@ -2255,161 +2334,68 @@
     "ModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef",
     "DescribeVolumesResultTypeDef",
     "VolumeStatusItemTypeDef",
     "AssociateVpcCidrBlockResultTypeDef",
     "DisassociateVpcCidrBlockResultTypeDef",
     "VpcTypeDef",
     "VpcPeeringConnectionTypeDef",
+    "CreateLocalGatewayRouteTableResultTypeDef",
+    "DeleteLocalGatewayRouteTableResultTypeDef",
+    "DescribeLocalGatewayRouteTablesResultTypeDef",
     "AssociateInstanceEventWindowResultTypeDef",
     "CreateInstanceEventWindowResultTypeDef",
     "DescribeInstanceEventWindowsResultTypeDef",
     "DisassociateInstanceEventWindowResultTypeDef",
     "ModifyInstanceEventWindowResultTypeDef",
-    "AcceptAddressTransferRequestRequestTypeDef",
-    "AllocateAddressRequestRequestTypeDef",
-    "AllocateHostsRequestRequestTypeDef",
-    "AssociateIpamResourceDiscoveryRequestRequestTypeDef",
-    "CopySnapshotRequestRequestTypeDef",
-    "CreateCapacityReservationFleetRequestRequestTypeDef",
-    "CreateCapacityReservationRequestRequestTypeDef",
-    "CreateCarrierGatewayRequestRequestTypeDef",
-    "CreateClientVpnEndpointRequestRequestTypeDef",
-    "CreateCoipPoolRequestRequestTypeDef",
-    "CreateCustomerGatewayRequestRequestTypeDef",
-    "CreateDhcpOptionsRequestRequestTypeDef",
-    "CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
-    "CreateEgressOnlyInternetGatewayRequestRequestTypeDef",
-    "CreateFlowLogsRequestRequestTypeDef",
-    "CreateFpgaImageRequestRequestTypeDef",
-    "CreateImageRequestRequestTypeDef",
-    "CreateInstanceConnectEndpointRequestRequestTypeDef",
-    "CreateInstanceEventWindowRequestRequestTypeDef",
-    "CreateInstanceExportTaskRequestRequestTypeDef",
-    "CreateInternetGatewayRequestRequestTypeDef",
-    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
-    "CreateIpamPoolRequestRequestTypeDef",
-    "CreateIpamRequestRequestTypeDef",
-    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
-    "CreateIpamScopeRequestRequestTypeDef",
-    "CreateKeyPairRequestRequestTypeDef",
-    "CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
-    "CreateLocalGatewayRouteTableRequestRequestTypeDef",
-    "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
-    "CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
-    "CreateManagedPrefixListRequestRequestTypeDef",
-    "CreateNatGatewayRequestRequestTypeDef",
-    "CreateNetworkAclRequestRequestTypeDef",
-    "CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
-    "CreateNetworkInsightsPathRequestRequestTypeDef",
-    "CreateNetworkInterfaceRequestRequestTypeDef",
-    "CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
-    "CreatePlacementGroupRequestRequestTypeDef",
-    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
-    "CreatePublicIpv4PoolRequestRequestTypeDef",
-    "CreateReplaceRootVolumeTaskRequestRequestTypeDef",
-    "CreateRestoreImageTaskRequestRequestTypeDef",
-    "CreateRouteTableRequestRequestTypeDef",
-    "CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
-    "CreateSecurityGroupRequestRequestTypeDef",
-    "CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
-    "CreateSnapshotRequestRequestTypeDef",
-    "CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
-    "CreateSnapshotsRequestRequestTypeDef",
-    "CreateSubnetCidrReservationRequestRequestTypeDef",
-    "CreateSubnetRequestRequestTypeDef",
-    "CreateSubnetRequestServiceResourceCreateSubnetTypeDef",
-    "CreateTrafficMirrorFilterRequestRequestTypeDef",
-    "CreateTrafficMirrorSessionRequestRequestTypeDef",
-    "CreateTrafficMirrorTargetRequestRequestTypeDef",
-    "CreateTransitGatewayConnectPeerRequestRequestTypeDef",
-    "CreateTransitGatewayConnectRequestRequestTypeDef",
-    "CreateTransitGatewayMulticastDomainRequestRequestTypeDef",
-    "CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
-    "CreateTransitGatewayPolicyTableRequestRequestTypeDef",
-    "CreateTransitGatewayRequestRequestTypeDef",
-    "CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
-    "CreateTransitGatewayRouteTableRequestRequestTypeDef",
-    "CreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
-    "CreateVerifiedAccessEndpointRequestRequestTypeDef",
-    "CreateVerifiedAccessGroupRequestRequestTypeDef",
-    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
-    "CreateVerifiedAccessTrustProviderRequestRequestTypeDef",
-    "CreateVolumeRequestRequestTypeDef",
-    "CreateVolumeRequestServiceResourceCreateVolumeTypeDef",
-    "CreateVpcEndpointRequestRequestTypeDef",
-    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
-    "CreateVpcPeeringConnectionRequestRequestTypeDef",
-    "CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
-    "CreateVpcRequestRequestTypeDef",
-    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
-    "CreateVpnGatewayRequestRequestTypeDef",
-    "ExportImageRequestRequestTypeDef",
-    "ImportImageRequestRequestTypeDef",
-    "ImportKeyPairRequestRequestTypeDef",
-    "ImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
-    "ImportSnapshotRequestRequestTypeDef",
-    "ProvisionByoipCidrRequestRequestTypeDef",
-    "PurchaseHostReservationRequestRequestTypeDef",
-    "StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
-    "StartNetworkInsightsAnalysisRequestRequestTypeDef",
     "PathComponentTypeDef",
     "CreateRouteTableResultTypeDef",
     "DescribeRouteTablesResultTypeDef",
     "GetFlowLogsIntegrationTemplateRequestRequestTypeDef",
     "RequestLaunchTemplateDataTypeDef",
+    "RunInstancesRequestRequestTypeDef",
+    "RunInstancesRequestServiceResourceCreateInstancesTypeDef",
     "RunInstancesRequestSubnetCreateInstancesTypeDef",
     "DescribeNetworkInterfaceAttributeResultTypeDef",
     "NetworkInterfaceTypeDef",
     "CreateDhcpOptionsResultTypeDef",
     "DescribeDhcpOptionsResultTypeDef",
     "DescribeHostsResultTypeDef",
     "BundleInstanceRequestRequestTypeDef",
-    "StorageUnionTypeDef",
+    "BundleTaskTypeDef",
     "DescribeImagesResultTypeDef",
     "DescribeClientVpnEndpointsResultTypeDef",
     "ModifyVpnTunnelOptionsRequestRequestTypeDef",
     "VpnConnectionOptionsSpecificationTypeDef",
     "VpnConnectionOptionsTypeDef",
     "CreateNetworkAclResultTypeDef",
     "DescribeNetworkAclsResultTypeDef",
     "SpotInstanceRequestTypeDef",
-    "RunInstancesRequestRequestTypeDef",
-    "RunInstancesRequestServiceResourceCreateInstancesTypeDef",
     "RequestSpotInstancesRequestRequestTypeDef",
     "DisableFastSnapshotRestoresResultTypeDef",
     "ConversionTaskTypeDef",
     "EnableFastSnapshotRestoresResultTypeDef",
     "CreateNetworkInsightsPathResultTypeDef",
     "DescribeNetworkInsightsPathsResultTypeDef",
     "InstanceTypeInfoTypeDef",
     "InstanceTypeDef",
-    "FleetLaunchTemplateConfigTypeDef",
-    "LaunchTemplateAndOverridesResponseTypeDef",
-    "LaunchTemplateConfigOutputTypeDef",
-    "LaunchTemplateConfigTypeDef",
     "FleetLaunchTemplateConfigRequestTypeDef",
     "GetSpotPlacementScoresRequestGetSpotPlacementScoresPaginateTypeDef",
     "GetSpotPlacementScoresRequestRequestTypeDef",
+    "FleetLaunchTemplateConfigTypeDef",
+    "LaunchTemplateAndOverridesResponseTypeDef",
+    "LaunchTemplateConfigTypeDef",
     "DescribeInstanceStatusResultTypeDef",
     "DescribeSecurityGroupsResultTypeDef",
-    "AuthorizeSecurityGroupEgressRequestRequestTypeDef",
-    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
-    "RevokeSecurityGroupEgressRequestRequestTypeDef",
-    "RevokeSecurityGroupIngressRequestRequestTypeDef",
-    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
-    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
+    "DescribeSecurityGroupsResultVpcAddressTypeDef",
     "DescribeStaleSecurityGroupsResultTypeDef",
     "GetLaunchTemplateDataResultTypeDef",
     "LaunchTemplateVersionTypeDef",
     "DescribeReservedInstancesModificationsResultTypeDef",
     "CreateNetworkInsightsAccessScopeRequestRequestTypeDef",
     "NetworkInsightsAccessScopeContentTypeDef",
-    "BundleInstanceResultTypeDef",
-    "CancelBundleTaskResultTypeDef",
-    "DescribeBundleTasksResultTypeDef",
     "RunScheduledInstancesRequestRequestTypeDef",
     "DescribeImportImageTasksResultTypeDef",
     "DescribeImportSnapshotTasksResultTypeDef",
     "CreateDefaultSubnetResultTypeDef",
     "CreateSubnetResultTypeDef",
     "DescribeSubnetsResultTypeDef",
     "CreateTrafficMirrorFilterResultTypeDef",
@@ -2429,33 +2415,36 @@
     "DescribeVpcPeeringConnectionsResultTypeDef",
     "AccessScopeAnalysisFindingTypeDef",
     "NetworkInsightsAnalysisTypeDef",
     "CreateLaunchTemplateRequestRequestTypeDef",
     "CreateLaunchTemplateVersionRequestRequestTypeDef",
     "CreateNetworkInterfaceResultTypeDef",
     "DescribeNetworkInterfacesResultTypeDef",
+    "BundleInstanceResultTypeDef",
+    "CancelBundleTaskResultTypeDef",
+    "DescribeBundleTasksResultTypeDef",
     "CreateVpnConnectionRequestRequestTypeDef",
     "VpnConnectionTypeDef",
     "DescribeSpotInstanceRequestsResultTypeDef",
     "RequestSpotInstancesResultTypeDef",
     "DescribeConversionTasksResultTypeDef",
     "ImportInstanceResultTypeDef",
     "ImportVolumeResultTypeDef",
     "DescribeInstanceTypesResultTypeDef",
     "ReservationResponseTypeDef",
     "ReservationTypeDef",
+    "CreateFleetRequestRequestTypeDef",
+    "ModifyFleetRequestRequestTypeDef",
     "CreateFleetErrorTypeDef",
     "CreateFleetInstanceTypeDef",
     "DescribeFleetErrorTypeDef",
     "DescribeFleetsInstancesTypeDef",
-    "SpotFleetRequestConfigDataOutputTypeDef",
-    "LaunchTemplateConfigUnionTypeDef",
+    "ModifySpotFleetRequestRequestRequestTypeDef",
     "SpotFleetRequestConfigDataTypeDef",
-    "CreateFleetRequestRequestTypeDef",
-    "ModifyFleetRequestRequestTypeDef",
+    "SpotFleetRequestConfigDataVpcAddressTypeDef",
     "CreateLaunchTemplateVersionResultTypeDef",
     "DescribeLaunchTemplateVersionsResultTypeDef",
     "CreateNetworkInsightsAccessScopeResultTypeDef",
     "GetNetworkInsightsAccessScopeContentResultTypeDef",
     "DescribeVerifiedAccessInstanceLoggingConfigurationsResultTypeDef",
     "ModifyVerifiedAccessInstanceLoggingConfigurationResultTypeDef",
     "GetNetworkInsightsAccessScopeAnalysisFindingsResultTypeDef",
@@ -2466,20 +2455,20 @@
     "ModifyVpnConnectionOptionsResultTypeDef",
     "ModifyVpnConnectionResultTypeDef",
     "ModifyVpnTunnelCertificateResultTypeDef",
     "ModifyVpnTunnelOptionsResultTypeDef",
     "DescribeInstancesResultTypeDef",
     "CreateFleetResultTypeDef",
     "FleetDataTypeDef",
-    "SpotFleetRequestConfigTypeDef",
-    "ModifySpotFleetRequestRequestRequestTypeDef",
     "RequestSpotFleetRequestRequestTypeDef",
-    "SpotFleetRequestConfigDataUnionTypeDef",
+    "SpotFleetRequestConfigTypeDef",
+    "SpotFleetRequestConfigVpcAddressTypeDef",
     "DescribeFleetsResultTypeDef",
     "DescribeSpotFleetRequestsResponseTypeDef",
+    "DescribeSpotFleetRequestsResponseVpcAddressTypeDef",
 )
 
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
     {
         "Min": int,
         "Max": int,
@@ -10102,23 +10091,14 @@
         "Description": str,
         "RecycleBinEnterTime": datetime,
         "RecycleBinExitTime": datetime,
     },
     total=False,
 )
 
-StateReasonTypeDef = TypedDict(
-    "StateReasonTypeDef",
-    {
-        "Code": str,
-        "Message": str,
-    },
-    total=False,
-)
-
 _RequiredImportClientVpnClientCertificateRevocationListRequestRequestTypeDef = TypedDict(
     "_RequiredImportClientVpnClientCertificateRevocationListRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
         "CertificateRevocationList": str,
     },
 )
@@ -10308,144 +10288,144 @@
         "DeviceIndex": int,
         "Status": AttachmentStatusType,
         "NetworkCardIndex": int,
     },
     total=False,
 )
 
-MemoryGiBPerVCpuTypeDef = TypedDict(
-    "MemoryGiBPerVCpuTypeDef",
+MemoryGiBPerVCpuRequestTypeDef = TypedDict(
+    "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-MemoryMiBTypeDef = TypedDict(
-    "MemoryMiBTypeDef",
+_RequiredMemoryMiBRequestTypeDef = TypedDict(
+    "_RequiredMemoryMiBRequestTypeDef",
     {
         "Min": int,
+    },
+)
+_OptionalMemoryMiBRequestTypeDef = TypedDict(
+    "_OptionalMemoryMiBRequestTypeDef",
+    {
         "Max": int,
     },
     total=False,
 )
 
-NetworkBandwidthGbpsTypeDef = TypedDict(
-    "NetworkBandwidthGbpsTypeDef",
+
+class MemoryMiBRequestTypeDef(_RequiredMemoryMiBRequestTypeDef, _OptionalMemoryMiBRequestTypeDef):
+    pass
+
+
+NetworkBandwidthGbpsRequestTypeDef = TypedDict(
+    "NetworkBandwidthGbpsRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-NetworkInterfaceCountTypeDef = TypedDict(
-    "NetworkInterfaceCountTypeDef",
+NetworkInterfaceCountRequestTypeDef = TypedDict(
+    "NetworkInterfaceCountRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
 )
 
-TotalLocalStorageGBTypeDef = TypedDict(
-    "TotalLocalStorageGBTypeDef",
+TotalLocalStorageGBRequestTypeDef = TypedDict(
+    "TotalLocalStorageGBRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-VCpuCountRangeTypeDef = TypedDict(
-    "VCpuCountRangeTypeDef",
+_RequiredVCpuCountRangeRequestTypeDef = TypedDict(
+    "_RequiredVCpuCountRangeRequestTypeDef",
     {
         "Min": int,
+    },
+)
+_OptionalVCpuCountRangeRequestTypeDef = TypedDict(
+    "_OptionalVCpuCountRangeRequestTypeDef",
+    {
         "Max": int,
     },
     total=False,
 )
 
-MemoryGiBPerVCpuRequestTypeDef = TypedDict(
-    "MemoryGiBPerVCpuRequestTypeDef",
+
+class VCpuCountRangeRequestTypeDef(
+    _RequiredVCpuCountRangeRequestTypeDef, _OptionalVCpuCountRangeRequestTypeDef
+):
+    pass
+
+
+MemoryGiBPerVCpuTypeDef = TypedDict(
+    "MemoryGiBPerVCpuTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-_RequiredMemoryMiBRequestTypeDef = TypedDict(
-    "_RequiredMemoryMiBRequestTypeDef",
+MemoryMiBTypeDef = TypedDict(
+    "MemoryMiBTypeDef",
     {
         "Min": int,
-    },
-)
-_OptionalMemoryMiBRequestTypeDef = TypedDict(
-    "_OptionalMemoryMiBRequestTypeDef",
-    {
         "Max": int,
     },
     total=False,
 )
 
-
-class MemoryMiBRequestTypeDef(_RequiredMemoryMiBRequestTypeDef, _OptionalMemoryMiBRequestTypeDef):
-    pass
-
-
-NetworkBandwidthGbpsRequestTypeDef = TypedDict(
-    "NetworkBandwidthGbpsRequestTypeDef",
+NetworkBandwidthGbpsTypeDef = TypedDict(
+    "NetworkBandwidthGbpsTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-NetworkInterfaceCountRequestTypeDef = TypedDict(
-    "NetworkInterfaceCountRequestTypeDef",
+NetworkInterfaceCountTypeDef = TypedDict(
+    "NetworkInterfaceCountTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
 )
 
-TotalLocalStorageGBRequestTypeDef = TypedDict(
-    "TotalLocalStorageGBRequestTypeDef",
+TotalLocalStorageGBTypeDef = TypedDict(
+    "TotalLocalStorageGBTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-_RequiredVCpuCountRangeRequestTypeDef = TypedDict(
-    "_RequiredVCpuCountRangeRequestTypeDef",
+VCpuCountRangeTypeDef = TypedDict(
+    "VCpuCountRangeTypeDef",
     {
         "Min": int,
-    },
-)
-_OptionalVCpuCountRangeRequestTypeDef = TypedDict(
-    "_OptionalVCpuCountRangeRequestTypeDef",
-    {
         "Max": int,
     },
     total=False,
 )
 
-
-class VCpuCountRangeRequestTypeDef(
-    _RequiredVCpuCountRangeRequestTypeDef, _OptionalVCpuCountRangeRequestTypeDef
-):
-    pass
-
-
 InstanceStateTypeDef = TypedDict(
     "InstanceStateTypeDef",
     {
         "Code": int,
         "Name": InstanceStateNameType,
     },
     total=False,
@@ -13231,26 +13211,14 @@
         "State": RouteStateType,
         "VpcPeeringConnectionId": str,
         "CoreNetworkArn": str,
     },
     total=False,
 )
 
-S3StorageOutputTypeDef = TypedDict(
-    "S3StorageOutputTypeDef",
-    {
-        "AWSAccessKeyId": str,
-        "Bucket": str,
-        "Prefix": str,
-        "UploadPolicy": bytes,
-        "UploadPolicySignature": str,
-    },
-    total=False,
-)
-
 ScheduledInstanceRecurrenceTypeDef = TypedDict(
     "ScheduledInstanceRecurrenceTypeDef",
     {
         "Frequency": str,
         "Interval": int,
         "OccurrenceDaySet": List[int],
         "OccurrenceRelativeToEnd": bool,
@@ -15171,14 +15139,23 @@
     {
         "Code": str,
         "Message": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StateReasonTypeDef = TypedDict(
+    "StateReasonTypeDef",
+    {
+        "Code": str,
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UnassignIpv6AddressesResultTypeDef = TypedDict(
     "UnassignIpv6AddressesResultTypeDef",
     {
         "NetworkInterfaceId": str,
         "UnassignedIpv6Addresses": List[str],
         "UnassignedIpv6Prefixes": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -15932,28 +15909,19 @@
         "Tags": List[TagTypeDef],
         "StorageTier": StorageTierType,
         "RestoreExpiryTime": datetime,
     },
     total=False,
 )
 
-SpotFleetTagSpecificationOutputTypeDef = TypedDict(
-    "SpotFleetTagSpecificationOutputTypeDef",
-    {
-        "ResourceType": ResourceTypeType,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 SpotFleetTagSpecificationTypeDef = TypedDict(
     "SpotFleetTagSpecificationTypeDef",
     {
         "ResourceType": ResourceTypeType,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 SubnetCidrReservationTypeDef = TypedDict(
     "SubnetCidrReservationTypeDef",
     {
@@ -15964,28 +15932,28 @@
         "OwnerId": str,
         "Description": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-TagSpecificationOutputTypeDef = TypedDict(
-    "TagSpecificationOutputTypeDef",
+TagSpecificationTypeDef = TypedDict(
+    "TagSpecificationTypeDef",
     {
         "ResourceType": ResourceTypeType,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-TagSpecificationTypeDef = TypedDict(
-    "TagSpecificationTypeDef",
+TagSpecificationVpcAddressTypeDef = TypedDict(
+    "TagSpecificationVpcAddressTypeDef",
     {
         "ResourceType": ResourceTypeType,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 TrafficMirrorSessionTypeDef = TypedDict(
     "TrafficMirrorSessionTypeDef",
     {
@@ -17161,26 +17129,18 @@
         "InstanceId": str,
         "Tags": List[TagTypeDef],
         "VpcId": str,
     },
     total=False,
 )
 
-ClassicLoadBalancersConfigOutputTypeDef = TypedDict(
-    "ClassicLoadBalancersConfigOutputTypeDef",
-    {
-        "ClassicLoadBalancers": List[ClassicLoadBalancerTypeDef],
-    },
-    total=False,
-)
-
 ClassicLoadBalancersConfigTypeDef = TypedDict(
     "ClassicLoadBalancersConfigTypeDef",
     {
-        "ClassicLoadBalancers": Sequence[ClassicLoadBalancerTypeDef],
+        "ClassicLoadBalancers": List[ClassicLoadBalancerTypeDef],
     },
     total=False,
 )
 
 ExportClientVpnClientCertificateRevocationListResultTypeDef = TypedDict(
     "ExportClientVpnClientCertificateRevocationListResultTypeDef",
     {
@@ -17577,42 +17537,42 @@
 class ReplaceNetworkAclEntryRequestRequestTypeDef(
     _RequiredReplaceNetworkAclEntryRequestRequestTypeDef,
     _OptionalReplaceNetworkAclEntryRequestRequestTypeDef,
 ):
     pass
 
 
-InstanceNetworkInterfaceSpecificationOutputTypeDef = TypedDict(
-    "InstanceNetworkInterfaceSpecificationOutputTypeDef",
+InstanceNetworkInterfaceSpecificationServiceResourceTypeDef = TypedDict(
+    "InstanceNetworkInterfaceSpecificationServiceResourceTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "DeleteOnTermination": bool,
         "Description": str,
         "DeviceIndex": int,
-        "Groups": List[str],
+        "Groups": Sequence[str],
         "Ipv6AddressCount": int,
-        "Ipv6Addresses": List[InstanceIpv6AddressTypeDef],
+        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
         "NetworkInterfaceId": str,
         "PrivateIpAddress": str,
-        "PrivateIpAddresses": List[PrivateIpAddressSpecificationTypeDef],
+        "PrivateIpAddresses": Sequence[PrivateIpAddressSpecificationTypeDef],
         "SecondaryPrivateIpAddressCount": int,
         "SubnetId": str,
         "AssociateCarrierIpAddress": bool,
         "InterfaceType": str,
         "NetworkCardIndex": int,
-        "Ipv4Prefixes": List[Ipv4PrefixSpecificationRequestTypeDef],
+        "Ipv4Prefixes": Sequence[Ipv4PrefixSpecificationRequestTypeDef],
         "Ipv4PrefixCount": int,
-        "Ipv6Prefixes": List[Ipv6PrefixSpecificationRequestTypeDef],
+        "Ipv6Prefixes": Sequence[Ipv6PrefixSpecificationRequestTypeDef],
         "Ipv6PrefixCount": int,
     },
     total=False,
 )
 
-InstanceNetworkInterfaceSpecificationTypeDef = TypedDict(
-    "InstanceNetworkInterfaceSpecificationTypeDef",
+InstanceNetworkInterfaceSpecificationSubnetTypeDef = TypedDict(
+    "InstanceNetworkInterfaceSpecificationSubnetTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "DeleteOnTermination": bool,
         "Description": str,
         "DeviceIndex": int,
         "Groups": Sequence[str],
         "Ipv6AddressCount": int,
@@ -17629,14 +17589,40 @@
         "Ipv4PrefixCount": int,
         "Ipv6Prefixes": Sequence[Ipv6PrefixSpecificationRequestTypeDef],
         "Ipv6PrefixCount": int,
     },
     total=False,
 )
 
+InstanceNetworkInterfaceSpecificationTypeDef = TypedDict(
+    "InstanceNetworkInterfaceSpecificationTypeDef",
+    {
+        "AssociatePublicIpAddress": bool,
+        "DeleteOnTermination": bool,
+        "Description": str,
+        "DeviceIndex": int,
+        "Groups": List[str],
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": List[InstanceIpv6AddressTypeDef],
+        "NetworkInterfaceId": str,
+        "PrivateIpAddress": str,
+        "PrivateIpAddresses": List[PrivateIpAddressSpecificationTypeDef],
+        "SecondaryPrivateIpAddressCount": int,
+        "SubnetId": str,
+        "AssociateCarrierIpAddress": bool,
+        "InterfaceType": str,
+        "NetworkCardIndex": int,
+        "Ipv4Prefixes": List[Ipv4PrefixSpecificationRequestTypeDef],
+        "Ipv4PrefixCount": int,
+        "Ipv6Prefixes": List[Ipv6PrefixSpecificationRequestTypeDef],
+        "Ipv6PrefixCount": int,
+    },
+    total=False,
+)
+
 CreateReservedInstancesListingRequestRequestTypeDef = TypedDict(
     "CreateReservedInstancesListingRequestRequestTypeDef",
     {
         "ClientToken": str,
         "InstanceCount": int,
         "PriceSchedules": Sequence[PriceScheduleSpecificationTypeDef],
         "ReservedInstancesId": str,
@@ -23030,30 +23016,14 @@
     {
         "Images": List[ImageRecycleBinInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LocalGatewayRouteTableTypeDef = TypedDict(
-    "LocalGatewayRouteTableTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-        "LocalGatewayRouteTableArn": str,
-        "LocalGatewayId": str,
-        "OutpostArn": str,
-        "OwnerId": str,
-        "State": str,
-        "Tags": List[TagTypeDef],
-        "Mode": LocalGatewayRouteTableModeType,
-        "StateReason": StateReasonTypeDef,
-    },
-    total=False,
-)
-
 ImportInstanceLaunchSpecificationTypeDef = TypedDict(
     "ImportInstanceLaunchSpecificationTypeDef",
     {
         "AdditionalInfo": str,
         "Architecture": ArchitectureValuesType,
         "GroupIds": Sequence[str],
         "GroupNames": Sequence[str],
@@ -23150,74 +23120,14 @@
         "Primary": bool,
         "PrivateDnsName": str,
         "PrivateIpAddress": str,
     },
     total=False,
 )
 
-InstanceRequirementsOutputTypeDef = TypedDict(
-    "InstanceRequirementsOutputTypeDef",
-    {
-        "VCpuCount": VCpuCountRangeTypeDef,
-        "MemoryMiB": MemoryMiBTypeDef,
-        "CpuManufacturers": List[CpuManufacturerType],
-        "MemoryGiBPerVCpu": MemoryGiBPerVCpuTypeDef,
-        "ExcludedInstanceTypes": List[str],
-        "InstanceGenerations": List[InstanceGenerationType],
-        "SpotMaxPricePercentageOverLowestPrice": int,
-        "OnDemandMaxPricePercentageOverLowestPrice": int,
-        "BareMetal": BareMetalType,
-        "BurstablePerformance": BurstablePerformanceType,
-        "RequireHibernateSupport": bool,
-        "NetworkInterfaceCount": NetworkInterfaceCountTypeDef,
-        "LocalStorage": LocalStorageType,
-        "LocalStorageTypes": List[LocalStorageTypeType],
-        "TotalLocalStorageGB": TotalLocalStorageGBTypeDef,
-        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsTypeDef,
-        "AcceleratorTypes": List[AcceleratorTypeType],
-        "AcceleratorCount": AcceleratorCountTypeDef,
-        "AcceleratorManufacturers": List[AcceleratorManufacturerType],
-        "AcceleratorNames": List[AcceleratorNameType],
-        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBTypeDef,
-        "NetworkBandwidthGbps": NetworkBandwidthGbpsTypeDef,
-        "AllowedInstanceTypes": List[str],
-    },
-    total=False,
-)
-
-InstanceRequirementsTypeDef = TypedDict(
-    "InstanceRequirementsTypeDef",
-    {
-        "VCpuCount": VCpuCountRangeTypeDef,
-        "MemoryMiB": MemoryMiBTypeDef,
-        "CpuManufacturers": Sequence[CpuManufacturerType],
-        "MemoryGiBPerVCpu": MemoryGiBPerVCpuTypeDef,
-        "ExcludedInstanceTypes": Sequence[str],
-        "InstanceGenerations": Sequence[InstanceGenerationType],
-        "SpotMaxPricePercentageOverLowestPrice": int,
-        "OnDemandMaxPricePercentageOverLowestPrice": int,
-        "BareMetal": BareMetalType,
-        "BurstablePerformance": BurstablePerformanceType,
-        "RequireHibernateSupport": bool,
-        "NetworkInterfaceCount": NetworkInterfaceCountTypeDef,
-        "LocalStorage": LocalStorageType,
-        "LocalStorageTypes": Sequence[LocalStorageTypeType],
-        "TotalLocalStorageGB": TotalLocalStorageGBTypeDef,
-        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsTypeDef,
-        "AcceleratorTypes": Sequence[AcceleratorTypeType],
-        "AcceleratorCount": AcceleratorCountTypeDef,
-        "AcceleratorManufacturers": Sequence[AcceleratorManufacturerType],
-        "AcceleratorNames": Sequence[AcceleratorNameType],
-        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBTypeDef,
-        "NetworkBandwidthGbps": NetworkBandwidthGbpsTypeDef,
-        "AllowedInstanceTypes": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredInstanceRequirementsRequestTypeDef = TypedDict(
     "_RequiredInstanceRequirementsRequestTypeDef",
     {
         "VCpuCount": VCpuCountRangeRequestTypeDef,
         "MemoryMiB": MemoryMiBRequestTypeDef,
     },
 )
@@ -23252,14 +23162,44 @@
 
 class InstanceRequirementsRequestTypeDef(
     _RequiredInstanceRequirementsRequestTypeDef, _OptionalInstanceRequirementsRequestTypeDef
 ):
     pass
 
 
+InstanceRequirementsTypeDef = TypedDict(
+    "InstanceRequirementsTypeDef",
+    {
+        "VCpuCount": VCpuCountRangeTypeDef,
+        "MemoryMiB": MemoryMiBTypeDef,
+        "CpuManufacturers": List[CpuManufacturerType],
+        "MemoryGiBPerVCpu": MemoryGiBPerVCpuTypeDef,
+        "ExcludedInstanceTypes": List[str],
+        "InstanceGenerations": List[InstanceGenerationType],
+        "SpotMaxPricePercentageOverLowestPrice": int,
+        "OnDemandMaxPricePercentageOverLowestPrice": int,
+        "BareMetal": BareMetalType,
+        "BurstablePerformance": BurstablePerformanceType,
+        "RequireHibernateSupport": bool,
+        "NetworkInterfaceCount": NetworkInterfaceCountTypeDef,
+        "LocalStorage": LocalStorageType,
+        "LocalStorageTypes": List[LocalStorageTypeType],
+        "TotalLocalStorageGB": TotalLocalStorageGBTypeDef,
+        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsTypeDef,
+        "AcceleratorTypes": List[AcceleratorTypeType],
+        "AcceleratorCount": AcceleratorCountTypeDef,
+        "AcceleratorManufacturers": List[AcceleratorManufacturerType],
+        "AcceleratorNames": List[AcceleratorNameType],
+        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBTypeDef,
+        "NetworkBandwidthGbps": NetworkBandwidthGbpsTypeDef,
+        "AllowedInstanceTypes": List[str],
+    },
+    total=False,
+)
+
 InstanceStateChangeTypeDef = TypedDict(
     "InstanceStateChangeTypeDef",
     {
         "CurrentState": InstanceStateTypeDef,
         "InstanceId": str,
         "PreviousState": InstanceStateTypeDef,
     },
@@ -23279,38 +23219,38 @@
     "ModifyInstanceEventStartTimeResultTypeDef",
     {
         "Event": InstanceStatusEventTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IpPermissionOutputTypeDef = TypedDict(
-    "IpPermissionOutputTypeDef",
+IpPermissionTypeDef = TypedDict(
+    "IpPermissionTypeDef",
     {
         "FromPort": int,
         "IpProtocol": str,
-        "IpRanges": List[IpRangeTypeDef],
-        "Ipv6Ranges": List[Ipv6RangeTypeDef],
-        "PrefixListIds": List[PrefixListIdTypeDef],
+        "IpRanges": Sequence[IpRangeTypeDef],
+        "Ipv6Ranges": Sequence[Ipv6RangeTypeDef],
+        "PrefixListIds": Sequence[PrefixListIdTypeDef],
         "ToPort": int,
-        "UserIdGroupPairs": List[UserIdGroupPairTypeDef],
+        "UserIdGroupPairs": Sequence[UserIdGroupPairTypeDef],
     },
     total=False,
 )
 
-IpPermissionTypeDef = TypedDict(
-    "IpPermissionTypeDef",
+IpPermissionVpcAddressTypeDef = TypedDict(
+    "IpPermissionVpcAddressTypeDef",
     {
         "FromPort": int,
         "IpProtocol": str,
-        "IpRanges": Sequence[IpRangeTypeDef],
-        "Ipv6Ranges": Sequence[Ipv6RangeTypeDef],
-        "PrefixListIds": Sequence[PrefixListIdTypeDef],
+        "IpRanges": List[IpRangeTypeDef],
+        "Ipv6Ranges": List[Ipv6RangeTypeDef],
+        "PrefixListIds": List[PrefixListIdTypeDef],
         "ToPort": int,
-        "UserIdGroupPairs": Sequence[UserIdGroupPairTypeDef],
+        "UserIdGroupPairs": List[UserIdGroupPairTypeDef],
     },
     total=False,
 )
 
 StaleIpPermissionTypeDef = TypedDict(
     "StaleIpPermissionTypeDef",
     {
@@ -24123,22 +24063,14 @@
     "RegisterTransitGatewayMulticastGroupSourcesResultTypeDef",
     {
         "RegisteredMulticastGroupSources": TransitGatewayMulticastRegisteredGroupSourcesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StorageOutputTypeDef = TypedDict(
-    "StorageOutputTypeDef",
-    {
-        "S3": S3StorageOutputTypeDef,
-    },
-    total=False,
-)
-
 ScheduledInstanceAvailabilityTypeDef = TypedDict(
     "ScheduledInstanceAvailabilityTypeDef",
     {
         "AvailabilityZone": str,
         "AvailableInstanceCount": int,
         "FirstSlotStartTime": datetime,
         "HourlyPrice": str,
@@ -24402,26 +24334,18 @@
     {
         "ReservationValue": ReservationValueTypeDef,
         "TargetConfiguration": TargetConfigurationTypeDef,
     },
     total=False,
 )
 
-TargetGroupsConfigOutputTypeDef = TypedDict(
-    "TargetGroupsConfigOutputTypeDef",
-    {
-        "TargetGroups": List[TargetGroupTypeDef],
-    },
-    total=False,
-)
-
 TargetGroupsConfigTypeDef = TypedDict(
     "TargetGroupsConfigTypeDef",
     {
-        "TargetGroups": Sequence[TargetGroupTypeDef],
+        "TargetGroups": List[TargetGroupTypeDef],
     },
     total=False,
 )
 
 TrafficMirrorFilterRuleTypeDef = TypedDict(
     "TrafficMirrorFilterRuleTypeDef",
     {
@@ -24793,14 +24717,30 @@
         "PeeringOptions": VpcPeeringConnectionOptionsDescriptionTypeDef,
         "VpcId": str,
         "Region": str,
     },
     total=False,
 )
 
+LocalGatewayRouteTableTypeDef = TypedDict(
+    "LocalGatewayRouteTableTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+        "LocalGatewayRouteTableArn": str,
+        "LocalGatewayId": str,
+        "OutpostArn": str,
+        "OwnerId": str,
+        "State": str,
+        "Tags": List[TagTypeDef],
+        "Mode": LocalGatewayRouteTableModeType,
+        "StateReason": StateReasonTypeDef,
+    },
+    total=False,
+)
+
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -25345,14 +25285,135 @@
         "SubnetIpv4CidrReservations": List[SubnetCidrReservationTypeDef],
         "SubnetIpv6CidrReservations": List[SubnetCidrReservationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredAcceptAddressTransferRequestRequestTypeDef = TypedDict(
+    "_RequiredAcceptAddressTransferRequestRequestTypeDef",
+    {
+        "Address": str,
+    },
+)
+_OptionalAcceptAddressTransferRequestRequestTypeDef = TypedDict(
+    "_OptionalAcceptAddressTransferRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class AcceptAddressTransferRequestRequestTypeDef(
+    _RequiredAcceptAddressTransferRequestRequestTypeDef,
+    _OptionalAcceptAddressTransferRequestRequestTypeDef,
+):
+    pass
+
+
+AllocateAddressRequestRequestTypeDef = TypedDict(
+    "AllocateAddressRequestRequestTypeDef",
+    {
+        "Domain": DomainTypeType,
+        "Address": str,
+        "PublicIpv4Pool": str,
+        "NetworkBorderGroup": str,
+        "CustomerOwnedIpv4Pool": str,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+_RequiredAllocateHostsRequestRequestTypeDef = TypedDict(
+    "_RequiredAllocateHostsRequestRequestTypeDef",
+    {
+        "AvailabilityZone": str,
+    },
+)
+_OptionalAllocateHostsRequestRequestTypeDef = TypedDict(
+    "_OptionalAllocateHostsRequestRequestTypeDef",
+    {
+        "AutoPlacement": AutoPlacementType,
+        "ClientToken": str,
+        "InstanceType": str,
+        "InstanceFamily": str,
+        "Quantity": int,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "HostRecovery": HostRecoveryType,
+        "OutpostArn": str,
+        "HostMaintenance": HostMaintenanceType,
+        "AssetIds": Sequence[str],
+    },
+    total=False,
+)
+
+
+class AllocateHostsRequestRequestTypeDef(
+    _RequiredAllocateHostsRequestRequestTypeDef, _OptionalAllocateHostsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredAssociateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateIpamResourceDiscoveryRequestRequestTypeDef",
+    {
+        "IpamId": str,
+        "IpamResourceDiscoveryId": str,
+    },
+)
+_OptionalAssociateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateIpamResourceDiscoveryRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class AssociateIpamResourceDiscoveryRequestRequestTypeDef(
+    _RequiredAssociateIpamResourceDiscoveryRequestRequestTypeDef,
+    _OptionalAssociateIpamResourceDiscoveryRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCopySnapshotRequestRequestTypeDef = TypedDict(
+    "_RequiredCopySnapshotRequestRequestTypeDef",
+    {
+        "SourceRegion": str,
+        "SourceSnapshotId": str,
+    },
+)
+_OptionalCopySnapshotRequestRequestTypeDef = TypedDict(
+    "_OptionalCopySnapshotRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DestinationOutpostArn": str,
+        "DestinationRegion": str,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "PresignedUrl": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CopySnapshotRequestRequestTypeDef(
+    _RequiredCopySnapshotRequestRequestTypeDef, _OptionalCopySnapshotRequestRequestTypeDef
+):
+    pass
+
+
 _RequiredCopySnapshotRequestSnapshotCopyTypeDef = TypedDict(
     "_RequiredCopySnapshotRequestSnapshotCopyTypeDef",
     {
         "SourceRegion": str,
     },
 )
 _OptionalCopySnapshotRequestSnapshotCopyTypeDef = TypedDict(
@@ -25373,23 +25434,748 @@
 
 class CopySnapshotRequestSnapshotCopyTypeDef(
     _RequiredCopySnapshotRequestSnapshotCopyTypeDef, _OptionalCopySnapshotRequestSnapshotCopyTypeDef
 ):
     pass
 
 
+_RequiredCreateCapacityReservationFleetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCapacityReservationFleetRequestRequestTypeDef",
+    {
+        "InstanceTypeSpecifications": Sequence[ReservationFleetInstanceSpecificationTypeDef],
+        "TotalTargetCapacity": int,
+    },
+)
+_OptionalCreateCapacityReservationFleetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCapacityReservationFleetRequestRequestTypeDef",
+    {
+        "AllocationStrategy": str,
+        "ClientToken": str,
+        "Tenancy": Literal["default"],
+        "EndDate": TimestampTypeDef,
+        "InstanceMatchCriteria": Literal["open"],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateCapacityReservationFleetRequestRequestTypeDef(
+    _RequiredCreateCapacityReservationFleetRequestRequestTypeDef,
+    _OptionalCreateCapacityReservationFleetRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateCapacityReservationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCapacityReservationRequestRequestTypeDef",
+    {
+        "InstanceType": str,
+        "InstancePlatform": CapacityReservationInstancePlatformType,
+        "InstanceCount": int,
+    },
+)
+_OptionalCreateCapacityReservationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCapacityReservationRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "AvailabilityZone": str,
+        "AvailabilityZoneId": str,
+        "Tenancy": CapacityReservationTenancyType,
+        "EbsOptimized": bool,
+        "EphemeralStorage": bool,
+        "EndDate": TimestampTypeDef,
+        "EndDateType": EndDateTypeType,
+        "InstanceMatchCriteria": InstanceMatchCriteriaType,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "OutpostArn": str,
+        "PlacementGroupArn": str,
+    },
+    total=False,
+)
+
+
+class CreateCapacityReservationRequestRequestTypeDef(
+    _RequiredCreateCapacityReservationRequestRequestTypeDef,
+    _OptionalCreateCapacityReservationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateCarrierGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCarrierGatewayRequestRequestTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateCarrierGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCarrierGatewayRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateCarrierGatewayRequestRequestTypeDef(
+    _RequiredCreateCarrierGatewayRequestRequestTypeDef,
+    _OptionalCreateCarrierGatewayRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateCoipPoolRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCoipPoolRequestRequestTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+    },
+)
+_OptionalCreateCoipPoolRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCoipPoolRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateCoipPoolRequestRequestTypeDef(
+    _RequiredCreateCoipPoolRequestRequestTypeDef, _OptionalCreateCoipPoolRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateCustomerGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCustomerGatewayRequestRequestTypeDef",
+    {
+        "Type": Literal["ipsec.1"],
+    },
+)
+_OptionalCreateCustomerGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCustomerGatewayRequestRequestTypeDef",
+    {
+        "BgpAsn": int,
+        "PublicIp": str,
+        "CertificateArn": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DeviceName": str,
+        "IpAddress": str,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateCustomerGatewayRequestRequestTypeDef(
+    _RequiredCreateCustomerGatewayRequestRequestTypeDef,
+    _OptionalCreateCustomerGatewayRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateDhcpOptionsRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDhcpOptionsRequestRequestTypeDef",
+    {
+        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
+    },
+)
+_OptionalCreateDhcpOptionsRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDhcpOptionsRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateDhcpOptionsRequestRequestTypeDef(
+    _RequiredCreateDhcpOptionsRequestRequestTypeDef, _OptionalCreateDhcpOptionsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef = TypedDict(
+    "_RequiredCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
+    {
+        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
+    },
+)
+_OptionalCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef = TypedDict(
+    "_OptionalCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef(
+    _RequiredCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef,
+    _OptionalCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef,
+):
+    pass
+
+
+_RequiredCreateEgressOnlyInternetGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEgressOnlyInternetGatewayRequestRequestTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateEgressOnlyInternetGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEgressOnlyInternetGatewayRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateEgressOnlyInternetGatewayRequestRequestTypeDef(
+    _RequiredCreateEgressOnlyInternetGatewayRequestRequestTypeDef,
+    _OptionalCreateEgressOnlyInternetGatewayRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateFlowLogsRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFlowLogsRequestRequestTypeDef",
+    {
+        "ResourceIds": Sequence[str],
+        "ResourceType": FlowLogsResourceTypeType,
+    },
+)
+_OptionalCreateFlowLogsRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFlowLogsRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "ClientToken": str,
+        "DeliverLogsPermissionArn": str,
+        "DeliverCrossAccountRole": str,
+        "LogGroupName": str,
+        "TrafficType": TrafficTypeType,
+        "LogDestinationType": LogDestinationTypeType,
+        "LogDestination": str,
+        "LogFormat": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "MaxAggregationInterval": int,
+        "DestinationOptions": DestinationOptionsRequestTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateFlowLogsRequestRequestTypeDef(
+    _RequiredCreateFlowLogsRequestRequestTypeDef, _OptionalCreateFlowLogsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateFpgaImageRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFpgaImageRequestRequestTypeDef",
+    {
+        "InputStorageLocation": StorageLocationTypeDef,
+    },
+)
+_OptionalCreateFpgaImageRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFpgaImageRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "LogsStorageLocation": StorageLocationTypeDef,
+        "Description": str,
+        "Name": str,
+        "ClientToken": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateFpgaImageRequestRequestTypeDef(
+    _RequiredCreateFpgaImageRequestRequestTypeDef, _OptionalCreateFpgaImageRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateInstanceConnectEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInstanceConnectEndpointRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+    },
+)
+_OptionalCreateInstanceConnectEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInstanceConnectEndpointRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "SecurityGroupIds": Sequence[str],
+        "PreserveClientIp": bool,
+        "ClientToken": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateInstanceConnectEndpointRequestRequestTypeDef(
+    _RequiredCreateInstanceConnectEndpointRequestRequestTypeDef,
+    _OptionalCreateInstanceConnectEndpointRequestRequestTypeDef,
+):
+    pass
+
+
+CreateInstanceEventWindowRequestRequestTypeDef = TypedDict(
+    "CreateInstanceEventWindowRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "Name": str,
+        "TimeRanges": Sequence[InstanceEventWindowTimeRangeRequestTypeDef],
+        "CronExpression": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateInstanceExportTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInstanceExportTaskRequestRequestTypeDef",
+    {
+        "ExportToS3Task": ExportToS3TaskSpecificationTypeDef,
+        "InstanceId": str,
+        "TargetEnvironment": ExportEnvironmentType,
+    },
+)
+_OptionalCreateInstanceExportTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInstanceExportTaskRequestRequestTypeDef",
+    {
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateInstanceExportTaskRequestRequestTypeDef(
+    _RequiredCreateInstanceExportTaskRequestRequestTypeDef,
+    _OptionalCreateInstanceExportTaskRequestRequestTypeDef,
+):
+    pass
+
+
+CreateInternetGatewayRequestRequestTypeDef = TypedDict(
+    "CreateInternetGatewayRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef = TypedDict(
+    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+_RequiredCreateIpamPoolRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIpamPoolRequestRequestTypeDef",
+    {
+        "IpamScopeId": str,
+        "AddressFamily": AddressFamilyType,
+    },
+)
+_OptionalCreateIpamPoolRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIpamPoolRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "Locale": str,
+        "SourceIpamPoolId": str,
+        "Description": str,
+        "AutoImport": bool,
+        "PubliclyAdvertisable": bool,
+        "AllocationMinNetmaskLength": int,
+        "AllocationMaxNetmaskLength": int,
+        "AllocationDefaultNetmaskLength": int,
+        "AllocationResourceTags": Sequence[RequestIpamResourceTagTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+        "AwsService": Literal["ec2"],
+        "PublicIpSource": IpamPoolPublicIpSourceType,
+    },
+    total=False,
+)
+
+
+class CreateIpamPoolRequestRequestTypeDef(
+    _RequiredCreateIpamPoolRequestRequestTypeDef, _OptionalCreateIpamPoolRequestRequestTypeDef
+):
+    pass
+
+
+CreateIpamRequestRequestTypeDef = TypedDict(
+    "CreateIpamRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "Description": str,
+        "OperatingRegions": Sequence[AddIpamOperatingRegionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+CreateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
+    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "Description": str,
+        "OperatingRegions": Sequence[AddIpamOperatingRegionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+_RequiredCreateIpamScopeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIpamScopeRequestRequestTypeDef",
+    {
+        "IpamId": str,
+    },
+)
+_OptionalCreateIpamScopeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIpamScopeRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateIpamScopeRequestRequestTypeDef(
+    _RequiredCreateIpamScopeRequestRequestTypeDef, _OptionalCreateIpamScopeRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateKeyPairRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyPairRequestRequestTypeDef",
+    {
+        "KeyName": str,
+    },
+)
+_OptionalCreateKeyPairRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyPairRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "KeyType": KeyTypeType,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "KeyFormat": KeyFormatType,
+    },
+    total=False,
+)
+
+
+class CreateKeyPairRequestRequestTypeDef(
+    _RequiredCreateKeyPairRequestRequestTypeDef, _OptionalCreateKeyPairRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef = TypedDict(
+    "_RequiredCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
+    {
+        "KeyName": str,
+    },
+)
+_OptionalCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef = TypedDict(
+    "_OptionalCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
+    {
+        "DryRun": bool,
+        "KeyType": KeyTypeType,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "KeyFormat": KeyFormatType,
+    },
+    total=False,
+)
+
+
+class CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef(
+    _RequiredCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef,
+    _OptionalCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef,
+):
+    pass
+
+
+_RequiredCreateLocalGatewayRouteTableRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLocalGatewayRouteTableRequestRequestTypeDef",
+    {
+        "LocalGatewayId": str,
+    },
+)
+_OptionalCreateLocalGatewayRouteTableRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLocalGatewayRouteTableRequestRequestTypeDef",
+    {
+        "Mode": LocalGatewayRouteTableModeType,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateLocalGatewayRouteTableRequestRequestTypeDef(
+    _RequiredCreateLocalGatewayRouteTableRequestRequestTypeDef,
+    _OptionalCreateLocalGatewayRouteTableRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+        "LocalGatewayVirtualInterfaceGroupId": str,
+    },
+)
+_OptionalCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef(
+    _RequiredCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef,
+    _OptionalCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+        "VpcId": str,
+    },
+)
+_OptionalCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef(
+    _RequiredCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef,
+    _OptionalCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateManagedPrefixListRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateManagedPrefixListRequestRequestTypeDef",
+    {
+        "PrefixListName": str,
+        "MaxEntries": int,
+        "AddressFamily": str,
+    },
+)
+_OptionalCreateManagedPrefixListRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateManagedPrefixListRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "Entries": Sequence[AddPrefixListEntryTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateManagedPrefixListRequestRequestTypeDef(
+    _RequiredCreateManagedPrefixListRequestRequestTypeDef,
+    _OptionalCreateManagedPrefixListRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateNatGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNatGatewayRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+    },
+)
+_OptionalCreateNatGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNatGatewayRequestRequestTypeDef",
+    {
+        "AllocationId": str,
+        "ClientToken": str,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ConnectivityType": ConnectivityTypeType,
+        "PrivateIpAddress": str,
+        "SecondaryAllocationIds": Sequence[str],
+        "SecondaryPrivateIpAddresses": Sequence[str],
+        "SecondaryPrivateIpAddressCount": int,
+    },
+    total=False,
+)
+
+
+class CreateNatGatewayRequestRequestTypeDef(
+    _RequiredCreateNatGatewayRequestRequestTypeDef, _OptionalCreateNatGatewayRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateNetworkAclRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNetworkAclRequestRequestTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateNetworkAclRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNetworkAclRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateNetworkAclRequestRequestTypeDef(
+    _RequiredCreateNetworkAclRequestRequestTypeDef, _OptionalCreateNetworkAclRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef = TypedDict(
+    "_RequiredCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef = TypedDict(
+    "_OptionalCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef(
+    _RequiredCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef,
+    _OptionalCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef,
+):
+    pass
+
+
 CreateNetworkAclRequestVpcCreateNetworkAclTypeDef = TypedDict(
     "CreateNetworkAclRequestVpcCreateNetworkAclTypeDef",
     {
         "DryRun": bool,
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
     total=False,
 )
 
+_RequiredCreateNetworkInterfaceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNetworkInterfaceRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+    },
+)
+_OptionalCreateNetworkInterfaceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNetworkInterfaceRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DryRun": bool,
+        "Groups": Sequence[str],
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
+        "PrivateIpAddress": str,
+        "PrivateIpAddresses": Sequence[PrivateIpAddressSpecificationTypeDef],
+        "SecondaryPrivateIpAddressCount": int,
+        "Ipv4Prefixes": Sequence[Ipv4PrefixSpecificationRequestTypeDef],
+        "Ipv4PrefixCount": int,
+        "Ipv6Prefixes": Sequence[Ipv6PrefixSpecificationRequestTypeDef],
+        "Ipv6PrefixCount": int,
+        "InterfaceType": NetworkInterfaceCreationTypeType,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateNetworkInterfaceRequestRequestTypeDef(
+    _RequiredCreateNetworkInterfaceRequestRequestTypeDef,
+    _OptionalCreateNetworkInterfaceRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef = TypedDict(
+    "_RequiredCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
+    {
+        "SubnetId": str,
+    },
+)
+_OptionalCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef = TypedDict(
+    "_OptionalCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
+    {
+        "Description": str,
+        "DryRun": bool,
+        "Groups": Sequence[str],
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
+        "PrivateIpAddress": str,
+        "PrivateIpAddresses": Sequence[PrivateIpAddressSpecificationTypeDef],
+        "SecondaryPrivateIpAddressCount": int,
+        "Ipv4Prefixes": Sequence[Ipv4PrefixSpecificationRequestTypeDef],
+        "Ipv4PrefixCount": int,
+        "Ipv6Prefixes": Sequence[Ipv6PrefixSpecificationRequestTypeDef],
+        "Ipv6PrefixCount": int,
+        "InterfaceType": NetworkInterfaceCreationTypeType,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef(
+    _RequiredCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef,
+    _OptionalCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef,
+):
+    pass
+
+
 CreateNetworkInterfaceRequestSubnetCreateNetworkInterfaceTypeDef = TypedDict(
     "CreateNetworkInterfaceRequestSubnetCreateNetworkInterfaceTypeDef",
     {
         "Description": str,
         "DryRun": bool,
         "Groups": Sequence[str],
         "Ipv6AddressCount": int,
@@ -25404,23 +26190,205 @@
         "InterfaceType": NetworkInterfaceCreationTypeType,
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
+CreatePlacementGroupRequestRequestTypeDef = TypedDict(
+    "CreatePlacementGroupRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "GroupName": str,
+        "Strategy": PlacementStrategyType,
+        "PartitionCount": int,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "SpreadLevel": SpreadLevelType,
+    },
+    total=False,
+)
+
+CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef = TypedDict(
+    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
+    {
+        "DryRun": bool,
+        "GroupName": str,
+        "Strategy": PlacementStrategyType,
+        "PartitionCount": int,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "SpreadLevel": SpreadLevelType,
+    },
+    total=False,
+)
+
+CreatePublicIpv4PoolRequestRequestTypeDef = TypedDict(
+    "CreatePublicIpv4PoolRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateReplaceRootVolumeTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReplaceRootVolumeTaskRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalCreateReplaceRootVolumeTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReplaceRootVolumeTaskRequestRequestTypeDef",
+    {
+        "SnapshotId": str,
+        "ClientToken": str,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ImageId": str,
+        "DeleteReplacedRootVolume": bool,
+    },
+    total=False,
+)
+
+
+class CreateReplaceRootVolumeTaskRequestRequestTypeDef(
+    _RequiredCreateReplaceRootVolumeTaskRequestRequestTypeDef,
+    _OptionalCreateReplaceRootVolumeTaskRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateRestoreImageTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRestoreImageTaskRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "ObjectKey": str,
+    },
+)
+_OptionalCreateRestoreImageTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRestoreImageTaskRequestRequestTypeDef",
+    {
+        "Name": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateRestoreImageTaskRequestRequestTypeDef(
+    _RequiredCreateRestoreImageTaskRequestRequestTypeDef,
+    _OptionalCreateRestoreImageTaskRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateRouteTableRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRouteTableRequestRequestTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateRouteTableRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRouteTableRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateRouteTableRequestRequestTypeDef(
+    _RequiredCreateRouteTableRequestRequestTypeDef, _OptionalCreateRouteTableRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef = TypedDict(
+    "_RequiredCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef = TypedDict(
+    "_OptionalCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef(
+    _RequiredCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef,
+    _OptionalCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef,
+):
+    pass
+
+
 CreateRouteTableRequestVpcCreateRouteTableTypeDef = TypedDict(
     "CreateRouteTableRequestVpcCreateRouteTableTypeDef",
     {
         "DryRun": bool,
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
     total=False,
 )
 
+_RequiredCreateSecurityGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSecurityGroupRequestRequestTypeDef",
+    {
+        "Description": str,
+        "GroupName": str,
+    },
+)
+_OptionalCreateSecurityGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSecurityGroupRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateSecurityGroupRequestRequestTypeDef(
+    _RequiredCreateSecurityGroupRequestRequestTypeDef,
+    _OptionalCreateSecurityGroupRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef = TypedDict(
+    "_RequiredCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
+    {
+        "Description": str,
+        "GroupName": str,
+    },
+)
+_OptionalCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef = TypedDict(
+    "_OptionalCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
+    {
+        "VpcId": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef(
+    _RequiredCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef,
+    _OptionalCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef,
+):
+    pass
+
+
 _RequiredCreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef = TypedDict(
     "_RequiredCreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef",
     {
         "Description": str,
         "GroupName": str,
     },
 )
@@ -25437,25 +26405,182 @@
 class CreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef(
     _RequiredCreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef,
     _OptionalCreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef,
 ):
     pass
 
 
+_RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSnapshotRequestRequestTypeDef",
+    {
+        "VolumeId": str,
+    },
+)
+_OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSnapshotRequestRequestTypeDef",
+    {
+        "Description": str,
+        "OutpostArn": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateSnapshotRequestRequestTypeDef(
+    _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef = TypedDict(
+    "_RequiredCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
+    {
+        "VolumeId": str,
+    },
+)
+_OptionalCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef = TypedDict(
+    "_OptionalCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
+    {
+        "Description": str,
+        "OutpostArn": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef(
+    _RequiredCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef,
+    _OptionalCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef,
+):
+    pass
+
+
 CreateSnapshotRequestVolumeCreateSnapshotTypeDef = TypedDict(
     "CreateSnapshotRequestVolumeCreateSnapshotTypeDef",
     {
         "Description": str,
         "OutpostArn": str,
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "DryRun": bool,
     },
     total=False,
 )
 
+_RequiredCreateSnapshotsRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSnapshotsRequestRequestTypeDef",
+    {
+        "InstanceSpecification": InstanceSpecificationTypeDef,
+    },
+)
+_OptionalCreateSnapshotsRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSnapshotsRequestRequestTypeDef",
+    {
+        "Description": str,
+        "OutpostArn": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "CopyTagsFromSource": Literal["volume"],
+    },
+    total=False,
+)
+
+
+class CreateSnapshotsRequestRequestTypeDef(
+    _RequiredCreateSnapshotsRequestRequestTypeDef, _OptionalCreateSnapshotsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateSubnetCidrReservationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSubnetCidrReservationRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+        "Cidr": str,
+        "ReservationType": SubnetCidrReservationTypeType,
+    },
+)
+_OptionalCreateSubnetCidrReservationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSubnetCidrReservationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateSubnetCidrReservationRequestRequestTypeDef(
+    _RequiredCreateSubnetCidrReservationRequestRequestTypeDef,
+    _OptionalCreateSubnetCidrReservationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateSubnetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSubnetRequestRequestTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateSubnetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSubnetRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "AvailabilityZone": str,
+        "AvailabilityZoneId": str,
+        "CidrBlock": str,
+        "Ipv6CidrBlock": str,
+        "OutpostArn": str,
+        "DryRun": bool,
+        "Ipv6Native": bool,
+    },
+    total=False,
+)
+
+
+class CreateSubnetRequestRequestTypeDef(
+    _RequiredCreateSubnetRequestRequestTypeDef, _OptionalCreateSubnetRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateSubnetRequestServiceResourceCreateSubnetTypeDef = TypedDict(
+    "_RequiredCreateSubnetRequestServiceResourceCreateSubnetTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateSubnetRequestServiceResourceCreateSubnetTypeDef = TypedDict(
+    "_OptionalCreateSubnetRequestServiceResourceCreateSubnetTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "AvailabilityZone": str,
+        "AvailabilityZoneId": str,
+        "CidrBlock": str,
+        "Ipv6CidrBlock": str,
+        "OutpostArn": str,
+        "DryRun": bool,
+        "Ipv6Native": bool,
+    },
+    total=False,
+)
+
+
+class CreateSubnetRequestServiceResourceCreateSubnetTypeDef(
+    _RequiredCreateSubnetRequestServiceResourceCreateSubnetTypeDef,
+    _OptionalCreateSubnetRequestServiceResourceCreateSubnetTypeDef,
+):
+    pass
+
+
 CreateSubnetRequestVpcCreateSubnetTypeDef = TypedDict(
     "CreateSubnetRequestVpcCreateSubnetTypeDef",
     {
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "AvailabilityZone": str,
         "AvailabilityZoneId": str,
         "CidrBlock": str,
@@ -25463,27 +26588,794 @@
         "OutpostArn": str,
         "DryRun": bool,
         "Ipv6Native": bool,
     },
     total=False,
 )
 
+CreateTrafficMirrorFilterRequestRequestTypeDef = TypedDict(
+    "CreateTrafficMirrorFilterRequestRequestTypeDef",
+    {
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+_RequiredCreateTrafficMirrorSessionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTrafficMirrorSessionRequestRequestTypeDef",
+    {
+        "NetworkInterfaceId": str,
+        "TrafficMirrorTargetId": str,
+        "TrafficMirrorFilterId": str,
+        "SessionNumber": int,
+    },
+)
+_OptionalCreateTrafficMirrorSessionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTrafficMirrorSessionRequestRequestTypeDef",
+    {
+        "PacketLength": int,
+        "VirtualNetworkId": int,
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateTrafficMirrorSessionRequestRequestTypeDef(
+    _RequiredCreateTrafficMirrorSessionRequestRequestTypeDef,
+    _OptionalCreateTrafficMirrorSessionRequestRequestTypeDef,
+):
+    pass
+
+
+CreateTrafficMirrorTargetRequestRequestTypeDef = TypedDict(
+    "CreateTrafficMirrorTargetRequestRequestTypeDef",
+    {
+        "NetworkInterfaceId": str,
+        "NetworkLoadBalancerArn": str,
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "ClientToken": str,
+        "GatewayLoadBalancerEndpointId": str,
+    },
+    total=False,
+)
+
+_RequiredCreateTransitGatewayConnectPeerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayConnectPeerRequestRequestTypeDef",
+    {
+        "TransitGatewayAttachmentId": str,
+        "PeerAddress": str,
+        "InsideCidrBlocks": Sequence[str],
+    },
+)
+_OptionalCreateTransitGatewayConnectPeerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayConnectPeerRequestRequestTypeDef",
+    {
+        "TransitGatewayAddress": str,
+        "BgpOptions": TransitGatewayConnectRequestBgpOptionsTypeDef,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateTransitGatewayConnectPeerRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayConnectPeerRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayConnectPeerRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateTransitGatewayConnectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayConnectRequestRequestTypeDef",
+    {
+        "TransportTransitGatewayAttachmentId": str,
+        "Options": CreateTransitGatewayConnectRequestOptionsTypeDef,
+    },
+)
+_OptionalCreateTransitGatewayConnectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayConnectRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateTransitGatewayConnectRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayConnectRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayConnectRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateTransitGatewayMulticastDomainRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayMulticastDomainRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+    },
+)
+_OptionalCreateTransitGatewayMulticastDomainRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayMulticastDomainRequestRequestTypeDef",
+    {
+        "Options": CreateTransitGatewayMulticastDomainRequestOptionsTypeDef,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateTransitGatewayMulticastDomainRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayMulticastDomainRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayMulticastDomainRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "PeerTransitGatewayId": str,
+        "PeerAccountId": str,
+        "PeerRegion": str,
+    },
+)
+_OptionalCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
+    {
+        "Options": CreateTransitGatewayPeeringAttachmentRequestOptionsTypeDef,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateTransitGatewayPolicyTableRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayPolicyTableRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+    },
+)
+_OptionalCreateTransitGatewayPolicyTableRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayPolicyTableRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateTransitGatewayPolicyTableRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayPolicyTableRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayPolicyTableRequestRequestTypeDef,
+):
+    pass
+
+
+CreateTransitGatewayRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Options": TransitGatewayRequestOptionsTypeDef,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+_RequiredCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
+    {
+        "TransitGatewayRouteTableId": str,
+        "PeeringAttachmentId": str,
+    },
+)
+_OptionalCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayRouteTableRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+    },
+)
+_OptionalCreateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayRouteTableRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateTransitGatewayRouteTableRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayRouteTableRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayRouteTableRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateTransitGatewayVpcAttachmentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "VpcId": str,
+        "SubnetIds": Sequence[str],
+    },
+)
+_OptionalCreateTransitGatewayVpcAttachmentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
+    {
+        "Options": CreateTransitGatewayVpcAttachmentRequestOptionsTypeDef,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateTransitGatewayVpcAttachmentRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayVpcAttachmentRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayVpcAttachmentRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateVerifiedAccessEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVerifiedAccessEndpointRequestRequestTypeDef",
+    {
+        "VerifiedAccessGroupId": str,
+        "EndpointType": VerifiedAccessEndpointTypeType,
+        "AttachmentType": Literal["vpc"],
+        "DomainCertificateArn": str,
+        "ApplicationDomain": str,
+        "EndpointDomainPrefix": str,
+    },
+)
+_OptionalCreateVerifiedAccessEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVerifiedAccessEndpointRequestRequestTypeDef",
+    {
+        "SecurityGroupIds": Sequence[str],
+        "LoadBalancerOptions": CreateVerifiedAccessEndpointLoadBalancerOptionsTypeDef,
+        "NetworkInterfaceOptions": CreateVerifiedAccessEndpointEniOptionsTypeDef,
+        "Description": str,
+        "PolicyDocument": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateVerifiedAccessEndpointRequestRequestTypeDef(
+    _RequiredCreateVerifiedAccessEndpointRequestRequestTypeDef,
+    _OptionalCreateVerifiedAccessEndpointRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateVerifiedAccessGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVerifiedAccessGroupRequestRequestTypeDef",
+    {
+        "VerifiedAccessInstanceId": str,
+    },
+)
+_OptionalCreateVerifiedAccessGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVerifiedAccessGroupRequestRequestTypeDef",
+    {
+        "Description": str,
+        "PolicyDocument": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateVerifiedAccessGroupRequestRequestTypeDef(
+    _RequiredCreateVerifiedAccessGroupRequestRequestTypeDef,
+    _OptionalCreateVerifiedAccessGroupRequestRequestTypeDef,
+):
+    pass
+
+
+CreateVerifiedAccessInstanceRequestRequestTypeDef = TypedDict(
+    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
+    {
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+_RequiredCreateVerifiedAccessTrustProviderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVerifiedAccessTrustProviderRequestRequestTypeDef",
+    {
+        "TrustProviderType": TrustProviderTypeType,
+        "PolicyReferenceName": str,
+    },
+)
+_OptionalCreateVerifiedAccessTrustProviderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVerifiedAccessTrustProviderRequestRequestTypeDef",
+    {
+        "UserTrustProviderType": UserTrustProviderTypeType,
+        "DeviceTrustProviderType": DeviceTrustProviderTypeType,
+        "OidcOptions": CreateVerifiedAccessTrustProviderOidcOptionsTypeDef,
+        "DeviceOptions": CreateVerifiedAccessTrustProviderDeviceOptionsTypeDef,
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateVerifiedAccessTrustProviderRequestRequestTypeDef(
+    _RequiredCreateVerifiedAccessTrustProviderRequestRequestTypeDef,
+    _OptionalCreateVerifiedAccessTrustProviderRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVolumeRequestRequestTypeDef",
+    {
+        "AvailabilityZone": str,
+    },
+)
+_OptionalCreateVolumeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVolumeRequestRequestTypeDef",
+    {
+        "Encrypted": bool,
+        "Iops": int,
+        "KmsKeyId": str,
+        "OutpostArn": str,
+        "Size": int,
+        "SnapshotId": str,
+        "VolumeType": VolumeTypeType,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "MultiAttachEnabled": bool,
+        "Throughput": int,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateVolumeRequestRequestTypeDef(
+    _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredCreateVolumeRequestServiceResourceCreateVolumeTypeDef = TypedDict(
+    "_RequiredCreateVolumeRequestServiceResourceCreateVolumeTypeDef",
+    {
+        "AvailabilityZone": str,
+    },
+)
+_OptionalCreateVolumeRequestServiceResourceCreateVolumeTypeDef = TypedDict(
+    "_OptionalCreateVolumeRequestServiceResourceCreateVolumeTypeDef",
+    {
+        "Encrypted": bool,
+        "Iops": int,
+        "KmsKeyId": str,
+        "OutpostArn": str,
+        "Size": int,
+        "SnapshotId": str,
+        "VolumeType": VolumeTypeType,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "MultiAttachEnabled": bool,
+        "Throughput": int,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class CreateVolumeRequestServiceResourceCreateVolumeTypeDef(
+    _RequiredCreateVolumeRequestServiceResourceCreateVolumeTypeDef,
+    _OptionalCreateVolumeRequestServiceResourceCreateVolumeTypeDef,
+):
+    pass
+
+
+_RequiredCreateVpcEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVpcEndpointRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "ServiceName": str,
+    },
+)
+_OptionalCreateVpcEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVpcEndpointRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "VpcEndpointType": VpcEndpointTypeType,
+        "PolicyDocument": str,
+        "RouteTableIds": Sequence[str],
+        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": Sequence[str],
+        "IpAddressType": IpAddressTypeType,
+        "DnsOptions": DnsOptionsSpecificationTypeDef,
+        "ClientToken": str,
+        "PrivateDnsEnabled": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateVpcEndpointRequestRequestTypeDef(
+    _RequiredCreateVpcEndpointRequestRequestTypeDef, _OptionalCreateVpcEndpointRequestRequestTypeDef
+):
+    pass
+
+
+CreateVpcEndpointServiceConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "AcceptanceRequired": bool,
+        "PrivateDnsName": str,
+        "NetworkLoadBalancerArns": Sequence[str],
+        "GatewayLoadBalancerArns": Sequence[str],
+        "SupportedIpAddressTypes": Sequence[str],
+        "ClientToken": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateVpcPeeringConnectionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVpcPeeringConnectionRequestRequestTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateVpcPeeringConnectionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVpcPeeringConnectionRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "PeerOwnerId": str,
+        "PeerVpcId": str,
+        "PeerRegion": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateVpcPeeringConnectionRequestRequestTypeDef(
+    _RequiredCreateVpcPeeringConnectionRequestRequestTypeDef,
+    _OptionalCreateVpcPeeringConnectionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef = TypedDict(
+    "_RequiredCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef = TypedDict(
+    "_OptionalCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
+    {
+        "DryRun": bool,
+        "PeerOwnerId": str,
+        "PeerVpcId": str,
+        "PeerRegion": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef(
+    _RequiredCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef,
+    _OptionalCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef,
+):
+    pass
+
+
 CreateVpcPeeringConnectionRequestVpcRequestVpcPeeringConnectionTypeDef = TypedDict(
     "CreateVpcPeeringConnectionRequestVpcRequestVpcPeeringConnectionTypeDef",
     {
         "DryRun": bool,
         "PeerOwnerId": str,
         "PeerVpcId": str,
         "PeerRegion": str,
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
     total=False,
 )
 
-TagSpecificationUnionTypeDef = Union[TagSpecificationTypeDef, TagSpecificationOutputTypeDef]
+CreateVpcRequestRequestTypeDef = TypedDict(
+    "CreateVpcRequestRequestTypeDef",
+    {
+        "CidrBlock": str,
+        "AmazonProvidedIpv6CidrBlock": bool,
+        "Ipv6Pool": str,
+        "Ipv6CidrBlock": str,
+        "Ipv4IpamPoolId": str,
+        "Ipv4NetmaskLength": int,
+        "Ipv6IpamPoolId": str,
+        "Ipv6NetmaskLength": int,
+        "DryRun": bool,
+        "InstanceTenancy": TenancyType,
+        "Ipv6CidrBlockNetworkBorderGroup": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+CreateVpcRequestServiceResourceCreateVpcTypeDef = TypedDict(
+    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
+    {
+        "CidrBlock": str,
+        "AmazonProvidedIpv6CidrBlock": bool,
+        "Ipv6Pool": str,
+        "Ipv6CidrBlock": str,
+        "Ipv4IpamPoolId": str,
+        "Ipv4NetmaskLength": int,
+        "Ipv6IpamPoolId": str,
+        "Ipv6NetmaskLength": int,
+        "DryRun": bool,
+        "InstanceTenancy": TenancyType,
+        "Ipv6CidrBlockNetworkBorderGroup": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateVpnGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVpnGatewayRequestRequestTypeDef",
+    {
+        "Type": Literal["ipsec.1"],
+    },
+)
+_OptionalCreateVpnGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVpnGatewayRequestRequestTypeDef",
+    {
+        "AvailabilityZone": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "AmazonSideAsn": int,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+
+class CreateVpnGatewayRequestRequestTypeDef(
+    _RequiredCreateVpnGatewayRequestRequestTypeDef, _OptionalCreateVpnGatewayRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredExportImageRequestRequestTypeDef = TypedDict(
+    "_RequiredExportImageRequestRequestTypeDef",
+    {
+        "DiskImageFormat": DiskImageFormatType,
+        "ImageId": str,
+        "S3ExportLocation": ExportTaskS3LocationRequestTypeDef,
+    },
+)
+_OptionalExportImageRequestRequestTypeDef = TypedDict(
+    "_OptionalExportImageRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "Description": str,
+        "DryRun": bool,
+        "RoleName": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class ExportImageRequestRequestTypeDef(
+    _RequiredExportImageRequestRequestTypeDef, _OptionalExportImageRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredImportKeyPairRequestRequestTypeDef = TypedDict(
+    "_RequiredImportKeyPairRequestRequestTypeDef",
+    {
+        "KeyName": str,
+        "PublicKeyMaterial": BlobTypeDef,
+    },
+)
+_OptionalImportKeyPairRequestRequestTypeDef = TypedDict(
+    "_OptionalImportKeyPairRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class ImportKeyPairRequestRequestTypeDef(
+    _RequiredImportKeyPairRequestRequestTypeDef, _OptionalImportKeyPairRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredImportKeyPairRequestServiceResourceImportKeyPairTypeDef = TypedDict(
+    "_RequiredImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
+    {
+        "KeyName": str,
+        "PublicKeyMaterial": BlobTypeDef,
+    },
+)
+_OptionalImportKeyPairRequestServiceResourceImportKeyPairTypeDef = TypedDict(
+    "_OptionalImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class ImportKeyPairRequestServiceResourceImportKeyPairTypeDef(
+    _RequiredImportKeyPairRequestServiceResourceImportKeyPairTypeDef,
+    _OptionalImportKeyPairRequestServiceResourceImportKeyPairTypeDef,
+):
+    pass
+
+
+_RequiredProvisionByoipCidrRequestRequestTypeDef = TypedDict(
+    "_RequiredProvisionByoipCidrRequestRequestTypeDef",
+    {
+        "Cidr": str,
+    },
+)
+_OptionalProvisionByoipCidrRequestRequestTypeDef = TypedDict(
+    "_OptionalProvisionByoipCidrRequestRequestTypeDef",
+    {
+        "CidrAuthorizationContext": CidrAuthorizationContextTypeDef,
+        "PubliclyAdvertisable": bool,
+        "Description": str,
+        "DryRun": bool,
+        "PoolTagSpecifications": Sequence[TagSpecificationTypeDef],
+        "MultiRegion": bool,
+    },
+    total=False,
+)
+
+
+class ProvisionByoipCidrRequestRequestTypeDef(
+    _RequiredProvisionByoipCidrRequestRequestTypeDef,
+    _OptionalProvisionByoipCidrRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredPurchaseHostReservationRequestRequestTypeDef = TypedDict(
+    "_RequiredPurchaseHostReservationRequestRequestTypeDef",
+    {
+        "HostIdSet": Sequence[str],
+        "OfferingId": str,
+    },
+)
+_OptionalPurchaseHostReservationRequestRequestTypeDef = TypedDict(
+    "_OptionalPurchaseHostReservationRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "CurrencyCode": Literal["USD"],
+        "LimitPrice": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class PurchaseHostReservationRequestRequestTypeDef(
+    _RequiredPurchaseHostReservationRequestRequestTypeDef,
+    _OptionalPurchaseHostReservationRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef = TypedDict(
+    "_RequiredStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
+    {
+        "NetworkInsightsAccessScopeId": str,
+        "ClientToken": str,
+    },
+)
+_OptionalStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef = TypedDict(
+    "_OptionalStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef(
+    _RequiredStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef,
+    _OptionalStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredStartNetworkInsightsAnalysisRequestRequestTypeDef = TypedDict(
+    "_RequiredStartNetworkInsightsAnalysisRequestRequestTypeDef",
+    {
+        "NetworkInsightsPathId": str,
+        "ClientToken": str,
+    },
+)
+_OptionalStartNetworkInsightsAnalysisRequestRequestTypeDef = TypedDict(
+    "_OptionalStartNetworkInsightsAnalysisRequestRequestTypeDef",
+    {
+        "AdditionalAccounts": Sequence[str],
+        "FilterInArns": Sequence[str],
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class StartNetworkInsightsAnalysisRequestRequestTypeDef(
+    _RequiredStartNetworkInsightsAnalysisRequestRequestTypeDef,
+    _OptionalStartNetworkInsightsAnalysisRequestRequestTypeDef,
+):
+    pass
+
+
 CreateTrafficMirrorSessionResultTypeDef = TypedDict(
     "CreateTrafficMirrorSessionResultTypeDef",
     {
         "TrafficMirrorSession": TrafficMirrorSessionTypeDef,
         "ClientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -25980,14 +27872,40 @@
 class CreateImageRequestInstanceCreateImageTypeDef(
     _RequiredCreateImageRequestInstanceCreateImageTypeDef,
     _OptionalCreateImageRequestInstanceCreateImageTypeDef,
 ):
     pass
 
 
+_RequiredCreateImageRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateImageRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+    },
+)
+_OptionalCreateImageRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateImageRequestRequestTypeDef",
+    {
+        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "Description": str,
+        "DryRun": bool,
+        "NoReboot": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateImageRequestRequestTypeDef(
+    _RequiredCreateImageRequestRequestTypeDef, _OptionalCreateImageRequestRequestTypeDef
+):
+    pass
+
+
 ImageAttributeTypeDef = TypedDict(
     "ImageAttributeTypeDef",
     {
         "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
         "ImageId": str,
         "LaunchPermissions": List[LaunchPermissionTypeDef],
         "ProductCodes": List[ProductCodeTypeDef],
@@ -26186,14 +28104,52 @@
     {
         "Instances": List[ClassicLinkInstanceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateClientVpnEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateClientVpnEndpointRequestRequestTypeDef",
+    {
+        "ClientCidrBlock": str,
+        "ServerCertificateArn": str,
+        "AuthenticationOptions": Sequence[ClientVpnAuthenticationRequestTypeDef],
+        "ConnectionLogOptions": ConnectionLogOptionsTypeDef,
+    },
+)
+_OptionalCreateClientVpnEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateClientVpnEndpointRequestRequestTypeDef",
+    {
+        "DnsServers": Sequence[str],
+        "TransportProtocol": TransportProtocolType,
+        "VpnPort": int,
+        "Description": str,
+        "SplitTunnel": bool,
+        "DryRun": bool,
+        "ClientToken": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "SecurityGroupIds": Sequence[str],
+        "VpcId": str,
+        "SelfServicePortal": SelfServicePortalType,
+        "ClientConnectOptions": ClientConnectOptionsTypeDef,
+        "SessionTimeoutHours": int,
+        "ClientLoginBannerOptions": ClientLoginBannerOptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateClientVpnEndpointRequestRequestTypeDef(
+    _RequiredCreateClientVpnEndpointRequestRequestTypeDef,
+    _OptionalCreateClientVpnEndpointRequestRequestTypeDef,
+):
+    pass
+
+
 ClientVpnEndpointTypeDef = TypedDict(
     "ClientVpnEndpointTypeDef",
     {
         "ClientVpnEndpointId": str,
         "Description": str,
         "Status": ClientVpnEndpointStatusTypeDef,
         "CreationTime": str,
@@ -26353,26 +28309,23 @@
         "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
         "EbsOptimized": bool,
         "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
         "ImageId": str,
         "InstanceType": InstanceTypeType,
         "KernelId": str,
         "KeyName": str,
-        "NetworkInterfaces": List[InstanceNetworkInterfaceSpecificationOutputTypeDef],
+        "NetworkInterfaces": List[InstanceNetworkInterfaceSpecificationTypeDef],
         "Placement": SpotPlacementTypeDef,
         "RamdiskId": str,
         "SubnetId": str,
         "Monitoring": RunInstancesMonitoringEnabledTypeDef,
     },
     total=False,
 )
 
-InstanceNetworkInterfaceSpecificationUnionTypeDef = Union[
-    InstanceNetworkInterfaceSpecificationTypeDef, InstanceNetworkInterfaceSpecificationOutputTypeDef
-]
 RequestSpotLaunchSpecificationTypeDef = TypedDict(
     "RequestSpotLaunchSpecificationTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SecurityGroups": Sequence[str],
         "AddressingType": str,
         "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
@@ -26981,37 +28934,51 @@
 class ModifyImageAttributeRequestRequestTypeDef(
     _RequiredModifyImageAttributeRequestRequestTypeDef,
     _OptionalModifyImageAttributeRequestRequestTypeDef,
 ):
     pass
 
 
-CreateLocalGatewayRouteTableResultTypeDef = TypedDict(
-    "CreateLocalGatewayRouteTableResultTypeDef",
-    {
-        "LocalGatewayRouteTable": LocalGatewayRouteTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteLocalGatewayRouteTableResultTypeDef = TypedDict(
-    "DeleteLocalGatewayRouteTableResultTypeDef",
+ImportImageRequestRequestTypeDef = TypedDict(
+    "ImportImageRequestRequestTypeDef",
     {
-        "LocalGatewayRouteTable": LocalGatewayRouteTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Architecture": str,
+        "ClientData": ClientDataTypeDef,
+        "ClientToken": str,
+        "Description": str,
+        "DiskContainers": Sequence[ImageDiskContainerTypeDef],
+        "DryRun": bool,
+        "Encrypted": bool,
+        "Hypervisor": str,
+        "KmsKeyId": str,
+        "LicenseType": str,
+        "Platform": str,
+        "RoleName": str,
+        "LicenseSpecifications": Sequence[ImportImageLicenseConfigurationRequestTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "UsageOperation": str,
+        "BootMode": BootModeValuesType,
     },
+    total=False,
 )
 
-DescribeLocalGatewayRouteTablesResultTypeDef = TypedDict(
-    "DescribeLocalGatewayRouteTablesResultTypeDef",
+ImportSnapshotRequestRequestTypeDef = TypedDict(
+    "ImportSnapshotRequestRequestTypeDef",
     {
-        "LocalGatewayRouteTables": List[LocalGatewayRouteTableTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ClientData": ClientDataTypeDef,
+        "ClientToken": str,
+        "Description": str,
+        "DiskContainer": SnapshotDiskContainerTypeDef,
+        "DryRun": bool,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "RoleName": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
+    total=False,
 )
 
 _RequiredImportInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredImportInstanceRequestRequestTypeDef",
     {
         "Platform": Literal["Windows"],
     },
@@ -27071,110 +29038,14 @@
         "InterfaceType": str,
         "Ipv4Prefixes": List[InstanceIpv4PrefixTypeDef],
         "Ipv6Prefixes": List[InstanceIpv6PrefixTypeDef],
     },
     total=False,
 )
 
-FleetLaunchTemplateOverridesTypeDef = TypedDict(
-    "FleetLaunchTemplateOverridesTypeDef",
-    {
-        "InstanceType": InstanceTypeType,
-        "MaxPrice": str,
-        "SubnetId": str,
-        "AvailabilityZone": str,
-        "WeightedCapacity": float,
-        "Priority": float,
-        "Placement": PlacementResponseTypeDef,
-        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
-        "ImageId": str,
-    },
-    total=False,
-)
-
-LaunchTemplateOverridesOutputTypeDef = TypedDict(
-    "LaunchTemplateOverridesOutputTypeDef",
-    {
-        "InstanceType": InstanceTypeType,
-        "SpotPrice": str,
-        "SubnetId": str,
-        "AvailabilityZone": str,
-        "WeightedCapacity": float,
-        "Priority": float,
-        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
-    },
-    total=False,
-)
-
-SpotFleetLaunchSpecificationOutputTypeDef = TypedDict(
-    "SpotFleetLaunchSpecificationOutputTypeDef",
-    {
-        "SecurityGroups": List[GroupIdentifierTypeDef],
-        "AddressingType": str,
-        "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
-        "EbsOptimized": bool,
-        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
-        "ImageId": str,
-        "InstanceType": InstanceTypeType,
-        "KernelId": str,
-        "KeyName": str,
-        "Monitoring": SpotFleetMonitoringTypeDef,
-        "NetworkInterfaces": List[InstanceNetworkInterfaceSpecificationOutputTypeDef],
-        "Placement": SpotPlacementTypeDef,
-        "RamdiskId": str,
-        "SpotPrice": str,
-        "SubnetId": str,
-        "UserData": str,
-        "WeightedCapacity": float,
-        "TagSpecifications": List[SpotFleetTagSpecificationOutputTypeDef],
-        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
-    },
-    total=False,
-)
-
-LaunchTemplateOverridesTypeDef = TypedDict(
-    "LaunchTemplateOverridesTypeDef",
-    {
-        "InstanceType": InstanceTypeType,
-        "SpotPrice": str,
-        "SubnetId": str,
-        "AvailabilityZone": str,
-        "WeightedCapacity": float,
-        "Priority": float,
-        "InstanceRequirements": InstanceRequirementsTypeDef,
-    },
-    total=False,
-)
-
-SpotFleetLaunchSpecificationTypeDef = TypedDict(
-    "SpotFleetLaunchSpecificationTypeDef",
-    {
-        "SecurityGroups": Sequence[GroupIdentifierTypeDef],
-        "AddressingType": str,
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
-        "EbsOptimized": bool,
-        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
-        "ImageId": str,
-        "InstanceType": InstanceTypeType,
-        "KernelId": str,
-        "KeyName": str,
-        "Monitoring": SpotFleetMonitoringTypeDef,
-        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationTypeDef],
-        "Placement": SpotPlacementTypeDef,
-        "RamdiskId": str,
-        "SpotPrice": str,
-        "SubnetId": str,
-        "UserData": str,
-        "WeightedCapacity": float,
-        "TagSpecifications": Sequence[SpotFleetTagSpecificationTypeDef],
-        "InstanceRequirements": InstanceRequirementsTypeDef,
-    },
-    total=False,
-)
-
 FleetLaunchTemplateOverridesRequestTypeDef = TypedDict(
     "FleetLaunchTemplateOverridesRequestTypeDef",
     {
         "InstanceType": InstanceTypeType,
         "MaxPrice": str,
         "SubnetId": str,
         "AvailabilityZone": str,
@@ -27244,14 +29115,70 @@
         "ArchitectureTypes": Sequence[ArchitectureTypeType],
         "VirtualizationTypes": Sequence[VirtualizationTypeType],
         "InstanceRequirements": InstanceRequirementsRequestTypeDef,
     },
     total=False,
 )
 
+FleetLaunchTemplateOverridesTypeDef = TypedDict(
+    "FleetLaunchTemplateOverridesTypeDef",
+    {
+        "InstanceType": InstanceTypeType,
+        "MaxPrice": str,
+        "SubnetId": str,
+        "AvailabilityZone": str,
+        "WeightedCapacity": float,
+        "Priority": float,
+        "Placement": PlacementResponseTypeDef,
+        "InstanceRequirements": InstanceRequirementsTypeDef,
+        "ImageId": str,
+    },
+    total=False,
+)
+
+LaunchTemplateOverridesTypeDef = TypedDict(
+    "LaunchTemplateOverridesTypeDef",
+    {
+        "InstanceType": InstanceTypeType,
+        "SpotPrice": str,
+        "SubnetId": str,
+        "AvailabilityZone": str,
+        "WeightedCapacity": float,
+        "Priority": float,
+        "InstanceRequirements": InstanceRequirementsTypeDef,
+    },
+    total=False,
+)
+
+SpotFleetLaunchSpecificationTypeDef = TypedDict(
+    "SpotFleetLaunchSpecificationTypeDef",
+    {
+        "SecurityGroups": List[GroupIdentifierTypeDef],
+        "AddressingType": str,
+        "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
+        "EbsOptimized": bool,
+        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
+        "ImageId": str,
+        "InstanceType": InstanceTypeType,
+        "KernelId": str,
+        "KeyName": str,
+        "Monitoring": SpotFleetMonitoringTypeDef,
+        "NetworkInterfaces": List[InstanceNetworkInterfaceSpecificationTypeDef],
+        "Placement": SpotPlacementTypeDef,
+        "RamdiskId": str,
+        "SpotPrice": str,
+        "SubnetId": str,
+        "UserData": str,
+        "WeightedCapacity": float,
+        "TagSpecifications": List[SpotFleetTagSpecificationTypeDef],
+        "InstanceRequirements": InstanceRequirementsTypeDef,
+    },
+    total=False,
+)
+
 StartInstancesResultTypeDef = TypedDict(
     "StartInstancesResultTypeDef",
     {
         "StartingInstances": List[InstanceStateChangeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -27282,47 +29209,44 @@
         "InstanceState": InstanceStateTypeDef,
         "InstanceStatus": InstanceStatusSummaryTypeDef,
         "SystemStatus": InstanceStatusSummaryTypeDef,
     },
     total=False,
 )
 
-RevokeSecurityGroupEgressResultTypeDef = TypedDict(
-    "RevokeSecurityGroupEgressResultTypeDef",
-    {
-        "Return": bool,
-        "UnknownIpPermissions": List[IpPermissionOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RevokeSecurityGroupIngressResultTypeDef = TypedDict(
-    "RevokeSecurityGroupIngressResultTypeDef",
+_RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
+    "_RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef",
     {
-        "Return": bool,
-        "UnknownIpPermissions": List[IpPermissionOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "GroupId": str,
     },
 )
-
-SecurityGroupTypeDef = TypedDict(
-    "SecurityGroupTypeDef",
+_OptionalAuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
+    "_OptionalAuthorizeSecurityGroupEgressRequestRequestTypeDef",
     {
-        "Description": str,
-        "GroupName": str,
-        "IpPermissions": List[IpPermissionOutputTypeDef],
-        "OwnerId": str,
-        "GroupId": str,
-        "IpPermissionsEgress": List[IpPermissionOutputTypeDef],
-        "Tags": List[TagTypeDef],
-        "VpcId": str,
+        "DryRun": bool,
+        "IpPermissions": Sequence[IpPermissionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "CidrIp": str,
+        "FromPort": int,
+        "IpProtocol": str,
+        "ToPort": int,
+        "SourceSecurityGroupName": str,
+        "SourceSecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+
+class AuthorizeSecurityGroupEgressRequestRequestTypeDef(
+    _RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef,
+    _OptionalAuthorizeSecurityGroupEgressRequestRequestTypeDef,
+):
+    pass
+
+
 AuthorizeSecurityGroupEgressRequestSecurityGroupAuthorizeEgressTypeDef = TypedDict(
     "AuthorizeSecurityGroupEgressRequestSecurityGroupAuthorizeEgressTypeDef",
     {
         "DryRun": bool,
         "IpPermissions": Sequence[IpPermissionTypeDef],
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "CidrIp": str,
@@ -27331,14 +29255,32 @@
         "ToPort": int,
         "SourceSecurityGroupName": str,
         "SourceSecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+AuthorizeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
+    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
+    {
+        "CidrIp": str,
+        "FromPort": int,
+        "GroupId": str,
+        "GroupName": str,
+        "IpPermissions": Sequence[IpPermissionTypeDef],
+        "IpProtocol": str,
+        "SourceSecurityGroupName": str,
+        "SourceSecurityGroupOwnerId": str,
+        "ToPort": int,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
 AuthorizeSecurityGroupIngressRequestSecurityGroupAuthorizeIngressTypeDef = TypedDict(
     "AuthorizeSecurityGroupIngressRequestSecurityGroupAuthorizeIngressTypeDef",
     {
         "CidrIp": str,
         "FromPort": int,
         "GroupName": str,
         "IpPermissions": Sequence[IpPermissionTypeDef],
@@ -27348,15 +29290,44 @@
         "ToPort": int,
         "DryRun": bool,
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
     total=False,
 )
 
-IpPermissionUnionTypeDef = Union[IpPermissionTypeDef, IpPermissionOutputTypeDef]
+_RequiredRevokeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
+    "_RequiredRevokeSecurityGroupEgressRequestRequestTypeDef",
+    {
+        "GroupId": str,
+    },
+)
+_OptionalRevokeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
+    "_OptionalRevokeSecurityGroupEgressRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "IpPermissions": Sequence[IpPermissionTypeDef],
+        "SecurityGroupRuleIds": Sequence[str],
+        "CidrIp": str,
+        "FromPort": int,
+        "IpProtocol": str,
+        "ToPort": int,
+        "SourceSecurityGroupName": str,
+        "SourceSecurityGroupOwnerId": str,
+    },
+    total=False,
+)
+
+
+class RevokeSecurityGroupEgressRequestRequestTypeDef(
+    _RequiredRevokeSecurityGroupEgressRequestRequestTypeDef,
+    _OptionalRevokeSecurityGroupEgressRequestRequestTypeDef,
+):
+    pass
+
+
 RevokeSecurityGroupEgressRequestSecurityGroupRevokeEgressTypeDef = TypedDict(
     "RevokeSecurityGroupEgressRequestSecurityGroupRevokeEgressTypeDef",
     {
         "DryRun": bool,
         "IpPermissions": Sequence[IpPermissionTypeDef],
         "SecurityGroupRuleIds": Sequence[str],
         "CidrIp": str,
@@ -27365,14 +29336,41 @@
         "ToPort": int,
         "SourceSecurityGroupName": str,
         "SourceSecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+RevokeSecurityGroupEgressResultTypeDef = TypedDict(
+    "RevokeSecurityGroupEgressResultTypeDef",
+    {
+        "Return": bool,
+        "UnknownIpPermissions": List[IpPermissionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RevokeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
+    "RevokeSecurityGroupIngressRequestRequestTypeDef",
+    {
+        "CidrIp": str,
+        "FromPort": int,
+        "GroupId": str,
+        "GroupName": str,
+        "IpPermissions": Sequence[IpPermissionTypeDef],
+        "IpProtocol": str,
+        "SourceSecurityGroupName": str,
+        "SourceSecurityGroupOwnerId": str,
+        "ToPort": int,
+        "DryRun": bool,
+        "SecurityGroupRuleIds": Sequence[str],
+    },
+    total=False,
+)
+
 RevokeSecurityGroupIngressRequestSecurityGroupRevokeIngressTypeDef = TypedDict(
     "RevokeSecurityGroupIngressRequestSecurityGroupRevokeIngressTypeDef",
     {
         "CidrIp": str,
         "FromPort": int,
         "GroupName": str,
         "IpPermissions": Sequence[IpPermissionTypeDef],
@@ -27382,14 +29380,77 @@
         "ToPort": int,
         "DryRun": bool,
         "SecurityGroupRuleIds": Sequence[str],
     },
     total=False,
 )
 
+RevokeSecurityGroupIngressResultTypeDef = TypedDict(
+    "RevokeSecurityGroupIngressResultTypeDef",
+    {
+        "Return": bool,
+        "UnknownIpPermissions": List[IpPermissionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SecurityGroupTypeDef = TypedDict(
+    "SecurityGroupTypeDef",
+    {
+        "Description": str,
+        "GroupName": str,
+        "IpPermissions": List[IpPermissionTypeDef],
+        "OwnerId": str,
+        "GroupId": str,
+        "IpPermissionsEgress": List[IpPermissionTypeDef],
+        "Tags": List[TagTypeDef],
+        "VpcId": str,
+    },
+    total=False,
+)
+
+UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef = TypedDict(
+    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "GroupId": str,
+        "GroupName": str,
+        "IpPermissions": Sequence[IpPermissionTypeDef],
+        "SecurityGroupRuleDescriptions": Sequence[SecurityGroupRuleDescriptionTypeDef],
+    },
+    total=False,
+)
+
+UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef = TypedDict(
+    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "GroupId": str,
+        "GroupName": str,
+        "IpPermissions": Sequence[IpPermissionTypeDef],
+        "SecurityGroupRuleDescriptions": Sequence[SecurityGroupRuleDescriptionTypeDef],
+    },
+    total=False,
+)
+
+SecurityGroupVpcAddressTypeDef = TypedDict(
+    "SecurityGroupVpcAddressTypeDef",
+    {
+        "Description": str,
+        "GroupName": str,
+        "IpPermissions": List[IpPermissionVpcAddressTypeDef],
+        "OwnerId": str,
+        "GroupId": str,
+        "IpPermissionsEgress": List[IpPermissionVpcAddressTypeDef],
+        "Tags": List[TagTypeDef],
+        "VpcId": str,
+    },
+    total=False,
+)
+
 StaleSecurityGroupTypeDef = TypedDict(
     "StaleSecurityGroupTypeDef",
     {
         "Description": str,
         "GroupId": str,
         "GroupName": str,
         "StaleIpPermissions": List[StaleIpPermissionTypeDef],
@@ -27597,15 +29658,15 @@
         "CapacityReservationSpecification": (
             LaunchTemplateCapacityReservationSpecificationResponseTypeDef
         ),
         "LicenseSpecifications": List[LaunchTemplateLicenseConfigurationTypeDef],
         "HibernationOptions": LaunchTemplateHibernationOptionsTypeDef,
         "MetadataOptions": LaunchTemplateInstanceMetadataOptionsTypeDef,
         "EnclaveOptions": LaunchTemplateEnclaveOptionsTypeDef,
-        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
+        "InstanceRequirements": InstanceRequirementsTypeDef,
         "PrivateDnsNameOptions": LaunchTemplatePrivateDnsNameOptionsTypeDef,
         "MaintenanceOptions": LaunchTemplateInstanceMaintenanceOptionsTypeDef,
         "DisableApiStop": bool,
     },
     total=False,
 )
 
@@ -27719,14 +29780,45 @@
     "ModifyVerifiedAccessTrustProviderResultTypeDef",
     {
         "VerifiedAccessTrustProvider": VerifiedAccessTrustProviderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateNetworkInsightsPathRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNetworkInsightsPathRequestRequestTypeDef",
+    {
+        "Source": str,
+        "Protocol": ProtocolType,
+        "ClientToken": str,
+    },
+)
+_OptionalCreateNetworkInsightsPathRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNetworkInsightsPathRequestRequestTypeDef",
+    {
+        "SourceIp": str,
+        "DestinationIp": str,
+        "Destination": str,
+        "DestinationPort": int,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "FilterAtSource": PathRequestFilterTypeDef,
+        "FilterAtDestination": PathRequestFilterTypeDef,
+    },
+    total=False,
+)
+
+
+class CreateNetworkInsightsPathRequestRequestTypeDef(
+    _RequiredCreateNetworkInsightsPathRequestRequestTypeDef,
+    _OptionalCreateNetworkInsightsPathRequestRequestTypeDef,
+):
+    pass
+
+
 AccessScopePathRequestTypeDef = TypedDict(
     "AccessScopePathRequestTypeDef",
     {
         "Source": PathStatementRequestTypeDef,
         "Destination": PathStatementRequestTypeDef,
         "ThroughResources": Sequence[ThroughResourcesStatementRequestTypeDef],
     },
@@ -27816,29 +29908,14 @@
     {
         "SecurityGroupRules": List[SecurityGroupRuleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BundleTaskTypeDef = TypedDict(
-    "BundleTaskTypeDef",
-    {
-        "BundleId": str,
-        "BundleTaskError": BundleTaskErrorTypeDef,
-        "InstanceId": str,
-        "Progress": str,
-        "StartTime": datetime,
-        "State": BundleTaskStateType,
-        "Storage": StorageOutputTypeDef,
-        "UpdateTime": datetime,
-    },
-    total=False,
-)
-
 DescribeScheduledInstanceAvailabilityResultTypeDef = TypedDict(
     "DescribeScheduledInstanceAvailabilityResultTypeDef",
     {
         "NextToken": str,
         "ScheduledInstanceAvailabilitySet": List[ScheduledInstanceAvailabilityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -28148,23 +30225,14 @@
         "TargetConfigurationValueRollup": ReservationValueTypeDef,
         "TargetConfigurationValueSet": List[TargetReservationValueTypeDef],
         "ValidationFailureReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoadBalancersConfigOutputTypeDef = TypedDict(
-    "LoadBalancersConfigOutputTypeDef",
-    {
-        "ClassicLoadBalancersConfig": ClassicLoadBalancersConfigOutputTypeDef,
-        "TargetGroupsConfig": TargetGroupsConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 LoadBalancersConfigTypeDef = TypedDict(
     "LoadBalancersConfigTypeDef",
     {
         "ClassicLoadBalancersConfig": ClassicLoadBalancersConfigTypeDef,
         "TargetGroupsConfig": TargetGroupsConfigTypeDef,
     },
     total=False,
@@ -28758,14 +30826,39 @@
         "Status": VpcPeeringConnectionStateReasonTypeDef,
         "Tags": List[TagTypeDef],
         "VpcPeeringConnectionId": str,
     },
     total=False,
 )
 
+CreateLocalGatewayRouteTableResultTypeDef = TypedDict(
+    "CreateLocalGatewayRouteTableResultTypeDef",
+    {
+        "LocalGatewayRouteTable": LocalGatewayRouteTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteLocalGatewayRouteTableResultTypeDef = TypedDict(
+    "DeleteLocalGatewayRouteTableResultTypeDef",
+    {
+        "LocalGatewayRouteTable": LocalGatewayRouteTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLocalGatewayRouteTablesResultTypeDef = TypedDict(
+    "DescribeLocalGatewayRouteTablesResultTypeDef",
+    {
+        "LocalGatewayRouteTables": List[LocalGatewayRouteTableTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AssociateInstanceEventWindowResultTypeDef = TypedDict(
     "AssociateInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindow": InstanceEventWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -28799,2101 +30892,14 @@
     "ModifyInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindow": InstanceEventWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAcceptAddressTransferRequestRequestTypeDef = TypedDict(
-    "_RequiredAcceptAddressTransferRequestRequestTypeDef",
-    {
-        "Address": str,
-    },
-)
-_OptionalAcceptAddressTransferRequestRequestTypeDef = TypedDict(
-    "_OptionalAcceptAddressTransferRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class AcceptAddressTransferRequestRequestTypeDef(
-    _RequiredAcceptAddressTransferRequestRequestTypeDef,
-    _OptionalAcceptAddressTransferRequestRequestTypeDef,
-):
-    pass
-
-
-AllocateAddressRequestRequestTypeDef = TypedDict(
-    "AllocateAddressRequestRequestTypeDef",
-    {
-        "Domain": DomainTypeType,
-        "Address": str,
-        "PublicIpv4Pool": str,
-        "NetworkBorderGroup": str,
-        "CustomerOwnedIpv4Pool": str,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-_RequiredAllocateHostsRequestRequestTypeDef = TypedDict(
-    "_RequiredAllocateHostsRequestRequestTypeDef",
-    {
-        "AvailabilityZone": str,
-    },
-)
-_OptionalAllocateHostsRequestRequestTypeDef = TypedDict(
-    "_OptionalAllocateHostsRequestRequestTypeDef",
-    {
-        "AutoPlacement": AutoPlacementType,
-        "ClientToken": str,
-        "InstanceType": str,
-        "InstanceFamily": str,
-        "Quantity": int,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "HostRecovery": HostRecoveryType,
-        "OutpostArn": str,
-        "HostMaintenance": HostMaintenanceType,
-        "AssetIds": Sequence[str],
-    },
-    total=False,
-)
-
-
-class AllocateHostsRequestRequestTypeDef(
-    _RequiredAllocateHostsRequestRequestTypeDef, _OptionalAllocateHostsRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredAssociateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateIpamResourceDiscoveryRequestRequestTypeDef",
-    {
-        "IpamId": str,
-        "IpamResourceDiscoveryId": str,
-    },
-)
-_OptionalAssociateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateIpamResourceDiscoveryRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class AssociateIpamResourceDiscoveryRequestRequestTypeDef(
-    _RequiredAssociateIpamResourceDiscoveryRequestRequestTypeDef,
-    _OptionalAssociateIpamResourceDiscoveryRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCopySnapshotRequestRequestTypeDef = TypedDict(
-    "_RequiredCopySnapshotRequestRequestTypeDef",
-    {
-        "SourceRegion": str,
-        "SourceSnapshotId": str,
-    },
-)
-_OptionalCopySnapshotRequestRequestTypeDef = TypedDict(
-    "_OptionalCopySnapshotRequestRequestTypeDef",
-    {
-        "Description": str,
-        "DestinationOutpostArn": str,
-        "DestinationRegion": str,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "PresignedUrl": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CopySnapshotRequestRequestTypeDef(
-    _RequiredCopySnapshotRequestRequestTypeDef, _OptionalCopySnapshotRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateCapacityReservationFleetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCapacityReservationFleetRequestRequestTypeDef",
-    {
-        "InstanceTypeSpecifications": Sequence[ReservationFleetInstanceSpecificationTypeDef],
-        "TotalTargetCapacity": int,
-    },
-)
-_OptionalCreateCapacityReservationFleetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCapacityReservationFleetRequestRequestTypeDef",
-    {
-        "AllocationStrategy": str,
-        "ClientToken": str,
-        "Tenancy": Literal["default"],
-        "EndDate": TimestampTypeDef,
-        "InstanceMatchCriteria": Literal["open"],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateCapacityReservationFleetRequestRequestTypeDef(
-    _RequiredCreateCapacityReservationFleetRequestRequestTypeDef,
-    _OptionalCreateCapacityReservationFleetRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateCapacityReservationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCapacityReservationRequestRequestTypeDef",
-    {
-        "InstanceType": str,
-        "InstancePlatform": CapacityReservationInstancePlatformType,
-        "InstanceCount": int,
-    },
-)
-_OptionalCreateCapacityReservationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCapacityReservationRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "AvailabilityZone": str,
-        "AvailabilityZoneId": str,
-        "Tenancy": CapacityReservationTenancyType,
-        "EbsOptimized": bool,
-        "EphemeralStorage": bool,
-        "EndDate": TimestampTypeDef,
-        "EndDateType": EndDateTypeType,
-        "InstanceMatchCriteria": InstanceMatchCriteriaType,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "OutpostArn": str,
-        "PlacementGroupArn": str,
-    },
-    total=False,
-)
-
-
-class CreateCapacityReservationRequestRequestTypeDef(
-    _RequiredCreateCapacityReservationRequestRequestTypeDef,
-    _OptionalCreateCapacityReservationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateCarrierGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCarrierGatewayRequestRequestTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateCarrierGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCarrierGatewayRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateCarrierGatewayRequestRequestTypeDef(
-    _RequiredCreateCarrierGatewayRequestRequestTypeDef,
-    _OptionalCreateCarrierGatewayRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateClientVpnEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateClientVpnEndpointRequestRequestTypeDef",
-    {
-        "ClientCidrBlock": str,
-        "ServerCertificateArn": str,
-        "AuthenticationOptions": Sequence[ClientVpnAuthenticationRequestTypeDef],
-        "ConnectionLogOptions": ConnectionLogOptionsTypeDef,
-    },
-)
-_OptionalCreateClientVpnEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateClientVpnEndpointRequestRequestTypeDef",
-    {
-        "DnsServers": Sequence[str],
-        "TransportProtocol": TransportProtocolType,
-        "VpnPort": int,
-        "Description": str,
-        "SplitTunnel": bool,
-        "DryRun": bool,
-        "ClientToken": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "SecurityGroupIds": Sequence[str],
-        "VpcId": str,
-        "SelfServicePortal": SelfServicePortalType,
-        "ClientConnectOptions": ClientConnectOptionsTypeDef,
-        "SessionTimeoutHours": int,
-        "ClientLoginBannerOptions": ClientLoginBannerOptionsTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateClientVpnEndpointRequestRequestTypeDef(
-    _RequiredCreateClientVpnEndpointRequestRequestTypeDef,
-    _OptionalCreateClientVpnEndpointRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateCoipPoolRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCoipPoolRequestRequestTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-    },
-)
-_OptionalCreateCoipPoolRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCoipPoolRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateCoipPoolRequestRequestTypeDef(
-    _RequiredCreateCoipPoolRequestRequestTypeDef, _OptionalCreateCoipPoolRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateCustomerGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCustomerGatewayRequestRequestTypeDef",
-    {
-        "Type": Literal["ipsec.1"],
-    },
-)
-_OptionalCreateCustomerGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCustomerGatewayRequestRequestTypeDef",
-    {
-        "BgpAsn": int,
-        "PublicIp": str,
-        "CertificateArn": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DeviceName": str,
-        "IpAddress": str,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateCustomerGatewayRequestRequestTypeDef(
-    _RequiredCreateCustomerGatewayRequestRequestTypeDef,
-    _OptionalCreateCustomerGatewayRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateDhcpOptionsRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDhcpOptionsRequestRequestTypeDef",
-    {
-        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
-    },
-)
-_OptionalCreateDhcpOptionsRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDhcpOptionsRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateDhcpOptionsRequestRequestTypeDef(
-    _RequiredCreateDhcpOptionsRequestRequestTypeDef, _OptionalCreateDhcpOptionsRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef = TypedDict(
-    "_RequiredCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
-    {
-        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
-    },
-)
-_OptionalCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef = TypedDict(
-    "_OptionalCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef(
-    _RequiredCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef,
-    _OptionalCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef,
-):
-    pass
-
-
-_RequiredCreateEgressOnlyInternetGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEgressOnlyInternetGatewayRequestRequestTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateEgressOnlyInternetGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEgressOnlyInternetGatewayRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateEgressOnlyInternetGatewayRequestRequestTypeDef(
-    _RequiredCreateEgressOnlyInternetGatewayRequestRequestTypeDef,
-    _OptionalCreateEgressOnlyInternetGatewayRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateFlowLogsRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFlowLogsRequestRequestTypeDef",
-    {
-        "ResourceIds": Sequence[str],
-        "ResourceType": FlowLogsResourceTypeType,
-    },
-)
-_OptionalCreateFlowLogsRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFlowLogsRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "ClientToken": str,
-        "DeliverLogsPermissionArn": str,
-        "DeliverCrossAccountRole": str,
-        "LogGroupName": str,
-        "TrafficType": TrafficTypeType,
-        "LogDestinationType": LogDestinationTypeType,
-        "LogDestination": str,
-        "LogFormat": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "MaxAggregationInterval": int,
-        "DestinationOptions": DestinationOptionsRequestTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateFlowLogsRequestRequestTypeDef(
-    _RequiredCreateFlowLogsRequestRequestTypeDef, _OptionalCreateFlowLogsRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateFpgaImageRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFpgaImageRequestRequestTypeDef",
-    {
-        "InputStorageLocation": StorageLocationTypeDef,
-    },
-)
-_OptionalCreateFpgaImageRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFpgaImageRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "LogsStorageLocation": StorageLocationTypeDef,
-        "Description": str,
-        "Name": str,
-        "ClientToken": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateFpgaImageRequestRequestTypeDef(
-    _RequiredCreateFpgaImageRequestRequestTypeDef, _OptionalCreateFpgaImageRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateImageRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateImageRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-        "Name": str,
-    },
-)
-_OptionalCreateImageRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateImageRequestRequestTypeDef",
-    {
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
-        "Description": str,
-        "DryRun": bool,
-        "NoReboot": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateImageRequestRequestTypeDef(
-    _RequiredCreateImageRequestRequestTypeDef, _OptionalCreateImageRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateInstanceConnectEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInstanceConnectEndpointRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-    },
-)
-_OptionalCreateInstanceConnectEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInstanceConnectEndpointRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "SecurityGroupIds": Sequence[str],
-        "PreserveClientIp": bool,
-        "ClientToken": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateInstanceConnectEndpointRequestRequestTypeDef(
-    _RequiredCreateInstanceConnectEndpointRequestRequestTypeDef,
-    _OptionalCreateInstanceConnectEndpointRequestRequestTypeDef,
-):
-    pass
-
-
-CreateInstanceEventWindowRequestRequestTypeDef = TypedDict(
-    "CreateInstanceEventWindowRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "Name": str,
-        "TimeRanges": Sequence[InstanceEventWindowTimeRangeRequestTypeDef],
-        "CronExpression": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateInstanceExportTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInstanceExportTaskRequestRequestTypeDef",
-    {
-        "ExportToS3Task": ExportToS3TaskSpecificationTypeDef,
-        "InstanceId": str,
-        "TargetEnvironment": ExportEnvironmentType,
-    },
-)
-_OptionalCreateInstanceExportTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInstanceExportTaskRequestRequestTypeDef",
-    {
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateInstanceExportTaskRequestRequestTypeDef(
-    _RequiredCreateInstanceExportTaskRequestRequestTypeDef,
-    _OptionalCreateInstanceExportTaskRequestRequestTypeDef,
-):
-    pass
-
-
-CreateInternetGatewayRequestRequestTypeDef = TypedDict(
-    "CreateInternetGatewayRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef = TypedDict(
-    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-_RequiredCreateIpamPoolRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIpamPoolRequestRequestTypeDef",
-    {
-        "IpamScopeId": str,
-        "AddressFamily": AddressFamilyType,
-    },
-)
-_OptionalCreateIpamPoolRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIpamPoolRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "Locale": str,
-        "SourceIpamPoolId": str,
-        "Description": str,
-        "AutoImport": bool,
-        "PubliclyAdvertisable": bool,
-        "AllocationMinNetmaskLength": int,
-        "AllocationMaxNetmaskLength": int,
-        "AllocationDefaultNetmaskLength": int,
-        "AllocationResourceTags": Sequence[RequestIpamResourceTagTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-        "AwsService": Literal["ec2"],
-        "PublicIpSource": IpamPoolPublicIpSourceType,
-    },
-    total=False,
-)
-
-
-class CreateIpamPoolRequestRequestTypeDef(
-    _RequiredCreateIpamPoolRequestRequestTypeDef, _OptionalCreateIpamPoolRequestRequestTypeDef
-):
-    pass
-
-
-CreateIpamRequestRequestTypeDef = TypedDict(
-    "CreateIpamRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "Description": str,
-        "OperatingRegions": Sequence[AddIpamOperatingRegionTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-CreateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
-    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "Description": str,
-        "OperatingRegions": Sequence[AddIpamOperatingRegionTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-_RequiredCreateIpamScopeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIpamScopeRequestRequestTypeDef",
-    {
-        "IpamId": str,
-    },
-)
-_OptionalCreateIpamScopeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIpamScopeRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateIpamScopeRequestRequestTypeDef(
-    _RequiredCreateIpamScopeRequestRequestTypeDef, _OptionalCreateIpamScopeRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateKeyPairRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyPairRequestRequestTypeDef",
-    {
-        "KeyName": str,
-    },
-)
-_OptionalCreateKeyPairRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyPairRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "KeyType": KeyTypeType,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "KeyFormat": KeyFormatType,
-    },
-    total=False,
-)
-
-
-class CreateKeyPairRequestRequestTypeDef(
-    _RequiredCreateKeyPairRequestRequestTypeDef, _OptionalCreateKeyPairRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef = TypedDict(
-    "_RequiredCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
-    {
-        "KeyName": str,
-    },
-)
-_OptionalCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef = TypedDict(
-    "_OptionalCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
-    {
-        "DryRun": bool,
-        "KeyType": KeyTypeType,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "KeyFormat": KeyFormatType,
-    },
-    total=False,
-)
-
-
-class CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef(
-    _RequiredCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef,
-    _OptionalCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef,
-):
-    pass
-
-
-_RequiredCreateLocalGatewayRouteTableRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLocalGatewayRouteTableRequestRequestTypeDef",
-    {
-        "LocalGatewayId": str,
-    },
-)
-_OptionalCreateLocalGatewayRouteTableRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLocalGatewayRouteTableRequestRequestTypeDef",
-    {
-        "Mode": LocalGatewayRouteTableModeType,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateLocalGatewayRouteTableRequestRequestTypeDef(
-    _RequiredCreateLocalGatewayRouteTableRequestRequestTypeDef,
-    _OptionalCreateLocalGatewayRouteTableRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-        "LocalGatewayVirtualInterfaceGroupId": str,
-    },
-)
-_OptionalCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef(
-    _RequiredCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef,
-    _OptionalCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-        "VpcId": str,
-    },
-)
-_OptionalCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef(
-    _RequiredCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef,
-    _OptionalCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateManagedPrefixListRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateManagedPrefixListRequestRequestTypeDef",
-    {
-        "PrefixListName": str,
-        "MaxEntries": int,
-        "AddressFamily": str,
-    },
-)
-_OptionalCreateManagedPrefixListRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateManagedPrefixListRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "Entries": Sequence[AddPrefixListEntryTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateManagedPrefixListRequestRequestTypeDef(
-    _RequiredCreateManagedPrefixListRequestRequestTypeDef,
-    _OptionalCreateManagedPrefixListRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateNatGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNatGatewayRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-    },
-)
-_OptionalCreateNatGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNatGatewayRequestRequestTypeDef",
-    {
-        "AllocationId": str,
-        "ClientToken": str,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ConnectivityType": ConnectivityTypeType,
-        "PrivateIpAddress": str,
-        "SecondaryAllocationIds": Sequence[str],
-        "SecondaryPrivateIpAddresses": Sequence[str],
-        "SecondaryPrivateIpAddressCount": int,
-    },
-    total=False,
-)
-
-
-class CreateNatGatewayRequestRequestTypeDef(
-    _RequiredCreateNatGatewayRequestRequestTypeDef, _OptionalCreateNatGatewayRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateNetworkAclRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNetworkAclRequestRequestTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateNetworkAclRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNetworkAclRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateNetworkAclRequestRequestTypeDef(
-    _RequiredCreateNetworkAclRequestRequestTypeDef, _OptionalCreateNetworkAclRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef = TypedDict(
-    "_RequiredCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef = TypedDict(
-    "_OptionalCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef(
-    _RequiredCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef,
-    _OptionalCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef,
-):
-    pass
-
-
-_RequiredCreateNetworkInsightsPathRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNetworkInsightsPathRequestRequestTypeDef",
-    {
-        "Source": str,
-        "Protocol": ProtocolType,
-        "ClientToken": str,
-    },
-)
-_OptionalCreateNetworkInsightsPathRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNetworkInsightsPathRequestRequestTypeDef",
-    {
-        "SourceIp": str,
-        "DestinationIp": str,
-        "Destination": str,
-        "DestinationPort": int,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "FilterAtSource": PathRequestFilterTypeDef,
-        "FilterAtDestination": PathRequestFilterTypeDef,
-    },
-    total=False,
-)
-
-
-class CreateNetworkInsightsPathRequestRequestTypeDef(
-    _RequiredCreateNetworkInsightsPathRequestRequestTypeDef,
-    _OptionalCreateNetworkInsightsPathRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateNetworkInterfaceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNetworkInterfaceRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-    },
-)
-_OptionalCreateNetworkInterfaceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNetworkInterfaceRequestRequestTypeDef",
-    {
-        "Description": str,
-        "DryRun": bool,
-        "Groups": Sequence[str],
-        "Ipv6AddressCount": int,
-        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
-        "PrivateIpAddress": str,
-        "PrivateIpAddresses": Sequence[PrivateIpAddressSpecificationTypeDef],
-        "SecondaryPrivateIpAddressCount": int,
-        "Ipv4Prefixes": Sequence[Ipv4PrefixSpecificationRequestTypeDef],
-        "Ipv4PrefixCount": int,
-        "Ipv6Prefixes": Sequence[Ipv6PrefixSpecificationRequestTypeDef],
-        "Ipv6PrefixCount": int,
-        "InterfaceType": NetworkInterfaceCreationTypeType,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateNetworkInterfaceRequestRequestTypeDef(
-    _RequiredCreateNetworkInterfaceRequestRequestTypeDef,
-    _OptionalCreateNetworkInterfaceRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef = TypedDict(
-    "_RequiredCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
-    {
-        "SubnetId": str,
-    },
-)
-_OptionalCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef = TypedDict(
-    "_OptionalCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
-    {
-        "Description": str,
-        "DryRun": bool,
-        "Groups": Sequence[str],
-        "Ipv6AddressCount": int,
-        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
-        "PrivateIpAddress": str,
-        "PrivateIpAddresses": Sequence[PrivateIpAddressSpecificationTypeDef],
-        "SecondaryPrivateIpAddressCount": int,
-        "Ipv4Prefixes": Sequence[Ipv4PrefixSpecificationRequestTypeDef],
-        "Ipv4PrefixCount": int,
-        "Ipv6Prefixes": Sequence[Ipv6PrefixSpecificationRequestTypeDef],
-        "Ipv6PrefixCount": int,
-        "InterfaceType": NetworkInterfaceCreationTypeType,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef(
-    _RequiredCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef,
-    _OptionalCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef,
-):
-    pass
-
-
-CreatePlacementGroupRequestRequestTypeDef = TypedDict(
-    "CreatePlacementGroupRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "GroupName": str,
-        "Strategy": PlacementStrategyType,
-        "PartitionCount": int,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "SpreadLevel": SpreadLevelType,
-    },
-    total=False,
-)
-
-CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef = TypedDict(
-    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
-    {
-        "DryRun": bool,
-        "GroupName": str,
-        "Strategy": PlacementStrategyType,
-        "PartitionCount": int,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "SpreadLevel": SpreadLevelType,
-    },
-    total=False,
-)
-
-CreatePublicIpv4PoolRequestRequestTypeDef = TypedDict(
-    "CreatePublicIpv4PoolRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateReplaceRootVolumeTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReplaceRootVolumeTaskRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalCreateReplaceRootVolumeTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReplaceRootVolumeTaskRequestRequestTypeDef",
-    {
-        "SnapshotId": str,
-        "ClientToken": str,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ImageId": str,
-        "DeleteReplacedRootVolume": bool,
-    },
-    total=False,
-)
-
-
-class CreateReplaceRootVolumeTaskRequestRequestTypeDef(
-    _RequiredCreateReplaceRootVolumeTaskRequestRequestTypeDef,
-    _OptionalCreateReplaceRootVolumeTaskRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateRestoreImageTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRestoreImageTaskRequestRequestTypeDef",
-    {
-        "Bucket": str,
-        "ObjectKey": str,
-    },
-)
-_OptionalCreateRestoreImageTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRestoreImageTaskRequestRequestTypeDef",
-    {
-        "Name": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateRestoreImageTaskRequestRequestTypeDef(
-    _RequiredCreateRestoreImageTaskRequestRequestTypeDef,
-    _OptionalCreateRestoreImageTaskRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateRouteTableRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRouteTableRequestRequestTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateRouteTableRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRouteTableRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateRouteTableRequestRequestTypeDef(
-    _RequiredCreateRouteTableRequestRequestTypeDef, _OptionalCreateRouteTableRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef = TypedDict(
-    "_RequiredCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef = TypedDict(
-    "_OptionalCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef(
-    _RequiredCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef,
-    _OptionalCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef,
-):
-    pass
-
-
-_RequiredCreateSecurityGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSecurityGroupRequestRequestTypeDef",
-    {
-        "Description": str,
-        "GroupName": str,
-    },
-)
-_OptionalCreateSecurityGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSecurityGroupRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateSecurityGroupRequestRequestTypeDef(
-    _RequiredCreateSecurityGroupRequestRequestTypeDef,
-    _OptionalCreateSecurityGroupRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef = TypedDict(
-    "_RequiredCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
-    {
-        "Description": str,
-        "GroupName": str,
-    },
-)
-_OptionalCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef = TypedDict(
-    "_OptionalCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
-    {
-        "VpcId": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef(
-    _RequiredCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef,
-    _OptionalCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef,
-):
-    pass
-
-
-_RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSnapshotRequestRequestTypeDef",
-    {
-        "VolumeId": str,
-    },
-)
-_OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSnapshotRequestRequestTypeDef",
-    {
-        "Description": str,
-        "OutpostArn": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateSnapshotRequestRequestTypeDef(
-    _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef = TypedDict(
-    "_RequiredCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
-    {
-        "VolumeId": str,
-    },
-)
-_OptionalCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef = TypedDict(
-    "_OptionalCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
-    {
-        "Description": str,
-        "OutpostArn": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef(
-    _RequiredCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef,
-    _OptionalCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef,
-):
-    pass
-
-
-_RequiredCreateSnapshotsRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSnapshotsRequestRequestTypeDef",
-    {
-        "InstanceSpecification": InstanceSpecificationTypeDef,
-    },
-)
-_OptionalCreateSnapshotsRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSnapshotsRequestRequestTypeDef",
-    {
-        "Description": str,
-        "OutpostArn": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "CopyTagsFromSource": Literal["volume"],
-    },
-    total=False,
-)
-
-
-class CreateSnapshotsRequestRequestTypeDef(
-    _RequiredCreateSnapshotsRequestRequestTypeDef, _OptionalCreateSnapshotsRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateSubnetCidrReservationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSubnetCidrReservationRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-        "Cidr": str,
-        "ReservationType": SubnetCidrReservationTypeType,
-    },
-)
-_OptionalCreateSubnetCidrReservationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSubnetCidrReservationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateSubnetCidrReservationRequestRequestTypeDef(
-    _RequiredCreateSubnetCidrReservationRequestRequestTypeDef,
-    _OptionalCreateSubnetCidrReservationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateSubnetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSubnetRequestRequestTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateSubnetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSubnetRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "AvailabilityZone": str,
-        "AvailabilityZoneId": str,
-        "CidrBlock": str,
-        "Ipv6CidrBlock": str,
-        "OutpostArn": str,
-        "DryRun": bool,
-        "Ipv6Native": bool,
-    },
-    total=False,
-)
-
-
-class CreateSubnetRequestRequestTypeDef(
-    _RequiredCreateSubnetRequestRequestTypeDef, _OptionalCreateSubnetRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateSubnetRequestServiceResourceCreateSubnetTypeDef = TypedDict(
-    "_RequiredCreateSubnetRequestServiceResourceCreateSubnetTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateSubnetRequestServiceResourceCreateSubnetTypeDef = TypedDict(
-    "_OptionalCreateSubnetRequestServiceResourceCreateSubnetTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "AvailabilityZone": str,
-        "AvailabilityZoneId": str,
-        "CidrBlock": str,
-        "Ipv6CidrBlock": str,
-        "OutpostArn": str,
-        "DryRun": bool,
-        "Ipv6Native": bool,
-    },
-    total=False,
-)
-
-
-class CreateSubnetRequestServiceResourceCreateSubnetTypeDef(
-    _RequiredCreateSubnetRequestServiceResourceCreateSubnetTypeDef,
-    _OptionalCreateSubnetRequestServiceResourceCreateSubnetTypeDef,
-):
-    pass
-
-
-CreateTrafficMirrorFilterRequestRequestTypeDef = TypedDict(
-    "CreateTrafficMirrorFilterRequestRequestTypeDef",
-    {
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-_RequiredCreateTrafficMirrorSessionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTrafficMirrorSessionRequestRequestTypeDef",
-    {
-        "NetworkInterfaceId": str,
-        "TrafficMirrorTargetId": str,
-        "TrafficMirrorFilterId": str,
-        "SessionNumber": int,
-    },
-)
-_OptionalCreateTrafficMirrorSessionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTrafficMirrorSessionRequestRequestTypeDef",
-    {
-        "PacketLength": int,
-        "VirtualNetworkId": int,
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateTrafficMirrorSessionRequestRequestTypeDef(
-    _RequiredCreateTrafficMirrorSessionRequestRequestTypeDef,
-    _OptionalCreateTrafficMirrorSessionRequestRequestTypeDef,
-):
-    pass
-
-
-CreateTrafficMirrorTargetRequestRequestTypeDef = TypedDict(
-    "CreateTrafficMirrorTargetRequestRequestTypeDef",
-    {
-        "NetworkInterfaceId": str,
-        "NetworkLoadBalancerArn": str,
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "ClientToken": str,
-        "GatewayLoadBalancerEndpointId": str,
-    },
-    total=False,
-)
-
-_RequiredCreateTransitGatewayConnectPeerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayConnectPeerRequestRequestTypeDef",
-    {
-        "TransitGatewayAttachmentId": str,
-        "PeerAddress": str,
-        "InsideCidrBlocks": Sequence[str],
-    },
-)
-_OptionalCreateTransitGatewayConnectPeerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayConnectPeerRequestRequestTypeDef",
-    {
-        "TransitGatewayAddress": str,
-        "BgpOptions": TransitGatewayConnectRequestBgpOptionsTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateTransitGatewayConnectPeerRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayConnectPeerRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayConnectPeerRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateTransitGatewayConnectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayConnectRequestRequestTypeDef",
-    {
-        "TransportTransitGatewayAttachmentId": str,
-        "Options": CreateTransitGatewayConnectRequestOptionsTypeDef,
-    },
-)
-_OptionalCreateTransitGatewayConnectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayConnectRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateTransitGatewayConnectRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayConnectRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayConnectRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateTransitGatewayMulticastDomainRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayMulticastDomainRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-    },
-)
-_OptionalCreateTransitGatewayMulticastDomainRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayMulticastDomainRequestRequestTypeDef",
-    {
-        "Options": CreateTransitGatewayMulticastDomainRequestOptionsTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateTransitGatewayMulticastDomainRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayMulticastDomainRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayMulticastDomainRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "PeerTransitGatewayId": str,
-        "PeerAccountId": str,
-        "PeerRegion": str,
-    },
-)
-_OptionalCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
-    {
-        "Options": CreateTransitGatewayPeeringAttachmentRequestOptionsTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateTransitGatewayPolicyTableRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayPolicyTableRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-    },
-)
-_OptionalCreateTransitGatewayPolicyTableRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayPolicyTableRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateTransitGatewayPolicyTableRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayPolicyTableRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayPolicyTableRequestRequestTypeDef,
-):
-    pass
-
-
-CreateTransitGatewayRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Options": TransitGatewayRequestOptionsTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-_RequiredCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
-    {
-        "TransitGatewayRouteTableId": str,
-        "PeeringAttachmentId": str,
-    },
-)
-_OptionalCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayRouteTableRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-    },
-)
-_OptionalCreateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayRouteTableRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateTransitGatewayRouteTableRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayRouteTableRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayRouteTableRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateTransitGatewayVpcAttachmentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "VpcId": str,
-        "SubnetIds": Sequence[str],
-    },
-)
-_OptionalCreateTransitGatewayVpcAttachmentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
-    {
-        "Options": CreateTransitGatewayVpcAttachmentRequestOptionsTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateTransitGatewayVpcAttachmentRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayVpcAttachmentRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayVpcAttachmentRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateVerifiedAccessEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVerifiedAccessEndpointRequestRequestTypeDef",
-    {
-        "VerifiedAccessGroupId": str,
-        "EndpointType": VerifiedAccessEndpointTypeType,
-        "AttachmentType": Literal["vpc"],
-        "DomainCertificateArn": str,
-        "ApplicationDomain": str,
-        "EndpointDomainPrefix": str,
-    },
-)
-_OptionalCreateVerifiedAccessEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVerifiedAccessEndpointRequestRequestTypeDef",
-    {
-        "SecurityGroupIds": Sequence[str],
-        "LoadBalancerOptions": CreateVerifiedAccessEndpointLoadBalancerOptionsTypeDef,
-        "NetworkInterfaceOptions": CreateVerifiedAccessEndpointEniOptionsTypeDef,
-        "Description": str,
-        "PolicyDocument": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateVerifiedAccessEndpointRequestRequestTypeDef(
-    _RequiredCreateVerifiedAccessEndpointRequestRequestTypeDef,
-    _OptionalCreateVerifiedAccessEndpointRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateVerifiedAccessGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVerifiedAccessGroupRequestRequestTypeDef",
-    {
-        "VerifiedAccessInstanceId": str,
-    },
-)
-_OptionalCreateVerifiedAccessGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVerifiedAccessGroupRequestRequestTypeDef",
-    {
-        "Description": str,
-        "PolicyDocument": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateVerifiedAccessGroupRequestRequestTypeDef(
-    _RequiredCreateVerifiedAccessGroupRequestRequestTypeDef,
-    _OptionalCreateVerifiedAccessGroupRequestRequestTypeDef,
-):
-    pass
-
-
-CreateVerifiedAccessInstanceRequestRequestTypeDef = TypedDict(
-    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
-    {
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-_RequiredCreateVerifiedAccessTrustProviderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVerifiedAccessTrustProviderRequestRequestTypeDef",
-    {
-        "TrustProviderType": TrustProviderTypeType,
-        "PolicyReferenceName": str,
-    },
-)
-_OptionalCreateVerifiedAccessTrustProviderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVerifiedAccessTrustProviderRequestRequestTypeDef",
-    {
-        "UserTrustProviderType": UserTrustProviderTypeType,
-        "DeviceTrustProviderType": DeviceTrustProviderTypeType,
-        "OidcOptions": CreateVerifiedAccessTrustProviderOidcOptionsTypeDef,
-        "DeviceOptions": CreateVerifiedAccessTrustProviderDeviceOptionsTypeDef,
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateVerifiedAccessTrustProviderRequestRequestTypeDef(
-    _RequiredCreateVerifiedAccessTrustProviderRequestRequestTypeDef,
-    _OptionalCreateVerifiedAccessTrustProviderRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVolumeRequestRequestTypeDef",
-    {
-        "AvailabilityZone": str,
-    },
-)
-_OptionalCreateVolumeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVolumeRequestRequestTypeDef",
-    {
-        "Encrypted": bool,
-        "Iops": int,
-        "KmsKeyId": str,
-        "OutpostArn": str,
-        "Size": int,
-        "SnapshotId": str,
-        "VolumeType": VolumeTypeType,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "MultiAttachEnabled": bool,
-        "Throughput": int,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateVolumeRequestRequestTypeDef(
-    _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredCreateVolumeRequestServiceResourceCreateVolumeTypeDef = TypedDict(
-    "_RequiredCreateVolumeRequestServiceResourceCreateVolumeTypeDef",
-    {
-        "AvailabilityZone": str,
-    },
-)
-_OptionalCreateVolumeRequestServiceResourceCreateVolumeTypeDef = TypedDict(
-    "_OptionalCreateVolumeRequestServiceResourceCreateVolumeTypeDef",
-    {
-        "Encrypted": bool,
-        "Iops": int,
-        "KmsKeyId": str,
-        "OutpostArn": str,
-        "Size": int,
-        "SnapshotId": str,
-        "VolumeType": VolumeTypeType,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "MultiAttachEnabled": bool,
-        "Throughput": int,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class CreateVolumeRequestServiceResourceCreateVolumeTypeDef(
-    _RequiredCreateVolumeRequestServiceResourceCreateVolumeTypeDef,
-    _OptionalCreateVolumeRequestServiceResourceCreateVolumeTypeDef,
-):
-    pass
-
-
-_RequiredCreateVpcEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVpcEndpointRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "ServiceName": str,
-    },
-)
-_OptionalCreateVpcEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVpcEndpointRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "VpcEndpointType": VpcEndpointTypeType,
-        "PolicyDocument": str,
-        "RouteTableIds": Sequence[str],
-        "SubnetIds": Sequence[str],
-        "SecurityGroupIds": Sequence[str],
-        "IpAddressType": IpAddressTypeType,
-        "DnsOptions": DnsOptionsSpecificationTypeDef,
-        "ClientToken": str,
-        "PrivateDnsEnabled": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateVpcEndpointRequestRequestTypeDef(
-    _RequiredCreateVpcEndpointRequestRequestTypeDef, _OptionalCreateVpcEndpointRequestRequestTypeDef
-):
-    pass
-
-
-CreateVpcEndpointServiceConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "AcceptanceRequired": bool,
-        "PrivateDnsName": str,
-        "NetworkLoadBalancerArns": Sequence[str],
-        "GatewayLoadBalancerArns": Sequence[str],
-        "SupportedIpAddressTypes": Sequence[str],
-        "ClientToken": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateVpcPeeringConnectionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVpcPeeringConnectionRequestRequestTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateVpcPeeringConnectionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVpcPeeringConnectionRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "PeerOwnerId": str,
-        "PeerVpcId": str,
-        "PeerRegion": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateVpcPeeringConnectionRequestRequestTypeDef(
-    _RequiredCreateVpcPeeringConnectionRequestRequestTypeDef,
-    _OptionalCreateVpcPeeringConnectionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef = TypedDict(
-    "_RequiredCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef = TypedDict(
-    "_OptionalCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
-    {
-        "DryRun": bool,
-        "PeerOwnerId": str,
-        "PeerVpcId": str,
-        "PeerRegion": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef(
-    _RequiredCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef,
-    _OptionalCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef,
-):
-    pass
-
-
-CreateVpcRequestRequestTypeDef = TypedDict(
-    "CreateVpcRequestRequestTypeDef",
-    {
-        "CidrBlock": str,
-        "AmazonProvidedIpv6CidrBlock": bool,
-        "Ipv6Pool": str,
-        "Ipv6CidrBlock": str,
-        "Ipv4IpamPoolId": str,
-        "Ipv4NetmaskLength": int,
-        "Ipv6IpamPoolId": str,
-        "Ipv6NetmaskLength": int,
-        "DryRun": bool,
-        "InstanceTenancy": TenancyType,
-        "Ipv6CidrBlockNetworkBorderGroup": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-CreateVpcRequestServiceResourceCreateVpcTypeDef = TypedDict(
-    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
-    {
-        "CidrBlock": str,
-        "AmazonProvidedIpv6CidrBlock": bool,
-        "Ipv6Pool": str,
-        "Ipv6CidrBlock": str,
-        "Ipv4IpamPoolId": str,
-        "Ipv4NetmaskLength": int,
-        "Ipv6IpamPoolId": str,
-        "Ipv6NetmaskLength": int,
-        "DryRun": bool,
-        "InstanceTenancy": TenancyType,
-        "Ipv6CidrBlockNetworkBorderGroup": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateVpnGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVpnGatewayRequestRequestTypeDef",
-    {
-        "Type": Literal["ipsec.1"],
-    },
-)
-_OptionalCreateVpnGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVpnGatewayRequestRequestTypeDef",
-    {
-        "AvailabilityZone": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "AmazonSideAsn": int,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-
-class CreateVpnGatewayRequestRequestTypeDef(
-    _RequiredCreateVpnGatewayRequestRequestTypeDef, _OptionalCreateVpnGatewayRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredExportImageRequestRequestTypeDef = TypedDict(
-    "_RequiredExportImageRequestRequestTypeDef",
-    {
-        "DiskImageFormat": DiskImageFormatType,
-        "ImageId": str,
-        "S3ExportLocation": ExportTaskS3LocationRequestTypeDef,
-    },
-)
-_OptionalExportImageRequestRequestTypeDef = TypedDict(
-    "_OptionalExportImageRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "Description": str,
-        "DryRun": bool,
-        "RoleName": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class ExportImageRequestRequestTypeDef(
-    _RequiredExportImageRequestRequestTypeDef, _OptionalExportImageRequestRequestTypeDef
-):
-    pass
-
-
-ImportImageRequestRequestTypeDef = TypedDict(
-    "ImportImageRequestRequestTypeDef",
-    {
-        "Architecture": str,
-        "ClientData": ClientDataTypeDef,
-        "ClientToken": str,
-        "Description": str,
-        "DiskContainers": Sequence[ImageDiskContainerTypeDef],
-        "DryRun": bool,
-        "Encrypted": bool,
-        "Hypervisor": str,
-        "KmsKeyId": str,
-        "LicenseType": str,
-        "Platform": str,
-        "RoleName": str,
-        "LicenseSpecifications": Sequence[ImportImageLicenseConfigurationRequestTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "UsageOperation": str,
-        "BootMode": BootModeValuesType,
-    },
-    total=False,
-)
-
-_RequiredImportKeyPairRequestRequestTypeDef = TypedDict(
-    "_RequiredImportKeyPairRequestRequestTypeDef",
-    {
-        "KeyName": str,
-        "PublicKeyMaterial": BlobTypeDef,
-    },
-)
-_OptionalImportKeyPairRequestRequestTypeDef = TypedDict(
-    "_OptionalImportKeyPairRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class ImportKeyPairRequestRequestTypeDef(
-    _RequiredImportKeyPairRequestRequestTypeDef, _OptionalImportKeyPairRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredImportKeyPairRequestServiceResourceImportKeyPairTypeDef = TypedDict(
-    "_RequiredImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
-    {
-        "KeyName": str,
-        "PublicKeyMaterial": BlobTypeDef,
-    },
-)
-_OptionalImportKeyPairRequestServiceResourceImportKeyPairTypeDef = TypedDict(
-    "_OptionalImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class ImportKeyPairRequestServiceResourceImportKeyPairTypeDef(
-    _RequiredImportKeyPairRequestServiceResourceImportKeyPairTypeDef,
-    _OptionalImportKeyPairRequestServiceResourceImportKeyPairTypeDef,
-):
-    pass
-
-
-ImportSnapshotRequestRequestTypeDef = TypedDict(
-    "ImportSnapshotRequestRequestTypeDef",
-    {
-        "ClientData": ClientDataTypeDef,
-        "ClientToken": str,
-        "Description": str,
-        "DiskContainer": SnapshotDiskContainerTypeDef,
-        "DryRun": bool,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "RoleName": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-_RequiredProvisionByoipCidrRequestRequestTypeDef = TypedDict(
-    "_RequiredProvisionByoipCidrRequestRequestTypeDef",
-    {
-        "Cidr": str,
-    },
-)
-_OptionalProvisionByoipCidrRequestRequestTypeDef = TypedDict(
-    "_OptionalProvisionByoipCidrRequestRequestTypeDef",
-    {
-        "CidrAuthorizationContext": CidrAuthorizationContextTypeDef,
-        "PubliclyAdvertisable": bool,
-        "Description": str,
-        "DryRun": bool,
-        "PoolTagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "MultiRegion": bool,
-    },
-    total=False,
-)
-
-
-class ProvisionByoipCidrRequestRequestTypeDef(
-    _RequiredProvisionByoipCidrRequestRequestTypeDef,
-    _OptionalProvisionByoipCidrRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredPurchaseHostReservationRequestRequestTypeDef = TypedDict(
-    "_RequiredPurchaseHostReservationRequestRequestTypeDef",
-    {
-        "HostIdSet": Sequence[str],
-        "OfferingId": str,
-    },
-)
-_OptionalPurchaseHostReservationRequestRequestTypeDef = TypedDict(
-    "_OptionalPurchaseHostReservationRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "CurrencyCode": Literal["USD"],
-        "LimitPrice": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class PurchaseHostReservationRequestRequestTypeDef(
-    _RequiredPurchaseHostReservationRequestRequestTypeDef,
-    _OptionalPurchaseHostReservationRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef = TypedDict(
-    "_RequiredStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
-    {
-        "NetworkInsightsAccessScopeId": str,
-        "ClientToken": str,
-    },
-)
-_OptionalStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef = TypedDict(
-    "_OptionalStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef(
-    _RequiredStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef,
-    _OptionalStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredStartNetworkInsightsAnalysisRequestRequestTypeDef = TypedDict(
-    "_RequiredStartNetworkInsightsAnalysisRequestRequestTypeDef",
-    {
-        "NetworkInsightsPathId": str,
-        "ClientToken": str,
-    },
-)
-_OptionalStartNetworkInsightsAnalysisRequestRequestTypeDef = TypedDict(
-    "_OptionalStartNetworkInsightsAnalysisRequestRequestTypeDef",
-    {
-        "AdditionalAccounts": Sequence[str],
-        "FilterInArns": Sequence[str],
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class StartNetworkInsightsAnalysisRequestRequestTypeDef(
-    _RequiredStartNetworkInsightsAnalysisRequestRequestTypeDef,
-    _OptionalStartNetworkInsightsAnalysisRequestRequestTypeDef,
-):
-    pass
-
-
 PathComponentTypeDef = TypedDict(
     "PathComponentTypeDef",
     {
         "SequenceNumber": int,
         "AclRule": AnalysisAclRuleTypeDef,
         "AttachedTo": AnalysisComponentTypeDef,
         "Component": AnalysisComponentTypeDef,
@@ -30996,14 +31002,133 @@
         "PrivateDnsNameOptions": LaunchTemplatePrivateDnsNameOptionsRequestTypeDef,
         "MaintenanceOptions": LaunchTemplateInstanceMaintenanceOptionsRequestTypeDef,
         "DisableApiStop": bool,
     },
     total=False,
 )
 
+_RequiredRunInstancesRequestRequestTypeDef = TypedDict(
+    "_RequiredRunInstancesRequestRequestTypeDef",
+    {
+        "MaxCount": int,
+        "MinCount": int,
+    },
+)
+_OptionalRunInstancesRequestRequestTypeDef = TypedDict(
+    "_OptionalRunInstancesRequestRequestTypeDef",
+    {
+        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "ImageId": str,
+        "InstanceType": InstanceTypeType,
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
+        "KernelId": str,
+        "KeyName": str,
+        "Monitoring": RunInstancesMonitoringEnabledTypeDef,
+        "Placement": PlacementTypeDef,
+        "RamdiskId": str,
+        "SecurityGroupIds": Sequence[str],
+        "SecurityGroups": Sequence[str],
+        "SubnetId": str,
+        "UserData": str,
+        "AdditionalInfo": str,
+        "ClientToken": str,
+        "DisableApiTermination": bool,
+        "DryRun": bool,
+        "EbsOptimized": bool,
+        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
+        "InstanceInitiatedShutdownBehavior": ShutdownBehaviorType,
+        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationTypeDef],
+        "PrivateIpAddress": str,
+        "ElasticGpuSpecification": Sequence[ElasticGpuSpecificationTypeDef],
+        "ElasticInferenceAccelerators": Sequence[ElasticInferenceAcceleratorTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
+        "InstanceMarketOptions": InstanceMarketOptionsRequestTypeDef,
+        "CreditSpecification": CreditSpecificationRequestTypeDef,
+        "CpuOptions": CpuOptionsRequestTypeDef,
+        "CapacityReservationSpecification": CapacityReservationSpecificationTypeDef,
+        "HibernationOptions": HibernationOptionsRequestTypeDef,
+        "LicenseSpecifications": Sequence[LicenseConfigurationRequestTypeDef],
+        "MetadataOptions": InstanceMetadataOptionsRequestTypeDef,
+        "EnclaveOptions": EnclaveOptionsRequestTypeDef,
+        "PrivateDnsNameOptions": PrivateDnsNameOptionsRequestTypeDef,
+        "MaintenanceOptions": InstanceMaintenanceOptionsRequestTypeDef,
+        "DisableApiStop": bool,
+    },
+    total=False,
+)
+
+
+class RunInstancesRequestRequestTypeDef(
+    _RequiredRunInstancesRequestRequestTypeDef, _OptionalRunInstancesRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredRunInstancesRequestServiceResourceCreateInstancesTypeDef = TypedDict(
+    "_RequiredRunInstancesRequestServiceResourceCreateInstancesTypeDef",
+    {
+        "MaxCount": int,
+        "MinCount": int,
+    },
+)
+_OptionalRunInstancesRequestServiceResourceCreateInstancesTypeDef = TypedDict(
+    "_OptionalRunInstancesRequestServiceResourceCreateInstancesTypeDef",
+    {
+        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "ImageId": str,
+        "InstanceType": InstanceTypeType,
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
+        "KernelId": str,
+        "KeyName": str,
+        "Monitoring": RunInstancesMonitoringEnabledTypeDef,
+        "Placement": PlacementTypeDef,
+        "RamdiskId": str,
+        "SecurityGroupIds": Sequence[str],
+        "SecurityGroups": Sequence[str],
+        "SubnetId": str,
+        "UserData": str,
+        "AdditionalInfo": str,
+        "ClientToken": str,
+        "DisableApiTermination": bool,
+        "DryRun": bool,
+        "EbsOptimized": bool,
+        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
+        "InstanceInitiatedShutdownBehavior": ShutdownBehaviorType,
+        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationServiceResourceTypeDef],
+        "PrivateIpAddress": str,
+        "ElasticGpuSpecification": Sequence[ElasticGpuSpecificationTypeDef],
+        "ElasticInferenceAccelerators": Sequence[ElasticInferenceAcceleratorTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
+        "InstanceMarketOptions": InstanceMarketOptionsRequestTypeDef,
+        "CreditSpecification": CreditSpecificationRequestTypeDef,
+        "CpuOptions": CpuOptionsRequestTypeDef,
+        "CapacityReservationSpecification": CapacityReservationSpecificationTypeDef,
+        "HibernationOptions": HibernationOptionsRequestTypeDef,
+        "LicenseSpecifications": Sequence[LicenseConfigurationRequestTypeDef],
+        "MetadataOptions": InstanceMetadataOptionsRequestTypeDef,
+        "EnclaveOptions": EnclaveOptionsRequestTypeDef,
+        "PrivateDnsNameOptions": PrivateDnsNameOptionsRequestTypeDef,
+        "MaintenanceOptions": InstanceMaintenanceOptionsRequestTypeDef,
+        "DisableApiStop": bool,
+    },
+    total=False,
+)
+
+
+class RunInstancesRequestServiceResourceCreateInstancesTypeDef(
+    _RequiredRunInstancesRequestServiceResourceCreateInstancesTypeDef,
+    _OptionalRunInstancesRequestServiceResourceCreateInstancesTypeDef,
+):
+    pass
+
+
 _RequiredRunInstancesRequestSubnetCreateInstancesTypeDef = TypedDict(
     "_RequiredRunInstancesRequestSubnetCreateInstancesTypeDef",
     {
         "MaxCount": int,
         "MinCount": int,
     },
 )
@@ -31026,15 +31151,15 @@
         "AdditionalInfo": str,
         "ClientToken": str,
         "DisableApiTermination": bool,
         "DryRun": bool,
         "EbsOptimized": bool,
         "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
         "InstanceInitiatedShutdownBehavior": ShutdownBehaviorType,
-        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationTypeDef],
+        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationSubnetTypeDef],
         "PrivateIpAddress": str,
         "ElasticGpuSpecification": Sequence[ElasticGpuSpecificationTypeDef],
         "ElasticInferenceAccelerators": Sequence[ElasticInferenceAcceleratorTypeDef],
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "InstanceMarketOptions": InstanceMarketOptionsRequestTypeDef,
         "CreditSpecification": CreditSpecificationRequestTypeDef,
@@ -31148,15 +31273,29 @@
 
 class BundleInstanceRequestRequestTypeDef(
     _RequiredBundleInstanceRequestRequestTypeDef, _OptionalBundleInstanceRequestRequestTypeDef
 ):
     pass
 
 
-StorageUnionTypeDef = Union[StorageTypeDef, StorageOutputTypeDef]
+BundleTaskTypeDef = TypedDict(
+    "BundleTaskTypeDef",
+    {
+        "BundleId": str,
+        "BundleTaskError": BundleTaskErrorTypeDef,
+        "InstanceId": str,
+        "Progress": str,
+        "StartTime": datetime,
+        "State": BundleTaskStateType,
+        "Storage": StorageTypeDef,
+        "UpdateTime": datetime,
+    },
+    total=False,
+)
+
 DescribeImagesResultTypeDef = TypedDict(
     "DescribeImagesResultTypeDef",
     {
         "Images": List[ImageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -31269,148 +31408,29 @@
         "ValidFrom": datetime,
         "ValidUntil": datetime,
         "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
     },
     total=False,
 )
 
-_RequiredRunInstancesRequestRequestTypeDef = TypedDict(
-    "_RequiredRunInstancesRequestRequestTypeDef",
-    {
-        "MaxCount": int,
-        "MinCount": int,
-    },
-)
-_OptionalRunInstancesRequestRequestTypeDef = TypedDict(
-    "_OptionalRunInstancesRequestRequestTypeDef",
-    {
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
-        "ImageId": str,
-        "InstanceType": InstanceTypeType,
-        "Ipv6AddressCount": int,
-        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
-        "KernelId": str,
-        "KeyName": str,
-        "Monitoring": RunInstancesMonitoringEnabledTypeDef,
-        "Placement": PlacementTypeDef,
-        "RamdiskId": str,
-        "SecurityGroupIds": Sequence[str],
-        "SecurityGroups": Sequence[str],
-        "SubnetId": str,
-        "UserData": str,
-        "AdditionalInfo": str,
-        "ClientToken": str,
-        "DisableApiTermination": bool,
-        "DryRun": bool,
-        "EbsOptimized": bool,
-        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
-        "InstanceInitiatedShutdownBehavior": ShutdownBehaviorType,
-        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef],
-        "PrivateIpAddress": str,
-        "ElasticGpuSpecification": Sequence[ElasticGpuSpecificationTypeDef],
-        "ElasticInferenceAccelerators": Sequence[ElasticInferenceAcceleratorTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "InstanceMarketOptions": InstanceMarketOptionsRequestTypeDef,
-        "CreditSpecification": CreditSpecificationRequestTypeDef,
-        "CpuOptions": CpuOptionsRequestTypeDef,
-        "CapacityReservationSpecification": CapacityReservationSpecificationTypeDef,
-        "HibernationOptions": HibernationOptionsRequestTypeDef,
-        "LicenseSpecifications": Sequence[LicenseConfigurationRequestTypeDef],
-        "MetadataOptions": InstanceMetadataOptionsRequestTypeDef,
-        "EnclaveOptions": EnclaveOptionsRequestTypeDef,
-        "PrivateDnsNameOptions": PrivateDnsNameOptionsRequestTypeDef,
-        "MaintenanceOptions": InstanceMaintenanceOptionsRequestTypeDef,
-        "DisableApiStop": bool,
-    },
-    total=False,
-)
-
-
-class RunInstancesRequestRequestTypeDef(
-    _RequiredRunInstancesRequestRequestTypeDef, _OptionalRunInstancesRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredRunInstancesRequestServiceResourceCreateInstancesTypeDef = TypedDict(
-    "_RequiredRunInstancesRequestServiceResourceCreateInstancesTypeDef",
-    {
-        "MaxCount": int,
-        "MinCount": int,
-    },
-)
-_OptionalRunInstancesRequestServiceResourceCreateInstancesTypeDef = TypedDict(
-    "_OptionalRunInstancesRequestServiceResourceCreateInstancesTypeDef",
-    {
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
-        "ImageId": str,
-        "InstanceType": InstanceTypeType,
-        "Ipv6AddressCount": int,
-        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
-        "KernelId": str,
-        "KeyName": str,
-        "Monitoring": RunInstancesMonitoringEnabledTypeDef,
-        "Placement": PlacementTypeDef,
-        "RamdiskId": str,
-        "SecurityGroupIds": Sequence[str],
-        "SecurityGroups": Sequence[str],
-        "SubnetId": str,
-        "UserData": str,
-        "AdditionalInfo": str,
-        "ClientToken": str,
-        "DisableApiTermination": bool,
-        "DryRun": bool,
-        "EbsOptimized": bool,
-        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
-        "InstanceInitiatedShutdownBehavior": ShutdownBehaviorType,
-        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef],
-        "PrivateIpAddress": str,
-        "ElasticGpuSpecification": Sequence[ElasticGpuSpecificationTypeDef],
-        "ElasticInferenceAccelerators": Sequence[ElasticInferenceAcceleratorTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "InstanceMarketOptions": InstanceMarketOptionsRequestTypeDef,
-        "CreditSpecification": CreditSpecificationRequestTypeDef,
-        "CpuOptions": CpuOptionsRequestTypeDef,
-        "CapacityReservationSpecification": CapacityReservationSpecificationTypeDef,
-        "HibernationOptions": HibernationOptionsRequestTypeDef,
-        "LicenseSpecifications": Sequence[LicenseConfigurationRequestTypeDef],
-        "MetadataOptions": InstanceMetadataOptionsRequestTypeDef,
-        "EnclaveOptions": EnclaveOptionsRequestTypeDef,
-        "PrivateDnsNameOptions": PrivateDnsNameOptionsRequestTypeDef,
-        "MaintenanceOptions": InstanceMaintenanceOptionsRequestTypeDef,
-        "DisableApiStop": bool,
-    },
-    total=False,
-)
-
-
-class RunInstancesRequestServiceResourceCreateInstancesTypeDef(
-    _RequiredRunInstancesRequestServiceResourceCreateInstancesTypeDef,
-    _OptionalRunInstancesRequestServiceResourceCreateInstancesTypeDef,
-):
-    pass
-
-
 RequestSpotInstancesRequestRequestTypeDef = TypedDict(
     "RequestSpotInstancesRequestRequestTypeDef",
     {
         "AvailabilityZoneGroup": str,
         "BlockDurationMinutes": int,
         "ClientToken": str,
         "DryRun": bool,
         "InstanceCount": int,
         "LaunchGroup": str,
         "LaunchSpecification": RequestSpotLaunchSpecificationTypeDef,
         "SpotPrice": str,
         "Type": SpotInstanceTypeType,
         "ValidFrom": TimestampTypeDef,
         "ValidUntil": TimestampTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
     },
     total=False,
 )
 
 DisableFastSnapshotRestoresResultTypeDef = TypedDict(
     "DisableFastSnapshotRestoresResultTypeDef",
@@ -31554,50 +31574,14 @@
         "TpmSupport": str,
         "MaintenanceOptions": InstanceMaintenanceOptionsTypeDef,
         "CurrentInstanceBootMode": InstanceBootModeValuesType,
     },
     total=False,
 )
 
-FleetLaunchTemplateConfigTypeDef = TypedDict(
-    "FleetLaunchTemplateConfigTypeDef",
-    {
-        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
-        "Overrides": List[FleetLaunchTemplateOverridesTypeDef],
-    },
-    total=False,
-)
-
-LaunchTemplateAndOverridesResponseTypeDef = TypedDict(
-    "LaunchTemplateAndOverridesResponseTypeDef",
-    {
-        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
-        "Overrides": FleetLaunchTemplateOverridesTypeDef,
-    },
-    total=False,
-)
-
-LaunchTemplateConfigOutputTypeDef = TypedDict(
-    "LaunchTemplateConfigOutputTypeDef",
-    {
-        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
-        "Overrides": List[LaunchTemplateOverridesOutputTypeDef],
-    },
-    total=False,
-)
-
-LaunchTemplateConfigTypeDef = TypedDict(
-    "LaunchTemplateConfigTypeDef",
-    {
-        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
-        "Overrides": Sequence[LaunchTemplateOverridesTypeDef],
-    },
-    total=False,
-)
-
 FleetLaunchTemplateConfigRequestTypeDef = TypedDict(
     "FleetLaunchTemplateConfigRequestTypeDef",
     {
         "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationRequestTypeDef,
         "Overrides": Sequence[FleetLaunchTemplateOverridesRequestTypeDef],
     },
     total=False,
@@ -31656,150 +31640,66 @@
 class GetSpotPlacementScoresRequestRequestTypeDef(
     _RequiredGetSpotPlacementScoresRequestRequestTypeDef,
     _OptionalGetSpotPlacementScoresRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeInstanceStatusResultTypeDef = TypedDict(
-    "DescribeInstanceStatusResultTypeDef",
-    {
-        "InstanceStatuses": List[InstanceStatusTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSecurityGroupsResultTypeDef = TypedDict(
-    "DescribeSecurityGroupsResultTypeDef",
-    {
-        "SecurityGroups": List[SecurityGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
-    "_RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef",
-    {
-        "GroupId": str,
-    },
-)
-_OptionalAuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
-    "_OptionalAuthorizeSecurityGroupEgressRequestRequestTypeDef",
+FleetLaunchTemplateConfigTypeDef = TypedDict(
+    "FleetLaunchTemplateConfigTypeDef",
     {
-        "DryRun": bool,
-        "IpPermissions": Sequence[IpPermissionUnionTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "CidrIp": str,
-        "FromPort": int,
-        "IpProtocol": str,
-        "ToPort": int,
-        "SourceSecurityGroupName": str,
-        "SourceSecurityGroupOwnerId": str,
+        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
+        "Overrides": List[FleetLaunchTemplateOverridesTypeDef],
     },
     total=False,
 )
 
-
-class AuthorizeSecurityGroupEgressRequestRequestTypeDef(
-    _RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef,
-    _OptionalAuthorizeSecurityGroupEgressRequestRequestTypeDef,
-):
-    pass
-
-
-AuthorizeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
-    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
+LaunchTemplateAndOverridesResponseTypeDef = TypedDict(
+    "LaunchTemplateAndOverridesResponseTypeDef",
     {
-        "CidrIp": str,
-        "FromPort": int,
-        "GroupId": str,
-        "GroupName": str,
-        "IpPermissions": Sequence[IpPermissionUnionTypeDef],
-        "IpProtocol": str,
-        "SourceSecurityGroupName": str,
-        "SourceSecurityGroupOwnerId": str,
-        "ToPort": int,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
+        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
+        "Overrides": FleetLaunchTemplateOverridesTypeDef,
     },
     total=False,
 )
 
-_RequiredRevokeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
-    "_RequiredRevokeSecurityGroupEgressRequestRequestTypeDef",
-    {
-        "GroupId": str,
-    },
-)
-_OptionalRevokeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
-    "_OptionalRevokeSecurityGroupEgressRequestRequestTypeDef",
+LaunchTemplateConfigTypeDef = TypedDict(
+    "LaunchTemplateConfigTypeDef",
     {
-        "DryRun": bool,
-        "IpPermissions": Sequence[IpPermissionUnionTypeDef],
-        "SecurityGroupRuleIds": Sequence[str],
-        "CidrIp": str,
-        "FromPort": int,
-        "IpProtocol": str,
-        "ToPort": int,
-        "SourceSecurityGroupName": str,
-        "SourceSecurityGroupOwnerId": str,
+        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
+        "Overrides": List[LaunchTemplateOverridesTypeDef],
     },
     total=False,
 )
 
-
-class RevokeSecurityGroupEgressRequestRequestTypeDef(
-    _RequiredRevokeSecurityGroupEgressRequestRequestTypeDef,
-    _OptionalRevokeSecurityGroupEgressRequestRequestTypeDef,
-):
-    pass
-
-
-RevokeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
-    "RevokeSecurityGroupIngressRequestRequestTypeDef",
+DescribeInstanceStatusResultTypeDef = TypedDict(
+    "DescribeInstanceStatusResultTypeDef",
     {
-        "CidrIp": str,
-        "FromPort": int,
-        "GroupId": str,
-        "GroupName": str,
-        "IpPermissions": Sequence[IpPermissionUnionTypeDef],
-        "IpProtocol": str,
-        "SourceSecurityGroupName": str,
-        "SourceSecurityGroupOwnerId": str,
-        "ToPort": int,
-        "DryRun": bool,
-        "SecurityGroupRuleIds": Sequence[str],
+        "InstanceStatuses": List[InstanceStatusTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef = TypedDict(
-    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
+DescribeSecurityGroupsResultTypeDef = TypedDict(
+    "DescribeSecurityGroupsResultTypeDef",
     {
-        "DryRun": bool,
-        "GroupId": str,
-        "GroupName": str,
-        "IpPermissions": Sequence[IpPermissionUnionTypeDef],
-        "SecurityGroupRuleDescriptions": Sequence[SecurityGroupRuleDescriptionTypeDef],
+        "SecurityGroups": List[SecurityGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef = TypedDict(
-    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
+DescribeSecurityGroupsResultVpcAddressTypeDef = TypedDict(
+    "DescribeSecurityGroupsResultVpcAddressTypeDef",
     {
-        "DryRun": bool,
-        "GroupId": str,
-        "GroupName": str,
-        "IpPermissions": Sequence[IpPermissionUnionTypeDef],
-        "SecurityGroupRuleDescriptions": Sequence[SecurityGroupRuleDescriptionTypeDef],
+        "SecurityGroups": List[SecurityGroupVpcAddressTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeStaleSecurityGroupsResultTypeDef = TypedDict(
     "DescribeStaleSecurityGroupsResultTypeDef",
     {
         "NextToken": str,
         "StaleSecurityGroupSet": List[StaleSecurityGroupTypeDef],
@@ -31846,15 +31746,15 @@
     },
 )
 _OptionalCreateNetworkInsightsAccessScopeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateNetworkInsightsAccessScopeRequestRequestTypeDef",
     {
         "MatchPaths": Sequence[AccessScopePathRequestTypeDef],
         "ExcludePaths": Sequence[AccessScopePathRequestTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "DryRun": bool,
     },
     total=False,
 )
 
 
 class CreateNetworkInsightsAccessScopeRequestRequestTypeDef(
@@ -31870,38 +31770,14 @@
         "NetworkInsightsAccessScopeId": str,
         "MatchPaths": List[AccessScopePathTypeDef],
         "ExcludePaths": List[AccessScopePathTypeDef],
     },
     total=False,
 )
 
-BundleInstanceResultTypeDef = TypedDict(
-    "BundleInstanceResultTypeDef",
-    {
-        "BundleTask": BundleTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelBundleTaskResultTypeDef = TypedDict(
-    "CancelBundleTaskResultTypeDef",
-    {
-        "BundleTask": BundleTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBundleTasksResultTypeDef = TypedDict(
-    "DescribeBundleTasksResultTypeDef",
-    {
-        "BundleTasks": List[BundleTaskTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredRunScheduledInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredRunScheduledInstancesRequestRequestTypeDef",
     {
         "LaunchSpecification": ScheduledInstancesLaunchSpecificationTypeDef,
         "ScheduledInstanceId": str,
     },
 )
@@ -32136,15 +32012,15 @@
 )
 _OptionalCreateLaunchTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateLaunchTemplateRequestRequestTypeDef",
     {
         "DryRun": bool,
         "ClientToken": str,
         "VersionDescription": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
     total=False,
 )
 
 
 class CreateLaunchTemplateRequestRequestTypeDef(
     _RequiredCreateLaunchTemplateRequestRequestTypeDef,
@@ -32195,29 +32071,53 @@
     {
         "NetworkInterfaces": List[NetworkInterfaceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BundleInstanceResultTypeDef = TypedDict(
+    "BundleInstanceResultTypeDef",
+    {
+        "BundleTask": BundleTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelBundleTaskResultTypeDef = TypedDict(
+    "CancelBundleTaskResultTypeDef",
+    {
+        "BundleTask": BundleTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBundleTasksResultTypeDef = TypedDict(
+    "DescribeBundleTasksResultTypeDef",
+    {
+        "BundleTasks": List[BundleTaskTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateVpnConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpnConnectionRequestRequestTypeDef",
     {
         "CustomerGatewayId": str,
         "Type": str,
     },
 )
 _OptionalCreateVpnConnectionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateVpnConnectionRequestRequestTypeDef",
     {
         "VpnGatewayId": str,
         "TransitGatewayId": str,
         "DryRun": bool,
         "Options": VpnConnectionOptionsSpecificationTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
     total=False,
 )
 
 
 class CreateVpnConnectionRequestRequestTypeDef(
     _RequiredCreateVpnConnectionRequestRequestTypeDef,
@@ -32318,14 +32218,72 @@
         "OwnerId": str,
         "RequesterId": str,
         "ReservationId": str,
     },
     total=False,
 )
 
+_RequiredCreateFleetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFleetRequestRequestTypeDef",
+    {
+        "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
+        "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
+    },
+)
+_OptionalCreateFleetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFleetRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "ClientToken": str,
+        "SpotOptions": SpotOptionsRequestTypeDef,
+        "OnDemandOptions": OnDemandOptionsRequestTypeDef,
+        "ExcessCapacityTerminationPolicy": FleetExcessCapacityTerminationPolicyType,
+        "TerminateInstancesWithExpiration": bool,
+        "Type": FleetTypeType,
+        "ValidFrom": TimestampTypeDef,
+        "ValidUntil": TimestampTypeDef,
+        "ReplaceUnhealthyInstances": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "Context": str,
+    },
+    total=False,
+)
+
+
+class CreateFleetRequestRequestTypeDef(
+    _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredModifyFleetRequestRequestTypeDef = TypedDict(
+    "_RequiredModifyFleetRequestRequestTypeDef",
+    {
+        "FleetId": str,
+    },
+)
+_OptionalModifyFleetRequestRequestTypeDef = TypedDict(
+    "_OptionalModifyFleetRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "ExcessCapacityTerminationPolicy": FleetExcessCapacityTerminationPolicyType,
+        "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
+        "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
+        "Context": str,
+    },
+    total=False,
+)
+
+
+class ModifyFleetRequestRequestTypeDef(
+    _RequiredModifyFleetRequestRequestTypeDef, _OptionalModifyFleetRequestRequestTypeDef
+):
+    pass
+
+
 CreateFleetErrorTypeDef = TypedDict(
     "CreateFleetErrorTypeDef",
     {
         "LaunchTemplateAndOverrides": LaunchTemplateAndOverridesResponseTypeDef,
         "Lifecycle": InstanceLifecycleType,
         "ErrorCode": str,
         "ErrorMessage": str,
@@ -32364,63 +32322,40 @@
         "InstanceIds": List[str],
         "InstanceType": InstanceTypeType,
         "Platform": Literal["Windows"],
     },
     total=False,
 )
 
-_RequiredSpotFleetRequestConfigDataOutputTypeDef = TypedDict(
-    "_RequiredSpotFleetRequestConfigDataOutputTypeDef",
+_RequiredModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
+    "_RequiredModifySpotFleetRequestRequestRequestTypeDef",
     {
-        "IamFleetRole": str,
-        "TargetCapacity": int,
+        "SpotFleetRequestId": str,
     },
 )
-_OptionalSpotFleetRequestConfigDataOutputTypeDef = TypedDict(
-    "_OptionalSpotFleetRequestConfigDataOutputTypeDef",
+_OptionalModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
+    "_OptionalModifySpotFleetRequestRequestRequestTypeDef",
     {
-        "AllocationStrategy": AllocationStrategyType,
-        "OnDemandAllocationStrategy": OnDemandAllocationStrategyType,
-        "SpotMaintenanceStrategies": SpotMaintenanceStrategiesTypeDef,
-        "ClientToken": str,
         "ExcessCapacityTerminationPolicy": ExcessCapacityTerminationPolicyType,
-        "FulfilledCapacity": float,
-        "OnDemandFulfilledCapacity": float,
-        "LaunchSpecifications": List[SpotFleetLaunchSpecificationOutputTypeDef],
-        "LaunchTemplateConfigs": List[LaunchTemplateConfigOutputTypeDef],
-        "SpotPrice": str,
+        "LaunchTemplateConfigs": Sequence[LaunchTemplateConfigTypeDef],
+        "TargetCapacity": int,
         "OnDemandTargetCapacity": int,
-        "OnDemandMaxTotalPrice": str,
-        "SpotMaxTotalPrice": str,
-        "TerminateInstancesWithExpiration": bool,
-        "Type": FleetTypeType,
-        "ValidFrom": datetime,
-        "ValidUntil": datetime,
-        "ReplaceUnhealthyInstances": bool,
-        "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
-        "LoadBalancersConfig": LoadBalancersConfigOutputTypeDef,
-        "InstancePoolsToUseCount": int,
         "Context": str,
-        "TargetCapacityUnitType": TargetCapacityUnitTypeType,
-        "TagSpecifications": List[TagSpecificationOutputTypeDef],
     },
     total=False,
 )
 
 
-class SpotFleetRequestConfigDataOutputTypeDef(
-    _RequiredSpotFleetRequestConfigDataOutputTypeDef,
-    _OptionalSpotFleetRequestConfigDataOutputTypeDef,
+class ModifySpotFleetRequestRequestRequestTypeDef(
+    _RequiredModifySpotFleetRequestRequestRequestTypeDef,
+    _OptionalModifySpotFleetRequestRequestRequestTypeDef,
 ):
     pass
 
 
-LaunchTemplateConfigUnionTypeDef = Union[
-    LaunchTemplateConfigTypeDef, LaunchTemplateConfigOutputTypeDef
-]
 _RequiredSpotFleetRequestConfigDataTypeDef = TypedDict(
     "_RequiredSpotFleetRequestConfigDataTypeDef",
     {
         "IamFleetRole": str,
         "TargetCapacity": int,
     },
 )
@@ -32430,96 +32365,84 @@
         "AllocationStrategy": AllocationStrategyType,
         "OnDemandAllocationStrategy": OnDemandAllocationStrategyType,
         "SpotMaintenanceStrategies": SpotMaintenanceStrategiesTypeDef,
         "ClientToken": str,
         "ExcessCapacityTerminationPolicy": ExcessCapacityTerminationPolicyType,
         "FulfilledCapacity": float,
         "OnDemandFulfilledCapacity": float,
-        "LaunchSpecifications": Sequence[SpotFleetLaunchSpecificationTypeDef],
-        "LaunchTemplateConfigs": Sequence[LaunchTemplateConfigTypeDef],
+        "LaunchSpecifications": List[SpotFleetLaunchSpecificationTypeDef],
+        "LaunchTemplateConfigs": List[LaunchTemplateConfigTypeDef],
         "SpotPrice": str,
         "OnDemandTargetCapacity": int,
         "OnDemandMaxTotalPrice": str,
         "SpotMaxTotalPrice": str,
         "TerminateInstancesWithExpiration": bool,
         "Type": FleetTypeType,
-        "ValidFrom": TimestampTypeDef,
-        "ValidUntil": TimestampTypeDef,
+        "ValidFrom": datetime,
+        "ValidUntil": datetime,
         "ReplaceUnhealthyInstances": bool,
         "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
         "LoadBalancersConfig": LoadBalancersConfigTypeDef,
         "InstancePoolsToUseCount": int,
         "Context": str,
         "TargetCapacityUnitType": TargetCapacityUnitTypeType,
-        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "TagSpecifications": List[TagSpecificationTypeDef],
     },
     total=False,
 )
 
 
 class SpotFleetRequestConfigDataTypeDef(
     _RequiredSpotFleetRequestConfigDataTypeDef, _OptionalSpotFleetRequestConfigDataTypeDef
 ):
     pass
 
 
-_RequiredCreateFleetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFleetRequestRequestTypeDef",
+_RequiredSpotFleetRequestConfigDataVpcAddressTypeDef = TypedDict(
+    "_RequiredSpotFleetRequestConfigDataVpcAddressTypeDef",
     {
-        "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
-        "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
+        "IamFleetRole": str,
+        "TargetCapacity": int,
     },
 )
-_OptionalCreateFleetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFleetRequestRequestTypeDef",
+_OptionalSpotFleetRequestConfigDataVpcAddressTypeDef = TypedDict(
+    "_OptionalSpotFleetRequestConfigDataVpcAddressTypeDef",
     {
-        "DryRun": bool,
+        "AllocationStrategy": AllocationStrategyType,
+        "OnDemandAllocationStrategy": OnDemandAllocationStrategyType,
+        "SpotMaintenanceStrategies": SpotMaintenanceStrategiesTypeDef,
         "ClientToken": str,
-        "SpotOptions": SpotOptionsRequestTypeDef,
-        "OnDemandOptions": OnDemandOptionsRequestTypeDef,
-        "ExcessCapacityTerminationPolicy": FleetExcessCapacityTerminationPolicyType,
+        "ExcessCapacityTerminationPolicy": ExcessCapacityTerminationPolicyType,
+        "FulfilledCapacity": float,
+        "OnDemandFulfilledCapacity": float,
+        "LaunchSpecifications": List[SpotFleetLaunchSpecificationTypeDef],
+        "LaunchTemplateConfigs": List[LaunchTemplateConfigTypeDef],
+        "SpotPrice": str,
+        "OnDemandTargetCapacity": int,
+        "OnDemandMaxTotalPrice": str,
+        "SpotMaxTotalPrice": str,
         "TerminateInstancesWithExpiration": bool,
         "Type": FleetTypeType,
-        "ValidFrom": TimestampTypeDef,
-        "ValidUntil": TimestampTypeDef,
+        "ValidFrom": datetime,
+        "ValidUntil": datetime,
         "ReplaceUnhealthyInstances": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "Context": str,
-    },
-    total=False,
-)
-
-
-class CreateFleetRequestRequestTypeDef(
-    _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredModifyFleetRequestRequestTypeDef = TypedDict(
-    "_RequiredModifyFleetRequestRequestTypeDef",
-    {
-        "FleetId": str,
-    },
-)
-_OptionalModifyFleetRequestRequestTypeDef = TypedDict(
-    "_OptionalModifyFleetRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "ExcessCapacityTerminationPolicy": FleetExcessCapacityTerminationPolicyType,
-        "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
-        "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
+        "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
+        "LoadBalancersConfig": LoadBalancersConfigTypeDef,
+        "InstancePoolsToUseCount": int,
         "Context": str,
+        "TargetCapacityUnitType": TargetCapacityUnitTypeType,
+        "TagSpecifications": List[TagSpecificationVpcAddressTypeDef],
     },
     total=False,
 )
 
 
-class ModifyFleetRequestRequestTypeDef(
-    _RequiredModifyFleetRequestRequestTypeDef, _OptionalModifyFleetRequestRequestTypeDef
+class SpotFleetRequestConfigDataVpcAddressTypeDef(
+    _RequiredSpotFleetRequestConfigDataVpcAddressTypeDef,
+    _OptionalSpotFleetRequestConfigDataVpcAddressTypeDef,
 ):
     pass
 
 
 CreateLaunchTemplateVersionResultTypeDef = TypedDict(
     "CreateLaunchTemplateVersionResultTypeDef",
     {
@@ -32691,77 +32614,61 @@
         "Errors": List[DescribeFleetErrorTypeDef],
         "Instances": List[DescribeFleetsInstancesTypeDef],
         "Context": str,
     },
     total=False,
 )
 
-SpotFleetRequestConfigTypeDef = TypedDict(
-    "SpotFleetRequestConfigTypeDef",
-    {
-        "ActivityStatus": ActivityStatusType,
-        "CreateTime": datetime,
-        "SpotFleetRequestConfig": SpotFleetRequestConfigDataOutputTypeDef,
-        "SpotFleetRequestId": str,
-        "SpotFleetRequestState": BatchStateType,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-_RequiredModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
-    "_RequiredModifySpotFleetRequestRequestRequestTypeDef",
+_RequiredRequestSpotFleetRequestRequestTypeDef = TypedDict(
+    "_RequiredRequestSpotFleetRequestRequestTypeDef",
     {
-        "SpotFleetRequestId": str,
+        "SpotFleetRequestConfig": SpotFleetRequestConfigDataTypeDef,
     },
 )
-_OptionalModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
-    "_OptionalModifySpotFleetRequestRequestRequestTypeDef",
+_OptionalRequestSpotFleetRequestRequestTypeDef = TypedDict(
+    "_OptionalRequestSpotFleetRequestRequestTypeDef",
     {
-        "ExcessCapacityTerminationPolicy": ExcessCapacityTerminationPolicyType,
-        "LaunchTemplateConfigs": Sequence[LaunchTemplateConfigUnionTypeDef],
-        "TargetCapacity": int,
-        "OnDemandTargetCapacity": int,
-        "Context": str,
+        "DryRun": bool,
     },
     total=False,
 )
 
 
-class ModifySpotFleetRequestRequestRequestTypeDef(
-    _RequiredModifySpotFleetRequestRequestRequestTypeDef,
-    _OptionalModifySpotFleetRequestRequestRequestTypeDef,
+class RequestSpotFleetRequestRequestTypeDef(
+    _RequiredRequestSpotFleetRequestRequestTypeDef, _OptionalRequestSpotFleetRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredRequestSpotFleetRequestRequestTypeDef = TypedDict(
-    "_RequiredRequestSpotFleetRequestRequestTypeDef",
+SpotFleetRequestConfigTypeDef = TypedDict(
+    "SpotFleetRequestConfigTypeDef",
     {
+        "ActivityStatus": ActivityStatusType,
+        "CreateTime": datetime,
         "SpotFleetRequestConfig": SpotFleetRequestConfigDataTypeDef,
+        "SpotFleetRequestId": str,
+        "SpotFleetRequestState": BatchStateType,
+        "Tags": List[TagTypeDef],
     },
+    total=False,
 )
-_OptionalRequestSpotFleetRequestRequestTypeDef = TypedDict(
-    "_OptionalRequestSpotFleetRequestRequestTypeDef",
+
+SpotFleetRequestConfigVpcAddressTypeDef = TypedDict(
+    "SpotFleetRequestConfigVpcAddressTypeDef",
     {
-        "DryRun": bool,
+        "ActivityStatus": ActivityStatusType,
+        "CreateTime": datetime,
+        "SpotFleetRequestConfig": SpotFleetRequestConfigDataVpcAddressTypeDef,
+        "SpotFleetRequestId": str,
+        "SpotFleetRequestState": BatchStateType,
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-
-class RequestSpotFleetRequestRequestTypeDef(
-    _RequiredRequestSpotFleetRequestRequestTypeDef, _OptionalRequestSpotFleetRequestRequestTypeDef
-):
-    pass
-
-
-SpotFleetRequestConfigDataUnionTypeDef = Union[
-    SpotFleetRequestConfigDataTypeDef, SpotFleetRequestConfigDataOutputTypeDef
-]
 DescribeFleetsResultTypeDef = TypedDict(
     "DescribeFleetsResultTypeDef",
     {
         "NextToken": str,
         "Fleets": List[FleetDataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -32771,7 +32678,16 @@
     "DescribeSpotFleetRequestsResponseTypeDef",
     {
         "NextToken": str,
         "SpotFleetRequestConfigs": List[SpotFleetRequestConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+DescribeSpotFleetRequestsResponseVpcAddressTypeDef = TypedDict(
+    "DescribeSpotFleetRequestsResponseVpcAddressTypeDef",
+    {
+        "NextToken": str,
+        "SpotFleetRequestConfigs": List[SpotFleetRequestConfigVpcAddressTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/type_defs.pyi` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -805,15 +805,14 @@
     "HostPropertiesTypeDef",
     "IKEVersionsListValueTypeDef",
     "IKEVersionsRequestListValueTypeDef",
     "IamInstanceProfileTypeDef",
     "LaunchPermissionTypeDef",
     "UserBucketTypeDef",
     "ImageRecycleBinInfoTypeDef",
-    "StateReasonTypeDef",
     "ImportClientVpnClientCertificateRevocationListRequestRequestTypeDef",
     "ImportImageLicenseConfigurationRequestTypeDef",
     "ImportImageLicenseConfigurationResponseTypeDef",
     "UserDataTypeDef",
     "InferenceDeviceInfoTypeDef",
     "InstanceCountTypeDef",
     "InstanceCreditSpecificationRequestTypeDef",
@@ -824,26 +823,26 @@
     "InstanceMaintenanceOptionsRequestTypeDef",
     "InstanceMaintenanceOptionsTypeDef",
     "InstanceMetadataOptionsRequestTypeDef",
     "InstanceMetadataOptionsResponseTypeDef",
     "MonitoringTypeDef",
     "InstanceNetworkInterfaceAssociationTypeDef",
     "InstanceNetworkInterfaceAttachmentTypeDef",
-    "MemoryGiBPerVCpuTypeDef",
-    "MemoryMiBTypeDef",
-    "NetworkBandwidthGbpsTypeDef",
-    "NetworkInterfaceCountTypeDef",
-    "TotalLocalStorageGBTypeDef",
-    "VCpuCountRangeTypeDef",
     "MemoryGiBPerVCpuRequestTypeDef",
     "MemoryMiBRequestTypeDef",
     "NetworkBandwidthGbpsRequestTypeDef",
     "NetworkInterfaceCountRequestTypeDef",
     "TotalLocalStorageGBRequestTypeDef",
     "VCpuCountRangeRequestTypeDef",
+    "MemoryGiBPerVCpuTypeDef",
+    "MemoryMiBTypeDef",
+    "NetworkBandwidthGbpsTypeDef",
+    "NetworkInterfaceCountTypeDef",
+    "TotalLocalStorageGBTypeDef",
+    "VCpuCountRangeTypeDef",
     "InstanceStateTypeDef",
     "InstanceStatusDetailsTypeDef",
     "InstanceStatusEventTypeDef",
     "LicenseConfigurationTypeDef",
     "PrivateDnsNameOptionsResponseTypeDef",
     "MemoryInfoTypeDef",
     "PlacementGroupInfoTypeDef",
@@ -1028,15 +1027,14 @@
     "RestoreAddressToClassicRequestRequestTypeDef",
     "RestoreImageFromRecycleBinRequestRequestTypeDef",
     "RestoreManagedPrefixListVersionRequestRequestTypeDef",
     "RestoreSnapshotFromRecycleBinRequestRequestTypeDef",
     "RestoreSnapshotTierRequestRequestTypeDef",
     "RevokeClientVpnIngressRequestRequestTypeDef",
     "RouteTypeDef",
-    "S3StorageOutputTypeDef",
     "ScheduledInstanceRecurrenceTypeDef",
     "ScheduledInstancesEbsTypeDef",
     "ScheduledInstancesIamInstanceProfileTypeDef",
     "ScheduledInstancesIpv6AddressTypeDef",
     "ScheduledInstancesMonitoringTypeDef",
     "ScheduledInstancesPlacementTypeDef",
     "ScheduledInstancesPrivateIpAddressConfigTypeDef",
@@ -1222,14 +1220,15 @@
     "RestoreImageFromRecycleBinResultTypeDef",
     "RestoreSnapshotFromRecycleBinResultTypeDef",
     "RestoreSnapshotTierResultTypeDef",
     "RouteTableAssociationStateResponseTypeDef",
     "RunScheduledInstancesResultTypeDef",
     "StartVpcEndpointServicePrivateDnsVerificationResultTypeDef",
     "StateReasonResponseTypeDef",
+    "StateReasonTypeDef",
     "UnassignIpv6AddressesResultTypeDef",
     "UpdateSecurityGroupRuleDescriptionsEgressResultTypeDef",
     "UpdateSecurityGroupRuleDescriptionsIngressResultTypeDef",
     "VolumeAttachmentResponseTypeDef",
     "VpcPeeringConnectionStateReasonResponseTypeDef",
     "AcceptReservedInstancesExchangeQuoteRequestRequestTypeDef",
     "GetReservedInstancesExchangeQuoteRequestRequestTypeDef",
@@ -1275,19 +1274,18 @@
     "NetworkInsightsAccessScopeTypeDef",
     "PlacementGroupTypeDef",
     "ReplaceRootVolumeTaskTypeDef",
     "SnapshotInfoTypeDef",
     "SnapshotResponseTypeDef",
     "SnapshotTierStatusTypeDef",
     "SnapshotTypeDef",
-    "SpotFleetTagSpecificationOutputTypeDef",
     "SpotFleetTagSpecificationTypeDef",
     "SubnetCidrReservationTypeDef",
-    "TagSpecificationOutputTypeDef",
     "TagSpecificationTypeDef",
+    "TagSpecificationVpcAddressTypeDef",
     "TrafficMirrorSessionTypeDef",
     "TrafficMirrorTargetTypeDef",
     "TransitGatewayPolicyTableTypeDef",
     "TransitGatewayRouteTableAnnouncementTypeDef",
     "TransitGatewayRouteTableTypeDef",
     "TrunkInterfaceAssociationTypeDef",
     "VerifiedAccessGroupTypeDef",
@@ -1370,15 +1368,14 @@
     "CapacityReservationSpecificationResponseResponseTypeDef",
     "CapacityReservationSpecificationResponseTypeDef",
     "LaunchTemplateCapacityReservationSpecificationResponseTypeDef",
     "CapacityReservationSpecificationTypeDef",
     "LaunchTemplateCapacityReservationSpecificationRequestTypeDef",
     "DescribeVpcClassicLinkDnsSupportResultTypeDef",
     "ClassicLinkInstanceTypeDef",
-    "ClassicLoadBalancersConfigOutputTypeDef",
     "ClassicLoadBalancersConfigTypeDef",
     "ExportClientVpnClientCertificateRevocationListResultTypeDef",
     "ClientConnectResponseOptionsTypeDef",
     "ClientVpnAuthenticationRequestTypeDef",
     "ClientVpnAuthenticationTypeDef",
     "ClientVpnConnectionTypeDef",
     "TerminateConnectionStatusTypeDef",
@@ -1401,15 +1398,16 @@
     "ModifyLocalGatewayRouteResultTypeDef",
     "SearchLocalGatewayRoutesResultTypeDef",
     "CreateNetworkAclEntryRequestNetworkAclCreateEntryTypeDef",
     "CreateNetworkAclEntryRequestRequestTypeDef",
     "NetworkAclEntryTypeDef",
     "ReplaceNetworkAclEntryRequestNetworkAclReplaceEntryTypeDef",
     "ReplaceNetworkAclEntryRequestRequestTypeDef",
-    "InstanceNetworkInterfaceSpecificationOutputTypeDef",
+    "InstanceNetworkInterfaceSpecificationServiceResourceTypeDef",
+    "InstanceNetworkInterfaceSpecificationSubnetTypeDef",
     "InstanceNetworkInterfaceSpecificationTypeDef",
     "CreateReservedInstancesListingRequestRequestTypeDef",
     "CreateStoreImageTaskRequestRequestTypeDef",
     "CreateTrafficMirrorFilterRuleRequestRequestTypeDef",
     "ModifyTrafficMirrorFilterRuleRequestRequestTypeDef",
     "CreateVolumePermissionModificationsTypeDef",
     "ModifyVpcEndpointRequestRequestTypeDef",
@@ -1804,30 +1802,28 @@
     "GetVpnTunnelReplacementStatusResultTypeDef",
     "GpuDeviceInfoTypeDef",
     "IamInstanceProfileAssociationTypeDef",
     "LaunchPermissionModificationsTypeDef",
     "ImageDiskContainerTypeDef",
     "SnapshotDiskContainerTypeDef",
     "ListImagesInRecycleBinResultTypeDef",
-    "LocalGatewayRouteTableTypeDef",
     "ImportInstanceLaunchSpecificationTypeDef",
     "InferenceAcceleratorInfoTypeDef",
     "ModifyInstanceCreditSpecificationRequestRequestTypeDef",
     "LaunchTemplateInstanceNetworkInterfaceSpecificationRequestTypeDef",
     "ModifyInstanceMetadataOptionsResultTypeDef",
     "InstanceMonitoringTypeDef",
     "InstancePrivateIpAddressTypeDef",
-    "InstanceRequirementsOutputTypeDef",
-    "InstanceRequirementsTypeDef",
     "InstanceRequirementsRequestTypeDef",
+    "InstanceRequirementsTypeDef",
     "InstanceStateChangeTypeDef",
     "InstanceStatusSummaryTypeDef",
     "ModifyInstanceEventStartTimeResultTypeDef",
-    "IpPermissionOutputTypeDef",
     "IpPermissionTypeDef",
+    "IpPermissionVpcAddressTypeDef",
     "StaleIpPermissionTypeDef",
     "ProvisionIpamPoolCidrRequestRequestTypeDef",
     "IpamDiscoveredAccountTypeDef",
     "IpamDiscoveredResourceCidrTypeDef",
     "IpamPoolTypeDef",
     "IpamResourceCidrTypeDef",
     "IpamResourceDiscoveryTypeDef",
@@ -1868,15 +1864,14 @@
     "PurchaseReservedInstancesOfferingRequestRequestTypeDef",
     "ReservedInstancesOfferingTypeDef",
     "ReservedInstancesTypeDef",
     "SecurityGroupRuleTypeDef",
     "RegisterInstanceEventNotificationAttributesRequestRequestTypeDef",
     "RegisterTransitGatewayMulticastGroupMembersResultTypeDef",
     "RegisterTransitGatewayMulticastGroupSourcesResultTypeDef",
-    "StorageOutputTypeDef",
     "ScheduledInstanceAvailabilityTypeDef",
     "ScheduledInstanceTypeDef",
     "ScheduledInstancesBlockDeviceMappingTypeDef",
     "ScheduledInstancesNetworkInterfaceTypeDef",
     "SearchTransitGatewayMulticastGroupsResultTypeDef",
     "VpcEndpointTypeDef",
     "SecurityGroupRuleUpdateTypeDef",
@@ -1886,15 +1881,14 @@
     "SnapshotTaskDetailTypeDef",
     "SpotMaintenanceStrategiesTypeDef",
     "SpotDatafeedSubscriptionTypeDef",
     "TransitGatewayMulticastDomainAssociationTypeDef",
     "TransitGatewayMulticastDomainAssociationsTypeDef",
     "SubnetIpv6CidrBlockAssociationTypeDef",
     "TargetReservationValueTypeDef",
-    "TargetGroupsConfigOutputTypeDef",
     "TargetGroupsConfigTypeDef",
     "TrafficMirrorFilterRuleTypeDef",
     "TransitGatewayAttachmentTypeDef",
     "TransitGatewayConnectPeerConfigurationTypeDef",
     "TransitGatewayConnectTypeDef",
     "TransitGatewayMulticastDomainTypeDef",
     "TransitGatewayTypeDef",
@@ -1915,14 +1909,15 @@
     "VolumeResponseTypeDef",
     "VolumeTypeDef",
     "VolumeStatusInfoTypeDef",
     "VpcCidrBlockAssociationTypeDef",
     "VpcIpv6CidrBlockAssociationTypeDef",
     "VpcPeeringConnectionVpcInfoResponseTypeDef",
     "VpcPeeringConnectionVpcInfoTypeDef",
+    "LocalGatewayRouteTableTypeDef",
     "DescribeAccountAttributesResultTypeDef",
     "AdditionalDetailTypeDef",
     "DescribeAddressesAttributeResultTypeDef",
     "ModifyAddressAttributeResultTypeDef",
     "ResetAddressAttributeResultTypeDef",
     "DescribeAddressesResultTypeDef",
     "DescribeVpcEndpointServicePermissionsResultTypeDef",
@@ -1975,23 +1970,104 @@
     "DescribeReplaceRootVolumeTasksResultTypeDef",
     "CreateSnapshotsResultTypeDef",
     "DescribeSnapshotTierStatusResultTypeDef",
     "DescribeSnapshotsResultTypeDef",
     "CreateSubnetCidrReservationResultTypeDef",
     "DeleteSubnetCidrReservationResultTypeDef",
     "GetSubnetCidrReservationsResultTypeDef",
+    "AcceptAddressTransferRequestRequestTypeDef",
+    "AllocateAddressRequestRequestTypeDef",
+    "AllocateHostsRequestRequestTypeDef",
+    "AssociateIpamResourceDiscoveryRequestRequestTypeDef",
+    "CopySnapshotRequestRequestTypeDef",
     "CopySnapshotRequestSnapshotCopyTypeDef",
+    "CreateCapacityReservationFleetRequestRequestTypeDef",
+    "CreateCapacityReservationRequestRequestTypeDef",
+    "CreateCarrierGatewayRequestRequestTypeDef",
+    "CreateCoipPoolRequestRequestTypeDef",
+    "CreateCustomerGatewayRequestRequestTypeDef",
+    "CreateDhcpOptionsRequestRequestTypeDef",
+    "CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
+    "CreateEgressOnlyInternetGatewayRequestRequestTypeDef",
+    "CreateFlowLogsRequestRequestTypeDef",
+    "CreateFpgaImageRequestRequestTypeDef",
+    "CreateInstanceConnectEndpointRequestRequestTypeDef",
+    "CreateInstanceEventWindowRequestRequestTypeDef",
+    "CreateInstanceExportTaskRequestRequestTypeDef",
+    "CreateInternetGatewayRequestRequestTypeDef",
+    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
+    "CreateIpamPoolRequestRequestTypeDef",
+    "CreateIpamRequestRequestTypeDef",
+    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
+    "CreateIpamScopeRequestRequestTypeDef",
+    "CreateKeyPairRequestRequestTypeDef",
+    "CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
+    "CreateLocalGatewayRouteTableRequestRequestTypeDef",
+    "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
+    "CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
+    "CreateManagedPrefixListRequestRequestTypeDef",
+    "CreateNatGatewayRequestRequestTypeDef",
+    "CreateNetworkAclRequestRequestTypeDef",
+    "CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
     "CreateNetworkAclRequestVpcCreateNetworkAclTypeDef",
+    "CreateNetworkInterfaceRequestRequestTypeDef",
+    "CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
     "CreateNetworkInterfaceRequestSubnetCreateNetworkInterfaceTypeDef",
+    "CreatePlacementGroupRequestRequestTypeDef",
+    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
+    "CreatePublicIpv4PoolRequestRequestTypeDef",
+    "CreateReplaceRootVolumeTaskRequestRequestTypeDef",
+    "CreateRestoreImageTaskRequestRequestTypeDef",
+    "CreateRouteTableRequestRequestTypeDef",
+    "CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
     "CreateRouteTableRequestVpcCreateRouteTableTypeDef",
+    "CreateSecurityGroupRequestRequestTypeDef",
+    "CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
     "CreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef",
+    "CreateSnapshotRequestRequestTypeDef",
+    "CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
     "CreateSnapshotRequestVolumeCreateSnapshotTypeDef",
+    "CreateSnapshotsRequestRequestTypeDef",
+    "CreateSubnetCidrReservationRequestRequestTypeDef",
+    "CreateSubnetRequestRequestTypeDef",
+    "CreateSubnetRequestServiceResourceCreateSubnetTypeDef",
     "CreateSubnetRequestVpcCreateSubnetTypeDef",
+    "CreateTrafficMirrorFilterRequestRequestTypeDef",
+    "CreateTrafficMirrorSessionRequestRequestTypeDef",
+    "CreateTrafficMirrorTargetRequestRequestTypeDef",
+    "CreateTransitGatewayConnectPeerRequestRequestTypeDef",
+    "CreateTransitGatewayConnectRequestRequestTypeDef",
+    "CreateTransitGatewayMulticastDomainRequestRequestTypeDef",
+    "CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
+    "CreateTransitGatewayPolicyTableRequestRequestTypeDef",
+    "CreateTransitGatewayRequestRequestTypeDef",
+    "CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
+    "CreateTransitGatewayRouteTableRequestRequestTypeDef",
+    "CreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
+    "CreateVerifiedAccessEndpointRequestRequestTypeDef",
+    "CreateVerifiedAccessGroupRequestRequestTypeDef",
+    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
+    "CreateVerifiedAccessTrustProviderRequestRequestTypeDef",
+    "CreateVolumeRequestRequestTypeDef",
+    "CreateVolumeRequestServiceResourceCreateVolumeTypeDef",
+    "CreateVpcEndpointRequestRequestTypeDef",
+    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
+    "CreateVpcPeeringConnectionRequestRequestTypeDef",
+    "CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
     "CreateVpcPeeringConnectionRequestVpcRequestVpcPeeringConnectionTypeDef",
-    "TagSpecificationUnionTypeDef",
+    "CreateVpcRequestRequestTypeDef",
+    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
+    "CreateVpnGatewayRequestRequestTypeDef",
+    "ExportImageRequestRequestTypeDef",
+    "ImportKeyPairRequestRequestTypeDef",
+    "ImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
+    "ProvisionByoipCidrRequestRequestTypeDef",
+    "PurchaseHostReservationRequestRequestTypeDef",
+    "StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
+    "StartNetworkInsightsAnalysisRequestRequestTypeDef",
     "CreateTrafficMirrorSessionResultTypeDef",
     "DescribeTrafficMirrorSessionsResultTypeDef",
     "ModifyTrafficMirrorSessionResultTypeDef",
     "CreateTrafficMirrorTargetResultTypeDef",
     "DescribeTrafficMirrorTargetsResultTypeDef",
     "CreateTransitGatewayPolicyTableResultTypeDef",
     "DeleteTransitGatewayPolicyTableResultTypeDef",
@@ -2025,35 +2101,36 @@
     "NetworkInterfaceAttachmentTypeDef",
     "DhcpOptionsTypeDef",
     "DescribeClientVpnAuthorizationRulesResultTypeDef",
     "DescribeAvailabilityZonesResultTypeDef",
     "HostTypeDef",
     "StorageTypeDef",
     "CreateImageRequestInstanceCreateImageTypeDef",
+    "CreateImageRequestRequestTypeDef",
     "ImageAttributeTypeDef",
     "ImageTypeDef",
     "RegisterImageRequestRequestTypeDef",
     "RegisterImageRequestServiceResourceRegisterImageTypeDef",
     "CancelCapacityReservationFleetsResultTypeDef",
     "CancelSpotFleetRequestsResponseTypeDef",
     "CreateCapacityReservationResultTypeDef",
     "DescribeCapacityReservationsResultTypeDef",
     "DescribeCapacityReservationFleetsResultTypeDef",
     "ModifyInstanceCapacityReservationAttributesRequestRequestTypeDef",
     "DescribeClassicLinkInstancesResultTypeDef",
+    "CreateClientVpnEndpointRequestRequestTypeDef",
     "ClientVpnEndpointTypeDef",
     "DescribeClientVpnConnectionsResultTypeDef",
     "TerminateClientVpnConnectionsResultTypeDef",
     "DescribeClientVpnRoutesResultTypeDef",
     "ModifyVpnTunnelOptionsSpecificationTypeDef",
     "VpnTunnelOptionsSpecificationTypeDef",
     "TunnelOptionTypeDef",
     "NetworkAclTypeDef",
     "LaunchSpecificationTypeDef",
-    "InstanceNetworkInterfaceSpecificationUnionTypeDef",
     "RequestSpotLaunchSpecificationTypeDef",
     "ModifySnapshotAttributeRequestRequestTypeDef",
     "ModifySnapshotAttributeRequestSnapshotModifyAttributeTypeDef",
     "GetAwsNetworkPerformanceDataResultTypeDef",
     "DeleteFleetsResultTypeDef",
     "DeleteLaunchTemplateVersionsResultTypeDef",
     "DeleteQueuedReservedInstancesResultTypeDef",
@@ -2091,42 +2168,45 @@
     "GpuInfoTypeDef",
     "AssociateIamInstanceProfileResultTypeDef",
     "DescribeIamInstanceProfileAssociationsResultTypeDef",
     "DisassociateIamInstanceProfileResultTypeDef",
     "ReplaceIamInstanceProfileAssociationResultTypeDef",
     "ModifyImageAttributeRequestImageModifyAttributeTypeDef",
     "ModifyImageAttributeRequestRequestTypeDef",
-    "CreateLocalGatewayRouteTableResultTypeDef",
-    "DeleteLocalGatewayRouteTableResultTypeDef",
-    "DescribeLocalGatewayRouteTablesResultTypeDef",
+    "ImportImageRequestRequestTypeDef",
+    "ImportSnapshotRequestRequestTypeDef",
     "ImportInstanceRequestRequestTypeDef",
     "MonitorInstancesResultTypeDef",
     "UnmonitorInstancesResultTypeDef",
     "InstanceNetworkInterfaceTypeDef",
-    "FleetLaunchTemplateOverridesTypeDef",
-    "LaunchTemplateOverridesOutputTypeDef",
-    "SpotFleetLaunchSpecificationOutputTypeDef",
-    "LaunchTemplateOverridesTypeDef",
-    "SpotFleetLaunchSpecificationTypeDef",
     "FleetLaunchTemplateOverridesRequestTypeDef",
     "GetInstanceTypesFromInstanceRequirementsRequestGetInstanceTypesFromInstanceRequirementsPaginateTypeDef",
     "GetInstanceTypesFromInstanceRequirementsRequestRequestTypeDef",
     "InstanceRequirementsWithMetadataRequestTypeDef",
+    "FleetLaunchTemplateOverridesTypeDef",
+    "LaunchTemplateOverridesTypeDef",
+    "SpotFleetLaunchSpecificationTypeDef",
     "StartInstancesResultTypeDef",
     "StopInstancesResultTypeDef",
     "TerminateInstancesResultTypeDef",
     "InstanceStatusTypeDef",
-    "RevokeSecurityGroupEgressResultTypeDef",
-    "RevokeSecurityGroupIngressResultTypeDef",
-    "SecurityGroupTypeDef",
+    "AuthorizeSecurityGroupEgressRequestRequestTypeDef",
     "AuthorizeSecurityGroupEgressRequestSecurityGroupAuthorizeEgressTypeDef",
+    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
     "AuthorizeSecurityGroupIngressRequestSecurityGroupAuthorizeIngressTypeDef",
-    "IpPermissionUnionTypeDef",
+    "RevokeSecurityGroupEgressRequestRequestTypeDef",
     "RevokeSecurityGroupEgressRequestSecurityGroupRevokeEgressTypeDef",
+    "RevokeSecurityGroupEgressResultTypeDef",
+    "RevokeSecurityGroupIngressRequestRequestTypeDef",
     "RevokeSecurityGroupIngressRequestSecurityGroupRevokeIngressTypeDef",
+    "RevokeSecurityGroupIngressResultTypeDef",
+    "SecurityGroupTypeDef",
+    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
+    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
+    "SecurityGroupVpcAddressTypeDef",
     "StaleSecurityGroupTypeDef",
     "GetIpamDiscoveredAccountsResultTypeDef",
     "GetIpamDiscoveredResourceCidrsResultTypeDef",
     "CreateIpamPoolResultTypeDef",
     "DeleteIpamPoolResultTypeDef",
     "DescribeIpamPoolsResultTypeDef",
     "ModifyIpamPoolResultTypeDef",
@@ -2151,26 +2231,26 @@
     "DescribeNatGatewaysResultTypeDef",
     "CreateNetworkInterfacePermissionResultTypeDef",
     "DescribeNetworkInterfacePermissionsResultTypeDef",
     "CreateVerifiedAccessTrustProviderResultTypeDef",
     "DeleteVerifiedAccessTrustProviderResultTypeDef",
     "DescribeVerifiedAccessTrustProvidersResultTypeDef",
     "ModifyVerifiedAccessTrustProviderResultTypeDef",
+    "CreateNetworkInsightsPathRequestRequestTypeDef",
     "AccessScopePathRequestTypeDef",
     "AccessScopePathTypeDef",
     "CancelReservedInstancesListingResultTypeDef",
     "CreateReservedInstancesListingResultTypeDef",
     "DescribeReservedInstancesListingsResultTypeDef",
     "DescribePublicIpv4PoolsResultTypeDef",
     "DescribeReservedInstancesOfferingsResultTypeDef",
     "DescribeReservedInstancesResultTypeDef",
     "AuthorizeSecurityGroupEgressResultTypeDef",
     "AuthorizeSecurityGroupIngressResultTypeDef",
     "DescribeSecurityGroupRulesResultTypeDef",
-    "BundleTaskTypeDef",
     "DescribeScheduledInstanceAvailabilityResultTypeDef",
     "DescribeScheduledInstancesResultTypeDef",
     "PurchaseScheduledInstancesResultTypeDef",
     "ScheduledInstancesLaunchSpecificationTypeDef",
     "CreateVpcEndpointResultTypeDef",
     "DescribeVpcEndpointsResultTypeDef",
     "ModifySecurityGroupRulesRequestRequestTypeDef",
@@ -2188,15 +2268,14 @@
     "AssociateTransitGatewayMulticastDomainResultTypeDef",
     "DisassociateTransitGatewayMulticastDomainResultTypeDef",
     "RejectTransitGatewayMulticastDomainAssociationsResultTypeDef",
     "AssociateSubnetCidrBlockResultTypeDef",
     "DisassociateSubnetCidrBlockResultTypeDef",
     "SubnetTypeDef",
     "GetReservedInstancesExchangeQuoteResultTypeDef",
-    "LoadBalancersConfigOutputTypeDef",
     "LoadBalancersConfigTypeDef",
     "CreateTrafficMirrorFilterRuleResultTypeDef",
     "ModifyTrafficMirrorFilterRuleResultTypeDef",
     "TrafficMirrorFilterTypeDef",
     "DescribeTransitGatewayAttachmentsResultTypeDef",
     "TransitGatewayConnectPeerTypeDef",
     "CreateTransitGatewayConnectResultTypeDef",
@@ -2254,161 +2333,68 @@
     "ModifyVerifiedAccessInstanceLoggingConfigurationRequestRequestTypeDef",
     "DescribeVolumesResultTypeDef",
     "VolumeStatusItemTypeDef",
     "AssociateVpcCidrBlockResultTypeDef",
     "DisassociateVpcCidrBlockResultTypeDef",
     "VpcTypeDef",
     "VpcPeeringConnectionTypeDef",
+    "CreateLocalGatewayRouteTableResultTypeDef",
+    "DeleteLocalGatewayRouteTableResultTypeDef",
+    "DescribeLocalGatewayRouteTablesResultTypeDef",
     "AssociateInstanceEventWindowResultTypeDef",
     "CreateInstanceEventWindowResultTypeDef",
     "DescribeInstanceEventWindowsResultTypeDef",
     "DisassociateInstanceEventWindowResultTypeDef",
     "ModifyInstanceEventWindowResultTypeDef",
-    "AcceptAddressTransferRequestRequestTypeDef",
-    "AllocateAddressRequestRequestTypeDef",
-    "AllocateHostsRequestRequestTypeDef",
-    "AssociateIpamResourceDiscoveryRequestRequestTypeDef",
-    "CopySnapshotRequestRequestTypeDef",
-    "CreateCapacityReservationFleetRequestRequestTypeDef",
-    "CreateCapacityReservationRequestRequestTypeDef",
-    "CreateCarrierGatewayRequestRequestTypeDef",
-    "CreateClientVpnEndpointRequestRequestTypeDef",
-    "CreateCoipPoolRequestRequestTypeDef",
-    "CreateCustomerGatewayRequestRequestTypeDef",
-    "CreateDhcpOptionsRequestRequestTypeDef",
-    "CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
-    "CreateEgressOnlyInternetGatewayRequestRequestTypeDef",
-    "CreateFlowLogsRequestRequestTypeDef",
-    "CreateFpgaImageRequestRequestTypeDef",
-    "CreateImageRequestRequestTypeDef",
-    "CreateInstanceConnectEndpointRequestRequestTypeDef",
-    "CreateInstanceEventWindowRequestRequestTypeDef",
-    "CreateInstanceExportTaskRequestRequestTypeDef",
-    "CreateInternetGatewayRequestRequestTypeDef",
-    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
-    "CreateIpamPoolRequestRequestTypeDef",
-    "CreateIpamRequestRequestTypeDef",
-    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
-    "CreateIpamScopeRequestRequestTypeDef",
-    "CreateKeyPairRequestRequestTypeDef",
-    "CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
-    "CreateLocalGatewayRouteTableRequestRequestTypeDef",
-    "CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
-    "CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
-    "CreateManagedPrefixListRequestRequestTypeDef",
-    "CreateNatGatewayRequestRequestTypeDef",
-    "CreateNetworkAclRequestRequestTypeDef",
-    "CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
-    "CreateNetworkInsightsPathRequestRequestTypeDef",
-    "CreateNetworkInterfaceRequestRequestTypeDef",
-    "CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
-    "CreatePlacementGroupRequestRequestTypeDef",
-    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
-    "CreatePublicIpv4PoolRequestRequestTypeDef",
-    "CreateReplaceRootVolumeTaskRequestRequestTypeDef",
-    "CreateRestoreImageTaskRequestRequestTypeDef",
-    "CreateRouteTableRequestRequestTypeDef",
-    "CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
-    "CreateSecurityGroupRequestRequestTypeDef",
-    "CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
-    "CreateSnapshotRequestRequestTypeDef",
-    "CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
-    "CreateSnapshotsRequestRequestTypeDef",
-    "CreateSubnetCidrReservationRequestRequestTypeDef",
-    "CreateSubnetRequestRequestTypeDef",
-    "CreateSubnetRequestServiceResourceCreateSubnetTypeDef",
-    "CreateTrafficMirrorFilterRequestRequestTypeDef",
-    "CreateTrafficMirrorSessionRequestRequestTypeDef",
-    "CreateTrafficMirrorTargetRequestRequestTypeDef",
-    "CreateTransitGatewayConnectPeerRequestRequestTypeDef",
-    "CreateTransitGatewayConnectRequestRequestTypeDef",
-    "CreateTransitGatewayMulticastDomainRequestRequestTypeDef",
-    "CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
-    "CreateTransitGatewayPolicyTableRequestRequestTypeDef",
-    "CreateTransitGatewayRequestRequestTypeDef",
-    "CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
-    "CreateTransitGatewayRouteTableRequestRequestTypeDef",
-    "CreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
-    "CreateVerifiedAccessEndpointRequestRequestTypeDef",
-    "CreateVerifiedAccessGroupRequestRequestTypeDef",
-    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
-    "CreateVerifiedAccessTrustProviderRequestRequestTypeDef",
-    "CreateVolumeRequestRequestTypeDef",
-    "CreateVolumeRequestServiceResourceCreateVolumeTypeDef",
-    "CreateVpcEndpointRequestRequestTypeDef",
-    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
-    "CreateVpcPeeringConnectionRequestRequestTypeDef",
-    "CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
-    "CreateVpcRequestRequestTypeDef",
-    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
-    "CreateVpnGatewayRequestRequestTypeDef",
-    "ExportImageRequestRequestTypeDef",
-    "ImportImageRequestRequestTypeDef",
-    "ImportKeyPairRequestRequestTypeDef",
-    "ImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
-    "ImportSnapshotRequestRequestTypeDef",
-    "ProvisionByoipCidrRequestRequestTypeDef",
-    "PurchaseHostReservationRequestRequestTypeDef",
-    "StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
-    "StartNetworkInsightsAnalysisRequestRequestTypeDef",
     "PathComponentTypeDef",
     "CreateRouteTableResultTypeDef",
     "DescribeRouteTablesResultTypeDef",
     "GetFlowLogsIntegrationTemplateRequestRequestTypeDef",
     "RequestLaunchTemplateDataTypeDef",
+    "RunInstancesRequestRequestTypeDef",
+    "RunInstancesRequestServiceResourceCreateInstancesTypeDef",
     "RunInstancesRequestSubnetCreateInstancesTypeDef",
     "DescribeNetworkInterfaceAttributeResultTypeDef",
     "NetworkInterfaceTypeDef",
     "CreateDhcpOptionsResultTypeDef",
     "DescribeDhcpOptionsResultTypeDef",
     "DescribeHostsResultTypeDef",
     "BundleInstanceRequestRequestTypeDef",
-    "StorageUnionTypeDef",
+    "BundleTaskTypeDef",
     "DescribeImagesResultTypeDef",
     "DescribeClientVpnEndpointsResultTypeDef",
     "ModifyVpnTunnelOptionsRequestRequestTypeDef",
     "VpnConnectionOptionsSpecificationTypeDef",
     "VpnConnectionOptionsTypeDef",
     "CreateNetworkAclResultTypeDef",
     "DescribeNetworkAclsResultTypeDef",
     "SpotInstanceRequestTypeDef",
-    "RunInstancesRequestRequestTypeDef",
-    "RunInstancesRequestServiceResourceCreateInstancesTypeDef",
     "RequestSpotInstancesRequestRequestTypeDef",
     "DisableFastSnapshotRestoresResultTypeDef",
     "ConversionTaskTypeDef",
     "EnableFastSnapshotRestoresResultTypeDef",
     "CreateNetworkInsightsPathResultTypeDef",
     "DescribeNetworkInsightsPathsResultTypeDef",
     "InstanceTypeInfoTypeDef",
     "InstanceTypeDef",
-    "FleetLaunchTemplateConfigTypeDef",
-    "LaunchTemplateAndOverridesResponseTypeDef",
-    "LaunchTemplateConfigOutputTypeDef",
-    "LaunchTemplateConfigTypeDef",
     "FleetLaunchTemplateConfigRequestTypeDef",
     "GetSpotPlacementScoresRequestGetSpotPlacementScoresPaginateTypeDef",
     "GetSpotPlacementScoresRequestRequestTypeDef",
+    "FleetLaunchTemplateConfigTypeDef",
+    "LaunchTemplateAndOverridesResponseTypeDef",
+    "LaunchTemplateConfigTypeDef",
     "DescribeInstanceStatusResultTypeDef",
     "DescribeSecurityGroupsResultTypeDef",
-    "AuthorizeSecurityGroupEgressRequestRequestTypeDef",
-    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
-    "RevokeSecurityGroupEgressRequestRequestTypeDef",
-    "RevokeSecurityGroupIngressRequestRequestTypeDef",
-    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
-    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
+    "DescribeSecurityGroupsResultVpcAddressTypeDef",
     "DescribeStaleSecurityGroupsResultTypeDef",
     "GetLaunchTemplateDataResultTypeDef",
     "LaunchTemplateVersionTypeDef",
     "DescribeReservedInstancesModificationsResultTypeDef",
     "CreateNetworkInsightsAccessScopeRequestRequestTypeDef",
     "NetworkInsightsAccessScopeContentTypeDef",
-    "BundleInstanceResultTypeDef",
-    "CancelBundleTaskResultTypeDef",
-    "DescribeBundleTasksResultTypeDef",
     "RunScheduledInstancesRequestRequestTypeDef",
     "DescribeImportImageTasksResultTypeDef",
     "DescribeImportSnapshotTasksResultTypeDef",
     "CreateDefaultSubnetResultTypeDef",
     "CreateSubnetResultTypeDef",
     "DescribeSubnetsResultTypeDef",
     "CreateTrafficMirrorFilterResultTypeDef",
@@ -2428,33 +2414,36 @@
     "DescribeVpcPeeringConnectionsResultTypeDef",
     "AccessScopeAnalysisFindingTypeDef",
     "NetworkInsightsAnalysisTypeDef",
     "CreateLaunchTemplateRequestRequestTypeDef",
     "CreateLaunchTemplateVersionRequestRequestTypeDef",
     "CreateNetworkInterfaceResultTypeDef",
     "DescribeNetworkInterfacesResultTypeDef",
+    "BundleInstanceResultTypeDef",
+    "CancelBundleTaskResultTypeDef",
+    "DescribeBundleTasksResultTypeDef",
     "CreateVpnConnectionRequestRequestTypeDef",
     "VpnConnectionTypeDef",
     "DescribeSpotInstanceRequestsResultTypeDef",
     "RequestSpotInstancesResultTypeDef",
     "DescribeConversionTasksResultTypeDef",
     "ImportInstanceResultTypeDef",
     "ImportVolumeResultTypeDef",
     "DescribeInstanceTypesResultTypeDef",
     "ReservationResponseTypeDef",
     "ReservationTypeDef",
+    "CreateFleetRequestRequestTypeDef",
+    "ModifyFleetRequestRequestTypeDef",
     "CreateFleetErrorTypeDef",
     "CreateFleetInstanceTypeDef",
     "DescribeFleetErrorTypeDef",
     "DescribeFleetsInstancesTypeDef",
-    "SpotFleetRequestConfigDataOutputTypeDef",
-    "LaunchTemplateConfigUnionTypeDef",
+    "ModifySpotFleetRequestRequestRequestTypeDef",
     "SpotFleetRequestConfigDataTypeDef",
-    "CreateFleetRequestRequestTypeDef",
-    "ModifyFleetRequestRequestTypeDef",
+    "SpotFleetRequestConfigDataVpcAddressTypeDef",
     "CreateLaunchTemplateVersionResultTypeDef",
     "DescribeLaunchTemplateVersionsResultTypeDef",
     "CreateNetworkInsightsAccessScopeResultTypeDef",
     "GetNetworkInsightsAccessScopeContentResultTypeDef",
     "DescribeVerifiedAccessInstanceLoggingConfigurationsResultTypeDef",
     "ModifyVerifiedAccessInstanceLoggingConfigurationResultTypeDef",
     "GetNetworkInsightsAccessScopeAnalysisFindingsResultTypeDef",
@@ -2465,20 +2454,20 @@
     "ModifyVpnConnectionOptionsResultTypeDef",
     "ModifyVpnConnectionResultTypeDef",
     "ModifyVpnTunnelCertificateResultTypeDef",
     "ModifyVpnTunnelOptionsResultTypeDef",
     "DescribeInstancesResultTypeDef",
     "CreateFleetResultTypeDef",
     "FleetDataTypeDef",
-    "SpotFleetRequestConfigTypeDef",
-    "ModifySpotFleetRequestRequestRequestTypeDef",
     "RequestSpotFleetRequestRequestTypeDef",
-    "SpotFleetRequestConfigDataUnionTypeDef",
+    "SpotFleetRequestConfigTypeDef",
+    "SpotFleetRequestConfigVpcAddressTypeDef",
     "DescribeFleetsResultTypeDef",
     "DescribeSpotFleetRequestsResponseTypeDef",
+    "DescribeSpotFleetRequestsResponseVpcAddressTypeDef",
 )
 
 AcceleratorCountRequestTypeDef = TypedDict(
     "AcceleratorCountRequestTypeDef",
     {
         "Min": int,
         "Max": int,
@@ -9685,23 +9674,14 @@
         "Description": str,
         "RecycleBinEnterTime": datetime,
         "RecycleBinExitTime": datetime,
     },
     total=False,
 )
 
-StateReasonTypeDef = TypedDict(
-    "StateReasonTypeDef",
-    {
-        "Code": str,
-        "Message": str,
-    },
-    total=False,
-)
-
 _RequiredImportClientVpnClientCertificateRevocationListRequestRequestTypeDef = TypedDict(
     "_RequiredImportClientVpnClientCertificateRevocationListRequestRequestTypeDef",
     {
         "ClientVpnEndpointId": str,
         "CertificateRevocationList": str,
     },
 )
@@ -9887,140 +9867,140 @@
         "DeviceIndex": int,
         "Status": AttachmentStatusType,
         "NetworkCardIndex": int,
     },
     total=False,
 )
 
-MemoryGiBPerVCpuTypeDef = TypedDict(
-    "MemoryGiBPerVCpuTypeDef",
+MemoryGiBPerVCpuRequestTypeDef = TypedDict(
+    "MemoryGiBPerVCpuRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-MemoryMiBTypeDef = TypedDict(
-    "MemoryMiBTypeDef",
+_RequiredMemoryMiBRequestTypeDef = TypedDict(
+    "_RequiredMemoryMiBRequestTypeDef",
     {
         "Min": int,
+    },
+)
+_OptionalMemoryMiBRequestTypeDef = TypedDict(
+    "_OptionalMemoryMiBRequestTypeDef",
+    {
         "Max": int,
     },
     total=False,
 )
 
-NetworkBandwidthGbpsTypeDef = TypedDict(
-    "NetworkBandwidthGbpsTypeDef",
+class MemoryMiBRequestTypeDef(_RequiredMemoryMiBRequestTypeDef, _OptionalMemoryMiBRequestTypeDef):
+    pass
+
+NetworkBandwidthGbpsRequestTypeDef = TypedDict(
+    "NetworkBandwidthGbpsRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-NetworkInterfaceCountTypeDef = TypedDict(
-    "NetworkInterfaceCountTypeDef",
+NetworkInterfaceCountRequestTypeDef = TypedDict(
+    "NetworkInterfaceCountRequestTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
 )
 
-TotalLocalStorageGBTypeDef = TypedDict(
-    "TotalLocalStorageGBTypeDef",
+TotalLocalStorageGBRequestTypeDef = TypedDict(
+    "TotalLocalStorageGBRequestTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-VCpuCountRangeTypeDef = TypedDict(
-    "VCpuCountRangeTypeDef",
+_RequiredVCpuCountRangeRequestTypeDef = TypedDict(
+    "_RequiredVCpuCountRangeRequestTypeDef",
     {
         "Min": int,
+    },
+)
+_OptionalVCpuCountRangeRequestTypeDef = TypedDict(
+    "_OptionalVCpuCountRangeRequestTypeDef",
+    {
         "Max": int,
     },
     total=False,
 )
 
-MemoryGiBPerVCpuRequestTypeDef = TypedDict(
-    "MemoryGiBPerVCpuRequestTypeDef",
+class VCpuCountRangeRequestTypeDef(
+    _RequiredVCpuCountRangeRequestTypeDef, _OptionalVCpuCountRangeRequestTypeDef
+):
+    pass
+
+MemoryGiBPerVCpuTypeDef = TypedDict(
+    "MemoryGiBPerVCpuTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-_RequiredMemoryMiBRequestTypeDef = TypedDict(
-    "_RequiredMemoryMiBRequestTypeDef",
+MemoryMiBTypeDef = TypedDict(
+    "MemoryMiBTypeDef",
     {
         "Min": int,
-    },
-)
-_OptionalMemoryMiBRequestTypeDef = TypedDict(
-    "_OptionalMemoryMiBRequestTypeDef",
-    {
         "Max": int,
     },
     total=False,
 )
 
-class MemoryMiBRequestTypeDef(_RequiredMemoryMiBRequestTypeDef, _OptionalMemoryMiBRequestTypeDef):
-    pass
-
-NetworkBandwidthGbpsRequestTypeDef = TypedDict(
-    "NetworkBandwidthGbpsRequestTypeDef",
+NetworkBandwidthGbpsTypeDef = TypedDict(
+    "NetworkBandwidthGbpsTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-NetworkInterfaceCountRequestTypeDef = TypedDict(
-    "NetworkInterfaceCountRequestTypeDef",
+NetworkInterfaceCountTypeDef = TypedDict(
+    "NetworkInterfaceCountTypeDef",
     {
         "Min": int,
         "Max": int,
     },
     total=False,
 )
 
-TotalLocalStorageGBRequestTypeDef = TypedDict(
-    "TotalLocalStorageGBRequestTypeDef",
+TotalLocalStorageGBTypeDef = TypedDict(
+    "TotalLocalStorageGBTypeDef",
     {
         "Min": float,
         "Max": float,
     },
     total=False,
 )
 
-_RequiredVCpuCountRangeRequestTypeDef = TypedDict(
-    "_RequiredVCpuCountRangeRequestTypeDef",
+VCpuCountRangeTypeDef = TypedDict(
+    "VCpuCountRangeTypeDef",
     {
         "Min": int,
-    },
-)
-_OptionalVCpuCountRangeRequestTypeDef = TypedDict(
-    "_OptionalVCpuCountRangeRequestTypeDef",
-    {
         "Max": int,
     },
     total=False,
 )
 
-class VCpuCountRangeRequestTypeDef(
-    _RequiredVCpuCountRangeRequestTypeDef, _OptionalVCpuCountRangeRequestTypeDef
-):
-    pass
-
 InstanceStateTypeDef = TypedDict(
     "InstanceStateTypeDef",
     {
         "Code": int,
         "Name": InstanceStateNameType,
     },
     total=False,
@@ -12678,26 +12658,14 @@
         "State": RouteStateType,
         "VpcPeeringConnectionId": str,
         "CoreNetworkArn": str,
     },
     total=False,
 )
 
-S3StorageOutputTypeDef = TypedDict(
-    "S3StorageOutputTypeDef",
-    {
-        "AWSAccessKeyId": str,
-        "Bucket": str,
-        "Prefix": str,
-        "UploadPolicy": bytes,
-        "UploadPolicySignature": str,
-    },
-    total=False,
-)
-
 ScheduledInstanceRecurrenceTypeDef = TypedDict(
     "ScheduledInstanceRecurrenceTypeDef",
     {
         "Frequency": str,
         "Interval": int,
         "OccurrenceDaySet": List[int],
         "OccurrenceRelativeToEnd": bool,
@@ -14590,14 +14558,23 @@
     {
         "Code": str,
         "Message": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+StateReasonTypeDef = TypedDict(
+    "StateReasonTypeDef",
+    {
+        "Code": str,
+        "Message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UnassignIpv6AddressesResultTypeDef = TypedDict(
     "UnassignIpv6AddressesResultTypeDef",
     {
         "NetworkInterfaceId": str,
         "UnassignedIpv6Addresses": List[str],
         "UnassignedIpv6Prefixes": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -15339,28 +15316,19 @@
         "Tags": List[TagTypeDef],
         "StorageTier": StorageTierType,
         "RestoreExpiryTime": datetime,
     },
     total=False,
 )
 
-SpotFleetTagSpecificationOutputTypeDef = TypedDict(
-    "SpotFleetTagSpecificationOutputTypeDef",
-    {
-        "ResourceType": ResourceTypeType,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
 SpotFleetTagSpecificationTypeDef = TypedDict(
     "SpotFleetTagSpecificationTypeDef",
     {
         "ResourceType": ResourceTypeType,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 SubnetCidrReservationTypeDef = TypedDict(
     "SubnetCidrReservationTypeDef",
     {
@@ -15371,28 +15339,28 @@
         "OwnerId": str,
         "Description": str,
         "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-TagSpecificationOutputTypeDef = TypedDict(
-    "TagSpecificationOutputTypeDef",
+TagSpecificationTypeDef = TypedDict(
+    "TagSpecificationTypeDef",
     {
         "ResourceType": ResourceTypeType,
-        "Tags": List[TagTypeDef],
+        "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-TagSpecificationTypeDef = TypedDict(
-    "TagSpecificationTypeDef",
+TagSpecificationVpcAddressTypeDef = TypedDict(
+    "TagSpecificationVpcAddressTypeDef",
     {
         "ResourceType": ResourceTypeType,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 TrafficMirrorSessionTypeDef = TypedDict(
     "TrafficMirrorSessionTypeDef",
     {
@@ -16540,26 +16508,18 @@
         "InstanceId": str,
         "Tags": List[TagTypeDef],
         "VpcId": str,
     },
     total=False,
 )
 
-ClassicLoadBalancersConfigOutputTypeDef = TypedDict(
-    "ClassicLoadBalancersConfigOutputTypeDef",
-    {
-        "ClassicLoadBalancers": List[ClassicLoadBalancerTypeDef],
-    },
-    total=False,
-)
-
 ClassicLoadBalancersConfigTypeDef = TypedDict(
     "ClassicLoadBalancersConfigTypeDef",
     {
-        "ClassicLoadBalancers": Sequence[ClassicLoadBalancerTypeDef],
+        "ClassicLoadBalancers": List[ClassicLoadBalancerTypeDef],
     },
     total=False,
 )
 
 ExportClientVpnClientCertificateRevocationListResultTypeDef = TypedDict(
     "ExportClientVpnClientCertificateRevocationListResultTypeDef",
     {
@@ -16944,42 +16904,42 @@
 
 class ReplaceNetworkAclEntryRequestRequestTypeDef(
     _RequiredReplaceNetworkAclEntryRequestRequestTypeDef,
     _OptionalReplaceNetworkAclEntryRequestRequestTypeDef,
 ):
     pass
 
-InstanceNetworkInterfaceSpecificationOutputTypeDef = TypedDict(
-    "InstanceNetworkInterfaceSpecificationOutputTypeDef",
+InstanceNetworkInterfaceSpecificationServiceResourceTypeDef = TypedDict(
+    "InstanceNetworkInterfaceSpecificationServiceResourceTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "DeleteOnTermination": bool,
         "Description": str,
         "DeviceIndex": int,
-        "Groups": List[str],
+        "Groups": Sequence[str],
         "Ipv6AddressCount": int,
-        "Ipv6Addresses": List[InstanceIpv6AddressTypeDef],
+        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
         "NetworkInterfaceId": str,
         "PrivateIpAddress": str,
-        "PrivateIpAddresses": List[PrivateIpAddressSpecificationTypeDef],
+        "PrivateIpAddresses": Sequence[PrivateIpAddressSpecificationTypeDef],
         "SecondaryPrivateIpAddressCount": int,
         "SubnetId": str,
         "AssociateCarrierIpAddress": bool,
         "InterfaceType": str,
         "NetworkCardIndex": int,
-        "Ipv4Prefixes": List[Ipv4PrefixSpecificationRequestTypeDef],
+        "Ipv4Prefixes": Sequence[Ipv4PrefixSpecificationRequestTypeDef],
         "Ipv4PrefixCount": int,
-        "Ipv6Prefixes": List[Ipv6PrefixSpecificationRequestTypeDef],
+        "Ipv6Prefixes": Sequence[Ipv6PrefixSpecificationRequestTypeDef],
         "Ipv6PrefixCount": int,
     },
     total=False,
 )
 
-InstanceNetworkInterfaceSpecificationTypeDef = TypedDict(
-    "InstanceNetworkInterfaceSpecificationTypeDef",
+InstanceNetworkInterfaceSpecificationSubnetTypeDef = TypedDict(
+    "InstanceNetworkInterfaceSpecificationSubnetTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "DeleteOnTermination": bool,
         "Description": str,
         "DeviceIndex": int,
         "Groups": Sequence[str],
         "Ipv6AddressCount": int,
@@ -16996,14 +16956,40 @@
         "Ipv4PrefixCount": int,
         "Ipv6Prefixes": Sequence[Ipv6PrefixSpecificationRequestTypeDef],
         "Ipv6PrefixCount": int,
     },
     total=False,
 )
 
+InstanceNetworkInterfaceSpecificationTypeDef = TypedDict(
+    "InstanceNetworkInterfaceSpecificationTypeDef",
+    {
+        "AssociatePublicIpAddress": bool,
+        "DeleteOnTermination": bool,
+        "Description": str,
+        "DeviceIndex": int,
+        "Groups": List[str],
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": List[InstanceIpv6AddressTypeDef],
+        "NetworkInterfaceId": str,
+        "PrivateIpAddress": str,
+        "PrivateIpAddresses": List[PrivateIpAddressSpecificationTypeDef],
+        "SecondaryPrivateIpAddressCount": int,
+        "SubnetId": str,
+        "AssociateCarrierIpAddress": bool,
+        "InterfaceType": str,
+        "NetworkCardIndex": int,
+        "Ipv4Prefixes": List[Ipv4PrefixSpecificationRequestTypeDef],
+        "Ipv4PrefixCount": int,
+        "Ipv6Prefixes": List[Ipv6PrefixSpecificationRequestTypeDef],
+        "Ipv6PrefixCount": int,
+    },
+    total=False,
+)
+
 CreateReservedInstancesListingRequestRequestTypeDef = TypedDict(
     "CreateReservedInstancesListingRequestRequestTypeDef",
     {
         "ClientToken": str,
         "InstanceCount": int,
         "PriceSchedules": Sequence[PriceScheduleSpecificationTypeDef],
         "ReservedInstancesId": str,
@@ -22279,30 +22265,14 @@
     {
         "Images": List[ImageRecycleBinInfoTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LocalGatewayRouteTableTypeDef = TypedDict(
-    "LocalGatewayRouteTableTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-        "LocalGatewayRouteTableArn": str,
-        "LocalGatewayId": str,
-        "OutpostArn": str,
-        "OwnerId": str,
-        "State": str,
-        "Tags": List[TagTypeDef],
-        "Mode": LocalGatewayRouteTableModeType,
-        "StateReason": StateReasonTypeDef,
-    },
-    total=False,
-)
-
 ImportInstanceLaunchSpecificationTypeDef = TypedDict(
     "ImportInstanceLaunchSpecificationTypeDef",
     {
         "AdditionalInfo": str,
         "Architecture": ArchitectureValuesType,
         "GroupIds": Sequence[str],
         "GroupNames": Sequence[str],
@@ -22397,74 +22367,14 @@
         "Primary": bool,
         "PrivateDnsName": str,
         "PrivateIpAddress": str,
     },
     total=False,
 )
 
-InstanceRequirementsOutputTypeDef = TypedDict(
-    "InstanceRequirementsOutputTypeDef",
-    {
-        "VCpuCount": VCpuCountRangeTypeDef,
-        "MemoryMiB": MemoryMiBTypeDef,
-        "CpuManufacturers": List[CpuManufacturerType],
-        "MemoryGiBPerVCpu": MemoryGiBPerVCpuTypeDef,
-        "ExcludedInstanceTypes": List[str],
-        "InstanceGenerations": List[InstanceGenerationType],
-        "SpotMaxPricePercentageOverLowestPrice": int,
-        "OnDemandMaxPricePercentageOverLowestPrice": int,
-        "BareMetal": BareMetalType,
-        "BurstablePerformance": BurstablePerformanceType,
-        "RequireHibernateSupport": bool,
-        "NetworkInterfaceCount": NetworkInterfaceCountTypeDef,
-        "LocalStorage": LocalStorageType,
-        "LocalStorageTypes": List[LocalStorageTypeType],
-        "TotalLocalStorageGB": TotalLocalStorageGBTypeDef,
-        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsTypeDef,
-        "AcceleratorTypes": List[AcceleratorTypeType],
-        "AcceleratorCount": AcceleratorCountTypeDef,
-        "AcceleratorManufacturers": List[AcceleratorManufacturerType],
-        "AcceleratorNames": List[AcceleratorNameType],
-        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBTypeDef,
-        "NetworkBandwidthGbps": NetworkBandwidthGbpsTypeDef,
-        "AllowedInstanceTypes": List[str],
-    },
-    total=False,
-)
-
-InstanceRequirementsTypeDef = TypedDict(
-    "InstanceRequirementsTypeDef",
-    {
-        "VCpuCount": VCpuCountRangeTypeDef,
-        "MemoryMiB": MemoryMiBTypeDef,
-        "CpuManufacturers": Sequence[CpuManufacturerType],
-        "MemoryGiBPerVCpu": MemoryGiBPerVCpuTypeDef,
-        "ExcludedInstanceTypes": Sequence[str],
-        "InstanceGenerations": Sequence[InstanceGenerationType],
-        "SpotMaxPricePercentageOverLowestPrice": int,
-        "OnDemandMaxPricePercentageOverLowestPrice": int,
-        "BareMetal": BareMetalType,
-        "BurstablePerformance": BurstablePerformanceType,
-        "RequireHibernateSupport": bool,
-        "NetworkInterfaceCount": NetworkInterfaceCountTypeDef,
-        "LocalStorage": LocalStorageType,
-        "LocalStorageTypes": Sequence[LocalStorageTypeType],
-        "TotalLocalStorageGB": TotalLocalStorageGBTypeDef,
-        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsTypeDef,
-        "AcceleratorTypes": Sequence[AcceleratorTypeType],
-        "AcceleratorCount": AcceleratorCountTypeDef,
-        "AcceleratorManufacturers": Sequence[AcceleratorManufacturerType],
-        "AcceleratorNames": Sequence[AcceleratorNameType],
-        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBTypeDef,
-        "NetworkBandwidthGbps": NetworkBandwidthGbpsTypeDef,
-        "AllowedInstanceTypes": Sequence[str],
-    },
-    total=False,
-)
-
 _RequiredInstanceRequirementsRequestTypeDef = TypedDict(
     "_RequiredInstanceRequirementsRequestTypeDef",
     {
         "VCpuCount": VCpuCountRangeRequestTypeDef,
         "MemoryMiB": MemoryMiBRequestTypeDef,
     },
 )
@@ -22497,14 +22407,44 @@
 )
 
 class InstanceRequirementsRequestTypeDef(
     _RequiredInstanceRequirementsRequestTypeDef, _OptionalInstanceRequirementsRequestTypeDef
 ):
     pass
 
+InstanceRequirementsTypeDef = TypedDict(
+    "InstanceRequirementsTypeDef",
+    {
+        "VCpuCount": VCpuCountRangeTypeDef,
+        "MemoryMiB": MemoryMiBTypeDef,
+        "CpuManufacturers": List[CpuManufacturerType],
+        "MemoryGiBPerVCpu": MemoryGiBPerVCpuTypeDef,
+        "ExcludedInstanceTypes": List[str],
+        "InstanceGenerations": List[InstanceGenerationType],
+        "SpotMaxPricePercentageOverLowestPrice": int,
+        "OnDemandMaxPricePercentageOverLowestPrice": int,
+        "BareMetal": BareMetalType,
+        "BurstablePerformance": BurstablePerformanceType,
+        "RequireHibernateSupport": bool,
+        "NetworkInterfaceCount": NetworkInterfaceCountTypeDef,
+        "LocalStorage": LocalStorageType,
+        "LocalStorageTypes": List[LocalStorageTypeType],
+        "TotalLocalStorageGB": TotalLocalStorageGBTypeDef,
+        "BaselineEbsBandwidthMbps": BaselineEbsBandwidthMbpsTypeDef,
+        "AcceleratorTypes": List[AcceleratorTypeType],
+        "AcceleratorCount": AcceleratorCountTypeDef,
+        "AcceleratorManufacturers": List[AcceleratorManufacturerType],
+        "AcceleratorNames": List[AcceleratorNameType],
+        "AcceleratorTotalMemoryMiB": AcceleratorTotalMemoryMiBTypeDef,
+        "NetworkBandwidthGbps": NetworkBandwidthGbpsTypeDef,
+        "AllowedInstanceTypes": List[str],
+    },
+    total=False,
+)
+
 InstanceStateChangeTypeDef = TypedDict(
     "InstanceStateChangeTypeDef",
     {
         "CurrentState": InstanceStateTypeDef,
         "InstanceId": str,
         "PreviousState": InstanceStateTypeDef,
     },
@@ -22524,38 +22464,38 @@
     "ModifyInstanceEventStartTimeResultTypeDef",
     {
         "Event": InstanceStatusEventTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-IpPermissionOutputTypeDef = TypedDict(
-    "IpPermissionOutputTypeDef",
+IpPermissionTypeDef = TypedDict(
+    "IpPermissionTypeDef",
     {
         "FromPort": int,
         "IpProtocol": str,
-        "IpRanges": List[IpRangeTypeDef],
-        "Ipv6Ranges": List[Ipv6RangeTypeDef],
-        "PrefixListIds": List[PrefixListIdTypeDef],
+        "IpRanges": Sequence[IpRangeTypeDef],
+        "Ipv6Ranges": Sequence[Ipv6RangeTypeDef],
+        "PrefixListIds": Sequence[PrefixListIdTypeDef],
         "ToPort": int,
-        "UserIdGroupPairs": List[UserIdGroupPairTypeDef],
+        "UserIdGroupPairs": Sequence[UserIdGroupPairTypeDef],
     },
     total=False,
 )
 
-IpPermissionTypeDef = TypedDict(
-    "IpPermissionTypeDef",
+IpPermissionVpcAddressTypeDef = TypedDict(
+    "IpPermissionVpcAddressTypeDef",
     {
         "FromPort": int,
         "IpProtocol": str,
-        "IpRanges": Sequence[IpRangeTypeDef],
-        "Ipv6Ranges": Sequence[Ipv6RangeTypeDef],
-        "PrefixListIds": Sequence[PrefixListIdTypeDef],
+        "IpRanges": List[IpRangeTypeDef],
+        "Ipv6Ranges": List[Ipv6RangeTypeDef],
+        "PrefixListIds": List[PrefixListIdTypeDef],
         "ToPort": int,
-        "UserIdGroupPairs": Sequence[UserIdGroupPairTypeDef],
+        "UserIdGroupPairs": List[UserIdGroupPairTypeDef],
     },
     total=False,
 )
 
 StaleIpPermissionTypeDef = TypedDict(
     "StaleIpPermissionTypeDef",
     {
@@ -23342,22 +23282,14 @@
     "RegisterTransitGatewayMulticastGroupSourcesResultTypeDef",
     {
         "RegisteredMulticastGroupSources": TransitGatewayMulticastRegisteredGroupSourcesTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StorageOutputTypeDef = TypedDict(
-    "StorageOutputTypeDef",
-    {
-        "S3": S3StorageOutputTypeDef,
-    },
-    total=False,
-)
-
 ScheduledInstanceAvailabilityTypeDef = TypedDict(
     "ScheduledInstanceAvailabilityTypeDef",
     {
         "AvailabilityZone": str,
         "AvailableInstanceCount": int,
         "FirstSlotStartTime": datetime,
         "HourlyPrice": str,
@@ -23619,26 +23551,18 @@
     {
         "ReservationValue": ReservationValueTypeDef,
         "TargetConfiguration": TargetConfigurationTypeDef,
     },
     total=False,
 )
 
-TargetGroupsConfigOutputTypeDef = TypedDict(
-    "TargetGroupsConfigOutputTypeDef",
-    {
-        "TargetGroups": List[TargetGroupTypeDef],
-    },
-    total=False,
-)
-
 TargetGroupsConfigTypeDef = TypedDict(
     "TargetGroupsConfigTypeDef",
     {
-        "TargetGroups": Sequence[TargetGroupTypeDef],
+        "TargetGroups": List[TargetGroupTypeDef],
     },
     total=False,
 )
 
 TrafficMirrorFilterRuleTypeDef = TypedDict(
     "TrafficMirrorFilterRuleTypeDef",
     {
@@ -24010,14 +23934,30 @@
         "PeeringOptions": VpcPeeringConnectionOptionsDescriptionTypeDef,
         "VpcId": str,
         "Region": str,
     },
     total=False,
 )
 
+LocalGatewayRouteTableTypeDef = TypedDict(
+    "LocalGatewayRouteTableTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+        "LocalGatewayRouteTableArn": str,
+        "LocalGatewayId": str,
+        "OutpostArn": str,
+        "OwnerId": str,
+        "State": str,
+        "Tags": List[TagTypeDef],
+        "Mode": LocalGatewayRouteTableModeType,
+        "StateReason": StateReasonTypeDef,
+    },
+    total=False,
+)
+
 DescribeAccountAttributesResultTypeDef = TypedDict(
     "DescribeAccountAttributesResultTypeDef",
     {
         "AccountAttributes": List[AccountAttributeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -24558,14 +24498,127 @@
         "SubnetIpv4CidrReservations": List[SubnetCidrReservationTypeDef],
         "SubnetIpv6CidrReservations": List[SubnetCidrReservationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredAcceptAddressTransferRequestRequestTypeDef = TypedDict(
+    "_RequiredAcceptAddressTransferRequestRequestTypeDef",
+    {
+        "Address": str,
+    },
+)
+_OptionalAcceptAddressTransferRequestRequestTypeDef = TypedDict(
+    "_OptionalAcceptAddressTransferRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class AcceptAddressTransferRequestRequestTypeDef(
+    _RequiredAcceptAddressTransferRequestRequestTypeDef,
+    _OptionalAcceptAddressTransferRequestRequestTypeDef,
+):
+    pass
+
+AllocateAddressRequestRequestTypeDef = TypedDict(
+    "AllocateAddressRequestRequestTypeDef",
+    {
+        "Domain": DomainTypeType,
+        "Address": str,
+        "PublicIpv4Pool": str,
+        "NetworkBorderGroup": str,
+        "CustomerOwnedIpv4Pool": str,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+_RequiredAllocateHostsRequestRequestTypeDef = TypedDict(
+    "_RequiredAllocateHostsRequestRequestTypeDef",
+    {
+        "AvailabilityZone": str,
+    },
+)
+_OptionalAllocateHostsRequestRequestTypeDef = TypedDict(
+    "_OptionalAllocateHostsRequestRequestTypeDef",
+    {
+        "AutoPlacement": AutoPlacementType,
+        "ClientToken": str,
+        "InstanceType": str,
+        "InstanceFamily": str,
+        "Quantity": int,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "HostRecovery": HostRecoveryType,
+        "OutpostArn": str,
+        "HostMaintenance": HostMaintenanceType,
+        "AssetIds": Sequence[str],
+    },
+    total=False,
+)
+
+class AllocateHostsRequestRequestTypeDef(
+    _RequiredAllocateHostsRequestRequestTypeDef, _OptionalAllocateHostsRequestRequestTypeDef
+):
+    pass
+
+_RequiredAssociateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
+    "_RequiredAssociateIpamResourceDiscoveryRequestRequestTypeDef",
+    {
+        "IpamId": str,
+        "IpamResourceDiscoveryId": str,
+    },
+)
+_OptionalAssociateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
+    "_OptionalAssociateIpamResourceDiscoveryRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class AssociateIpamResourceDiscoveryRequestRequestTypeDef(
+    _RequiredAssociateIpamResourceDiscoveryRequestRequestTypeDef,
+    _OptionalAssociateIpamResourceDiscoveryRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCopySnapshotRequestRequestTypeDef = TypedDict(
+    "_RequiredCopySnapshotRequestRequestTypeDef",
+    {
+        "SourceRegion": str,
+        "SourceSnapshotId": str,
+    },
+)
+_OptionalCopySnapshotRequestRequestTypeDef = TypedDict(
+    "_OptionalCopySnapshotRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DestinationOutpostArn": str,
+        "DestinationRegion": str,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "PresignedUrl": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CopySnapshotRequestRequestTypeDef(
+    _RequiredCopySnapshotRequestRequestTypeDef, _OptionalCopySnapshotRequestRequestTypeDef
+):
+    pass
+
 _RequiredCopySnapshotRequestSnapshotCopyTypeDef = TypedDict(
     "_RequiredCopySnapshotRequestSnapshotCopyTypeDef",
     {
         "SourceRegion": str,
     },
 )
 _OptionalCopySnapshotRequestSnapshotCopyTypeDef = TypedDict(
@@ -24584,23 +24637,698 @@
 )
 
 class CopySnapshotRequestSnapshotCopyTypeDef(
     _RequiredCopySnapshotRequestSnapshotCopyTypeDef, _OptionalCopySnapshotRequestSnapshotCopyTypeDef
 ):
     pass
 
+_RequiredCreateCapacityReservationFleetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCapacityReservationFleetRequestRequestTypeDef",
+    {
+        "InstanceTypeSpecifications": Sequence[ReservationFleetInstanceSpecificationTypeDef],
+        "TotalTargetCapacity": int,
+    },
+)
+_OptionalCreateCapacityReservationFleetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCapacityReservationFleetRequestRequestTypeDef",
+    {
+        "AllocationStrategy": str,
+        "ClientToken": str,
+        "Tenancy": Literal["default"],
+        "EndDate": TimestampTypeDef,
+        "InstanceMatchCriteria": Literal["open"],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateCapacityReservationFleetRequestRequestTypeDef(
+    _RequiredCreateCapacityReservationFleetRequestRequestTypeDef,
+    _OptionalCreateCapacityReservationFleetRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateCapacityReservationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCapacityReservationRequestRequestTypeDef",
+    {
+        "InstanceType": str,
+        "InstancePlatform": CapacityReservationInstancePlatformType,
+        "InstanceCount": int,
+    },
+)
+_OptionalCreateCapacityReservationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCapacityReservationRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "AvailabilityZone": str,
+        "AvailabilityZoneId": str,
+        "Tenancy": CapacityReservationTenancyType,
+        "EbsOptimized": bool,
+        "EphemeralStorage": bool,
+        "EndDate": TimestampTypeDef,
+        "EndDateType": EndDateTypeType,
+        "InstanceMatchCriteria": InstanceMatchCriteriaType,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "OutpostArn": str,
+        "PlacementGroupArn": str,
+    },
+    total=False,
+)
+
+class CreateCapacityReservationRequestRequestTypeDef(
+    _RequiredCreateCapacityReservationRequestRequestTypeDef,
+    _OptionalCreateCapacityReservationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateCarrierGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCarrierGatewayRequestRequestTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateCarrierGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCarrierGatewayRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class CreateCarrierGatewayRequestRequestTypeDef(
+    _RequiredCreateCarrierGatewayRequestRequestTypeDef,
+    _OptionalCreateCarrierGatewayRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateCoipPoolRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCoipPoolRequestRequestTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+    },
+)
+_OptionalCreateCoipPoolRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCoipPoolRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateCoipPoolRequestRequestTypeDef(
+    _RequiredCreateCoipPoolRequestRequestTypeDef, _OptionalCreateCoipPoolRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateCustomerGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCustomerGatewayRequestRequestTypeDef",
+    {
+        "Type": Literal["ipsec.1"],
+    },
+)
+_OptionalCreateCustomerGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCustomerGatewayRequestRequestTypeDef",
+    {
+        "BgpAsn": int,
+        "PublicIp": str,
+        "CertificateArn": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DeviceName": str,
+        "IpAddress": str,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateCustomerGatewayRequestRequestTypeDef(
+    _RequiredCreateCustomerGatewayRequestRequestTypeDef,
+    _OptionalCreateCustomerGatewayRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateDhcpOptionsRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDhcpOptionsRequestRequestTypeDef",
+    {
+        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
+    },
+)
+_OptionalCreateDhcpOptionsRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDhcpOptionsRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateDhcpOptionsRequestRequestTypeDef(
+    _RequiredCreateDhcpOptionsRequestRequestTypeDef, _OptionalCreateDhcpOptionsRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef = TypedDict(
+    "_RequiredCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
+    {
+        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
+    },
+)
+_OptionalCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef = TypedDict(
+    "_OptionalCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef(
+    _RequiredCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef,
+    _OptionalCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef,
+):
+    pass
+
+_RequiredCreateEgressOnlyInternetGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEgressOnlyInternetGatewayRequestRequestTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateEgressOnlyInternetGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEgressOnlyInternetGatewayRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class CreateEgressOnlyInternetGatewayRequestRequestTypeDef(
+    _RequiredCreateEgressOnlyInternetGatewayRequestRequestTypeDef,
+    _OptionalCreateEgressOnlyInternetGatewayRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateFlowLogsRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFlowLogsRequestRequestTypeDef",
+    {
+        "ResourceIds": Sequence[str],
+        "ResourceType": FlowLogsResourceTypeType,
+    },
+)
+_OptionalCreateFlowLogsRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFlowLogsRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "ClientToken": str,
+        "DeliverLogsPermissionArn": str,
+        "DeliverCrossAccountRole": str,
+        "LogGroupName": str,
+        "TrafficType": TrafficTypeType,
+        "LogDestinationType": LogDestinationTypeType,
+        "LogDestination": str,
+        "LogFormat": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "MaxAggregationInterval": int,
+        "DestinationOptions": DestinationOptionsRequestTypeDef,
+    },
+    total=False,
+)
+
+class CreateFlowLogsRequestRequestTypeDef(
+    _RequiredCreateFlowLogsRequestRequestTypeDef, _OptionalCreateFlowLogsRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateFpgaImageRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFpgaImageRequestRequestTypeDef",
+    {
+        "InputStorageLocation": StorageLocationTypeDef,
+    },
+)
+_OptionalCreateFpgaImageRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFpgaImageRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "LogsStorageLocation": StorageLocationTypeDef,
+        "Description": str,
+        "Name": str,
+        "ClientToken": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class CreateFpgaImageRequestRequestTypeDef(
+    _RequiredCreateFpgaImageRequestRequestTypeDef, _OptionalCreateFpgaImageRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateInstanceConnectEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInstanceConnectEndpointRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+    },
+)
+_OptionalCreateInstanceConnectEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInstanceConnectEndpointRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "SecurityGroupIds": Sequence[str],
+        "PreserveClientIp": bool,
+        "ClientToken": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class CreateInstanceConnectEndpointRequestRequestTypeDef(
+    _RequiredCreateInstanceConnectEndpointRequestRequestTypeDef,
+    _OptionalCreateInstanceConnectEndpointRequestRequestTypeDef,
+):
+    pass
+
+CreateInstanceEventWindowRequestRequestTypeDef = TypedDict(
+    "CreateInstanceEventWindowRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "Name": str,
+        "TimeRanges": Sequence[InstanceEventWindowTimeRangeRequestTypeDef],
+        "CronExpression": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateInstanceExportTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateInstanceExportTaskRequestRequestTypeDef",
+    {
+        "ExportToS3Task": ExportToS3TaskSpecificationTypeDef,
+        "InstanceId": str,
+        "TargetEnvironment": ExportEnvironmentType,
+    },
+)
+_OptionalCreateInstanceExportTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateInstanceExportTaskRequestRequestTypeDef",
+    {
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class CreateInstanceExportTaskRequestRequestTypeDef(
+    _RequiredCreateInstanceExportTaskRequestRequestTypeDef,
+    _OptionalCreateInstanceExportTaskRequestRequestTypeDef,
+):
+    pass
+
+CreateInternetGatewayRequestRequestTypeDef = TypedDict(
+    "CreateInternetGatewayRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef = TypedDict(
+    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+_RequiredCreateIpamPoolRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIpamPoolRequestRequestTypeDef",
+    {
+        "IpamScopeId": str,
+        "AddressFamily": AddressFamilyType,
+    },
+)
+_OptionalCreateIpamPoolRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIpamPoolRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "Locale": str,
+        "SourceIpamPoolId": str,
+        "Description": str,
+        "AutoImport": bool,
+        "PubliclyAdvertisable": bool,
+        "AllocationMinNetmaskLength": int,
+        "AllocationMaxNetmaskLength": int,
+        "AllocationDefaultNetmaskLength": int,
+        "AllocationResourceTags": Sequence[RequestIpamResourceTagTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+        "AwsService": Literal["ec2"],
+        "PublicIpSource": IpamPoolPublicIpSourceType,
+    },
+    total=False,
+)
+
+class CreateIpamPoolRequestRequestTypeDef(
+    _RequiredCreateIpamPoolRequestRequestTypeDef, _OptionalCreateIpamPoolRequestRequestTypeDef
+):
+    pass
+
+CreateIpamRequestRequestTypeDef = TypedDict(
+    "CreateIpamRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "Description": str,
+        "OperatingRegions": Sequence[AddIpamOperatingRegionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+CreateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
+    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "Description": str,
+        "OperatingRegions": Sequence[AddIpamOperatingRegionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+_RequiredCreateIpamScopeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateIpamScopeRequestRequestTypeDef",
+    {
+        "IpamId": str,
+    },
+)
+_OptionalCreateIpamScopeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateIpamScopeRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class CreateIpamScopeRequestRequestTypeDef(
+    _RequiredCreateIpamScopeRequestRequestTypeDef, _OptionalCreateIpamScopeRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateKeyPairRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateKeyPairRequestRequestTypeDef",
+    {
+        "KeyName": str,
+    },
+)
+_OptionalCreateKeyPairRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateKeyPairRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "KeyType": KeyTypeType,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "KeyFormat": KeyFormatType,
+    },
+    total=False,
+)
+
+class CreateKeyPairRequestRequestTypeDef(
+    _RequiredCreateKeyPairRequestRequestTypeDef, _OptionalCreateKeyPairRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef = TypedDict(
+    "_RequiredCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
+    {
+        "KeyName": str,
+    },
+)
+_OptionalCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef = TypedDict(
+    "_OptionalCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
+    {
+        "DryRun": bool,
+        "KeyType": KeyTypeType,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "KeyFormat": KeyFormatType,
+    },
+    total=False,
+)
+
+class CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef(
+    _RequiredCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef,
+    _OptionalCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef,
+):
+    pass
+
+_RequiredCreateLocalGatewayRouteTableRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLocalGatewayRouteTableRequestRequestTypeDef",
+    {
+        "LocalGatewayId": str,
+    },
+)
+_OptionalCreateLocalGatewayRouteTableRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLocalGatewayRouteTableRequestRequestTypeDef",
+    {
+        "Mode": LocalGatewayRouteTableModeType,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateLocalGatewayRouteTableRequestRequestTypeDef(
+    _RequiredCreateLocalGatewayRouteTableRequestRequestTypeDef,
+    _OptionalCreateLocalGatewayRouteTableRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+        "LocalGatewayVirtualInterfaceGroupId": str,
+    },
+)
+_OptionalCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef(
+    _RequiredCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef,
+    _OptionalCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
+    {
+        "LocalGatewayRouteTableId": str,
+        "VpcId": str,
+    },
+)
+_OptionalCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef(
+    _RequiredCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef,
+    _OptionalCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateManagedPrefixListRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateManagedPrefixListRequestRequestTypeDef",
+    {
+        "PrefixListName": str,
+        "MaxEntries": int,
+        "AddressFamily": str,
+    },
+)
+_OptionalCreateManagedPrefixListRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateManagedPrefixListRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "Entries": Sequence[AddPrefixListEntryTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class CreateManagedPrefixListRequestRequestTypeDef(
+    _RequiredCreateManagedPrefixListRequestRequestTypeDef,
+    _OptionalCreateManagedPrefixListRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateNatGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNatGatewayRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+    },
+)
+_OptionalCreateNatGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNatGatewayRequestRequestTypeDef",
+    {
+        "AllocationId": str,
+        "ClientToken": str,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ConnectivityType": ConnectivityTypeType,
+        "PrivateIpAddress": str,
+        "SecondaryAllocationIds": Sequence[str],
+        "SecondaryPrivateIpAddresses": Sequence[str],
+        "SecondaryPrivateIpAddressCount": int,
+    },
+    total=False,
+)
+
+class CreateNatGatewayRequestRequestTypeDef(
+    _RequiredCreateNatGatewayRequestRequestTypeDef, _OptionalCreateNatGatewayRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateNetworkAclRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNetworkAclRequestRequestTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateNetworkAclRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNetworkAclRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class CreateNetworkAclRequestRequestTypeDef(
+    _RequiredCreateNetworkAclRequestRequestTypeDef, _OptionalCreateNetworkAclRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef = TypedDict(
+    "_RequiredCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef = TypedDict(
+    "_OptionalCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef(
+    _RequiredCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef,
+    _OptionalCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef,
+):
+    pass
+
 CreateNetworkAclRequestVpcCreateNetworkAclTypeDef = TypedDict(
     "CreateNetworkAclRequestVpcCreateNetworkAclTypeDef",
     {
         "DryRun": bool,
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
     total=False,
 )
 
+_RequiredCreateNetworkInterfaceRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNetworkInterfaceRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+    },
+)
+_OptionalCreateNetworkInterfaceRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNetworkInterfaceRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DryRun": bool,
+        "Groups": Sequence[str],
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
+        "PrivateIpAddress": str,
+        "PrivateIpAddresses": Sequence[PrivateIpAddressSpecificationTypeDef],
+        "SecondaryPrivateIpAddressCount": int,
+        "Ipv4Prefixes": Sequence[Ipv4PrefixSpecificationRequestTypeDef],
+        "Ipv4PrefixCount": int,
+        "Ipv6Prefixes": Sequence[Ipv6PrefixSpecificationRequestTypeDef],
+        "Ipv6PrefixCount": int,
+        "InterfaceType": NetworkInterfaceCreationTypeType,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class CreateNetworkInterfaceRequestRequestTypeDef(
+    _RequiredCreateNetworkInterfaceRequestRequestTypeDef,
+    _OptionalCreateNetworkInterfaceRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef = TypedDict(
+    "_RequiredCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
+    {
+        "SubnetId": str,
+    },
+)
+_OptionalCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef = TypedDict(
+    "_OptionalCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
+    {
+        "Description": str,
+        "DryRun": bool,
+        "Groups": Sequence[str],
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
+        "PrivateIpAddress": str,
+        "PrivateIpAddresses": Sequence[PrivateIpAddressSpecificationTypeDef],
+        "SecondaryPrivateIpAddressCount": int,
+        "Ipv4Prefixes": Sequence[Ipv4PrefixSpecificationRequestTypeDef],
+        "Ipv4PrefixCount": int,
+        "Ipv6Prefixes": Sequence[Ipv6PrefixSpecificationRequestTypeDef],
+        "Ipv6PrefixCount": int,
+        "InterfaceType": NetworkInterfaceCreationTypeType,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef(
+    _RequiredCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef,
+    _OptionalCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef,
+):
+    pass
+
 CreateNetworkInterfaceRequestSubnetCreateNetworkInterfaceTypeDef = TypedDict(
     "CreateNetworkInterfaceRequestSubnetCreateNetworkInterfaceTypeDef",
     {
         "Description": str,
         "DryRun": bool,
         "Groups": Sequence[str],
         "Ipv6AddressCount": int,
@@ -24615,23 +25343,193 @@
         "InterfaceType": NetworkInterfaceCreationTypeType,
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
+CreatePlacementGroupRequestRequestTypeDef = TypedDict(
+    "CreatePlacementGroupRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "GroupName": str,
+        "Strategy": PlacementStrategyType,
+        "PartitionCount": int,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "SpreadLevel": SpreadLevelType,
+    },
+    total=False,
+)
+
+CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef = TypedDict(
+    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
+    {
+        "DryRun": bool,
+        "GroupName": str,
+        "Strategy": PlacementStrategyType,
+        "PartitionCount": int,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "SpreadLevel": SpreadLevelType,
+    },
+    total=False,
+)
+
+CreatePublicIpv4PoolRequestRequestTypeDef = TypedDict(
+    "CreatePublicIpv4PoolRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateReplaceRootVolumeTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReplaceRootVolumeTaskRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+    },
+)
+_OptionalCreateReplaceRootVolumeTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReplaceRootVolumeTaskRequestRequestTypeDef",
+    {
+        "SnapshotId": str,
+        "ClientToken": str,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ImageId": str,
+        "DeleteReplacedRootVolume": bool,
+    },
+    total=False,
+)
+
+class CreateReplaceRootVolumeTaskRequestRequestTypeDef(
+    _RequiredCreateReplaceRootVolumeTaskRequestRequestTypeDef,
+    _OptionalCreateReplaceRootVolumeTaskRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateRestoreImageTaskRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRestoreImageTaskRequestRequestTypeDef",
+    {
+        "Bucket": str,
+        "ObjectKey": str,
+    },
+)
+_OptionalCreateRestoreImageTaskRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRestoreImageTaskRequestRequestTypeDef",
+    {
+        "Name": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateRestoreImageTaskRequestRequestTypeDef(
+    _RequiredCreateRestoreImageTaskRequestRequestTypeDef,
+    _OptionalCreateRestoreImageTaskRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateRouteTableRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRouteTableRequestRequestTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateRouteTableRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRouteTableRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class CreateRouteTableRequestRequestTypeDef(
+    _RequiredCreateRouteTableRequestRequestTypeDef, _OptionalCreateRouteTableRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef = TypedDict(
+    "_RequiredCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef = TypedDict(
+    "_OptionalCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef(
+    _RequiredCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef,
+    _OptionalCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef,
+):
+    pass
+
 CreateRouteTableRequestVpcCreateRouteTableTypeDef = TypedDict(
     "CreateRouteTableRequestVpcCreateRouteTableTypeDef",
     {
         "DryRun": bool,
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
     total=False,
 )
 
+_RequiredCreateSecurityGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSecurityGroupRequestRequestTypeDef",
+    {
+        "Description": str,
+        "GroupName": str,
+    },
+)
+_OptionalCreateSecurityGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSecurityGroupRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateSecurityGroupRequestRequestTypeDef(
+    _RequiredCreateSecurityGroupRequestRequestTypeDef,
+    _OptionalCreateSecurityGroupRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef = TypedDict(
+    "_RequiredCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
+    {
+        "Description": str,
+        "GroupName": str,
+    },
+)
+_OptionalCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef = TypedDict(
+    "_OptionalCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
+    {
+        "VpcId": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef(
+    _RequiredCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef,
+    _OptionalCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef,
+):
+    pass
+
 _RequiredCreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef = TypedDict(
     "_RequiredCreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef",
     {
         "Description": str,
         "GroupName": str,
     },
 )
@@ -24646,25 +25544,170 @@
 
 class CreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef(
     _RequiredCreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef,
     _OptionalCreateSecurityGroupRequestVpcCreateSecurityGroupTypeDef,
 ):
     pass
 
+_RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSnapshotRequestRequestTypeDef",
+    {
+        "VolumeId": str,
+    },
+)
+_OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSnapshotRequestRequestTypeDef",
+    {
+        "Description": str,
+        "OutpostArn": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateSnapshotRequestRequestTypeDef(
+    _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef = TypedDict(
+    "_RequiredCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
+    {
+        "VolumeId": str,
+    },
+)
+_OptionalCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef = TypedDict(
+    "_OptionalCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
+    {
+        "Description": str,
+        "OutpostArn": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef(
+    _RequiredCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef,
+    _OptionalCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef,
+):
+    pass
+
 CreateSnapshotRequestVolumeCreateSnapshotTypeDef = TypedDict(
     "CreateSnapshotRequestVolumeCreateSnapshotTypeDef",
     {
         "Description": str,
         "OutpostArn": str,
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "DryRun": bool,
     },
     total=False,
 )
 
+_RequiredCreateSnapshotsRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSnapshotsRequestRequestTypeDef",
+    {
+        "InstanceSpecification": InstanceSpecificationTypeDef,
+    },
+)
+_OptionalCreateSnapshotsRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSnapshotsRequestRequestTypeDef",
+    {
+        "Description": str,
+        "OutpostArn": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "CopyTagsFromSource": Literal["volume"],
+    },
+    total=False,
+)
+
+class CreateSnapshotsRequestRequestTypeDef(
+    _RequiredCreateSnapshotsRequestRequestTypeDef, _OptionalCreateSnapshotsRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateSubnetCidrReservationRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSubnetCidrReservationRequestRequestTypeDef",
+    {
+        "SubnetId": str,
+        "Cidr": str,
+        "ReservationType": SubnetCidrReservationTypeType,
+    },
+)
+_OptionalCreateSubnetCidrReservationRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSubnetCidrReservationRequestRequestTypeDef",
+    {
+        "Description": str,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class CreateSubnetCidrReservationRequestRequestTypeDef(
+    _RequiredCreateSubnetCidrReservationRequestRequestTypeDef,
+    _OptionalCreateSubnetCidrReservationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateSubnetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateSubnetRequestRequestTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateSubnetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateSubnetRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "AvailabilityZone": str,
+        "AvailabilityZoneId": str,
+        "CidrBlock": str,
+        "Ipv6CidrBlock": str,
+        "OutpostArn": str,
+        "DryRun": bool,
+        "Ipv6Native": bool,
+    },
+    total=False,
+)
+
+class CreateSubnetRequestRequestTypeDef(
+    _RequiredCreateSubnetRequestRequestTypeDef, _OptionalCreateSubnetRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateSubnetRequestServiceResourceCreateSubnetTypeDef = TypedDict(
+    "_RequiredCreateSubnetRequestServiceResourceCreateSubnetTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateSubnetRequestServiceResourceCreateSubnetTypeDef = TypedDict(
+    "_OptionalCreateSubnetRequestServiceResourceCreateSubnetTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "AvailabilityZone": str,
+        "AvailabilityZoneId": str,
+        "CidrBlock": str,
+        "Ipv6CidrBlock": str,
+        "OutpostArn": str,
+        "DryRun": bool,
+        "Ipv6Native": bool,
+    },
+    total=False,
+)
+
+class CreateSubnetRequestServiceResourceCreateSubnetTypeDef(
+    _RequiredCreateSubnetRequestServiceResourceCreateSubnetTypeDef,
+    _OptionalCreateSubnetRequestServiceResourceCreateSubnetTypeDef,
+):
+    pass
+
 CreateSubnetRequestVpcCreateSubnetTypeDef = TypedDict(
     "CreateSubnetRequestVpcCreateSubnetTypeDef",
     {
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "AvailabilityZone": str,
         "AvailabilityZoneId": str,
         "CidrBlock": str,
@@ -24672,27 +25715,744 @@
         "OutpostArn": str,
         "DryRun": bool,
         "Ipv6Native": bool,
     },
     total=False,
 )
 
+CreateTrafficMirrorFilterRequestRequestTypeDef = TypedDict(
+    "CreateTrafficMirrorFilterRequestRequestTypeDef",
+    {
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+_RequiredCreateTrafficMirrorSessionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTrafficMirrorSessionRequestRequestTypeDef",
+    {
+        "NetworkInterfaceId": str,
+        "TrafficMirrorTargetId": str,
+        "TrafficMirrorFilterId": str,
+        "SessionNumber": int,
+    },
+)
+_OptionalCreateTrafficMirrorSessionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTrafficMirrorSessionRequestRequestTypeDef",
+    {
+        "PacketLength": int,
+        "VirtualNetworkId": int,
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class CreateTrafficMirrorSessionRequestRequestTypeDef(
+    _RequiredCreateTrafficMirrorSessionRequestRequestTypeDef,
+    _OptionalCreateTrafficMirrorSessionRequestRequestTypeDef,
+):
+    pass
+
+CreateTrafficMirrorTargetRequestRequestTypeDef = TypedDict(
+    "CreateTrafficMirrorTargetRequestRequestTypeDef",
+    {
+        "NetworkInterfaceId": str,
+        "NetworkLoadBalancerArn": str,
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "ClientToken": str,
+        "GatewayLoadBalancerEndpointId": str,
+    },
+    total=False,
+)
+
+_RequiredCreateTransitGatewayConnectPeerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayConnectPeerRequestRequestTypeDef",
+    {
+        "TransitGatewayAttachmentId": str,
+        "PeerAddress": str,
+        "InsideCidrBlocks": Sequence[str],
+    },
+)
+_OptionalCreateTransitGatewayConnectPeerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayConnectPeerRequestRequestTypeDef",
+    {
+        "TransitGatewayAddress": str,
+        "BgpOptions": TransitGatewayConnectRequestBgpOptionsTypeDef,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateTransitGatewayConnectPeerRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayConnectPeerRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayConnectPeerRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateTransitGatewayConnectRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayConnectRequestRequestTypeDef",
+    {
+        "TransportTransitGatewayAttachmentId": str,
+        "Options": CreateTransitGatewayConnectRequestOptionsTypeDef,
+    },
+)
+_OptionalCreateTransitGatewayConnectRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayConnectRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateTransitGatewayConnectRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayConnectRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayConnectRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateTransitGatewayMulticastDomainRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayMulticastDomainRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+    },
+)
+_OptionalCreateTransitGatewayMulticastDomainRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayMulticastDomainRequestRequestTypeDef",
+    {
+        "Options": CreateTransitGatewayMulticastDomainRequestOptionsTypeDef,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateTransitGatewayMulticastDomainRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayMulticastDomainRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayMulticastDomainRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "PeerTransitGatewayId": str,
+        "PeerAccountId": str,
+        "PeerRegion": str,
+    },
+)
+_OptionalCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
+    {
+        "Options": CreateTransitGatewayPeeringAttachmentRequestOptionsTypeDef,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateTransitGatewayPolicyTableRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayPolicyTableRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+    },
+)
+_OptionalCreateTransitGatewayPolicyTableRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayPolicyTableRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateTransitGatewayPolicyTableRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayPolicyTableRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayPolicyTableRequestRequestTypeDef,
+):
+    pass
+
+CreateTransitGatewayRequestRequestTypeDef = TypedDict(
+    "CreateTransitGatewayRequestRequestTypeDef",
+    {
+        "Description": str,
+        "Options": TransitGatewayRequestOptionsTypeDef,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+_RequiredCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
+    {
+        "TransitGatewayRouteTableId": str,
+        "PeeringAttachmentId": str,
+    },
+)
+_OptionalCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayRouteTableRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+    },
+)
+_OptionalCreateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayRouteTableRequestRequestTypeDef",
+    {
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateTransitGatewayRouteTableRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayRouteTableRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayRouteTableRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateTransitGatewayVpcAttachmentRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
+    {
+        "TransitGatewayId": str,
+        "VpcId": str,
+        "SubnetIds": Sequence[str],
+    },
+)
+_OptionalCreateTransitGatewayVpcAttachmentRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
+    {
+        "Options": CreateTransitGatewayVpcAttachmentRequestOptionsTypeDef,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateTransitGatewayVpcAttachmentRequestRequestTypeDef(
+    _RequiredCreateTransitGatewayVpcAttachmentRequestRequestTypeDef,
+    _OptionalCreateTransitGatewayVpcAttachmentRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateVerifiedAccessEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVerifiedAccessEndpointRequestRequestTypeDef",
+    {
+        "VerifiedAccessGroupId": str,
+        "EndpointType": VerifiedAccessEndpointTypeType,
+        "AttachmentType": Literal["vpc"],
+        "DomainCertificateArn": str,
+        "ApplicationDomain": str,
+        "EndpointDomainPrefix": str,
+    },
+)
+_OptionalCreateVerifiedAccessEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVerifiedAccessEndpointRequestRequestTypeDef",
+    {
+        "SecurityGroupIds": Sequence[str],
+        "LoadBalancerOptions": CreateVerifiedAccessEndpointLoadBalancerOptionsTypeDef,
+        "NetworkInterfaceOptions": CreateVerifiedAccessEndpointEniOptionsTypeDef,
+        "Description": str,
+        "PolicyDocument": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateVerifiedAccessEndpointRequestRequestTypeDef(
+    _RequiredCreateVerifiedAccessEndpointRequestRequestTypeDef,
+    _OptionalCreateVerifiedAccessEndpointRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateVerifiedAccessGroupRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVerifiedAccessGroupRequestRequestTypeDef",
+    {
+        "VerifiedAccessInstanceId": str,
+    },
+)
+_OptionalCreateVerifiedAccessGroupRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVerifiedAccessGroupRequestRequestTypeDef",
+    {
+        "Description": str,
+        "PolicyDocument": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateVerifiedAccessGroupRequestRequestTypeDef(
+    _RequiredCreateVerifiedAccessGroupRequestRequestTypeDef,
+    _OptionalCreateVerifiedAccessGroupRequestRequestTypeDef,
+):
+    pass
+
+CreateVerifiedAccessInstanceRequestRequestTypeDef = TypedDict(
+    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
+    {
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+_RequiredCreateVerifiedAccessTrustProviderRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVerifiedAccessTrustProviderRequestRequestTypeDef",
+    {
+        "TrustProviderType": TrustProviderTypeType,
+        "PolicyReferenceName": str,
+    },
+)
+_OptionalCreateVerifiedAccessTrustProviderRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVerifiedAccessTrustProviderRequestRequestTypeDef",
+    {
+        "UserTrustProviderType": UserTrustProviderTypeType,
+        "DeviceTrustProviderType": DeviceTrustProviderTypeType,
+        "OidcOptions": CreateVerifiedAccessTrustProviderOidcOptionsTypeDef,
+        "DeviceOptions": CreateVerifiedAccessTrustProviderDeviceOptionsTypeDef,
+        "Description": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "ClientToken": str,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateVerifiedAccessTrustProviderRequestRequestTypeDef(
+    _RequiredCreateVerifiedAccessTrustProviderRequestRequestTypeDef,
+    _OptionalCreateVerifiedAccessTrustProviderRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVolumeRequestRequestTypeDef",
+    {
+        "AvailabilityZone": str,
+    },
+)
+_OptionalCreateVolumeRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVolumeRequestRequestTypeDef",
+    {
+        "Encrypted": bool,
+        "Iops": int,
+        "KmsKeyId": str,
+        "OutpostArn": str,
+        "Size": int,
+        "SnapshotId": str,
+        "VolumeType": VolumeTypeType,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "MultiAttachEnabled": bool,
+        "Throughput": int,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class CreateVolumeRequestRequestTypeDef(
+    _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
+):
+    pass
+
+_RequiredCreateVolumeRequestServiceResourceCreateVolumeTypeDef = TypedDict(
+    "_RequiredCreateVolumeRequestServiceResourceCreateVolumeTypeDef",
+    {
+        "AvailabilityZone": str,
+    },
+)
+_OptionalCreateVolumeRequestServiceResourceCreateVolumeTypeDef = TypedDict(
+    "_OptionalCreateVolumeRequestServiceResourceCreateVolumeTypeDef",
+    {
+        "Encrypted": bool,
+        "Iops": int,
+        "KmsKeyId": str,
+        "OutpostArn": str,
+        "Size": int,
+        "SnapshotId": str,
+        "VolumeType": VolumeTypeType,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "MultiAttachEnabled": bool,
+        "Throughput": int,
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class CreateVolumeRequestServiceResourceCreateVolumeTypeDef(
+    _RequiredCreateVolumeRequestServiceResourceCreateVolumeTypeDef,
+    _OptionalCreateVolumeRequestServiceResourceCreateVolumeTypeDef,
+):
+    pass
+
+_RequiredCreateVpcEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVpcEndpointRequestRequestTypeDef",
+    {
+        "VpcId": str,
+        "ServiceName": str,
+    },
+)
+_OptionalCreateVpcEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVpcEndpointRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "VpcEndpointType": VpcEndpointTypeType,
+        "PolicyDocument": str,
+        "RouteTableIds": Sequence[str],
+        "SubnetIds": Sequence[str],
+        "SecurityGroupIds": Sequence[str],
+        "IpAddressType": IpAddressTypeType,
+        "DnsOptions": DnsOptionsSpecificationTypeDef,
+        "ClientToken": str,
+        "PrivateDnsEnabled": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class CreateVpcEndpointRequestRequestTypeDef(
+    _RequiredCreateVpcEndpointRequestRequestTypeDef, _OptionalCreateVpcEndpointRequestRequestTypeDef
+):
+    pass
+
+CreateVpcEndpointServiceConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "AcceptanceRequired": bool,
+        "PrivateDnsName": str,
+        "NetworkLoadBalancerArns": Sequence[str],
+        "GatewayLoadBalancerArns": Sequence[str],
+        "SupportedIpAddressTypes": Sequence[str],
+        "ClientToken": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateVpcPeeringConnectionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVpcPeeringConnectionRequestRequestTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateVpcPeeringConnectionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVpcPeeringConnectionRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "PeerOwnerId": str,
+        "PeerVpcId": str,
+        "PeerRegion": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class CreateVpcPeeringConnectionRequestRequestTypeDef(
+    _RequiredCreateVpcPeeringConnectionRequestRequestTypeDef,
+    _OptionalCreateVpcPeeringConnectionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef = TypedDict(
+    "_RequiredCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
+    {
+        "VpcId": str,
+    },
+)
+_OptionalCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef = TypedDict(
+    "_OptionalCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
+    {
+        "DryRun": bool,
+        "PeerOwnerId": str,
+        "PeerVpcId": str,
+        "PeerRegion": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef(
+    _RequiredCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef,
+    _OptionalCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef,
+):
+    pass
+
 CreateVpcPeeringConnectionRequestVpcRequestVpcPeeringConnectionTypeDef = TypedDict(
     "CreateVpcPeeringConnectionRequestVpcRequestVpcPeeringConnectionTypeDef",
     {
         "DryRun": bool,
         "PeerOwnerId": str,
         "PeerVpcId": str,
         "PeerRegion": str,
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
     total=False,
 )
 
-TagSpecificationUnionTypeDef = Union[TagSpecificationTypeDef, TagSpecificationOutputTypeDef]
+CreateVpcRequestRequestTypeDef = TypedDict(
+    "CreateVpcRequestRequestTypeDef",
+    {
+        "CidrBlock": str,
+        "AmazonProvidedIpv6CidrBlock": bool,
+        "Ipv6Pool": str,
+        "Ipv6CidrBlock": str,
+        "Ipv4IpamPoolId": str,
+        "Ipv4NetmaskLength": int,
+        "Ipv6IpamPoolId": str,
+        "Ipv6NetmaskLength": int,
+        "DryRun": bool,
+        "InstanceTenancy": TenancyType,
+        "Ipv6CidrBlockNetworkBorderGroup": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+CreateVpcRequestServiceResourceCreateVpcTypeDef = TypedDict(
+    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
+    {
+        "CidrBlock": str,
+        "AmazonProvidedIpv6CidrBlock": bool,
+        "Ipv6Pool": str,
+        "Ipv6CidrBlock": str,
+        "Ipv4IpamPoolId": str,
+        "Ipv4NetmaskLength": int,
+        "Ipv6IpamPoolId": str,
+        "Ipv6NetmaskLength": int,
+        "DryRun": bool,
+        "InstanceTenancy": TenancyType,
+        "Ipv6CidrBlockNetworkBorderGroup": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+_RequiredCreateVpnGatewayRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateVpnGatewayRequestRequestTypeDef",
+    {
+        "Type": Literal["ipsec.1"],
+    },
+)
+_OptionalCreateVpnGatewayRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateVpnGatewayRequestRequestTypeDef",
+    {
+        "AvailabilityZone": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "AmazonSideAsn": int,
+        "DryRun": bool,
+    },
+    total=False,
+)
+
+class CreateVpnGatewayRequestRequestTypeDef(
+    _RequiredCreateVpnGatewayRequestRequestTypeDef, _OptionalCreateVpnGatewayRequestRequestTypeDef
+):
+    pass
+
+_RequiredExportImageRequestRequestTypeDef = TypedDict(
+    "_RequiredExportImageRequestRequestTypeDef",
+    {
+        "DiskImageFormat": DiskImageFormatType,
+        "ImageId": str,
+        "S3ExportLocation": ExportTaskS3LocationRequestTypeDef,
+    },
+)
+_OptionalExportImageRequestRequestTypeDef = TypedDict(
+    "_OptionalExportImageRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "Description": str,
+        "DryRun": bool,
+        "RoleName": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class ExportImageRequestRequestTypeDef(
+    _RequiredExportImageRequestRequestTypeDef, _OptionalExportImageRequestRequestTypeDef
+):
+    pass
+
+_RequiredImportKeyPairRequestRequestTypeDef = TypedDict(
+    "_RequiredImportKeyPairRequestRequestTypeDef",
+    {
+        "KeyName": str,
+        "PublicKeyMaterial": BlobTypeDef,
+    },
+)
+_OptionalImportKeyPairRequestRequestTypeDef = TypedDict(
+    "_OptionalImportKeyPairRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class ImportKeyPairRequestRequestTypeDef(
+    _RequiredImportKeyPairRequestRequestTypeDef, _OptionalImportKeyPairRequestRequestTypeDef
+):
+    pass
+
+_RequiredImportKeyPairRequestServiceResourceImportKeyPairTypeDef = TypedDict(
+    "_RequiredImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
+    {
+        "KeyName": str,
+        "PublicKeyMaterial": BlobTypeDef,
+    },
+)
+_OptionalImportKeyPairRequestServiceResourceImportKeyPairTypeDef = TypedDict(
+    "_OptionalImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class ImportKeyPairRequestServiceResourceImportKeyPairTypeDef(
+    _RequiredImportKeyPairRequestServiceResourceImportKeyPairTypeDef,
+    _OptionalImportKeyPairRequestServiceResourceImportKeyPairTypeDef,
+):
+    pass
+
+_RequiredProvisionByoipCidrRequestRequestTypeDef = TypedDict(
+    "_RequiredProvisionByoipCidrRequestRequestTypeDef",
+    {
+        "Cidr": str,
+    },
+)
+_OptionalProvisionByoipCidrRequestRequestTypeDef = TypedDict(
+    "_OptionalProvisionByoipCidrRequestRequestTypeDef",
+    {
+        "CidrAuthorizationContext": CidrAuthorizationContextTypeDef,
+        "PubliclyAdvertisable": bool,
+        "Description": str,
+        "DryRun": bool,
+        "PoolTagSpecifications": Sequence[TagSpecificationTypeDef],
+        "MultiRegion": bool,
+    },
+    total=False,
+)
+
+class ProvisionByoipCidrRequestRequestTypeDef(
+    _RequiredProvisionByoipCidrRequestRequestTypeDef,
+    _OptionalProvisionByoipCidrRequestRequestTypeDef,
+):
+    pass
+
+_RequiredPurchaseHostReservationRequestRequestTypeDef = TypedDict(
+    "_RequiredPurchaseHostReservationRequestRequestTypeDef",
+    {
+        "HostIdSet": Sequence[str],
+        "OfferingId": str,
+    },
+)
+_OptionalPurchaseHostReservationRequestRequestTypeDef = TypedDict(
+    "_OptionalPurchaseHostReservationRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+        "CurrencyCode": Literal["USD"],
+        "LimitPrice": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class PurchaseHostReservationRequestRequestTypeDef(
+    _RequiredPurchaseHostReservationRequestRequestTypeDef,
+    _OptionalPurchaseHostReservationRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef = TypedDict(
+    "_RequiredStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
+    {
+        "NetworkInsightsAccessScopeId": str,
+        "ClientToken": str,
+    },
+)
+_OptionalStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef = TypedDict(
+    "_OptionalStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef(
+    _RequiredStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef,
+    _OptionalStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef,
+):
+    pass
+
+_RequiredStartNetworkInsightsAnalysisRequestRequestTypeDef = TypedDict(
+    "_RequiredStartNetworkInsightsAnalysisRequestRequestTypeDef",
+    {
+        "NetworkInsightsPathId": str,
+        "ClientToken": str,
+    },
+)
+_OptionalStartNetworkInsightsAnalysisRequestRequestTypeDef = TypedDict(
+    "_OptionalStartNetworkInsightsAnalysisRequestRequestTypeDef",
+    {
+        "AdditionalAccounts": Sequence[str],
+        "FilterInArns": Sequence[str],
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class StartNetworkInsightsAnalysisRequestRequestTypeDef(
+    _RequiredStartNetworkInsightsAnalysisRequestRequestTypeDef,
+    _OptionalStartNetworkInsightsAnalysisRequestRequestTypeDef,
+):
+    pass
+
 CreateTrafficMirrorSessionResultTypeDef = TypedDict(
     "CreateTrafficMirrorSessionResultTypeDef",
     {
         "TrafficMirrorSession": TrafficMirrorSessionTypeDef,
         "ClientToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -25183,14 +26943,38 @@
 
 class CreateImageRequestInstanceCreateImageTypeDef(
     _RequiredCreateImageRequestInstanceCreateImageTypeDef,
     _OptionalCreateImageRequestInstanceCreateImageTypeDef,
 ):
     pass
 
+_RequiredCreateImageRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateImageRequestRequestTypeDef",
+    {
+        "InstanceId": str,
+        "Name": str,
+    },
+)
+_OptionalCreateImageRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateImageRequestRequestTypeDef",
+    {
+        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "Description": str,
+        "DryRun": bool,
+        "NoReboot": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
+class CreateImageRequestRequestTypeDef(
+    _RequiredCreateImageRequestRequestTypeDef, _OptionalCreateImageRequestRequestTypeDef
+):
+    pass
+
 ImageAttributeTypeDef = TypedDict(
     "ImageAttributeTypeDef",
     {
         "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
         "ImageId": str,
         "LaunchPermissions": List[LaunchPermissionTypeDef],
         "ProductCodes": List[ProductCodeTypeDef],
@@ -25383,14 +27167,50 @@
     {
         "Instances": List[ClassicLinkInstanceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateClientVpnEndpointRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateClientVpnEndpointRequestRequestTypeDef",
+    {
+        "ClientCidrBlock": str,
+        "ServerCertificateArn": str,
+        "AuthenticationOptions": Sequence[ClientVpnAuthenticationRequestTypeDef],
+        "ConnectionLogOptions": ConnectionLogOptionsTypeDef,
+    },
+)
+_OptionalCreateClientVpnEndpointRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateClientVpnEndpointRequestRequestTypeDef",
+    {
+        "DnsServers": Sequence[str],
+        "TransportProtocol": TransportProtocolType,
+        "VpnPort": int,
+        "Description": str,
+        "SplitTunnel": bool,
+        "DryRun": bool,
+        "ClientToken": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "SecurityGroupIds": Sequence[str],
+        "VpcId": str,
+        "SelfServicePortal": SelfServicePortalType,
+        "ClientConnectOptions": ClientConnectOptionsTypeDef,
+        "SessionTimeoutHours": int,
+        "ClientLoginBannerOptions": ClientLoginBannerOptionsTypeDef,
+    },
+    total=False,
+)
+
+class CreateClientVpnEndpointRequestRequestTypeDef(
+    _RequiredCreateClientVpnEndpointRequestRequestTypeDef,
+    _OptionalCreateClientVpnEndpointRequestRequestTypeDef,
+):
+    pass
+
 ClientVpnEndpointTypeDef = TypedDict(
     "ClientVpnEndpointTypeDef",
     {
         "ClientVpnEndpointId": str,
         "Description": str,
         "Status": ClientVpnEndpointStatusTypeDef,
         "CreationTime": str,
@@ -25550,26 +27370,23 @@
         "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
         "EbsOptimized": bool,
         "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
         "ImageId": str,
         "InstanceType": InstanceTypeType,
         "KernelId": str,
         "KeyName": str,
-        "NetworkInterfaces": List[InstanceNetworkInterfaceSpecificationOutputTypeDef],
+        "NetworkInterfaces": List[InstanceNetworkInterfaceSpecificationTypeDef],
         "Placement": SpotPlacementTypeDef,
         "RamdiskId": str,
         "SubnetId": str,
         "Monitoring": RunInstancesMonitoringEnabledTypeDef,
     },
     total=False,
 )
 
-InstanceNetworkInterfaceSpecificationUnionTypeDef = Union[
-    InstanceNetworkInterfaceSpecificationTypeDef, InstanceNetworkInterfaceSpecificationOutputTypeDef
-]
 RequestSpotLaunchSpecificationTypeDef = TypedDict(
     "RequestSpotLaunchSpecificationTypeDef",
     {
         "SecurityGroupIds": Sequence[str],
         "SecurityGroups": Sequence[str],
         "AddressingType": str,
         "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
@@ -26166,37 +27983,51 @@
 
 class ModifyImageAttributeRequestRequestTypeDef(
     _RequiredModifyImageAttributeRequestRequestTypeDef,
     _OptionalModifyImageAttributeRequestRequestTypeDef,
 ):
     pass
 
-CreateLocalGatewayRouteTableResultTypeDef = TypedDict(
-    "CreateLocalGatewayRouteTableResultTypeDef",
-    {
-        "LocalGatewayRouteTable": LocalGatewayRouteTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DeleteLocalGatewayRouteTableResultTypeDef = TypedDict(
-    "DeleteLocalGatewayRouteTableResultTypeDef",
+ImportImageRequestRequestTypeDef = TypedDict(
+    "ImportImageRequestRequestTypeDef",
     {
-        "LocalGatewayRouteTable": LocalGatewayRouteTableTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Architecture": str,
+        "ClientData": ClientDataTypeDef,
+        "ClientToken": str,
+        "Description": str,
+        "DiskContainers": Sequence[ImageDiskContainerTypeDef],
+        "DryRun": bool,
+        "Encrypted": bool,
+        "Hypervisor": str,
+        "KmsKeyId": str,
+        "LicenseType": str,
+        "Platform": str,
+        "RoleName": str,
+        "LicenseSpecifications": Sequence[ImportImageLicenseConfigurationRequestTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "UsageOperation": str,
+        "BootMode": BootModeValuesType,
     },
+    total=False,
 )
 
-DescribeLocalGatewayRouteTablesResultTypeDef = TypedDict(
-    "DescribeLocalGatewayRouteTablesResultTypeDef",
+ImportSnapshotRequestRequestTypeDef = TypedDict(
+    "ImportSnapshotRequestRequestTypeDef",
     {
-        "LocalGatewayRouteTables": List[LocalGatewayRouteTableTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "ClientData": ClientDataTypeDef,
+        "ClientToken": str,
+        "Description": str,
+        "DiskContainer": SnapshotDiskContainerTypeDef,
+        "DryRun": bool,
+        "Encrypted": bool,
+        "KmsKeyId": str,
+        "RoleName": str,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
+    total=False,
 )
 
 _RequiredImportInstanceRequestRequestTypeDef = TypedDict(
     "_RequiredImportInstanceRequestRequestTypeDef",
     {
         "Platform": Literal["Windows"],
     },
@@ -26254,110 +28085,14 @@
         "InterfaceType": str,
         "Ipv4Prefixes": List[InstanceIpv4PrefixTypeDef],
         "Ipv6Prefixes": List[InstanceIpv6PrefixTypeDef],
     },
     total=False,
 )
 
-FleetLaunchTemplateOverridesTypeDef = TypedDict(
-    "FleetLaunchTemplateOverridesTypeDef",
-    {
-        "InstanceType": InstanceTypeType,
-        "MaxPrice": str,
-        "SubnetId": str,
-        "AvailabilityZone": str,
-        "WeightedCapacity": float,
-        "Priority": float,
-        "Placement": PlacementResponseTypeDef,
-        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
-        "ImageId": str,
-    },
-    total=False,
-)
-
-LaunchTemplateOverridesOutputTypeDef = TypedDict(
-    "LaunchTemplateOverridesOutputTypeDef",
-    {
-        "InstanceType": InstanceTypeType,
-        "SpotPrice": str,
-        "SubnetId": str,
-        "AvailabilityZone": str,
-        "WeightedCapacity": float,
-        "Priority": float,
-        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
-    },
-    total=False,
-)
-
-SpotFleetLaunchSpecificationOutputTypeDef = TypedDict(
-    "SpotFleetLaunchSpecificationOutputTypeDef",
-    {
-        "SecurityGroups": List[GroupIdentifierTypeDef],
-        "AddressingType": str,
-        "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
-        "EbsOptimized": bool,
-        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
-        "ImageId": str,
-        "InstanceType": InstanceTypeType,
-        "KernelId": str,
-        "KeyName": str,
-        "Monitoring": SpotFleetMonitoringTypeDef,
-        "NetworkInterfaces": List[InstanceNetworkInterfaceSpecificationOutputTypeDef],
-        "Placement": SpotPlacementTypeDef,
-        "RamdiskId": str,
-        "SpotPrice": str,
-        "SubnetId": str,
-        "UserData": str,
-        "WeightedCapacity": float,
-        "TagSpecifications": List[SpotFleetTagSpecificationOutputTypeDef],
-        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
-    },
-    total=False,
-)
-
-LaunchTemplateOverridesTypeDef = TypedDict(
-    "LaunchTemplateOverridesTypeDef",
-    {
-        "InstanceType": InstanceTypeType,
-        "SpotPrice": str,
-        "SubnetId": str,
-        "AvailabilityZone": str,
-        "WeightedCapacity": float,
-        "Priority": float,
-        "InstanceRequirements": InstanceRequirementsTypeDef,
-    },
-    total=False,
-)
-
-SpotFleetLaunchSpecificationTypeDef = TypedDict(
-    "SpotFleetLaunchSpecificationTypeDef",
-    {
-        "SecurityGroups": Sequence[GroupIdentifierTypeDef],
-        "AddressingType": str,
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
-        "EbsOptimized": bool,
-        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
-        "ImageId": str,
-        "InstanceType": InstanceTypeType,
-        "KernelId": str,
-        "KeyName": str,
-        "Monitoring": SpotFleetMonitoringTypeDef,
-        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationTypeDef],
-        "Placement": SpotPlacementTypeDef,
-        "RamdiskId": str,
-        "SpotPrice": str,
-        "SubnetId": str,
-        "UserData": str,
-        "WeightedCapacity": float,
-        "TagSpecifications": Sequence[SpotFleetTagSpecificationTypeDef],
-        "InstanceRequirements": InstanceRequirementsTypeDef,
-    },
-    total=False,
-)
-
 FleetLaunchTemplateOverridesRequestTypeDef = TypedDict(
     "FleetLaunchTemplateOverridesRequestTypeDef",
     {
         "InstanceType": InstanceTypeType,
         "MaxPrice": str,
         "SubnetId": str,
         "AvailabilityZone": str,
@@ -26423,14 +28158,70 @@
         "ArchitectureTypes": Sequence[ArchitectureTypeType],
         "VirtualizationTypes": Sequence[VirtualizationTypeType],
         "InstanceRequirements": InstanceRequirementsRequestTypeDef,
     },
     total=False,
 )
 
+FleetLaunchTemplateOverridesTypeDef = TypedDict(
+    "FleetLaunchTemplateOverridesTypeDef",
+    {
+        "InstanceType": InstanceTypeType,
+        "MaxPrice": str,
+        "SubnetId": str,
+        "AvailabilityZone": str,
+        "WeightedCapacity": float,
+        "Priority": float,
+        "Placement": PlacementResponseTypeDef,
+        "InstanceRequirements": InstanceRequirementsTypeDef,
+        "ImageId": str,
+    },
+    total=False,
+)
+
+LaunchTemplateOverridesTypeDef = TypedDict(
+    "LaunchTemplateOverridesTypeDef",
+    {
+        "InstanceType": InstanceTypeType,
+        "SpotPrice": str,
+        "SubnetId": str,
+        "AvailabilityZone": str,
+        "WeightedCapacity": float,
+        "Priority": float,
+        "InstanceRequirements": InstanceRequirementsTypeDef,
+    },
+    total=False,
+)
+
+SpotFleetLaunchSpecificationTypeDef = TypedDict(
+    "SpotFleetLaunchSpecificationTypeDef",
+    {
+        "SecurityGroups": List[GroupIdentifierTypeDef],
+        "AddressingType": str,
+        "BlockDeviceMappings": List[BlockDeviceMappingTypeDef],
+        "EbsOptimized": bool,
+        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
+        "ImageId": str,
+        "InstanceType": InstanceTypeType,
+        "KernelId": str,
+        "KeyName": str,
+        "Monitoring": SpotFleetMonitoringTypeDef,
+        "NetworkInterfaces": List[InstanceNetworkInterfaceSpecificationTypeDef],
+        "Placement": SpotPlacementTypeDef,
+        "RamdiskId": str,
+        "SpotPrice": str,
+        "SubnetId": str,
+        "UserData": str,
+        "WeightedCapacity": float,
+        "TagSpecifications": List[SpotFleetTagSpecificationTypeDef],
+        "InstanceRequirements": InstanceRequirementsTypeDef,
+    },
+    total=False,
+)
+
 StartInstancesResultTypeDef = TypedDict(
     "StartInstancesResultTypeDef",
     {
         "StartingInstances": List[InstanceStateChangeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -26461,47 +28252,42 @@
         "InstanceState": InstanceStateTypeDef,
         "InstanceStatus": InstanceStatusSummaryTypeDef,
         "SystemStatus": InstanceStatusSummaryTypeDef,
     },
     total=False,
 )
 
-RevokeSecurityGroupEgressResultTypeDef = TypedDict(
-    "RevokeSecurityGroupEgressResultTypeDef",
-    {
-        "Return": bool,
-        "UnknownIpPermissions": List[IpPermissionOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RevokeSecurityGroupIngressResultTypeDef = TypedDict(
-    "RevokeSecurityGroupIngressResultTypeDef",
+_RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
+    "_RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef",
     {
-        "Return": bool,
-        "UnknownIpPermissions": List[IpPermissionOutputTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "GroupId": str,
     },
 )
-
-SecurityGroupTypeDef = TypedDict(
-    "SecurityGroupTypeDef",
+_OptionalAuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
+    "_OptionalAuthorizeSecurityGroupEgressRequestRequestTypeDef",
     {
-        "Description": str,
-        "GroupName": str,
-        "IpPermissions": List[IpPermissionOutputTypeDef],
-        "OwnerId": str,
-        "GroupId": str,
-        "IpPermissionsEgress": List[IpPermissionOutputTypeDef],
-        "Tags": List[TagTypeDef],
-        "VpcId": str,
+        "DryRun": bool,
+        "IpPermissions": Sequence[IpPermissionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "CidrIp": str,
+        "FromPort": int,
+        "IpProtocol": str,
+        "ToPort": int,
+        "SourceSecurityGroupName": str,
+        "SourceSecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+class AuthorizeSecurityGroupEgressRequestRequestTypeDef(
+    _RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef,
+    _OptionalAuthorizeSecurityGroupEgressRequestRequestTypeDef,
+):
+    pass
+
 AuthorizeSecurityGroupEgressRequestSecurityGroupAuthorizeEgressTypeDef = TypedDict(
     "AuthorizeSecurityGroupEgressRequestSecurityGroupAuthorizeEgressTypeDef",
     {
         "DryRun": bool,
         "IpPermissions": Sequence[IpPermissionTypeDef],
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "CidrIp": str,
@@ -26510,14 +28296,32 @@
         "ToPort": int,
         "SourceSecurityGroupName": str,
         "SourceSecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+AuthorizeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
+    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
+    {
+        "CidrIp": str,
+        "FromPort": int,
+        "GroupId": str,
+        "GroupName": str,
+        "IpPermissions": Sequence[IpPermissionTypeDef],
+        "IpProtocol": str,
+        "SourceSecurityGroupName": str,
+        "SourceSecurityGroupOwnerId": str,
+        "ToPort": int,
+        "DryRun": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+    },
+    total=False,
+)
+
 AuthorizeSecurityGroupIngressRequestSecurityGroupAuthorizeIngressTypeDef = TypedDict(
     "AuthorizeSecurityGroupIngressRequestSecurityGroupAuthorizeIngressTypeDef",
     {
         "CidrIp": str,
         "FromPort": int,
         "GroupName": str,
         "IpPermissions": Sequence[IpPermissionTypeDef],
@@ -26527,15 +28331,42 @@
         "ToPort": int,
         "DryRun": bool,
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
     total=False,
 )
 
-IpPermissionUnionTypeDef = Union[IpPermissionTypeDef, IpPermissionOutputTypeDef]
+_RequiredRevokeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
+    "_RequiredRevokeSecurityGroupEgressRequestRequestTypeDef",
+    {
+        "GroupId": str,
+    },
+)
+_OptionalRevokeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
+    "_OptionalRevokeSecurityGroupEgressRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "IpPermissions": Sequence[IpPermissionTypeDef],
+        "SecurityGroupRuleIds": Sequence[str],
+        "CidrIp": str,
+        "FromPort": int,
+        "IpProtocol": str,
+        "ToPort": int,
+        "SourceSecurityGroupName": str,
+        "SourceSecurityGroupOwnerId": str,
+    },
+    total=False,
+)
+
+class RevokeSecurityGroupEgressRequestRequestTypeDef(
+    _RequiredRevokeSecurityGroupEgressRequestRequestTypeDef,
+    _OptionalRevokeSecurityGroupEgressRequestRequestTypeDef,
+):
+    pass
+
 RevokeSecurityGroupEgressRequestSecurityGroupRevokeEgressTypeDef = TypedDict(
     "RevokeSecurityGroupEgressRequestSecurityGroupRevokeEgressTypeDef",
     {
         "DryRun": bool,
         "IpPermissions": Sequence[IpPermissionTypeDef],
         "SecurityGroupRuleIds": Sequence[str],
         "CidrIp": str,
@@ -26544,14 +28375,41 @@
         "ToPort": int,
         "SourceSecurityGroupName": str,
         "SourceSecurityGroupOwnerId": str,
     },
     total=False,
 )
 
+RevokeSecurityGroupEgressResultTypeDef = TypedDict(
+    "RevokeSecurityGroupEgressResultTypeDef",
+    {
+        "Return": bool,
+        "UnknownIpPermissions": List[IpPermissionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RevokeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
+    "RevokeSecurityGroupIngressRequestRequestTypeDef",
+    {
+        "CidrIp": str,
+        "FromPort": int,
+        "GroupId": str,
+        "GroupName": str,
+        "IpPermissions": Sequence[IpPermissionTypeDef],
+        "IpProtocol": str,
+        "SourceSecurityGroupName": str,
+        "SourceSecurityGroupOwnerId": str,
+        "ToPort": int,
+        "DryRun": bool,
+        "SecurityGroupRuleIds": Sequence[str],
+    },
+    total=False,
+)
+
 RevokeSecurityGroupIngressRequestSecurityGroupRevokeIngressTypeDef = TypedDict(
     "RevokeSecurityGroupIngressRequestSecurityGroupRevokeIngressTypeDef",
     {
         "CidrIp": str,
         "FromPort": int,
         "GroupName": str,
         "IpPermissions": Sequence[IpPermissionTypeDef],
@@ -26561,14 +28419,77 @@
         "ToPort": int,
         "DryRun": bool,
         "SecurityGroupRuleIds": Sequence[str],
     },
     total=False,
 )
 
+RevokeSecurityGroupIngressResultTypeDef = TypedDict(
+    "RevokeSecurityGroupIngressResultTypeDef",
+    {
+        "Return": bool,
+        "UnknownIpPermissions": List[IpPermissionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SecurityGroupTypeDef = TypedDict(
+    "SecurityGroupTypeDef",
+    {
+        "Description": str,
+        "GroupName": str,
+        "IpPermissions": List[IpPermissionTypeDef],
+        "OwnerId": str,
+        "GroupId": str,
+        "IpPermissionsEgress": List[IpPermissionTypeDef],
+        "Tags": List[TagTypeDef],
+        "VpcId": str,
+    },
+    total=False,
+)
+
+UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef = TypedDict(
+    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "GroupId": str,
+        "GroupName": str,
+        "IpPermissions": Sequence[IpPermissionTypeDef],
+        "SecurityGroupRuleDescriptions": Sequence[SecurityGroupRuleDescriptionTypeDef],
+    },
+    total=False,
+)
+
+UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef = TypedDict(
+    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "GroupId": str,
+        "GroupName": str,
+        "IpPermissions": Sequence[IpPermissionTypeDef],
+        "SecurityGroupRuleDescriptions": Sequence[SecurityGroupRuleDescriptionTypeDef],
+    },
+    total=False,
+)
+
+SecurityGroupVpcAddressTypeDef = TypedDict(
+    "SecurityGroupVpcAddressTypeDef",
+    {
+        "Description": str,
+        "GroupName": str,
+        "IpPermissions": List[IpPermissionVpcAddressTypeDef],
+        "OwnerId": str,
+        "GroupId": str,
+        "IpPermissionsEgress": List[IpPermissionVpcAddressTypeDef],
+        "Tags": List[TagTypeDef],
+        "VpcId": str,
+    },
+    total=False,
+)
+
 StaleSecurityGroupTypeDef = TypedDict(
     "StaleSecurityGroupTypeDef",
     {
         "Description": str,
         "GroupId": str,
         "GroupName": str,
         "StaleIpPermissions": List[StaleIpPermissionTypeDef],
@@ -26776,15 +28697,15 @@
         "CapacityReservationSpecification": (
             LaunchTemplateCapacityReservationSpecificationResponseTypeDef
         ),
         "LicenseSpecifications": List[LaunchTemplateLicenseConfigurationTypeDef],
         "HibernationOptions": LaunchTemplateHibernationOptionsTypeDef,
         "MetadataOptions": LaunchTemplateInstanceMetadataOptionsTypeDef,
         "EnclaveOptions": LaunchTemplateEnclaveOptionsTypeDef,
-        "InstanceRequirements": InstanceRequirementsOutputTypeDef,
+        "InstanceRequirements": InstanceRequirementsTypeDef,
         "PrivateDnsNameOptions": LaunchTemplatePrivateDnsNameOptionsTypeDef,
         "MaintenanceOptions": LaunchTemplateInstanceMaintenanceOptionsTypeDef,
         "DisableApiStop": bool,
     },
     total=False,
 )
 
@@ -26896,14 +28817,43 @@
     "ModifyVerifiedAccessTrustProviderResultTypeDef",
     {
         "VerifiedAccessTrustProvider": VerifiedAccessTrustProviderTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateNetworkInsightsPathRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateNetworkInsightsPathRequestRequestTypeDef",
+    {
+        "Source": str,
+        "Protocol": ProtocolType,
+        "ClientToken": str,
+    },
+)
+_OptionalCreateNetworkInsightsPathRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateNetworkInsightsPathRequestRequestTypeDef",
+    {
+        "SourceIp": str,
+        "DestinationIp": str,
+        "Destination": str,
+        "DestinationPort": int,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "DryRun": bool,
+        "FilterAtSource": PathRequestFilterTypeDef,
+        "FilterAtDestination": PathRequestFilterTypeDef,
+    },
+    total=False,
+)
+
+class CreateNetworkInsightsPathRequestRequestTypeDef(
+    _RequiredCreateNetworkInsightsPathRequestRequestTypeDef,
+    _OptionalCreateNetworkInsightsPathRequestRequestTypeDef,
+):
+    pass
+
 AccessScopePathRequestTypeDef = TypedDict(
     "AccessScopePathRequestTypeDef",
     {
         "Source": PathStatementRequestTypeDef,
         "Destination": PathStatementRequestTypeDef,
         "ThroughResources": Sequence[ThroughResourcesStatementRequestTypeDef],
     },
@@ -26993,29 +28943,14 @@
     {
         "SecurityGroupRules": List[SecurityGroupRuleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BundleTaskTypeDef = TypedDict(
-    "BundleTaskTypeDef",
-    {
-        "BundleId": str,
-        "BundleTaskError": BundleTaskErrorTypeDef,
-        "InstanceId": str,
-        "Progress": str,
-        "StartTime": datetime,
-        "State": BundleTaskStateType,
-        "Storage": StorageOutputTypeDef,
-        "UpdateTime": datetime,
-    },
-    total=False,
-)
-
 DescribeScheduledInstanceAvailabilityResultTypeDef = TypedDict(
     "DescribeScheduledInstanceAvailabilityResultTypeDef",
     {
         "NextToken": str,
         "ScheduledInstanceAvailabilitySet": List[ScheduledInstanceAvailabilityTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -27321,23 +29256,14 @@
         "TargetConfigurationValueRollup": ReservationValueTypeDef,
         "TargetConfigurationValueSet": List[TargetReservationValueTypeDef],
         "ValidationFailureReason": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoadBalancersConfigOutputTypeDef = TypedDict(
-    "LoadBalancersConfigOutputTypeDef",
-    {
-        "ClassicLoadBalancersConfig": ClassicLoadBalancersConfigOutputTypeDef,
-        "TargetGroupsConfig": TargetGroupsConfigOutputTypeDef,
-    },
-    total=False,
-)
-
 LoadBalancersConfigTypeDef = TypedDict(
     "LoadBalancersConfigTypeDef",
     {
         "ClassicLoadBalancersConfig": ClassicLoadBalancersConfigTypeDef,
         "TargetGroupsConfig": TargetGroupsConfigTypeDef,
     },
     total=False,
@@ -27929,14 +29855,39 @@
         "Status": VpcPeeringConnectionStateReasonTypeDef,
         "Tags": List[TagTypeDef],
         "VpcPeeringConnectionId": str,
     },
     total=False,
 )
 
+CreateLocalGatewayRouteTableResultTypeDef = TypedDict(
+    "CreateLocalGatewayRouteTableResultTypeDef",
+    {
+        "LocalGatewayRouteTable": LocalGatewayRouteTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteLocalGatewayRouteTableResultTypeDef = TypedDict(
+    "DeleteLocalGatewayRouteTableResultTypeDef",
+    {
+        "LocalGatewayRouteTable": LocalGatewayRouteTableTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLocalGatewayRouteTablesResultTypeDef = TypedDict(
+    "DescribeLocalGatewayRouteTablesResultTypeDef",
+    {
+        "LocalGatewayRouteTables": List[LocalGatewayRouteTableTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AssociateInstanceEventWindowResultTypeDef = TypedDict(
     "AssociateInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindow": InstanceEventWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -27970,1963 +29921,14 @@
     "ModifyInstanceEventWindowResultTypeDef",
     {
         "InstanceEventWindow": InstanceEventWindowTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAcceptAddressTransferRequestRequestTypeDef = TypedDict(
-    "_RequiredAcceptAddressTransferRequestRequestTypeDef",
-    {
-        "Address": str,
-    },
-)
-_OptionalAcceptAddressTransferRequestRequestTypeDef = TypedDict(
-    "_OptionalAcceptAddressTransferRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class AcceptAddressTransferRequestRequestTypeDef(
-    _RequiredAcceptAddressTransferRequestRequestTypeDef,
-    _OptionalAcceptAddressTransferRequestRequestTypeDef,
-):
-    pass
-
-AllocateAddressRequestRequestTypeDef = TypedDict(
-    "AllocateAddressRequestRequestTypeDef",
-    {
-        "Domain": DomainTypeType,
-        "Address": str,
-        "PublicIpv4Pool": str,
-        "NetworkBorderGroup": str,
-        "CustomerOwnedIpv4Pool": str,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-_RequiredAllocateHostsRequestRequestTypeDef = TypedDict(
-    "_RequiredAllocateHostsRequestRequestTypeDef",
-    {
-        "AvailabilityZone": str,
-    },
-)
-_OptionalAllocateHostsRequestRequestTypeDef = TypedDict(
-    "_OptionalAllocateHostsRequestRequestTypeDef",
-    {
-        "AutoPlacement": AutoPlacementType,
-        "ClientToken": str,
-        "InstanceType": str,
-        "InstanceFamily": str,
-        "Quantity": int,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "HostRecovery": HostRecoveryType,
-        "OutpostArn": str,
-        "HostMaintenance": HostMaintenanceType,
-        "AssetIds": Sequence[str],
-    },
-    total=False,
-)
-
-class AllocateHostsRequestRequestTypeDef(
-    _RequiredAllocateHostsRequestRequestTypeDef, _OptionalAllocateHostsRequestRequestTypeDef
-):
-    pass
-
-_RequiredAssociateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
-    "_RequiredAssociateIpamResourceDiscoveryRequestRequestTypeDef",
-    {
-        "IpamId": str,
-        "IpamResourceDiscoveryId": str,
-    },
-)
-_OptionalAssociateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
-    "_OptionalAssociateIpamResourceDiscoveryRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class AssociateIpamResourceDiscoveryRequestRequestTypeDef(
-    _RequiredAssociateIpamResourceDiscoveryRequestRequestTypeDef,
-    _OptionalAssociateIpamResourceDiscoveryRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCopySnapshotRequestRequestTypeDef = TypedDict(
-    "_RequiredCopySnapshotRequestRequestTypeDef",
-    {
-        "SourceRegion": str,
-        "SourceSnapshotId": str,
-    },
-)
-_OptionalCopySnapshotRequestRequestTypeDef = TypedDict(
-    "_OptionalCopySnapshotRequestRequestTypeDef",
-    {
-        "Description": str,
-        "DestinationOutpostArn": str,
-        "DestinationRegion": str,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "PresignedUrl": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CopySnapshotRequestRequestTypeDef(
-    _RequiredCopySnapshotRequestRequestTypeDef, _OptionalCopySnapshotRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateCapacityReservationFleetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCapacityReservationFleetRequestRequestTypeDef",
-    {
-        "InstanceTypeSpecifications": Sequence[ReservationFleetInstanceSpecificationTypeDef],
-        "TotalTargetCapacity": int,
-    },
-)
-_OptionalCreateCapacityReservationFleetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCapacityReservationFleetRequestRequestTypeDef",
-    {
-        "AllocationStrategy": str,
-        "ClientToken": str,
-        "Tenancy": Literal["default"],
-        "EndDate": TimestampTypeDef,
-        "InstanceMatchCriteria": Literal["open"],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateCapacityReservationFleetRequestRequestTypeDef(
-    _RequiredCreateCapacityReservationFleetRequestRequestTypeDef,
-    _OptionalCreateCapacityReservationFleetRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateCapacityReservationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCapacityReservationRequestRequestTypeDef",
-    {
-        "InstanceType": str,
-        "InstancePlatform": CapacityReservationInstancePlatformType,
-        "InstanceCount": int,
-    },
-)
-_OptionalCreateCapacityReservationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCapacityReservationRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "AvailabilityZone": str,
-        "AvailabilityZoneId": str,
-        "Tenancy": CapacityReservationTenancyType,
-        "EbsOptimized": bool,
-        "EphemeralStorage": bool,
-        "EndDate": TimestampTypeDef,
-        "EndDateType": EndDateTypeType,
-        "InstanceMatchCriteria": InstanceMatchCriteriaType,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "OutpostArn": str,
-        "PlacementGroupArn": str,
-    },
-    total=False,
-)
-
-class CreateCapacityReservationRequestRequestTypeDef(
-    _RequiredCreateCapacityReservationRequestRequestTypeDef,
-    _OptionalCreateCapacityReservationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateCarrierGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCarrierGatewayRequestRequestTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateCarrierGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCarrierGatewayRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class CreateCarrierGatewayRequestRequestTypeDef(
-    _RequiredCreateCarrierGatewayRequestRequestTypeDef,
-    _OptionalCreateCarrierGatewayRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateClientVpnEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateClientVpnEndpointRequestRequestTypeDef",
-    {
-        "ClientCidrBlock": str,
-        "ServerCertificateArn": str,
-        "AuthenticationOptions": Sequence[ClientVpnAuthenticationRequestTypeDef],
-        "ConnectionLogOptions": ConnectionLogOptionsTypeDef,
-    },
-)
-_OptionalCreateClientVpnEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateClientVpnEndpointRequestRequestTypeDef",
-    {
-        "DnsServers": Sequence[str],
-        "TransportProtocol": TransportProtocolType,
-        "VpnPort": int,
-        "Description": str,
-        "SplitTunnel": bool,
-        "DryRun": bool,
-        "ClientToken": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "SecurityGroupIds": Sequence[str],
-        "VpcId": str,
-        "SelfServicePortal": SelfServicePortalType,
-        "ClientConnectOptions": ClientConnectOptionsTypeDef,
-        "SessionTimeoutHours": int,
-        "ClientLoginBannerOptions": ClientLoginBannerOptionsTypeDef,
-    },
-    total=False,
-)
-
-class CreateClientVpnEndpointRequestRequestTypeDef(
-    _RequiredCreateClientVpnEndpointRequestRequestTypeDef,
-    _OptionalCreateClientVpnEndpointRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateCoipPoolRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCoipPoolRequestRequestTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-    },
-)
-_OptionalCreateCoipPoolRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCoipPoolRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateCoipPoolRequestRequestTypeDef(
-    _RequiredCreateCoipPoolRequestRequestTypeDef, _OptionalCreateCoipPoolRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateCustomerGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCustomerGatewayRequestRequestTypeDef",
-    {
-        "Type": Literal["ipsec.1"],
-    },
-)
-_OptionalCreateCustomerGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCustomerGatewayRequestRequestTypeDef",
-    {
-        "BgpAsn": int,
-        "PublicIp": str,
-        "CertificateArn": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DeviceName": str,
-        "IpAddress": str,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateCustomerGatewayRequestRequestTypeDef(
-    _RequiredCreateCustomerGatewayRequestRequestTypeDef,
-    _OptionalCreateCustomerGatewayRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateDhcpOptionsRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDhcpOptionsRequestRequestTypeDef",
-    {
-        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
-    },
-)
-_OptionalCreateDhcpOptionsRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDhcpOptionsRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateDhcpOptionsRequestRequestTypeDef(
-    _RequiredCreateDhcpOptionsRequestRequestTypeDef, _OptionalCreateDhcpOptionsRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef = TypedDict(
-    "_RequiredCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
-    {
-        "DhcpConfigurations": Sequence[NewDhcpConfigurationTypeDef],
-    },
-)
-_OptionalCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef = TypedDict(
-    "_OptionalCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef(
-    _RequiredCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef,
-    _OptionalCreateDhcpOptionsRequestServiceResourceCreateDhcpOptionsTypeDef,
-):
-    pass
-
-_RequiredCreateEgressOnlyInternetGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEgressOnlyInternetGatewayRequestRequestTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateEgressOnlyInternetGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEgressOnlyInternetGatewayRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateEgressOnlyInternetGatewayRequestRequestTypeDef(
-    _RequiredCreateEgressOnlyInternetGatewayRequestRequestTypeDef,
-    _OptionalCreateEgressOnlyInternetGatewayRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateFlowLogsRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFlowLogsRequestRequestTypeDef",
-    {
-        "ResourceIds": Sequence[str],
-        "ResourceType": FlowLogsResourceTypeType,
-    },
-)
-_OptionalCreateFlowLogsRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFlowLogsRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "ClientToken": str,
-        "DeliverLogsPermissionArn": str,
-        "DeliverCrossAccountRole": str,
-        "LogGroupName": str,
-        "TrafficType": TrafficTypeType,
-        "LogDestinationType": LogDestinationTypeType,
-        "LogDestination": str,
-        "LogFormat": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "MaxAggregationInterval": int,
-        "DestinationOptions": DestinationOptionsRequestTypeDef,
-    },
-    total=False,
-)
-
-class CreateFlowLogsRequestRequestTypeDef(
-    _RequiredCreateFlowLogsRequestRequestTypeDef, _OptionalCreateFlowLogsRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateFpgaImageRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFpgaImageRequestRequestTypeDef",
-    {
-        "InputStorageLocation": StorageLocationTypeDef,
-    },
-)
-_OptionalCreateFpgaImageRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFpgaImageRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "LogsStorageLocation": StorageLocationTypeDef,
-        "Description": str,
-        "Name": str,
-        "ClientToken": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateFpgaImageRequestRequestTypeDef(
-    _RequiredCreateFpgaImageRequestRequestTypeDef, _OptionalCreateFpgaImageRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateImageRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateImageRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-        "Name": str,
-    },
-)
-_OptionalCreateImageRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateImageRequestRequestTypeDef",
-    {
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
-        "Description": str,
-        "DryRun": bool,
-        "NoReboot": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateImageRequestRequestTypeDef(
-    _RequiredCreateImageRequestRequestTypeDef, _OptionalCreateImageRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateInstanceConnectEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInstanceConnectEndpointRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-    },
-)
-_OptionalCreateInstanceConnectEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInstanceConnectEndpointRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "SecurityGroupIds": Sequence[str],
-        "PreserveClientIp": bool,
-        "ClientToken": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateInstanceConnectEndpointRequestRequestTypeDef(
-    _RequiredCreateInstanceConnectEndpointRequestRequestTypeDef,
-    _OptionalCreateInstanceConnectEndpointRequestRequestTypeDef,
-):
-    pass
-
-CreateInstanceEventWindowRequestRequestTypeDef = TypedDict(
-    "CreateInstanceEventWindowRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "Name": str,
-        "TimeRanges": Sequence[InstanceEventWindowTimeRangeRequestTypeDef],
-        "CronExpression": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateInstanceExportTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateInstanceExportTaskRequestRequestTypeDef",
-    {
-        "ExportToS3Task": ExportToS3TaskSpecificationTypeDef,
-        "InstanceId": str,
-        "TargetEnvironment": ExportEnvironmentType,
-    },
-)
-_OptionalCreateInstanceExportTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateInstanceExportTaskRequestRequestTypeDef",
-    {
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateInstanceExportTaskRequestRequestTypeDef(
-    _RequiredCreateInstanceExportTaskRequestRequestTypeDef,
-    _OptionalCreateInstanceExportTaskRequestRequestTypeDef,
-):
-    pass
-
-CreateInternetGatewayRequestRequestTypeDef = TypedDict(
-    "CreateInternetGatewayRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef = TypedDict(
-    "CreateInternetGatewayRequestServiceResourceCreateInternetGatewayTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-_RequiredCreateIpamPoolRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIpamPoolRequestRequestTypeDef",
-    {
-        "IpamScopeId": str,
-        "AddressFamily": AddressFamilyType,
-    },
-)
-_OptionalCreateIpamPoolRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIpamPoolRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "Locale": str,
-        "SourceIpamPoolId": str,
-        "Description": str,
-        "AutoImport": bool,
-        "PubliclyAdvertisable": bool,
-        "AllocationMinNetmaskLength": int,
-        "AllocationMaxNetmaskLength": int,
-        "AllocationDefaultNetmaskLength": int,
-        "AllocationResourceTags": Sequence[RequestIpamResourceTagTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-        "AwsService": Literal["ec2"],
-        "PublicIpSource": IpamPoolPublicIpSourceType,
-    },
-    total=False,
-)
-
-class CreateIpamPoolRequestRequestTypeDef(
-    _RequiredCreateIpamPoolRequestRequestTypeDef, _OptionalCreateIpamPoolRequestRequestTypeDef
-):
-    pass
-
-CreateIpamRequestRequestTypeDef = TypedDict(
-    "CreateIpamRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "Description": str,
-        "OperatingRegions": Sequence[AddIpamOperatingRegionTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-CreateIpamResourceDiscoveryRequestRequestTypeDef = TypedDict(
-    "CreateIpamResourceDiscoveryRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "Description": str,
-        "OperatingRegions": Sequence[AddIpamOperatingRegionTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-_RequiredCreateIpamScopeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateIpamScopeRequestRequestTypeDef",
-    {
-        "IpamId": str,
-    },
-)
-_OptionalCreateIpamScopeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateIpamScopeRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class CreateIpamScopeRequestRequestTypeDef(
-    _RequiredCreateIpamScopeRequestRequestTypeDef, _OptionalCreateIpamScopeRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateKeyPairRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateKeyPairRequestRequestTypeDef",
-    {
-        "KeyName": str,
-    },
-)
-_OptionalCreateKeyPairRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateKeyPairRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "KeyType": KeyTypeType,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "KeyFormat": KeyFormatType,
-    },
-    total=False,
-)
-
-class CreateKeyPairRequestRequestTypeDef(
-    _RequiredCreateKeyPairRequestRequestTypeDef, _OptionalCreateKeyPairRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef = TypedDict(
-    "_RequiredCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
-    {
-        "KeyName": str,
-    },
-)
-_OptionalCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef = TypedDict(
-    "_OptionalCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef",
-    {
-        "DryRun": bool,
-        "KeyType": KeyTypeType,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "KeyFormat": KeyFormatType,
-    },
-    total=False,
-)
-
-class CreateKeyPairRequestServiceResourceCreateKeyPairTypeDef(
-    _RequiredCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef,
-    _OptionalCreateKeyPairRequestServiceResourceCreateKeyPairTypeDef,
-):
-    pass
-
-_RequiredCreateLocalGatewayRouteTableRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLocalGatewayRouteTableRequestRequestTypeDef",
-    {
-        "LocalGatewayId": str,
-    },
-)
-_OptionalCreateLocalGatewayRouteTableRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLocalGatewayRouteTableRequestRequestTypeDef",
-    {
-        "Mode": LocalGatewayRouteTableModeType,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateLocalGatewayRouteTableRequestRequestTypeDef(
-    _RequiredCreateLocalGatewayRouteTableRequestRequestTypeDef,
-    _OptionalCreateLocalGatewayRouteTableRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-        "LocalGatewayVirtualInterfaceGroupId": str,
-    },
-)
-_OptionalCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef(
-    _RequiredCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef,
-    _OptionalCreateLocalGatewayRouteTableVirtualInterfaceGroupAssociationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
-    {
-        "LocalGatewayRouteTableId": str,
-        "VpcId": str,
-    },
-)
-_OptionalCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef(
-    _RequiredCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef,
-    _OptionalCreateLocalGatewayRouteTableVpcAssociationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateManagedPrefixListRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateManagedPrefixListRequestRequestTypeDef",
-    {
-        "PrefixListName": str,
-        "MaxEntries": int,
-        "AddressFamily": str,
-    },
-)
-_OptionalCreateManagedPrefixListRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateManagedPrefixListRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "Entries": Sequence[AddPrefixListEntryTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class CreateManagedPrefixListRequestRequestTypeDef(
-    _RequiredCreateManagedPrefixListRequestRequestTypeDef,
-    _OptionalCreateManagedPrefixListRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateNatGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNatGatewayRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-    },
-)
-_OptionalCreateNatGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNatGatewayRequestRequestTypeDef",
-    {
-        "AllocationId": str,
-        "ClientToken": str,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ConnectivityType": ConnectivityTypeType,
-        "PrivateIpAddress": str,
-        "SecondaryAllocationIds": Sequence[str],
-        "SecondaryPrivateIpAddresses": Sequence[str],
-        "SecondaryPrivateIpAddressCount": int,
-    },
-    total=False,
-)
-
-class CreateNatGatewayRequestRequestTypeDef(
-    _RequiredCreateNatGatewayRequestRequestTypeDef, _OptionalCreateNatGatewayRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateNetworkAclRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNetworkAclRequestRequestTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateNetworkAclRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNetworkAclRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateNetworkAclRequestRequestTypeDef(
-    _RequiredCreateNetworkAclRequestRequestTypeDef, _OptionalCreateNetworkAclRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef = TypedDict(
-    "_RequiredCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef = TypedDict(
-    "_OptionalCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef(
-    _RequiredCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef,
-    _OptionalCreateNetworkAclRequestServiceResourceCreateNetworkAclTypeDef,
-):
-    pass
-
-_RequiredCreateNetworkInsightsPathRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNetworkInsightsPathRequestRequestTypeDef",
-    {
-        "Source": str,
-        "Protocol": ProtocolType,
-        "ClientToken": str,
-    },
-)
-_OptionalCreateNetworkInsightsPathRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNetworkInsightsPathRequestRequestTypeDef",
-    {
-        "SourceIp": str,
-        "DestinationIp": str,
-        "Destination": str,
-        "DestinationPort": int,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "FilterAtSource": PathRequestFilterTypeDef,
-        "FilterAtDestination": PathRequestFilterTypeDef,
-    },
-    total=False,
-)
-
-class CreateNetworkInsightsPathRequestRequestTypeDef(
-    _RequiredCreateNetworkInsightsPathRequestRequestTypeDef,
-    _OptionalCreateNetworkInsightsPathRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateNetworkInterfaceRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateNetworkInterfaceRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-    },
-)
-_OptionalCreateNetworkInterfaceRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateNetworkInterfaceRequestRequestTypeDef",
-    {
-        "Description": str,
-        "DryRun": bool,
-        "Groups": Sequence[str],
-        "Ipv6AddressCount": int,
-        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
-        "PrivateIpAddress": str,
-        "PrivateIpAddresses": Sequence[PrivateIpAddressSpecificationTypeDef],
-        "SecondaryPrivateIpAddressCount": int,
-        "Ipv4Prefixes": Sequence[Ipv4PrefixSpecificationRequestTypeDef],
-        "Ipv4PrefixCount": int,
-        "Ipv6Prefixes": Sequence[Ipv6PrefixSpecificationRequestTypeDef],
-        "Ipv6PrefixCount": int,
-        "InterfaceType": NetworkInterfaceCreationTypeType,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class CreateNetworkInterfaceRequestRequestTypeDef(
-    _RequiredCreateNetworkInterfaceRequestRequestTypeDef,
-    _OptionalCreateNetworkInterfaceRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef = TypedDict(
-    "_RequiredCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
-    {
-        "SubnetId": str,
-    },
-)
-_OptionalCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef = TypedDict(
-    "_OptionalCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef",
-    {
-        "Description": str,
-        "DryRun": bool,
-        "Groups": Sequence[str],
-        "Ipv6AddressCount": int,
-        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
-        "PrivateIpAddress": str,
-        "PrivateIpAddresses": Sequence[PrivateIpAddressSpecificationTypeDef],
-        "SecondaryPrivateIpAddressCount": int,
-        "Ipv4Prefixes": Sequence[Ipv4PrefixSpecificationRequestTypeDef],
-        "Ipv4PrefixCount": int,
-        "Ipv6Prefixes": Sequence[Ipv6PrefixSpecificationRequestTypeDef],
-        "Ipv6PrefixCount": int,
-        "InterfaceType": NetworkInterfaceCreationTypeType,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class CreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef(
-    _RequiredCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef,
-    _OptionalCreateNetworkInterfaceRequestServiceResourceCreateNetworkInterfaceTypeDef,
-):
-    pass
-
-CreatePlacementGroupRequestRequestTypeDef = TypedDict(
-    "CreatePlacementGroupRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "GroupName": str,
-        "Strategy": PlacementStrategyType,
-        "PartitionCount": int,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "SpreadLevel": SpreadLevelType,
-    },
-    total=False,
-)
-
-CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef = TypedDict(
-    "CreatePlacementGroupRequestServiceResourceCreatePlacementGroupTypeDef",
-    {
-        "DryRun": bool,
-        "GroupName": str,
-        "Strategy": PlacementStrategyType,
-        "PartitionCount": int,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "SpreadLevel": SpreadLevelType,
-    },
-    total=False,
-)
-
-CreatePublicIpv4PoolRequestRequestTypeDef = TypedDict(
-    "CreatePublicIpv4PoolRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateReplaceRootVolumeTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReplaceRootVolumeTaskRequestRequestTypeDef",
-    {
-        "InstanceId": str,
-    },
-)
-_OptionalCreateReplaceRootVolumeTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReplaceRootVolumeTaskRequestRequestTypeDef",
-    {
-        "SnapshotId": str,
-        "ClientToken": str,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ImageId": str,
-        "DeleteReplacedRootVolume": bool,
-    },
-    total=False,
-)
-
-class CreateReplaceRootVolumeTaskRequestRequestTypeDef(
-    _RequiredCreateReplaceRootVolumeTaskRequestRequestTypeDef,
-    _OptionalCreateReplaceRootVolumeTaskRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateRestoreImageTaskRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRestoreImageTaskRequestRequestTypeDef",
-    {
-        "Bucket": str,
-        "ObjectKey": str,
-    },
-)
-_OptionalCreateRestoreImageTaskRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRestoreImageTaskRequestRequestTypeDef",
-    {
-        "Name": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateRestoreImageTaskRequestRequestTypeDef(
-    _RequiredCreateRestoreImageTaskRequestRequestTypeDef,
-    _OptionalCreateRestoreImageTaskRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateRouteTableRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRouteTableRequestRequestTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateRouteTableRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRouteTableRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateRouteTableRequestRequestTypeDef(
-    _RequiredCreateRouteTableRequestRequestTypeDef, _OptionalCreateRouteTableRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef = TypedDict(
-    "_RequiredCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef = TypedDict(
-    "_OptionalCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateRouteTableRequestServiceResourceCreateRouteTableTypeDef(
-    _RequiredCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef,
-    _OptionalCreateRouteTableRequestServiceResourceCreateRouteTableTypeDef,
-):
-    pass
-
-_RequiredCreateSecurityGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSecurityGroupRequestRequestTypeDef",
-    {
-        "Description": str,
-        "GroupName": str,
-    },
-)
-_OptionalCreateSecurityGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSecurityGroupRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateSecurityGroupRequestRequestTypeDef(
-    _RequiredCreateSecurityGroupRequestRequestTypeDef,
-    _OptionalCreateSecurityGroupRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef = TypedDict(
-    "_RequiredCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
-    {
-        "Description": str,
-        "GroupName": str,
-    },
-)
-_OptionalCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef = TypedDict(
-    "_OptionalCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef",
-    {
-        "VpcId": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef(
-    _RequiredCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef,
-    _OptionalCreateSecurityGroupRequestServiceResourceCreateSecurityGroupTypeDef,
-):
-    pass
-
-_RequiredCreateSnapshotRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSnapshotRequestRequestTypeDef",
-    {
-        "VolumeId": str,
-    },
-)
-_OptionalCreateSnapshotRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSnapshotRequestRequestTypeDef",
-    {
-        "Description": str,
-        "OutpostArn": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateSnapshotRequestRequestTypeDef(
-    _RequiredCreateSnapshotRequestRequestTypeDef, _OptionalCreateSnapshotRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef = TypedDict(
-    "_RequiredCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
-    {
-        "VolumeId": str,
-    },
-)
-_OptionalCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef = TypedDict(
-    "_OptionalCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef",
-    {
-        "Description": str,
-        "OutpostArn": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateSnapshotRequestServiceResourceCreateSnapshotTypeDef(
-    _RequiredCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef,
-    _OptionalCreateSnapshotRequestServiceResourceCreateSnapshotTypeDef,
-):
-    pass
-
-_RequiredCreateSnapshotsRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSnapshotsRequestRequestTypeDef",
-    {
-        "InstanceSpecification": InstanceSpecificationTypeDef,
-    },
-)
-_OptionalCreateSnapshotsRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSnapshotsRequestRequestTypeDef",
-    {
-        "Description": str,
-        "OutpostArn": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "CopyTagsFromSource": Literal["volume"],
-    },
-    total=False,
-)
-
-class CreateSnapshotsRequestRequestTypeDef(
-    _RequiredCreateSnapshotsRequestRequestTypeDef, _OptionalCreateSnapshotsRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateSubnetCidrReservationRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSubnetCidrReservationRequestRequestTypeDef",
-    {
-        "SubnetId": str,
-        "Cidr": str,
-        "ReservationType": SubnetCidrReservationTypeType,
-    },
-)
-_OptionalCreateSubnetCidrReservationRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSubnetCidrReservationRequestRequestTypeDef",
-    {
-        "Description": str,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateSubnetCidrReservationRequestRequestTypeDef(
-    _RequiredCreateSubnetCidrReservationRequestRequestTypeDef,
-    _OptionalCreateSubnetCidrReservationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateSubnetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateSubnetRequestRequestTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateSubnetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateSubnetRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "AvailabilityZone": str,
-        "AvailabilityZoneId": str,
-        "CidrBlock": str,
-        "Ipv6CidrBlock": str,
-        "OutpostArn": str,
-        "DryRun": bool,
-        "Ipv6Native": bool,
-    },
-    total=False,
-)
-
-class CreateSubnetRequestRequestTypeDef(
-    _RequiredCreateSubnetRequestRequestTypeDef, _OptionalCreateSubnetRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateSubnetRequestServiceResourceCreateSubnetTypeDef = TypedDict(
-    "_RequiredCreateSubnetRequestServiceResourceCreateSubnetTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateSubnetRequestServiceResourceCreateSubnetTypeDef = TypedDict(
-    "_OptionalCreateSubnetRequestServiceResourceCreateSubnetTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "AvailabilityZone": str,
-        "AvailabilityZoneId": str,
-        "CidrBlock": str,
-        "Ipv6CidrBlock": str,
-        "OutpostArn": str,
-        "DryRun": bool,
-        "Ipv6Native": bool,
-    },
-    total=False,
-)
-
-class CreateSubnetRequestServiceResourceCreateSubnetTypeDef(
-    _RequiredCreateSubnetRequestServiceResourceCreateSubnetTypeDef,
-    _OptionalCreateSubnetRequestServiceResourceCreateSubnetTypeDef,
-):
-    pass
-
-CreateTrafficMirrorFilterRequestRequestTypeDef = TypedDict(
-    "CreateTrafficMirrorFilterRequestRequestTypeDef",
-    {
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-_RequiredCreateTrafficMirrorSessionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTrafficMirrorSessionRequestRequestTypeDef",
-    {
-        "NetworkInterfaceId": str,
-        "TrafficMirrorTargetId": str,
-        "TrafficMirrorFilterId": str,
-        "SessionNumber": int,
-    },
-)
-_OptionalCreateTrafficMirrorSessionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTrafficMirrorSessionRequestRequestTypeDef",
-    {
-        "PacketLength": int,
-        "VirtualNetworkId": int,
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class CreateTrafficMirrorSessionRequestRequestTypeDef(
-    _RequiredCreateTrafficMirrorSessionRequestRequestTypeDef,
-    _OptionalCreateTrafficMirrorSessionRequestRequestTypeDef,
-):
-    pass
-
-CreateTrafficMirrorTargetRequestRequestTypeDef = TypedDict(
-    "CreateTrafficMirrorTargetRequestRequestTypeDef",
-    {
-        "NetworkInterfaceId": str,
-        "NetworkLoadBalancerArn": str,
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-        "ClientToken": str,
-        "GatewayLoadBalancerEndpointId": str,
-    },
-    total=False,
-)
-
-_RequiredCreateTransitGatewayConnectPeerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayConnectPeerRequestRequestTypeDef",
-    {
-        "TransitGatewayAttachmentId": str,
-        "PeerAddress": str,
-        "InsideCidrBlocks": Sequence[str],
-    },
-)
-_OptionalCreateTransitGatewayConnectPeerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayConnectPeerRequestRequestTypeDef",
-    {
-        "TransitGatewayAddress": str,
-        "BgpOptions": TransitGatewayConnectRequestBgpOptionsTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateTransitGatewayConnectPeerRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayConnectPeerRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayConnectPeerRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateTransitGatewayConnectRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayConnectRequestRequestTypeDef",
-    {
-        "TransportTransitGatewayAttachmentId": str,
-        "Options": CreateTransitGatewayConnectRequestOptionsTypeDef,
-    },
-)
-_OptionalCreateTransitGatewayConnectRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayConnectRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateTransitGatewayConnectRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayConnectRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayConnectRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateTransitGatewayMulticastDomainRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayMulticastDomainRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-    },
-)
-_OptionalCreateTransitGatewayMulticastDomainRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayMulticastDomainRequestRequestTypeDef",
-    {
-        "Options": CreateTransitGatewayMulticastDomainRequestOptionsTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateTransitGatewayMulticastDomainRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayMulticastDomainRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayMulticastDomainRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "PeerTransitGatewayId": str,
-        "PeerAccountId": str,
-        "PeerRegion": str,
-    },
-)
-_OptionalCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef",
-    {
-        "Options": CreateTransitGatewayPeeringAttachmentRequestOptionsTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateTransitGatewayPeeringAttachmentRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayPeeringAttachmentRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateTransitGatewayPolicyTableRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayPolicyTableRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-    },
-)
-_OptionalCreateTransitGatewayPolicyTableRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayPolicyTableRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateTransitGatewayPolicyTableRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayPolicyTableRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayPolicyTableRequestRequestTypeDef,
-):
-    pass
-
-CreateTransitGatewayRequestRequestTypeDef = TypedDict(
-    "CreateTransitGatewayRequestRequestTypeDef",
-    {
-        "Description": str,
-        "Options": TransitGatewayRequestOptionsTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-_RequiredCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
-    {
-        "TransitGatewayRouteTableId": str,
-        "PeeringAttachmentId": str,
-    },
-)
-_OptionalCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayRouteTableAnnouncementRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayRouteTableRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-    },
-)
-_OptionalCreateTransitGatewayRouteTableRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayRouteTableRequestRequestTypeDef",
-    {
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateTransitGatewayRouteTableRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayRouteTableRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayRouteTableRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateTransitGatewayVpcAttachmentRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
-    {
-        "TransitGatewayId": str,
-        "VpcId": str,
-        "SubnetIds": Sequence[str],
-    },
-)
-_OptionalCreateTransitGatewayVpcAttachmentRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateTransitGatewayVpcAttachmentRequestRequestTypeDef",
-    {
-        "Options": CreateTransitGatewayVpcAttachmentRequestOptionsTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateTransitGatewayVpcAttachmentRequestRequestTypeDef(
-    _RequiredCreateTransitGatewayVpcAttachmentRequestRequestTypeDef,
-    _OptionalCreateTransitGatewayVpcAttachmentRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateVerifiedAccessEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVerifiedAccessEndpointRequestRequestTypeDef",
-    {
-        "VerifiedAccessGroupId": str,
-        "EndpointType": VerifiedAccessEndpointTypeType,
-        "AttachmentType": Literal["vpc"],
-        "DomainCertificateArn": str,
-        "ApplicationDomain": str,
-        "EndpointDomainPrefix": str,
-    },
-)
-_OptionalCreateVerifiedAccessEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVerifiedAccessEndpointRequestRequestTypeDef",
-    {
-        "SecurityGroupIds": Sequence[str],
-        "LoadBalancerOptions": CreateVerifiedAccessEndpointLoadBalancerOptionsTypeDef,
-        "NetworkInterfaceOptions": CreateVerifiedAccessEndpointEniOptionsTypeDef,
-        "Description": str,
-        "PolicyDocument": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateVerifiedAccessEndpointRequestRequestTypeDef(
-    _RequiredCreateVerifiedAccessEndpointRequestRequestTypeDef,
-    _OptionalCreateVerifiedAccessEndpointRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateVerifiedAccessGroupRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVerifiedAccessGroupRequestRequestTypeDef",
-    {
-        "VerifiedAccessInstanceId": str,
-    },
-)
-_OptionalCreateVerifiedAccessGroupRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVerifiedAccessGroupRequestRequestTypeDef",
-    {
-        "Description": str,
-        "PolicyDocument": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateVerifiedAccessGroupRequestRequestTypeDef(
-    _RequiredCreateVerifiedAccessGroupRequestRequestTypeDef,
-    _OptionalCreateVerifiedAccessGroupRequestRequestTypeDef,
-):
-    pass
-
-CreateVerifiedAccessInstanceRequestRequestTypeDef = TypedDict(
-    "CreateVerifiedAccessInstanceRequestRequestTypeDef",
-    {
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-_RequiredCreateVerifiedAccessTrustProviderRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVerifiedAccessTrustProviderRequestRequestTypeDef",
-    {
-        "TrustProviderType": TrustProviderTypeType,
-        "PolicyReferenceName": str,
-    },
-)
-_OptionalCreateVerifiedAccessTrustProviderRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVerifiedAccessTrustProviderRequestRequestTypeDef",
-    {
-        "UserTrustProviderType": UserTrustProviderTypeType,
-        "DeviceTrustProviderType": DeviceTrustProviderTypeType,
-        "OidcOptions": CreateVerifiedAccessTrustProviderOidcOptionsTypeDef,
-        "DeviceOptions": CreateVerifiedAccessTrustProviderDeviceOptionsTypeDef,
-        "Description": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "ClientToken": str,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateVerifiedAccessTrustProviderRequestRequestTypeDef(
-    _RequiredCreateVerifiedAccessTrustProviderRequestRequestTypeDef,
-    _OptionalCreateVerifiedAccessTrustProviderRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateVolumeRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVolumeRequestRequestTypeDef",
-    {
-        "AvailabilityZone": str,
-    },
-)
-_OptionalCreateVolumeRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVolumeRequestRequestTypeDef",
-    {
-        "Encrypted": bool,
-        "Iops": int,
-        "KmsKeyId": str,
-        "OutpostArn": str,
-        "Size": int,
-        "SnapshotId": str,
-        "VolumeType": VolumeTypeType,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "MultiAttachEnabled": bool,
-        "Throughput": int,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class CreateVolumeRequestRequestTypeDef(
-    _RequiredCreateVolumeRequestRequestTypeDef, _OptionalCreateVolumeRequestRequestTypeDef
-):
-    pass
-
-_RequiredCreateVolumeRequestServiceResourceCreateVolumeTypeDef = TypedDict(
-    "_RequiredCreateVolumeRequestServiceResourceCreateVolumeTypeDef",
-    {
-        "AvailabilityZone": str,
-    },
-)
-_OptionalCreateVolumeRequestServiceResourceCreateVolumeTypeDef = TypedDict(
-    "_OptionalCreateVolumeRequestServiceResourceCreateVolumeTypeDef",
-    {
-        "Encrypted": bool,
-        "Iops": int,
-        "KmsKeyId": str,
-        "OutpostArn": str,
-        "Size": int,
-        "SnapshotId": str,
-        "VolumeType": VolumeTypeType,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "MultiAttachEnabled": bool,
-        "Throughput": int,
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class CreateVolumeRequestServiceResourceCreateVolumeTypeDef(
-    _RequiredCreateVolumeRequestServiceResourceCreateVolumeTypeDef,
-    _OptionalCreateVolumeRequestServiceResourceCreateVolumeTypeDef,
-):
-    pass
-
-_RequiredCreateVpcEndpointRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVpcEndpointRequestRequestTypeDef",
-    {
-        "VpcId": str,
-        "ServiceName": str,
-    },
-)
-_OptionalCreateVpcEndpointRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVpcEndpointRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "VpcEndpointType": VpcEndpointTypeType,
-        "PolicyDocument": str,
-        "RouteTableIds": Sequence[str],
-        "SubnetIds": Sequence[str],
-        "SecurityGroupIds": Sequence[str],
-        "IpAddressType": IpAddressTypeType,
-        "DnsOptions": DnsOptionsSpecificationTypeDef,
-        "ClientToken": str,
-        "PrivateDnsEnabled": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateVpcEndpointRequestRequestTypeDef(
-    _RequiredCreateVpcEndpointRequestRequestTypeDef, _OptionalCreateVpcEndpointRequestRequestTypeDef
-):
-    pass
-
-CreateVpcEndpointServiceConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateVpcEndpointServiceConfigurationRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "AcceptanceRequired": bool,
-        "PrivateDnsName": str,
-        "NetworkLoadBalancerArns": Sequence[str],
-        "GatewayLoadBalancerArns": Sequence[str],
-        "SupportedIpAddressTypes": Sequence[str],
-        "ClientToken": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateVpcPeeringConnectionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVpcPeeringConnectionRequestRequestTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateVpcPeeringConnectionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVpcPeeringConnectionRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "PeerOwnerId": str,
-        "PeerVpcId": str,
-        "PeerRegion": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateVpcPeeringConnectionRequestRequestTypeDef(
-    _RequiredCreateVpcPeeringConnectionRequestRequestTypeDef,
-    _OptionalCreateVpcPeeringConnectionRequestRequestTypeDef,
-):
-    pass
-
-_RequiredCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef = TypedDict(
-    "_RequiredCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
-    {
-        "VpcId": str,
-    },
-)
-_OptionalCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef = TypedDict(
-    "_OptionalCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef",
-    {
-        "DryRun": bool,
-        "PeerOwnerId": str,
-        "PeerVpcId": str,
-        "PeerRegion": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class CreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef(
-    _RequiredCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef,
-    _OptionalCreateVpcPeeringConnectionRequestServiceResourceCreateVpcPeeringConnectionTypeDef,
-):
-    pass
-
-CreateVpcRequestRequestTypeDef = TypedDict(
-    "CreateVpcRequestRequestTypeDef",
-    {
-        "CidrBlock": str,
-        "AmazonProvidedIpv6CidrBlock": bool,
-        "Ipv6Pool": str,
-        "Ipv6CidrBlock": str,
-        "Ipv4IpamPoolId": str,
-        "Ipv4NetmaskLength": int,
-        "Ipv6IpamPoolId": str,
-        "Ipv6NetmaskLength": int,
-        "DryRun": bool,
-        "InstanceTenancy": TenancyType,
-        "Ipv6CidrBlockNetworkBorderGroup": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-CreateVpcRequestServiceResourceCreateVpcTypeDef = TypedDict(
-    "CreateVpcRequestServiceResourceCreateVpcTypeDef",
-    {
-        "CidrBlock": str,
-        "AmazonProvidedIpv6CidrBlock": bool,
-        "Ipv6Pool": str,
-        "Ipv6CidrBlock": str,
-        "Ipv4IpamPoolId": str,
-        "Ipv4NetmaskLength": int,
-        "Ipv6IpamPoolId": str,
-        "Ipv6NetmaskLength": int,
-        "DryRun": bool,
-        "InstanceTenancy": TenancyType,
-        "Ipv6CidrBlockNetworkBorderGroup": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-_RequiredCreateVpnGatewayRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateVpnGatewayRequestRequestTypeDef",
-    {
-        "Type": Literal["ipsec.1"],
-    },
-)
-_OptionalCreateVpnGatewayRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateVpnGatewayRequestRequestTypeDef",
-    {
-        "AvailabilityZone": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "AmazonSideAsn": int,
-        "DryRun": bool,
-    },
-    total=False,
-)
-
-class CreateVpnGatewayRequestRequestTypeDef(
-    _RequiredCreateVpnGatewayRequestRequestTypeDef, _OptionalCreateVpnGatewayRequestRequestTypeDef
-):
-    pass
-
-_RequiredExportImageRequestRequestTypeDef = TypedDict(
-    "_RequiredExportImageRequestRequestTypeDef",
-    {
-        "DiskImageFormat": DiskImageFormatType,
-        "ImageId": str,
-        "S3ExportLocation": ExportTaskS3LocationRequestTypeDef,
-    },
-)
-_OptionalExportImageRequestRequestTypeDef = TypedDict(
-    "_OptionalExportImageRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "Description": str,
-        "DryRun": bool,
-        "RoleName": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class ExportImageRequestRequestTypeDef(
-    _RequiredExportImageRequestRequestTypeDef, _OptionalExportImageRequestRequestTypeDef
-):
-    pass
-
-ImportImageRequestRequestTypeDef = TypedDict(
-    "ImportImageRequestRequestTypeDef",
-    {
-        "Architecture": str,
-        "ClientData": ClientDataTypeDef,
-        "ClientToken": str,
-        "Description": str,
-        "DiskContainers": Sequence[ImageDiskContainerTypeDef],
-        "DryRun": bool,
-        "Encrypted": bool,
-        "Hypervisor": str,
-        "KmsKeyId": str,
-        "LicenseType": str,
-        "Platform": str,
-        "RoleName": str,
-        "LicenseSpecifications": Sequence[ImportImageLicenseConfigurationRequestTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "UsageOperation": str,
-        "BootMode": BootModeValuesType,
-    },
-    total=False,
-)
-
-_RequiredImportKeyPairRequestRequestTypeDef = TypedDict(
-    "_RequiredImportKeyPairRequestRequestTypeDef",
-    {
-        "KeyName": str,
-        "PublicKeyMaterial": BlobTypeDef,
-    },
-)
-_OptionalImportKeyPairRequestRequestTypeDef = TypedDict(
-    "_OptionalImportKeyPairRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class ImportKeyPairRequestRequestTypeDef(
-    _RequiredImportKeyPairRequestRequestTypeDef, _OptionalImportKeyPairRequestRequestTypeDef
-):
-    pass
-
-_RequiredImportKeyPairRequestServiceResourceImportKeyPairTypeDef = TypedDict(
-    "_RequiredImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
-    {
-        "KeyName": str,
-        "PublicKeyMaterial": BlobTypeDef,
-    },
-)
-_OptionalImportKeyPairRequestServiceResourceImportKeyPairTypeDef = TypedDict(
-    "_OptionalImportKeyPairRequestServiceResourceImportKeyPairTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class ImportKeyPairRequestServiceResourceImportKeyPairTypeDef(
-    _RequiredImportKeyPairRequestServiceResourceImportKeyPairTypeDef,
-    _OptionalImportKeyPairRequestServiceResourceImportKeyPairTypeDef,
-):
-    pass
-
-ImportSnapshotRequestRequestTypeDef = TypedDict(
-    "ImportSnapshotRequestRequestTypeDef",
-    {
-        "ClientData": ClientDataTypeDef,
-        "ClientToken": str,
-        "Description": str,
-        "DiskContainer": SnapshotDiskContainerTypeDef,
-        "DryRun": bool,
-        "Encrypted": bool,
-        "KmsKeyId": str,
-        "RoleName": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-_RequiredProvisionByoipCidrRequestRequestTypeDef = TypedDict(
-    "_RequiredProvisionByoipCidrRequestRequestTypeDef",
-    {
-        "Cidr": str,
-    },
-)
-_OptionalProvisionByoipCidrRequestRequestTypeDef = TypedDict(
-    "_OptionalProvisionByoipCidrRequestRequestTypeDef",
-    {
-        "CidrAuthorizationContext": CidrAuthorizationContextTypeDef,
-        "PubliclyAdvertisable": bool,
-        "Description": str,
-        "DryRun": bool,
-        "PoolTagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "MultiRegion": bool,
-    },
-    total=False,
-)
-
-class ProvisionByoipCidrRequestRequestTypeDef(
-    _RequiredProvisionByoipCidrRequestRequestTypeDef,
-    _OptionalProvisionByoipCidrRequestRequestTypeDef,
-):
-    pass
-
-_RequiredPurchaseHostReservationRequestRequestTypeDef = TypedDict(
-    "_RequiredPurchaseHostReservationRequestRequestTypeDef",
-    {
-        "HostIdSet": Sequence[str],
-        "OfferingId": str,
-    },
-)
-_OptionalPurchaseHostReservationRequestRequestTypeDef = TypedDict(
-    "_OptionalPurchaseHostReservationRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-        "CurrencyCode": Literal["USD"],
-        "LimitPrice": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class PurchaseHostReservationRequestRequestTypeDef(
-    _RequiredPurchaseHostReservationRequestRequestTypeDef,
-    _OptionalPurchaseHostReservationRequestRequestTypeDef,
-):
-    pass
-
-_RequiredStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef = TypedDict(
-    "_RequiredStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
-    {
-        "NetworkInsightsAccessScopeId": str,
-        "ClientToken": str,
-    },
-)
-_OptionalStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef = TypedDict(
-    "_OptionalStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class StartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef(
-    _RequiredStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef,
-    _OptionalStartNetworkInsightsAccessScopeAnalysisRequestRequestTypeDef,
-):
-    pass
-
-_RequiredStartNetworkInsightsAnalysisRequestRequestTypeDef = TypedDict(
-    "_RequiredStartNetworkInsightsAnalysisRequestRequestTypeDef",
-    {
-        "NetworkInsightsPathId": str,
-        "ClientToken": str,
-    },
-)
-_OptionalStartNetworkInsightsAnalysisRequestRequestTypeDef = TypedDict(
-    "_OptionalStartNetworkInsightsAnalysisRequestRequestTypeDef",
-    {
-        "AdditionalAccounts": Sequence[str],
-        "FilterInArns": Sequence[str],
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-    },
-    total=False,
-)
-
-class StartNetworkInsightsAnalysisRequestRequestTypeDef(
-    _RequiredStartNetworkInsightsAnalysisRequestRequestTypeDef,
-    _OptionalStartNetworkInsightsAnalysisRequestRequestTypeDef,
-):
-    pass
-
 PathComponentTypeDef = TypedDict(
     "PathComponentTypeDef",
     {
         "SequenceNumber": int,
         "AclRule": AnalysisAclRuleTypeDef,
         "AttachedTo": AnalysisComponentTypeDef,
         "Component": AnalysisComponentTypeDef,
@@ -30027,14 +30029,129 @@
         "PrivateDnsNameOptions": LaunchTemplatePrivateDnsNameOptionsRequestTypeDef,
         "MaintenanceOptions": LaunchTemplateInstanceMaintenanceOptionsRequestTypeDef,
         "DisableApiStop": bool,
     },
     total=False,
 )
 
+_RequiredRunInstancesRequestRequestTypeDef = TypedDict(
+    "_RequiredRunInstancesRequestRequestTypeDef",
+    {
+        "MaxCount": int,
+        "MinCount": int,
+    },
+)
+_OptionalRunInstancesRequestRequestTypeDef = TypedDict(
+    "_OptionalRunInstancesRequestRequestTypeDef",
+    {
+        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "ImageId": str,
+        "InstanceType": InstanceTypeType,
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
+        "KernelId": str,
+        "KeyName": str,
+        "Monitoring": RunInstancesMonitoringEnabledTypeDef,
+        "Placement": PlacementTypeDef,
+        "RamdiskId": str,
+        "SecurityGroupIds": Sequence[str],
+        "SecurityGroups": Sequence[str],
+        "SubnetId": str,
+        "UserData": str,
+        "AdditionalInfo": str,
+        "ClientToken": str,
+        "DisableApiTermination": bool,
+        "DryRun": bool,
+        "EbsOptimized": bool,
+        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
+        "InstanceInitiatedShutdownBehavior": ShutdownBehaviorType,
+        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationTypeDef],
+        "PrivateIpAddress": str,
+        "ElasticGpuSpecification": Sequence[ElasticGpuSpecificationTypeDef],
+        "ElasticInferenceAccelerators": Sequence[ElasticInferenceAcceleratorTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
+        "InstanceMarketOptions": InstanceMarketOptionsRequestTypeDef,
+        "CreditSpecification": CreditSpecificationRequestTypeDef,
+        "CpuOptions": CpuOptionsRequestTypeDef,
+        "CapacityReservationSpecification": CapacityReservationSpecificationTypeDef,
+        "HibernationOptions": HibernationOptionsRequestTypeDef,
+        "LicenseSpecifications": Sequence[LicenseConfigurationRequestTypeDef],
+        "MetadataOptions": InstanceMetadataOptionsRequestTypeDef,
+        "EnclaveOptions": EnclaveOptionsRequestTypeDef,
+        "PrivateDnsNameOptions": PrivateDnsNameOptionsRequestTypeDef,
+        "MaintenanceOptions": InstanceMaintenanceOptionsRequestTypeDef,
+        "DisableApiStop": bool,
+    },
+    total=False,
+)
+
+class RunInstancesRequestRequestTypeDef(
+    _RequiredRunInstancesRequestRequestTypeDef, _OptionalRunInstancesRequestRequestTypeDef
+):
+    pass
+
+_RequiredRunInstancesRequestServiceResourceCreateInstancesTypeDef = TypedDict(
+    "_RequiredRunInstancesRequestServiceResourceCreateInstancesTypeDef",
+    {
+        "MaxCount": int,
+        "MinCount": int,
+    },
+)
+_OptionalRunInstancesRequestServiceResourceCreateInstancesTypeDef = TypedDict(
+    "_OptionalRunInstancesRequestServiceResourceCreateInstancesTypeDef",
+    {
+        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
+        "ImageId": str,
+        "InstanceType": InstanceTypeType,
+        "Ipv6AddressCount": int,
+        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
+        "KernelId": str,
+        "KeyName": str,
+        "Monitoring": RunInstancesMonitoringEnabledTypeDef,
+        "Placement": PlacementTypeDef,
+        "RamdiskId": str,
+        "SecurityGroupIds": Sequence[str],
+        "SecurityGroups": Sequence[str],
+        "SubnetId": str,
+        "UserData": str,
+        "AdditionalInfo": str,
+        "ClientToken": str,
+        "DisableApiTermination": bool,
+        "DryRun": bool,
+        "EbsOptimized": bool,
+        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
+        "InstanceInitiatedShutdownBehavior": ShutdownBehaviorType,
+        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationServiceResourceTypeDef],
+        "PrivateIpAddress": str,
+        "ElasticGpuSpecification": Sequence[ElasticGpuSpecificationTypeDef],
+        "ElasticInferenceAccelerators": Sequence[ElasticInferenceAcceleratorTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
+        "InstanceMarketOptions": InstanceMarketOptionsRequestTypeDef,
+        "CreditSpecification": CreditSpecificationRequestTypeDef,
+        "CpuOptions": CpuOptionsRequestTypeDef,
+        "CapacityReservationSpecification": CapacityReservationSpecificationTypeDef,
+        "HibernationOptions": HibernationOptionsRequestTypeDef,
+        "LicenseSpecifications": Sequence[LicenseConfigurationRequestTypeDef],
+        "MetadataOptions": InstanceMetadataOptionsRequestTypeDef,
+        "EnclaveOptions": EnclaveOptionsRequestTypeDef,
+        "PrivateDnsNameOptions": PrivateDnsNameOptionsRequestTypeDef,
+        "MaintenanceOptions": InstanceMaintenanceOptionsRequestTypeDef,
+        "DisableApiStop": bool,
+    },
+    total=False,
+)
+
+class RunInstancesRequestServiceResourceCreateInstancesTypeDef(
+    _RequiredRunInstancesRequestServiceResourceCreateInstancesTypeDef,
+    _OptionalRunInstancesRequestServiceResourceCreateInstancesTypeDef,
+):
+    pass
+
 _RequiredRunInstancesRequestSubnetCreateInstancesTypeDef = TypedDict(
     "_RequiredRunInstancesRequestSubnetCreateInstancesTypeDef",
     {
         "MaxCount": int,
         "MinCount": int,
     },
 )
@@ -30057,15 +30174,15 @@
         "AdditionalInfo": str,
         "ClientToken": str,
         "DisableApiTermination": bool,
         "DryRun": bool,
         "EbsOptimized": bool,
         "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
         "InstanceInitiatedShutdownBehavior": ShutdownBehaviorType,
-        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationTypeDef],
+        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationSubnetTypeDef],
         "PrivateIpAddress": str,
         "ElasticGpuSpecification": Sequence[ElasticGpuSpecificationTypeDef],
         "ElasticInferenceAccelerators": Sequence[ElasticInferenceAcceleratorTypeDef],
         "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
         "InstanceMarketOptions": InstanceMarketOptionsRequestTypeDef,
         "CreditSpecification": CreditSpecificationRequestTypeDef,
@@ -30175,15 +30292,29 @@
 )
 
 class BundleInstanceRequestRequestTypeDef(
     _RequiredBundleInstanceRequestRequestTypeDef, _OptionalBundleInstanceRequestRequestTypeDef
 ):
     pass
 
-StorageUnionTypeDef = Union[StorageTypeDef, StorageOutputTypeDef]
+BundleTaskTypeDef = TypedDict(
+    "BundleTaskTypeDef",
+    {
+        "BundleId": str,
+        "BundleTaskError": BundleTaskErrorTypeDef,
+        "InstanceId": str,
+        "Progress": str,
+        "StartTime": datetime,
+        "State": BundleTaskStateType,
+        "Storage": StorageTypeDef,
+        "UpdateTime": datetime,
+    },
+    total=False,
+)
+
 DescribeImagesResultTypeDef = TypedDict(
     "DescribeImagesResultTypeDef",
     {
         "Images": List[ImageTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -30294,144 +30425,29 @@
         "ValidFrom": datetime,
         "ValidUntil": datetime,
         "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
     },
     total=False,
 )
 
-_RequiredRunInstancesRequestRequestTypeDef = TypedDict(
-    "_RequiredRunInstancesRequestRequestTypeDef",
-    {
-        "MaxCount": int,
-        "MinCount": int,
-    },
-)
-_OptionalRunInstancesRequestRequestTypeDef = TypedDict(
-    "_OptionalRunInstancesRequestRequestTypeDef",
-    {
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
-        "ImageId": str,
-        "InstanceType": InstanceTypeType,
-        "Ipv6AddressCount": int,
-        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
-        "KernelId": str,
-        "KeyName": str,
-        "Monitoring": RunInstancesMonitoringEnabledTypeDef,
-        "Placement": PlacementTypeDef,
-        "RamdiskId": str,
-        "SecurityGroupIds": Sequence[str],
-        "SecurityGroups": Sequence[str],
-        "SubnetId": str,
-        "UserData": str,
-        "AdditionalInfo": str,
-        "ClientToken": str,
-        "DisableApiTermination": bool,
-        "DryRun": bool,
-        "EbsOptimized": bool,
-        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
-        "InstanceInitiatedShutdownBehavior": ShutdownBehaviorType,
-        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef],
-        "PrivateIpAddress": str,
-        "ElasticGpuSpecification": Sequence[ElasticGpuSpecificationTypeDef],
-        "ElasticInferenceAccelerators": Sequence[ElasticInferenceAcceleratorTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "InstanceMarketOptions": InstanceMarketOptionsRequestTypeDef,
-        "CreditSpecification": CreditSpecificationRequestTypeDef,
-        "CpuOptions": CpuOptionsRequestTypeDef,
-        "CapacityReservationSpecification": CapacityReservationSpecificationTypeDef,
-        "HibernationOptions": HibernationOptionsRequestTypeDef,
-        "LicenseSpecifications": Sequence[LicenseConfigurationRequestTypeDef],
-        "MetadataOptions": InstanceMetadataOptionsRequestTypeDef,
-        "EnclaveOptions": EnclaveOptionsRequestTypeDef,
-        "PrivateDnsNameOptions": PrivateDnsNameOptionsRequestTypeDef,
-        "MaintenanceOptions": InstanceMaintenanceOptionsRequestTypeDef,
-        "DisableApiStop": bool,
-    },
-    total=False,
-)
-
-class RunInstancesRequestRequestTypeDef(
-    _RequiredRunInstancesRequestRequestTypeDef, _OptionalRunInstancesRequestRequestTypeDef
-):
-    pass
-
-_RequiredRunInstancesRequestServiceResourceCreateInstancesTypeDef = TypedDict(
-    "_RequiredRunInstancesRequestServiceResourceCreateInstancesTypeDef",
-    {
-        "MaxCount": int,
-        "MinCount": int,
-    },
-)
-_OptionalRunInstancesRequestServiceResourceCreateInstancesTypeDef = TypedDict(
-    "_OptionalRunInstancesRequestServiceResourceCreateInstancesTypeDef",
-    {
-        "BlockDeviceMappings": Sequence[BlockDeviceMappingTypeDef],
-        "ImageId": str,
-        "InstanceType": InstanceTypeType,
-        "Ipv6AddressCount": int,
-        "Ipv6Addresses": Sequence[InstanceIpv6AddressTypeDef],
-        "KernelId": str,
-        "KeyName": str,
-        "Monitoring": RunInstancesMonitoringEnabledTypeDef,
-        "Placement": PlacementTypeDef,
-        "RamdiskId": str,
-        "SecurityGroupIds": Sequence[str],
-        "SecurityGroups": Sequence[str],
-        "SubnetId": str,
-        "UserData": str,
-        "AdditionalInfo": str,
-        "ClientToken": str,
-        "DisableApiTermination": bool,
-        "DryRun": bool,
-        "EbsOptimized": bool,
-        "IamInstanceProfile": IamInstanceProfileSpecificationTypeDef,
-        "InstanceInitiatedShutdownBehavior": ShutdownBehaviorType,
-        "NetworkInterfaces": Sequence[InstanceNetworkInterfaceSpecificationUnionTypeDef],
-        "PrivateIpAddress": str,
-        "ElasticGpuSpecification": Sequence[ElasticGpuSpecificationTypeDef],
-        "ElasticInferenceAccelerators": Sequence[ElasticInferenceAcceleratorTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "LaunchTemplate": LaunchTemplateSpecificationTypeDef,
-        "InstanceMarketOptions": InstanceMarketOptionsRequestTypeDef,
-        "CreditSpecification": CreditSpecificationRequestTypeDef,
-        "CpuOptions": CpuOptionsRequestTypeDef,
-        "CapacityReservationSpecification": CapacityReservationSpecificationTypeDef,
-        "HibernationOptions": HibernationOptionsRequestTypeDef,
-        "LicenseSpecifications": Sequence[LicenseConfigurationRequestTypeDef],
-        "MetadataOptions": InstanceMetadataOptionsRequestTypeDef,
-        "EnclaveOptions": EnclaveOptionsRequestTypeDef,
-        "PrivateDnsNameOptions": PrivateDnsNameOptionsRequestTypeDef,
-        "MaintenanceOptions": InstanceMaintenanceOptionsRequestTypeDef,
-        "DisableApiStop": bool,
-    },
-    total=False,
-)
-
-class RunInstancesRequestServiceResourceCreateInstancesTypeDef(
-    _RequiredRunInstancesRequestServiceResourceCreateInstancesTypeDef,
-    _OptionalRunInstancesRequestServiceResourceCreateInstancesTypeDef,
-):
-    pass
-
 RequestSpotInstancesRequestRequestTypeDef = TypedDict(
     "RequestSpotInstancesRequestRequestTypeDef",
     {
         "AvailabilityZoneGroup": str,
         "BlockDurationMinutes": int,
         "ClientToken": str,
         "DryRun": bool,
         "InstanceCount": int,
         "LaunchGroup": str,
         "LaunchSpecification": RequestSpotLaunchSpecificationTypeDef,
         "SpotPrice": str,
         "Type": SpotInstanceTypeType,
         "ValidFrom": TimestampTypeDef,
         "ValidUntil": TimestampTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
     },
     total=False,
 )
 
 DisableFastSnapshotRestoresResultTypeDef = TypedDict(
     "DisableFastSnapshotRestoresResultTypeDef",
@@ -30575,50 +30591,14 @@
         "TpmSupport": str,
         "MaintenanceOptions": InstanceMaintenanceOptionsTypeDef,
         "CurrentInstanceBootMode": InstanceBootModeValuesType,
     },
     total=False,
 )
 
-FleetLaunchTemplateConfigTypeDef = TypedDict(
-    "FleetLaunchTemplateConfigTypeDef",
-    {
-        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
-        "Overrides": List[FleetLaunchTemplateOverridesTypeDef],
-    },
-    total=False,
-)
-
-LaunchTemplateAndOverridesResponseTypeDef = TypedDict(
-    "LaunchTemplateAndOverridesResponseTypeDef",
-    {
-        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
-        "Overrides": FleetLaunchTemplateOverridesTypeDef,
-    },
-    total=False,
-)
-
-LaunchTemplateConfigOutputTypeDef = TypedDict(
-    "LaunchTemplateConfigOutputTypeDef",
-    {
-        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
-        "Overrides": List[LaunchTemplateOverridesOutputTypeDef],
-    },
-    total=False,
-)
-
-LaunchTemplateConfigTypeDef = TypedDict(
-    "LaunchTemplateConfigTypeDef",
-    {
-        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
-        "Overrides": Sequence[LaunchTemplateOverridesTypeDef],
-    },
-    total=False,
-)
-
 FleetLaunchTemplateConfigRequestTypeDef = TypedDict(
     "FleetLaunchTemplateConfigRequestTypeDef",
     {
         "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationRequestTypeDef,
         "Overrides": Sequence[FleetLaunchTemplateOverridesRequestTypeDef],
     },
     total=False,
@@ -30673,146 +30653,66 @@
 
 class GetSpotPlacementScoresRequestRequestTypeDef(
     _RequiredGetSpotPlacementScoresRequestRequestTypeDef,
     _OptionalGetSpotPlacementScoresRequestRequestTypeDef,
 ):
     pass
 
-DescribeInstanceStatusResultTypeDef = TypedDict(
-    "DescribeInstanceStatusResultTypeDef",
-    {
-        "InstanceStatuses": List[InstanceStatusTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeSecurityGroupsResultTypeDef = TypedDict(
-    "DescribeSecurityGroupsResultTypeDef",
-    {
-        "SecurityGroups": List[SecurityGroupTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
-    "_RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef",
-    {
-        "GroupId": str,
-    },
-)
-_OptionalAuthorizeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
-    "_OptionalAuthorizeSecurityGroupEgressRequestRequestTypeDef",
+FleetLaunchTemplateConfigTypeDef = TypedDict(
+    "FleetLaunchTemplateConfigTypeDef",
     {
-        "DryRun": bool,
-        "IpPermissions": Sequence[IpPermissionUnionTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "CidrIp": str,
-        "FromPort": int,
-        "IpProtocol": str,
-        "ToPort": int,
-        "SourceSecurityGroupName": str,
-        "SourceSecurityGroupOwnerId": str,
+        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
+        "Overrides": List[FleetLaunchTemplateOverridesTypeDef],
     },
     total=False,
 )
 
-class AuthorizeSecurityGroupEgressRequestRequestTypeDef(
-    _RequiredAuthorizeSecurityGroupEgressRequestRequestTypeDef,
-    _OptionalAuthorizeSecurityGroupEgressRequestRequestTypeDef,
-):
-    pass
-
-AuthorizeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
-    "AuthorizeSecurityGroupIngressRequestRequestTypeDef",
+LaunchTemplateAndOverridesResponseTypeDef = TypedDict(
+    "LaunchTemplateAndOverridesResponseTypeDef",
     {
-        "CidrIp": str,
-        "FromPort": int,
-        "GroupId": str,
-        "GroupName": str,
-        "IpPermissions": Sequence[IpPermissionUnionTypeDef],
-        "IpProtocol": str,
-        "SourceSecurityGroupName": str,
-        "SourceSecurityGroupOwnerId": str,
-        "ToPort": int,
-        "DryRun": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
+        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
+        "Overrides": FleetLaunchTemplateOverridesTypeDef,
     },
     total=False,
 )
 
-_RequiredRevokeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
-    "_RequiredRevokeSecurityGroupEgressRequestRequestTypeDef",
-    {
-        "GroupId": str,
-    },
-)
-_OptionalRevokeSecurityGroupEgressRequestRequestTypeDef = TypedDict(
-    "_OptionalRevokeSecurityGroupEgressRequestRequestTypeDef",
+LaunchTemplateConfigTypeDef = TypedDict(
+    "LaunchTemplateConfigTypeDef",
     {
-        "DryRun": bool,
-        "IpPermissions": Sequence[IpPermissionUnionTypeDef],
-        "SecurityGroupRuleIds": Sequence[str],
-        "CidrIp": str,
-        "FromPort": int,
-        "IpProtocol": str,
-        "ToPort": int,
-        "SourceSecurityGroupName": str,
-        "SourceSecurityGroupOwnerId": str,
+        "LaunchTemplateSpecification": FleetLaunchTemplateSpecificationTypeDef,
+        "Overrides": List[LaunchTemplateOverridesTypeDef],
     },
     total=False,
 )
 
-class RevokeSecurityGroupEgressRequestRequestTypeDef(
-    _RequiredRevokeSecurityGroupEgressRequestRequestTypeDef,
-    _OptionalRevokeSecurityGroupEgressRequestRequestTypeDef,
-):
-    pass
-
-RevokeSecurityGroupIngressRequestRequestTypeDef = TypedDict(
-    "RevokeSecurityGroupIngressRequestRequestTypeDef",
+DescribeInstanceStatusResultTypeDef = TypedDict(
+    "DescribeInstanceStatusResultTypeDef",
     {
-        "CidrIp": str,
-        "FromPort": int,
-        "GroupId": str,
-        "GroupName": str,
-        "IpPermissions": Sequence[IpPermissionUnionTypeDef],
-        "IpProtocol": str,
-        "SourceSecurityGroupName": str,
-        "SourceSecurityGroupOwnerId": str,
-        "ToPort": int,
-        "DryRun": bool,
-        "SecurityGroupRuleIds": Sequence[str],
+        "InstanceStatuses": List[InstanceStatusTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef = TypedDict(
-    "UpdateSecurityGroupRuleDescriptionsEgressRequestRequestTypeDef",
+DescribeSecurityGroupsResultTypeDef = TypedDict(
+    "DescribeSecurityGroupsResultTypeDef",
     {
-        "DryRun": bool,
-        "GroupId": str,
-        "GroupName": str,
-        "IpPermissions": Sequence[IpPermissionUnionTypeDef],
-        "SecurityGroupRuleDescriptions": Sequence[SecurityGroupRuleDescriptionTypeDef],
+        "SecurityGroups": List[SecurityGroupTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef = TypedDict(
-    "UpdateSecurityGroupRuleDescriptionsIngressRequestRequestTypeDef",
+DescribeSecurityGroupsResultVpcAddressTypeDef = TypedDict(
+    "DescribeSecurityGroupsResultVpcAddressTypeDef",
     {
-        "DryRun": bool,
-        "GroupId": str,
-        "GroupName": str,
-        "IpPermissions": Sequence[IpPermissionUnionTypeDef],
-        "SecurityGroupRuleDescriptions": Sequence[SecurityGroupRuleDescriptionTypeDef],
+        "SecurityGroups": List[SecurityGroupVpcAddressTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 DescribeStaleSecurityGroupsResultTypeDef = TypedDict(
     "DescribeStaleSecurityGroupsResultTypeDef",
     {
         "NextToken": str,
         "StaleSecurityGroupSet": List[StaleSecurityGroupTypeDef],
@@ -30859,15 +30759,15 @@
     },
 )
 _OptionalCreateNetworkInsightsAccessScopeRequestRequestTypeDef = TypedDict(
     "_OptionalCreateNetworkInsightsAccessScopeRequestRequestTypeDef",
     {
         "MatchPaths": Sequence[AccessScopePathRequestTypeDef],
         "ExcludePaths": Sequence[AccessScopePathRequestTypeDef],
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
         "DryRun": bool,
     },
     total=False,
 )
 
 class CreateNetworkInsightsAccessScopeRequestRequestTypeDef(
     _RequiredCreateNetworkInsightsAccessScopeRequestRequestTypeDef,
@@ -30881,38 +30781,14 @@
         "NetworkInsightsAccessScopeId": str,
         "MatchPaths": List[AccessScopePathTypeDef],
         "ExcludePaths": List[AccessScopePathTypeDef],
     },
     total=False,
 )
 
-BundleInstanceResultTypeDef = TypedDict(
-    "BundleInstanceResultTypeDef",
-    {
-        "BundleTask": BundleTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-CancelBundleTaskResultTypeDef = TypedDict(
-    "CancelBundleTaskResultTypeDef",
-    {
-        "BundleTask": BundleTaskTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-DescribeBundleTasksResultTypeDef = TypedDict(
-    "DescribeBundleTasksResultTypeDef",
-    {
-        "BundleTasks": List[BundleTaskTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredRunScheduledInstancesRequestRequestTypeDef = TypedDict(
     "_RequiredRunScheduledInstancesRequestRequestTypeDef",
     {
         "LaunchSpecification": ScheduledInstancesLaunchSpecificationTypeDef,
         "ScheduledInstanceId": str,
     },
 )
@@ -31145,15 +31021,15 @@
 )
 _OptionalCreateLaunchTemplateRequestRequestTypeDef = TypedDict(
     "_OptionalCreateLaunchTemplateRequestRequestTypeDef",
     {
         "DryRun": bool,
         "ClientToken": str,
         "VersionDescription": str,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
     total=False,
 )
 
 class CreateLaunchTemplateRequestRequestTypeDef(
     _RequiredCreateLaunchTemplateRequestRequestTypeDef,
     _OptionalCreateLaunchTemplateRequestRequestTypeDef,
@@ -31200,29 +31076,53 @@
     {
         "NetworkInterfaces": List[NetworkInterfaceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BundleInstanceResultTypeDef = TypedDict(
+    "BundleInstanceResultTypeDef",
+    {
+        "BundleTask": BundleTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelBundleTaskResultTypeDef = TypedDict(
+    "CancelBundleTaskResultTypeDef",
+    {
+        "BundleTask": BundleTaskTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBundleTasksResultTypeDef = TypedDict(
+    "DescribeBundleTasksResultTypeDef",
+    {
+        "BundleTasks": List[BundleTaskTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateVpnConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpnConnectionRequestRequestTypeDef",
     {
         "CustomerGatewayId": str,
         "Type": str,
     },
 )
 _OptionalCreateVpnConnectionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateVpnConnectionRequestRequestTypeDef",
     {
         "VpnGatewayId": str,
         "TransitGatewayId": str,
         "DryRun": bool,
         "Options": VpnConnectionOptionsSpecificationTypeDef,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
     },
     total=False,
 )
 
 class CreateVpnConnectionRequestRequestTypeDef(
     _RequiredCreateVpnConnectionRequestRequestTypeDef,
     _OptionalCreateVpnConnectionRequestRequestTypeDef,
@@ -31321,14 +31221,68 @@
         "OwnerId": str,
         "RequesterId": str,
         "ReservationId": str,
     },
     total=False,
 )
 
+_RequiredCreateFleetRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateFleetRequestRequestTypeDef",
+    {
+        "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
+        "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
+    },
+)
+_OptionalCreateFleetRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateFleetRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "ClientToken": str,
+        "SpotOptions": SpotOptionsRequestTypeDef,
+        "OnDemandOptions": OnDemandOptionsRequestTypeDef,
+        "ExcessCapacityTerminationPolicy": FleetExcessCapacityTerminationPolicyType,
+        "TerminateInstancesWithExpiration": bool,
+        "Type": FleetTypeType,
+        "ValidFrom": TimestampTypeDef,
+        "ValidUntil": TimestampTypeDef,
+        "ReplaceUnhealthyInstances": bool,
+        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "Context": str,
+    },
+    total=False,
+)
+
+class CreateFleetRequestRequestTypeDef(
+    _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
+):
+    pass
+
+_RequiredModifyFleetRequestRequestTypeDef = TypedDict(
+    "_RequiredModifyFleetRequestRequestTypeDef",
+    {
+        "FleetId": str,
+    },
+)
+_OptionalModifyFleetRequestRequestTypeDef = TypedDict(
+    "_OptionalModifyFleetRequestRequestTypeDef",
+    {
+        "DryRun": bool,
+        "ExcessCapacityTerminationPolicy": FleetExcessCapacityTerminationPolicyType,
+        "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
+        "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
+        "Context": str,
+    },
+    total=False,
+)
+
+class ModifyFleetRequestRequestTypeDef(
+    _RequiredModifyFleetRequestRequestTypeDef, _OptionalModifyFleetRequestRequestTypeDef
+):
+    pass
+
 CreateFleetErrorTypeDef = TypedDict(
     "CreateFleetErrorTypeDef",
     {
         "LaunchTemplateAndOverrides": LaunchTemplateAndOverridesResponseTypeDef,
         "Lifecycle": InstanceLifecycleType,
         "ErrorCode": str,
         "ErrorMessage": str,
@@ -31367,61 +31321,38 @@
         "InstanceIds": List[str],
         "InstanceType": InstanceTypeType,
         "Platform": Literal["Windows"],
     },
     total=False,
 )
 
-_RequiredSpotFleetRequestConfigDataOutputTypeDef = TypedDict(
-    "_RequiredSpotFleetRequestConfigDataOutputTypeDef",
+_RequiredModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
+    "_RequiredModifySpotFleetRequestRequestRequestTypeDef",
     {
-        "IamFleetRole": str,
-        "TargetCapacity": int,
+        "SpotFleetRequestId": str,
     },
 )
-_OptionalSpotFleetRequestConfigDataOutputTypeDef = TypedDict(
-    "_OptionalSpotFleetRequestConfigDataOutputTypeDef",
+_OptionalModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
+    "_OptionalModifySpotFleetRequestRequestRequestTypeDef",
     {
-        "AllocationStrategy": AllocationStrategyType,
-        "OnDemandAllocationStrategy": OnDemandAllocationStrategyType,
-        "SpotMaintenanceStrategies": SpotMaintenanceStrategiesTypeDef,
-        "ClientToken": str,
         "ExcessCapacityTerminationPolicy": ExcessCapacityTerminationPolicyType,
-        "FulfilledCapacity": float,
-        "OnDemandFulfilledCapacity": float,
-        "LaunchSpecifications": List[SpotFleetLaunchSpecificationOutputTypeDef],
-        "LaunchTemplateConfigs": List[LaunchTemplateConfigOutputTypeDef],
-        "SpotPrice": str,
+        "LaunchTemplateConfigs": Sequence[LaunchTemplateConfigTypeDef],
+        "TargetCapacity": int,
         "OnDemandTargetCapacity": int,
-        "OnDemandMaxTotalPrice": str,
-        "SpotMaxTotalPrice": str,
-        "TerminateInstancesWithExpiration": bool,
-        "Type": FleetTypeType,
-        "ValidFrom": datetime,
-        "ValidUntil": datetime,
-        "ReplaceUnhealthyInstances": bool,
-        "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
-        "LoadBalancersConfig": LoadBalancersConfigOutputTypeDef,
-        "InstancePoolsToUseCount": int,
         "Context": str,
-        "TargetCapacityUnitType": TargetCapacityUnitTypeType,
-        "TagSpecifications": List[TagSpecificationOutputTypeDef],
     },
     total=False,
 )
 
-class SpotFleetRequestConfigDataOutputTypeDef(
-    _RequiredSpotFleetRequestConfigDataOutputTypeDef,
-    _OptionalSpotFleetRequestConfigDataOutputTypeDef,
+class ModifySpotFleetRequestRequestRequestTypeDef(
+    _RequiredModifySpotFleetRequestRequestRequestTypeDef,
+    _OptionalModifySpotFleetRequestRequestRequestTypeDef,
 ):
     pass
 
-LaunchTemplateConfigUnionTypeDef = Union[
-    LaunchTemplateConfigTypeDef, LaunchTemplateConfigOutputTypeDef
-]
 _RequiredSpotFleetRequestConfigDataTypeDef = TypedDict(
     "_RequiredSpotFleetRequestConfigDataTypeDef",
     {
         "IamFleetRole": str,
         "TargetCapacity": int,
     },
 )
@@ -31431,91 +31362,81 @@
         "AllocationStrategy": AllocationStrategyType,
         "OnDemandAllocationStrategy": OnDemandAllocationStrategyType,
         "SpotMaintenanceStrategies": SpotMaintenanceStrategiesTypeDef,
         "ClientToken": str,
         "ExcessCapacityTerminationPolicy": ExcessCapacityTerminationPolicyType,
         "FulfilledCapacity": float,
         "OnDemandFulfilledCapacity": float,
-        "LaunchSpecifications": Sequence[SpotFleetLaunchSpecificationTypeDef],
-        "LaunchTemplateConfigs": Sequence[LaunchTemplateConfigTypeDef],
+        "LaunchSpecifications": List[SpotFleetLaunchSpecificationTypeDef],
+        "LaunchTemplateConfigs": List[LaunchTemplateConfigTypeDef],
         "SpotPrice": str,
         "OnDemandTargetCapacity": int,
         "OnDemandMaxTotalPrice": str,
         "SpotMaxTotalPrice": str,
         "TerminateInstancesWithExpiration": bool,
         "Type": FleetTypeType,
-        "ValidFrom": TimestampTypeDef,
-        "ValidUntil": TimestampTypeDef,
+        "ValidFrom": datetime,
+        "ValidUntil": datetime,
         "ReplaceUnhealthyInstances": bool,
         "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
         "LoadBalancersConfig": LoadBalancersConfigTypeDef,
         "InstancePoolsToUseCount": int,
         "Context": str,
         "TargetCapacityUnitType": TargetCapacityUnitTypeType,
-        "TagSpecifications": Sequence[TagSpecificationTypeDef],
+        "TagSpecifications": List[TagSpecificationTypeDef],
     },
     total=False,
 )
 
 class SpotFleetRequestConfigDataTypeDef(
     _RequiredSpotFleetRequestConfigDataTypeDef, _OptionalSpotFleetRequestConfigDataTypeDef
 ):
     pass
 
-_RequiredCreateFleetRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateFleetRequestRequestTypeDef",
+_RequiredSpotFleetRequestConfigDataVpcAddressTypeDef = TypedDict(
+    "_RequiredSpotFleetRequestConfigDataVpcAddressTypeDef",
     {
-        "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
-        "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
+        "IamFleetRole": str,
+        "TargetCapacity": int,
     },
 )
-_OptionalCreateFleetRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateFleetRequestRequestTypeDef",
+_OptionalSpotFleetRequestConfigDataVpcAddressTypeDef = TypedDict(
+    "_OptionalSpotFleetRequestConfigDataVpcAddressTypeDef",
     {
-        "DryRun": bool,
+        "AllocationStrategy": AllocationStrategyType,
+        "OnDemandAllocationStrategy": OnDemandAllocationStrategyType,
+        "SpotMaintenanceStrategies": SpotMaintenanceStrategiesTypeDef,
         "ClientToken": str,
-        "SpotOptions": SpotOptionsRequestTypeDef,
-        "OnDemandOptions": OnDemandOptionsRequestTypeDef,
-        "ExcessCapacityTerminationPolicy": FleetExcessCapacityTerminationPolicyType,
+        "ExcessCapacityTerminationPolicy": ExcessCapacityTerminationPolicyType,
+        "FulfilledCapacity": float,
+        "OnDemandFulfilledCapacity": float,
+        "LaunchSpecifications": List[SpotFleetLaunchSpecificationTypeDef],
+        "LaunchTemplateConfigs": List[LaunchTemplateConfigTypeDef],
+        "SpotPrice": str,
+        "OnDemandTargetCapacity": int,
+        "OnDemandMaxTotalPrice": str,
+        "SpotMaxTotalPrice": str,
         "TerminateInstancesWithExpiration": bool,
         "Type": FleetTypeType,
-        "ValidFrom": TimestampTypeDef,
-        "ValidUntil": TimestampTypeDef,
+        "ValidFrom": datetime,
+        "ValidUntil": datetime,
         "ReplaceUnhealthyInstances": bool,
-        "TagSpecifications": Sequence[TagSpecificationUnionTypeDef],
-        "Context": str,
-    },
-    total=False,
-)
-
-class CreateFleetRequestRequestTypeDef(
-    _RequiredCreateFleetRequestRequestTypeDef, _OptionalCreateFleetRequestRequestTypeDef
-):
-    pass
-
-_RequiredModifyFleetRequestRequestTypeDef = TypedDict(
-    "_RequiredModifyFleetRequestRequestTypeDef",
-    {
-        "FleetId": str,
-    },
-)
-_OptionalModifyFleetRequestRequestTypeDef = TypedDict(
-    "_OptionalModifyFleetRequestRequestTypeDef",
-    {
-        "DryRun": bool,
-        "ExcessCapacityTerminationPolicy": FleetExcessCapacityTerminationPolicyType,
-        "LaunchTemplateConfigs": Sequence[FleetLaunchTemplateConfigRequestTypeDef],
-        "TargetCapacitySpecification": TargetCapacitySpecificationRequestTypeDef,
+        "InstanceInterruptionBehavior": InstanceInterruptionBehaviorType,
+        "LoadBalancersConfig": LoadBalancersConfigTypeDef,
+        "InstancePoolsToUseCount": int,
         "Context": str,
+        "TargetCapacityUnitType": TargetCapacityUnitTypeType,
+        "TagSpecifications": List[TagSpecificationVpcAddressTypeDef],
     },
     total=False,
 )
 
-class ModifyFleetRequestRequestTypeDef(
-    _RequiredModifyFleetRequestRequestTypeDef, _OptionalModifyFleetRequestRequestTypeDef
+class SpotFleetRequestConfigDataVpcAddressTypeDef(
+    _RequiredSpotFleetRequestConfigDataVpcAddressTypeDef,
+    _OptionalSpotFleetRequestConfigDataVpcAddressTypeDef,
 ):
     pass
 
 CreateLaunchTemplateVersionResultTypeDef = TypedDict(
     "CreateLaunchTemplateVersionResultTypeDef",
     {
         "LaunchTemplateVersion": LaunchTemplateVersionTypeDef,
@@ -31686,73 +31607,59 @@
         "Errors": List[DescribeFleetErrorTypeDef],
         "Instances": List[DescribeFleetsInstancesTypeDef],
         "Context": str,
     },
     total=False,
 )
 
-SpotFleetRequestConfigTypeDef = TypedDict(
-    "SpotFleetRequestConfigTypeDef",
-    {
-        "ActivityStatus": ActivityStatusType,
-        "CreateTime": datetime,
-        "SpotFleetRequestConfig": SpotFleetRequestConfigDataOutputTypeDef,
-        "SpotFleetRequestId": str,
-        "SpotFleetRequestState": BatchStateType,
-        "Tags": List[TagTypeDef],
-    },
-    total=False,
-)
-
-_RequiredModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
-    "_RequiredModifySpotFleetRequestRequestRequestTypeDef",
+_RequiredRequestSpotFleetRequestRequestTypeDef = TypedDict(
+    "_RequiredRequestSpotFleetRequestRequestTypeDef",
     {
-        "SpotFleetRequestId": str,
+        "SpotFleetRequestConfig": SpotFleetRequestConfigDataTypeDef,
     },
 )
-_OptionalModifySpotFleetRequestRequestRequestTypeDef = TypedDict(
-    "_OptionalModifySpotFleetRequestRequestRequestTypeDef",
+_OptionalRequestSpotFleetRequestRequestTypeDef = TypedDict(
+    "_OptionalRequestSpotFleetRequestRequestTypeDef",
     {
-        "ExcessCapacityTerminationPolicy": ExcessCapacityTerminationPolicyType,
-        "LaunchTemplateConfigs": Sequence[LaunchTemplateConfigUnionTypeDef],
-        "TargetCapacity": int,
-        "OnDemandTargetCapacity": int,
-        "Context": str,
+        "DryRun": bool,
     },
     total=False,
 )
 
-class ModifySpotFleetRequestRequestRequestTypeDef(
-    _RequiredModifySpotFleetRequestRequestRequestTypeDef,
-    _OptionalModifySpotFleetRequestRequestRequestTypeDef,
+class RequestSpotFleetRequestRequestTypeDef(
+    _RequiredRequestSpotFleetRequestRequestTypeDef, _OptionalRequestSpotFleetRequestRequestTypeDef
 ):
     pass
 
-_RequiredRequestSpotFleetRequestRequestTypeDef = TypedDict(
-    "_RequiredRequestSpotFleetRequestRequestTypeDef",
+SpotFleetRequestConfigTypeDef = TypedDict(
+    "SpotFleetRequestConfigTypeDef",
     {
+        "ActivityStatus": ActivityStatusType,
+        "CreateTime": datetime,
         "SpotFleetRequestConfig": SpotFleetRequestConfigDataTypeDef,
+        "SpotFleetRequestId": str,
+        "SpotFleetRequestState": BatchStateType,
+        "Tags": List[TagTypeDef],
     },
+    total=False,
 )
-_OptionalRequestSpotFleetRequestRequestTypeDef = TypedDict(
-    "_OptionalRequestSpotFleetRequestRequestTypeDef",
+
+SpotFleetRequestConfigVpcAddressTypeDef = TypedDict(
+    "SpotFleetRequestConfigVpcAddressTypeDef",
     {
-        "DryRun": bool,
+        "ActivityStatus": ActivityStatusType,
+        "CreateTime": datetime,
+        "SpotFleetRequestConfig": SpotFleetRequestConfigDataVpcAddressTypeDef,
+        "SpotFleetRequestId": str,
+        "SpotFleetRequestState": BatchStateType,
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
-class RequestSpotFleetRequestRequestTypeDef(
-    _RequiredRequestSpotFleetRequestRequestTypeDef, _OptionalRequestSpotFleetRequestRequestTypeDef
-):
-    pass
-
-SpotFleetRequestConfigDataUnionTypeDef = Union[
-    SpotFleetRequestConfigDataTypeDef, SpotFleetRequestConfigDataOutputTypeDef
-]
 DescribeFleetsResultTypeDef = TypedDict(
     "DescribeFleetsResultTypeDef",
     {
         "NextToken": str,
         "Fleets": List[FleetDataTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -31762,7 +31669,16 @@
     "DescribeSpotFleetRequestsResponseTypeDef",
     {
         "NextToken": str,
         "SpotFleetRequestConfigs": List[SpotFleetRequestConfigTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+DescribeSpotFleetRequestsResponseVpcAddressTypeDef = TypedDict(
+    "DescribeSpotFleetRequestsResponseVpcAddressTypeDef",
+    {
+        "NextToken": str,
+        "SpotFleetRequestConfigs": List[SpotFleetRequestConfigVpcAddressTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/waiter.py` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2/waiter.pyi` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ec2-2.5.2.post1/types_aiobotocore_ec2.egg-info/SOURCES.txt` & `types-aiobotocore-ec2-2.5.2.post2/types_aiobotocore_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

