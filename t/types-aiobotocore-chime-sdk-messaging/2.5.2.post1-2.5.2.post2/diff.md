# Comparing `tmp/types-aiobotocore-chime-sdk-messaging-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-chime-sdk-messaging-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-sdk-messaging-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-sdk-messaging-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:31 2023, max compression
```

## Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post1.tar` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.801642 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-08-02 14:51:57.801642 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.801642 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.793642 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40498 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    40439 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48005 2023-08-02 14:34:12.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    47948 2023-08-02 14:34:12.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:11.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.801642 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:31.195334 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-08-04 12:00:31.191334 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11286 2023-08-04 11:41:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:31.195334 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-08-04 11:41:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:31.191334 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-04 11:41:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-04 11:41:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-04 11:41:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40488 2023-08-04 11:41:24.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40429 2023-08-04 11:41:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9351 2023-08-04 11:41:24.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9349 2023-08-04 11:41:24.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    47633 2023-08-04 11:41:25.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47576 2023-08-04 11:41:25.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:23.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:31.191334 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12850 2023-08-04 12:00:31.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-08-04 12:00:31.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:31.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:31.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:31.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:31.000000 types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/LICENSE` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/setup.py` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime-sdk-messaging",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_chime_sdk_messaging"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ChimeSDKMessaging 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/__init__.py` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/__init__.pyi` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/__main__.py` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ChimeSDKMessaging 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime_sdk_messaging//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime-sdk-messaging.html#ChimeSDKMessaging\nOther"
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

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/client.py` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     ListChannelMessagesResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsResponseTypeDef,
     ListSubChannelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MessageAttributeValueUnionTypeDef,
+    MessageAttributeValueTypeDef,
     ProcessorTypeDef,
     PushNotificationConfigurationTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     RedactChannelMessageResponseTypeDef,
     SearchChannelsResponseTypeDef,
@@ -688,15 +688,15 @@
         Content: str,
         Type: ChannelMessageTypeType,
         Persistence: ChannelMessagePersistenceTypeType,
         ClientRequestToken: str,
         ChimeBearer: str,
         Metadata: str = ...,
         PushNotification: PushNotificationConfigurationTypeDef = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueUnionTypeDef] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         SubChannelId: str = ...,
         ContentType: str = ...,
         Target: Sequence[TargetTypeDef] = ...
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/client.pyi` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     ListChannelMessagesResponseTypeDef,
     ListChannelModeratorsResponseTypeDef,
     ListChannelsAssociatedWithChannelFlowResponseTypeDef,
     ListChannelsModeratedByAppInstanceUserResponseTypeDef,
     ListChannelsResponseTypeDef,
     ListSubChannelsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MessageAttributeValueUnionTypeDef,
+    MessageAttributeValueTypeDef,
     ProcessorTypeDef,
     PushNotificationConfigurationTypeDef,
     PutChannelExpirationSettingsResponseTypeDef,
     PutChannelMembershipPreferencesResponseTypeDef,
     PutMessagingStreamingConfigurationsResponseTypeDef,
     RedactChannelMessageResponseTypeDef,
     SearchChannelsResponseTypeDef,
@@ -637,15 +637,15 @@
         Content: str,
         Type: ChannelMessageTypeType,
         Persistence: ChannelMessagePersistenceTypeType,
         ClientRequestToken: str,
         ChimeBearer: str,
         Metadata: str = ...,
         PushNotification: PushNotificationConfigurationTypeDef = ...,
-        MessageAttributes: Mapping[str, MessageAttributeValueUnionTypeDef] = ...,
+        MessageAttributes: Mapping[str, MessageAttributeValueTypeDef] = ...,
         SubChannelId: str = ...,
         ContentType: str = ...,
         Target: Sequence[TargetTypeDef] = ...
     ) -> SendChannelMessageResponseTypeDef:
         """
         Sends a message to a particular channel that the member is a part of.
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/literals.py` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/literals.pyi` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/type_defs.py` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,14 @@
     "ResponseMetadataTypeDef",
     "ChannelAssociatedWithFlowSummaryTypeDef",
     "ChannelSummaryTypeDef",
     "PushNotificationPreferencesTypeDef",
     "MessageAttributeValueTypeDef",
     "PushNotificationConfigurationTypeDef",
     "ChannelMessageStatusStructureTypeDef",
-    "MessageAttributeValueOutputTypeDef",
     "TargetTypeDef",
     "ElasticChannelConfigurationTypeDef",
     "ExpirationSettingsTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "TagTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
@@ -127,17 +126,17 @@
     "ListChannelsResponseTypeDef",
     "SearchChannelsResponseTypeDef",
     "ChannelMembershipPreferencesTypeDef",
     "ChannelMessageCallbackTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
-    "MessageAttributeValueUnionTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
+    "SendChannelMessageRequestRequestTypeDef",
     "ChannelTypeDef",
     "PutChannelExpirationSettingsRequestRequestTypeDef",
     "PutChannelExpirationSettingsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
@@ -159,15 +158,14 @@
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "GetChannelMembershipPreferencesResponseTypeDef",
     "PutChannelMembershipPreferencesRequestRequestTypeDef",
     "PutChannelMembershipPreferencesResponseTypeDef",
     "ChannelFlowCallbackRequestRequestTypeDef",
-    "SendChannelMessageRequestRequestTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "ProcessorTypeDef",
     "ChannelFlowSummaryTypeDef",
     "ChannelFlowTypeDef",
     "CreateChannelFlowRequestRequestTypeDef",
@@ -319,22 +317,14 @@
     {
         "Value": ChannelMessageStatusType,
         "Detail": str,
     },
     total=False,
 )
 
-MessageAttributeValueOutputTypeDef = TypedDict(
-    "MessageAttributeValueOutputTypeDef",
-    {
-        "StringValues": List[str],
-    },
-    total=False,
-)
-
 TargetTypeDef = TypedDict(
     "TargetTypeDef",
     {
         "MemberArn": str,
     },
     total=False,
 )
@@ -1266,31 +1256,28 @@
         "MessageId": str,
         "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MessageAttributeValueUnionTypeDef = Union[
-    MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef
-]
 ChannelMessageSummaryTypeDef = TypedDict(
     "ChannelMessageSummaryTypeDef",
     {
         "MessageId": str,
         "Content": str,
         "Metadata": str,
         "Type": ChannelMessageTypeType,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Status": ChannelMessageStatusStructureTypeDef,
-        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
         "ContentType": str,
         "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
 ChannelMessageTypeDef = TypedDict(
@@ -1304,22 +1291,54 @@
         "CreatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Persistence": ChannelMessagePersistenceTypeType,
         "Status": ChannelMessageStatusStructureTypeDef,
-        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
         "ContentType": str,
         "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
+_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_RequiredSendChannelMessageRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "Content": str,
+        "Type": ChannelMessageTypeType,
+        "Persistence": ChannelMessagePersistenceTypeType,
+        "ClientRequestToken": str,
+        "ChimeBearer": str,
+    },
+)
+_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_OptionalSendChannelMessageRequestRequestTypeDef",
+    {
+        "Metadata": str,
+        "PushNotification": PushNotificationConfigurationTypeDef,
+        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
+        "SubChannelId": str,
+        "ContentType": str,
+        "Target": Sequence[TargetTypeDef],
+    },
+    total=False,
+)
+
+
+class SendChannelMessageRequestRequestTypeDef(
+    _RequiredSendChannelMessageRequestRequestTypeDef,
+    _OptionalSendChannelMessageRequestRequestTypeDef,
+):
+    pass
+
+
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -1662,46 +1681,14 @@
 class ChannelFlowCallbackRequestRequestTypeDef(
     _RequiredChannelFlowCallbackRequestRequestTypeDef,
     _OptionalChannelFlowCallbackRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_RequiredSendChannelMessageRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "Content": str,
-        "Type": ChannelMessageTypeType,
-        "Persistence": ChannelMessagePersistenceTypeType,
-        "ClientRequestToken": str,
-        "ChimeBearer": str,
-    },
-)
-_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_OptionalSendChannelMessageRequestRequestTypeDef",
-    {
-        "Metadata": str,
-        "PushNotification": PushNotificationConfigurationTypeDef,
-        "MessageAttributes": Mapping[str, MessageAttributeValueUnionTypeDef],
-        "SubChannelId": str,
-        "ContentType": str,
-        "Target": Sequence[TargetTypeDef],
-    },
-    total=False,
-)
-
-
-class SendChannelMessageRequestRequestTypeDef(
-    _RequiredSendChannelMessageRequestRequestTypeDef,
-    _OptionalSendChannelMessageRequestRequestTypeDef,
-):
-    pass
-
-
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
         "SubChannelId": str,
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging/type_defs.pyi` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     "ResponseMetadataTypeDef",
     "ChannelAssociatedWithFlowSummaryTypeDef",
     "ChannelSummaryTypeDef",
     "PushNotificationPreferencesTypeDef",
     "MessageAttributeValueTypeDef",
     "PushNotificationConfigurationTypeDef",
     "ChannelMessageStatusStructureTypeDef",
-    "MessageAttributeValueOutputTypeDef",
     "TargetTypeDef",
     "ElasticChannelConfigurationTypeDef",
     "ExpirationSettingsTypeDef",
     "CreateChannelBanRequestRequestTypeDef",
     "TagTypeDef",
     "CreateChannelMembershipRequestRequestTypeDef",
     "CreateChannelModeratorRequestRequestTypeDef",
@@ -126,17 +125,17 @@
     "ListChannelsResponseTypeDef",
     "SearchChannelsResponseTypeDef",
     "ChannelMembershipPreferencesTypeDef",
     "ChannelMessageCallbackTypeDef",
     "GetChannelMessageStatusResponseTypeDef",
     "SendChannelMessageResponseTypeDef",
     "UpdateChannelMessageResponseTypeDef",
-    "MessageAttributeValueUnionTypeDef",
     "ChannelMessageSummaryTypeDef",
     "ChannelMessageTypeDef",
+    "SendChannelMessageRequestRequestTypeDef",
     "ChannelTypeDef",
     "PutChannelExpirationSettingsRequestRequestTypeDef",
     "PutChannelExpirationSettingsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
@@ -158,15 +157,14 @@
     "ListChannelMembershipsForAppInstanceUserResponseTypeDef",
     "DescribeChannelModeratedByAppInstanceUserResponseTypeDef",
     "ListChannelsModeratedByAppInstanceUserResponseTypeDef",
     "GetChannelMembershipPreferencesResponseTypeDef",
     "PutChannelMembershipPreferencesRequestRequestTypeDef",
     "PutChannelMembershipPreferencesResponseTypeDef",
     "ChannelFlowCallbackRequestRequestTypeDef",
-    "SendChannelMessageRequestRequestTypeDef",
     "ListChannelMessagesResponseTypeDef",
     "GetChannelMessageResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "ProcessorTypeDef",
     "ChannelFlowSummaryTypeDef",
     "ChannelFlowTypeDef",
     "CreateChannelFlowRequestRequestTypeDef",
@@ -314,22 +312,14 @@
     {
         "Value": ChannelMessageStatusType,
         "Detail": str,
     },
     total=False,
 )
 
-MessageAttributeValueOutputTypeDef = TypedDict(
-    "MessageAttributeValueOutputTypeDef",
-    {
-        "StringValues": List[str],
-    },
-    total=False,
-)
-
 TargetTypeDef = TypedDict(
     "TargetTypeDef",
     {
         "MemberArn": str,
     },
     total=False,
 )
@@ -1223,31 +1213,28 @@
         "MessageId": str,
         "Status": ChannelMessageStatusStructureTypeDef,
         "SubChannelId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-MessageAttributeValueUnionTypeDef = Union[
-    MessageAttributeValueTypeDef, MessageAttributeValueOutputTypeDef
-]
 ChannelMessageSummaryTypeDef = TypedDict(
     "ChannelMessageSummaryTypeDef",
     {
         "MessageId": str,
         "Content": str,
         "Metadata": str,
         "Type": ChannelMessageTypeType,
         "CreatedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Status": ChannelMessageStatusStructureTypeDef,
-        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
         "ContentType": str,
         "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
 ChannelMessageTypeDef = TypedDict(
@@ -1261,22 +1248,52 @@
         "CreatedTimestamp": datetime,
         "LastEditedTimestamp": datetime,
         "LastUpdatedTimestamp": datetime,
         "Sender": IdentityTypeDef,
         "Redacted": bool,
         "Persistence": ChannelMessagePersistenceTypeType,
         "Status": ChannelMessageStatusStructureTypeDef,
-        "MessageAttributes": Dict[str, MessageAttributeValueOutputTypeDef],
+        "MessageAttributes": Dict[str, MessageAttributeValueTypeDef],
         "SubChannelId": str,
         "ContentType": str,
         "Target": List[TargetTypeDef],
     },
     total=False,
 )
 
+_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_RequiredSendChannelMessageRequestRequestTypeDef",
+    {
+        "ChannelArn": str,
+        "Content": str,
+        "Type": ChannelMessageTypeType,
+        "Persistence": ChannelMessagePersistenceTypeType,
+        "ClientRequestToken": str,
+        "ChimeBearer": str,
+    },
+)
+_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
+    "_OptionalSendChannelMessageRequestRequestTypeDef",
+    {
+        "Metadata": str,
+        "PushNotification": PushNotificationConfigurationTypeDef,
+        "MessageAttributes": Mapping[str, MessageAttributeValueTypeDef],
+        "SubChannelId": str,
+        "ContentType": str,
+        "Target": Sequence[TargetTypeDef],
+    },
+    total=False,
+)
+
+class SendChannelMessageRequestRequestTypeDef(
+    _RequiredSendChannelMessageRequestRequestTypeDef,
+    _OptionalSendChannelMessageRequestRequestTypeDef,
+):
+    pass
+
 ChannelTypeDef = TypedDict(
     "ChannelTypeDef",
     {
         "Name": str,
         "ChannelArn": str,
         "Mode": ChannelModeType,
         "Privacy": ChannelPrivacyType,
@@ -1609,44 +1626,14 @@
 
 class ChannelFlowCallbackRequestRequestTypeDef(
     _RequiredChannelFlowCallbackRequestRequestTypeDef,
     _OptionalChannelFlowCallbackRequestRequestTypeDef,
 ):
     pass
 
-_RequiredSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_RequiredSendChannelMessageRequestRequestTypeDef",
-    {
-        "ChannelArn": str,
-        "Content": str,
-        "Type": ChannelMessageTypeType,
-        "Persistence": ChannelMessagePersistenceTypeType,
-        "ClientRequestToken": str,
-        "ChimeBearer": str,
-    },
-)
-_OptionalSendChannelMessageRequestRequestTypeDef = TypedDict(
-    "_OptionalSendChannelMessageRequestRequestTypeDef",
-    {
-        "Metadata": str,
-        "PushNotification": PushNotificationConfigurationTypeDef,
-        "MessageAttributes": Mapping[str, MessageAttributeValueUnionTypeDef],
-        "SubChannelId": str,
-        "ContentType": str,
-        "Target": Sequence[TargetTypeDef],
-    },
-    total=False,
-)
-
-class SendChannelMessageRequestRequestTypeDef(
-    _RequiredSendChannelMessageRequestRequestTypeDef,
-    _OptionalSendChannelMessageRequestRequestTypeDef,
-):
-    pass
-
 ListChannelMessagesResponseTypeDef = TypedDict(
     "ListChannelMessagesResponseTypeDef",
     {
         "ChannelArn": str,
         "NextToken": str,
         "ChannelMessages": List[ChannelMessageSummaryTypeDef],
         "SubChannelId": str,
```

### Comparing `types-aiobotocore-chime-sdk-messaging-2.5.2.post1/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt` & `types-aiobotocore-chime-sdk-messaging-2.5.2.post2/types_aiobotocore_chime_sdk_messaging.egg-info/SOURCES.txt`

 * *Files identical despite different names*

