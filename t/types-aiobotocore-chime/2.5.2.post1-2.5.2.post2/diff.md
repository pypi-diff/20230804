# Comparing `tmp/types-aiobotocore-chime-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-chime-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-chime-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-chime-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:30 2023, max compression
```

## Comparing `types-aiobotocore-chime-2.5.2.post1.tar` & `types-aiobotocore-chime-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.553643 types-aiobotocore-chime-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    33302 2023-08-02 14:51:57.549643 types-aiobotocore-chime-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    31792 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.553643 types-aiobotocore-chime-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.545642 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)   127555 2023-08-02 14:34:01.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)   127353 2023-08-02 14:34:01.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-08-02 14:34:01.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-08-02 14:34:01.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-08-02 14:34:01.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-08-02 14:34:01.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   147475 2023-08-02 14:34:05.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   147314 2023-08-02 14:34:03.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:00.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.549643 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    33302 2023-08-02 14:51:57.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 14:51:57.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:51:57.000000 types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.975326 types-aiobotocore-chime-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:12.000000 types-aiobotocore-chime-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-08-04 12:00:30.975326 types-aiobotocore-chime-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11363 2023-08-04 11:41:12.000000 types-aiobotocore-chime-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:30.975326 types-aiobotocore-chime-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-04 11:41:12.000000 types-aiobotocore-chime-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.975326 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-08-04 11:41:12.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-04 11:41:12.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-04 11:41:12.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127505 2023-08-04 11:41:14.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)   127303 2023-08-04 11:41:13.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13503 2023-08-04 11:41:14.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-08-04 11:41:14.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-08-04 11:41:14.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-08-04 11:41:14.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:12.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   144510 2023-08-04 11:41:18.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144351 2023-08-04 11:41:16.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:12.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:30.975326 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12873 2023-08-04 12:00:30.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-04 12:00:30.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:30.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:30.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-04 12:00:30.000000 types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-chime-2.5.2.post1/LICENSE` & `types-aiobotocore-chime-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post1/setup.py` & `types-aiobotocore-chime-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-chime",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_chime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Chime 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/__init__.py` & `types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/__init__.pyi` & `types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/__main__.py` & `types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Chime 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.Chime 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime\nOther"
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

### Comparing `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/client.py` & `types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     BatchCreateRoomMembershipResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
     BatchUnsuspendUserResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     BatchUpdateUserResponseTypeDef,
     BusinessCallingSettingsTypeDef,
-    ChimeSdkMeetingConfigurationUnionTypeDef,
+    ChimeSdkMeetingConfigurationTypeDef,
     CreateAccountResponseTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeResponseTypeDef,
     CreateBotResponseTypeDef,
@@ -92,15 +92,15 @@
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmergencyCallingConfigurationUnionTypeDef,
+    EmergencyCallingConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetAccountResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     GetAppInstanceStreamingConfigurationsResponseTypeDef,
     GetAttendeeResponseTypeDef,
@@ -161,15 +161,15 @@
     ListUsersResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     LoggingConfigurationTypeDef,
     MeetingNotificationConfigurationTypeDef,
     MembershipItemTypeDef,
-    OriginationUnionTypeDef,
+    OriginationTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     PutRetentionSettingsResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
@@ -184,17 +184,17 @@
     RetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     SigninDelegateGroupTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
-    StreamingConfigurationUnionTypeDef,
+    StreamingConfigurationTypeDef,
     TagTypeDef,
-    TerminationUnionTypeDef,
+    TerminationTypeDef,
     TimestampTypeDef,
     TranscriptionConfigurationTypeDef,
     UpdateAccountResponseTypeDef,
     UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserResponseTypeDef,
     UpdateBotResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
@@ -543,15 +543,15 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationUnionTypeDef = ...
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media capture pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_media_capture_pipeline)
         """
@@ -1920,15 +1920,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_sip_media_application_logging_configuration)
         """
 
     async def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
-        EmergencyCallingConfiguration: EmergencyCallingConfigurationUnionTypeDef
+        EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
         Puts emergency calling configuration details to the specified Amazon Chime Voice
         Connector, such as emergency phone numbers and calling countries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_emergency_calling_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_emergency_calling_configuration)
@@ -1941,15 +1941,15 @@
         Adds a logging configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_logging_configuration)
         """
 
     async def put_voice_connector_origination(
-        self, *, VoiceConnectorId: str, Origination: OriginationUnionTypeDef
+        self, *, VoiceConnectorId: str, Origination: OriginationTypeDef
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
         Adds origination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_origination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_origination)
         """
@@ -1968,25 +1968,25 @@
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_proxy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_proxy)
         """
 
     async def put_voice_connector_streaming_configuration(
-        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationUnionTypeDef
+        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationTypeDef
     ) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
         Adds a streaming configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_streaming_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_streaming_configuration)
         """
 
     async def put_voice_connector_termination(
-        self, *, VoiceConnectorId: str, Termination: TerminationUnionTypeDef
+        self, *, VoiceConnectorId: str, Termination: TerminationTypeDef
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
         Adds termination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_termination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_termination)
         """
```

### Comparing `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/client.pyi` & `types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     BatchCreateRoomMembershipResponseTypeDef,
     BatchDeletePhoneNumberResponseTypeDef,
     BatchSuspendUserResponseTypeDef,
     BatchUnsuspendUserResponseTypeDef,
     BatchUpdatePhoneNumberResponseTypeDef,
     BatchUpdateUserResponseTypeDef,
     BusinessCallingSettingsTypeDef,
-    ChimeSdkMeetingConfigurationUnionTypeDef,
+    ChimeSdkMeetingConfigurationTypeDef,
     CreateAccountResponseTypeDef,
     CreateAppInstanceAdminResponseTypeDef,
     CreateAppInstanceResponseTypeDef,
     CreateAppInstanceUserResponseTypeDef,
     CreateAttendeeRequestItemTypeDef,
     CreateAttendeeResponseTypeDef,
     CreateBotResponseTypeDef,
@@ -92,15 +92,15 @@
     DescribeChannelMembershipForAppInstanceUserResponseTypeDef,
     DescribeChannelMembershipResponseTypeDef,
     DescribeChannelModeratedByAppInstanceUserResponseTypeDef,
     DescribeChannelModeratorResponseTypeDef,
     DescribeChannelResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorGroupResponseTypeDef,
     DisassociatePhoneNumbersFromVoiceConnectorResponseTypeDef,
-    EmergencyCallingConfigurationUnionTypeDef,
+    EmergencyCallingConfigurationTypeDef,
     EmptyResponseMetadataTypeDef,
     GeoMatchParamsTypeDef,
     GetAccountResponseTypeDef,
     GetAccountSettingsResponseTypeDef,
     GetAppInstanceRetentionSettingsResponseTypeDef,
     GetAppInstanceStreamingConfigurationsResponseTypeDef,
     GetAttendeeResponseTypeDef,
@@ -161,15 +161,15 @@
     ListUsersResponseTypeDef,
     ListVoiceConnectorGroupsResponseTypeDef,
     ListVoiceConnectorsResponseTypeDef,
     ListVoiceConnectorTerminationCredentialsResponseTypeDef,
     LoggingConfigurationTypeDef,
     MeetingNotificationConfigurationTypeDef,
     MembershipItemTypeDef,
-    OriginationUnionTypeDef,
+    OriginationTypeDef,
     PutAppInstanceRetentionSettingsResponseTypeDef,
     PutAppInstanceStreamingConfigurationsResponseTypeDef,
     PutEventsConfigurationResponseTypeDef,
     PutRetentionSettingsResponseTypeDef,
     PutSipMediaApplicationLoggingConfigurationResponseTypeDef,
     PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef,
     PutVoiceConnectorLoggingConfigurationResponseTypeDef,
@@ -184,17 +184,17 @@
     RetentionSettingsTypeDef,
     SearchAvailablePhoneNumbersResponseTypeDef,
     SendChannelMessageResponseTypeDef,
     SigninDelegateGroupTypeDef,
     SipMediaApplicationEndpointTypeDef,
     SipMediaApplicationLoggingConfigurationTypeDef,
     SipRuleTargetApplicationTypeDef,
-    StreamingConfigurationUnionTypeDef,
+    StreamingConfigurationTypeDef,
     TagTypeDef,
-    TerminationUnionTypeDef,
+    TerminationTypeDef,
     TimestampTypeDef,
     TranscriptionConfigurationTypeDef,
     UpdateAccountResponseTypeDef,
     UpdateAppInstanceResponseTypeDef,
     UpdateAppInstanceUserResponseTypeDef,
     UpdateBotResponseTypeDef,
     UpdateChannelMessageResponseTypeDef,
@@ -514,15 +514,15 @@
         self,
         *,
         SourceType: Literal["ChimeSdkMeeting"],
         SourceArn: str,
         SinkType: Literal["S3Bucket"],
         SinkArn: str,
         ClientRequestToken: str = ...,
-        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationUnionTypeDef = ...
+        ChimeSdkMeetingConfiguration: ChimeSdkMeetingConfigurationTypeDef = ...
     ) -> CreateMediaCapturePipelineResponseTypeDef:
         """
         Creates a media capture pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.create_media_capture_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#create_media_capture_pipeline)
         """
@@ -1766,15 +1766,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_sip_media_application_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_sip_media_application_logging_configuration)
         """
     async def put_voice_connector_emergency_calling_configuration(
         self,
         *,
         VoiceConnectorId: str,
-        EmergencyCallingConfiguration: EmergencyCallingConfigurationUnionTypeDef
+        EmergencyCallingConfiguration: EmergencyCallingConfigurationTypeDef
     ) -> PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef:
         """
         Puts emergency calling configuration details to the specified Amazon Chime Voice
         Connector, such as emergency phone numbers and calling countries.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_emergency_calling_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_emergency_calling_configuration)
@@ -1785,15 +1785,15 @@
         """
         Adds a logging configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_logging_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_logging_configuration)
         """
     async def put_voice_connector_origination(
-        self, *, VoiceConnectorId: str, Origination: OriginationUnionTypeDef
+        self, *, VoiceConnectorId: str, Origination: OriginationTypeDef
     ) -> PutVoiceConnectorOriginationResponseTypeDef:
         """
         Adds origination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_origination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_origination)
         """
@@ -1810,24 +1810,24 @@
         Puts the specified proxy configuration to the specified Amazon Chime Voice
         Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_proxy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_proxy)
         """
     async def put_voice_connector_streaming_configuration(
-        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationUnionTypeDef
+        self, *, VoiceConnectorId: str, StreamingConfiguration: StreamingConfigurationTypeDef
     ) -> PutVoiceConnectorStreamingConfigurationResponseTypeDef:
         """
         Adds a streaming configuration for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_streaming_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_streaming_configuration)
         """
     async def put_voice_connector_termination(
-        self, *, VoiceConnectorId: str, Termination: TerminationUnionTypeDef
+        self, *, VoiceConnectorId: str, Termination: TerminationTypeDef
     ) -> PutVoiceConnectorTerminationResponseTypeDef:
         """
         Adds termination settings for the specified Amazon Chime Voice Connector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/chime.html#Chime.Client.put_voice_connector_termination)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_chime/client/#put_voice_connector_termination)
         """
```

### Comparing `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/literals.py` & `types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/literals.pyi` & `types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/paginator.py` & `types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/paginator.pyi` & `types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/type_defs.py` & `types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -206,15 +206,15 @@
     "GetVoiceConnectorProxyRequestRequestTypeDef",
     "ProxyTypeDef",
     "GetVoiceConnectorRequestRequestTypeDef",
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
-    "TerminationOutputTypeDef",
+    "TerminationTypeDef",
     "InviteTypeDef",
     "InviteUsersRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
@@ -251,24 +251,22 @@
     "OrderedPhoneNumberTypeDef",
     "OriginationRouteTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutEventsConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
-    "TerminationTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
     "RedactConversationMessageRequestRequestTypeDef",
     "RedactRoomMessageRequestRequestTypeDef",
     "RegenerateSecurityTokenRequestRequestTypeDef",
     "ResetPersonalPINRequestRequestTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "RoomRetentionSettingsTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
-    "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "SendChannelMessageRequestRequestTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "StreamingNotificationTargetTypeDef",
     "TelephonySettingsTypeDef",
     "UntagAttendeeRequestRequestTypeDef",
     "UntagMeetingRequestRequestTypeDef",
@@ -389,15 +387,14 @@
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
     "VoiceConnectorGroupTypeDef",
     "CreateVoiceConnectorResponseTypeDef",
     "GetVoiceConnectorResponseTypeDef",
     "ListVoiceConnectorsResponseTypeDef",
     "UpdateVoiceConnectorResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
-    "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "TranscriptionConfigurationTypeDef",
     "GetEventsConfigurationResponseTypeDef",
     "PutEventsConfigurationResponseTypeDef",
     "GetGlobalSettingsResponseTypeDef",
     "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
@@ -407,33 +404,29 @@
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "InviteUsersResponseTypeDef",
     "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListChannelMessagesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     "MeetingTypeDef",
     "RoomMembershipTypeDef",
     "PhoneNumberOrderTypeDef",
-    "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    "TerminationUnionTypeDef",
     "RetentionSettingsTypeDef",
-    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
-    "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
     "UserSettingsTypeDef",
     "CreateAccountResponseTypeDef",
     "GetAccountResponseTypeDef",
     "ListAccountsResponseTypeDef",
     "UpdateAccountResponseTypeDef",
     "BatchUpdateUserRequestRequestTypeDef",
@@ -472,54 +465,49 @@
     "ListSipRulesResponseTypeDef",
     "UpdateSipRuleResponseTypeDef",
     "CreateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorGroupResponseTypeDef",
     "ListVoiceConnectorGroupsResponseTypeDef",
     "UpdateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    "EmergencyCallingConfigurationUnionTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
+    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
     "ListMeetingsResponseTypeDef",
     "CreateRoomMembershipResponseTypeDef",
     "ListRoomMembershipsResponseTypeDef",
     "UpdateRoomMembershipResponseTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
-    "PutVoiceConnectorOriginationResponseTypeDef",
-    "OriginationUnionTypeDef",
     "PutVoiceConnectorOriginationRequestRequestTypeDef",
+    "PutVoiceConnectorOriginationResponseTypeDef",
     "CreateProxySessionResponseTypeDef",
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
     "GetRetentionSettingsResponseTypeDef",
     "PutRetentionSettingsRequestRequestTypeDef",
     "PutRetentionSettingsResponseTypeDef",
-    "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
-    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
-    "StreamingConfigurationUnionTypeDef",
+    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
-    "MediaCapturePipelineTypeDef",
-    "ChimeSdkMeetingConfigurationUnionTypeDef",
     "CreateMediaCapturePipelineRequestRequestTypeDef",
+    "MediaCapturePipelineTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
@@ -2116,16 +2104,16 @@
 GetVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-TerminationOutputTypeDef = TypedDict(
-    "TerminationOutputTypeDef",
+TerminationTypeDef = TypedDict(
+    "TerminationTypeDef",
     {
         "CpsLimit": int,
         "DefaultPhoneNumber": str,
         "CallingRegions": List[str],
         "CidrAllowedList": List[str],
         "Disabled": bool,
     },
@@ -2753,26 +2741,14 @@
 class PutVoiceConnectorProxyRequestRequestTypeDef(
     _RequiredPutVoiceConnectorProxyRequestRequestTypeDef,
     _OptionalPutVoiceConnectorProxyRequestRequestTypeDef,
 ):
     pass
 
 
-TerminationTypeDef = TypedDict(
-    "TerminationTypeDef",
-    {
-        "CpsLimit": int,
-        "DefaultPhoneNumber": str,
-        "CallingRegions": Sequence[str],
-        "CidrAllowedList": Sequence[str],
-        "Disabled": bool,
-    },
-    total=False,
-)
-
 _RequiredRedactChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredRedactChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
     },
 )
@@ -2852,23 +2828,14 @@
         "PhoneNumberType": PhoneNumberTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-SelectedVideoStreamsOutputTypeDef = TypedDict(
-    "SelectedVideoStreamsOutputTypeDef",
-    {
-        "AttendeeIds": List[str],
-        "ExternalUserIds": List[str],
-    },
-    total=False,
-)
-
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
     },
     total=False,
@@ -4420,26 +4387,18 @@
 class PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef(
     _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     _OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
 ):
     pass
 
 
-EmergencyCallingConfigurationOutputTypeDef = TypedDict(
-    "EmergencyCallingConfigurationOutputTypeDef",
-    {
-        "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
-    },
-    total=False,
-)
-
 EmergencyCallingConfigurationTypeDef = TypedDict(
     "EmergencyCallingConfigurationTypeDef",
     {
-        "DNIS": Sequence[DNISEmergencyCallingConfigurationTypeDef],
+        "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
     },
     total=False,
 )
 
 TranscriptionConfigurationTypeDef = TypedDict(
     "TranscriptionConfigurationTypeDef",
     {
@@ -4576,23 +4535,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationOutputTypeDef,
+        "Termination": TerminationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "Termination": TerminationTypeDef,
+    },
+)
+
 PutVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "PutVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationOutputTypeDef,
+        "Termination": TerminationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InviteUsersResponseTypeDef = TypedDict(
     "InviteUsersResponseTypeDef",
     {
@@ -4702,27 +4669,18 @@
         "OrderedPhoneNumbers": List[OrderedPhoneNumberTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-OriginationOutputTypeDef = TypedDict(
-    "OriginationOutputTypeDef",
-    {
-        "Routes": List[OriginationRouteTypeDef],
-        "Disabled": bool,
-    },
-    total=False,
-)
-
 OriginationTypeDef = TypedDict(
     "OriginationTypeDef",
     {
-        "Routes": Sequence[OriginationRouteTypeDef],
+        "Routes": List[OriginationRouteTypeDef],
         "Disabled": bool,
     },
     total=False,
 )
 
 ProxySessionTypeDef = TypedDict(
     "ProxySessionTypeDef",
@@ -4760,81 +4718,42 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "DeletionTimestamp": datetime,
     },
     total=False,
 )
 
-PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "Termination": TerminationTypeDef,
-    },
-)
-
-TerminationUnionTypeDef = Union[TerminationTypeDef, TerminationOutputTypeDef]
 RetentionSettingsTypeDef = TypedDict(
     "RetentionSettingsTypeDef",
     {
         "RoomRetentionSettings": RoomRetentionSettingsTypeDef,
         "ConversationRetentionSettings": ConversationRetentionSettingsTypeDef,
     },
     total=False,
 )
 
-SourceConfigurationOutputTypeDef = TypedDict(
-    "SourceConfigurationOutputTypeDef",
-    {
-        "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
-_RequiredStreamingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredStreamingConfigurationOutputTypeDef",
-    {
-        "DataRetentionInHours": int,
-    },
-)
-_OptionalStreamingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalStreamingConfigurationOutputTypeDef",
-    {
-        "Disabled": bool,
-        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
-    },
-    total=False,
-)
-
-
-class StreamingConfigurationOutputTypeDef(
-    _RequiredStreamingConfigurationOutputTypeDef, _OptionalStreamingConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredStreamingConfigurationTypeDef = TypedDict(
     "_RequiredStreamingConfigurationTypeDef",
     {
         "DataRetentionInHours": int,
     },
 )
 _OptionalStreamingConfigurationTypeDef = TypedDict(
     "_OptionalStreamingConfigurationTypeDef",
     {
         "Disabled": bool,
-        "StreamingNotificationTargets": Sequence[StreamingNotificationTargetTypeDef],
+        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
     },
     total=False,
 )
 
 
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
@@ -5231,35 +5150,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VoiceConnectorId": str,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
     },
 )
 
-EmergencyCallingConfigurationUnionTypeDef = Union[
-    EmergencyCallingConfigurationTypeDef, EmergencyCallingConfigurationOutputTypeDef
-]
-PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
+PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StartMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -5351,33 +5267,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "GetVoiceConnectorOriginationResponseTypeDef",
     {
-        "Origination": OriginationOutputTypeDef,
+        "Origination": OriginationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationResponseTypeDef",
+PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
-        "Origination": OriginationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VoiceConnectorId": str,
+        "Origination": OriginationTypeDef,
     },
 )
 
-OriginationUnionTypeDef = Union[OriginationTypeDef, OriginationOutputTypeDef]
-PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationRequestRequestTypeDef",
+PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
         "Origination": OriginationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProxySessionResponseTypeDef = TypedDict(
     "CreateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
@@ -5465,59 +5380,47 @@
     {
         "RetentionSettings": RetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
-    "ChimeSdkMeetingConfigurationOutputTypeDef",
-    {
-        "SourceConfiguration": SourceConfigurationOutputTypeDef,
-        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
-    },
-    total=False,
-)
-
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
+        "StreamingConfiguration": StreamingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VoiceConnectorId": str,
+        "StreamingConfiguration": StreamingConfigurationTypeDef,
     },
 )
 
-PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
         "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StreamingConfigurationUnionTypeDef = Union[
-    StreamingConfigurationTypeDef, StreamingConfigurationOutputTypeDef
-]
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "UserSettings": UserSettingsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5527,33 +5430,14 @@
     {
         "AccountId": str,
         "UserId": str,
         "UserSettings": UserSettingsTypeDef,
     },
 )
 
-MediaCapturePipelineTypeDef = TypedDict(
-    "MediaCapturePipelineTypeDef",
-    {
-        "MediaPipelineId": str,
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "SourceArn": str,
-        "Status": MediaPipelineStatusType,
-        "SinkType": Literal["S3Bucket"],
-        "SinkArn": str,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-ChimeSdkMeetingConfigurationUnionTypeDef = Union[
-    ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
-]
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
@@ -5572,14 +5456,30 @@
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
 
+MediaCapturePipelineTypeDef = TypedDict(
+    "MediaCapturePipelineTypeDef",
+    {
+        "MediaPipelineId": str,
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "SourceArn": str,
+        "Status": MediaPipelineStatusType,
+        "SinkType": Literal["S3Bucket"],
+        "SinkArn": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
+    },
+    total=False,
+)
+
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime/type_defs.pyi` & `types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     "GetVoiceConnectorProxyRequestRequestTypeDef",
     "ProxyTypeDef",
     "GetVoiceConnectorRequestRequestTypeDef",
     "GetVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     "GetVoiceConnectorTerminationHealthRequestRequestTypeDef",
     "TerminationHealthTypeDef",
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
-    "TerminationOutputTypeDef",
+    "TerminationTypeDef",
     "InviteTypeDef",
     "InviteUsersRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "ListAppInstanceAdminsRequestRequestTypeDef",
     "ListAppInstanceUsersRequestRequestTypeDef",
     "ListAppInstancesRequestRequestTypeDef",
@@ -250,24 +250,22 @@
     "OrderedPhoneNumberTypeDef",
     "OriginationRouteTypeDef",
     "ParticipantTypeDef",
     "PhoneNumberAssociationTypeDef",
     "PhoneNumberCapabilitiesTypeDef",
     "PutEventsConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorProxyRequestRequestTypeDef",
-    "TerminationTypeDef",
     "RedactChannelMessageRequestRequestTypeDef",
     "RedactConversationMessageRequestRequestTypeDef",
     "RedactRoomMessageRequestRequestTypeDef",
     "RegenerateSecurityTokenRequestRequestTypeDef",
     "ResetPersonalPINRequestRequestTypeDef",
     "RestorePhoneNumberRequestRequestTypeDef",
     "RoomRetentionSettingsTypeDef",
     "SearchAvailablePhoneNumbersRequestRequestTypeDef",
-    "SelectedVideoStreamsOutputTypeDef",
     "SelectedVideoStreamsTypeDef",
     "SendChannelMessageRequestRequestTypeDef",
     "StopMeetingTranscriptionRequestRequestTypeDef",
     "StreamingNotificationTargetTypeDef",
     "TelephonySettingsTypeDef",
     "UntagAttendeeRequestRequestTypeDef",
     "UntagMeetingRequestRequestTypeDef",
@@ -388,15 +386,14 @@
     "UpdateVoiceConnectorGroupRequestRequestTypeDef",
     "VoiceConnectorGroupTypeDef",
     "CreateVoiceConnectorResponseTypeDef",
     "GetVoiceConnectorResponseTypeDef",
     "ListVoiceConnectorsResponseTypeDef",
     "UpdateVoiceConnectorResponseTypeDef",
     "PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef",
-    "EmergencyCallingConfigurationOutputTypeDef",
     "EmergencyCallingConfigurationTypeDef",
     "TranscriptionConfigurationTypeDef",
     "GetEventsConfigurationResponseTypeDef",
     "PutEventsConfigurationResponseTypeDef",
     "GetGlobalSettingsResponseTypeDef",
     "UpdateGlobalSettingsRequestRequestTypeDef",
     "GetMessagingSessionEndpointResponseTypeDef",
@@ -406,33 +403,29 @@
     "GetVoiceConnectorLoggingConfigurationResponseTypeDef",
     "PutVoiceConnectorLoggingConfigurationRequestRequestTypeDef",
     "PutVoiceConnectorLoggingConfigurationResponseTypeDef",
     "GetVoiceConnectorProxyResponseTypeDef",
     "PutVoiceConnectorProxyResponseTypeDef",
     "GetVoiceConnectorTerminationHealthResponseTypeDef",
     "GetVoiceConnectorTerminationResponseTypeDef",
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
     "PutVoiceConnectorTerminationResponseTypeDef",
     "InviteUsersResponseTypeDef",
     "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "ListChannelMessagesRequestRequestTypeDef",
     "ListSupportedPhoneNumberCountriesResponseTypeDef",
     "MeetingTypeDef",
     "RoomMembershipTypeDef",
     "PhoneNumberOrderTypeDef",
-    "OriginationOutputTypeDef",
     "OriginationTypeDef",
     "ProxySessionTypeDef",
     "PhoneNumberTypeDef",
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    "TerminationUnionTypeDef",
     "RetentionSettingsTypeDef",
-    "SourceConfigurationOutputTypeDef",
     "SourceConfigurationTypeDef",
-    "StreamingConfigurationOutputTypeDef",
     "StreamingConfigurationTypeDef",
     "UserSettingsTypeDef",
     "CreateAccountResponseTypeDef",
     "GetAccountResponseTypeDef",
     "ListAccountsResponseTypeDef",
     "UpdateAccountResponseTypeDef",
     "BatchUpdateUserRequestRequestTypeDef",
@@ -471,54 +464,49 @@
     "ListSipRulesResponseTypeDef",
     "UpdateSipRuleResponseTypeDef",
     "CreateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorGroupResponseTypeDef",
     "ListVoiceConnectorGroupsResponseTypeDef",
     "UpdateVoiceConnectorGroupResponseTypeDef",
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
-    "EmergencyCallingConfigurationUnionTypeDef",
     "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
+    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     "StartMeetingTranscriptionRequestRequestTypeDef",
     "CreateMeetingResponseTypeDef",
     "CreateMeetingWithAttendeesResponseTypeDef",
     "GetMeetingResponseTypeDef",
     "ListMeetingsResponseTypeDef",
     "CreateRoomMembershipResponseTypeDef",
     "ListRoomMembershipsResponseTypeDef",
     "UpdateRoomMembershipResponseTypeDef",
     "CreatePhoneNumberOrderResponseTypeDef",
     "GetPhoneNumberOrderResponseTypeDef",
     "ListPhoneNumberOrdersResponseTypeDef",
     "GetVoiceConnectorOriginationResponseTypeDef",
-    "PutVoiceConnectorOriginationResponseTypeDef",
-    "OriginationUnionTypeDef",
     "PutVoiceConnectorOriginationRequestRequestTypeDef",
+    "PutVoiceConnectorOriginationResponseTypeDef",
     "CreateProxySessionResponseTypeDef",
     "GetProxySessionResponseTypeDef",
     "ListProxySessionsResponseTypeDef",
     "UpdateProxySessionResponseTypeDef",
     "GetPhoneNumberResponseTypeDef",
     "ListPhoneNumbersResponseTypeDef",
     "RestorePhoneNumberResponseTypeDef",
     "UpdatePhoneNumberResponseTypeDef",
     "GetRetentionSettingsResponseTypeDef",
     "PutRetentionSettingsRequestRequestTypeDef",
     "PutRetentionSettingsResponseTypeDef",
-    "ChimeSdkMeetingConfigurationOutputTypeDef",
     "ChimeSdkMeetingConfigurationTypeDef",
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
-    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
-    "StreamingConfigurationUnionTypeDef",
+    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     "GetUserSettingsResponseTypeDef",
     "UpdateUserSettingsRequestRequestTypeDef",
-    "MediaCapturePipelineTypeDef",
-    "ChimeSdkMeetingConfigurationUnionTypeDef",
     "CreateMediaCapturePipelineRequestRequestTypeDef",
+    "MediaCapturePipelineTypeDef",
     "CreateMediaCapturePipelineResponseTypeDef",
     "GetMediaCapturePipelineResponseTypeDef",
     "ListMediaCapturePipelinesResponseTypeDef",
 )
 
 AccountSettingsTypeDef = TypedDict(
     "AccountSettingsTypeDef",
@@ -2057,16 +2045,16 @@
 GetVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
     "GetVoiceConnectorTerminationRequestRequestTypeDef",
     {
         "VoiceConnectorId": str,
     },
 )
 
-TerminationOutputTypeDef = TypedDict(
-    "TerminationOutputTypeDef",
+TerminationTypeDef = TypedDict(
+    "TerminationTypeDef",
     {
         "CpsLimit": int,
         "DefaultPhoneNumber": str,
         "CallingRegions": List[str],
         "CidrAllowedList": List[str],
         "Disabled": bool,
     },
@@ -2664,26 +2652,14 @@
 
 class PutVoiceConnectorProxyRequestRequestTypeDef(
     _RequiredPutVoiceConnectorProxyRequestRequestTypeDef,
     _OptionalPutVoiceConnectorProxyRequestRequestTypeDef,
 ):
     pass
 
-TerminationTypeDef = TypedDict(
-    "TerminationTypeDef",
-    {
-        "CpsLimit": int,
-        "DefaultPhoneNumber": str,
-        "CallingRegions": Sequence[str],
-        "CidrAllowedList": Sequence[str],
-        "Disabled": bool,
-    },
-    total=False,
-)
-
 _RequiredRedactChannelMessageRequestRequestTypeDef = TypedDict(
     "_RequiredRedactChannelMessageRequestRequestTypeDef",
     {
         "ChannelArn": str,
         "MessageId": str,
     },
 )
@@ -2761,23 +2737,14 @@
         "PhoneNumberType": PhoneNumberTypeType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-SelectedVideoStreamsOutputTypeDef = TypedDict(
-    "SelectedVideoStreamsOutputTypeDef",
-    {
-        "AttendeeIds": List[str],
-        "ExternalUserIds": List[str],
-    },
-    total=False,
-)
-
 SelectedVideoStreamsTypeDef = TypedDict(
     "SelectedVideoStreamsTypeDef",
     {
         "AttendeeIds": Sequence[str],
         "ExternalUserIds": Sequence[str],
     },
     total=False,
@@ -4273,26 +4240,18 @@
 
 class PutVoiceConnectorTerminationCredentialsRequestRequestTypeDef(
     _RequiredPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
     _OptionalPutVoiceConnectorTerminationCredentialsRequestRequestTypeDef,
 ):
     pass
 
-EmergencyCallingConfigurationOutputTypeDef = TypedDict(
-    "EmergencyCallingConfigurationOutputTypeDef",
-    {
-        "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
-    },
-    total=False,
-)
-
 EmergencyCallingConfigurationTypeDef = TypedDict(
     "EmergencyCallingConfigurationTypeDef",
     {
-        "DNIS": Sequence[DNISEmergencyCallingConfigurationTypeDef],
+        "DNIS": List[DNISEmergencyCallingConfigurationTypeDef],
     },
     total=False,
 )
 
 TranscriptionConfigurationTypeDef = TypedDict(
     "TranscriptionConfigurationTypeDef",
     {
@@ -4427,23 +4386,31 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "GetVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationOutputTypeDef,
+        "Termination": TerminationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorTerminationRequestRequestTypeDef",
+    {
+        "VoiceConnectorId": str,
+        "Termination": TerminationTypeDef,
+    },
+)
+
 PutVoiceConnectorTerminationResponseTypeDef = TypedDict(
     "PutVoiceConnectorTerminationResponseTypeDef",
     {
-        "Termination": TerminationOutputTypeDef,
+        "Termination": TerminationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InviteUsersResponseTypeDef = TypedDict(
     "InviteUsersResponseTypeDef",
     {
@@ -4549,27 +4516,18 @@
         "OrderedPhoneNumbers": List[OrderedPhoneNumberTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
 )
 
-OriginationOutputTypeDef = TypedDict(
-    "OriginationOutputTypeDef",
-    {
-        "Routes": List[OriginationRouteTypeDef],
-        "Disabled": bool,
-    },
-    total=False,
-)
-
 OriginationTypeDef = TypedDict(
     "OriginationTypeDef",
     {
-        "Routes": Sequence[OriginationRouteTypeDef],
+        "Routes": List[OriginationRouteTypeDef],
         "Disabled": bool,
     },
     total=False,
 )
 
 ProxySessionTypeDef = TypedDict(
     "ProxySessionTypeDef",
@@ -4607,79 +4565,42 @@
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "DeletionTimestamp": datetime,
     },
     total=False,
 )
 
-PutVoiceConnectorTerminationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorTerminationRequestRequestTypeDef",
-    {
-        "VoiceConnectorId": str,
-        "Termination": TerminationTypeDef,
-    },
-)
-
-TerminationUnionTypeDef = Union[TerminationTypeDef, TerminationOutputTypeDef]
 RetentionSettingsTypeDef = TypedDict(
     "RetentionSettingsTypeDef",
     {
         "RoomRetentionSettings": RoomRetentionSettingsTypeDef,
         "ConversationRetentionSettings": ConversationRetentionSettingsTypeDef,
     },
     total=False,
 )
 
-SourceConfigurationOutputTypeDef = TypedDict(
-    "SourceConfigurationOutputTypeDef",
-    {
-        "SelectedVideoStreams": SelectedVideoStreamsOutputTypeDef,
-    },
-    total=False,
-)
-
 SourceConfigurationTypeDef = TypedDict(
     "SourceConfigurationTypeDef",
     {
         "SelectedVideoStreams": SelectedVideoStreamsTypeDef,
     },
     total=False,
 )
 
-_RequiredStreamingConfigurationOutputTypeDef = TypedDict(
-    "_RequiredStreamingConfigurationOutputTypeDef",
-    {
-        "DataRetentionInHours": int,
-    },
-)
-_OptionalStreamingConfigurationOutputTypeDef = TypedDict(
-    "_OptionalStreamingConfigurationOutputTypeDef",
-    {
-        "Disabled": bool,
-        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
-    },
-    total=False,
-)
-
-class StreamingConfigurationOutputTypeDef(
-    _RequiredStreamingConfigurationOutputTypeDef, _OptionalStreamingConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredStreamingConfigurationTypeDef = TypedDict(
     "_RequiredStreamingConfigurationTypeDef",
     {
         "DataRetentionInHours": int,
     },
 )
 _OptionalStreamingConfigurationTypeDef = TypedDict(
     "_OptionalStreamingConfigurationTypeDef",
     {
         "Disabled": bool,
-        "StreamingNotificationTargets": Sequence[StreamingNotificationTargetTypeDef],
+        "StreamingNotificationTargets": List[StreamingNotificationTargetTypeDef],
     },
     total=False,
 )
 
 class StreamingConfigurationTypeDef(
     _RequiredStreamingConfigurationTypeDef, _OptionalStreamingConfigurationTypeDef
 ):
@@ -5072,35 +4993,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
+PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
     {
-        "EmergencyCallingConfiguration": EmergencyCallingConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VoiceConnectorId": str,
+        "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
     },
 )
 
-EmergencyCallingConfigurationUnionTypeDef = Union[
-    EmergencyCallingConfigurationTypeDef, EmergencyCallingConfigurationOutputTypeDef
-]
-PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorEmergencyCallingConfigurationRequestRequestTypeDef",
+PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorEmergencyCallingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
         "EmergencyCallingConfiguration": EmergencyCallingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMeetingTranscriptionRequestRequestTypeDef = TypedDict(
     "StartMeetingTranscriptionRequestRequestTypeDef",
     {
         "MeetingId": str,
@@ -5192,33 +5110,32 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVoiceConnectorOriginationResponseTypeDef = TypedDict(
     "GetVoiceConnectorOriginationResponseTypeDef",
     {
-        "Origination": OriginationOutputTypeDef,
+        "Origination": OriginationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationResponseTypeDef",
+PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationRequestRequestTypeDef",
     {
-        "Origination": OriginationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VoiceConnectorId": str,
+        "Origination": OriginationTypeDef,
     },
 )
 
-OriginationUnionTypeDef = Union[OriginationTypeDef, OriginationOutputTypeDef]
-PutVoiceConnectorOriginationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorOriginationRequestRequestTypeDef",
+PutVoiceConnectorOriginationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorOriginationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
         "Origination": OriginationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateProxySessionResponseTypeDef = TypedDict(
     "CreateProxySessionResponseTypeDef",
     {
         "ProxySession": ProxySessionTypeDef,
@@ -5306,59 +5223,47 @@
     {
         "RetentionSettings": RetentionSettingsTypeDef,
         "InitiateDeletionTimestamp": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ChimeSdkMeetingConfigurationOutputTypeDef = TypedDict(
-    "ChimeSdkMeetingConfigurationOutputTypeDef",
-    {
-        "SourceConfiguration": SourceConfigurationOutputTypeDef,
-        "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
-    },
-    total=False,
-)
-
 ChimeSdkMeetingConfigurationTypeDef = TypedDict(
     "ChimeSdkMeetingConfigurationTypeDef",
     {
         "SourceConfiguration": SourceConfigurationTypeDef,
         "ArtifactsConfiguration": ArtifactsConfigurationTypeDef,
     },
     total=False,
 )
 
 GetVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
     "GetVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
+        "StreamingConfiguration": StreamingConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
+PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
     {
-        "StreamingConfiguration": StreamingConfigurationOutputTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VoiceConnectorId": str,
+        "StreamingConfiguration": StreamingConfigurationTypeDef,
     },
 )
 
-PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef = TypedDict(
-    "PutVoiceConnectorStreamingConfigurationRequestRequestTypeDef",
+PutVoiceConnectorStreamingConfigurationResponseTypeDef = TypedDict(
+    "PutVoiceConnectorStreamingConfigurationResponseTypeDef",
     {
-        "VoiceConnectorId": str,
         "StreamingConfiguration": StreamingConfigurationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StreamingConfigurationUnionTypeDef = Union[
-    StreamingConfigurationTypeDef, StreamingConfigurationOutputTypeDef
-]
 GetUserSettingsResponseTypeDef = TypedDict(
     "GetUserSettingsResponseTypeDef",
     {
         "UserSettings": UserSettingsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -5368,33 +5273,14 @@
     {
         "AccountId": str,
         "UserId": str,
         "UserSettings": UserSettingsTypeDef,
     },
 )
 
-MediaCapturePipelineTypeDef = TypedDict(
-    "MediaCapturePipelineTypeDef",
-    {
-        "MediaPipelineId": str,
-        "SourceType": Literal["ChimeSdkMeeting"],
-        "SourceArn": str,
-        "Status": MediaPipelineStatusType,
-        "SinkType": Literal["S3Bucket"],
-        "SinkArn": str,
-        "CreatedTimestamp": datetime,
-        "UpdatedTimestamp": datetime,
-        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationOutputTypeDef,
-    },
-    total=False,
-)
-
-ChimeSdkMeetingConfigurationUnionTypeDef = Union[
-    ChimeSdkMeetingConfigurationTypeDef, ChimeSdkMeetingConfigurationOutputTypeDef
-]
 _RequiredCreateMediaCapturePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMediaCapturePipelineRequestRequestTypeDef",
     {
         "SourceType": Literal["ChimeSdkMeeting"],
         "SourceArn": str,
         "SinkType": Literal["S3Bucket"],
         "SinkArn": str,
@@ -5411,14 +5297,30 @@
 
 class CreateMediaCapturePipelineRequestRequestTypeDef(
     _RequiredCreateMediaCapturePipelineRequestRequestTypeDef,
     _OptionalCreateMediaCapturePipelineRequestRequestTypeDef,
 ):
     pass
 
+MediaCapturePipelineTypeDef = TypedDict(
+    "MediaCapturePipelineTypeDef",
+    {
+        "MediaPipelineId": str,
+        "SourceType": Literal["ChimeSdkMeeting"],
+        "SourceArn": str,
+        "Status": MediaPipelineStatusType,
+        "SinkType": Literal["S3Bucket"],
+        "SinkArn": str,
+        "CreatedTimestamp": datetime,
+        "UpdatedTimestamp": datetime,
+        "ChimeSdkMeetingConfiguration": ChimeSdkMeetingConfigurationTypeDef,
+    },
+    total=False,
+)
+
 CreateMediaCapturePipelineResponseTypeDef = TypedDict(
     "CreateMediaCapturePipelineResponseTypeDef",
     {
         "MediaCapturePipeline": MediaCapturePipelineTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-chime-2.5.2.post1/types_aiobotocore_chime.egg-info/SOURCES.txt` & `types-aiobotocore-chime-2.5.2.post2/types_aiobotocore_chime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

