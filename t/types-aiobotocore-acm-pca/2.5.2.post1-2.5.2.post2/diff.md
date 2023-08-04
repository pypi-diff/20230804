# Comparing `tmp/types-aiobotocore-acm-pca-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-acm-pca-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-acm-pca-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-acm-pca-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:19 2023, max compression
```

## Comparing `types-aiobotocore-acm-pca-2.5.2.post1.tar` & `types-aiobotocore-acm-pca-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.845667 types-aiobotocore-acm-pca-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-08-02 14:51:47.845667 types-aiobotocore-acm-pca-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16300 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:47.845667 types-aiobotocore-acm-pca-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.841667 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23882 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29793 2023-08-02 14:32:44.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29748 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-02 14:32:43.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.845667 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17817 2023-08-02 14:51:47.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 14:51:47.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:47.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:47.000000 types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.734887 types-aiobotocore-acm-pca-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:39:47.000000 types-aiobotocore-acm-pca-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-08-04 12:00:19.726886 types-aiobotocore-acm-pca-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12732 2023-08-04 11:39:47.000000 types-aiobotocore-acm-pca-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:19.734887 types-aiobotocore-acm-pca-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-04 11:39:47.000000 types-aiobotocore-acm-pca-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.726886 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-08-04 11:39:47.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-08-04 11:39:47.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-08-04 11:39:47.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23872 2023-08-04 11:39:47.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23834 2023-08-04 11:39:47.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11219 2023-08-04 11:39:48.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-08-04 11:39:48.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-08-04 11:39:47.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-08-04 11:39:47.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:39:47.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    27348 2023-08-04 11:39:48.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27305 2023-08-04 11:39:48.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:39:47.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-08-04 11:39:48.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-08-04 11:39:48.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:19.726886 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-08-04 12:00:19.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-04 12:00:19.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:19.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:19.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 12:00:19.000000 types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/LICENSE` & `types-aiobotocore-acm-pca-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/setup.py` & `types-aiobotocore-acm-pca-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-acm-pca",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_acm_pca"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ACMPCA 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/__init__.py` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/__init__.pyi` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/__main__.py` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ACMPCA 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.ACMPCA 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA\nOther"
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

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/client.py` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     ListCertificateAuthoritiesPaginator,
     ListPermissionsPaginator,
     ListTagsPaginator,
 )
 from .type_defs import (
     ApiPassthroughTypeDef,
     BlobTypeDef,
-    CertificateAuthorityConfigurationUnionTypeDef,
+    CertificateAuthorityConfigurationTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
@@ -135,15 +135,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#close)
         """
 
     async def create_certificate_authority(
         self,
         *,
-        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationUnionTypeDef,
+        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationTypeDef,
         CertificateAuthorityType: CertificateAuthorityTypeType,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
         IdempotencyToken: str = ...,
         KeyStorageSecurityStandard: KeyStorageSecurityStandardType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UsageMode: CertificateAuthorityUsageModeType = ...
     ) -> CreateCertificateAuthorityResponseTypeDef:
```

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/client.pyi` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     ListCertificateAuthoritiesPaginator,
     ListPermissionsPaginator,
     ListTagsPaginator,
 )
 from .type_defs import (
     ApiPassthroughTypeDef,
     BlobTypeDef,
-    CertificateAuthorityConfigurationUnionTypeDef,
+    CertificateAuthorityConfigurationTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
@@ -128,15 +128,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_acm_pca/client/#close)
         """
     async def create_certificate_authority(
         self,
         *,
-        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationUnionTypeDef,
+        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationTypeDef,
         CertificateAuthorityType: CertificateAuthorityTypeType,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
         IdempotencyToken: str = ...,
         KeyStorageSecurityStandard: KeyStorageSecurityStandardType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UsageMode: CertificateAuthorityUsageModeType = ...
     ) -> CreateCertificateAuthorityResponseTypeDef:
```

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/literals.py` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/literals.pyi` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/paginator.py` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/paginator.pyi` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/type_defs.py` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,14 @@
     "PermissionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OcspConfigurationTypeDef",
     "QualifierTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "RestoreCertificateAuthorityRequestRequestTypeDef",
     "RevokeCertificateRequestRequestTypeDef",
-    "ASN1SubjectOutputTypeDef",
     "ASN1SubjectTypeDef",
     "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     "CreateCertificateAuthorityResponseTypeDef",
     "DescribeCertificateAuthorityAuditReportResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCertificateAuthorityCertificateResponseTypeDef",
@@ -101,29 +100,24 @@
     "GetCertificateRequestCertificateIssuedWaitTypeDef",
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListPermissionsResponseTypeDef",
     "RevocationConfigurationTypeDef",
     "PolicyQualifierInfoTypeDef",
-    "GeneralNameOutputTypeDef",
     "GeneralNameTypeDef",
     "UpdateCertificateAuthorityRequestRequestTypeDef",
     "PolicyInformationTypeDef",
-    "AccessDescriptionOutputTypeDef",
     "AccessDescriptionTypeDef",
     "ExtensionsTypeDef",
-    "CsrExtensionsOutputTypeDef",
     "CsrExtensionsTypeDef",
     "ApiPassthroughTypeDef",
-    "CertificateAuthorityConfigurationOutputTypeDef",
     "CertificateAuthorityConfigurationTypeDef",
     "IssueCertificateRequestRequestTypeDef",
     "CertificateAuthorityTypeDef",
-    "CertificateAuthorityConfigurationUnionTypeDef",
     "CreateCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityResponseTypeDef",
     "ListCertificateAuthoritiesResponseTypeDef",
 )
 
 CustomAttributeTypeDef = TypedDict(
     "CustomAttributeTypeDef",
@@ -536,36 +530,14 @@
     {
         "CertificateAuthorityArn": str,
         "CertificateSerial": str,
         "RevocationReason": RevocationReasonType,
     },
 )
 
-ASN1SubjectOutputTypeDef = TypedDict(
-    "ASN1SubjectOutputTypeDef",
-    {
-        "Country": str,
-        "Organization": str,
-        "OrganizationalUnit": str,
-        "DistinguishedNameQualifier": str,
-        "State": str,
-        "CommonName": str,
-        "SerialNumber": str,
-        "Locality": str,
-        "Title": str,
-        "Surname": str,
-        "GivenName": str,
-        "Initials": str,
-        "Pseudonym": str,
-        "GenerationQualifier": str,
-        "CustomAttributes": List[CustomAttributeTypeDef],
-    },
-    total=False,
-)
-
 ASN1SubjectTypeDef = TypedDict(
     "ASN1SubjectTypeDef",
     {
         "Country": str,
         "Organization": str,
         "OrganizationalUnit": str,
         "DistinguishedNameQualifier": str,
@@ -851,29 +823,14 @@
     "PolicyQualifierInfoTypeDef",
     {
         "PolicyQualifierId": Literal["CPS"],
         "Qualifier": QualifierTypeDef,
     },
 )
 
-GeneralNameOutputTypeDef = TypedDict(
-    "GeneralNameOutputTypeDef",
-    {
-        "OtherName": OtherNameTypeDef,
-        "Rfc822Name": str,
-        "DnsName": str,
-        "DirectoryName": ASN1SubjectOutputTypeDef,
-        "EdiPartyName": EdiPartyNameTypeDef,
-        "UniformResourceIdentifier": str,
-        "IpAddress": str,
-        "RegisteredId": str,
-    },
-    total=False,
-)
-
 GeneralNameTypeDef = TypedDict(
     "GeneralNameTypeDef",
     {
         "OtherName": OtherNameTypeDef,
         "Rfc822Name": str,
         "DnsName": str,
         "DirectoryName": ASN1SubjectTypeDef,
@@ -925,22 +882,14 @@
 
 class PolicyInformationTypeDef(
     _RequiredPolicyInformationTypeDef, _OptionalPolicyInformationTypeDef
 ):
     pass
 
 
-AccessDescriptionOutputTypeDef = TypedDict(
-    "AccessDescriptionOutputTypeDef",
-    {
-        "AccessMethod": AccessMethodTypeDef,
-        "AccessLocation": GeneralNameOutputTypeDef,
-    },
-)
-
 AccessDescriptionTypeDef = TypedDict(
     "AccessDescriptionTypeDef",
     {
         "AccessMethod": AccessMethodTypeDef,
         "AccessLocation": GeneralNameTypeDef,
     },
 )
@@ -953,23 +902,14 @@
         "KeyUsage": KeyUsageTypeDef,
         "SubjectAlternativeNames": Sequence[GeneralNameTypeDef],
         "CustomExtensions": Sequence[CustomExtensionTypeDef],
     },
     total=False,
 )
 
-CsrExtensionsOutputTypeDef = TypedDict(
-    "CsrExtensionsOutputTypeDef",
-    {
-        "KeyUsage": KeyUsageTypeDef,
-        "SubjectInformationAccess": List[AccessDescriptionOutputTypeDef],
-    },
-    total=False,
-)
-
 CsrExtensionsTypeDef = TypedDict(
     "CsrExtensionsTypeDef",
     {
         "KeyUsage": KeyUsageTypeDef,
         "SubjectInformationAccess": Sequence[AccessDescriptionTypeDef],
     },
     total=False,
@@ -980,38 +920,14 @@
     {
         "Extensions": ExtensionsTypeDef,
         "Subject": ASN1SubjectTypeDef,
     },
     total=False,
 )
 
-_RequiredCertificateAuthorityConfigurationOutputTypeDef = TypedDict(
-    "_RequiredCertificateAuthorityConfigurationOutputTypeDef",
-    {
-        "KeyAlgorithm": KeyAlgorithmType,
-        "SigningAlgorithm": SigningAlgorithmType,
-        "Subject": ASN1SubjectOutputTypeDef,
-    },
-)
-_OptionalCertificateAuthorityConfigurationOutputTypeDef = TypedDict(
-    "_OptionalCertificateAuthorityConfigurationOutputTypeDef",
-    {
-        "CsrExtensions": CsrExtensionsOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class CertificateAuthorityConfigurationOutputTypeDef(
-    _RequiredCertificateAuthorityConfigurationOutputTypeDef,
-    _OptionalCertificateAuthorityConfigurationOutputTypeDef,
-):
-    pass
-
-
 _RequiredCertificateAuthorityConfigurationTypeDef = TypedDict(
     "_RequiredCertificateAuthorityConfigurationTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "SigningAlgorithm": SigningAlgorithmType,
         "Subject": ASN1SubjectTypeDef,
     },
@@ -1068,26 +984,23 @@
         "LastStateChangeAt": datetime,
         "Type": CertificateAuthorityTypeType,
         "Serial": str,
         "Status": CertificateAuthorityStatusType,
         "NotBefore": datetime,
         "NotAfter": datetime,
         "FailureReason": FailureReasonType,
-        "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationOutputTypeDef,
+        "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
         "RevocationConfiguration": RevocationConfigurationTypeDef,
         "RestorableUntil": datetime,
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
 
-CertificateAuthorityConfigurationUnionTypeDef = Union[
-    CertificateAuthorityConfigurationTypeDef, CertificateAuthorityConfigurationOutputTypeDef
-]
 _RequiredCreateCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
         "CertificateAuthorityType": CertificateAuthorityTypeType,
     },
 )
```

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/type_defs.pyi` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,14 @@
     "PermissionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OcspConfigurationTypeDef",
     "QualifierTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "RestoreCertificateAuthorityRequestRequestTypeDef",
     "RevokeCertificateRequestRequestTypeDef",
-    "ASN1SubjectOutputTypeDef",
     "ASN1SubjectTypeDef",
     "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     "CreateCertificateAuthorityResponseTypeDef",
     "DescribeCertificateAuthorityAuditReportResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCertificateAuthorityCertificateResponseTypeDef",
@@ -100,29 +99,24 @@
     "GetCertificateRequestCertificateIssuedWaitTypeDef",
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListPermissionsResponseTypeDef",
     "RevocationConfigurationTypeDef",
     "PolicyQualifierInfoTypeDef",
-    "GeneralNameOutputTypeDef",
     "GeneralNameTypeDef",
     "UpdateCertificateAuthorityRequestRequestTypeDef",
     "PolicyInformationTypeDef",
-    "AccessDescriptionOutputTypeDef",
     "AccessDescriptionTypeDef",
     "ExtensionsTypeDef",
-    "CsrExtensionsOutputTypeDef",
     "CsrExtensionsTypeDef",
     "ApiPassthroughTypeDef",
-    "CertificateAuthorityConfigurationOutputTypeDef",
     "CertificateAuthorityConfigurationTypeDef",
     "IssueCertificateRequestRequestTypeDef",
     "CertificateAuthorityTypeDef",
-    "CertificateAuthorityConfigurationUnionTypeDef",
     "CreateCertificateAuthorityRequestRequestTypeDef",
     "DescribeCertificateAuthorityResponseTypeDef",
     "ListCertificateAuthoritiesResponseTypeDef",
 )
 
 CustomAttributeTypeDef = TypedDict(
     "CustomAttributeTypeDef",
@@ -515,36 +509,14 @@
     {
         "CertificateAuthorityArn": str,
         "CertificateSerial": str,
         "RevocationReason": RevocationReasonType,
     },
 )
 
-ASN1SubjectOutputTypeDef = TypedDict(
-    "ASN1SubjectOutputTypeDef",
-    {
-        "Country": str,
-        "Organization": str,
-        "OrganizationalUnit": str,
-        "DistinguishedNameQualifier": str,
-        "State": str,
-        "CommonName": str,
-        "SerialNumber": str,
-        "Locality": str,
-        "Title": str,
-        "Surname": str,
-        "GivenName": str,
-        "Initials": str,
-        "Pseudonym": str,
-        "GenerationQualifier": str,
-        "CustomAttributes": List[CustomAttributeTypeDef],
-    },
-    total=False,
-)
-
 ASN1SubjectTypeDef = TypedDict(
     "ASN1SubjectTypeDef",
     {
         "Country": str,
         "Organization": str,
         "OrganizationalUnit": str,
         "DistinguishedNameQualifier": str,
@@ -818,29 +790,14 @@
     "PolicyQualifierInfoTypeDef",
     {
         "PolicyQualifierId": Literal["CPS"],
         "Qualifier": QualifierTypeDef,
     },
 )
 
-GeneralNameOutputTypeDef = TypedDict(
-    "GeneralNameOutputTypeDef",
-    {
-        "OtherName": OtherNameTypeDef,
-        "Rfc822Name": str,
-        "DnsName": str,
-        "DirectoryName": ASN1SubjectOutputTypeDef,
-        "EdiPartyName": EdiPartyNameTypeDef,
-        "UniformResourceIdentifier": str,
-        "IpAddress": str,
-        "RegisteredId": str,
-    },
-    total=False,
-)
-
 GeneralNameTypeDef = TypedDict(
     "GeneralNameTypeDef",
     {
         "OtherName": OtherNameTypeDef,
         "Rfc822Name": str,
         "DnsName": str,
         "DirectoryName": ASN1SubjectTypeDef,
@@ -888,22 +845,14 @@
 )
 
 class PolicyInformationTypeDef(
     _RequiredPolicyInformationTypeDef, _OptionalPolicyInformationTypeDef
 ):
     pass
 
-AccessDescriptionOutputTypeDef = TypedDict(
-    "AccessDescriptionOutputTypeDef",
-    {
-        "AccessMethod": AccessMethodTypeDef,
-        "AccessLocation": GeneralNameOutputTypeDef,
-    },
-)
-
 AccessDescriptionTypeDef = TypedDict(
     "AccessDescriptionTypeDef",
     {
         "AccessMethod": AccessMethodTypeDef,
         "AccessLocation": GeneralNameTypeDef,
     },
 )
@@ -916,23 +865,14 @@
         "KeyUsage": KeyUsageTypeDef,
         "SubjectAlternativeNames": Sequence[GeneralNameTypeDef],
         "CustomExtensions": Sequence[CustomExtensionTypeDef],
     },
     total=False,
 )
 
-CsrExtensionsOutputTypeDef = TypedDict(
-    "CsrExtensionsOutputTypeDef",
-    {
-        "KeyUsage": KeyUsageTypeDef,
-        "SubjectInformationAccess": List[AccessDescriptionOutputTypeDef],
-    },
-    total=False,
-)
-
 CsrExtensionsTypeDef = TypedDict(
     "CsrExtensionsTypeDef",
     {
         "KeyUsage": KeyUsageTypeDef,
         "SubjectInformationAccess": Sequence[AccessDescriptionTypeDef],
     },
     total=False,
@@ -943,36 +883,14 @@
     {
         "Extensions": ExtensionsTypeDef,
         "Subject": ASN1SubjectTypeDef,
     },
     total=False,
 )
 
-_RequiredCertificateAuthorityConfigurationOutputTypeDef = TypedDict(
-    "_RequiredCertificateAuthorityConfigurationOutputTypeDef",
-    {
-        "KeyAlgorithm": KeyAlgorithmType,
-        "SigningAlgorithm": SigningAlgorithmType,
-        "Subject": ASN1SubjectOutputTypeDef,
-    },
-)
-_OptionalCertificateAuthorityConfigurationOutputTypeDef = TypedDict(
-    "_OptionalCertificateAuthorityConfigurationOutputTypeDef",
-    {
-        "CsrExtensions": CsrExtensionsOutputTypeDef,
-    },
-    total=False,
-)
-
-class CertificateAuthorityConfigurationOutputTypeDef(
-    _RequiredCertificateAuthorityConfigurationOutputTypeDef,
-    _OptionalCertificateAuthorityConfigurationOutputTypeDef,
-):
-    pass
-
 _RequiredCertificateAuthorityConfigurationTypeDef = TypedDict(
     "_RequiredCertificateAuthorityConfigurationTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "SigningAlgorithm": SigningAlgorithmType,
         "Subject": ASN1SubjectTypeDef,
     },
@@ -1025,26 +943,23 @@
         "LastStateChangeAt": datetime,
         "Type": CertificateAuthorityTypeType,
         "Serial": str,
         "Status": CertificateAuthorityStatusType,
         "NotBefore": datetime,
         "NotAfter": datetime,
         "FailureReason": FailureReasonType,
-        "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationOutputTypeDef,
+        "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
         "RevocationConfiguration": RevocationConfigurationTypeDef,
         "RestorableUntil": datetime,
         "KeyStorageSecurityStandard": KeyStorageSecurityStandardType,
         "UsageMode": CertificateAuthorityUsageModeType,
     },
     total=False,
 )
 
-CertificateAuthorityConfigurationUnionTypeDef = Union[
-    CertificateAuthorityConfigurationTypeDef, CertificateAuthorityConfigurationOutputTypeDef
-]
 _RequiredCreateCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
         "CertificateAuthorityType": CertificateAuthorityTypeType,
     },
 )
```

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/waiter.py` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca/waiter.pyi` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-acm-pca-2.5.2.post1/types_aiobotocore_acm_pca.egg-info/SOURCES.txt` & `types-aiobotocore-acm-pca-2.5.2.post2/types_aiobotocore_acm_pca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

