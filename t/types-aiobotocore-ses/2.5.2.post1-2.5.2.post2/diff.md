# Comparing `tmp/types-aiobotocore-ses-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-ses-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ses-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:01 2023, max compression
+gzip compressed data, was "types-aiobotocore-ses-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
```

## Comparing `types-aiobotocore-ses-2.5.2.post1.tar` & `types-aiobotocore-ses-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.109457 types-aiobotocore-ses-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-02 14:53:01.101457 types-aiobotocore-ses-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19536 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:01.109457 types-aiobotocore-ses-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.101457 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52089 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52003 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    49787 2023-08-02 14:49:42.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    49720 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:40.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-08-02 14:49:41.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:01.101457 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21038 2023-08-02 14:53:00.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:53:00.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:00.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:00.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:00.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:00.000000 types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.626643 types-aiobotocore-ses-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14033 2023-08-04 13:59:26.626643 types-aiobotocore-ses-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12531 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.626643 types-aiobotocore-ses-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2020 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.626643 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1797 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1796 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      916 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    52059 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    51973 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10983 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10981 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6591 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6584 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    48024 2023-08-04 13:53:32.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    47961 2023-08-04 13:53:32.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:30.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/version.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1521 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/waiter.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1520 2023-08-04 13:53:31.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/waiter.pyi
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.626643 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14033 2023-08-04 13:59:26.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      802 2023-08-04 13:59:26.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       22 2023-08-04 13:59:26.000000 types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ses-2.5.2.post1/LICENSE` & `types-aiobotocore-ses-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post1/setup.py` & `types-aiobotocore-ses-2.5.2.post2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ses",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_ses"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SES 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/__init__.py` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/__init__.pyi` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/__main__.py` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SES 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
-        " 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.SES 2.5.2\nVersion:         2.5.2.post2\nBuilder version:"
+        " 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES\nOther"
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

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/client.py` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     DeliveryOptionsTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventDestinationUnionTypeDef,
+    EventDestinationTypeDef,
     GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityPoliciesResponseTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
@@ -64,15 +64,15 @@
     ListTemplatesResponseTypeDef,
     ListVerifiedEmailAddressesResponseTypeDef,
     MessageDsnTypeDef,
     MessageTagTypeDef,
     MessageTypeDef,
     RawMessageTypeDef,
     ReceiptFilterTypeDef,
-    ReceiptRuleUnionTypeDef,
+    ReceiptRuleTypeDef,
     SendBounceResponseTypeDef,
     SendBulkTemplatedEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendRawEmailResponseTypeDef,
     SendTemplatedEmailResponseTypeDef,
     TemplateTypeDef,
@@ -188,15 +188,15 @@
         Creates a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_configuration_set)
         """
 
     async def create_configuration_set_event_destination(
-        self, *, ConfigurationSetName: str, EventDestination: EventDestinationUnionTypeDef
+        self, *, ConfigurationSetName: str, EventDestination: EventDestinationTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a configuration set event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_configuration_set_event_destination)
         """
@@ -234,15 +234,15 @@
         Creates a new IP address filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_receipt_filter)
         """
 
     async def create_receipt_rule(
-        self, *, RuleSetName: str, Rule: ReceiptRuleUnionTypeDef, After: str = ...
+        self, *, RuleSetName: str, Rule: ReceiptRuleTypeDef, After: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_receipt_rule)
         """
@@ -840,15 +840,15 @@
         current AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_account_sending_enabled)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_account_sending_enabled)
         """
 
     async def update_configuration_set_event_destination(
-        self, *, ConfigurationSetName: str, EventDestination: EventDestinationUnionTypeDef
+        self, *, ConfigurationSetName: str, EventDestination: EventDestinationTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the event destination of a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_configuration_set_event_destination)
         """
@@ -900,15 +900,15 @@
         Updates an existing custom verification email template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_custom_verification_email_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_custom_verification_email_template)
         """
 
     async def update_receipt_rule(
-        self, *, RuleSetName: str, Rule: ReceiptRuleUnionTypeDef
+        self, *, RuleSetName: str, Rule: ReceiptRuleTypeDef
     ) -> Dict[str, Any]:
         """
         Updates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_receipt_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_receipt_rule)
         """
```

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/client.pyi` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     DeliveryOptionsTypeDef,
     DescribeActiveReceiptRuleSetResponseTypeDef,
     DescribeConfigurationSetResponseTypeDef,
     DescribeReceiptRuleResponseTypeDef,
     DescribeReceiptRuleSetResponseTypeDef,
     DestinationTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventDestinationUnionTypeDef,
+    EventDestinationTypeDef,
     GetAccountSendingEnabledResponseTypeDef,
     GetCustomVerificationEmailTemplateResponseTypeDef,
     GetIdentityDkimAttributesResponseTypeDef,
     GetIdentityMailFromDomainAttributesResponseTypeDef,
     GetIdentityNotificationAttributesResponseTypeDef,
     GetIdentityPoliciesResponseTypeDef,
     GetIdentityVerificationAttributesResponseTypeDef,
@@ -64,15 +64,15 @@
     ListTemplatesResponseTypeDef,
     ListVerifiedEmailAddressesResponseTypeDef,
     MessageDsnTypeDef,
     MessageTagTypeDef,
     MessageTypeDef,
     RawMessageTypeDef,
     ReceiptFilterTypeDef,
-    ReceiptRuleUnionTypeDef,
+    ReceiptRuleTypeDef,
     SendBounceResponseTypeDef,
     SendBulkTemplatedEmailResponseTypeDef,
     SendCustomVerificationEmailResponseTypeDef,
     SendEmailResponseTypeDef,
     SendRawEmailResponseTypeDef,
     SendTemplatedEmailResponseTypeDef,
     TemplateTypeDef,
@@ -179,15 +179,15 @@
         """
         Creates a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_configuration_set)
         """
     async def create_configuration_set_event_destination(
-        self, *, ConfigurationSetName: str, EventDestination: EventDestinationUnionTypeDef
+        self, *, ConfigurationSetName: str, EventDestination: EventDestinationTypeDef
     ) -> Dict[str, Any]:
         """
         Creates a configuration set event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_configuration_set_event_destination)
         """
@@ -221,15 +221,15 @@
         """
         Creates a new IP address filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_receipt_filter)
         """
     async def create_receipt_rule(
-        self, *, RuleSetName: str, Rule: ReceiptRuleUnionTypeDef, After: str = ...
+        self, *, RuleSetName: str, Rule: ReceiptRuleTypeDef, After: str = ...
     ) -> Dict[str, Any]:
         """
         Creates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.create_receipt_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#create_receipt_rule)
         """
@@ -772,15 +772,15 @@
         Enables or disables email sending across your entire Amazon SES account in the
         current AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_account_sending_enabled)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_account_sending_enabled)
         """
     async def update_configuration_set_event_destination(
-        self, *, ConfigurationSetName: str, EventDestination: EventDestinationUnionTypeDef
+        self, *, ConfigurationSetName: str, EventDestination: EventDestinationTypeDef
     ) -> Dict[str, Any]:
         """
         Updates the event destination of a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_configuration_set_event_destination)
         """
@@ -827,15 +827,15 @@
         """
         Updates an existing custom verification email template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_custom_verification_email_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_custom_verification_email_template)
         """
     async def update_receipt_rule(
-        self, *, RuleSetName: str, Rule: ReceiptRuleUnionTypeDef
+        self, *, RuleSetName: str, Rule: ReceiptRuleTypeDef
     ) -> Dict[str, Any]:
         """
         Updates a receipt rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ses.html#SES.Client.update_receipt_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ses/client/#update_receipt_rule)
         """
```

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/literals.py` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
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
@@ -216,14 +217,15 @@
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
@@ -302,26 +304,28 @@
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

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/literals.pyi` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,15 @@
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
@@ -214,14 +215,15 @@
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
@@ -300,26 +302,28 @@
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

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/paginator.py` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/paginator.pyi` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/type_defs.py` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AddHeaderActionTypeDef",
     "BlobTypeDef",
     "ContentTypeDef",
     "BounceActionTypeDef",
     "BulkEmailDestinationStatusTypeDef",
     "DestinationTypeDef",
@@ -129,15 +128,14 @@
     "VerifyDomainIdentityRequestRequestTypeDef",
     "VerifyEmailAddressRequestRequestTypeDef",
     "VerifyEmailIdentityRequestRequestTypeDef",
     "RawMessageTypeDef",
     "BodyTypeDef",
     "BulkEmailDestinationTypeDef",
     "SendTemplatedEmailRequestRequestTypeDef",
-    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
@@ -177,32 +175,28 @@
     "MessageDsnTypeDef",
     "RecipientDsnFieldsTypeDef",
     "ReceiptActionTypeDef",
     "ReceiptFilterTypeDef",
     "SendRawEmailRequestRequestTypeDef",
     "MessageTypeDef",
     "SendBulkTemplatedEmailRequestRequestTypeDef",
-    "EventDestinationOutputTypeDef",
     "EventDestinationTypeDef",
     "BouncedRecipientInfoTypeDef",
-    "ReceiptRuleOutputTypeDef",
     "ReceiptRuleTypeDef",
     "CreateReceiptFilterRequestRequestTypeDef",
     "ListReceiptFiltersResponseTypeDef",
     "SendEmailRequestRequestTypeDef",
-    "DescribeConfigurationSetResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "EventDestinationUnionTypeDef",
+    "DescribeConfigurationSetResponseTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "SendBounceRequestRequestTypeDef",
+    "CreateReceiptRuleRequestRequestTypeDef",
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     "DescribeReceiptRuleResponseTypeDef",
     "DescribeReceiptRuleSetResponseTypeDef",
-    "CreateReceiptRuleRequestRequestTypeDef",
-    "ReceiptRuleUnionTypeDef",
     "UpdateReceiptRuleRequestRequestTypeDef",
 )
 
 AddHeaderActionTypeDef = TypedDict(
     "AddHeaderActionTypeDef",
     {
         "HeaderName": str,
@@ -221,19 +215,17 @@
     "_OptionalContentTypeDef",
     {
         "Charset": str,
     },
     total=False,
 )
 
-
 class ContentTypeDef(_RequiredContentTypeDef, _OptionalContentTypeDef):
     pass
 
-
 _RequiredBounceActionTypeDef = TypedDict(
     "_RequiredBounceActionTypeDef",
     {
         "SmtpReplyCode": str,
         "Message": str,
         "Sender": str,
     },
@@ -243,19 +235,17 @@
     {
         "TopicArn": str,
         "StatusCode": str,
     },
     total=False,
 )
 
-
 class BounceActionTypeDef(_RequiredBounceActionTypeDef, _OptionalBounceActionTypeDef):
     pass
 
-
 BulkEmailDestinationStatusTypeDef = TypedDict(
     "BulkEmailDestinationStatusTypeDef",
     {
         "Status": BulkEmailStatusType,
         "Error": str,
         "MessageId": str,
     },
@@ -343,19 +333,17 @@
         "SubjectPart": str,
         "TextPart": str,
         "HtmlPart": str,
     },
     total=False,
 )
 
-
 class TemplateTypeDef(_RequiredTemplateTypeDef, _OptionalTemplateTypeDef):
     pass
 
-
 CustomVerificationEmailTemplateTypeDef = TypedDict(
     "CustomVerificationEmailTemplateTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "SuccessRedirectionURL": str,
@@ -482,22 +470,20 @@
     "_OptionalDescribeConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetAttributeNames": Sequence[ConfigurationSetAttributeType],
     },
     total=False,
 )
 
-
 class DescribeConfigurationSetRequestRequestTypeDef(
     _RequiredDescribeConfigurationSetRequestRequestTypeDef,
     _OptionalDescribeConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
-
 ReputationOptionsTypeDef = TypedDict(
     "ReputationOptionsTypeDef",
     {
         "SendingEnabled": bool,
         "ReputationMetricsEnabled": bool,
         "LastFreshStart": datetime,
     },
@@ -567,21 +553,19 @@
     "_OptionalIdentityDkimAttributesTypeDef",
     {
         "DkimTokens": List[str],
     },
     total=False,
 )
 
-
 class IdentityDkimAttributesTypeDef(
     _RequiredIdentityDkimAttributesTypeDef, _OptionalIdentityDkimAttributesTypeDef
 ):
     pass
 
-
 GetIdentityMailFromDomainAttributesRequestRequestTypeDef = TypedDict(
     "GetIdentityMailFromDomainAttributesRequestRequestTypeDef",
     {
         "Identities": Sequence[str],
     },
 )
 
@@ -616,21 +600,19 @@
         "HeadersInBounceNotificationsEnabled": bool,
         "HeadersInComplaintNotificationsEnabled": bool,
         "HeadersInDeliveryNotificationsEnabled": bool,
     },
     total=False,
 )
 
-
 class IdentityNotificationAttributesTypeDef(
     _RequiredIdentityNotificationAttributesTypeDef, _OptionalIdentityNotificationAttributesTypeDef
 ):
     pass
 
-
 GetIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "GetIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyNames": Sequence[str],
     },
 )
@@ -661,21 +643,19 @@
     "_OptionalIdentityVerificationAttributesTypeDef",
     {
         "VerificationToken": str,
     },
     total=False,
 )
 
-
 class IdentityVerificationAttributesTypeDef(
     _RequiredIdentityVerificationAttributesTypeDef, _OptionalIdentityVerificationAttributesTypeDef
 ):
     pass
 
-
 SendDataPointTypeDef = TypedDict(
     "SendDataPointTypeDef",
     {
         "Timestamp": datetime,
         "DeliveryAttempts": int,
         "Bounces": int,
         "Complaints": int,
@@ -702,19 +682,17 @@
     {
         "TopicArn": str,
         "InvocationType": InvocationTypeType,
     },
     total=False,
 )
 
-
 class LambdaActionTypeDef(_RequiredLambdaActionTypeDef, _OptionalLambdaActionTypeDef):
     pass
 
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -804,76 +782,68 @@
         "TopicArn": str,
         "ObjectKeyPrefix": str,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-
 class S3ActionTypeDef(_RequiredS3ActionTypeDef, _OptionalS3ActionTypeDef):
     pass
 
-
 _RequiredSNSActionTypeDef = TypedDict(
     "_RequiredSNSActionTypeDef",
     {
         "TopicArn": str,
     },
 )
 _OptionalSNSActionTypeDef = TypedDict(
     "_OptionalSNSActionTypeDef",
     {
         "Encoding": SNSActionEncodingType,
     },
     total=False,
 )
 
-
 class SNSActionTypeDef(_RequiredSNSActionTypeDef, _OptionalSNSActionTypeDef):
     pass
 
-
 _RequiredStopActionTypeDef = TypedDict(
     "_RequiredStopActionTypeDef",
     {
         "Scope": Literal["RuleSet"],
     },
 )
 _OptionalStopActionTypeDef = TypedDict(
     "_OptionalStopActionTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
-
 class StopActionTypeDef(_RequiredStopActionTypeDef, _OptionalStopActionTypeDef):
     pass
 
-
 _RequiredWorkmailActionTypeDef = TypedDict(
     "_RequiredWorkmailActionTypeDef",
     {
         "OrganizationArn": str,
     },
 )
 _OptionalWorkmailActionTypeDef = TypedDict(
     "_OptionalWorkmailActionTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
-
 class WorkmailActionTypeDef(_RequiredWorkmailActionTypeDef, _OptionalWorkmailActionTypeDef):
     pass
 
-
 ReceiptIpFilterTypeDef = TypedDict(
     "ReceiptIpFilterTypeDef",
     {
         "Policy": ReceiptFilterPolicyType,
         "Cidr": str,
     },
 )
@@ -897,22 +867,20 @@
     "_OptionalSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class SendCustomVerificationEmailRequestRequestTypeDef(
     _RequiredSendCustomVerificationEmailRequestRequestTypeDef,
     _OptionalSendCustomVerificationEmailRequestRequestTypeDef,
 ):
     pass
 
-
 SetActiveReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
     total=False,
 )
@@ -953,22 +921,20 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMXFailure": BehaviorOnMXFailureType,
     },
     total=False,
 )
 
-
 class SetIdentityMailFromDomainRequestRequestTypeDef(
     _RequiredSetIdentityMailFromDomainRequestRequestTypeDef,
     _OptionalSetIdentityMailFromDomainRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSetIdentityNotificationTopicRequestRequestTypeDef = TypedDict(
     "_RequiredSetIdentityNotificationTopicRequestRequestTypeDef",
     {
         "Identity": str,
         "NotificationType": NotificationTypeType,
     },
 )
@@ -976,22 +942,20 @@
     "_OptionalSetIdentityNotificationTopicRequestRequestTypeDef",
     {
         "SnsTopic": str,
     },
     total=False,
 )
 
-
 class SetIdentityNotificationTopicRequestRequestTypeDef(
     _RequiredSetIdentityNotificationTopicRequestRequestTypeDef,
     _OptionalSetIdentityNotificationTopicRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSetReceiptRulePositionRequestRequestTypeDef = TypedDict(
     "_RequiredSetReceiptRulePositionRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleName": str,
     },
 )
@@ -999,22 +963,20 @@
     "_OptionalSetReceiptRulePositionRequestRequestTypeDef",
     {
         "After": str,
     },
     total=False,
 )
 
-
 class SetReceiptRulePositionRequestRequestTypeDef(
     _RequiredSetReceiptRulePositionRequestRequestTypeDef,
     _OptionalSetReceiptRulePositionRequestRequestTypeDef,
 ):
     pass
 
-
 TestRenderTemplateRequestRequestTypeDef = TypedDict(
     "TestRenderTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
@@ -1057,22 +1019,20 @@
         "TemplateContent": str,
         "SuccessRedirectionURL": str,
         "FailureRedirectionURL": str,
     },
     total=False,
 )
 
-
 class UpdateCustomVerificationEmailTemplateRequestRequestTypeDef(
     _RequiredUpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     _OptionalUpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
-
 VerifyDomainDkimRequestRequestTypeDef = TypedDict(
     "VerifyDomainDkimRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
@@ -1124,21 +1084,19 @@
     {
         "ReplacementTags": Sequence[MessageTagTypeDef],
         "ReplacementTemplateData": str,
     },
     total=False,
 )
 
-
 class BulkEmailDestinationTypeDef(
     _RequiredBulkEmailDestinationTypeDef, _OptionalBulkEmailDestinationTypeDef
 ):
     pass
 
-
 _RequiredSendTemplatedEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendTemplatedEmailRequestRequestTypeDef",
     {
         "Source": str,
         "Destination": DestinationTypeDef,
         "Template": str,
         "TemplateData": str,
@@ -1154,29 +1112,20 @@
         "Tags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
         "TemplateArn": str,
     },
     total=False,
 )
 
-
 class SendTemplatedEmailRequestRequestTypeDef(
     _RequiredSendTemplatedEmailRequestRequestTypeDef,
     _OptionalSendTemplatedEmailRequestRequestTypeDef,
 ):
     pass
 
-
-CloudWatchDestinationOutputTypeDef = TypedDict(
-    "CloudWatchDestinationOutputTypeDef",
-    {
-        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
-    },
-)
-
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
     },
 )
 
@@ -1227,22 +1176,20 @@
     "_OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     {
         "DeliveryOptions": DeliveryOptionsTypeDef,
     },
     total=False,
 )
 
-
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1451,22 +1398,20 @@
     "_OptionalGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef(
     _RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     _OptionalGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
 ):
     pass
 
-
 GetIdentityVerificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityVerificationAttributesResponseTypeDef",
     {
         "VerificationAttributes": Dict[str, IdentityVerificationAttributesTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1540,19 +1485,17 @@
     {
         "ArrivalDate": TimestampTypeDef,
         "ExtensionFields": Sequence[ExtensionFieldTypeDef],
     },
     total=False,
 )
 
-
 class MessageDsnTypeDef(_RequiredMessageDsnTypeDef, _OptionalMessageDsnTypeDef):
     pass
 
-
 _RequiredRecipientDsnFieldsTypeDef = TypedDict(
     "_RequiredRecipientDsnFieldsTypeDef",
     {
         "Action": DsnActionType,
         "Status": str,
     },
 )
@@ -1564,21 +1507,19 @@
         "DiagnosticCode": str,
         "LastAttemptDate": TimestampTypeDef,
         "ExtensionFields": Sequence[ExtensionFieldTypeDef],
     },
     total=False,
 )
 
-
 class RecipientDsnFieldsTypeDef(
     _RequiredRecipientDsnFieldsTypeDef, _OptionalRecipientDsnFieldsTypeDef
 ):
     pass
 
-
 ReceiptActionTypeDef = TypedDict(
     "ReceiptActionTypeDef",
     {
         "S3Action": S3ActionTypeDef,
         "BounceAction": BounceActionTypeDef,
         "WorkmailAction": WorkmailActionTypeDef,
         "LambdaAction": LambdaActionTypeDef,
@@ -1613,21 +1554,19 @@
         "ReturnPathArn": str,
         "Tags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class SendRawEmailRequestRequestTypeDef(
     _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
 ):
     pass
 
-
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
@@ -1651,47 +1590,20 @@
         "DefaultTags": Sequence[MessageTagTypeDef],
         "TemplateArn": str,
         "DefaultTemplateData": str,
     },
     total=False,
 )
 
-
 class SendBulkTemplatedEmailRequestRequestTypeDef(
     _RequiredSendBulkTemplatedEmailRequestRequestTypeDef,
     _OptionalSendBulkTemplatedEmailRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredEventDestinationOutputTypeDef = TypedDict(
-    "_RequiredEventDestinationOutputTypeDef",
-    {
-        "Name": str,
-        "MatchingEventTypes": List[EventTypeType],
-    },
-)
-_OptionalEventDestinationOutputTypeDef = TypedDict(
-    "_OptionalEventDestinationOutputTypeDef",
-    {
-        "Enabled": bool,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
-        "SNSDestination": SNSDestinationTypeDef,
-    },
-    total=False,
-)
-
-
-class EventDestinationOutputTypeDef(
-    _RequiredEventDestinationOutputTypeDef, _OptionalEventDestinationOutputTypeDef
-):
-    pass
-
-
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": Sequence[EventTypeType],
     },
 )
@@ -1702,19 +1614,17 @@
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationTypeDef,
         "SNSDestination": SNSDestinationTypeDef,
     },
     total=False,
 )
 
-
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
-
 _RequiredBouncedRecipientInfoTypeDef = TypedDict(
     "_RequiredBouncedRecipientInfoTypeDef",
     {
         "Recipient": str,
     },
 )
 _OptionalBouncedRecipientInfoTypeDef = TypedDict(
@@ -1723,46 +1633,19 @@
         "RecipientArn": str,
         "BounceType": BounceTypeType,
         "RecipientDsnFields": RecipientDsnFieldsTypeDef,
     },
     total=False,
 )
 
-
 class BouncedRecipientInfoTypeDef(
     _RequiredBouncedRecipientInfoTypeDef, _OptionalBouncedRecipientInfoTypeDef
 ):
     pass
 
-
-_RequiredReceiptRuleOutputTypeDef = TypedDict(
-    "_RequiredReceiptRuleOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalReceiptRuleOutputTypeDef = TypedDict(
-    "_OptionalReceiptRuleOutputTypeDef",
-    {
-        "Enabled": bool,
-        "TlsPolicy": TlsPolicyType,
-        "Recipients": List[str],
-        "Actions": List[ReceiptActionTypeDef],
-        "ScanEnabled": bool,
-    },
-    total=False,
-)
-
-
-class ReceiptRuleOutputTypeDef(
-    _RequiredReceiptRuleOutputTypeDef, _OptionalReceiptRuleOutputTypeDef
-):
-    pass
-
-
 _RequiredReceiptRuleTypeDef = TypedDict(
     "_RequiredReceiptRuleTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalReceiptRuleTypeDef = TypedDict(
@@ -1773,19 +1656,17 @@
         "Recipients": Sequence[str],
         "Actions": Sequence[ReceiptActionTypeDef],
         "ScanEnabled": bool,
     },
     total=False,
 )
 
-
 class ReceiptRuleTypeDef(_RequiredReceiptRuleTypeDef, _OptionalReceiptRuleTypeDef):
     pass
 
-
 CreateReceiptFilterRequestRequestTypeDef = TypedDict(
     "CreateReceiptFilterRequestRequestTypeDef",
     {
         "Filter": ReceiptFilterTypeDef,
     },
 )
 
@@ -1814,42 +1695,39 @@
         "ReturnPathArn": str,
         "Tags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
 
+CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
+    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
+    {
+        "ConfigurationSetName": str,
+        "EventDestination": EventDestinationTypeDef,
+    },
+)
 
 DescribeConfigurationSetResponseTypeDef = TypedDict(
     "DescribeConfigurationSetResponseTypeDef",
     {
         "ConfigurationSet": ConfigurationSetTypeDef,
-        "EventDestinations": List[EventDestinationOutputTypeDef],
+        "EventDestinations": List[EventDestinationTypeDef],
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
-    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
-    {
-        "ConfigurationSetName": str,
-        "EventDestination": EventDestinationTypeDef,
-    },
-)
-
-EventDestinationUnionTypeDef = Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
 UpdateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
     },
 )
@@ -1868,70 +1746,65 @@
         "Explanation": str,
         "MessageDsn": MessageDsnTypeDef,
         "BounceSenderArn": str,
     },
     total=False,
 )
 
-
 class SendBounceRequestRequestTypeDef(
     _RequiredSendBounceRequestRequestTypeDef, _OptionalSendBounceRequestRequestTypeDef
 ):
     pass
 
+_RequiredCreateReceiptRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReceiptRuleRequestRequestTypeDef",
+    {
+        "RuleSetName": str,
+        "Rule": ReceiptRuleTypeDef,
+    },
+)
+_OptionalCreateReceiptRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReceiptRuleRequestRequestTypeDef",
+    {
+        "After": str,
+    },
+    total=False,
+)
+
+class CreateReceiptRuleRequestRequestTypeDef(
+    _RequiredCreateReceiptRuleRequestRequestTypeDef, _OptionalCreateReceiptRuleRequestRequestTypeDef
+):
+    pass
 
 DescribeActiveReceiptRuleSetResponseTypeDef = TypedDict(
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     {
         "Metadata": ReceiptRuleSetMetadataTypeDef,
-        "Rules": List[ReceiptRuleOutputTypeDef],
+        "Rules": List[ReceiptRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReceiptRuleResponseTypeDef = TypedDict(
     "DescribeReceiptRuleResponseTypeDef",
     {
-        "Rule": ReceiptRuleOutputTypeDef,
+        "Rule": ReceiptRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReceiptRuleSetResponseTypeDef = TypedDict(
     "DescribeReceiptRuleSetResponseTypeDef",
     {
         "Metadata": ReceiptRuleSetMetadataTypeDef,
-        "Rules": List[ReceiptRuleOutputTypeDef],
+        "Rules": List[ReceiptRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateReceiptRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReceiptRuleRequestRequestTypeDef",
-    {
-        "RuleSetName": str,
-        "Rule": ReceiptRuleTypeDef,
-    },
-)
-_OptionalCreateReceiptRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReceiptRuleRequestRequestTypeDef",
-    {
-        "After": str,
-    },
-    total=False,
-)
-
-
-class CreateReceiptRuleRequestRequestTypeDef(
-    _RequiredCreateReceiptRuleRequestRequestTypeDef, _OptionalCreateReceiptRuleRequestRequestTypeDef
-):
-    pass
-
-
-ReceiptRuleUnionTypeDef = Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef]
 UpdateReceiptRuleRequestRequestTypeDef = TypedDict(
     "UpdateReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "Rule": ReceiptRuleTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/type_defs.pyi` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AddHeaderActionTypeDef",
     "BlobTypeDef",
     "ContentTypeDef",
     "BounceActionTypeDef",
     "BulkEmailDestinationStatusTypeDef",
     "DestinationTypeDef",
@@ -128,15 +129,14 @@
     "VerifyDomainIdentityRequestRequestTypeDef",
     "VerifyEmailAddressRequestRequestTypeDef",
     "VerifyEmailIdentityRequestRequestTypeDef",
     "RawMessageTypeDef",
     "BodyTypeDef",
     "BulkEmailDestinationTypeDef",
     "SendTemplatedEmailRequestRequestTypeDef",
-    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateConfigurationSetRequestRequestTypeDef",
     "CreateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "UpdateConfigurationSetTrackingOptionsRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "PutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
@@ -176,32 +176,28 @@
     "MessageDsnTypeDef",
     "RecipientDsnFieldsTypeDef",
     "ReceiptActionTypeDef",
     "ReceiptFilterTypeDef",
     "SendRawEmailRequestRequestTypeDef",
     "MessageTypeDef",
     "SendBulkTemplatedEmailRequestRequestTypeDef",
-    "EventDestinationOutputTypeDef",
     "EventDestinationTypeDef",
     "BouncedRecipientInfoTypeDef",
-    "ReceiptRuleOutputTypeDef",
     "ReceiptRuleTypeDef",
     "CreateReceiptFilterRequestRequestTypeDef",
     "ListReceiptFiltersResponseTypeDef",
     "SendEmailRequestRequestTypeDef",
-    "DescribeConfigurationSetResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "EventDestinationUnionTypeDef",
+    "DescribeConfigurationSetResponseTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     "SendBounceRequestRequestTypeDef",
+    "CreateReceiptRuleRequestRequestTypeDef",
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     "DescribeReceiptRuleResponseTypeDef",
     "DescribeReceiptRuleSetResponseTypeDef",
-    "CreateReceiptRuleRequestRequestTypeDef",
-    "ReceiptRuleUnionTypeDef",
     "UpdateReceiptRuleRequestRequestTypeDef",
 )
 
 AddHeaderActionTypeDef = TypedDict(
     "AddHeaderActionTypeDef",
     {
         "HeaderName": str,
@@ -220,17 +216,19 @@
     "_OptionalContentTypeDef",
     {
         "Charset": str,
     },
     total=False,
 )
 
+
 class ContentTypeDef(_RequiredContentTypeDef, _OptionalContentTypeDef):
     pass
 
+
 _RequiredBounceActionTypeDef = TypedDict(
     "_RequiredBounceActionTypeDef",
     {
         "SmtpReplyCode": str,
         "Message": str,
         "Sender": str,
     },
@@ -240,17 +238,19 @@
     {
         "TopicArn": str,
         "StatusCode": str,
     },
     total=False,
 )
 
+
 class BounceActionTypeDef(_RequiredBounceActionTypeDef, _OptionalBounceActionTypeDef):
     pass
 
+
 BulkEmailDestinationStatusTypeDef = TypedDict(
     "BulkEmailDestinationStatusTypeDef",
     {
         "Status": BulkEmailStatusType,
         "Error": str,
         "MessageId": str,
     },
@@ -338,17 +338,19 @@
         "SubjectPart": str,
         "TextPart": str,
         "HtmlPart": str,
     },
     total=False,
 )
 
+
 class TemplateTypeDef(_RequiredTemplateTypeDef, _OptionalTemplateTypeDef):
     pass
 
+
 CustomVerificationEmailTemplateTypeDef = TypedDict(
     "CustomVerificationEmailTemplateTypeDef",
     {
         "TemplateName": str,
         "FromEmailAddress": str,
         "TemplateSubject": str,
         "SuccessRedirectionURL": str,
@@ -475,20 +477,22 @@
     "_OptionalDescribeConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetAttributeNames": Sequence[ConfigurationSetAttributeType],
     },
     total=False,
 )
 
+
 class DescribeConfigurationSetRequestRequestTypeDef(
     _RequiredDescribeConfigurationSetRequestRequestTypeDef,
     _OptionalDescribeConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
+
 ReputationOptionsTypeDef = TypedDict(
     "ReputationOptionsTypeDef",
     {
         "SendingEnabled": bool,
         "ReputationMetricsEnabled": bool,
         "LastFreshStart": datetime,
     },
@@ -558,19 +562,21 @@
     "_OptionalIdentityDkimAttributesTypeDef",
     {
         "DkimTokens": List[str],
     },
     total=False,
 )
 
+
 class IdentityDkimAttributesTypeDef(
     _RequiredIdentityDkimAttributesTypeDef, _OptionalIdentityDkimAttributesTypeDef
 ):
     pass
 
+
 GetIdentityMailFromDomainAttributesRequestRequestTypeDef = TypedDict(
     "GetIdentityMailFromDomainAttributesRequestRequestTypeDef",
     {
         "Identities": Sequence[str],
     },
 )
 
@@ -605,19 +611,21 @@
         "HeadersInBounceNotificationsEnabled": bool,
         "HeadersInComplaintNotificationsEnabled": bool,
         "HeadersInDeliveryNotificationsEnabled": bool,
     },
     total=False,
 )
 
+
 class IdentityNotificationAttributesTypeDef(
     _RequiredIdentityNotificationAttributesTypeDef, _OptionalIdentityNotificationAttributesTypeDef
 ):
     pass
 
+
 GetIdentityPoliciesRequestRequestTypeDef = TypedDict(
     "GetIdentityPoliciesRequestRequestTypeDef",
     {
         "Identity": str,
         "PolicyNames": Sequence[str],
     },
 )
@@ -648,19 +656,21 @@
     "_OptionalIdentityVerificationAttributesTypeDef",
     {
         "VerificationToken": str,
     },
     total=False,
 )
 
+
 class IdentityVerificationAttributesTypeDef(
     _RequiredIdentityVerificationAttributesTypeDef, _OptionalIdentityVerificationAttributesTypeDef
 ):
     pass
 
+
 SendDataPointTypeDef = TypedDict(
     "SendDataPointTypeDef",
     {
         "Timestamp": datetime,
         "DeliveryAttempts": int,
         "Bounces": int,
         "Complaints": int,
@@ -687,17 +697,19 @@
     {
         "TopicArn": str,
         "InvocationType": InvocationTypeType,
     },
     total=False,
 )
 
+
 class LambdaActionTypeDef(_RequiredLambdaActionTypeDef, _OptionalLambdaActionTypeDef):
     pass
 
+
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
     },
@@ -787,68 +799,76 @@
         "TopicArn": str,
         "ObjectKeyPrefix": str,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
+
 class S3ActionTypeDef(_RequiredS3ActionTypeDef, _OptionalS3ActionTypeDef):
     pass
 
+
 _RequiredSNSActionTypeDef = TypedDict(
     "_RequiredSNSActionTypeDef",
     {
         "TopicArn": str,
     },
 )
 _OptionalSNSActionTypeDef = TypedDict(
     "_OptionalSNSActionTypeDef",
     {
         "Encoding": SNSActionEncodingType,
     },
     total=False,
 )
 
+
 class SNSActionTypeDef(_RequiredSNSActionTypeDef, _OptionalSNSActionTypeDef):
     pass
 
+
 _RequiredStopActionTypeDef = TypedDict(
     "_RequiredStopActionTypeDef",
     {
         "Scope": Literal["RuleSet"],
     },
 )
 _OptionalStopActionTypeDef = TypedDict(
     "_OptionalStopActionTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
+
 class StopActionTypeDef(_RequiredStopActionTypeDef, _OptionalStopActionTypeDef):
     pass
 
+
 _RequiredWorkmailActionTypeDef = TypedDict(
     "_RequiredWorkmailActionTypeDef",
     {
         "OrganizationArn": str,
     },
 )
 _OptionalWorkmailActionTypeDef = TypedDict(
     "_OptionalWorkmailActionTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
+
 class WorkmailActionTypeDef(_RequiredWorkmailActionTypeDef, _OptionalWorkmailActionTypeDef):
     pass
 
+
 ReceiptIpFilterTypeDef = TypedDict(
     "ReceiptIpFilterTypeDef",
     {
         "Policy": ReceiptFilterPolicyType,
         "Cidr": str,
     },
 )
@@ -872,20 +892,22 @@
     "_OptionalSendCustomVerificationEmailRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class SendCustomVerificationEmailRequestRequestTypeDef(
     _RequiredSendCustomVerificationEmailRequestRequestTypeDef,
     _OptionalSendCustomVerificationEmailRequestRequestTypeDef,
 ):
     pass
 
+
 SetActiveReceiptRuleSetRequestRequestTypeDef = TypedDict(
     "SetActiveReceiptRuleSetRequestRequestTypeDef",
     {
         "RuleSetName": str,
     },
     total=False,
 )
@@ -926,20 +948,22 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMXFailure": BehaviorOnMXFailureType,
     },
     total=False,
 )
 
+
 class SetIdentityMailFromDomainRequestRequestTypeDef(
     _RequiredSetIdentityMailFromDomainRequestRequestTypeDef,
     _OptionalSetIdentityMailFromDomainRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSetIdentityNotificationTopicRequestRequestTypeDef = TypedDict(
     "_RequiredSetIdentityNotificationTopicRequestRequestTypeDef",
     {
         "Identity": str,
         "NotificationType": NotificationTypeType,
     },
 )
@@ -947,20 +971,22 @@
     "_OptionalSetIdentityNotificationTopicRequestRequestTypeDef",
     {
         "SnsTopic": str,
     },
     total=False,
 )
 
+
 class SetIdentityNotificationTopicRequestRequestTypeDef(
     _RequiredSetIdentityNotificationTopicRequestRequestTypeDef,
     _OptionalSetIdentityNotificationTopicRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSetReceiptRulePositionRequestRequestTypeDef = TypedDict(
     "_RequiredSetReceiptRulePositionRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "RuleName": str,
     },
 )
@@ -968,20 +994,22 @@
     "_OptionalSetReceiptRulePositionRequestRequestTypeDef",
     {
         "After": str,
     },
     total=False,
 )
 
+
 class SetReceiptRulePositionRequestRequestTypeDef(
     _RequiredSetReceiptRulePositionRequestRequestTypeDef,
     _OptionalSetReceiptRulePositionRequestRequestTypeDef,
 ):
     pass
 
+
 TestRenderTemplateRequestRequestTypeDef = TypedDict(
     "TestRenderTemplateRequestRequestTypeDef",
     {
         "TemplateName": str,
         "TemplateData": str,
     },
 )
@@ -1024,20 +1052,22 @@
         "TemplateContent": str,
         "SuccessRedirectionURL": str,
         "FailureRedirectionURL": str,
     },
     total=False,
 )
 
+
 class UpdateCustomVerificationEmailTemplateRequestRequestTypeDef(
     _RequiredUpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
     _OptionalUpdateCustomVerificationEmailTemplateRequestRequestTypeDef,
 ):
     pass
 
+
 VerifyDomainDkimRequestRequestTypeDef = TypedDict(
     "VerifyDomainDkimRequestRequestTypeDef",
     {
         "Domain": str,
     },
 )
 
@@ -1089,19 +1119,21 @@
     {
         "ReplacementTags": Sequence[MessageTagTypeDef],
         "ReplacementTemplateData": str,
     },
     total=False,
 )
 
+
 class BulkEmailDestinationTypeDef(
     _RequiredBulkEmailDestinationTypeDef, _OptionalBulkEmailDestinationTypeDef
 ):
     pass
 
+
 _RequiredSendTemplatedEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendTemplatedEmailRequestRequestTypeDef",
     {
         "Source": str,
         "Destination": DestinationTypeDef,
         "Template": str,
         "TemplateData": str,
@@ -1117,26 +1149,21 @@
         "Tags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
         "TemplateArn": str,
     },
     total=False,
 )
 
+
 class SendTemplatedEmailRequestRequestTypeDef(
     _RequiredSendTemplatedEmailRequestRequestTypeDef,
     _OptionalSendTemplatedEmailRequestRequestTypeDef,
 ):
     pass
 
-CloudWatchDestinationOutputTypeDef = TypedDict(
-    "CloudWatchDestinationOutputTypeDef",
-    {
-        "DimensionConfigurations": List[CloudWatchDimensionConfigurationTypeDef],
-    },
-)
 
 CloudWatchDestinationTypeDef = TypedDict(
     "CloudWatchDestinationTypeDef",
     {
         "DimensionConfigurations": Sequence[CloudWatchDimensionConfigurationTypeDef],
     },
 )
@@ -1188,20 +1215,22 @@
     "_OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef",
     {
         "DeliveryOptions": DeliveryOptionsTypeDef,
     },
     total=False,
 )
 
+
 class PutConfigurationSetDeliveryOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetDeliveryOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 EmptyResponseMetadataTypeDef = TypedDict(
     "EmptyResponseMetadataTypeDef",
     {
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
@@ -1410,20 +1439,22 @@
     "_OptionalGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef",
     {
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef(
     _RequiredGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
     _OptionalGetIdentityVerificationAttributesRequestIdentityExistsWaitTypeDef,
 ):
     pass
 
+
 GetIdentityVerificationAttributesResponseTypeDef = TypedDict(
     "GetIdentityVerificationAttributesResponseTypeDef",
     {
         "VerificationAttributes": Dict[str, IdentityVerificationAttributesTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -1497,17 +1528,19 @@
     {
         "ArrivalDate": TimestampTypeDef,
         "ExtensionFields": Sequence[ExtensionFieldTypeDef],
     },
     total=False,
 )
 
+
 class MessageDsnTypeDef(_RequiredMessageDsnTypeDef, _OptionalMessageDsnTypeDef):
     pass
 
+
 _RequiredRecipientDsnFieldsTypeDef = TypedDict(
     "_RequiredRecipientDsnFieldsTypeDef",
     {
         "Action": DsnActionType,
         "Status": str,
     },
 )
@@ -1519,19 +1552,21 @@
         "DiagnosticCode": str,
         "LastAttemptDate": TimestampTypeDef,
         "ExtensionFields": Sequence[ExtensionFieldTypeDef],
     },
     total=False,
 )
 
+
 class RecipientDsnFieldsTypeDef(
     _RequiredRecipientDsnFieldsTypeDef, _OptionalRecipientDsnFieldsTypeDef
 ):
     pass
 
+
 ReceiptActionTypeDef = TypedDict(
     "ReceiptActionTypeDef",
     {
         "S3Action": S3ActionTypeDef,
         "BounceAction": BounceActionTypeDef,
         "WorkmailAction": WorkmailActionTypeDef,
         "LambdaAction": LambdaActionTypeDef,
@@ -1566,19 +1601,21 @@
         "ReturnPathArn": str,
         "Tags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class SendRawEmailRequestRequestTypeDef(
     _RequiredSendRawEmailRequestRequestTypeDef, _OptionalSendRawEmailRequestRequestTypeDef
 ):
     pass
 
+
 MessageTypeDef = TypedDict(
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
@@ -1602,42 +1639,21 @@
         "DefaultTags": Sequence[MessageTagTypeDef],
         "TemplateArn": str,
         "DefaultTemplateData": str,
     },
     total=False,
 )
 
+
 class SendBulkTemplatedEmailRequestRequestTypeDef(
     _RequiredSendBulkTemplatedEmailRequestRequestTypeDef,
     _OptionalSendBulkTemplatedEmailRequestRequestTypeDef,
 ):
     pass
 
-_RequiredEventDestinationOutputTypeDef = TypedDict(
-    "_RequiredEventDestinationOutputTypeDef",
-    {
-        "Name": str,
-        "MatchingEventTypes": List[EventTypeType],
-    },
-)
-_OptionalEventDestinationOutputTypeDef = TypedDict(
-    "_OptionalEventDestinationOutputTypeDef",
-    {
-        "Enabled": bool,
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
-        "SNSDestination": SNSDestinationTypeDef,
-    },
-    total=False,
-)
-
-class EventDestinationOutputTypeDef(
-    _RequiredEventDestinationOutputTypeDef, _OptionalEventDestinationOutputTypeDef
-):
-    pass
 
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": Sequence[EventTypeType],
     },
@@ -1649,17 +1665,19 @@
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
         "CloudWatchDestination": CloudWatchDestinationTypeDef,
         "SNSDestination": SNSDestinationTypeDef,
     },
     total=False,
 )
 
+
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
+
 _RequiredBouncedRecipientInfoTypeDef = TypedDict(
     "_RequiredBouncedRecipientInfoTypeDef",
     {
         "Recipient": str,
     },
 )
 _OptionalBouncedRecipientInfoTypeDef = TypedDict(
@@ -1668,41 +1686,20 @@
         "RecipientArn": str,
         "BounceType": BounceTypeType,
         "RecipientDsnFields": RecipientDsnFieldsTypeDef,
     },
     total=False,
 )
 
+
 class BouncedRecipientInfoTypeDef(
     _RequiredBouncedRecipientInfoTypeDef, _OptionalBouncedRecipientInfoTypeDef
 ):
     pass
 
-_RequiredReceiptRuleOutputTypeDef = TypedDict(
-    "_RequiredReceiptRuleOutputTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalReceiptRuleOutputTypeDef = TypedDict(
-    "_OptionalReceiptRuleOutputTypeDef",
-    {
-        "Enabled": bool,
-        "TlsPolicy": TlsPolicyType,
-        "Recipients": List[str],
-        "Actions": List[ReceiptActionTypeDef],
-        "ScanEnabled": bool,
-    },
-    total=False,
-)
-
-class ReceiptRuleOutputTypeDef(
-    _RequiredReceiptRuleOutputTypeDef, _OptionalReceiptRuleOutputTypeDef
-):
-    pass
 
 _RequiredReceiptRuleTypeDef = TypedDict(
     "_RequiredReceiptRuleTypeDef",
     {
         "Name": str,
     },
 )
@@ -1714,17 +1711,19 @@
         "Recipients": Sequence[str],
         "Actions": Sequence[ReceiptActionTypeDef],
         "ScanEnabled": bool,
     },
     total=False,
 )
 
+
 class ReceiptRuleTypeDef(_RequiredReceiptRuleTypeDef, _OptionalReceiptRuleTypeDef):
     pass
 
+
 CreateReceiptFilterRequestRequestTypeDef = TypedDict(
     "CreateReceiptFilterRequestRequestTypeDef",
     {
         "Filter": ReceiptFilterTypeDef,
     },
 )
 
@@ -1753,40 +1752,41 @@
         "ReturnPathArn": str,
         "Tags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
 
+
+CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
+    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
+    {
+        "ConfigurationSetName": str,
+        "EventDestination": EventDestinationTypeDef,
+    },
+)
+
 DescribeConfigurationSetResponseTypeDef = TypedDict(
     "DescribeConfigurationSetResponseTypeDef",
     {
         "ConfigurationSet": ConfigurationSetTypeDef,
-        "EventDestinations": List[EventDestinationOutputTypeDef],
+        "EventDestinations": List[EventDestinationTypeDef],
         "TrackingOptions": TrackingOptionsTypeDef,
         "DeliveryOptions": DeliveryOptionsTypeDef,
         "ReputationOptions": ReputationOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
-    "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
-    {
-        "ConfigurationSetName": str,
-        "EventDestination": EventDestinationTypeDef,
-    },
-)
-
-EventDestinationUnionTypeDef = Union[EventDestinationTypeDef, EventDestinationOutputTypeDef]
 UpdateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestination": EventDestinationTypeDef,
     },
 )
@@ -1805,66 +1805,69 @@
         "Explanation": str,
         "MessageDsn": MessageDsnTypeDef,
         "BounceSenderArn": str,
     },
     total=False,
 )
 
+
 class SendBounceRequestRequestTypeDef(
     _RequiredSendBounceRequestRequestTypeDef, _OptionalSendBounceRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredCreateReceiptRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateReceiptRuleRequestRequestTypeDef",
+    {
+        "RuleSetName": str,
+        "Rule": ReceiptRuleTypeDef,
+    },
+)
+_OptionalCreateReceiptRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateReceiptRuleRequestRequestTypeDef",
+    {
+        "After": str,
+    },
+    total=False,
+)
+
+
+class CreateReceiptRuleRequestRequestTypeDef(
+    _RequiredCreateReceiptRuleRequestRequestTypeDef, _OptionalCreateReceiptRuleRequestRequestTypeDef
+):
+    pass
+
+
 DescribeActiveReceiptRuleSetResponseTypeDef = TypedDict(
     "DescribeActiveReceiptRuleSetResponseTypeDef",
     {
         "Metadata": ReceiptRuleSetMetadataTypeDef,
-        "Rules": List[ReceiptRuleOutputTypeDef],
+        "Rules": List[ReceiptRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReceiptRuleResponseTypeDef = TypedDict(
     "DescribeReceiptRuleResponseTypeDef",
     {
-        "Rule": ReceiptRuleOutputTypeDef,
+        "Rule": ReceiptRuleTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeReceiptRuleSetResponseTypeDef = TypedDict(
     "DescribeReceiptRuleSetResponseTypeDef",
     {
         "Metadata": ReceiptRuleSetMetadataTypeDef,
-        "Rules": List[ReceiptRuleOutputTypeDef],
+        "Rules": List[ReceiptRuleTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateReceiptRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateReceiptRuleRequestRequestTypeDef",
-    {
-        "RuleSetName": str,
-        "Rule": ReceiptRuleTypeDef,
-    },
-)
-_OptionalCreateReceiptRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateReceiptRuleRequestRequestTypeDef",
-    {
-        "After": str,
-    },
-    total=False,
-)
-
-class CreateReceiptRuleRequestRequestTypeDef(
-    _RequiredCreateReceiptRuleRequestRequestTypeDef, _OptionalCreateReceiptRuleRequestRequestTypeDef
-):
-    pass
-
-ReceiptRuleUnionTypeDef = Union[ReceiptRuleTypeDef, ReceiptRuleOutputTypeDef]
 UpdateReceiptRuleRequestRequestTypeDef = TypedDict(
     "UpdateReceiptRuleRequestRequestTypeDef",
     {
         "RuleSetName": str,
         "Rule": ReceiptRuleTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/waiter.py` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses/waiter.pyi` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ses-2.5.2.post1/types_aiobotocore_ses.egg-info/SOURCES.txt` & `types-aiobotocore-ses-2.5.2.post2/types_aiobotocore_ses.egg-info/SOURCES.txt`

 * *Files identical despite different names*

