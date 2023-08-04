# Comparing `tmp/types-aiobotocore-events-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-events-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-events-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-events-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:53 2023, max compression
```

## Comparing `types-aiobotocore-events-2.5.2.post1.tar` & `types-aiobotocore-events-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:17.153588 types-aiobotocore-events-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-08-02 14:52:17.153588 types-aiobotocore-events-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19038 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:17.153588 types-aiobotocore-events-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:17.153588 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40230 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40162 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65130 2023-08-02 14:38:37.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65050 2023-08-02 14:38:37.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:36.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:17.153588 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20557 2023-08-02 14:52:16.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:52:17.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:16.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:52:16.000000 types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.120168 types-aiobotocore-events-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:05.000000 types-aiobotocore-events-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-08-04 12:00:53.112168 types-aiobotocore-events-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-08-04 11:46:05.000000 types-aiobotocore-events-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:53.120168 types-aiobotocore-events-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-08-04 11:46:05.000000 types-aiobotocore-events-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.112168 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-08-04 11:46:05.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-04 11:46:05.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-04 11:46:05.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40210 2023-08-04 11:46:05.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40142 2023-08-04 11:46:05.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-08-04 11:46:06.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10204 2023-08-04 11:46:05.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-08-04 11:46:05.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-08-04 11:46:05.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:05.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    59024 2023-08-04 11:46:07.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58955 2023-08-04 11:46:06.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:05.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.112168 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-08-04 12:00:52.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-04 12:00:52.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:52.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-04 12:00:52.000000 types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-events-2.5.2.post1/LICENSE` & `types-aiobotocore-events-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post1/setup.py` & `types-aiobotocore-events-2.5.2.post2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-events",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_events"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EventBridge 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/__init__.py` & `types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/__init__.pyi` & `types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/__main__.py` & `types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EventBridge 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.EventBridge 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge\nOther"
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

### Comparing `types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/client.py` & `types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,20 +72,20 @@
     PutEventsRequestEntryTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutRuleResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
-    ReplayDestinationUnionTypeDef,
+    ReplayDestinationTypeDef,
     ReplicationConfigTypeDef,
     RoutingConfigTypeDef,
     StartReplayResponseTypeDef,
     TagTypeDef,
-    TargetUnionTypeDef,
+    TargetTypeDef,
     TestEventPatternResponseTypeDef,
     TimestampTypeDef,
     UpdateApiDestinationResponseTypeDef,
     UpdateArchiveResponseTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionResponseTypeDef,
     UpdateEndpointResponseTypeDef,
@@ -669,15 +669,15 @@
         Creates or updates the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#put_rule)
         """
 
     async def put_targets(
-        self, *, Rule: str, Targets: Sequence[TargetUnionTypeDef], EventBusName: str = ...
+        self, *, Rule: str, Targets: Sequence[TargetTypeDef], EventBusName: str = ...
     ) -> PutTargetsResponseTypeDef:
         """
         Adds the specified targets to the specified rule, or updates the targets if they
         are already associated with the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#put_targets)
@@ -707,15 +707,15 @@
     async def start_replay(
         self,
         *,
         ReplayName: str,
         EventSourceArn: str,
         EventStartTime: TimestampTypeDef,
         EventEndTime: TimestampTypeDef,
-        Destination: ReplayDestinationUnionTypeDef,
+        Destination: ReplayDestinationTypeDef,
         Description: str = ...
     ) -> StartReplayResponseTypeDef:
         """
         Starts the specified replay.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.start_replay)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#start_replay)
```

### Comparing `types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/client.pyi` & `types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -72,20 +72,20 @@
     PutEventsRequestEntryTypeDef,
     PutEventsResponseTypeDef,
     PutPartnerEventsRequestEntryTypeDef,
     PutPartnerEventsResponseTypeDef,
     PutRuleResponseTypeDef,
     PutTargetsResponseTypeDef,
     RemoveTargetsResponseTypeDef,
-    ReplayDestinationUnionTypeDef,
+    ReplayDestinationTypeDef,
     ReplicationConfigTypeDef,
     RoutingConfigTypeDef,
     StartReplayResponseTypeDef,
     TagTypeDef,
-    TargetUnionTypeDef,
+    TargetTypeDef,
     TestEventPatternResponseTypeDef,
     TimestampTypeDef,
     UpdateApiDestinationResponseTypeDef,
     UpdateArchiveResponseTypeDef,
     UpdateConnectionAuthRequestParametersTypeDef,
     UpdateConnectionResponseTypeDef,
     UpdateEndpointResponseTypeDef,
@@ -616,15 +616,15 @@
         """
         Creates or updates the specified rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#put_rule)
         """
     async def put_targets(
-        self, *, Rule: str, Targets: Sequence[TargetUnionTypeDef], EventBusName: str = ...
+        self, *, Rule: str, Targets: Sequence[TargetTypeDef], EventBusName: str = ...
     ) -> PutTargetsResponseTypeDef:
         """
         Adds the specified targets to the specified rule, or updates the targets if they
         are already associated with the rule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.put_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#put_targets)
@@ -651,15 +651,15 @@
     async def start_replay(
         self,
         *,
         ReplayName: str,
         EventSourceArn: str,
         EventStartTime: TimestampTypeDef,
         EventEndTime: TimestampTypeDef,
-        Destination: ReplayDestinationUnionTypeDef,
+        Destination: ReplayDestinationTypeDef,
         Description: str = ...
     ) -> StartReplayResponseTypeDef:
         """
         Starts the specified replay.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/events.html#EventBridge.Client.start_replay)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_events/client/#start_replay)
```

### Comparing `types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/literals.py` & `types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/literals.pyi` & `types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/paginator.py` & `types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/paginator.pyi` & `types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/type_defs.py` & `types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_events.type_defs import ActivateEventSourceRequestRequestTypeDef
 
     data: ActivateEventSourceRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ApiDestinationHttpMethodType,
     ApiDestinationStateType,
     ArchiveStateType,
     AssignPublicIpType,
     ConnectionAuthorizationTypeType,
@@ -43,15 +43,14 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ActivateEventSourceRequestRequestTypeDef",
     "ApiDestinationTypeDef",
     "ArchiveTypeDef",
-    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
     "BatchArrayPropertiesTypeDef",
     "BatchRetryStrategyTypeDef",
     "CancelReplayRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "ConditionTypeDef",
@@ -85,27 +84,25 @@
     "DescribeArchiveRequestRequestTypeDef",
     "DescribeConnectionRequestRequestTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
     "DescribeEventBusRequestRequestTypeDef",
     "DescribeEventSourceRequestRequestTypeDef",
     "DescribePartnerEventSourceRequestRequestTypeDef",
     "DescribeReplayRequestRequestTypeDef",
-    "ReplayDestinationOutputTypeDef",
+    "ReplayDestinationTypeDef",
     "DescribeRuleRequestRequestTypeDef",
     "DisableRuleRequestRequestTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "EnableRuleRequestRequestTypeDef",
     "EventBusTypeDef",
     "EventSourceTypeDef",
     "PrimaryTypeDef",
     "SecondaryTypeDef",
-    "HttpParametersOutputTypeDef",
     "HttpParametersTypeDef",
-    "InputTransformerOutputTypeDef",
     "InputTransformerTypeDef",
     "KinesisParametersTypeDef",
     "ListApiDestinationsRequestRequestTypeDef",
     "ListArchivesRequestRequestTypeDef",
     "ListConnectionsRequestRequestTypeDef",
     "ListEndpointsRequestRequestTypeDef",
     "ListEventBusesRequestRequestTypeDef",
@@ -122,33 +119,29 @@
     "RuleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTargetsByRuleRequestRequestTypeDef",
     "TimestampTypeDef",
     "PutEventsResultEntryTypeDef",
     "PutPartnerEventsResultEntryTypeDef",
     "PutTargetsResultEntryTypeDef",
-    "RedshiftDataParametersOutputTypeDef",
     "RedshiftDataParametersTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RemoveTargetsRequestRequestTypeDef",
     "RemoveTargetsResultEntryTypeDef",
-    "ReplayDestinationTypeDef",
     "RetryPolicyTypeDef",
-    "RunCommandTargetOutputTypeDef",
     "RunCommandTargetTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "SqsParametersTypeDef",
     "TestEventPatternRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiDestinationRequestRequestTypeDef",
     "UpdateArchiveRequestRequestTypeDef",
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     "UpdateConnectionBasicAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthClientRequestParametersTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "BatchParametersTypeDef",
     "CancelReplayResponseTypeDef",
     "CreateApiDestinationResponseTypeDef",
     "CreateArchiveResponseTypeDef",
     "CreateConnectionResponseTypeDef",
     "CreateEventBusResponseTypeDef",
@@ -168,15 +161,14 @@
     "PutRuleResponseTypeDef",
     "StartReplayResponseTypeDef",
     "TestEventPatternResponseTypeDef",
     "UpdateApiDestinationResponseTypeDef",
     "UpdateArchiveResponseTypeDef",
     "UpdateConnectionResponseTypeDef",
     "PutPermissionRequestRequestTypeDef",
-    "ConnectionHttpParametersOutputTypeDef",
     "ConnectionHttpParametersTypeDef",
     "ListConnectionsResponseTypeDef",
     "CreateEventBusRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutRuleRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DescribeReplayResponseTypeDef",
@@ -188,50 +180,44 @@
     "ListReplaysResponseTypeDef",
     "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListRulesResponseTypeDef",
     "PutEventsRequestEntryTypeDef",
     "PutPartnerEventsRequestEntryTypeDef",
+    "StartReplayRequestRequestTypeDef",
     "PutEventsResponseTypeDef",
     "PutPartnerEventsResponseTypeDef",
     "PutTargetsResponseTypeDef",
     "RemoveTargetsResponseTypeDef",
-    "ReplayDestinationUnionTypeDef",
-    "StartReplayRequestRequestTypeDef",
-    "RunCommandParametersOutputTypeDef",
     "RunCommandParametersTypeDef",
-    "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
-    "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ConnectionOAuthResponseParametersTypeDef",
     "CreateConnectionOAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthRequestParametersTypeDef",
     "RoutingConfigTypeDef",
     "PutEventsRequestRequestTypeDef",
     "PutPartnerEventsRequestRequestTypeDef",
-    "TargetOutputTypeDef",
     "TargetTypeDef",
     "ConnectionAuthResponseParametersTypeDef",
     "CreateConnectionAuthRequestParametersTypeDef",
     "UpdateConnectionAuthRequestParametersTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "CreateEndpointResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "EndpointTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
     "ListTargetsByRuleResponseTypeDef",
-    "TargetUnionTypeDef",
+    "PutTargetsRequestRequestTypeDef",
     "DescribeConnectionResponseTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "ListEndpointsResponseTypeDef",
-    "PutTargetsRequestRequestTypeDef",
 )
 
 ActivateEventSourceRequestRequestTypeDef = TypedDict(
     "ActivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -264,46 +250,24 @@
         "SizeBytes": int,
         "EventCount": int,
         "CreationTime": datetime,
     },
     total=False,
 )
 
-_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAwsVpcConfigurationOutputTypeDef",
-    {
-        "Subnets": List[str],
-    },
-)
-_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAwsVpcConfigurationOutputTypeDef",
-    {
-        "SecurityGroups": List[str],
-        "AssignPublicIp": AssignPublicIpType,
-    },
-    total=False,
-)
-
-
-class AwsVpcConfigurationOutputTypeDef(
-    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
-        "Subnets": Sequence[str],
+        "Subnets": List[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
     "_OptionalAwsVpcConfigurationTypeDef",
     {
-        "SecurityGroups": Sequence[str],
+        "SecurityGroups": List[str],
         "AssignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
 
 class AwsVpcConfigurationTypeDef(
@@ -705,31 +669,31 @@
 DescribeReplayRequestRequestTypeDef = TypedDict(
     "DescribeReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
 
-_RequiredReplayDestinationOutputTypeDef = TypedDict(
-    "_RequiredReplayDestinationOutputTypeDef",
+_RequiredReplayDestinationTypeDef = TypedDict(
+    "_RequiredReplayDestinationTypeDef",
     {
         "Arn": str,
     },
 )
-_OptionalReplayDestinationOutputTypeDef = TypedDict(
-    "_OptionalReplayDestinationOutputTypeDef",
+_OptionalReplayDestinationTypeDef = TypedDict(
+    "_OptionalReplayDestinationTypeDef",
     {
         "FilterArns": List[str],
     },
     total=False,
 )
 
 
-class ReplayDestinationOutputTypeDef(
-    _RequiredReplayDestinationOutputTypeDef, _OptionalReplayDestinationOutputTypeDef
+class ReplayDestinationTypeDef(
+    _RequiredReplayDestinationTypeDef, _OptionalReplayDestinationTypeDef
 ):
     pass
 
 
 _RequiredDescribeRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRuleRequestRequestTypeDef",
     {
@@ -844,65 +808,34 @@
 SecondaryTypeDef = TypedDict(
     "SecondaryTypeDef",
     {
         "Route": str,
     },
 )
 
-HttpParametersOutputTypeDef = TypedDict(
-    "HttpParametersOutputTypeDef",
+HttpParametersTypeDef = TypedDict(
+    "HttpParametersTypeDef",
     {
         "PathParameterValues": List[str],
         "HeaderParameters": Dict[str, str],
         "QueryStringParameters": Dict[str, str],
     },
     total=False,
 )
 
-HttpParametersTypeDef = TypedDict(
-    "HttpParametersTypeDef",
-    {
-        "PathParameterValues": Sequence[str],
-        "HeaderParameters": Mapping[str, str],
-        "QueryStringParameters": Mapping[str, str],
-    },
-    total=False,
-)
-
-_RequiredInputTransformerOutputTypeDef = TypedDict(
-    "_RequiredInputTransformerOutputTypeDef",
-    {
-        "InputTemplate": str,
-    },
-)
-_OptionalInputTransformerOutputTypeDef = TypedDict(
-    "_OptionalInputTransformerOutputTypeDef",
-    {
-        "InputPathsMap": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class InputTransformerOutputTypeDef(
-    _RequiredInputTransformerOutputTypeDef, _OptionalInputTransformerOutputTypeDef
-):
-    pass
-
-
 _RequiredInputTransformerTypeDef = TypedDict(
     "_RequiredInputTransformerTypeDef",
     {
         "InputTemplate": str,
     },
 )
 _OptionalInputTransformerTypeDef = TypedDict(
     "_OptionalInputTransformerTypeDef",
     {
-        "InputPathsMap": Mapping[str, str],
+        "InputPathsMap": Dict[str, str],
     },
     total=False,
 )
 
 
 class InputTransformerTypeDef(_RequiredInputTransformerTypeDef, _OptionalInputTransformerTypeDef):
     pass
@@ -1192,55 +1125,29 @@
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredRedshiftDataParametersOutputTypeDef = TypedDict(
-    "_RequiredRedshiftDataParametersOutputTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalRedshiftDataParametersOutputTypeDef = TypedDict(
-    "_OptionalRedshiftDataParametersOutputTypeDef",
-    {
-        "SecretManagerArn": str,
-        "DbUser": str,
-        "Sql": str,
-        "StatementName": str,
-        "WithEvent": bool,
-        "Sqls": List[str],
-    },
-    total=False,
-)
-
-
-class RedshiftDataParametersOutputTypeDef(
-    _RequiredRedshiftDataParametersOutputTypeDef, _OptionalRedshiftDataParametersOutputTypeDef
-):
-    pass
-
-
 _RequiredRedshiftDataParametersTypeDef = TypedDict(
     "_RequiredRedshiftDataParametersTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalRedshiftDataParametersTypeDef = TypedDict(
     "_OptionalRedshiftDataParametersTypeDef",
     {
         "SecretManagerArn": str,
         "DbUser": str,
         "Sql": str,
         "StatementName": str,
         "WithEvent": bool,
-        "Sqls": Sequence[str],
+        "Sqls": List[str],
     },
     total=False,
 )
 
 
 class RedshiftDataParametersTypeDef(
     _RequiredRedshiftDataParametersTypeDef, _OptionalRedshiftDataParametersTypeDef
@@ -1287,57 +1194,28 @@
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredReplayDestinationTypeDef = TypedDict(
-    "_RequiredReplayDestinationTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalReplayDestinationTypeDef = TypedDict(
-    "_OptionalReplayDestinationTypeDef",
-    {
-        "FilterArns": Sequence[str],
-    },
-    total=False,
-)
-
-
-class ReplayDestinationTypeDef(
-    _RequiredReplayDestinationTypeDef, _OptionalReplayDestinationTypeDef
-):
-    pass
-
-
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
     },
     total=False,
 )
 
-RunCommandTargetOutputTypeDef = TypedDict(
-    "RunCommandTargetOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-    },
-)
-
 RunCommandTargetTypeDef = TypedDict(
     "RunCommandTargetTypeDef",
     {
         "Key": str,
-        "Values": Sequence[str],
+        "Values": List[str],
     },
 )
 
 SageMakerPipelineParameterTypeDef = TypedDict(
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
@@ -1441,22 +1319,14 @@
     {
         "ClientID": str,
         "ClientSecret": str,
     },
     total=False,
 )
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
-    {
-        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
@@ -1753,24 +1623,14 @@
         "StatementId": str,
         "Condition": ConditionTypeDef,
         "Policy": str,
     },
     total=False,
 )
 
-ConnectionHttpParametersOutputTypeDef = TypedDict(
-    "ConnectionHttpParametersOutputTypeDef",
-    {
-        "HeaderParameters": List[ConnectionHeaderParameterTypeDef],
-        "QueryStringParameters": List[ConnectionQueryStringParameterTypeDef],
-        "BodyParameters": List[ConnectionBodyParameterTypeDef],
-    },
-    total=False,
-)
-
 ConnectionHttpParametersTypeDef = TypedDict(
     "ConnectionHttpParametersTypeDef",
     {
         "HeaderParameters": Sequence[ConnectionHeaderParameterTypeDef],
         "QueryStringParameters": Sequence[ConnectionQueryStringParameterTypeDef],
         "BodyParameters": Sequence[ConnectionBodyParameterTypeDef],
     },
@@ -1856,15 +1716,15 @@
     {
         "ReplayName": str,
         "ReplayArn": str,
         "Description": str,
         "State": ReplayStateType,
         "StateReason": str,
         "EventSourceArn": str,
-        "Destination": ReplayDestinationOutputTypeDef,
+        "Destination": ReplayDestinationTypeDef,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2010,51 +1870,14 @@
         "Resources": Sequence[str],
         "DetailType": str,
         "Detail": str,
     },
     total=False,
 )
 
-PutEventsResponseTypeDef = TypedDict(
-    "PutEventsResponseTypeDef",
-    {
-        "FailedEntryCount": int,
-        "Entries": List[PutEventsResultEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutPartnerEventsResponseTypeDef = TypedDict(
-    "PutPartnerEventsResponseTypeDef",
-    {
-        "FailedEntryCount": int,
-        "Entries": List[PutPartnerEventsResultEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-PutTargetsResponseTypeDef = TypedDict(
-    "PutTargetsResponseTypeDef",
-    {
-        "FailedEntryCount": int,
-        "FailedEntries": List[PutTargetsResultEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-RemoveTargetsResponseTypeDef = TypedDict(
-    "RemoveTargetsResponseTypeDef",
-    {
-        "FailedEntryCount": int,
-        "FailedEntries": List[RemoveTargetsResultEntryTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-ReplayDestinationUnionTypeDef = Union[ReplayDestinationTypeDef, ReplayDestinationOutputTypeDef]
 _RequiredStartReplayRequestRequestTypeDef = TypedDict(
     "_RequiredStartReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
         "EventSourceArn": str,
         "EventStartTime": TimestampTypeDef,
         "EventEndTime": TimestampTypeDef,
@@ -2072,99 +1895,87 @@
 
 class StartReplayRequestRequestTypeDef(
     _RequiredStartReplayRequestRequestTypeDef, _OptionalStartReplayRequestRequestTypeDef
 ):
     pass
 
 
-RunCommandParametersOutputTypeDef = TypedDict(
-    "RunCommandParametersOutputTypeDef",
+PutEventsResponseTypeDef = TypedDict(
+    "PutEventsResponseTypeDef",
     {
-        "RunCommandTargets": List[RunCommandTargetOutputTypeDef],
+        "FailedEntryCount": int,
+        "Entries": List[PutEventsResultEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RunCommandParametersTypeDef = TypedDict(
-    "RunCommandParametersTypeDef",
+PutPartnerEventsResponseTypeDef = TypedDict(
+    "PutPartnerEventsResponseTypeDef",
     {
-        "RunCommandTargets": Sequence[RunCommandTargetTypeDef],
+        "FailedEntryCount": int,
+        "Entries": List[PutPartnerEventsResultEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SageMakerPipelineParametersOutputTypeDef = TypedDict(
-    "SageMakerPipelineParametersOutputTypeDef",
+PutTargetsResponseTypeDef = TypedDict(
+    "PutTargetsResponseTypeDef",
     {
-        "PipelineParameterList": List[SageMakerPipelineParameterTypeDef],
+        "FailedEntryCount": int,
+        "FailedEntries": List[PutTargetsResultEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-SageMakerPipelineParametersTypeDef = TypedDict(
-    "SageMakerPipelineParametersTypeDef",
+RemoveTargetsResponseTypeDef = TypedDict(
+    "RemoveTargetsResponseTypeDef",
     {
-        "PipelineParameterList": Sequence[SageMakerPipelineParameterTypeDef],
+        "FailedEntryCount": int,
+        "FailedEntries": List[RemoveTargetsResultEntryTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-_RequiredEcsParametersOutputTypeDef = TypedDict(
-    "_RequiredEcsParametersOutputTypeDef",
+RunCommandParametersTypeDef = TypedDict(
+    "RunCommandParametersTypeDef",
     {
-        "TaskDefinitionArn": str,
+        "RunCommandTargets": List[RunCommandTargetTypeDef],
     },
 )
-_OptionalEcsParametersOutputTypeDef = TypedDict(
-    "_OptionalEcsParametersOutputTypeDef",
+
+SageMakerPipelineParametersTypeDef = TypedDict(
+    "SageMakerPipelineParametersTypeDef",
     {
-        "TaskCount": int,
-        "LaunchType": LaunchTypeType,
-        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
-        "PlatformVersion": str,
-        "Group": str,
-        "CapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "EnableECSManagedTags": bool,
-        "EnableExecuteCommand": bool,
-        "PlacementConstraints": List[PlacementConstraintTypeDef],
-        "PlacementStrategy": List[PlacementStrategyTypeDef],
-        "PropagateTags": Literal["TASK_DEFINITION"],
-        "ReferenceId": str,
-        "Tags": List[TagTypeDef],
+        "PipelineParameterList": List[SageMakerPipelineParameterTypeDef],
     },
     total=False,
 )
 
-
-class EcsParametersOutputTypeDef(
-    _RequiredEcsParametersOutputTypeDef, _OptionalEcsParametersOutputTypeDef
-):
-    pass
-
-
 _RequiredEcsParametersTypeDef = TypedDict(
     "_RequiredEcsParametersTypeDef",
     {
         "TaskDefinitionArn": str,
     },
 )
 _OptionalEcsParametersTypeDef = TypedDict(
     "_OptionalEcsParametersTypeDef",
     {
         "TaskCount": int,
         "LaunchType": LaunchTypeType,
         "NetworkConfiguration": NetworkConfigurationTypeDef,
         "PlatformVersion": str,
         "Group": str,
-        "CapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
+        "CapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "EnableECSManagedTags": bool,
         "EnableExecuteCommand": bool,
-        "PlacementConstraints": Sequence[PlacementConstraintTypeDef],
-        "PlacementStrategy": Sequence[PlacementStrategyTypeDef],
+        "PlacementConstraints": List[PlacementConstraintTypeDef],
+        "PlacementStrategy": List[PlacementStrategyTypeDef],
         "PropagateTags": Literal["TASK_DEFINITION"],
         "ReferenceId": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 
 class EcsParametersTypeDef(_RequiredEcsParametersTypeDef, _OptionalEcsParametersTypeDef):
     pass
@@ -2172,15 +1983,15 @@
 
 ConnectionOAuthResponseParametersTypeDef = TypedDict(
     "ConnectionOAuthResponseParametersTypeDef",
     {
         "ClientParameters": ConnectionOAuthClientResponseParametersTypeDef,
         "AuthorizationEndpoint": str,
         "HttpMethod": ConnectionOAuthHttpMethodType,
-        "OAuthHttpParameters": ConnectionHttpParametersOutputTypeDef,
+        "OAuthHttpParameters": ConnectionHttpParametersTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateConnectionOAuthRequestParametersTypeDef = TypedDict(
     "_RequiredCreateConnectionOAuthRequestParametersTypeDef",
     {
@@ -2247,47 +2058,14 @@
 PutPartnerEventsRequestRequestTypeDef = TypedDict(
     "PutPartnerEventsRequestRequestTypeDef",
     {
         "Entries": Sequence[PutPartnerEventsRequestEntryTypeDef],
     },
 )
 
-_RequiredTargetOutputTypeDef = TypedDict(
-    "_RequiredTargetOutputTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-    },
-)
-_OptionalTargetOutputTypeDef = TypedDict(
-    "_OptionalTargetOutputTypeDef",
-    {
-        "RoleArn": str,
-        "Input": str,
-        "InputPath": str,
-        "InputTransformer": InputTransformerOutputTypeDef,
-        "KinesisParameters": KinesisParametersTypeDef,
-        "RunCommandParameters": RunCommandParametersOutputTypeDef,
-        "EcsParameters": EcsParametersOutputTypeDef,
-        "BatchParameters": BatchParametersTypeDef,
-        "SqsParameters": SqsParametersTypeDef,
-        "HttpParameters": HttpParametersOutputTypeDef,
-        "RedshiftDataParameters": RedshiftDataParametersOutputTypeDef,
-        "SageMakerPipelineParameters": SageMakerPipelineParametersOutputTypeDef,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "RetryPolicy": RetryPolicyTypeDef,
-    },
-    total=False,
-)
-
-
-class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
-    pass
-
-
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
@@ -2319,15 +2097,15 @@
 
 ConnectionAuthResponseParametersTypeDef = TypedDict(
     "ConnectionAuthResponseParametersTypeDef",
     {
         "BasicAuthParameters": ConnectionBasicAuthResponseParametersTypeDef,
         "OAuthParameters": ConnectionOAuthResponseParametersTypeDef,
         "ApiKeyAuthParameters": ConnectionApiKeyAuthResponseParametersTypeDef,
-        "InvocationHttpParameters": ConnectionHttpParametersOutputTypeDef,
+        "InvocationHttpParameters": ConnectionHttpParametersTypeDef,
     },
     total=False,
 )
 
 CreateConnectionAuthRequestParametersTypeDef = TypedDict(
     "CreateConnectionAuthRequestParametersTypeDef",
     {
@@ -2469,21 +2247,42 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsByRuleResponseTypeDef = TypedDict(
     "ListTargetsByRuleResponseTypeDef",
     {
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
+_RequiredPutTargetsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutTargetsRequestRequestTypeDef",
+    {
+        "Rule": str,
+        "Targets": Sequence[TargetTypeDef],
+    },
+)
+_OptionalPutTargetsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutTargetsRequestRequestTypeDef",
+    {
+        "EventBusName": str,
+    },
+    total=False,
+)
+
+
+class PutTargetsRequestRequestTypeDef(
+    _RequiredPutTargetsRequestRequestTypeDef, _OptionalPutTargetsRequestRequestTypeDef
+):
+    pass
+
+
 DescribeConnectionResponseTypeDef = TypedDict(
     "DescribeConnectionResponseTypeDef",
     {
         "ConnectionArn": str,
         "Name": str,
         "Description": str,
         "ConnectionState": ConnectionStateType,
@@ -2548,28 +2347,7 @@
     "ListEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredPutTargetsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutTargetsRequestRequestTypeDef",
-    {
-        "Rule": str,
-        "Targets": Sequence[TargetUnionTypeDef],
-    },
-)
-_OptionalPutTargetsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutTargetsRequestRequestTypeDef",
-    {
-        "EventBusName": str,
-    },
-    total=False,
-)
-
-
-class PutTargetsRequestRequestTypeDef(
-    _RequiredPutTargetsRequestRequestTypeDef, _OptionalPutTargetsRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events/type_defs.pyi` & `types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_events.type_defs import ActivateEventSourceRequestRequestTypeDef
 
     data: ActivateEventSourceRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     ApiDestinationHttpMethodType,
     ApiDestinationStateType,
     ArchiveStateType,
     AssignPublicIpType,
     ConnectionAuthorizationTypeType,
@@ -42,15 +42,14 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActivateEventSourceRequestRequestTypeDef",
     "ApiDestinationTypeDef",
     "ArchiveTypeDef",
-    "AwsVpcConfigurationOutputTypeDef",
     "AwsVpcConfigurationTypeDef",
     "BatchArrayPropertiesTypeDef",
     "BatchRetryStrategyTypeDef",
     "CancelReplayRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CapacityProviderStrategyItemTypeDef",
     "ConditionTypeDef",
@@ -84,27 +83,25 @@
     "DescribeArchiveRequestRequestTypeDef",
     "DescribeConnectionRequestRequestTypeDef",
     "DescribeEndpointRequestRequestTypeDef",
     "DescribeEventBusRequestRequestTypeDef",
     "DescribeEventSourceRequestRequestTypeDef",
     "DescribePartnerEventSourceRequestRequestTypeDef",
     "DescribeReplayRequestRequestTypeDef",
-    "ReplayDestinationOutputTypeDef",
+    "ReplayDestinationTypeDef",
     "DescribeRuleRequestRequestTypeDef",
     "DisableRuleRequestRequestTypeDef",
     "PlacementConstraintTypeDef",
     "PlacementStrategyTypeDef",
     "EnableRuleRequestRequestTypeDef",
     "EventBusTypeDef",
     "EventSourceTypeDef",
     "PrimaryTypeDef",
     "SecondaryTypeDef",
-    "HttpParametersOutputTypeDef",
     "HttpParametersTypeDef",
-    "InputTransformerOutputTypeDef",
     "InputTransformerTypeDef",
     "KinesisParametersTypeDef",
     "ListApiDestinationsRequestRequestTypeDef",
     "ListArchivesRequestRequestTypeDef",
     "ListConnectionsRequestRequestTypeDef",
     "ListEndpointsRequestRequestTypeDef",
     "ListEventBusesRequestRequestTypeDef",
@@ -121,33 +118,29 @@
     "RuleTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTargetsByRuleRequestRequestTypeDef",
     "TimestampTypeDef",
     "PutEventsResultEntryTypeDef",
     "PutPartnerEventsResultEntryTypeDef",
     "PutTargetsResultEntryTypeDef",
-    "RedshiftDataParametersOutputTypeDef",
     "RedshiftDataParametersTypeDef",
     "RemovePermissionRequestRequestTypeDef",
     "RemoveTargetsRequestRequestTypeDef",
     "RemoveTargetsResultEntryTypeDef",
-    "ReplayDestinationTypeDef",
     "RetryPolicyTypeDef",
-    "RunCommandTargetOutputTypeDef",
     "RunCommandTargetTypeDef",
     "SageMakerPipelineParameterTypeDef",
     "SqsParametersTypeDef",
     "TestEventPatternRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiDestinationRequestRequestTypeDef",
     "UpdateArchiveRequestRequestTypeDef",
     "UpdateConnectionApiKeyAuthRequestParametersTypeDef",
     "UpdateConnectionBasicAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthClientRequestParametersTypeDef",
-    "NetworkConfigurationOutputTypeDef",
     "NetworkConfigurationTypeDef",
     "BatchParametersTypeDef",
     "CancelReplayResponseTypeDef",
     "CreateApiDestinationResponseTypeDef",
     "CreateArchiveResponseTypeDef",
     "CreateConnectionResponseTypeDef",
     "CreateEventBusResponseTypeDef",
@@ -167,15 +160,14 @@
     "PutRuleResponseTypeDef",
     "StartReplayResponseTypeDef",
     "TestEventPatternResponseTypeDef",
     "UpdateApiDestinationResponseTypeDef",
     "UpdateArchiveResponseTypeDef",
     "UpdateConnectionResponseTypeDef",
     "PutPermissionRequestRequestTypeDef",
-    "ConnectionHttpParametersOutputTypeDef",
     "ConnectionHttpParametersTypeDef",
     "ListConnectionsResponseTypeDef",
     "CreateEventBusRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutRuleRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DescribeReplayResponseTypeDef",
@@ -187,50 +179,44 @@
     "ListReplaysResponseTypeDef",
     "ListRuleNamesByTargetRequestListRuleNamesByTargetPaginateTypeDef",
     "ListRulesRequestListRulesPaginateTypeDef",
     "ListTargetsByRuleRequestListTargetsByRulePaginateTypeDef",
     "ListRulesResponseTypeDef",
     "PutEventsRequestEntryTypeDef",
     "PutPartnerEventsRequestEntryTypeDef",
+    "StartReplayRequestRequestTypeDef",
     "PutEventsResponseTypeDef",
     "PutPartnerEventsResponseTypeDef",
     "PutTargetsResponseTypeDef",
     "RemoveTargetsResponseTypeDef",
-    "ReplayDestinationUnionTypeDef",
-    "StartReplayRequestRequestTypeDef",
-    "RunCommandParametersOutputTypeDef",
     "RunCommandParametersTypeDef",
-    "SageMakerPipelineParametersOutputTypeDef",
     "SageMakerPipelineParametersTypeDef",
-    "EcsParametersOutputTypeDef",
     "EcsParametersTypeDef",
     "ConnectionOAuthResponseParametersTypeDef",
     "CreateConnectionOAuthRequestParametersTypeDef",
     "UpdateConnectionOAuthRequestParametersTypeDef",
     "RoutingConfigTypeDef",
     "PutEventsRequestRequestTypeDef",
     "PutPartnerEventsRequestRequestTypeDef",
-    "TargetOutputTypeDef",
     "TargetTypeDef",
     "ConnectionAuthResponseParametersTypeDef",
     "CreateConnectionAuthRequestParametersTypeDef",
     "UpdateConnectionAuthRequestParametersTypeDef",
     "CreateEndpointRequestRequestTypeDef",
     "CreateEndpointResponseTypeDef",
     "DescribeEndpointResponseTypeDef",
     "EndpointTypeDef",
     "UpdateEndpointRequestRequestTypeDef",
     "UpdateEndpointResponseTypeDef",
     "ListTargetsByRuleResponseTypeDef",
-    "TargetUnionTypeDef",
+    "PutTargetsRequestRequestTypeDef",
     "DescribeConnectionResponseTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "ListEndpointsResponseTypeDef",
-    "PutTargetsRequestRequestTypeDef",
 )
 
 ActivateEventSourceRequestRequestTypeDef = TypedDict(
     "ActivateEventSourceRequestRequestTypeDef",
     {
         "Name": str,
     },
@@ -263,44 +249,24 @@
         "SizeBytes": int,
         "EventCount": int,
         "CreationTime": datetime,
     },
     total=False,
 )
 
-_RequiredAwsVpcConfigurationOutputTypeDef = TypedDict(
-    "_RequiredAwsVpcConfigurationOutputTypeDef",
-    {
-        "Subnets": List[str],
-    },
-)
-_OptionalAwsVpcConfigurationOutputTypeDef = TypedDict(
-    "_OptionalAwsVpcConfigurationOutputTypeDef",
-    {
-        "SecurityGroups": List[str],
-        "AssignPublicIp": AssignPublicIpType,
-    },
-    total=False,
-)
-
-class AwsVpcConfigurationOutputTypeDef(
-    _RequiredAwsVpcConfigurationOutputTypeDef, _OptionalAwsVpcConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredAwsVpcConfigurationTypeDef = TypedDict(
     "_RequiredAwsVpcConfigurationTypeDef",
     {
-        "Subnets": Sequence[str],
+        "Subnets": List[str],
     },
 )
 _OptionalAwsVpcConfigurationTypeDef = TypedDict(
     "_OptionalAwsVpcConfigurationTypeDef",
     {
-        "SecurityGroups": Sequence[str],
+        "SecurityGroups": List[str],
         "AssignPublicIp": AssignPublicIpType,
     },
     total=False,
 )
 
 class AwsVpcConfigurationTypeDef(
     _RequiredAwsVpcConfigurationTypeDef, _OptionalAwsVpcConfigurationTypeDef
@@ -690,30 +656,30 @@
 DescribeReplayRequestRequestTypeDef = TypedDict(
     "DescribeReplayRequestRequestTypeDef",
     {
         "ReplayName": str,
     },
 )
 
-_RequiredReplayDestinationOutputTypeDef = TypedDict(
-    "_RequiredReplayDestinationOutputTypeDef",
+_RequiredReplayDestinationTypeDef = TypedDict(
+    "_RequiredReplayDestinationTypeDef",
     {
         "Arn": str,
     },
 )
-_OptionalReplayDestinationOutputTypeDef = TypedDict(
-    "_OptionalReplayDestinationOutputTypeDef",
+_OptionalReplayDestinationTypeDef = TypedDict(
+    "_OptionalReplayDestinationTypeDef",
     {
         "FilterArns": List[str],
     },
     total=False,
 )
 
-class ReplayDestinationOutputTypeDef(
-    _RequiredReplayDestinationOutputTypeDef, _OptionalReplayDestinationOutputTypeDef
+class ReplayDestinationTypeDef(
+    _RequiredReplayDestinationTypeDef, _OptionalReplayDestinationTypeDef
 ):
     pass
 
 _RequiredDescribeRuleRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRuleRequestRequestTypeDef",
     {
         "Name": str,
@@ -821,63 +787,34 @@
 SecondaryTypeDef = TypedDict(
     "SecondaryTypeDef",
     {
         "Route": str,
     },
 )
 
-HttpParametersOutputTypeDef = TypedDict(
-    "HttpParametersOutputTypeDef",
+HttpParametersTypeDef = TypedDict(
+    "HttpParametersTypeDef",
     {
         "PathParameterValues": List[str],
         "HeaderParameters": Dict[str, str],
         "QueryStringParameters": Dict[str, str],
     },
     total=False,
 )
 
-HttpParametersTypeDef = TypedDict(
-    "HttpParametersTypeDef",
-    {
-        "PathParameterValues": Sequence[str],
-        "HeaderParameters": Mapping[str, str],
-        "QueryStringParameters": Mapping[str, str],
-    },
-    total=False,
-)
-
-_RequiredInputTransformerOutputTypeDef = TypedDict(
-    "_RequiredInputTransformerOutputTypeDef",
-    {
-        "InputTemplate": str,
-    },
-)
-_OptionalInputTransformerOutputTypeDef = TypedDict(
-    "_OptionalInputTransformerOutputTypeDef",
-    {
-        "InputPathsMap": Dict[str, str],
-    },
-    total=False,
-)
-
-class InputTransformerOutputTypeDef(
-    _RequiredInputTransformerOutputTypeDef, _OptionalInputTransformerOutputTypeDef
-):
-    pass
-
 _RequiredInputTransformerTypeDef = TypedDict(
     "_RequiredInputTransformerTypeDef",
     {
         "InputTemplate": str,
     },
 )
 _OptionalInputTransformerTypeDef = TypedDict(
     "_OptionalInputTransformerTypeDef",
     {
-        "InputPathsMap": Mapping[str, str],
+        "InputPathsMap": Dict[str, str],
     },
     total=False,
 )
 
 class InputTransformerTypeDef(_RequiredInputTransformerTypeDef, _OptionalInputTransformerTypeDef):
     pass
 
@@ -1157,53 +1094,29 @@
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredRedshiftDataParametersOutputTypeDef = TypedDict(
-    "_RequiredRedshiftDataParametersOutputTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalRedshiftDataParametersOutputTypeDef = TypedDict(
-    "_OptionalRedshiftDataParametersOutputTypeDef",
-    {
-        "SecretManagerArn": str,
-        "DbUser": str,
-        "Sql": str,
-        "StatementName": str,
-        "WithEvent": bool,
-        "Sqls": List[str],
-    },
-    total=False,
-)
-
-class RedshiftDataParametersOutputTypeDef(
-    _RequiredRedshiftDataParametersOutputTypeDef, _OptionalRedshiftDataParametersOutputTypeDef
-):
-    pass
-
 _RequiredRedshiftDataParametersTypeDef = TypedDict(
     "_RequiredRedshiftDataParametersTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalRedshiftDataParametersTypeDef = TypedDict(
     "_OptionalRedshiftDataParametersTypeDef",
     {
         "SecretManagerArn": str,
         "DbUser": str,
         "Sql": str,
         "StatementName": str,
         "WithEvent": bool,
-        "Sqls": Sequence[str],
+        "Sqls": List[str],
     },
     total=False,
 )
 
 class RedshiftDataParametersTypeDef(
     _RequiredRedshiftDataParametersTypeDef, _OptionalRedshiftDataParametersTypeDef
 ):
@@ -1246,55 +1159,28 @@
         "TargetId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-_RequiredReplayDestinationTypeDef = TypedDict(
-    "_RequiredReplayDestinationTypeDef",
-    {
-        "Arn": str,
-    },
-)
-_OptionalReplayDestinationTypeDef = TypedDict(
-    "_OptionalReplayDestinationTypeDef",
-    {
-        "FilterArns": Sequence[str],
-    },
-    total=False,
-)
-
-class ReplayDestinationTypeDef(
-    _RequiredReplayDestinationTypeDef, _OptionalReplayDestinationTypeDef
-):
-    pass
-
 RetryPolicyTypeDef = TypedDict(
     "RetryPolicyTypeDef",
     {
         "MaximumRetryAttempts": int,
         "MaximumEventAgeInSeconds": int,
     },
     total=False,
 )
 
-RunCommandTargetOutputTypeDef = TypedDict(
-    "RunCommandTargetOutputTypeDef",
-    {
-        "Key": str,
-        "Values": List[str],
-    },
-)
-
 RunCommandTargetTypeDef = TypedDict(
     "RunCommandTargetTypeDef",
     {
         "Key": str,
-        "Values": Sequence[str],
+        "Values": List[str],
     },
 )
 
 SageMakerPipelineParameterTypeDef = TypedDict(
     "SageMakerPipelineParameterTypeDef",
     {
         "Name": str,
@@ -1394,22 +1280,14 @@
     {
         "ClientID": str,
         "ClientSecret": str,
     },
     total=False,
 )
 
-NetworkConfigurationOutputTypeDef = TypedDict(
-    "NetworkConfigurationOutputTypeDef",
-    {
-        "awsvpcConfiguration": AwsVpcConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "awsvpcConfiguration": AwsVpcConfigurationTypeDef,
     },
     total=False,
 )
@@ -1704,24 +1582,14 @@
         "StatementId": str,
         "Condition": ConditionTypeDef,
         "Policy": str,
     },
     total=False,
 )
 
-ConnectionHttpParametersOutputTypeDef = TypedDict(
-    "ConnectionHttpParametersOutputTypeDef",
-    {
-        "HeaderParameters": List[ConnectionHeaderParameterTypeDef],
-        "QueryStringParameters": List[ConnectionQueryStringParameterTypeDef],
-        "BodyParameters": List[ConnectionBodyParameterTypeDef],
-    },
-    total=False,
-)
-
 ConnectionHttpParametersTypeDef = TypedDict(
     "ConnectionHttpParametersTypeDef",
     {
         "HeaderParameters": Sequence[ConnectionHeaderParameterTypeDef],
         "QueryStringParameters": Sequence[ConnectionQueryStringParameterTypeDef],
         "BodyParameters": Sequence[ConnectionBodyParameterTypeDef],
     },
@@ -1803,15 +1671,15 @@
     {
         "ReplayName": str,
         "ReplayArn": str,
         "Description": str,
         "State": ReplayStateType,
         "StateReason": str,
         "EventSourceArn": str,
-        "Destination": ReplayDestinationOutputTypeDef,
+        "Destination": ReplayDestinationTypeDef,
         "EventStartTime": datetime,
         "EventEndTime": datetime,
         "EventLastReplayedTime": datetime,
         "ReplayStartTime": datetime,
         "ReplayEndTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1953,14 +1821,37 @@
         "Resources": Sequence[str],
         "DetailType": str,
         "Detail": str,
     },
     total=False,
 )
 
+_RequiredStartReplayRequestRequestTypeDef = TypedDict(
+    "_RequiredStartReplayRequestRequestTypeDef",
+    {
+        "ReplayName": str,
+        "EventSourceArn": str,
+        "EventStartTime": TimestampTypeDef,
+        "EventEndTime": TimestampTypeDef,
+        "Destination": ReplayDestinationTypeDef,
+    },
+)
+_OptionalStartReplayRequestRequestTypeDef = TypedDict(
+    "_OptionalStartReplayRequestRequestTypeDef",
+    {
+        "Description": str,
+    },
+    total=False,
+)
+
+class StartReplayRequestRequestTypeDef(
+    _RequiredStartReplayRequestRequestTypeDef, _OptionalStartReplayRequestRequestTypeDef
+):
+    pass
+
 PutEventsResponseTypeDef = TypedDict(
     "PutEventsResponseTypeDef",
     {
         "FailedEntryCount": int,
         "Entries": List[PutEventsResultEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1989,135 +1880,65 @@
     {
         "FailedEntryCount": int,
         "FailedEntries": List[RemoveTargetsResultEntryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReplayDestinationUnionTypeDef = Union[ReplayDestinationTypeDef, ReplayDestinationOutputTypeDef]
-_RequiredStartReplayRequestRequestTypeDef = TypedDict(
-    "_RequiredStartReplayRequestRequestTypeDef",
-    {
-        "ReplayName": str,
-        "EventSourceArn": str,
-        "EventStartTime": TimestampTypeDef,
-        "EventEndTime": TimestampTypeDef,
-        "Destination": ReplayDestinationTypeDef,
-    },
-)
-_OptionalStartReplayRequestRequestTypeDef = TypedDict(
-    "_OptionalStartReplayRequestRequestTypeDef",
-    {
-        "Description": str,
-    },
-    total=False,
-)
-
-class StartReplayRequestRequestTypeDef(
-    _RequiredStartReplayRequestRequestTypeDef, _OptionalStartReplayRequestRequestTypeDef
-):
-    pass
-
-RunCommandParametersOutputTypeDef = TypedDict(
-    "RunCommandParametersOutputTypeDef",
-    {
-        "RunCommandTargets": List[RunCommandTargetOutputTypeDef],
-    },
-)
-
 RunCommandParametersTypeDef = TypedDict(
     "RunCommandParametersTypeDef",
     {
-        "RunCommandTargets": Sequence[RunCommandTargetTypeDef],
+        "RunCommandTargets": List[RunCommandTargetTypeDef],
     },
 )
 
-SageMakerPipelineParametersOutputTypeDef = TypedDict(
-    "SageMakerPipelineParametersOutputTypeDef",
-    {
-        "PipelineParameterList": List[SageMakerPipelineParameterTypeDef],
-    },
-    total=False,
-)
-
 SageMakerPipelineParametersTypeDef = TypedDict(
     "SageMakerPipelineParametersTypeDef",
     {
-        "PipelineParameterList": Sequence[SageMakerPipelineParameterTypeDef],
-    },
-    total=False,
-)
-
-_RequiredEcsParametersOutputTypeDef = TypedDict(
-    "_RequiredEcsParametersOutputTypeDef",
-    {
-        "TaskDefinitionArn": str,
-    },
-)
-_OptionalEcsParametersOutputTypeDef = TypedDict(
-    "_OptionalEcsParametersOutputTypeDef",
-    {
-        "TaskCount": int,
-        "LaunchType": LaunchTypeType,
-        "NetworkConfiguration": NetworkConfigurationOutputTypeDef,
-        "PlatformVersion": str,
-        "Group": str,
-        "CapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
-        "EnableECSManagedTags": bool,
-        "EnableExecuteCommand": bool,
-        "PlacementConstraints": List[PlacementConstraintTypeDef],
-        "PlacementStrategy": List[PlacementStrategyTypeDef],
-        "PropagateTags": Literal["TASK_DEFINITION"],
-        "ReferenceId": str,
-        "Tags": List[TagTypeDef],
+        "PipelineParameterList": List[SageMakerPipelineParameterTypeDef],
     },
     total=False,
 )
 
-class EcsParametersOutputTypeDef(
-    _RequiredEcsParametersOutputTypeDef, _OptionalEcsParametersOutputTypeDef
-):
-    pass
-
 _RequiredEcsParametersTypeDef = TypedDict(
     "_RequiredEcsParametersTypeDef",
     {
         "TaskDefinitionArn": str,
     },
 )
 _OptionalEcsParametersTypeDef = TypedDict(
     "_OptionalEcsParametersTypeDef",
     {
         "TaskCount": int,
         "LaunchType": LaunchTypeType,
         "NetworkConfiguration": NetworkConfigurationTypeDef,
         "PlatformVersion": str,
         "Group": str,
-        "CapacityProviderStrategy": Sequence[CapacityProviderStrategyItemTypeDef],
+        "CapacityProviderStrategy": List[CapacityProviderStrategyItemTypeDef],
         "EnableECSManagedTags": bool,
         "EnableExecuteCommand": bool,
-        "PlacementConstraints": Sequence[PlacementConstraintTypeDef],
-        "PlacementStrategy": Sequence[PlacementStrategyTypeDef],
+        "PlacementConstraints": List[PlacementConstraintTypeDef],
+        "PlacementStrategy": List[PlacementStrategyTypeDef],
         "PropagateTags": Literal["TASK_DEFINITION"],
         "ReferenceId": str,
-        "Tags": Sequence[TagTypeDef],
+        "Tags": List[TagTypeDef],
     },
     total=False,
 )
 
 class EcsParametersTypeDef(_RequiredEcsParametersTypeDef, _OptionalEcsParametersTypeDef):
     pass
 
 ConnectionOAuthResponseParametersTypeDef = TypedDict(
     "ConnectionOAuthResponseParametersTypeDef",
     {
         "ClientParameters": ConnectionOAuthClientResponseParametersTypeDef,
         "AuthorizationEndpoint": str,
         "HttpMethod": ConnectionOAuthHttpMethodType,
-        "OAuthHttpParameters": ConnectionHttpParametersOutputTypeDef,
+        "OAuthHttpParameters": ConnectionHttpParametersTypeDef,
     },
     total=False,
 )
 
 _RequiredCreateConnectionOAuthRequestParametersTypeDef = TypedDict(
     "_RequiredCreateConnectionOAuthRequestParametersTypeDef",
     {
@@ -2180,45 +2001,14 @@
 PutPartnerEventsRequestRequestTypeDef = TypedDict(
     "PutPartnerEventsRequestRequestTypeDef",
     {
         "Entries": Sequence[PutPartnerEventsRequestEntryTypeDef],
     },
 )
 
-_RequiredTargetOutputTypeDef = TypedDict(
-    "_RequiredTargetOutputTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-    },
-)
-_OptionalTargetOutputTypeDef = TypedDict(
-    "_OptionalTargetOutputTypeDef",
-    {
-        "RoleArn": str,
-        "Input": str,
-        "InputPath": str,
-        "InputTransformer": InputTransformerOutputTypeDef,
-        "KinesisParameters": KinesisParametersTypeDef,
-        "RunCommandParameters": RunCommandParametersOutputTypeDef,
-        "EcsParameters": EcsParametersOutputTypeDef,
-        "BatchParameters": BatchParametersTypeDef,
-        "SqsParameters": SqsParametersTypeDef,
-        "HttpParameters": HttpParametersOutputTypeDef,
-        "RedshiftDataParameters": RedshiftDataParametersOutputTypeDef,
-        "SageMakerPipelineParameters": SageMakerPipelineParametersOutputTypeDef,
-        "DeadLetterConfig": DeadLetterConfigTypeDef,
-        "RetryPolicy": RetryPolicyTypeDef,
-    },
-    total=False,
-)
-
-class TargetOutputTypeDef(_RequiredTargetOutputTypeDef, _OptionalTargetOutputTypeDef):
-    pass
-
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "Id": str,
         "Arn": str,
     },
 )
@@ -2248,15 +2038,15 @@
 
 ConnectionAuthResponseParametersTypeDef = TypedDict(
     "ConnectionAuthResponseParametersTypeDef",
     {
         "BasicAuthParameters": ConnectionBasicAuthResponseParametersTypeDef,
         "OAuthParameters": ConnectionOAuthResponseParametersTypeDef,
         "ApiKeyAuthParameters": ConnectionApiKeyAuthResponseParametersTypeDef,
-        "InvocationHttpParameters": ConnectionHttpParametersOutputTypeDef,
+        "InvocationHttpParameters": ConnectionHttpParametersTypeDef,
     },
     total=False,
 )
 
 CreateConnectionAuthRequestParametersTypeDef = TypedDict(
     "CreateConnectionAuthRequestParametersTypeDef",
     {
@@ -2394,21 +2184,40 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsByRuleResponseTypeDef = TypedDict(
     "ListTargetsByRuleResponseTypeDef",
     {
-        "Targets": List[TargetOutputTypeDef],
+        "Targets": List[TargetTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TargetUnionTypeDef = Union[TargetTypeDef, TargetOutputTypeDef]
+_RequiredPutTargetsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutTargetsRequestRequestTypeDef",
+    {
+        "Rule": str,
+        "Targets": Sequence[TargetTypeDef],
+    },
+)
+_OptionalPutTargetsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutTargetsRequestRequestTypeDef",
+    {
+        "EventBusName": str,
+    },
+    total=False,
+)
+
+class PutTargetsRequestRequestTypeDef(
+    _RequiredPutTargetsRequestRequestTypeDef, _OptionalPutTargetsRequestRequestTypeDef
+):
+    pass
+
 DescribeConnectionResponseTypeDef = TypedDict(
     "DescribeConnectionResponseTypeDef",
     {
         "ConnectionArn": str,
         "Name": str,
         "Description": str,
         "ConnectionState": ConnectionStateType,
@@ -2469,27 +2278,7 @@
     "ListEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredPutTargetsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutTargetsRequestRequestTypeDef",
-    {
-        "Rule": str,
-        "Targets": Sequence[TargetUnionTypeDef],
-    },
-)
-_OptionalPutTargetsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutTargetsRequestRequestTypeDef",
-    {
-        "EventBusName": str,
-    },
-    total=False,
-)
-
-class PutTargetsRequestRequestTypeDef(
-    _RequiredPutTargetsRequestRequestTypeDef, _OptionalPutTargetsRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-events-2.5.2.post1/types_aiobotocore_events.egg-info/SOURCES.txt` & `types-aiobotocore-events-2.5.2.post2/types_aiobotocore_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

