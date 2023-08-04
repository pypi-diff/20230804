# Comparing `tmp/types-aiobotocore-route53domains-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-route53domains-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53domains-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53domains-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:23 2023, max compression
```

## Comparing `types-aiobotocore-route53domains-2.5.2.post1.tar` & `types-aiobotocore-route53domains-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.005475 types-aiobotocore-route53domains-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-08-02 14:52:55.001475 types-aiobotocore-route53domains-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16113 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:55.005475 types-aiobotocore-route53domains-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.997475 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30925 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30878 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13230 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    28794 2023-08-02 14:48:10.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    28772 2023-08-02 14:48:10.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:09.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:55.001475 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17659 2023-08-02 14:52:54.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:54.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:54.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:54.000000 types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.946643 types-aiobotocore-route53domains-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:51:13.000000 types-aiobotocore-route53domains-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13744 2023-08-04 13:59:23.946643 types-aiobotocore-route53domains-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12198 2023-08-04 13:51:13.000000 types-aiobotocore-route53domains-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:23.946643 types-aiobotocore-route53domains-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2121 2023-08-04 13:51:13.000000 types-aiobotocore-route53domains-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.946643 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1237 2023-08-04 13:51:13.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1236 2023-08-04 13:51:13.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      971 2023-08-04 13:51:13.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    30828 2023-08-04 13:51:13.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    30781 2023-08-04 13:51:13.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13327 2023-08-04 13:51:14.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13325 2023-08-04 13:51:13.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6049 2023-08-04 13:51:13.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6042 2023-08-04 13:51:13.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:51:13.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27570 2023-08-04 13:51:17.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    27549 2023-08-04 13:51:14.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:51:13.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:23.946643 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13744 2023-08-04 13:59:23.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:23.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:23.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:23.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:23.000000 types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/LICENSE` & `types-aiobotocore-route53domains-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/setup.py` & `types-aiobotocore-route53domains-2.5.2.post2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53domains",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_route53domains"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Route53Domains 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/__init__.py` & `types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/__init__.pyi` & `types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/__main__.py` & `types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.Route53Domains 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains\nOther"
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

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/client.py` & `types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from .type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ConsentTypeDef,
-    ContactDetailUnionTypeDef,
+    ContactDetailTypeDef,
     DeleteDomainResponseTypeDef,
     DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecSigningAttributesTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
@@ -46,15 +46,15 @@
     GetDomainDetailResponseTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     GetOperationDetailResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListPricesResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
-    NameserverUnionTypeDef,
+    NameserverTypeDef,
     RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     SortConditionTypeDef,
     TagTypeDef,
@@ -370,17 +370,17 @@
         """
 
     async def register_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: ContactDetailUnionTypeDef,
-        RegistrantContact: ContactDetailUnionTypeDef,
-        TechContact: ContactDetailUnionTypeDef,
+        AdminContact: ContactDetailTypeDef,
+        RegistrantContact: ContactDetailTypeDef,
+        TechContact: ContactDetailTypeDef,
         IdnLangCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> RegisterDomainResponseTypeDef:
         """
@@ -445,19 +445,19 @@
         """
 
     async def transfer_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: ContactDetailUnionTypeDef,
-        RegistrantContact: ContactDetailUnionTypeDef,
-        TechContact: ContactDetailUnionTypeDef,
+        AdminContact: ContactDetailTypeDef,
+        RegistrantContact: ContactDetailTypeDef,
+        TechContact: ContactDetailTypeDef,
         IdnLangCode: str = ...,
-        Nameservers: Sequence[NameserverUnionTypeDef] = ...,
+        Nameservers: Sequence[NameserverTypeDef] = ...,
         AuthCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> TransferDomainResponseTypeDef:
         """
@@ -478,17 +478,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#transfer_domain_to_another_aws_account)
         """
 
     async def update_domain_contact(
         self,
         *,
         DomainName: str,
-        AdminContact: ContactDetailUnionTypeDef = ...,
-        RegistrantContact: ContactDetailUnionTypeDef = ...,
-        TechContact: ContactDetailUnionTypeDef = ...,
+        AdminContact: ContactDetailTypeDef = ...,
+        RegistrantContact: ContactDetailTypeDef = ...,
+        TechContact: ContactDetailTypeDef = ...,
         Consent: ConsentTypeDef = ...
     ) -> UpdateDomainContactResponseTypeDef:
         """
         This operation updates the contact information for a particular domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_contact)
@@ -506,19 +506,15 @@
         This operation updates the specified domain contact's privacy setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact_privacy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_contact_privacy)
         """
 
     async def update_domain_nameservers(
-        self,
-        *,
-        DomainName: str,
-        Nameservers: Sequence[NameserverUnionTypeDef],
-        FIAuthKey: str = ...
+        self, *, DomainName: str, Nameservers: Sequence[NameserverTypeDef], FIAuthKey: str = ...
     ) -> UpdateDomainNameserversResponseTypeDef:
         """
         This operation replaces the current set of name servers for the domain with the
         specified set of name servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_nameservers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_nameservers)
```

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/client.pyi` & `types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from .type_defs import (
     AcceptDomainTransferFromAnotherAwsAccountResponseTypeDef,
     AssociateDelegationSignerToDomainResponseTypeDef,
     CancelDomainTransferToAnotherAwsAccountResponseTypeDef,
     CheckDomainAvailabilityResponseTypeDef,
     CheckDomainTransferabilityResponseTypeDef,
     ConsentTypeDef,
-    ContactDetailUnionTypeDef,
+    ContactDetailTypeDef,
     DeleteDomainResponseTypeDef,
     DisableDomainTransferLockResponseTypeDef,
     DisassociateDelegationSignerFromDomainResponseTypeDef,
     DnssecSigningAttributesTypeDef,
     EmptyResponseMetadataTypeDef,
     EnableDomainTransferLockResponseTypeDef,
     FilterConditionTypeDef,
@@ -46,15 +46,15 @@
     GetDomainDetailResponseTypeDef,
     GetDomainSuggestionsResponseTypeDef,
     GetOperationDetailResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListOperationsResponseTypeDef,
     ListPricesResponseTypeDef,
     ListTagsForDomainResponseTypeDef,
-    NameserverUnionTypeDef,
+    NameserverTypeDef,
     RegisterDomainResponseTypeDef,
     RejectDomainTransferFromAnotherAwsAccountResponseTypeDef,
     RenewDomainResponseTypeDef,
     ResendContactReachabilityEmailResponseTypeDef,
     RetrieveDomainAuthCodeResponseTypeDef,
     SortConditionTypeDef,
     TagTypeDef,
@@ -341,17 +341,17 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#push_domain)
         """
     async def register_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: ContactDetailUnionTypeDef,
-        RegistrantContact: ContactDetailUnionTypeDef,
-        TechContact: ContactDetailUnionTypeDef,
+        AdminContact: ContactDetailTypeDef,
+        RegistrantContact: ContactDetailTypeDef,
+        TechContact: ContactDetailTypeDef,
         IdnLangCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> RegisterDomainResponseTypeDef:
         """
@@ -410,19 +410,19 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#retrieve_domain_auth_code)
         """
     async def transfer_domain(
         self,
         *,
         DomainName: str,
         DurationInYears: int,
-        AdminContact: ContactDetailUnionTypeDef,
-        RegistrantContact: ContactDetailUnionTypeDef,
-        TechContact: ContactDetailUnionTypeDef,
+        AdminContact: ContactDetailTypeDef,
+        RegistrantContact: ContactDetailTypeDef,
+        TechContact: ContactDetailTypeDef,
         IdnLangCode: str = ...,
-        Nameservers: Sequence[NameserverUnionTypeDef] = ...,
+        Nameservers: Sequence[NameserverTypeDef] = ...,
         AuthCode: str = ...,
         AutoRenew: bool = ...,
         PrivacyProtectAdminContact: bool = ...,
         PrivacyProtectRegistrantContact: bool = ...,
         PrivacyProtectTechContact: bool = ...
     ) -> TransferDomainResponseTypeDef:
         """
@@ -441,17 +441,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.transfer_domain_to_another_aws_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#transfer_domain_to_another_aws_account)
         """
     async def update_domain_contact(
         self,
         *,
         DomainName: str,
-        AdminContact: ContactDetailUnionTypeDef = ...,
-        RegistrantContact: ContactDetailUnionTypeDef = ...,
-        TechContact: ContactDetailUnionTypeDef = ...,
+        AdminContact: ContactDetailTypeDef = ...,
+        RegistrantContact: ContactDetailTypeDef = ...,
+        TechContact: ContactDetailTypeDef = ...,
         Consent: ConsentTypeDef = ...
     ) -> UpdateDomainContactResponseTypeDef:
         """
         This operation updates the contact information for a particular domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_contact)
@@ -467,19 +467,15 @@
         """
         This operation updates the specified domain contact's privacy setting.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_contact_privacy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_contact_privacy)
         """
     async def update_domain_nameservers(
-        self,
-        *,
-        DomainName: str,
-        Nameservers: Sequence[NameserverUnionTypeDef],
-        FIAuthKey: str = ...
+        self, *, DomainName: str, Nameservers: Sequence[NameserverTypeDef], FIAuthKey: str = ...
     ) -> UpdateDomainNameserversResponseTypeDef:
         """
         This operation replaces the current set of name servers for the domain with the
         specified set of name servers.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53domains.html#Route53Domains.Client.update_domain_nameservers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53domains/client/#update_domain_nameservers)
```

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/literals.py` & `types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "ContactTypeType",
     "CountryCodeType",
     "DomainAvailabilityType",
     "ExtraParamNameType",
     "ListDomainsAttributeNameType",
     "ListDomainsPaginatorName",
@@ -40,15 +39,14 @@
     "Route53DomainsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
-
 ContactTypeType = Literal["ASSOCIATION", "COMPANY", "PERSON", "PUBLIC_BODY", "RESELLER"]
 CountryCodeType = Literal[
     "AC",
     "AD",
     "AE",
     "AF",
     "AG",
@@ -399,14 +397,15 @@
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
@@ -502,14 +501,15 @@
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
@@ -588,26 +588,28 @@
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

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/literals.pyi` & `types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/literals.py`

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
     "ContactTypeType",
     "CountryCodeType",
     "DomainAvailabilityType",
     "ExtraParamNameType",
     "ListDomainsAttributeNameType",
     "ListDomainsPaginatorName",
@@ -39,14 +40,15 @@
     "Route53DomainsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
+
 ContactTypeType = Literal["ASSOCIATION", "COMPANY", "PERSON", "PUBLIC_BODY", "RESELLER"]
 CountryCodeType = Literal[
     "AC",
     "AD",
     "AE",
     "AF",
     "AG",
@@ -397,14 +399,15 @@
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
@@ -500,14 +503,15 @@
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
@@ -586,26 +590,28 @@
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

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/paginator.py` & `types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/paginator.pyi` & `types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/type_defs.py` & `types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,25 +61,24 @@
     "DomainSuggestionTypeDef",
     "DomainSummaryTypeDef",
     "EnableDomainAutoRenewRequestRequestTypeDef",
     "EnableDomainTransferLockRequestRequestTypeDef",
     "FilterConditionTypeDef",
     "GetContactReachabilityStatusRequestRequestTypeDef",
     "GetDomainDetailRequestRequestTypeDef",
-    "NameserverOutputTypeDef",
+    "NameserverTypeDef",
     "GetDomainSuggestionsRequestRequestTypeDef",
     "GetOperationDetailRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "SortConditionTypeDef",
     "TimestampTypeDef",
     "OperationSummaryTypeDef",
     "ListPricesRequestRequestTypeDef",
     "ListTagsForDomainRequestRequestTypeDef",
     "TagTypeDef",
-    "NameserverTypeDef",
     "PushDomainRequestRequestTypeDef",
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     "RenewDomainRequestRequestTypeDef",
     "ResendContactReachabilityEmailRequestRequestTypeDef",
     "ResendOperationAuthorizationRequestRequestTypeDef",
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
     "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
@@ -104,37 +103,34 @@
     "TransferDomainToAnotherAwsAccountResponseTypeDef",
     "UpdateDomainContactPrivacyResponseTypeDef",
     "UpdateDomainContactResponseTypeDef",
     "UpdateDomainNameserversResponseTypeDef",
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     "ViewBillingResponseTypeDef",
     "CheckDomainTransferabilityResponseTypeDef",
-    "ContactDetailOutputTypeDef",
     "ContactDetailTypeDef",
     "DomainPriceTypeDef",
     "GetDomainSuggestionsResponseTypeDef",
     "ListDomainsResponseTypeDef",
+    "UpdateDomainNameserversRequestRequestTypeDef",
     "ListPricesRequestListPricesPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "ViewBillingRequestRequestTypeDef",
     "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListOperationsResponseTypeDef",
     "ListTagsForDomainResponseTypeDef",
     "UpdateTagsForDomainRequestRequestTypeDef",
-    "NameserverUnionTypeDef",
     "GetDomainDetailResponseTypeDef",
-    "ContactDetailUnionTypeDef",
     "RegisterDomainRequestRequestTypeDef",
+    "TransferDomainRequestRequestTypeDef",
     "UpdateDomainContactRequestRequestTypeDef",
     "ListPricesResponseTypeDef",
-    "TransferDomainRequestRequestTypeDef",
-    "UpdateDomainNameserversRequestRequestTypeDef",
 )
 
 AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "Password": str,
@@ -362,30 +358,30 @@
 GetDomainDetailRequestRequestTypeDef = TypedDict(
     "GetDomainDetailRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-_RequiredNameserverOutputTypeDef = TypedDict(
-    "_RequiredNameserverOutputTypeDef",
+_RequiredNameserverTypeDef = TypedDict(
+    "_RequiredNameserverTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalNameserverOutputTypeDef = TypedDict(
-    "_OptionalNameserverOutputTypeDef",
+_OptionalNameserverTypeDef = TypedDict(
+    "_OptionalNameserverTypeDef",
     {
         "GlueIps": List[str],
     },
     total=False,
 )
 
 
-class NameserverOutputTypeDef(_RequiredNameserverOutputTypeDef, _OptionalNameserverOutputTypeDef):
+class NameserverTypeDef(_RequiredNameserverTypeDef, _OptionalNameserverTypeDef):
     pass
 
 
 GetDomainSuggestionsRequestRequestTypeDef = TypedDict(
     "GetDomainSuggestionsRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -457,33 +453,14 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredNameserverTypeDef = TypedDict(
-    "_RequiredNameserverTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalNameserverTypeDef = TypedDict(
-    "_OptionalNameserverTypeDef",
-    {
-        "GlueIps": Sequence[str],
-    },
-    total=False,
-)
-
-
-class NameserverTypeDef(_RequiredNameserverTypeDef, _OptionalNameserverTypeDef):
-    pass
-
-
 PushDomainRequestRequestTypeDef = TypedDict(
     "PushDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Target": str,
     },
 )
@@ -770,35 +747,14 @@
     "CheckDomainTransferabilityResponseTypeDef",
     {
         "Transferability": DomainTransferabilityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ContactDetailOutputTypeDef = TypedDict(
-    "ContactDetailOutputTypeDef",
-    {
-        "FirstName": str,
-        "LastName": str,
-        "ContactType": ContactTypeType,
-        "OrganizationName": str,
-        "AddressLine1": str,
-        "AddressLine2": str,
-        "City": str,
-        "State": str,
-        "CountryCode": CountryCodeType,
-        "ZipCode": str,
-        "PhoneNumber": str,
-        "Email": str,
-        "Fax": str,
-        "ExtraParams": List[ExtraParamTypeDef],
-    },
-    total=False,
-)
-
 ContactDetailTypeDef = TypedDict(
     "ContactDetailTypeDef",
     {
         "FirstName": str,
         "LastName": str,
         "ContactType": ContactTypeType,
         "OrganizationName": str,
@@ -807,15 +763,15 @@
         "City": str,
         "State": str,
         "CountryCode": CountryCodeType,
         "ZipCode": str,
         "PhoneNumber": str,
         "Email": str,
         "Fax": str,
-        "ExtraParams": Sequence[ExtraParamTypeDef],
+        "ExtraParams": List[ExtraParamTypeDef],
     },
     total=False,
 )
 
 DomainPriceTypeDef = TypedDict(
     "DomainPriceTypeDef",
     {
@@ -842,14 +798,37 @@
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextPageMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "Nameservers": Sequence[NameserverTypeDef],
+    },
+)
+_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
+    {
+        "FIAuthKey": str,
+    },
+    total=False,
+)
+
+
+class UpdateDomainNameserversRequestRequestTypeDef(
+    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
+    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
+):
+    pass
+
+
 ListPricesRequestListPricesPaginateTypeDef = TypedDict(
     "ListPricesRequestListPricesPaginateTypeDef",
     {
         "Tld": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -959,24 +938,23 @@
 class UpdateTagsForDomainRequestRequestTypeDef(
     _RequiredUpdateTagsForDomainRequestRequestTypeDef,
     _OptionalUpdateTagsForDomainRequestRequestTypeDef,
 ):
     pass
 
 
-NameserverUnionTypeDef = Union[NameserverTypeDef, NameserverOutputTypeDef]
 GetDomainDetailResponseTypeDef = TypedDict(
     "GetDomainDetailResponseTypeDef",
     {
         "DomainName": str,
-        "Nameservers": List[NameserverOutputTypeDef],
+        "Nameservers": List[NameserverTypeDef],
         "AutoRenew": bool,
-        "AdminContact": ContactDetailOutputTypeDef,
-        "RegistrantContact": ContactDetailOutputTypeDef,
-        "TechContact": ContactDetailOutputTypeDef,
+        "AdminContact": ContactDetailTypeDef,
+        "RegistrantContact": ContactDetailTypeDef,
+        "TechContact": ContactDetailTypeDef,
         "AdminPrivacy": bool,
         "RegistrantPrivacy": bool,
         "TechPrivacy": bool,
         "RegistrarName": str,
         "WhoIsServer": str,
         "RegistrarUrl": str,
         "AbuseContactEmail": str,
@@ -989,15 +967,14 @@
         "DnsSec": str,
         "StatusList": List[str],
         "DnssecKeys": List[DnssecKeyTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ContactDetailUnionTypeDef = Union[ContactDetailTypeDef, ContactDetailOutputTypeDef]
 _RequiredRegisterDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
         "RegistrantContact": ContactDetailTypeDef,
@@ -1019,63 +996,29 @@
 
 class RegisterDomainRequestRequestTypeDef(
     _RequiredRegisterDomainRequestRequestTypeDef, _OptionalRegisterDomainRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainContactRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainContactRequestRequestTypeDef",
-    {
-        "AdminContact": ContactDetailTypeDef,
-        "RegistrantContact": ContactDetailTypeDef,
-        "TechContact": ContactDetailTypeDef,
-        "Consent": ConsentTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateDomainContactRequestRequestTypeDef(
-    _RequiredUpdateDomainContactRequestRequestTypeDef,
-    _OptionalUpdateDomainContactRequestRequestTypeDef,
-):
-    pass
-
-
-ListPricesResponseTypeDef = TypedDict(
-    "ListPricesResponseTypeDef",
-    {
-        "Prices": List[DomainPriceTypeDef],
-        "NextPageMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredTransferDomainRequestRequestTypeDef = TypedDict(
     "_RequiredTransferDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
         "RegistrantContact": ContactDetailTypeDef,
         "TechContact": ContactDetailTypeDef,
     },
 )
 _OptionalTransferDomainRequestRequestTypeDef = TypedDict(
     "_OptionalTransferDomainRequestRequestTypeDef",
     {
         "IdnLangCode": str,
-        "Nameservers": Sequence[NameserverUnionTypeDef],
+        "Nameservers": Sequence[NameserverTypeDef],
         "AuthCode": str,
         "AutoRenew": bool,
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
@@ -1084,28 +1027,40 @@
 
 class TransferDomainRequestRequestTypeDef(
     _RequiredTransferDomainRequestRequestTypeDef, _OptionalTransferDomainRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
+_RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainContactRequestRequestTypeDef",
     {
         "DomainName": str,
-        "Nameservers": Sequence[NameserverUnionTypeDef],
     },
 )
-_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
+_OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainContactRequestRequestTypeDef",
     {
-        "FIAuthKey": str,
+        "AdminContact": ContactDetailTypeDef,
+        "RegistrantContact": ContactDetailTypeDef,
+        "TechContact": ContactDetailTypeDef,
+        "Consent": ConsentTypeDef,
     },
     total=False,
 )
 
 
-class UpdateDomainNameserversRequestRequestTypeDef(
-    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
-    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
+class UpdateDomainContactRequestRequestTypeDef(
+    _RequiredUpdateDomainContactRequestRequestTypeDef,
+    _OptionalUpdateDomainContactRequestRequestTypeDef,
 ):
     pass
+
+
+ListPricesResponseTypeDef = TypedDict(
+    "ListPricesResponseTypeDef",
+    {
+        "Prices": List[DomainPriceTypeDef],
+        "NextPageMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains/type_defs.pyi` & `types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,25 +60,24 @@
     "DomainSuggestionTypeDef",
     "DomainSummaryTypeDef",
     "EnableDomainAutoRenewRequestRequestTypeDef",
     "EnableDomainTransferLockRequestRequestTypeDef",
     "FilterConditionTypeDef",
     "GetContactReachabilityStatusRequestRequestTypeDef",
     "GetDomainDetailRequestRequestTypeDef",
-    "NameserverOutputTypeDef",
+    "NameserverTypeDef",
     "GetDomainSuggestionsRequestRequestTypeDef",
     "GetOperationDetailRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "SortConditionTypeDef",
     "TimestampTypeDef",
     "OperationSummaryTypeDef",
     "ListPricesRequestRequestTypeDef",
     "ListTagsForDomainRequestRequestTypeDef",
     "TagTypeDef",
-    "NameserverTypeDef",
     "PushDomainRequestRequestTypeDef",
     "RejectDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     "RenewDomainRequestRequestTypeDef",
     "ResendContactReachabilityEmailRequestRequestTypeDef",
     "ResendOperationAuthorizationRequestRequestTypeDef",
     "RetrieveDomainAuthCodeRequestRequestTypeDef",
     "TransferDomainToAnotherAwsAccountRequestRequestTypeDef",
@@ -103,37 +102,34 @@
     "TransferDomainToAnotherAwsAccountResponseTypeDef",
     "UpdateDomainContactPrivacyResponseTypeDef",
     "UpdateDomainContactResponseTypeDef",
     "UpdateDomainNameserversResponseTypeDef",
     "AssociateDelegationSignerToDomainRequestRequestTypeDef",
     "ViewBillingResponseTypeDef",
     "CheckDomainTransferabilityResponseTypeDef",
-    "ContactDetailOutputTypeDef",
     "ContactDetailTypeDef",
     "DomainPriceTypeDef",
     "GetDomainSuggestionsResponseTypeDef",
     "ListDomainsResponseTypeDef",
+    "UpdateDomainNameserversRequestRequestTypeDef",
     "ListPricesRequestListPricesPaginateTypeDef",
     "ListDomainsRequestListDomainsPaginateTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListOperationsRequestListOperationsPaginateTypeDef",
     "ListOperationsRequestRequestTypeDef",
     "ViewBillingRequestRequestTypeDef",
     "ViewBillingRequestViewBillingPaginateTypeDef",
     "ListOperationsResponseTypeDef",
     "ListTagsForDomainResponseTypeDef",
     "UpdateTagsForDomainRequestRequestTypeDef",
-    "NameserverUnionTypeDef",
     "GetDomainDetailResponseTypeDef",
-    "ContactDetailUnionTypeDef",
     "RegisterDomainRequestRequestTypeDef",
+    "TransferDomainRequestRequestTypeDef",
     "UpdateDomainContactRequestRequestTypeDef",
     "ListPricesResponseTypeDef",
-    "TransferDomainRequestRequestTypeDef",
-    "UpdateDomainNameserversRequestRequestTypeDef",
 )
 
 AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef = TypedDict(
     "AcceptDomainTransferFromAnotherAwsAccountRequestRequestTypeDef",
     {
         "DomainName": str,
         "Password": str,
@@ -357,29 +353,29 @@
 GetDomainDetailRequestRequestTypeDef = TypedDict(
     "GetDomainDetailRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-_RequiredNameserverOutputTypeDef = TypedDict(
-    "_RequiredNameserverOutputTypeDef",
+_RequiredNameserverTypeDef = TypedDict(
+    "_RequiredNameserverTypeDef",
     {
         "Name": str,
     },
 )
-_OptionalNameserverOutputTypeDef = TypedDict(
-    "_OptionalNameserverOutputTypeDef",
+_OptionalNameserverTypeDef = TypedDict(
+    "_OptionalNameserverTypeDef",
     {
         "GlueIps": List[str],
     },
     total=False,
 )
 
-class NameserverOutputTypeDef(_RequiredNameserverOutputTypeDef, _OptionalNameserverOutputTypeDef):
+class NameserverTypeDef(_RequiredNameserverTypeDef, _OptionalNameserverTypeDef):
     pass
 
 GetDomainSuggestionsRequestRequestTypeDef = TypedDict(
     "GetDomainSuggestionsRequestRequestTypeDef",
     {
         "DomainName": str,
         "SuggestionCount": int,
@@ -450,31 +446,14 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-_RequiredNameserverTypeDef = TypedDict(
-    "_RequiredNameserverTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalNameserverTypeDef = TypedDict(
-    "_OptionalNameserverTypeDef",
-    {
-        "GlueIps": Sequence[str],
-    },
-    total=False,
-)
-
-class NameserverTypeDef(_RequiredNameserverTypeDef, _OptionalNameserverTypeDef):
-    pass
-
 PushDomainRequestRequestTypeDef = TypedDict(
     "PushDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "Target": str,
     },
 )
@@ -757,35 +736,14 @@
     "CheckDomainTransferabilityResponseTypeDef",
     {
         "Transferability": DomainTransferabilityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ContactDetailOutputTypeDef = TypedDict(
-    "ContactDetailOutputTypeDef",
-    {
-        "FirstName": str,
-        "LastName": str,
-        "ContactType": ContactTypeType,
-        "OrganizationName": str,
-        "AddressLine1": str,
-        "AddressLine2": str,
-        "City": str,
-        "State": str,
-        "CountryCode": CountryCodeType,
-        "ZipCode": str,
-        "PhoneNumber": str,
-        "Email": str,
-        "Fax": str,
-        "ExtraParams": List[ExtraParamTypeDef],
-    },
-    total=False,
-)
-
 ContactDetailTypeDef = TypedDict(
     "ContactDetailTypeDef",
     {
         "FirstName": str,
         "LastName": str,
         "ContactType": ContactTypeType,
         "OrganizationName": str,
@@ -794,15 +752,15 @@
         "City": str,
         "State": str,
         "CountryCode": CountryCodeType,
         "ZipCode": str,
         "PhoneNumber": str,
         "Email": str,
         "Fax": str,
-        "ExtraParams": Sequence[ExtraParamTypeDef],
+        "ExtraParams": List[ExtraParamTypeDef],
     },
     total=False,
 )
 
 DomainPriceTypeDef = TypedDict(
     "DomainPriceTypeDef",
     {
@@ -829,14 +787,35 @@
     {
         "Domains": List[DomainSummaryTypeDef],
         "NextPageMarker": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
+    {
+        "DomainName": str,
+        "Nameservers": Sequence[NameserverTypeDef],
+    },
+)
+_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
+    {
+        "FIAuthKey": str,
+    },
+    total=False,
+)
+
+class UpdateDomainNameserversRequestRequestTypeDef(
+    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
+    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
+):
+    pass
+
 ListPricesRequestListPricesPaginateTypeDef = TypedDict(
     "ListPricesRequestListPricesPaginateTypeDef",
     {
         "Tld": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -944,24 +923,23 @@
 
 class UpdateTagsForDomainRequestRequestTypeDef(
     _RequiredUpdateTagsForDomainRequestRequestTypeDef,
     _OptionalUpdateTagsForDomainRequestRequestTypeDef,
 ):
     pass
 
-NameserverUnionTypeDef = Union[NameserverTypeDef, NameserverOutputTypeDef]
 GetDomainDetailResponseTypeDef = TypedDict(
     "GetDomainDetailResponseTypeDef",
     {
         "DomainName": str,
-        "Nameservers": List[NameserverOutputTypeDef],
+        "Nameservers": List[NameserverTypeDef],
         "AutoRenew": bool,
-        "AdminContact": ContactDetailOutputTypeDef,
-        "RegistrantContact": ContactDetailOutputTypeDef,
-        "TechContact": ContactDetailOutputTypeDef,
+        "AdminContact": ContactDetailTypeDef,
+        "RegistrantContact": ContactDetailTypeDef,
+        "TechContact": ContactDetailTypeDef,
         "AdminPrivacy": bool,
         "RegistrantPrivacy": bool,
         "TechPrivacy": bool,
         "RegistrarName": str,
         "WhoIsServer": str,
         "RegistrarUrl": str,
         "AbuseContactEmail": str,
@@ -974,15 +952,14 @@
         "DnsSec": str,
         "StatusList": List[str],
         "DnssecKeys": List[DnssecKeyTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ContactDetailUnionTypeDef = Union[ContactDetailTypeDef, ContactDetailOutputTypeDef]
 _RequiredRegisterDomainRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
         "RegistrantContact": ContactDetailTypeDef,
@@ -1002,88 +979,67 @@
 )
 
 class RegisterDomainRequestRequestTypeDef(
     _RequiredRegisterDomainRequestRequestTypeDef, _OptionalRegisterDomainRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainContactRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainContactRequestRequestTypeDef",
-    {
-        "AdminContact": ContactDetailTypeDef,
-        "RegistrantContact": ContactDetailTypeDef,
-        "TechContact": ContactDetailTypeDef,
-        "Consent": ConsentTypeDef,
-    },
-    total=False,
-)
-
-class UpdateDomainContactRequestRequestTypeDef(
-    _RequiredUpdateDomainContactRequestRequestTypeDef,
-    _OptionalUpdateDomainContactRequestRequestTypeDef,
-):
-    pass
-
-ListPricesResponseTypeDef = TypedDict(
-    "ListPricesResponseTypeDef",
-    {
-        "Prices": List[DomainPriceTypeDef],
-        "NextPageMarker": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 _RequiredTransferDomainRequestRequestTypeDef = TypedDict(
     "_RequiredTransferDomainRequestRequestTypeDef",
     {
         "DomainName": str,
         "DurationInYears": int,
         "AdminContact": ContactDetailTypeDef,
         "RegistrantContact": ContactDetailTypeDef,
         "TechContact": ContactDetailTypeDef,
     },
 )
 _OptionalTransferDomainRequestRequestTypeDef = TypedDict(
     "_OptionalTransferDomainRequestRequestTypeDef",
     {
         "IdnLangCode": str,
-        "Nameservers": Sequence[NameserverUnionTypeDef],
+        "Nameservers": Sequence[NameserverTypeDef],
         "AuthCode": str,
         "AutoRenew": bool,
         "PrivacyProtectAdminContact": bool,
         "PrivacyProtectRegistrantContact": bool,
         "PrivacyProtectTechContact": bool,
     },
     total=False,
 )
 
 class TransferDomainRequestRequestTypeDef(
     _RequiredTransferDomainRequestRequestTypeDef, _OptionalTransferDomainRequestRequestTypeDef
 ):
     pass
 
-_RequiredUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameserversRequestRequestTypeDef",
+_RequiredUpdateDomainContactRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainContactRequestRequestTypeDef",
     {
         "DomainName": str,
-        "Nameservers": Sequence[NameserverUnionTypeDef],
     },
 )
-_OptionalUpdateDomainNameserversRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameserversRequestRequestTypeDef",
+_OptionalUpdateDomainContactRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainContactRequestRequestTypeDef",
     {
-        "FIAuthKey": str,
+        "AdminContact": ContactDetailTypeDef,
+        "RegistrantContact": ContactDetailTypeDef,
+        "TechContact": ContactDetailTypeDef,
+        "Consent": ConsentTypeDef,
     },
     total=False,
 )
 
-class UpdateDomainNameserversRequestRequestTypeDef(
-    _RequiredUpdateDomainNameserversRequestRequestTypeDef,
-    _OptionalUpdateDomainNameserversRequestRequestTypeDef,
+class UpdateDomainContactRequestRequestTypeDef(
+    _RequiredUpdateDomainContactRequestRequestTypeDef,
+    _OptionalUpdateDomainContactRequestRequestTypeDef,
 ):
     pass
+
+ListPricesResponseTypeDef = TypedDict(
+    "ListPricesResponseTypeDef",
+    {
+        "Prices": List[DomainPriceTypeDef],
+        "NextPageMarker": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-route53domains-2.5.2.post1/types_aiobotocore_route53domains.egg-info/SOURCES.txt` & `types-aiobotocore-route53domains-2.5.2.post2/types_aiobotocore_route53domains.egg-info/SOURCES.txt`

 * *Files identical despite different names*

