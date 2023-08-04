# Comparing `tmp/types-aiobotocore-pinpoint-email-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-pinpoint-email-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-pinpoint-email-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:47 2023, max compression
+gzip compressed data, was "types-aiobotocore-pinpoint-email-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:21 2023, max compression
```

## Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1.tar` & `types-aiobotocore-pinpoint-email-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.989498 types-aiobotocore-pinpoint-email-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:56.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18984 2023-08-02 14:52:47.989498 types-aiobotocore-pinpoint-email-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17439 2023-08-02 14:44:56.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:47.989498 types-aiobotocore-pinpoint-email-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-08-02 14:44:56.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.981498 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-08-02 14:44:56.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-08-02 14:44:56.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:44:56.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35112 2023-08-02 14:44:57.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35056 2023-08-02 14:44:57.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-08-02 14:44:57.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9863 2023-08-02 14:44:57.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-08-02 14:44:57.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-08-02 14:44:57.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:56.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36484 2023-08-02 14:44:58.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36450 2023-08-02 14:44:57.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:56.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:47.989498 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18984 2023-08-02 14:52:47.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:47.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:47.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:47.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:47.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:47.000000 types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.136643 types-aiobotocore-pinpoint-email-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14046 2023-08-04 13:59:21.136643 types-aiobotocore-pinpoint-email-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12501 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:21.136643 types-aiobotocore-pinpoint-email-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2120 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.126643 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1700 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1699 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      969 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    35092 2023-08-04 13:46:55.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    35036 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9960 2023-08-04 13:46:55.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9958 2023-08-04 13:46:55.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6920 2023-08-04 13:46:55.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6913 2023-08-04 13:46:55.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    35045 2023-08-04 13:46:56.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    35011 2023-08-04 13:46:55.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:46:54.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:21.136643 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14046 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      946 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       33 2023-08-04 13:59:21.000000 types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/LICENSE` & `types-aiobotocore-pinpoint-email-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/setup.py` & `types-aiobotocore-pinpoint-email-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-pinpoint-email",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_pinpoint_email"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.PinpointEmail 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/__init__.py` & `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/__init__.pyi` & `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/__main__.py` & `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.PinpointEmail 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail\nOther"
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

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/client.py` & `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ListEmailIdentitiesPaginator,
 )
 from .type_defs import (
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
-    DomainDeliverabilityTrackingOptionUnionTypeDef,
+    DomainDeliverabilityTrackingOptionTypeDef,
     EmailContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
     GetDedicatedIpResponseTypeDef,
@@ -50,53 +50,49 @@
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
-    ReputationOptionsUnionTypeDef,
+    ReputationOptionsTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     TrackingOptionsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("PinpointEmailClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccountSuspendedException: Type[BotocoreClientError]
     AlreadyExistsException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConcurrentModificationException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     MailFromDomainNotVerifiedException: Type[BotocoreClientError]
     MessageRejected: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     SendingPausedException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
 
-
 class PinpointEmailClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/)
     """
 
     meta: ClientMeta
@@ -105,294 +101,267 @@
     def exceptions(self) -> Exceptions:
         """
         PinpointEmailClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#close)
         """
-
     async def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: ReputationOptionsUnionTypeDef = ...,
+        ReputationOptions: ReputationOptionsTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_configuration_set)
         """
-
     async def create_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
         EventDestination: EventDestinationDefinitionTypeDef
     ) -> Dict[str, Any]:
         """
         Create an event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_configuration_set_event_destination)
         """
-
     async def create_dedicated_ip_pool(
         self, *, PoolName: str, Tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Create a new pool of dedicated IP addresses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_dedicated_ip_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_dedicated_ip_pool)
         """
-
     async def create_deliverability_test_report(
         self,
         *,
         FromEmailAddress: str,
         Content: EmailContentTypeDef,
         ReportName: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDeliverabilityTestReportResponseTypeDef:
         """
         Create a new predictive inbox placement test.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_deliverability_test_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_deliverability_test_report)
         """
-
     async def create_email_identity(
         self, *, EmailIdentity: str, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateEmailIdentityResponseTypeDef:
         """
         Verifies an email identity for use with Amazon Pinpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_email_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_email_identity)
         """
-
     async def delete_configuration_set(self, *, ConfigurationSetName: str) -> Dict[str, Any]:
         """
         Delete an existing configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.delete_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#delete_configuration_set)
         """
-
     async def delete_configuration_set_event_destination(
         self, *, ConfigurationSetName: str, EventDestinationName: str
     ) -> Dict[str, Any]:
         """
         Delete an event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.delete_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#delete_configuration_set_event_destination)
         """
-
     async def delete_dedicated_ip_pool(self, *, PoolName: str) -> Dict[str, Any]:
         """
         Delete a dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.delete_dedicated_ip_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#delete_dedicated_ip_pool)
         """
-
     async def delete_email_identity(self, *, EmailIdentity: str) -> Dict[str, Any]:
         """
         Deletes an email identity that you previously verified for use with Amazon
         Pinpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.delete_email_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#delete_email_identity)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#generate_presigned_url)
         """
-
     async def get_account(self) -> GetAccountResponseTypeDef:
         """
         Obtain information about the email-sending status and capabilities of your
         Amazon Pinpoint account in the current AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_account)
         """
-
     async def get_blacklist_reports(
         self, *, BlacklistItemNames: Sequence[str]
     ) -> GetBlacklistReportsResponseTypeDef:
         """
         Retrieve a list of the blacklists that your dedicated IP addresses appear on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_blacklist_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_blacklist_reports)
         """
-
     async def get_configuration_set(
         self, *, ConfigurationSetName: str
     ) -> GetConfigurationSetResponseTypeDef:
         """
         Get information about an existing configuration set, including the dedicated IP
         pool that it's associated with, whether or not it's enabled for sending email,
         and more.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_configuration_set)
         """
-
     async def get_configuration_set_event_destinations(
         self, *, ConfigurationSetName: str
     ) -> GetConfigurationSetEventDestinationsResponseTypeDef:
         """
         Retrieve a list of event destinations that are associated with a configuration
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_configuration_set_event_destinations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_configuration_set_event_destinations)
         """
-
     async def get_dedicated_ip(self, *, Ip: str) -> GetDedicatedIpResponseTypeDef:
         """
         Get information about a dedicated IP address, including the name of the
         dedicated IP pool that it's associated with, as well information about the
         automatic warm-up process for the address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_dedicated_ip)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_dedicated_ip)
         """
-
     async def get_dedicated_ips(
         self, *, PoolName: str = ..., NextToken: str = ..., PageSize: int = ...
     ) -> GetDedicatedIpsResponseTypeDef:
         """
         List the dedicated IP addresses that are associated with your Amazon Pinpoint
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_dedicated_ips)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_dedicated_ips)
         """
-
     async def get_deliverability_dashboard_options(
         self,
     ) -> GetDeliverabilityDashboardOptionsResponseTypeDef:
         """
         Retrieve information about the status of the Deliverability dashboard for your
         Amazon Pinpoint account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_deliverability_dashboard_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_deliverability_dashboard_options)
         """
-
     async def get_deliverability_test_report(
         self, *, ReportId: str
     ) -> GetDeliverabilityTestReportResponseTypeDef:
         """
         Retrieve the results of a predictive inbox placement test.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_deliverability_test_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_deliverability_test_report)
         """
-
     async def get_domain_deliverability_campaign(
         self, *, CampaignId: str
     ) -> GetDomainDeliverabilityCampaignResponseTypeDef:
         """
         Retrieve all the deliverability data for a specific campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_domain_deliverability_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_domain_deliverability_campaign)
         """
-
     async def get_domain_statistics_report(
         self, *, Domain: str, StartDate: TimestampTypeDef, EndDate: TimestampTypeDef
     ) -> GetDomainStatisticsReportResponseTypeDef:
         """
         Retrieve inbox placement and engagement rates for the domains that you use to
         send email.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_domain_statistics_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_domain_statistics_report)
         """
-
     async def get_email_identity(self, *, EmailIdentity: str) -> GetEmailIdentityResponseTypeDef:
         """
         Provides information about a specific identity associated with your Amazon
         Pinpoint account, including the identity's verification status, its DKIM
         authentication status, and its custom Mail-From settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_email_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_email_identity)
         """
-
     async def list_configuration_sets(
         self, *, NextToken: str = ..., PageSize: int = ...
     ) -> ListConfigurationSetsResponseTypeDef:
         """
         List all of the configuration sets associated with your Amazon Pinpoint account
         in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_configuration_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#list_configuration_sets)
         """
-
     async def list_dedicated_ip_pools(
         self, *, NextToken: str = ..., PageSize: int = ...
     ) -> ListDedicatedIpPoolsResponseTypeDef:
         """
         List all of the dedicated IP pools that exist in your Amazon Pinpoint account in
         the current AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_dedicated_ip_pools)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#list_dedicated_ip_pools)
         """
-
     async def list_deliverability_test_reports(
         self, *, NextToken: str = ..., PageSize: int = ...
     ) -> ListDeliverabilityTestReportsResponseTypeDef:
         """
         Show a list of the predictive inbox placement tests that you've performed,
         regardless of their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_deliverability_test_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#list_deliverability_test_reports)
         """
-
     async def list_domain_deliverability_campaigns(
         self,
         *,
         StartDate: TimestampTypeDef,
         EndDate: TimestampTypeDef,
         SubscribedDomain: str,
         NextToken: str = ...,
@@ -401,172 +370,157 @@
         """
         Retrieve deliverability data for all the campaigns that used a specific domain
         to send email during a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_domain_deliverability_campaigns)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#list_domain_deliverability_campaigns)
         """
-
     async def list_email_identities(
         self, *, NextToken: str = ..., PageSize: int = ...
     ) -> ListEmailIdentitiesResponseTypeDef:
         """
         Returns a list of all of the email identities that are associated with your
         Amazon Pinpoint account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_email_identities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#list_email_identities)
         """
-
     async def list_tags_for_resource(
         self, *, ResourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieve a list of the tags (keys and values) that are associated with a
         specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#list_tags_for_resource)
         """
-
     async def put_account_dedicated_ip_warmup_attributes(
         self, *, AutoWarmupEnabled: bool = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable the automatic warm-up feature for dedicated IP addresses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_account_dedicated_ip_warmup_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_account_dedicated_ip_warmup_attributes)
         """
-
     async def put_account_sending_attributes(self, *, SendingEnabled: bool = ...) -> Dict[str, Any]:
         """
         Enable or disable the ability of your account to send email.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_account_sending_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_account_sending_attributes)
         """
-
     async def put_configuration_set_delivery_options(
         self,
         *,
         ConfigurationSetName: str,
         TlsPolicy: TlsPolicyType = ...,
         SendingPoolName: str = ...
     ) -> Dict[str, Any]:
         """
         Associate a configuration set with a dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_configuration_set_delivery_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_configuration_set_delivery_options)
         """
-
     async def put_configuration_set_reputation_options(
         self, *, ConfigurationSetName: str, ReputationMetricsEnabled: bool = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable collection of reputation metrics for emails that you send
         using a particular configuration set in a specific AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_configuration_set_reputation_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_configuration_set_reputation_options)
         """
-
     async def put_configuration_set_sending_options(
         self, *, ConfigurationSetName: str, SendingEnabled: bool = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable email sending for messages that use a particular configuration
         set in a specific AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_configuration_set_sending_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_configuration_set_sending_options)
         """
-
     async def put_configuration_set_tracking_options(
         self, *, ConfigurationSetName: str, CustomRedirectDomain: str = ...
     ) -> Dict[str, Any]:
         """
         Specify a custom domain to use for open and click tracking elements in email
         that you send using Amazon Pinpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_configuration_set_tracking_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_configuration_set_tracking_options)
         """
-
     async def put_dedicated_ip_in_pool(
         self, *, Ip: str, DestinationPoolName: str
     ) -> Dict[str, Any]:
         """
         Move a dedicated IP address to an existing dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_dedicated_ip_in_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_dedicated_ip_in_pool)
         """
-
     async def put_dedicated_ip_warmup_attributes(
         self, *, Ip: str, WarmupPercentage: int
     ) -> Dict[str, Any]:
         """
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/pinpoint-
         email-2018-07-26/PutDedicatedIpWarmupAttributes).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_dedicated_ip_warmup_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_dedicated_ip_warmup_attributes)
         """
-
     async def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef] = ...
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard for your Amazon Pinpoint account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_deliverability_dashboard_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_deliverability_dashboard_option)
         """
-
     async def put_email_identity_dkim_attributes(
         self, *, EmailIdentity: str, SigningEnabled: bool = ...
     ) -> Dict[str, Any]:
         """
         Used to enable or disable DKIM authentication for an email identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_email_identity_dkim_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_email_identity_dkim_attributes)
         """
-
     async def put_email_identity_feedback_attributes(
         self, *, EmailIdentity: str, EmailForwardingEnabled: bool = ...
     ) -> Dict[str, Any]:
         """
         Used to enable or disable feedback forwarding for an identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_email_identity_feedback_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_email_identity_feedback_attributes)
         """
-
     async def put_email_identity_mail_from_attributes(
         self,
         *,
         EmailIdentity: str,
         MailFromDomain: str = ...,
         BehaviorOnMxFailure: BehaviorOnMxFailureType = ...
     ) -> Dict[str, Any]:
         """
         Used to enable or disable the custom Mail-From domain configuration for an email
         identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_email_identity_mail_from_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_email_identity_mail_from_attributes)
         """
-
     async def send_email(
         self,
         *,
         Destination: DestinationTypeDef,
         Content: EmailContentTypeDef,
         FromEmailAddress: str = ...,
         ReplyToAddresses: Sequence[str] = ...,
@@ -576,94 +530,84 @@
     ) -> SendEmailResponseTypeDef:
         """
         Sends an email message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.send_email)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#send_email)
         """
-
     async def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Add one or more tags (keys and values) to a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#tag_resource)
         """
-
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Remove one or more tags (keys and values) from a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#untag_resource)
         """
-
     async def update_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
         EventDestination: EventDestinationDefinitionTypeDef
     ) -> Dict[str, Any]:
         """
         Update the configuration of an event destination for a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.update_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#update_configuration_set_event_destination)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_dedicated_ips"]
     ) -> GetDedicatedIpsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_configuration_sets"]
     ) -> ListConfigurationSetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_dedicated_ip_pools"]
     ) -> ListDedicatedIpPoolsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_deliverability_test_reports"]
     ) -> ListDeliverabilityTestReportsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_email_identities"]
     ) -> ListEmailIdentitiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "PinpointEmailClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/)
         """
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/client.pyi` & `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ListEmailIdentitiesPaginator,
 )
 from .type_defs import (
     CreateDeliverabilityTestReportResponseTypeDef,
     CreateEmailIdentityResponseTypeDef,
     DeliveryOptionsTypeDef,
     DestinationTypeDef,
-    DomainDeliverabilityTrackingOptionUnionTypeDef,
+    DomainDeliverabilityTrackingOptionTypeDef,
     EmailContentTypeDef,
     EventDestinationDefinitionTypeDef,
     GetAccountResponseTypeDef,
     GetBlacklistReportsResponseTypeDef,
     GetConfigurationSetEventDestinationsResponseTypeDef,
     GetConfigurationSetResponseTypeDef,
     GetDedicatedIpResponseTypeDef,
@@ -50,49 +50,53 @@
     ListConfigurationSetsResponseTypeDef,
     ListDedicatedIpPoolsResponseTypeDef,
     ListDeliverabilityTestReportsResponseTypeDef,
     ListDomainDeliverabilityCampaignsResponseTypeDef,
     ListEmailIdentitiesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MessageTagTypeDef,
-    ReputationOptionsUnionTypeDef,
+    ReputationOptionsTypeDef,
     SendEmailResponseTypeDef,
     SendingOptionsTypeDef,
     TagTypeDef,
     TimestampTypeDef,
     TrackingOptionsTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("PinpointEmailClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccountSuspendedException: Type[BotocoreClientError]
     AlreadyExistsException: Type[BotocoreClientError]
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConcurrentModificationException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     MailFromDomainNotVerifiedException: Type[BotocoreClientError]
     MessageRejected: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     SendingPausedException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
 
+
 class PinpointEmailClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/)
     """
 
     meta: ClientMeta
@@ -101,267 +105,294 @@
     def exceptions(self) -> Exceptions:
         """
         PinpointEmailClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#close)
         """
+
     async def create_configuration_set(
         self,
         *,
         ConfigurationSetName: str,
         TrackingOptions: TrackingOptionsTypeDef = ...,
         DeliveryOptions: DeliveryOptionsTypeDef = ...,
-        ReputationOptions: ReputationOptionsUnionTypeDef = ...,
+        ReputationOptions: ReputationOptionsTypeDef = ...,
         SendingOptions: SendingOptionsTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Create a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_configuration_set)
         """
+
     async def create_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
         EventDestination: EventDestinationDefinitionTypeDef
     ) -> Dict[str, Any]:
         """
         Create an event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_configuration_set_event_destination)
         """
+
     async def create_dedicated_ip_pool(
         self, *, PoolName: str, Tags: Sequence[TagTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Create a new pool of dedicated IP addresses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_dedicated_ip_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_dedicated_ip_pool)
         """
+
     async def create_deliverability_test_report(
         self,
         *,
         FromEmailAddress: str,
         Content: EmailContentTypeDef,
         ReportName: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDeliverabilityTestReportResponseTypeDef:
         """
         Create a new predictive inbox placement test.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_deliverability_test_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_deliverability_test_report)
         """
+
     async def create_email_identity(
         self, *, EmailIdentity: str, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateEmailIdentityResponseTypeDef:
         """
         Verifies an email identity for use with Amazon Pinpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.create_email_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#create_email_identity)
         """
+
     async def delete_configuration_set(self, *, ConfigurationSetName: str) -> Dict[str, Any]:
         """
         Delete an existing configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.delete_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#delete_configuration_set)
         """
+
     async def delete_configuration_set_event_destination(
         self, *, ConfigurationSetName: str, EventDestinationName: str
     ) -> Dict[str, Any]:
         """
         Delete an event destination.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.delete_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#delete_configuration_set_event_destination)
         """
+
     async def delete_dedicated_ip_pool(self, *, PoolName: str) -> Dict[str, Any]:
         """
         Delete a dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.delete_dedicated_ip_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#delete_dedicated_ip_pool)
         """
+
     async def delete_email_identity(self, *, EmailIdentity: str) -> Dict[str, Any]:
         """
         Deletes an email identity that you previously verified for use with Amazon
         Pinpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.delete_email_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#delete_email_identity)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#generate_presigned_url)
         """
+
     async def get_account(self) -> GetAccountResponseTypeDef:
         """
         Obtain information about the email-sending status and capabilities of your
         Amazon Pinpoint account in the current AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_account)
         """
+
     async def get_blacklist_reports(
         self, *, BlacklistItemNames: Sequence[str]
     ) -> GetBlacklistReportsResponseTypeDef:
         """
         Retrieve a list of the blacklists that your dedicated IP addresses appear on.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_blacklist_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_blacklist_reports)
         """
+
     async def get_configuration_set(
         self, *, ConfigurationSetName: str
     ) -> GetConfigurationSetResponseTypeDef:
         """
         Get information about an existing configuration set, including the dedicated IP
         pool that it's associated with, whether or not it's enabled for sending email,
         and more.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_configuration_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_configuration_set)
         """
+
     async def get_configuration_set_event_destinations(
         self, *, ConfigurationSetName: str
     ) -> GetConfigurationSetEventDestinationsResponseTypeDef:
         """
         Retrieve a list of event destinations that are associated with a configuration
         set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_configuration_set_event_destinations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_configuration_set_event_destinations)
         """
+
     async def get_dedicated_ip(self, *, Ip: str) -> GetDedicatedIpResponseTypeDef:
         """
         Get information about a dedicated IP address, including the name of the
         dedicated IP pool that it's associated with, as well information about the
         automatic warm-up process for the address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_dedicated_ip)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_dedicated_ip)
         """
+
     async def get_dedicated_ips(
         self, *, PoolName: str = ..., NextToken: str = ..., PageSize: int = ...
     ) -> GetDedicatedIpsResponseTypeDef:
         """
         List the dedicated IP addresses that are associated with your Amazon Pinpoint
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_dedicated_ips)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_dedicated_ips)
         """
+
     async def get_deliverability_dashboard_options(
         self,
     ) -> GetDeliverabilityDashboardOptionsResponseTypeDef:
         """
         Retrieve information about the status of the Deliverability dashboard for your
         Amazon Pinpoint account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_deliverability_dashboard_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_deliverability_dashboard_options)
         """
+
     async def get_deliverability_test_report(
         self, *, ReportId: str
     ) -> GetDeliverabilityTestReportResponseTypeDef:
         """
         Retrieve the results of a predictive inbox placement test.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_deliverability_test_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_deliverability_test_report)
         """
+
     async def get_domain_deliverability_campaign(
         self, *, CampaignId: str
     ) -> GetDomainDeliverabilityCampaignResponseTypeDef:
         """
         Retrieve all the deliverability data for a specific campaign.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_domain_deliverability_campaign)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_domain_deliverability_campaign)
         """
+
     async def get_domain_statistics_report(
         self, *, Domain: str, StartDate: TimestampTypeDef, EndDate: TimestampTypeDef
     ) -> GetDomainStatisticsReportResponseTypeDef:
         """
         Retrieve inbox placement and engagement rates for the domains that you use to
         send email.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_domain_statistics_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_domain_statistics_report)
         """
+
     async def get_email_identity(self, *, EmailIdentity: str) -> GetEmailIdentityResponseTypeDef:
         """
         Provides information about a specific identity associated with your Amazon
         Pinpoint account, including the identity's verification status, its DKIM
         authentication status, and its custom Mail-From settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_email_identity)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_email_identity)
         """
+
     async def list_configuration_sets(
         self, *, NextToken: str = ..., PageSize: int = ...
     ) -> ListConfigurationSetsResponseTypeDef:
         """
         List all of the configuration sets associated with your Amazon Pinpoint account
         in the current region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_configuration_sets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#list_configuration_sets)
         """
+
     async def list_dedicated_ip_pools(
         self, *, NextToken: str = ..., PageSize: int = ...
     ) -> ListDedicatedIpPoolsResponseTypeDef:
         """
         List all of the dedicated IP pools that exist in your Amazon Pinpoint account in
         the current AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_dedicated_ip_pools)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#list_dedicated_ip_pools)
         """
+
     async def list_deliverability_test_reports(
         self, *, NextToken: str = ..., PageSize: int = ...
     ) -> ListDeliverabilityTestReportsResponseTypeDef:
         """
         Show a list of the predictive inbox placement tests that you've performed,
         regardless of their statuses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_deliverability_test_reports)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#list_deliverability_test_reports)
         """
+
     async def list_domain_deliverability_campaigns(
         self,
         *,
         StartDate: TimestampTypeDef,
         EndDate: TimestampTypeDef,
         SubscribedDomain: str,
         NextToken: str = ...,
@@ -370,157 +401,172 @@
         """
         Retrieve deliverability data for all the campaigns that used a specific domain
         to send email during a specified time range.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_domain_deliverability_campaigns)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#list_domain_deliverability_campaigns)
         """
+
     async def list_email_identities(
         self, *, NextToken: str = ..., PageSize: int = ...
     ) -> ListEmailIdentitiesResponseTypeDef:
         """
         Returns a list of all of the email identities that are associated with your
         Amazon Pinpoint account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_email_identities)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#list_email_identities)
         """
+
     async def list_tags_for_resource(
         self, *, ResourceArn: str
     ) -> ListTagsForResourceResponseTypeDef:
         """
         Retrieve a list of the tags (keys and values) that are associated with a
         specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#list_tags_for_resource)
         """
+
     async def put_account_dedicated_ip_warmup_attributes(
         self, *, AutoWarmupEnabled: bool = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable the automatic warm-up feature for dedicated IP addresses.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_account_dedicated_ip_warmup_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_account_dedicated_ip_warmup_attributes)
         """
+
     async def put_account_sending_attributes(self, *, SendingEnabled: bool = ...) -> Dict[str, Any]:
         """
         Enable or disable the ability of your account to send email.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_account_sending_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_account_sending_attributes)
         """
+
     async def put_configuration_set_delivery_options(
         self,
         *,
         ConfigurationSetName: str,
         TlsPolicy: TlsPolicyType = ...,
         SendingPoolName: str = ...
     ) -> Dict[str, Any]:
         """
         Associate a configuration set with a dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_configuration_set_delivery_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_configuration_set_delivery_options)
         """
+
     async def put_configuration_set_reputation_options(
         self, *, ConfigurationSetName: str, ReputationMetricsEnabled: bool = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable collection of reputation metrics for emails that you send
         using a particular configuration set in a specific AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_configuration_set_reputation_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_configuration_set_reputation_options)
         """
+
     async def put_configuration_set_sending_options(
         self, *, ConfigurationSetName: str, SendingEnabled: bool = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable email sending for messages that use a particular configuration
         set in a specific AWS Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_configuration_set_sending_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_configuration_set_sending_options)
         """
+
     async def put_configuration_set_tracking_options(
         self, *, ConfigurationSetName: str, CustomRedirectDomain: str = ...
     ) -> Dict[str, Any]:
         """
         Specify a custom domain to use for open and click tracking elements in email
         that you send using Amazon Pinpoint.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_configuration_set_tracking_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_configuration_set_tracking_options)
         """
+
     async def put_dedicated_ip_in_pool(
         self, *, Ip: str, DestinationPoolName: str
     ) -> Dict[str, Any]:
         """
         Move a dedicated IP address to an existing dedicated IP pool.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_dedicated_ip_in_pool)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_dedicated_ip_in_pool)
         """
+
     async def put_dedicated_ip_warmup_attributes(
         self, *, Ip: str, WarmupPercentage: int
     ) -> Dict[str, Any]:
         """
         See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/pinpoint-
         email-2018-07-26/PutDedicatedIpWarmupAttributes).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_dedicated_ip_warmup_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_dedicated_ip_warmup_attributes)
         """
+
     async def put_deliverability_dashboard_option(
         self,
         *,
         DashboardEnabled: bool,
-        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef] = ...
+        SubscribedDomains: Sequence[DomainDeliverabilityTrackingOptionTypeDef] = ...
     ) -> Dict[str, Any]:
         """
         Enable or disable the Deliverability dashboard for your Amazon Pinpoint account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_deliverability_dashboard_option)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_deliverability_dashboard_option)
         """
+
     async def put_email_identity_dkim_attributes(
         self, *, EmailIdentity: str, SigningEnabled: bool = ...
     ) -> Dict[str, Any]:
         """
         Used to enable or disable DKIM authentication for an email identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_email_identity_dkim_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_email_identity_dkim_attributes)
         """
+
     async def put_email_identity_feedback_attributes(
         self, *, EmailIdentity: str, EmailForwardingEnabled: bool = ...
     ) -> Dict[str, Any]:
         """
         Used to enable or disable feedback forwarding for an identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_email_identity_feedback_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_email_identity_feedback_attributes)
         """
+
     async def put_email_identity_mail_from_attributes(
         self,
         *,
         EmailIdentity: str,
         MailFromDomain: str = ...,
         BehaviorOnMxFailure: BehaviorOnMxFailureType = ...
     ) -> Dict[str, Any]:
         """
         Used to enable or disable the custom Mail-From domain configuration for an email
         identity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.put_email_identity_mail_from_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#put_email_identity_mail_from_attributes)
         """
+
     async def send_email(
         self,
         *,
         Destination: DestinationTypeDef,
         Content: EmailContentTypeDef,
         FromEmailAddress: str = ...,
         ReplyToAddresses: Sequence[str] = ...,
@@ -530,84 +576,94 @@
     ) -> SendEmailResponseTypeDef:
         """
         Sends an email message.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.send_email)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#send_email)
         """
+
     async def tag_resource(self, *, ResourceArn: str, Tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Add one or more tags (keys and values) to a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#tag_resource)
         """
+
     async def untag_resource(self, *, ResourceArn: str, TagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Remove one or more tags (keys and values) from a specified resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#untag_resource)
         """
+
     async def update_configuration_set_event_destination(
         self,
         *,
         ConfigurationSetName: str,
         EventDestinationName: str,
         EventDestination: EventDestinationDefinitionTypeDef
     ) -> Dict[str, Any]:
         """
         Update the configuration of an event destination for a configuration set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.update_configuration_set_event_destination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#update_configuration_set_event_destination)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_dedicated_ips"]
     ) -> GetDedicatedIpsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_configuration_sets"]
     ) -> ListConfigurationSetsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_dedicated_ip_pools"]
     ) -> ListDedicatedIpPoolsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_deliverability_test_reports"]
     ) -> ListDeliverabilityTestReportsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_email_identities"]
     ) -> ListEmailIdentitiesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "PinpointEmailClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/pinpoint-email.html#PinpointEmail.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_pinpoint_email/client/)
         """
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/literals.py` & `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
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
@@ -175,14 +176,15 @@
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
@@ -261,26 +263,28 @@
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

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/literals.pyi` & `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -70,14 +70,15 @@
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
@@ -173,14 +174,15 @@
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
@@ -259,26 +261,28 @@
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

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/paginator.py` & `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/paginator.pyi` & `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/type_defs.py` & `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BlacklistEntryTypeDef",
     "BlobTypeDef",
     "ContentTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "DeliveryOptionsTypeDef",
     "SendingOptionsTypeDef",
@@ -53,32 +52,30 @@
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
     "DestinationTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
-    "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
-    "TimestampTypeDef",
     "TemplateTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "SendQuotaTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
-    "ReputationOptionsOutputTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "IdentityInfoTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
@@ -94,15 +91,14 @@
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "RawMessageTypeDef",
     "BodyTypeDef",
-    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
     "CreateEmailIdentityRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDeliverabilityTestReportResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "ListConfigurationSetsResponseTypeDef",
@@ -113,43 +109,40 @@
     "DailyVolumeTypeDef",
     "OverallVolumeTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
-    "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
-    "GetDomainStatisticsReportRequestRequestTypeDef",
-    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    "ReputationOptionsTypeDef",
     "GetAccountResponseTypeDef",
-    "GetConfigurationSetResponseTypeDef",
     "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
     "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
     "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
     "IspPlacementTypeDef",
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    "ReputationOptionsTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "MessageTypeDef",
-    "EventDestinationTypeDef",
     "EventDestinationDefinitionTypeDef",
+    "EventDestinationTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
-    "DomainDeliverabilityTrackingOptionUnionTypeDef",
-    "CreateConfigurationSetRequestRequestTypeDef",
-    "ReputationOptionsUnionTypeDef",
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
+    "CreateConfigurationSetRequestRequestTypeDef",
+    "GetConfigurationSetResponseTypeDef",
     "EmailContentTypeDef",
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 BlacklistEntryTypeDef = TypedDict(
     "BlacklistEntryTypeDef",
     {
@@ -171,19 +164,17 @@
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
 CloudWatchDimensionConfigurationTypeDef = TypedDict(
     "CloudWatchDimensionConfigurationTypeDef",
     {
         "DimensionName": str,
         "DimensionValueSource": DimensionValueSourceType,
         "DefaultDimensionValue": str,
     },
@@ -277,19 +268,17 @@
     "_OptionalDedicatedIpTypeDef",
     {
         "PoolName": str,
     },
     total=False,
 )
 
-
 class DedicatedIpTypeDef(_RequiredDedicatedIpTypeDef, _OptionalDedicatedIpTypeDef):
     pass
 
-
 DeleteConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -355,33 +344,23 @@
         "ReadDeleteRate": float,
         "ProjectedVolume": int,
         "Esps": List[str],
     },
     total=False,
 )
 
-InboxPlacementTrackingOptionOutputTypeDef = TypedDict(
-    "InboxPlacementTrackingOptionOutputTypeDef",
-    {
-        "Global": bool,
-        "TrackedIsps": List[str],
-    },
-    total=False,
-)
-
 InboxPlacementTrackingOptionTypeDef = TypedDict(
     "InboxPlacementTrackingOptionTypeDef",
     {
         "Global": bool,
-        "TrackedIsps": Sequence[str],
+        "TrackedIsps": List[str],
     },
     total=False,
 )
 
-TimestampTypeDef = Union[datetime, str]
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "TemplateArn": str,
         "TemplateData": str,
     },
     total=False,
@@ -437,23 +416,14 @@
 GetConfigurationSetRequestRequestTypeDef = TypedDict(
     "GetConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
-ReputationOptionsOutputTypeDef = TypedDict(
-    "ReputationOptionsOutputTypeDef",
-    {
-        "ReputationMetricsEnabled": bool,
-        "LastFreshStart": datetime,
-    },
-    total=False,
-)
-
 GetDedicatedIpRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpRequestRequestTypeDef",
     {
         "Ip": str,
     },
 )
 
@@ -499,14 +469,15 @@
 GetDomainDeliverabilityCampaignRequestRequestTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     {
         "CampaignId": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 GetEmailIdentityRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
@@ -607,88 +578,80 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
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
 _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ReputationMetricsEnabled": bool,
     },
     total=False,
 )
 
-
 class PutConfigurationSetReputationOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
 
-
 class PutConfigurationSetSendingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "CustomRedirectDomain": str,
     },
     total=False,
 )
 
-
 class PutConfigurationSetTrackingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
 ):
     pass
 
-
 PutDedicatedIpInPoolRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
@@ -711,44 +674,40 @@
     "_OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "SigningEnabled": bool,
     },
     total=False,
 )
 
-
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailForwardingEnabled": bool,
     },
     total=False,
 )
 
-
 class PutEmailIdentityFeedbackAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
@@ -756,22 +715,20 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMxFailure": BehaviorOnMxFailureType,
     },
     total=False,
 )
 
-
 class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -788,21 +745,14 @@
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
 )
 
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
 
@@ -816,44 +766,40 @@
     "_OptionalCreateDedicatedIpPoolRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDedicatedIpPoolRequestRequestTypeDef(
     _RequiredCreateDedicatedIpPoolRequestRequestTypeDef,
     _OptionalCreateDedicatedIpPoolRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_OptionalCreateEmailIdentityRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateEmailIdentityRequestRequestTypeDef(
     _RequiredCreateEmailIdentityRequestRequestTypeDef,
     _OptionalCreateEmailIdentityRequestRequestTypeDef,
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -978,102 +924,36 @@
     {
         "DomainDeliverabilityCampaigns": List[DomainDeliverabilityCampaignTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DomainDeliverabilityTrackingOptionOutputTypeDef = TypedDict(
-    "DomainDeliverabilityTrackingOptionOutputTypeDef",
-    {
-        "Domain": str,
-        "SubscriptionStartDate": datetime,
-        "InboxPlacementTrackingOption": InboxPlacementTrackingOptionOutputTypeDef,
-    },
-    total=False,
-)
-
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": str,
-        "SubscriptionStartDate": TimestampTypeDef,
+        "SubscriptionStartDate": datetime,
         "InboxPlacementTrackingOption": InboxPlacementTrackingOptionTypeDef,
     },
     total=False,
 )
 
-GetDomainStatisticsReportRequestRequestTypeDef = TypedDict(
-    "GetDomainStatisticsReportRequestRequestTypeDef",
-    {
-        "Domain": str,
-        "StartDate": TimestampTypeDef,
-        "EndDate": TimestampTypeDef,
-    },
-)
-
-_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    {
-        "StartDate": TimestampTypeDef,
-        "EndDate": TimestampTypeDef,
-        "SubscribedDomain": str,
-    },
-)
-_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "PageSize": int,
-    },
-    total=False,
-)
-
-
-class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
-    _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-    _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-):
-    pass
-
-
-ReputationOptionsTypeDef = TypedDict(
-    "ReputationOptionsTypeDef",
-    {
-        "ReputationMetricsEnabled": bool,
-        "LastFreshStart": TimestampTypeDef,
-    },
-    total=False,
-)
-
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetConfigurationSetResponseTypeDef = TypedDict(
-    "GetConfigurationSetResponseTypeDef",
-    {
-        "ConfigurationSetName": str,
-        "TrackingOptions": TrackingOptionsTypeDef,
-        "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsOutputTypeDef,
-        "SendingOptions": SendingOptionsTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef = TypedDict(
     "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     {
         "PoolName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1116,14 +996,55 @@
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
     },
     total=False,
 )
 
+GetDomainStatisticsReportRequestRequestTypeDef = TypedDict(
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    {
+        "Domain": str,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+    },
+)
+
+_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    {
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "SubscribedDomain": str,
+    },
+)
+_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "PageSize": int,
+    },
+    total=False,
+)
+
+class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
+    _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+):
+    pass
+
+ReputationOptionsTypeDef = TypedDict(
+    "ReputationOptionsTypeDef",
+    {
+        "ReputationMetricsEnabled": bool,
+        "LastFreshStart": TimestampTypeDef,
+    },
+    total=False,
+)
+
 GetEmailIdentityResponseTypeDef = TypedDict(
     "GetEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
@@ -1146,51 +1067,49 @@
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
 
+EventDestinationDefinitionTypeDef = TypedDict(
+    "EventDestinationDefinitionTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingEventTypes": Sequence[EventTypeType],
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationTypeDef,
+        "SnsDestination": SnsDestinationTypeDef,
+        "PinpointDestination": PinpointDestinationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationTypeDef = TypedDict(
     "_OptionalEventDestinationTypeDef",
     {
         "Enabled": bool,
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationTypeDef,
         "SnsDestination": SnsDestinationTypeDef,
         "PinpointDestination": PinpointDestinationTypeDef,
     },
     total=False,
 )
 
-
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
-
-EventDestinationDefinitionTypeDef = TypedDict(
-    "EventDestinationDefinitionTypeDef",
-    {
-        "Enabled": bool,
-        "MatchingEventTypes": Sequence[EventTypeType],
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationTypeDef,
-        "SnsDestination": SnsDestinationTypeDef,
-        "PinpointDestination": PinpointDestinationTypeDef,
-    },
-    total=False,
-)
-
 GetDomainStatisticsReportResponseTypeDef = TypedDict(
     "GetDomainStatisticsReportResponseTypeDef",
     {
         "OverallVolume": OverallVolumeTypeDef,
         "DailyVolumes": List[DailyVolumeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1198,23 +1117,52 @@
 
 GetDeliverabilityDashboardOptionsResponseTypeDef = TypedDict(
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     {
         "DashboardEnabled": bool,
         "SubscriptionExpiryDate": datetime,
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
-        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
-        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
+        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "DashboardEnabled": bool,
+    },
+)
+_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
+    },
+    total=False,
+)
+
+class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
+    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+):
+    pass
+
+GetDeliverabilityTestReportResponseTypeDef = TypedDict(
+    "GetDeliverabilityTestReportResponseTypeDef",
+    {
+        "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
+        "OverallPlacement": PlacementStatisticsTypeDef,
+        "IspPlacements": List[IspPlacementTypeDef],
+        "Message": str,
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
-    DomainDeliverabilityTrackingOptionTypeDef, DomainDeliverabilityTrackingOptionOutputTypeDef
-]
 _RequiredCreateConfigurationSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalCreateConfigurationSetRequestRequestTypeDef = TypedDict(
@@ -1225,30 +1173,28 @@
         "ReputationOptions": ReputationOptionsTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
-
-ReputationOptionsUnionTypeDef = Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef]
-GetDeliverabilityTestReportResponseTypeDef = TypedDict(
-    "GetDeliverabilityTestReportResponseTypeDef",
+GetConfigurationSetResponseTypeDef = TypedDict(
+    "GetConfigurationSetResponseTypeDef",
     {
-        "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
-        "OverallPlacement": PlacementStatisticsTypeDef,
-        "IspPlacements": List[IspPlacementTypeDef],
-        "Message": str,
+        "ConfigurationSetName": str,
+        "TrackingOptions": TrackingOptionsTypeDef,
+        "DeliveryOptions": DeliveryOptionsTypeDef,
+        "ReputationOptions": ReputationOptionsTypeDef,
+        "SendingOptions": SendingOptionsTypeDef,
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
@@ -1256,22 +1202,14 @@
         "Simple": MessageTypeDef,
         "Raw": RawMessageTypeDef,
         "Template": TemplateTypeDef,
     },
     total=False,
 )
 
-GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
-    {
-        "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
@@ -1282,36 +1220,22 @@
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
 )
 
-_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "DashboardEnabled": bool,
-    },
-)
-_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     {
-        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef],
+        "EventDestinations": List[EventDestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
-    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeliverabilityTestReportRequestRequestTypeDef",
     {
         "FromEmailAddress": str,
         "Content": EmailContentTypeDef,
     },
 )
@@ -1320,22 +1244,20 @@
     {
         "ReportName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDeliverabilityTestReportRequestRequestTypeDef(
     _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef,
     _OptionalCreateDeliverabilityTestReportRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Destination": DestinationTypeDef,
         "Content": EmailContentTypeDef,
     },
 )
@@ -1347,12 +1269,11 @@
         "FeedbackForwardingEmailAddress": str,
         "EmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
-
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email/type_defs.pyi` & `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BlacklistEntryTypeDef",
     "BlobTypeDef",
     "ContentTypeDef",
     "CloudWatchDimensionConfigurationTypeDef",
     "DeliveryOptionsTypeDef",
     "SendingOptionsTypeDef",
@@ -52,32 +53,30 @@
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     "DeleteConfigurationSetRequestRequestTypeDef",
     "DeleteDedicatedIpPoolRequestRequestTypeDef",
     "DeleteEmailIdentityRequestRequestTypeDef",
     "DeliverabilityTestReportTypeDef",
     "DestinationTypeDef",
     "DomainDeliverabilityCampaignTypeDef",
-    "InboxPlacementTrackingOptionOutputTypeDef",
     "InboxPlacementTrackingOptionTypeDef",
-    "TimestampTypeDef",
     "TemplateTypeDef",
     "KinesisFirehoseDestinationTypeDef",
     "PinpointDestinationTypeDef",
     "SnsDestinationTypeDef",
     "SendQuotaTypeDef",
     "GetBlacklistReportsRequestRequestTypeDef",
     "GetConfigurationSetEventDestinationsRequestRequestTypeDef",
     "GetConfigurationSetRequestRequestTypeDef",
-    "ReputationOptionsOutputTypeDef",
     "GetDedicatedIpRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "GetDedicatedIpsRequestRequestTypeDef",
     "GetDeliverabilityTestReportRequestRequestTypeDef",
     "PlacementStatisticsTypeDef",
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetEmailIdentityRequestRequestTypeDef",
     "MailFromAttributesTypeDef",
     "IdentityInfoTypeDef",
     "ListConfigurationSetsRequestRequestTypeDef",
     "ListDedicatedIpPoolsRequestRequestTypeDef",
     "ListDeliverabilityTestReportsRequestRequestTypeDef",
     "ListEmailIdentitiesRequestRequestTypeDef",
@@ -93,15 +92,14 @@
     "PutDedicatedIpWarmupAttributesRequestRequestTypeDef",
     "PutEmailIdentityDkimAttributesRequestRequestTypeDef",
     "PutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     "PutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "RawMessageTypeDef",
     "BodyTypeDef",
-    "CloudWatchDestinationOutputTypeDef",
     "CloudWatchDestinationTypeDef",
     "CreateDedicatedIpPoolRequestRequestTypeDef",
     "CreateEmailIdentityRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDeliverabilityTestReportResponseTypeDef",
     "GetBlacklistReportsResponseTypeDef",
     "ListConfigurationSetsResponseTypeDef",
@@ -112,43 +110,40 @@
     "DailyVolumeTypeDef",
     "OverallVolumeTypeDef",
     "GetDedicatedIpResponseTypeDef",
     "GetDedicatedIpsResponseTypeDef",
     "ListDeliverabilityTestReportsResponseTypeDef",
     "GetDomainDeliverabilityCampaignResponseTypeDef",
     "ListDomainDeliverabilityCampaignsResponseTypeDef",
-    "DomainDeliverabilityTrackingOptionOutputTypeDef",
     "DomainDeliverabilityTrackingOptionTypeDef",
-    "GetDomainStatisticsReportRequestRequestTypeDef",
-    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    "ReputationOptionsTypeDef",
     "GetAccountResponseTypeDef",
-    "GetConfigurationSetResponseTypeDef",
     "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     "ListConfigurationSetsRequestListConfigurationSetsPaginateTypeDef",
     "ListDedicatedIpPoolsRequestListDedicatedIpPoolsPaginateTypeDef",
     "ListDeliverabilityTestReportsRequestListDeliverabilityTestReportsPaginateTypeDef",
     "ListEmailIdentitiesRequestListEmailIdentitiesPaginateTypeDef",
     "IspPlacementTypeDef",
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    "ListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    "ReputationOptionsTypeDef",
     "GetEmailIdentityResponseTypeDef",
     "ListEmailIdentitiesResponseTypeDef",
     "MessageTypeDef",
-    "EventDestinationTypeDef",
     "EventDestinationDefinitionTypeDef",
+    "EventDestinationTypeDef",
     "GetDomainStatisticsReportResponseTypeDef",
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
-    "DomainDeliverabilityTrackingOptionUnionTypeDef",
-    "CreateConfigurationSetRequestRequestTypeDef",
-    "ReputationOptionsUnionTypeDef",
+    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
     "GetDeliverabilityTestReportResponseTypeDef",
+    "CreateConfigurationSetRequestRequestTypeDef",
+    "GetConfigurationSetResponseTypeDef",
     "EmailContentTypeDef",
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     "UpdateConfigurationSetEventDestinationRequestRequestTypeDef",
-    "PutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     "CreateDeliverabilityTestReportRequestRequestTypeDef",
     "SendEmailRequestRequestTypeDef",
 )
 
 BlacklistEntryTypeDef = TypedDict(
     "BlacklistEntryTypeDef",
     {
@@ -170,17 +165,19 @@
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
 CloudWatchDimensionConfigurationTypeDef = TypedDict(
     "CloudWatchDimensionConfigurationTypeDef",
     {
         "DimensionName": str,
         "DimensionValueSource": DimensionValueSourceType,
         "DefaultDimensionValue": str,
     },
@@ -274,17 +271,19 @@
     "_OptionalDedicatedIpTypeDef",
     {
         "PoolName": str,
     },
     total=False,
 )
 
+
 class DedicatedIpTypeDef(_RequiredDedicatedIpTypeDef, _OptionalDedicatedIpTypeDef):
     pass
 
+
 DeleteConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "DeleteConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
     },
 )
@@ -350,33 +349,23 @@
         "ReadDeleteRate": float,
         "ProjectedVolume": int,
         "Esps": List[str],
     },
     total=False,
 )
 
-InboxPlacementTrackingOptionOutputTypeDef = TypedDict(
-    "InboxPlacementTrackingOptionOutputTypeDef",
-    {
-        "Global": bool,
-        "TrackedIsps": List[str],
-    },
-    total=False,
-)
-
 InboxPlacementTrackingOptionTypeDef = TypedDict(
     "InboxPlacementTrackingOptionTypeDef",
     {
         "Global": bool,
-        "TrackedIsps": Sequence[str],
+        "TrackedIsps": List[str],
     },
     total=False,
 )
 
-TimestampTypeDef = Union[datetime, str]
 TemplateTypeDef = TypedDict(
     "TemplateTypeDef",
     {
         "TemplateArn": str,
         "TemplateData": str,
     },
     total=False,
@@ -432,23 +421,14 @@
 GetConfigurationSetRequestRequestTypeDef = TypedDict(
     "GetConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 
-ReputationOptionsOutputTypeDef = TypedDict(
-    "ReputationOptionsOutputTypeDef",
-    {
-        "ReputationMetricsEnabled": bool,
-        "LastFreshStart": datetime,
-    },
-    total=False,
-)
-
 GetDedicatedIpRequestRequestTypeDef = TypedDict(
     "GetDedicatedIpRequestRequestTypeDef",
     {
         "Ip": str,
     },
 )
 
@@ -494,14 +474,15 @@
 GetDomainDeliverabilityCampaignRequestRequestTypeDef = TypedDict(
     "GetDomainDeliverabilityCampaignRequestRequestTypeDef",
     {
         "CampaignId": str,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 GetEmailIdentityRequestRequestTypeDef = TypedDict(
     "GetEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 
@@ -602,80 +583,88 @@
     {
         "TlsPolicy": TlsPolicyType,
         "SendingPoolName": str,
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
 _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef",
     {
         "ReputationMetricsEnabled": bool,
     },
     total=False,
 )
 
+
 class PutConfigurationSetReputationOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetReputationOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetReputationOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef",
     {
         "SendingEnabled": bool,
     },
     total=False,
 )
 
+
 class PutConfigurationSetSendingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetSendingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetSendingOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef = TypedDict(
     "_OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef",
     {
         "CustomRedirectDomain": str,
     },
     total=False,
 )
 
+
 class PutConfigurationSetTrackingOptionsRequestRequestTypeDef(
     _RequiredPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
     _OptionalPutConfigurationSetTrackingOptionsRequestRequestTypeDef,
 ):
     pass
 
+
 PutDedicatedIpInPoolRequestRequestTypeDef = TypedDict(
     "PutDedicatedIpInPoolRequestRequestTypeDef",
     {
         "Ip": str,
         "DestinationPoolName": str,
     },
 )
@@ -698,40 +687,44 @@
     "_OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef",
     {
         "SigningEnabled": bool,
     },
     total=False,
 )
 
+
 class PutEmailIdentityDkimAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityDkimAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityDkimAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef = TypedDict(
     "_OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef",
     {
         "EmailForwardingEnabled": bool,
     },
     total=False,
 )
 
+
 class PutEmailIdentityFeedbackAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityFeedbackAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef = TypedDict(
@@ -739,20 +732,22 @@
     {
         "MailFromDomain": str,
         "BehaviorOnMxFailure": BehaviorOnMxFailureType,
     },
     total=False,
 )
 
+
 class PutEmailIdentityMailFromAttributesRequestRequestTypeDef(
     _RequiredPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
     _OptionalPutEmailIdentityMailFromAttributesRequestRequestTypeDef,
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -769,21 +764,14 @@
     {
         "Text": ContentTypeDef,
         "Html": ContentTypeDef,
     },
     total=False,
 )
 
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
 
@@ -797,40 +785,44 @@
     "_OptionalCreateDedicatedIpPoolRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDedicatedIpPoolRequestRequestTypeDef(
     _RequiredCreateDedicatedIpPoolRequestRequestTypeDef,
     _OptionalCreateDedicatedIpPoolRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_RequiredCreateEmailIdentityRequestRequestTypeDef",
     {
         "EmailIdentity": str,
     },
 )
 _OptionalCreateEmailIdentityRequestRequestTypeDef = TypedDict(
     "_OptionalCreateEmailIdentityRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateEmailIdentityRequestRequestTypeDef(
     _RequiredCreateEmailIdentityRequestRequestTypeDef,
     _OptionalCreateEmailIdentityRequestRequestTypeDef,
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -955,100 +947,36 @@
     {
         "DomainDeliverabilityCampaigns": List[DomainDeliverabilityCampaignTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DomainDeliverabilityTrackingOptionOutputTypeDef = TypedDict(
-    "DomainDeliverabilityTrackingOptionOutputTypeDef",
-    {
-        "Domain": str,
-        "SubscriptionStartDate": datetime,
-        "InboxPlacementTrackingOption": InboxPlacementTrackingOptionOutputTypeDef,
-    },
-    total=False,
-)
-
 DomainDeliverabilityTrackingOptionTypeDef = TypedDict(
     "DomainDeliverabilityTrackingOptionTypeDef",
     {
         "Domain": str,
-        "SubscriptionStartDate": TimestampTypeDef,
+        "SubscriptionStartDate": datetime,
         "InboxPlacementTrackingOption": InboxPlacementTrackingOptionTypeDef,
     },
     total=False,
 )
 
-GetDomainStatisticsReportRequestRequestTypeDef = TypedDict(
-    "GetDomainStatisticsReportRequestRequestTypeDef",
-    {
-        "Domain": str,
-        "StartDate": TimestampTypeDef,
-        "EndDate": TimestampTypeDef,
-    },
-)
-
-_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
-    "_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    {
-        "StartDate": TimestampTypeDef,
-        "EndDate": TimestampTypeDef,
-        "SubscribedDomain": str,
-    },
-)
-_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
-    "_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef",
-    {
-        "NextToken": str,
-        "PageSize": int,
-    },
-    total=False,
-)
-
-class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
-    _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-    _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
-):
-    pass
-
-ReputationOptionsTypeDef = TypedDict(
-    "ReputationOptionsTypeDef",
-    {
-        "ReputationMetricsEnabled": bool,
-        "LastFreshStart": TimestampTypeDef,
-    },
-    total=False,
-)
-
 GetAccountResponseTypeDef = TypedDict(
     "GetAccountResponseTypeDef",
     {
         "SendQuota": SendQuotaTypeDef,
         "SendingEnabled": bool,
         "DedicatedIpAutoWarmupEnabled": bool,
         "EnforcementStatus": str,
         "ProductionAccessEnabled": bool,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetConfigurationSetResponseTypeDef = TypedDict(
-    "GetConfigurationSetResponseTypeDef",
-    {
-        "ConfigurationSetName": str,
-        "TrackingOptions": TrackingOptionsTypeDef,
-        "DeliveryOptions": DeliveryOptionsTypeDef,
-        "ReputationOptions": ReputationOptionsOutputTypeDef,
-        "SendingOptions": SendingOptionsTypeDef,
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef = TypedDict(
     "GetDedicatedIpsRequestGetDedicatedIpsPaginateTypeDef",
     {
         "PoolName": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
@@ -1091,14 +1019,57 @@
     {
         "IspName": str,
         "PlacementStatistics": PlacementStatisticsTypeDef,
     },
     total=False,
 )
 
+GetDomainStatisticsReportRequestRequestTypeDef = TypedDict(
+    "GetDomainStatisticsReportRequestRequestTypeDef",
+    {
+        "Domain": str,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+    },
+)
+
+_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
+    "_RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    {
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "SubscribedDomain": str,
+    },
+)
+_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef = TypedDict(
+    "_OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef",
+    {
+        "NextToken": str,
+        "PageSize": int,
+    },
+    total=False,
+)
+
+
+class ListDomainDeliverabilityCampaignsRequestRequestTypeDef(
+    _RequiredListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+    _OptionalListDomainDeliverabilityCampaignsRequestRequestTypeDef,
+):
+    pass
+
+
+ReputationOptionsTypeDef = TypedDict(
+    "ReputationOptionsTypeDef",
+    {
+        "ReputationMetricsEnabled": bool,
+        "LastFreshStart": TimestampTypeDef,
+    },
+    total=False,
+)
+
 GetEmailIdentityResponseTypeDef = TypedDict(
     "GetEmailIdentityResponseTypeDef",
     {
         "IdentityType": IdentityTypeType,
         "FeedbackForwardingStatus": bool,
         "VerifiedForSendingStatus": bool,
         "DkimAttributes": DkimAttributesTypeDef,
@@ -1121,48 +1092,50 @@
     "MessageTypeDef",
     {
         "Subject": ContentTypeDef,
         "Body": BodyTypeDef,
     },
 )
 
+EventDestinationDefinitionTypeDef = TypedDict(
+    "EventDestinationDefinitionTypeDef",
+    {
+        "Enabled": bool,
+        "MatchingEventTypes": Sequence[EventTypeType],
+        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationTypeDef,
+        "SnsDestination": SnsDestinationTypeDef,
+        "PinpointDestination": PinpointDestinationTypeDef,
+    },
+    total=False,
+)
+
 _RequiredEventDestinationTypeDef = TypedDict(
     "_RequiredEventDestinationTypeDef",
     {
         "Name": str,
         "MatchingEventTypes": List[EventTypeType],
     },
 )
 _OptionalEventDestinationTypeDef = TypedDict(
     "_OptionalEventDestinationTypeDef",
     {
         "Enabled": bool,
         "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationOutputTypeDef,
+        "CloudWatchDestination": CloudWatchDestinationTypeDef,
         "SnsDestination": SnsDestinationTypeDef,
         "PinpointDestination": PinpointDestinationTypeDef,
     },
     total=False,
 )
 
+
 class EventDestinationTypeDef(_RequiredEventDestinationTypeDef, _OptionalEventDestinationTypeDef):
     pass
 
-EventDestinationDefinitionTypeDef = TypedDict(
-    "EventDestinationDefinitionTypeDef",
-    {
-        "Enabled": bool,
-        "MatchingEventTypes": Sequence[EventTypeType],
-        "KinesisFirehoseDestination": KinesisFirehoseDestinationTypeDef,
-        "CloudWatchDestination": CloudWatchDestinationTypeDef,
-        "SnsDestination": SnsDestinationTypeDef,
-        "PinpointDestination": PinpointDestinationTypeDef,
-    },
-    total=False,
-)
 
 GetDomainStatisticsReportResponseTypeDef = TypedDict(
     "GetDomainStatisticsReportResponseTypeDef",
     {
         "OverallVolume": OverallVolumeTypeDef,
         "DailyVolumes": List[DailyVolumeTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1171,23 +1144,54 @@
 
 GetDeliverabilityDashboardOptionsResponseTypeDef = TypedDict(
     "GetDeliverabilityDashboardOptionsResponseTypeDef",
     {
         "DashboardEnabled": bool,
         "SubscriptionExpiryDate": datetime,
         "AccountStatus": DeliverabilityDashboardAccountStatusType,
-        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
-        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionOutputTypeDef],
+        "ActiveSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
+        "PendingExpirationSubscribedDomains": List[DomainDeliverabilityTrackingOptionTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "DashboardEnabled": bool,
+    },
+)
+_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
+    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+    {
+        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionTypeDef],
+    },
+    total=False,
+)
+
+
+class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
+    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
+):
+    pass
+
+
+GetDeliverabilityTestReportResponseTypeDef = TypedDict(
+    "GetDeliverabilityTestReportResponseTypeDef",
+    {
+        "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
+        "OverallPlacement": PlacementStatisticsTypeDef,
+        "IspPlacements": List[IspPlacementTypeDef],
+        "Message": str,
+        "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DomainDeliverabilityTrackingOptionUnionTypeDef = Union[
-    DomainDeliverabilityTrackingOptionTypeDef, DomainDeliverabilityTrackingOptionOutputTypeDef
-]
 _RequiredCreateConfigurationSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConfigurationSetRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
     },
 )
 _OptionalCreateConfigurationSetRequestRequestTypeDef = TypedDict(
@@ -1198,28 +1202,30 @@
         "ReputationOptions": ReputationOptionsTypeDef,
         "SendingOptions": SendingOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateConfigurationSetRequestRequestTypeDef(
     _RequiredCreateConfigurationSetRequestRequestTypeDef,
     _OptionalCreateConfigurationSetRequestRequestTypeDef,
 ):
     pass
 
-ReputationOptionsUnionTypeDef = Union[ReputationOptionsTypeDef, ReputationOptionsOutputTypeDef]
-GetDeliverabilityTestReportResponseTypeDef = TypedDict(
-    "GetDeliverabilityTestReportResponseTypeDef",
+
+GetConfigurationSetResponseTypeDef = TypedDict(
+    "GetConfigurationSetResponseTypeDef",
     {
-        "DeliverabilityTestReport": DeliverabilityTestReportTypeDef,
-        "OverallPlacement": PlacementStatisticsTypeDef,
-        "IspPlacements": List[IspPlacementTypeDef],
-        "Message": str,
+        "ConfigurationSetName": str,
+        "TrackingOptions": TrackingOptionsTypeDef,
+        "DeliveryOptions": DeliveryOptionsTypeDef,
+        "ReputationOptions": ReputationOptionsTypeDef,
+        "SendingOptions": SendingOptionsTypeDef,
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EmailContentTypeDef = TypedDict(
     "EmailContentTypeDef",
@@ -1227,22 +1233,14 @@
         "Simple": MessageTypeDef,
         "Raw": RawMessageTypeDef,
         "Template": TemplateTypeDef,
     },
     total=False,
 )
 
-GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
-    "GetConfigurationSetEventDestinationsResponseTypeDef",
-    {
-        "EventDestinations": List[EventDestinationTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 CreateConfigurationSetEventDestinationRequestRequestTypeDef = TypedDict(
     "CreateConfigurationSetEventDestinationRequestRequestTypeDef",
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
@@ -1253,34 +1251,22 @@
     {
         "ConfigurationSetName": str,
         "EventDestinationName": str,
         "EventDestination": EventDestinationDefinitionTypeDef,
     },
 )
 
-_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef",
-    {
-        "DashboardEnabled": bool,
-    },
-)
-_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef = TypedDict(
-    "_OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef",
+GetConfigurationSetEventDestinationsResponseTypeDef = TypedDict(
+    "GetConfigurationSetEventDestinationsResponseTypeDef",
     {
-        "SubscribedDomains": Sequence[DomainDeliverabilityTrackingOptionUnionTypeDef],
+        "EventDestinations": List[EventDestinationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class PutDeliverabilityDashboardOptionRequestRequestTypeDef(
-    _RequiredPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-    _OptionalPutDeliverabilityDashboardOptionRequestRequestTypeDef,
-):
-    pass
-
 _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeliverabilityTestReportRequestRequestTypeDef",
     {
         "FromEmailAddress": str,
         "Content": EmailContentTypeDef,
     },
 )
@@ -1289,20 +1275,22 @@
     {
         "ReportName": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDeliverabilityTestReportRequestRequestTypeDef(
     _RequiredCreateDeliverabilityTestReportRequestRequestTypeDef,
     _OptionalCreateDeliverabilityTestReportRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredSendEmailRequestRequestTypeDef = TypedDict(
     "_RequiredSendEmailRequestRequestTypeDef",
     {
         "Destination": DestinationTypeDef,
         "Content": EmailContentTypeDef,
     },
 )
@@ -1314,11 +1302,12 @@
         "FeedbackForwardingEmailAddress": str,
         "EmailTags": Sequence[MessageTagTypeDef],
         "ConfigurationSetName": str,
     },
     total=False,
 )
 
+
 class SendEmailRequestRequestTypeDef(
     _RequiredSendEmailRequestRequestTypeDef, _OptionalSendEmailRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-pinpoint-email-2.5.2.post1/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt` & `types-aiobotocore-pinpoint-email-2.5.2.post2/types_aiobotocore_pinpoint_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

