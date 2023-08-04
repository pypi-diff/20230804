# Comparing `tmp/types-aiobotocore-sso-admin-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sso-admin-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sso-admin-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-sso-admin-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:27 2023, max compression
```

## Comparing `types-aiobotocore-sso-admin-2.5.2.post1.tar` & `types-aiobotocore-sso-admin-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.537447 types-aiobotocore-sso-admin-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:17.000000 types-aiobotocore-sso-admin-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20945 2023-08-02 14:53:04.533447 types-aiobotocore-sso-admin-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19420 2023-08-02 14:50:17.000000 types-aiobotocore-sso-admin-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:04.537447 types-aiobotocore-sso-admin-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-08-02 14:50:17.000000 types-aiobotocore-sso-admin-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.533447 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-08-02 14:50:17.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-08-02 14:50:17.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-02 14:50:17.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36948 2023-08-02 14:50:17.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    36891 2023-08-02 14:50:17.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10873 2023-08-02 14:50:18.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10871 2023-08-02 14:50:18.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-08-02 14:50:18.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15870 2023-08-02 14:50:17.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:17.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    40774 2023-08-02 14:50:18.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    40725 2023-08-02 14:50:18.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:17.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.533447 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20945 2023-08-02 14:53:04.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:53:04.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:04.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:04.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:04.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:53:04.000000 types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.746643 types-aiobotocore-sso-admin-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:54:31.000000 types-aiobotocore-sso-admin-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15318 2023-08-04 13:59:27.746643 types-aiobotocore-sso-admin-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13793 2023-08-04 13:54:31.000000 types-aiobotocore-sso-admin-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:27.746643 types-aiobotocore-sso-admin-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2085 2023-08-04 13:54:31.000000 types-aiobotocore-sso-admin-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.746643 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3748 2023-08-04 13:54:31.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     3747 2023-08-04 13:54:31.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      949 2023-08-04 13:54:31.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    36933 2023-08-04 13:54:31.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    36876 2023-08-04 13:54:31.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10968 2023-08-04 13:54:32.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10966 2023-08-04 13:54:32.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15883 2023-08-04 13:54:31.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15870 2023-08-04 13:54:31.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:54:31.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    39784 2023-08-04 13:54:33.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    39735 2023-08-04 13:54:32.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:54:31.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:27.746643 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    15318 2023-08-04 13:59:27.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      851 2023-08-04 13:59:27.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:27.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:27.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:27.000000 types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/LICENSE` & `types-aiobotocore-sso-admin-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/setup.py` & `types-aiobotocore-sso-admin-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sso-admin",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sso_admin"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SSOAdmin 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/__init__.py` & `types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/__init__.pyi` & `types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/__main__.py` & `types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSOAdmin 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SSOAdmin 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin\nOther"
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

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/client.py` & `types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     DescribeAccountAssignmentCreationStatusResponseTypeDef,
     DescribeAccountAssignmentDeletionStatusResponseTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef,
     DescribePermissionSetProvisioningStatusResponseTypeDef,
     DescribePermissionSetResponseTypeDef,
     GetInlinePolicyForPermissionSetResponseTypeDef,
     GetPermissionsBoundaryForPermissionSetResponseTypeDef,
-    InstanceAccessControlAttributeConfigurationUnionTypeDef,
+    InstanceAccessControlAttributeConfigurationTypeDef,
     ListAccountAssignmentCreationStatusResponseTypeDef,
     ListAccountAssignmentDeletionStatusResponseTypeDef,
     ListAccountAssignmentsResponseTypeDef,
     ListAccountsForProvisionedPermissionSetResponseTypeDef,
     ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
     ListInstancesResponseTypeDef,
     ListManagedPoliciesInPermissionSetResponseTypeDef,
@@ -167,15 +167,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#create_account_assignment)
         """
 
     async def create_instance_access_control_attribute_configuration(
         self,
         *,
         InstanceArn: str,
-        InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationUnionTypeDef
+        InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         Enables the attributes-based access control (ABAC) feature for the specified IAM
         Identity Center instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_instance_access_control_attribute_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#create_instance_access_control_attribute_configuration)
@@ -587,15 +587,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#untag_resource)
         """
 
     async def update_instance_access_control_attribute_configuration(
         self,
         *,
         InstanceArn: str,
-        InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationUnionTypeDef
+        InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the IAM Identity Center identity store attributes that you can use with
         the IAM Identity Center instance for attributes-based access control (ABAC).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.update_instance_access_control_attribute_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#update_instance_access_control_attribute_configuration)
```

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/client.pyi` & `types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     DescribeAccountAssignmentCreationStatusResponseTypeDef,
     DescribeAccountAssignmentDeletionStatusResponseTypeDef,
     DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef,
     DescribePermissionSetProvisioningStatusResponseTypeDef,
     DescribePermissionSetResponseTypeDef,
     GetInlinePolicyForPermissionSetResponseTypeDef,
     GetPermissionsBoundaryForPermissionSetResponseTypeDef,
-    InstanceAccessControlAttributeConfigurationUnionTypeDef,
+    InstanceAccessControlAttributeConfigurationTypeDef,
     ListAccountAssignmentCreationStatusResponseTypeDef,
     ListAccountAssignmentDeletionStatusResponseTypeDef,
     ListAccountAssignmentsResponseTypeDef,
     ListAccountsForProvisionedPermissionSetResponseTypeDef,
     ListCustomerManagedPolicyReferencesInPermissionSetResponseTypeDef,
     ListInstancesResponseTypeDef,
     ListManagedPoliciesInPermissionSetResponseTypeDef,
@@ -157,15 +157,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_account_assignment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#create_account_assignment)
         """
     async def create_instance_access_control_attribute_configuration(
         self,
         *,
         InstanceArn: str,
-        InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationUnionTypeDef
+        InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         Enables the attributes-based access control (ABAC) feature for the specified IAM
         Identity Center instance.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.create_instance_access_control_attribute_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#create_instance_access_control_attribute_configuration)
@@ -544,15 +544,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#untag_resource)
         """
     async def update_instance_access_control_attribute_configuration(
         self,
         *,
         InstanceArn: str,
-        InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationUnionTypeDef
+        InstanceAccessControlAttributeConfiguration: InstanceAccessControlAttributeConfigurationTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the IAM Identity Center identity store attributes that you can use with
         the IAM Identity Center instance for attributes-based access control (ABAC).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-admin.html#SSOAdmin.Client.update_instance_access_control_attribute_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/client/#update_instance_access_control_attribute_configuration)
```

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/literals.py` & `types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
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
@@ -193,14 +194,15 @@
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
@@ -279,26 +281,28 @@
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

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/literals.pyi` & `types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
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
@@ -191,14 +192,15 @@
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
@@ -277,26 +279,28 @@
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

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/paginator.py` & `types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/paginator.pyi` & `types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/type_defs.py` & `types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for sso-admin service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_sso_admin.type_defs import AccessControlAttributeValueOutputTypeDef
+    from types_aiobotocore_sso_admin.type_defs import AccessControlAttributeValueTypeDef
 
-    data: AccessControlAttributeValueOutputTypeDef = ...
+    data: AccessControlAttributeValueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     InstanceAccessControlAttributeConfigurationStatusType,
     PrincipalTypeType,
     ProvisioningStatusType,
     ProvisionTargetTypeType,
     StatusValuesType,
@@ -30,15 +30,14 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "AccessControlAttributeValueOutputTypeDef",
     "AccessControlAttributeValueTypeDef",
     "AccountAssignmentOperationStatusMetadataTypeDef",
     "AccountAssignmentOperationStatusTypeDef",
     "AccountAssignmentTypeDef",
     "CustomerManagedPolicyReferenceTypeDef",
     "AttachManagedPolicyToPermissionSetRequestRequestTypeDef",
     "AttachedManagedPolicyTypeDef",
@@ -72,15 +71,14 @@
     "ListPermissionSetsProvisionedToAccountRequestRequestTypeDef",
     "ListPermissionSetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ProvisionPermissionSetRequestRequestTypeDef",
     "PutInlinePolicyToPermissionSetRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePermissionSetRequestRequestTypeDef",
-    "AccessControlAttributeOutputTypeDef",
     "AccessControlAttributeTypeDef",
     "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
     "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
     "PermissionsBoundaryTypeDef",
     "CreateAccountAssignmentResponseTypeDef",
     "DeleteAccountAssignmentResponseTypeDef",
     "DescribeAccountAssignmentCreationStatusResponseTypeDef",
@@ -113,31 +111,22 @@
     "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
     "ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     "ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
     "ListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListPermissionSetProvisioningStatusResponseTypeDef",
-    "InstanceAccessControlAttributeConfigurationOutputTypeDef",
     "InstanceAccessControlAttributeConfigurationTypeDef",
     "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
-    "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
-    "InstanceAccessControlAttributeConfigurationUnionTypeDef",
+    "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
 )
 
-AccessControlAttributeValueOutputTypeDef = TypedDict(
-    "AccessControlAttributeValueOutputTypeDef",
-    {
-        "Source": List[str],
-    },
-)
-
 AccessControlAttributeValueTypeDef = TypedDict(
     "AccessControlAttributeValueTypeDef",
     {
         "Source": Sequence[str],
     },
 )
 
@@ -659,22 +648,14 @@
 class UpdatePermissionSetRequestRequestTypeDef(
     _RequiredUpdatePermissionSetRequestRequestTypeDef,
     _OptionalUpdatePermissionSetRequestRequestTypeDef,
 ):
     pass
 
 
-AccessControlAttributeOutputTypeDef = TypedDict(
-    "AccessControlAttributeOutputTypeDef",
-    {
-        "Key": str,
-        "Value": AccessControlAttributeValueOutputTypeDef,
-    },
-)
-
 AccessControlAttributeTypeDef = TypedDict(
     "AccessControlAttributeTypeDef",
     {
         "Key": str,
         "Value": AccessControlAttributeValueTypeDef,
     },
 )
@@ -1220,21 +1201,14 @@
     {
         "PermissionSetsProvisioningStatus": List[PermissionSetProvisioningStatusMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InstanceAccessControlAttributeConfigurationOutputTypeDef = TypedDict(
-    "InstanceAccessControlAttributeConfigurationOutputTypeDef",
-    {
-        "AccessControlAttributes": List[AccessControlAttributeOutputTypeDef],
-    },
-)
-
 InstanceAccessControlAttributeConfigurationTypeDef = TypedDict(
     "InstanceAccessControlAttributeConfigurationTypeDef",
     {
         "AccessControlAttributes": Sequence[AccessControlAttributeTypeDef],
     },
 )
 
@@ -1251,40 +1225,36 @@
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
         "PermissionsBoundary": PermissionsBoundaryTypeDef,
     },
 )
 
-DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef = TypedDict(
-    "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
+CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     {
-        "Status": InstanceAccessControlAttributeConfigurationStatusType,
-        "StatusReason": str,
+        "InstanceArn": str,
         "InstanceAccessControlAttributeConfiguration": (
-            InstanceAccessControlAttributeConfigurationOutputTypeDef
+            InstanceAccessControlAttributeConfigurationTypeDef
         ),
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
+DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef = TypedDict(
+    "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     {
-        "InstanceArn": str,
+        "Status": InstanceAccessControlAttributeConfigurationStatusType,
+        "StatusReason": str,
         "InstanceAccessControlAttributeConfiguration": (
             InstanceAccessControlAttributeConfigurationTypeDef
         ),
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InstanceAccessControlAttributeConfigurationUnionTypeDef = Union[
-    InstanceAccessControlAttributeConfigurationTypeDef,
-    InstanceAccessControlAttributeConfigurationOutputTypeDef,
-]
 UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "InstanceAccessControlAttributeConfiguration": (
             InstanceAccessControlAttributeConfigurationTypeDef
         ),
```

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin/type_defs.pyi` & `types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for sso-admin service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_admin/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_sso_admin.type_defs import AccessControlAttributeValueOutputTypeDef
+    from types_aiobotocore_sso_admin.type_defs import AccessControlAttributeValueTypeDef
 
-    data: AccessControlAttributeValueOutputTypeDef = ...
+    data: AccessControlAttributeValueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     InstanceAccessControlAttributeConfigurationStatusType,
     PrincipalTypeType,
     ProvisioningStatusType,
     ProvisionTargetTypeType,
     StatusValuesType,
@@ -29,15 +29,14 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "AccessControlAttributeValueOutputTypeDef",
     "AccessControlAttributeValueTypeDef",
     "AccountAssignmentOperationStatusMetadataTypeDef",
     "AccountAssignmentOperationStatusTypeDef",
     "AccountAssignmentTypeDef",
     "CustomerManagedPolicyReferenceTypeDef",
     "AttachManagedPolicyToPermissionSetRequestRequestTypeDef",
     "AttachedManagedPolicyTypeDef",
@@ -71,15 +70,14 @@
     "ListPermissionSetsProvisionedToAccountRequestRequestTypeDef",
     "ListPermissionSetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ProvisionPermissionSetRequestRequestTypeDef",
     "PutInlinePolicyToPermissionSetRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdatePermissionSetRequestRequestTypeDef",
-    "AccessControlAttributeOutputTypeDef",
     "AccessControlAttributeTypeDef",
     "AttachCustomerManagedPolicyReferenceToPermissionSetRequestRequestTypeDef",
     "DetachCustomerManagedPolicyReferenceFromPermissionSetRequestRequestTypeDef",
     "PermissionsBoundaryTypeDef",
     "CreateAccountAssignmentResponseTypeDef",
     "DeleteAccountAssignmentResponseTypeDef",
     "DescribeAccountAssignmentCreationStatusResponseTypeDef",
@@ -112,31 +110,22 @@
     "ListInstancesRequestListInstancesPaginateTypeDef",
     "ListManagedPoliciesInPermissionSetRequestListManagedPoliciesInPermissionSetPaginateTypeDef",
     "ListPermissionSetProvisioningStatusRequestListPermissionSetProvisioningStatusPaginateTypeDef",
     "ListPermissionSetsProvisionedToAccountRequestListPermissionSetsProvisionedToAccountPaginateTypeDef",
     "ListPermissionSetsRequestListPermissionSetsPaginateTypeDef",
     "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListPermissionSetProvisioningStatusResponseTypeDef",
-    "InstanceAccessControlAttributeConfigurationOutputTypeDef",
     "InstanceAccessControlAttributeConfigurationTypeDef",
     "GetPermissionsBoundaryForPermissionSetResponseTypeDef",
     "PutPermissionsBoundaryToPermissionSetRequestRequestTypeDef",
-    "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
-    "InstanceAccessControlAttributeConfigurationUnionTypeDef",
+    "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
 )
 
-AccessControlAttributeValueOutputTypeDef = TypedDict(
-    "AccessControlAttributeValueOutputTypeDef",
-    {
-        "Source": List[str],
-    },
-)
-
 AccessControlAttributeValueTypeDef = TypedDict(
     "AccessControlAttributeValueTypeDef",
     {
         "Source": Sequence[str],
     },
 )
 
@@ -638,22 +627,14 @@
 
 class UpdatePermissionSetRequestRequestTypeDef(
     _RequiredUpdatePermissionSetRequestRequestTypeDef,
     _OptionalUpdatePermissionSetRequestRequestTypeDef,
 ):
     pass
 
-AccessControlAttributeOutputTypeDef = TypedDict(
-    "AccessControlAttributeOutputTypeDef",
-    {
-        "Key": str,
-        "Value": AccessControlAttributeValueOutputTypeDef,
-    },
-)
-
 AccessControlAttributeTypeDef = TypedDict(
     "AccessControlAttributeTypeDef",
     {
         "Key": str,
         "Value": AccessControlAttributeValueTypeDef,
     },
 )
@@ -1171,21 +1152,14 @@
     {
         "PermissionSetsProvisioningStatus": List[PermissionSetProvisioningStatusMetadataTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InstanceAccessControlAttributeConfigurationOutputTypeDef = TypedDict(
-    "InstanceAccessControlAttributeConfigurationOutputTypeDef",
-    {
-        "AccessControlAttributes": List[AccessControlAttributeOutputTypeDef],
-    },
-)
-
 InstanceAccessControlAttributeConfigurationTypeDef = TypedDict(
     "InstanceAccessControlAttributeConfigurationTypeDef",
     {
         "AccessControlAttributes": Sequence[AccessControlAttributeTypeDef],
     },
 )
 
@@ -1202,40 +1176,36 @@
     {
         "InstanceArn": str,
         "PermissionSetArn": str,
         "PermissionsBoundary": PermissionsBoundaryTypeDef,
     },
 )
 
-DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef = TypedDict(
-    "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
+CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
+    "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     {
-        "Status": InstanceAccessControlAttributeConfigurationStatusType,
-        "StatusReason": str,
+        "InstanceArn": str,
         "InstanceAccessControlAttributeConfiguration": (
-            InstanceAccessControlAttributeConfigurationOutputTypeDef
+            InstanceAccessControlAttributeConfigurationTypeDef
         ),
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
-    "CreateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
+DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef = TypedDict(
+    "DescribeInstanceAccessControlAttributeConfigurationResponseTypeDef",
     {
-        "InstanceArn": str,
+        "Status": InstanceAccessControlAttributeConfigurationStatusType,
+        "StatusReason": str,
         "InstanceAccessControlAttributeConfiguration": (
             InstanceAccessControlAttributeConfigurationTypeDef
         ),
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-InstanceAccessControlAttributeConfigurationUnionTypeDef = Union[
-    InstanceAccessControlAttributeConfigurationTypeDef,
-    InstanceAccessControlAttributeConfigurationOutputTypeDef,
-]
 UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateInstanceAccessControlAttributeConfigurationRequestRequestTypeDef",
     {
         "InstanceArn": str,
         "InstanceAccessControlAttributeConfiguration": (
             InstanceAccessControlAttributeConfigurationTypeDef
         ),
```

### Comparing `types-aiobotocore-sso-admin-2.5.2.post1/types_aiobotocore_sso_admin.egg-info/SOURCES.txt` & `types-aiobotocore-sso-admin-2.5.2.post2/types_aiobotocore_sso_admin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

