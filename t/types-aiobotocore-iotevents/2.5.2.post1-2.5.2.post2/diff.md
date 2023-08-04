# Comparing `tmp/types-aiobotocore-iotevents-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-iotevents-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotevents-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:26 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotevents-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:12 2023, max compression
```

## Comparing `types-aiobotocore-iotevents-2.5.2.post1.tar` & `types-aiobotocore-iotevents-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.629562 types-aiobotocore-iotevents-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-08-02 14:52:26.629562 types-aiobotocore-iotevents-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:26.629562 types-aiobotocore-iotevents-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.625563 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20470 2023-08-02 14:40:45.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20436 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-08-02 14:40:45.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8752 2023-08-02 14:40:45.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43431 2023-08-02 14:40:47.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43352 2023-08-02 14:40:45.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:44.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:26.629562 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:26.000000 types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:58:49.596642 types-aiobotocore-iotevents-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12314 2023-08-04 13:59:12.396643 types-aiobotocore-iotevents-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10788 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:12.406643 types-aiobotocore-iotevents-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:58:49.596642 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      458 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      457 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      951 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20395 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    20361 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8849 2023-08-04 13:41:00.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     8847 2023-08-04 13:41:00.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    37370 2023-08-04 13:41:01.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    37305 2023-08-04 13:41:00.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:40:59.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:12.396643 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12314 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      768 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:12.000000 types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotevents-2.5.2.post1/LICENSE` & `types-aiobotocore-iotevents-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotevents-2.5.2.post1/setup.py` & `types-aiobotocore-iotevents-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotevents",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_iotevents"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTEvents 2.5.2 service generated with mypy-boto3-builder"
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

### Comparing `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/__main__.py` & `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTEvents 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.IoTEvents 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents\nOther"
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

### Comparing `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/client.py` & `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,38 +18,38 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import EvaluationMethodType
 from .type_defs import (
     AlarmCapabilitiesTypeDef,
-    AlarmEventActionsUnionTypeDef,
-    AlarmNotificationUnionTypeDef,
+    AlarmEventActionsTypeDef,
+    AlarmNotificationTypeDef,
     AlarmRuleTypeDef,
     CreateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     DescribeAlarmModelResponseTypeDef,
     DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelResponseTypeDef,
     DescribeInputResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    DetectorModelDefinitionUnionTypeDef,
+    DetectorModelDefinitionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
-    InputDefinitionUnionTypeDef,
+    InputDefinitionTypeDef,
     InputIdentifierTypeDef,
     ListAlarmModelsResponseTypeDef,
     ListAlarmModelVersionsResponseTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
     ListInputRoutingsResponseTypeDef,
     ListInputsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    LoggingOptionsUnionTypeDef,
+    LoggingOptionsTypeDef,
     StartDetectorModelAnalysisResponseTypeDef,
     TagTypeDef,
     UpdateAlarmModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     UpdateInputResponseTypeDef,
 )
 
@@ -116,30 +116,30 @@
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         key: str = ...,
         severity: int = ...,
-        alarmNotification: AlarmNotificationUnionTypeDef = ...,
-        alarmEventActions: AlarmEventActionsUnionTypeDef = ...,
+        alarmNotification: AlarmNotificationTypeDef = ...,
+        alarmEventActions: AlarmEventActionsTypeDef = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> CreateAlarmModelResponseTypeDef:
         """
         Creates an alarm model to monitor an AWS IoT Events input attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_alarm_model)
         """
 
     async def create_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,
+        detectorModelDefinition: DetectorModelDefinitionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         key: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> CreateDetectorModelResponseTypeDef:
         """
@@ -149,15 +149,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_detector_model)
         """
 
     async def create_input(
         self,
         *,
         inputName: str,
-        inputDefinition: InputDefinitionUnionTypeDef,
+        inputDefinition: InputDefinitionTypeDef,
         inputDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateInputResponseTypeDef:
         """
         Creates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_input)
@@ -329,25 +329,25 @@
         Lists the tags (metadata) you have assigned to the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_tags_for_resource)
         """
 
     async def put_logging_options(
-        self, *, loggingOptions: LoggingOptionsUnionTypeDef
+        self, *, loggingOptions: LoggingOptionsTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets or updates the AWS IoT Events logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.put_logging_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#put_logging_options)
         """
 
     async def start_detector_model_analysis(
-        self, *, detectorModelDefinition: DetectorModelDefinitionUnionTypeDef
+        self, *, detectorModelDefinition: DetectorModelDefinitionTypeDef
     ) -> StartDetectorModelAnalysisResponseTypeDef:
         """
         Performs an analysis of your detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.start_detector_model_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#start_detector_model_analysis)
         """
@@ -372,30 +372,30 @@
         self,
         *,
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         severity: int = ...,
-        alarmNotification: AlarmNotificationUnionTypeDef = ...,
-        alarmEventActions: AlarmEventActionsUnionTypeDef = ...,
+        alarmNotification: AlarmNotificationTypeDef = ...,
+        alarmEventActions: AlarmEventActionsTypeDef = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> UpdateAlarmModelResponseTypeDef:
         """
         Updates an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_alarm_model)
         """
 
     async def update_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,
+        detectorModelDefinition: DetectorModelDefinitionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> UpdateDetectorModelResponseTypeDef:
         """
         Updates a detector model.
 
@@ -403,15 +403,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_detector_model)
         """
 
     async def update_input(
         self,
         *,
         inputName: str,
-        inputDefinition: InputDefinitionUnionTypeDef,
+        inputDefinition: InputDefinitionTypeDef,
         inputDescription: str = ...
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_input)
```

### Comparing `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/client.pyi` & `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,38 +18,38 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import EvaluationMethodType
 from .type_defs import (
     AlarmCapabilitiesTypeDef,
-    AlarmEventActionsUnionTypeDef,
-    AlarmNotificationUnionTypeDef,
+    AlarmEventActionsTypeDef,
+    AlarmNotificationTypeDef,
     AlarmRuleTypeDef,
     CreateAlarmModelResponseTypeDef,
     CreateDetectorModelResponseTypeDef,
     CreateInputResponseTypeDef,
     DescribeAlarmModelResponseTypeDef,
     DescribeDetectorModelAnalysisResponseTypeDef,
     DescribeDetectorModelResponseTypeDef,
     DescribeInputResponseTypeDef,
     DescribeLoggingOptionsResponseTypeDef,
-    DetectorModelDefinitionUnionTypeDef,
+    DetectorModelDefinitionTypeDef,
     EmptyResponseMetadataTypeDef,
     GetDetectorModelAnalysisResultsResponseTypeDef,
-    InputDefinitionUnionTypeDef,
+    InputDefinitionTypeDef,
     InputIdentifierTypeDef,
     ListAlarmModelsResponseTypeDef,
     ListAlarmModelVersionsResponseTypeDef,
     ListDetectorModelsResponseTypeDef,
     ListDetectorModelVersionsResponseTypeDef,
     ListInputRoutingsResponseTypeDef,
     ListInputsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    LoggingOptionsUnionTypeDef,
+    LoggingOptionsTypeDef,
     StartDetectorModelAnalysisResponseTypeDef,
     TagTypeDef,
     UpdateAlarmModelResponseTypeDef,
     UpdateDetectorModelResponseTypeDef,
     UpdateInputResponseTypeDef,
 )
 
@@ -110,29 +110,29 @@
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         key: str = ...,
         severity: int = ...,
-        alarmNotification: AlarmNotificationUnionTypeDef = ...,
-        alarmEventActions: AlarmEventActionsUnionTypeDef = ...,
+        alarmNotification: AlarmNotificationTypeDef = ...,
+        alarmEventActions: AlarmEventActionsTypeDef = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> CreateAlarmModelResponseTypeDef:
         """
         Creates an alarm model to monitor an AWS IoT Events input attribute.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_alarm_model)
         """
     async def create_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,
+        detectorModelDefinition: DetectorModelDefinitionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         key: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> CreateDetectorModelResponseTypeDef:
         """
@@ -141,15 +141,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#create_detector_model)
         """
     async def create_input(
         self,
         *,
         inputName: str,
-        inputDefinition: InputDefinitionUnionTypeDef,
+        inputDefinition: InputDefinitionTypeDef,
         inputDescription: str = ...,
         tags: Sequence[TagTypeDef] = ...
     ) -> CreateInputResponseTypeDef:
         """
         Creates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.create_input)
@@ -303,24 +303,24 @@
         """
         Lists the tags (metadata) you have assigned to the resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#list_tags_for_resource)
         """
     async def put_logging_options(
-        self, *, loggingOptions: LoggingOptionsUnionTypeDef
+        self, *, loggingOptions: LoggingOptionsTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sets or updates the AWS IoT Events logging options.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.put_logging_options)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#put_logging_options)
         """
     async def start_detector_model_analysis(
-        self, *, detectorModelDefinition: DetectorModelDefinitionUnionTypeDef
+        self, *, detectorModelDefinition: DetectorModelDefinitionTypeDef
     ) -> StartDetectorModelAnalysisResponseTypeDef:
         """
         Performs an analysis of your detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.start_detector_model_analysis)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#start_detector_model_analysis)
         """
@@ -342,44 +342,44 @@
         self,
         *,
         alarmModelName: str,
         roleArn: str,
         alarmRule: AlarmRuleTypeDef,
         alarmModelDescription: str = ...,
         severity: int = ...,
-        alarmNotification: AlarmNotificationUnionTypeDef = ...,
-        alarmEventActions: AlarmEventActionsUnionTypeDef = ...,
+        alarmNotification: AlarmNotificationTypeDef = ...,
+        alarmEventActions: AlarmEventActionsTypeDef = ...,
         alarmCapabilities: AlarmCapabilitiesTypeDef = ...
     ) -> UpdateAlarmModelResponseTypeDef:
         """
         Updates an alarm model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_alarm_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_alarm_model)
         """
     async def update_detector_model(
         self,
         *,
         detectorModelName: str,
-        detectorModelDefinition: DetectorModelDefinitionUnionTypeDef,
+        detectorModelDefinition: DetectorModelDefinitionTypeDef,
         roleArn: str,
         detectorModelDescription: str = ...,
         evaluationMethod: EvaluationMethodType = ...
     ) -> UpdateDetectorModelResponseTypeDef:
         """
         Updates a detector model.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_detector_model)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_detector_model)
         """
     async def update_input(
         self,
         *,
         inputName: str,
-        inputDefinition: InputDefinitionUnionTypeDef,
+        inputDefinition: InputDefinitionTypeDef,
         inputDescription: str = ...
     ) -> UpdateInputResponseTypeDef:
         """
         Updates an input.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotevents.html#IoTEvents.Client.update_input)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotevents/client/#update_input)
```

### Comparing `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/literals.py` & `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "AlarmModelVersionStatusType",
     "AnalysisResultLevelType",
     "AnalysisStatusType",
     "ComparisonOperatorType",
     "DetectorModelVersionStatusType",
     "EvaluationMethodType",
@@ -31,15 +30,14 @@
     "PayloadTypeType",
     "IoTEventsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 AlarmModelVersionStatusType = Literal["ACTIVATING", "ACTIVE", "FAILED", "INACTIVE"]
 AnalysisResultLevelType = Literal["ERROR", "INFO", "WARNING"]
 AnalysisStatusType = Literal["COMPLETE", "FAILED", "RUNNING"]
 ComparisonOperatorType = Literal[
     "EQUAL", "GREATER", "GREATER_OR_EQUAL", "LESS", "LESS_OR_EQUAL", "NOT_EQUAL"
 ]
 DetectorModelVersionStatusType = Literal[
@@ -61,14 +59,15 @@
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
@@ -164,14 +163,15 @@
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
@@ -250,26 +250,28 @@
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

### Comparing `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/literals.pyi` & `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "AlarmModelVersionStatusType",
     "AnalysisResultLevelType",
     "AnalysisStatusType",
     "ComparisonOperatorType",
     "DetectorModelVersionStatusType",
     "EvaluationMethodType",
@@ -30,14 +31,15 @@
     "PayloadTypeType",
     "IoTEventsServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 AlarmModelVersionStatusType = Literal["ACTIVATING", "ACTIVE", "FAILED", "INACTIVE"]
 AnalysisResultLevelType = Literal["ERROR", "INFO", "WARNING"]
 AnalysisStatusType = Literal["COMPLETE", "FAILED", "RUNNING"]
 ComparisonOperatorType = Literal[
     "EQUAL", "GREATER", "GREATER_OR_EQUAL", "LESS", "LESS_OR_EQUAL", "NOT_EQUAL"
 ]
 DetectorModelVersionStatusType = Literal[
@@ -59,14 +61,15 @@
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
@@ -162,14 +165,15 @@
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
@@ -248,26 +252,28 @@
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

### Comparing `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/type_defs.py` & `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/type_defs.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_iotevents.type_defs import AcknowledgeFlowTypeDef
 
     data: AcknowledgeFlowTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     AlarmModelVersionStatusType,
     AnalysisResultLevelType,
     AnalysisStatusType,
     ComparisonOperatorType,
     DetectorModelVersionStatusType,
@@ -28,15 +28,14 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AcknowledgeFlowTypeDef",
     "ClearTimerActionTypeDef",
     "ResetTimerActionTypeDef",
     "SetTimerActionTypeDef",
     "SetVariableActionTypeDef",
     "InitializationConfigurationTypeDef",
@@ -76,30 +75,28 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "SSOIdentityTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AlarmCapabilitiesTypeDef",
     "AlarmRuleTypeDef",
     "AnalysisResultTypeDef",
     "AssetPropertyValueTypeDef",
-    "InputDefinitionOutputTypeDef",
     "InputDefinitionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateAlarmModelResponseTypeDef",
     "DescribeDetectorModelAnalysisResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListAlarmModelVersionsResponseTypeDef",
     "ListAlarmModelsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartDetectorModelAnalysisResponseTypeDef",
     "UpdateAlarmModelResponseTypeDef",
     "CreateDetectorModelResponseTypeDef",
     "UpdateDetectorModelResponseTypeDef",
     "CreateInputResponseTypeDef",
     "UpdateInputResponseTypeDef",
-    "LoggingOptionsOutputTypeDef",
     "LoggingOptionsTypeDef",
     "ListDetectorModelsResponseTypeDef",
     "ListDetectorModelVersionsResponseTypeDef",
     "DynamoDBActionTypeDef",
     "DynamoDBv2ActionTypeDef",
     "FirehoseActionTypeDef",
     "IotEventsActionTypeDef",
@@ -109,61 +106,43 @@
     "SqsActionTypeDef",
     "ListInputsResponseTypeDef",
     "IotSiteWiseInputIdentifierTypeDef",
     "ListInputRoutingsResponseTypeDef",
     "RecipientDetailTypeDef",
     "GetDetectorModelAnalysisResultsResponseTypeDef",
     "IotSiteWiseActionTypeDef",
-    "InputTypeDef",
     "CreateInputRequestRequestTypeDef",
-    "InputDefinitionUnionTypeDef",
+    "InputTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
-    "LoggingOptionsUnionTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "NotificationTargetActionsTypeDef",
     "InputIdentifierTypeDef",
-    "EmailRecipientsOutputTypeDef",
     "EmailRecipientsTypeDef",
-    "SMSConfigurationOutputTypeDef",
     "SMSConfigurationTypeDef",
     "ActionTypeDef",
     "AlarmActionTypeDef",
     "DescribeInputResponseTypeDef",
     "ListInputRoutingsRequestRequestTypeDef",
-    "EmailConfigurationOutputTypeDef",
     "EmailConfigurationTypeDef",
-    "EventOutputTypeDef",
     "EventTypeDef",
-    "TransitionEventOutputTypeDef",
     "TransitionEventTypeDef",
-    "AlarmEventActionsOutputTypeDef",
     "AlarmEventActionsTypeDef",
-    "NotificationActionOutputTypeDef",
     "NotificationActionTypeDef",
-    "OnEnterLifecycleOutputTypeDef",
-    "OnExitLifecycleOutputTypeDef",
     "OnEnterLifecycleTypeDef",
     "OnExitLifecycleTypeDef",
-    "OnInputLifecycleOutputTypeDef",
     "OnInputLifecycleTypeDef",
-    "AlarmEventActionsUnionTypeDef",
-    "AlarmNotificationOutputTypeDef",
     "AlarmNotificationTypeDef",
-    "StateOutputTypeDef",
     "StateTypeDef",
-    "DescribeAlarmModelResponseTypeDef",
-    "AlarmNotificationUnionTypeDef",
     "CreateAlarmModelRequestRequestTypeDef",
+    "DescribeAlarmModelResponseTypeDef",
     "UpdateAlarmModelRequestRequestTypeDef",
-    "DetectorModelDefinitionOutputTypeDef",
     "DetectorModelDefinitionTypeDef",
-    "DetectorModelTypeDef",
     "CreateDetectorModelRequestRequestTypeDef",
-    "DetectorModelDefinitionUnionTypeDef",
+    "DetectorModelTypeDef",
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     "UpdateDetectorModelRequestRequestTypeDef",
     "DescribeDetectorModelResponseTypeDef",
 )
 
 AcknowledgeFlowTypeDef = TypedDict(
     "AcknowledgeFlowTypeDef",
@@ -197,19 +176,17 @@
     {
         "seconds": int,
         "durationExpression": str,
     },
     total=False,
 )
 
-
 class SetTimerActionTypeDef(_RequiredSetTimerActionTypeDef, _OptionalSetTimerActionTypeDef):
     pass
 
-
 SetVariableActionTypeDef = TypedDict(
     "SetVariableActionTypeDef",
     {
         "variableName": str,
         "value": str,
     },
 )
@@ -273,21 +250,19 @@
     "_OptionalAssetPropertyTimestampTypeDef",
     {
         "offsetInNanos": str,
     },
     total=False,
 )
 
-
 class AssetPropertyTimestampTypeDef(
     _RequiredAssetPropertyTimestampTypeDef, _OptionalAssetPropertyTimestampTypeDef
 ):
     pass
 
-
 AssetPropertyVariantTypeDef = TypedDict(
     "AssetPropertyVariantTypeDef",
     {
         "stringValue": str,
         "integerValue": str,
         "doubleValue": str,
         "booleanValue": str,
@@ -352,21 +327,19 @@
     "_OptionalInputConfigurationTypeDef",
     {
         "inputDescription": str,
     },
     total=False,
 )
 
-
 class InputConfigurationTypeDef(
     _RequiredInputConfigurationTypeDef, _OptionalInputConfigurationTypeDef
 ):
     pass
 
-
 DeleteAlarmModelRequestRequestTypeDef = TypedDict(
     "DeleteAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
     },
 )
 
@@ -394,22 +367,20 @@
     "_OptionalDescribeAlarmModelRequestRequestTypeDef",
     {
         "alarmModelVersion": str,
     },
     total=False,
 )
 
-
 class DescribeAlarmModelRequestRequestTypeDef(
     _RequiredDescribeAlarmModelRequestRequestTypeDef,
     _OptionalDescribeAlarmModelRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 
@@ -423,22 +394,20 @@
     "_OptionalDescribeDetectorModelRequestRequestTypeDef",
     {
         "detectorModelVersion": str,
     },
     total=False,
 )
 
-
 class DescribeDetectorModelRequestRequestTypeDef(
     _RequiredDescribeDetectorModelRequestRequestTypeDef,
     _OptionalDescribeDetectorModelRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeInputRequestRequestTypeDef = TypedDict(
     "DescribeInputRequestRequestTypeDef",
     {
         "inputName": str,
     },
 )
 
@@ -452,21 +421,19 @@
     "_OptionalDetectorDebugOptionTypeDef",
     {
         "keyValue": str,
     },
     total=False,
 )
 
-
 class DetectorDebugOptionTypeDef(
     _RequiredDetectorDebugOptionTypeDef, _OptionalDetectorDebugOptionTypeDef
 ):
     pass
 
-
 DetectorModelSummaryTypeDef = TypedDict(
     "DetectorModelSummaryTypeDef",
     {
         "detectorModelName": str,
         "detectorModelDescription": str,
         "creationTime": datetime,
     },
@@ -516,22 +483,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class GetDetectorModelAnalysisResultsRequestRequestTypeDef(
     _RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef,
     _OptionalGetDetectorModelAnalysisResultsRequestRequestTypeDef,
 ):
     pass
 
-
 IotEventsInputIdentifierTypeDef = TypedDict(
     "IotEventsInputIdentifierTypeDef",
     {
         "inputName": str,
     },
 )
 
@@ -567,22 +532,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListAlarmModelVersionsRequestRequestTypeDef(
     _RequiredListAlarmModelVersionsRequestRequestTypeDef,
     _OptionalListAlarmModelVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListAlarmModelsRequestRequestTypeDef = TypedDict(
     "ListAlarmModelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -599,22 +562,20 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-
 class ListDetectorModelVersionsRequestRequestTypeDef(
     _RequiredListDetectorModelVersionsRequestRequestTypeDef,
     _OptionalListDetectorModelVersionsRequestRequestTypeDef,
 ):
     pass
 
-
 ListDetectorModelsRequestRequestTypeDef = TypedDict(
     "ListDetectorModelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -655,19 +616,17 @@
     "_OptionalSSOIdentityTypeDef",
     {
         "userId": str,
     },
     total=False,
 )
 
-
 class SSOIdentityTypeDef(_RequiredSSOIdentityTypeDef, _OptionalSSOIdentityTypeDef):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -706,21 +665,14 @@
         "value": AssetPropertyVariantTypeDef,
         "timestamp": AssetPropertyTimestampTypeDef,
         "quality": str,
     },
     total=False,
 )
 
-InputDefinitionOutputTypeDef = TypedDict(
-    "InputDefinitionOutputTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-    },
-)
-
 InputDefinitionTypeDef = TypedDict(
     "InputDefinitionTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 
@@ -833,58 +785,33 @@
     "UpdateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLoggingOptionsOutputTypeDef = TypedDict(
-    "_RequiredLoggingOptionsOutputTypeDef",
-    {
-        "roleArn": str,
-        "level": LoggingLevelType,
-        "enabled": bool,
-    },
-)
-_OptionalLoggingOptionsOutputTypeDef = TypedDict(
-    "_OptionalLoggingOptionsOutputTypeDef",
-    {
-        "detectorDebugOptions": List[DetectorDebugOptionTypeDef],
-    },
-    total=False,
-)
-
-
-class LoggingOptionsOutputTypeDef(
-    _RequiredLoggingOptionsOutputTypeDef, _OptionalLoggingOptionsOutputTypeDef
-):
-    pass
-
-
 _RequiredLoggingOptionsTypeDef = TypedDict(
     "_RequiredLoggingOptionsTypeDef",
     {
         "roleArn": str,
         "level": LoggingLevelType,
         "enabled": bool,
     },
 )
 _OptionalLoggingOptionsTypeDef = TypedDict(
     "_OptionalLoggingOptionsTypeDef",
     {
-        "detectorDebugOptions": Sequence[DetectorDebugOptionTypeDef],
+        "detectorDebugOptions": List[DetectorDebugOptionTypeDef],
     },
     total=False,
 )
 
-
 class LoggingOptionsTypeDef(_RequiredLoggingOptionsTypeDef, _OptionalLoggingOptionsTypeDef):
     pass
 
-
 ListDetectorModelsResponseTypeDef = TypedDict(
     "ListDetectorModelsResponseTypeDef",
     {
         "detectorModelSummaries": List[DetectorModelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -917,38 +844,34 @@
         "operation": str,
         "payloadField": str,
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class DynamoDBActionTypeDef(_RequiredDynamoDBActionTypeDef, _OptionalDynamoDBActionTypeDef):
     pass
 
-
 _RequiredDynamoDBv2ActionTypeDef = TypedDict(
     "_RequiredDynamoDBv2ActionTypeDef",
     {
         "tableName": str,
     },
 )
 _OptionalDynamoDBv2ActionTypeDef = TypedDict(
     "_OptionalDynamoDBv2ActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class DynamoDBv2ActionTypeDef(_RequiredDynamoDBv2ActionTypeDef, _OptionalDynamoDBv2ActionTypeDef):
     pass
 
-
 _RequiredFirehoseActionTypeDef = TypedDict(
     "_RequiredFirehoseActionTypeDef",
     {
         "deliveryStreamName": str,
     },
 )
 _OptionalFirehoseActionTypeDef = TypedDict(
@@ -956,99 +879,89 @@
     {
         "separator": str,
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class FirehoseActionTypeDef(_RequiredFirehoseActionTypeDef, _OptionalFirehoseActionTypeDef):
     pass
 
-
 _RequiredIotEventsActionTypeDef = TypedDict(
     "_RequiredIotEventsActionTypeDef",
     {
         "inputName": str,
     },
 )
 _OptionalIotEventsActionTypeDef = TypedDict(
     "_OptionalIotEventsActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class IotEventsActionTypeDef(_RequiredIotEventsActionTypeDef, _OptionalIotEventsActionTypeDef):
     pass
 
-
 _RequiredIotTopicPublishActionTypeDef = TypedDict(
     "_RequiredIotTopicPublishActionTypeDef",
     {
         "mqttTopic": str,
     },
 )
 _OptionalIotTopicPublishActionTypeDef = TypedDict(
     "_OptionalIotTopicPublishActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class IotTopicPublishActionTypeDef(
     _RequiredIotTopicPublishActionTypeDef, _OptionalIotTopicPublishActionTypeDef
 ):
     pass
 
-
 _RequiredLambdaActionTypeDef = TypedDict(
     "_RequiredLambdaActionTypeDef",
     {
         "functionArn": str,
     },
 )
 _OptionalLambdaActionTypeDef = TypedDict(
     "_OptionalLambdaActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class LambdaActionTypeDef(_RequiredLambdaActionTypeDef, _OptionalLambdaActionTypeDef):
     pass
 
-
 _RequiredSNSTopicPublishActionTypeDef = TypedDict(
     "_RequiredSNSTopicPublishActionTypeDef",
     {
         "targetArn": str,
     },
 )
 _OptionalSNSTopicPublishActionTypeDef = TypedDict(
     "_OptionalSNSTopicPublishActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class SNSTopicPublishActionTypeDef(
     _RequiredSNSTopicPublishActionTypeDef, _OptionalSNSTopicPublishActionTypeDef
 ):
     pass
 
-
 _RequiredSqsActionTypeDef = TypedDict(
     "_RequiredSqsActionTypeDef",
     {
         "queueUrl": str,
     },
 )
 _OptionalSqsActionTypeDef = TypedDict(
@@ -1056,19 +969,17 @@
     {
         "useBase64": bool,
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
-
 class SqsActionTypeDef(_RequiredSqsActionTypeDef, _OptionalSqsActionTypeDef):
     pass
 
-
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "inputSummaries": List[InputSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1116,23 +1027,14 @@
         "propertyId": str,
         "propertyAlias": str,
         "propertyValue": AssetPropertyValueTypeDef,
     },
     total=False,
 )
 
-InputTypeDef = TypedDict(
-    "InputTypeDef",
-    {
-        "inputConfiguration": InputConfigurationTypeDef,
-        "inputDefinition": InputDefinitionOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateInputRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInputRequestRequestTypeDef",
     {
         "inputName": str,
         "inputDefinition": InputDefinitionTypeDef,
     },
 )
@@ -1141,22 +1043,28 @@
     {
         "inputDescription": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateInputRequestRequestTypeDef(
     _RequiredCreateInputRequestRequestTypeDef, _OptionalCreateInputRequestRequestTypeDef
 ):
     pass
 
+InputTypeDef = TypedDict(
+    "InputTypeDef",
+    {
+        "inputConfiguration": InputConfigurationTypeDef,
+        "inputDefinition": InputDefinitionTypeDef,
+    },
+    total=False,
+)
 
-InputDefinitionUnionTypeDef = Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef]
 _RequiredUpdateInputRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInputRequestRequestTypeDef",
     {
         "inputName": str,
         "inputDefinition": InputDefinitionTypeDef,
     },
 )
@@ -1164,30 +1072,27 @@
     "_OptionalUpdateInputRequestRequestTypeDef",
     {
         "inputDescription": str,
     },
     total=False,
 )
 
-
 class UpdateInputRequestRequestTypeDef(
     _RequiredUpdateInputRequestRequestTypeDef, _OptionalUpdateInputRequestRequestTypeDef
 ):
     pass
 
-
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
-        "loggingOptions": LoggingOptionsOutputTypeDef,
+        "loggingOptions": LoggingOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoggingOptionsUnionTypeDef = Union[LoggingOptionsTypeDef, LoggingOptionsOutputTypeDef]
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
     },
 )
 
@@ -1204,52 +1109,22 @@
     {
         "iotEventsInputIdentifier": IotEventsInputIdentifierTypeDef,
         "iotSiteWiseInputIdentifier": IotSiteWiseInputIdentifierTypeDef,
     },
     total=False,
 )
 
-EmailRecipientsOutputTypeDef = TypedDict(
-    "EmailRecipientsOutputTypeDef",
-    {
-        "to": List[RecipientDetailTypeDef],
-    },
-    total=False,
-)
-
 EmailRecipientsTypeDef = TypedDict(
     "EmailRecipientsTypeDef",
     {
         "to": Sequence[RecipientDetailTypeDef],
     },
     total=False,
 )
 
-_RequiredSMSConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSMSConfigurationOutputTypeDef",
-    {
-        "recipients": List[RecipientDetailTypeDef],
-    },
-)
-_OptionalSMSConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSMSConfigurationOutputTypeDef",
-    {
-        "senderId": str,
-        "additionalMessage": str,
-    },
-    total=False,
-)
-
-
-class SMSConfigurationOutputTypeDef(
-    _RequiredSMSConfigurationOutputTypeDef, _OptionalSMSConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredSMSConfigurationTypeDef = TypedDict(
     "_RequiredSMSConfigurationTypeDef",
     {
         "recipients": Sequence[RecipientDetailTypeDef],
     },
 )
 _OptionalSMSConfigurationTypeDef = TypedDict(
@@ -1257,19 +1132,17 @@
     {
         "senderId": str,
         "additionalMessage": str,
     },
     total=False,
 )
 
-
 class SMSConfigurationTypeDef(_RequiredSMSConfigurationTypeDef, _OptionalSMSConfigurationTypeDef):
     pass
 
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "setVariable": SetVariableActionTypeDef,
         "sns": SNSTopicPublishActionTypeDef,
         "iotTopicPublish": IotTopicPublishActionTypeDef,
         "setTimer": SetTimerActionTypeDef,
@@ -1321,43 +1194,19 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListInputRoutingsRequestRequestTypeDef(
     _RequiredListInputRoutingsRequestRequestTypeDef, _OptionalListInputRoutingsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredEmailConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEmailConfigurationOutputTypeDef",
-    {
-        "from": str,
-        "recipients": EmailRecipientsOutputTypeDef,
-    },
-)
-_OptionalEmailConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEmailConfigurationOutputTypeDef",
-    {
-        "content": EmailContentTypeDef,
-    },
-    total=False,
-)
-
-
-class EmailConfigurationOutputTypeDef(
-    _RequiredEmailConfigurationOutputTypeDef, _OptionalEmailConfigurationOutputTypeDef
-):
-    pass
-
-
 _RequiredEmailConfigurationTypeDef = TypedDict(
     "_RequiredEmailConfigurationTypeDef",
     {
         "from": str,
         "recipients": EmailRecipientsTypeDef,
     },
 )
@@ -1365,41 +1214,19 @@
     "_OptionalEmailConfigurationTypeDef",
     {
         "content": EmailContentTypeDef,
     },
     total=False,
 )
 
-
 class EmailConfigurationTypeDef(
     _RequiredEmailConfigurationTypeDef, _OptionalEmailConfigurationTypeDef
 ):
     pass
 
-
-_RequiredEventOutputTypeDef = TypedDict(
-    "_RequiredEventOutputTypeDef",
-    {
-        "eventName": str,
-    },
-)
-_OptionalEventOutputTypeDef = TypedDict(
-    "_OptionalEventOutputTypeDef",
-    {
-        "condition": str,
-        "actions": List[ActionTypeDef],
-    },
-    total=False,
-)
-
-
-class EventOutputTypeDef(_RequiredEventOutputTypeDef, _OptionalEventOutputTypeDef):
-    pass
-
-
 _RequiredEventTypeDef = TypedDict(
     "_RequiredEventTypeDef",
     {
         "eventName": str,
     },
 )
 _OptionalEventTypeDef = TypedDict(
@@ -1407,42 +1234,17 @@
     {
         "condition": str,
         "actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
-
 class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
-
-_RequiredTransitionEventOutputTypeDef = TypedDict(
-    "_RequiredTransitionEventOutputTypeDef",
-    {
-        "eventName": str,
-        "condition": str,
-        "nextState": str,
-    },
-)
-_OptionalTransitionEventOutputTypeDef = TypedDict(
-    "_OptionalTransitionEventOutputTypeDef",
-    {
-        "actions": List[ActionTypeDef],
-    },
-    total=False,
-)
-
-
-class TransitionEventOutputTypeDef(
-    _RequiredTransitionEventOutputTypeDef, _OptionalTransitionEventOutputTypeDef
-):
-    pass
-
-
 _RequiredTransitionEventTypeDef = TypedDict(
     "_RequiredTransitionEventTypeDef",
     {
         "eventName": str,
         "condition": str,
         "nextState": str,
     },
@@ -1451,57 +1253,25 @@
     "_OptionalTransitionEventTypeDef",
     {
         "actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
-
 class TransitionEventTypeDef(_RequiredTransitionEventTypeDef, _OptionalTransitionEventTypeDef):
     pass
 
-
-AlarmEventActionsOutputTypeDef = TypedDict(
-    "AlarmEventActionsOutputTypeDef",
-    {
-        "alarmActions": List[AlarmActionTypeDef],
-    },
-    total=False,
-)
-
 AlarmEventActionsTypeDef = TypedDict(
     "AlarmEventActionsTypeDef",
     {
         "alarmActions": Sequence[AlarmActionTypeDef],
     },
     total=False,
 )
 
-_RequiredNotificationActionOutputTypeDef = TypedDict(
-    "_RequiredNotificationActionOutputTypeDef",
-    {
-        "action": NotificationTargetActionsTypeDef,
-    },
-)
-_OptionalNotificationActionOutputTypeDef = TypedDict(
-    "_OptionalNotificationActionOutputTypeDef",
-    {
-        "smsConfigurations": List[SMSConfigurationOutputTypeDef],
-        "emailConfigurations": List[EmailConfigurationOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class NotificationActionOutputTypeDef(
-    _RequiredNotificationActionOutputTypeDef, _OptionalNotificationActionOutputTypeDef
-):
-    pass
-
-
 _RequiredNotificationActionTypeDef = TypedDict(
     "_RequiredNotificationActionTypeDef",
     {
         "action": NotificationTargetActionsTypeDef,
     },
 )
 _OptionalNotificationActionTypeDef = TypedDict(
@@ -1509,37 +1279,19 @@
     {
         "smsConfigurations": Sequence[SMSConfigurationTypeDef],
         "emailConfigurations": Sequence[EmailConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class NotificationActionTypeDef(
     _RequiredNotificationActionTypeDef, _OptionalNotificationActionTypeDef
 ):
     pass
 
-
-OnEnterLifecycleOutputTypeDef = TypedDict(
-    "OnEnterLifecycleOutputTypeDef",
-    {
-        "events": List[EventOutputTypeDef],
-    },
-    total=False,
-)
-
-OnExitLifecycleOutputTypeDef = TypedDict(
-    "OnExitLifecycleOutputTypeDef",
-    {
-        "events": List[EventOutputTypeDef],
-    },
-    total=False,
-)
-
 OnEnterLifecycleTypeDef = TypedDict(
     "OnEnterLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
     },
     total=False,
 )
@@ -1548,70 +1300,31 @@
     "OnExitLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
     },
     total=False,
 )
 
-OnInputLifecycleOutputTypeDef = TypedDict(
-    "OnInputLifecycleOutputTypeDef",
-    {
-        "events": List[EventOutputTypeDef],
-        "transitionEvents": List[TransitionEventOutputTypeDef],
-    },
-    total=False,
-)
-
 OnInputLifecycleTypeDef = TypedDict(
     "OnInputLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
         "transitionEvents": Sequence[TransitionEventTypeDef],
     },
     total=False,
 )
 
-AlarmEventActionsUnionTypeDef = Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef]
-AlarmNotificationOutputTypeDef = TypedDict(
-    "AlarmNotificationOutputTypeDef",
-    {
-        "notificationActions": List[NotificationActionOutputTypeDef],
-    },
-    total=False,
-)
-
 AlarmNotificationTypeDef = TypedDict(
     "AlarmNotificationTypeDef",
     {
         "notificationActions": Sequence[NotificationActionTypeDef],
     },
     total=False,
 )
 
-_RequiredStateOutputTypeDef = TypedDict(
-    "_RequiredStateOutputTypeDef",
-    {
-        "stateName": str,
-    },
-)
-_OptionalStateOutputTypeDef = TypedDict(
-    "_OptionalStateOutputTypeDef",
-    {
-        "onInput": OnInputLifecycleOutputTypeDef,
-        "onEnter": OnEnterLifecycleOutputTypeDef,
-        "onExit": OnExitLifecycleOutputTypeDef,
-    },
-    total=False,
-)
-
-
-class StateOutputTypeDef(_RequiredStateOutputTypeDef, _OptionalStateOutputTypeDef):
-    pass
-
-
 _RequiredStateTypeDef = TypedDict(
     "_RequiredStateTypeDef",
     {
         "stateName": str,
     },
 )
 _OptionalStateTypeDef = TypedDict(
@@ -1620,42 +1333,17 @@
         "onInput": OnInputLifecycleTypeDef,
         "onEnter": OnEnterLifecycleTypeDef,
         "onExit": OnExitLifecycleTypeDef,
     },
     total=False,
 )
 
-
 class StateTypeDef(_RequiredStateTypeDef, _OptionalStateTypeDef):
     pass
 
-
-DescribeAlarmModelResponseTypeDef = TypedDict(
-    "DescribeAlarmModelResponseTypeDef",
-    {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "statusMessage": str,
-        "alarmModelName": str,
-        "alarmModelDescription": str,
-        "roleArn": str,
-        "key": str,
-        "severity": int,
-        "alarmRule": AlarmRuleTypeDef,
-        "alarmNotification": AlarmNotificationOutputTypeDef,
-        "alarmEventActions": AlarmEventActionsOutputTypeDef,
-        "alarmCapabilities": AlarmCapabilitiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-AlarmNotificationUnionTypeDef = Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef]
 _RequiredCreateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
         "roleArn": str,
         "alarmRule": AlarmRuleTypeDef,
     },
@@ -1670,20 +1358,40 @@
         "alarmNotification": AlarmNotificationTypeDef,
         "alarmEventActions": AlarmEventActionsTypeDef,
         "alarmCapabilities": AlarmCapabilitiesTypeDef,
     },
     total=False,
 )
 
-
 class CreateAlarmModelRequestRequestTypeDef(
     _RequiredCreateAlarmModelRequestRequestTypeDef, _OptionalCreateAlarmModelRequestRequestTypeDef
 ):
     pass
 
+DescribeAlarmModelResponseTypeDef = TypedDict(
+    "DescribeAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "statusMessage": str,
+        "alarmModelName": str,
+        "alarmModelDescription": str,
+        "roleArn": str,
+        "key": str,
+        "severity": int,
+        "alarmRule": AlarmRuleTypeDef,
+        "alarmNotification": AlarmNotificationTypeDef,
+        "alarmEventActions": AlarmEventActionsTypeDef,
+        "alarmCapabilities": AlarmCapabilitiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredUpdateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
         "roleArn": str,
         "alarmRule": AlarmRuleTypeDef,
@@ -1697,46 +1405,27 @@
         "alarmNotification": AlarmNotificationTypeDef,
         "alarmEventActions": AlarmEventActionsTypeDef,
         "alarmCapabilities": AlarmCapabilitiesTypeDef,
     },
     total=False,
 )
 
-
 class UpdateAlarmModelRequestRequestTypeDef(
     _RequiredUpdateAlarmModelRequestRequestTypeDef, _OptionalUpdateAlarmModelRequestRequestTypeDef
 ):
     pass
 
-
-DetectorModelDefinitionOutputTypeDef = TypedDict(
-    "DetectorModelDefinitionOutputTypeDef",
-    {
-        "states": List[StateOutputTypeDef],
-        "initialStateName": str,
-    },
-)
-
 DetectorModelDefinitionTypeDef = TypedDict(
     "DetectorModelDefinitionTypeDef",
     {
         "states": Sequence[StateTypeDef],
         "initialStateName": str,
     },
 )
 
-DetectorModelTypeDef = TypedDict(
-    "DetectorModelTypeDef",
-    {
-        "detectorModelDefinition": DetectorModelDefinitionOutputTypeDef,
-        "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateDetectorModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDetectorModelRequestRequestTypeDef",
     {
         "detectorModelName": str,
         "detectorModelDefinition": DetectorModelDefinitionTypeDef,
         "roleArn": str,
     },
@@ -1748,25 +1437,29 @@
         "key": str,
         "tags": Sequence[TagTypeDef],
         "evaluationMethod": EvaluationMethodType,
     },
     total=False,
 )
 
-
 class CreateDetectorModelRequestRequestTypeDef(
     _RequiredCreateDetectorModelRequestRequestTypeDef,
     _OptionalCreateDetectorModelRequestRequestTypeDef,
 ):
     pass
 
+DetectorModelTypeDef = TypedDict(
+    "DetectorModelTypeDef",
+    {
+        "detectorModelDefinition": DetectorModelDefinitionTypeDef,
+        "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
+    },
+    total=False,
+)
 
-DetectorModelDefinitionUnionTypeDef = Union[
-    DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
-]
 StartDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     {
         "detectorModelDefinition": DetectorModelDefinitionTypeDef,
     },
 )
 
@@ -1783,22 +1476,20 @@
     {
         "detectorModelDescription": str,
         "evaluationMethod": EvaluationMethodType,
     },
     total=False,
 )
 
-
 class UpdateDetectorModelRequestRequestTypeDef(
     _RequiredUpdateDetectorModelRequestRequestTypeDef,
     _OptionalUpdateDetectorModelRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeDetectorModelResponseTypeDef = TypedDict(
     "DescribeDetectorModelResponseTypeDef",
     {
         "detectorModel": DetectorModelTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents/type_defs.pyi` & `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents/type_defs.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_iotevents.type_defs import AcknowledgeFlowTypeDef
 
     data: AcknowledgeFlowTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Sequence
 
 from .literals import (
     AlarmModelVersionStatusType,
     AnalysisResultLevelType,
     AnalysisStatusType,
     ComparisonOperatorType,
     DetectorModelVersionStatusType,
@@ -28,14 +28,15 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AcknowledgeFlowTypeDef",
     "ClearTimerActionTypeDef",
     "ResetTimerActionTypeDef",
     "SetTimerActionTypeDef",
     "SetVariableActionTypeDef",
     "InitializationConfigurationTypeDef",
@@ -75,30 +76,28 @@
     "ListTagsForResourceRequestRequestTypeDef",
     "SSOIdentityTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AlarmCapabilitiesTypeDef",
     "AlarmRuleTypeDef",
     "AnalysisResultTypeDef",
     "AssetPropertyValueTypeDef",
-    "InputDefinitionOutputTypeDef",
     "InputDefinitionTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateAlarmModelResponseTypeDef",
     "DescribeDetectorModelAnalysisResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "ListAlarmModelVersionsResponseTypeDef",
     "ListAlarmModelsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "StartDetectorModelAnalysisResponseTypeDef",
     "UpdateAlarmModelResponseTypeDef",
     "CreateDetectorModelResponseTypeDef",
     "UpdateDetectorModelResponseTypeDef",
     "CreateInputResponseTypeDef",
     "UpdateInputResponseTypeDef",
-    "LoggingOptionsOutputTypeDef",
     "LoggingOptionsTypeDef",
     "ListDetectorModelsResponseTypeDef",
     "ListDetectorModelVersionsResponseTypeDef",
     "DynamoDBActionTypeDef",
     "DynamoDBv2ActionTypeDef",
     "FirehoseActionTypeDef",
     "IotEventsActionTypeDef",
@@ -108,61 +107,43 @@
     "SqsActionTypeDef",
     "ListInputsResponseTypeDef",
     "IotSiteWiseInputIdentifierTypeDef",
     "ListInputRoutingsResponseTypeDef",
     "RecipientDetailTypeDef",
     "GetDetectorModelAnalysisResultsResponseTypeDef",
     "IotSiteWiseActionTypeDef",
-    "InputTypeDef",
     "CreateInputRequestRequestTypeDef",
-    "InputDefinitionUnionTypeDef",
+    "InputTypeDef",
     "UpdateInputRequestRequestTypeDef",
     "DescribeLoggingOptionsResponseTypeDef",
-    "LoggingOptionsUnionTypeDef",
     "PutLoggingOptionsRequestRequestTypeDef",
     "NotificationTargetActionsTypeDef",
     "InputIdentifierTypeDef",
-    "EmailRecipientsOutputTypeDef",
     "EmailRecipientsTypeDef",
-    "SMSConfigurationOutputTypeDef",
     "SMSConfigurationTypeDef",
     "ActionTypeDef",
     "AlarmActionTypeDef",
     "DescribeInputResponseTypeDef",
     "ListInputRoutingsRequestRequestTypeDef",
-    "EmailConfigurationOutputTypeDef",
     "EmailConfigurationTypeDef",
-    "EventOutputTypeDef",
     "EventTypeDef",
-    "TransitionEventOutputTypeDef",
     "TransitionEventTypeDef",
-    "AlarmEventActionsOutputTypeDef",
     "AlarmEventActionsTypeDef",
-    "NotificationActionOutputTypeDef",
     "NotificationActionTypeDef",
-    "OnEnterLifecycleOutputTypeDef",
-    "OnExitLifecycleOutputTypeDef",
     "OnEnterLifecycleTypeDef",
     "OnExitLifecycleTypeDef",
-    "OnInputLifecycleOutputTypeDef",
     "OnInputLifecycleTypeDef",
-    "AlarmEventActionsUnionTypeDef",
-    "AlarmNotificationOutputTypeDef",
     "AlarmNotificationTypeDef",
-    "StateOutputTypeDef",
     "StateTypeDef",
-    "DescribeAlarmModelResponseTypeDef",
-    "AlarmNotificationUnionTypeDef",
     "CreateAlarmModelRequestRequestTypeDef",
+    "DescribeAlarmModelResponseTypeDef",
     "UpdateAlarmModelRequestRequestTypeDef",
-    "DetectorModelDefinitionOutputTypeDef",
     "DetectorModelDefinitionTypeDef",
-    "DetectorModelTypeDef",
     "CreateDetectorModelRequestRequestTypeDef",
-    "DetectorModelDefinitionUnionTypeDef",
+    "DetectorModelTypeDef",
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     "UpdateDetectorModelRequestRequestTypeDef",
     "DescribeDetectorModelResponseTypeDef",
 )
 
 AcknowledgeFlowTypeDef = TypedDict(
     "AcknowledgeFlowTypeDef",
@@ -196,17 +177,19 @@
     {
         "seconds": int,
         "durationExpression": str,
     },
     total=False,
 )
 
+
 class SetTimerActionTypeDef(_RequiredSetTimerActionTypeDef, _OptionalSetTimerActionTypeDef):
     pass
 
+
 SetVariableActionTypeDef = TypedDict(
     "SetVariableActionTypeDef",
     {
         "variableName": str,
         "value": str,
     },
 )
@@ -270,19 +253,21 @@
     "_OptionalAssetPropertyTimestampTypeDef",
     {
         "offsetInNanos": str,
     },
     total=False,
 )
 
+
 class AssetPropertyTimestampTypeDef(
     _RequiredAssetPropertyTimestampTypeDef, _OptionalAssetPropertyTimestampTypeDef
 ):
     pass
 
+
 AssetPropertyVariantTypeDef = TypedDict(
     "AssetPropertyVariantTypeDef",
     {
         "stringValue": str,
         "integerValue": str,
         "doubleValue": str,
         "booleanValue": str,
@@ -347,19 +332,21 @@
     "_OptionalInputConfigurationTypeDef",
     {
         "inputDescription": str,
     },
     total=False,
 )
 
+
 class InputConfigurationTypeDef(
     _RequiredInputConfigurationTypeDef, _OptionalInputConfigurationTypeDef
 ):
     pass
 
+
 DeleteAlarmModelRequestRequestTypeDef = TypedDict(
     "DeleteAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
     },
 )
 
@@ -387,20 +374,22 @@
     "_OptionalDescribeAlarmModelRequestRequestTypeDef",
     {
         "alarmModelVersion": str,
     },
     total=False,
 )
 
+
 class DescribeAlarmModelRequestRequestTypeDef(
     _RequiredDescribeAlarmModelRequestRequestTypeDef,
     _OptionalDescribeAlarmModelRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeDetectorModelAnalysisRequestRequestTypeDef",
     {
         "analysisId": str,
     },
 )
 
@@ -414,20 +403,22 @@
     "_OptionalDescribeDetectorModelRequestRequestTypeDef",
     {
         "detectorModelVersion": str,
     },
     total=False,
 )
 
+
 class DescribeDetectorModelRequestRequestTypeDef(
     _RequiredDescribeDetectorModelRequestRequestTypeDef,
     _OptionalDescribeDetectorModelRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeInputRequestRequestTypeDef = TypedDict(
     "DescribeInputRequestRequestTypeDef",
     {
         "inputName": str,
     },
 )
 
@@ -441,19 +432,21 @@
     "_OptionalDetectorDebugOptionTypeDef",
     {
         "keyValue": str,
     },
     total=False,
 )
 
+
 class DetectorDebugOptionTypeDef(
     _RequiredDetectorDebugOptionTypeDef, _OptionalDetectorDebugOptionTypeDef
 ):
     pass
 
+
 DetectorModelSummaryTypeDef = TypedDict(
     "DetectorModelSummaryTypeDef",
     {
         "detectorModelName": str,
         "detectorModelDescription": str,
         "creationTime": datetime,
     },
@@ -503,20 +496,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class GetDetectorModelAnalysisResultsRequestRequestTypeDef(
     _RequiredGetDetectorModelAnalysisResultsRequestRequestTypeDef,
     _OptionalGetDetectorModelAnalysisResultsRequestRequestTypeDef,
 ):
     pass
 
+
 IotEventsInputIdentifierTypeDef = TypedDict(
     "IotEventsInputIdentifierTypeDef",
     {
         "inputName": str,
     },
 )
 
@@ -552,20 +547,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListAlarmModelVersionsRequestRequestTypeDef(
     _RequiredListAlarmModelVersionsRequestRequestTypeDef,
     _OptionalListAlarmModelVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListAlarmModelsRequestRequestTypeDef = TypedDict(
     "ListAlarmModelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -582,20 +579,22 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+
 class ListDetectorModelVersionsRequestRequestTypeDef(
     _RequiredListDetectorModelVersionsRequestRequestTypeDef,
     _OptionalListDetectorModelVersionsRequestRequestTypeDef,
 ):
     pass
 
+
 ListDetectorModelsRequestRequestTypeDef = TypedDict(
     "ListDetectorModelsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
@@ -636,17 +635,19 @@
     "_OptionalSSOIdentityTypeDef",
     {
         "userId": str,
     },
     total=False,
 )
 
+
 class SSOIdentityTypeDef(_RequiredSSOIdentityTypeDef, _OptionalSSOIdentityTypeDef):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -685,21 +686,14 @@
         "value": AssetPropertyVariantTypeDef,
         "timestamp": AssetPropertyTimestampTypeDef,
         "quality": str,
     },
     total=False,
 )
 
-InputDefinitionOutputTypeDef = TypedDict(
-    "InputDefinitionOutputTypeDef",
-    {
-        "attributes": List[AttributeTypeDef],
-    },
-)
-
 InputDefinitionTypeDef = TypedDict(
     "InputDefinitionTypeDef",
     {
         "attributes": Sequence[AttributeTypeDef],
     },
 )
 
@@ -812,54 +806,35 @@
     "UpdateInputResponseTypeDef",
     {
         "inputConfiguration": InputConfigurationTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredLoggingOptionsOutputTypeDef = TypedDict(
-    "_RequiredLoggingOptionsOutputTypeDef",
-    {
-        "roleArn": str,
-        "level": LoggingLevelType,
-        "enabled": bool,
-    },
-)
-_OptionalLoggingOptionsOutputTypeDef = TypedDict(
-    "_OptionalLoggingOptionsOutputTypeDef",
-    {
-        "detectorDebugOptions": List[DetectorDebugOptionTypeDef],
-    },
-    total=False,
-)
-
-class LoggingOptionsOutputTypeDef(
-    _RequiredLoggingOptionsOutputTypeDef, _OptionalLoggingOptionsOutputTypeDef
-):
-    pass
-
 _RequiredLoggingOptionsTypeDef = TypedDict(
     "_RequiredLoggingOptionsTypeDef",
     {
         "roleArn": str,
         "level": LoggingLevelType,
         "enabled": bool,
     },
 )
 _OptionalLoggingOptionsTypeDef = TypedDict(
     "_OptionalLoggingOptionsTypeDef",
     {
-        "detectorDebugOptions": Sequence[DetectorDebugOptionTypeDef],
+        "detectorDebugOptions": List[DetectorDebugOptionTypeDef],
     },
     total=False,
 )
 
+
 class LoggingOptionsTypeDef(_RequiredLoggingOptionsTypeDef, _OptionalLoggingOptionsTypeDef):
     pass
 
+
 ListDetectorModelsResponseTypeDef = TypedDict(
     "ListDetectorModelsResponseTypeDef",
     {
         "detectorModelSummaries": List[DetectorModelSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -892,34 +867,38 @@
         "operation": str,
         "payloadField": str,
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
+
 class DynamoDBActionTypeDef(_RequiredDynamoDBActionTypeDef, _OptionalDynamoDBActionTypeDef):
     pass
 
+
 _RequiredDynamoDBv2ActionTypeDef = TypedDict(
     "_RequiredDynamoDBv2ActionTypeDef",
     {
         "tableName": str,
     },
 )
 _OptionalDynamoDBv2ActionTypeDef = TypedDict(
     "_OptionalDynamoDBv2ActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
+
 class DynamoDBv2ActionTypeDef(_RequiredDynamoDBv2ActionTypeDef, _OptionalDynamoDBv2ActionTypeDef):
     pass
 
+
 _RequiredFirehoseActionTypeDef = TypedDict(
     "_RequiredFirehoseActionTypeDef",
     {
         "deliveryStreamName": str,
     },
 )
 _OptionalFirehoseActionTypeDef = TypedDict(
@@ -927,89 +906,99 @@
     {
         "separator": str,
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
+
 class FirehoseActionTypeDef(_RequiredFirehoseActionTypeDef, _OptionalFirehoseActionTypeDef):
     pass
 
+
 _RequiredIotEventsActionTypeDef = TypedDict(
     "_RequiredIotEventsActionTypeDef",
     {
         "inputName": str,
     },
 )
 _OptionalIotEventsActionTypeDef = TypedDict(
     "_OptionalIotEventsActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
+
 class IotEventsActionTypeDef(_RequiredIotEventsActionTypeDef, _OptionalIotEventsActionTypeDef):
     pass
 
+
 _RequiredIotTopicPublishActionTypeDef = TypedDict(
     "_RequiredIotTopicPublishActionTypeDef",
     {
         "mqttTopic": str,
     },
 )
 _OptionalIotTopicPublishActionTypeDef = TypedDict(
     "_OptionalIotTopicPublishActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
+
 class IotTopicPublishActionTypeDef(
     _RequiredIotTopicPublishActionTypeDef, _OptionalIotTopicPublishActionTypeDef
 ):
     pass
 
+
 _RequiredLambdaActionTypeDef = TypedDict(
     "_RequiredLambdaActionTypeDef",
     {
         "functionArn": str,
     },
 )
 _OptionalLambdaActionTypeDef = TypedDict(
     "_OptionalLambdaActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
+
 class LambdaActionTypeDef(_RequiredLambdaActionTypeDef, _OptionalLambdaActionTypeDef):
     pass
 
+
 _RequiredSNSTopicPublishActionTypeDef = TypedDict(
     "_RequiredSNSTopicPublishActionTypeDef",
     {
         "targetArn": str,
     },
 )
 _OptionalSNSTopicPublishActionTypeDef = TypedDict(
     "_OptionalSNSTopicPublishActionTypeDef",
     {
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
+
 class SNSTopicPublishActionTypeDef(
     _RequiredSNSTopicPublishActionTypeDef, _OptionalSNSTopicPublishActionTypeDef
 ):
     pass
 
+
 _RequiredSqsActionTypeDef = TypedDict(
     "_RequiredSqsActionTypeDef",
     {
         "queueUrl": str,
     },
 )
 _OptionalSqsActionTypeDef = TypedDict(
@@ -1017,17 +1006,19 @@
     {
         "useBase64": bool,
         "payload": PayloadTypeDef,
     },
     total=False,
 )
 
+
 class SqsActionTypeDef(_RequiredSqsActionTypeDef, _OptionalSqsActionTypeDef):
     pass
 
+
 ListInputsResponseTypeDef = TypedDict(
     "ListInputsResponseTypeDef",
     {
         "inputSummaries": List[InputSummaryTypeDef],
         "nextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1075,23 +1066,14 @@
         "propertyId": str,
         "propertyAlias": str,
         "propertyValue": AssetPropertyValueTypeDef,
     },
     total=False,
 )
 
-InputTypeDef = TypedDict(
-    "InputTypeDef",
-    {
-        "inputConfiguration": InputConfigurationTypeDef,
-        "inputDefinition": InputDefinitionOutputTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateInputRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInputRequestRequestTypeDef",
     {
         "inputName": str,
         "inputDefinition": InputDefinitionTypeDef,
     },
 )
@@ -1100,20 +1082,30 @@
     {
         "inputDescription": str,
         "tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateInputRequestRequestTypeDef(
     _RequiredCreateInputRequestRequestTypeDef, _OptionalCreateInputRequestRequestTypeDef
 ):
     pass
 
-InputDefinitionUnionTypeDef = Union[InputDefinitionTypeDef, InputDefinitionOutputTypeDef]
+
+InputTypeDef = TypedDict(
+    "InputTypeDef",
+    {
+        "inputConfiguration": InputConfigurationTypeDef,
+        "inputDefinition": InputDefinitionTypeDef,
+    },
+    total=False,
+)
+
 _RequiredUpdateInputRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateInputRequestRequestTypeDef",
     {
         "inputName": str,
         "inputDefinition": InputDefinitionTypeDef,
     },
 )
@@ -1121,28 +1113,29 @@
     "_OptionalUpdateInputRequestRequestTypeDef",
     {
         "inputDescription": str,
     },
     total=False,
 )
 
+
 class UpdateInputRequestRequestTypeDef(
     _RequiredUpdateInputRequestRequestTypeDef, _OptionalUpdateInputRequestRequestTypeDef
 ):
     pass
 
+
 DescribeLoggingOptionsResponseTypeDef = TypedDict(
     "DescribeLoggingOptionsResponseTypeDef",
     {
-        "loggingOptions": LoggingOptionsOutputTypeDef,
+        "loggingOptions": LoggingOptionsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LoggingOptionsUnionTypeDef = Union[LoggingOptionsTypeDef, LoggingOptionsOutputTypeDef]
 PutLoggingOptionsRequestRequestTypeDef = TypedDict(
     "PutLoggingOptionsRequestRequestTypeDef",
     {
         "loggingOptions": LoggingOptionsTypeDef,
     },
 )
 
@@ -1159,50 +1152,22 @@
     {
         "iotEventsInputIdentifier": IotEventsInputIdentifierTypeDef,
         "iotSiteWiseInputIdentifier": IotSiteWiseInputIdentifierTypeDef,
     },
     total=False,
 )
 
-EmailRecipientsOutputTypeDef = TypedDict(
-    "EmailRecipientsOutputTypeDef",
-    {
-        "to": List[RecipientDetailTypeDef],
-    },
-    total=False,
-)
-
 EmailRecipientsTypeDef = TypedDict(
     "EmailRecipientsTypeDef",
     {
         "to": Sequence[RecipientDetailTypeDef],
     },
     total=False,
 )
 
-_RequiredSMSConfigurationOutputTypeDef = TypedDict(
-    "_RequiredSMSConfigurationOutputTypeDef",
-    {
-        "recipients": List[RecipientDetailTypeDef],
-    },
-)
-_OptionalSMSConfigurationOutputTypeDef = TypedDict(
-    "_OptionalSMSConfigurationOutputTypeDef",
-    {
-        "senderId": str,
-        "additionalMessage": str,
-    },
-    total=False,
-)
-
-class SMSConfigurationOutputTypeDef(
-    _RequiredSMSConfigurationOutputTypeDef, _OptionalSMSConfigurationOutputTypeDef
-):
-    pass
-
 _RequiredSMSConfigurationTypeDef = TypedDict(
     "_RequiredSMSConfigurationTypeDef",
     {
         "recipients": Sequence[RecipientDetailTypeDef],
     },
 )
 _OptionalSMSConfigurationTypeDef = TypedDict(
@@ -1210,17 +1175,19 @@
     {
         "senderId": str,
         "additionalMessage": str,
     },
     total=False,
 )
 
+
 class SMSConfigurationTypeDef(_RequiredSMSConfigurationTypeDef, _OptionalSMSConfigurationTypeDef):
     pass
 
+
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "setVariable": SetVariableActionTypeDef,
         "sns": SNSTopicPublishActionTypeDef,
         "iotTopicPublish": IotTopicPublishActionTypeDef,
         "setTimer": SetTimerActionTypeDef,
@@ -1272,38 +1239,20 @@
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListInputRoutingsRequestRequestTypeDef(
     _RequiredListInputRoutingsRequestRequestTypeDef, _OptionalListInputRoutingsRequestRequestTypeDef
 ):
     pass
 
-_RequiredEmailConfigurationOutputTypeDef = TypedDict(
-    "_RequiredEmailConfigurationOutputTypeDef",
-    {
-        "from": str,
-        "recipients": EmailRecipientsOutputTypeDef,
-    },
-)
-_OptionalEmailConfigurationOutputTypeDef = TypedDict(
-    "_OptionalEmailConfigurationOutputTypeDef",
-    {
-        "content": EmailContentTypeDef,
-    },
-    total=False,
-)
-
-class EmailConfigurationOutputTypeDef(
-    _RequiredEmailConfigurationOutputTypeDef, _OptionalEmailConfigurationOutputTypeDef
-):
-    pass
 
 _RequiredEmailConfigurationTypeDef = TypedDict(
     "_RequiredEmailConfigurationTypeDef",
     {
         "from": str,
         "recipients": EmailRecipientsTypeDef,
     },
@@ -1312,36 +1261,20 @@
     "_OptionalEmailConfigurationTypeDef",
     {
         "content": EmailContentTypeDef,
     },
     total=False,
 )
 
+
 class EmailConfigurationTypeDef(
     _RequiredEmailConfigurationTypeDef, _OptionalEmailConfigurationTypeDef
 ):
     pass
 
-_RequiredEventOutputTypeDef = TypedDict(
-    "_RequiredEventOutputTypeDef",
-    {
-        "eventName": str,
-    },
-)
-_OptionalEventOutputTypeDef = TypedDict(
-    "_OptionalEventOutputTypeDef",
-    {
-        "condition": str,
-        "actions": List[ActionTypeDef],
-    },
-    total=False,
-)
-
-class EventOutputTypeDef(_RequiredEventOutputTypeDef, _OptionalEventOutputTypeDef):
-    pass
 
 _RequiredEventTypeDef = TypedDict(
     "_RequiredEventTypeDef",
     {
         "eventName": str,
     },
 )
@@ -1350,37 +1283,18 @@
     {
         "condition": str,
         "actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
+
 class EventTypeDef(_RequiredEventTypeDef, _OptionalEventTypeDef):
     pass
 
-_RequiredTransitionEventOutputTypeDef = TypedDict(
-    "_RequiredTransitionEventOutputTypeDef",
-    {
-        "eventName": str,
-        "condition": str,
-        "nextState": str,
-    },
-)
-_OptionalTransitionEventOutputTypeDef = TypedDict(
-    "_OptionalTransitionEventOutputTypeDef",
-    {
-        "actions": List[ActionTypeDef],
-    },
-    total=False,
-)
-
-class TransitionEventOutputTypeDef(
-    _RequiredTransitionEventOutputTypeDef, _OptionalTransitionEventOutputTypeDef
-):
-    pass
 
 _RequiredTransitionEventTypeDef = TypedDict(
     "_RequiredTransitionEventTypeDef",
     {
         "eventName": str,
         "condition": str,
         "nextState": str,
@@ -1390,53 +1304,27 @@
     "_OptionalTransitionEventTypeDef",
     {
         "actions": Sequence[ActionTypeDef],
     },
     total=False,
 )
 
+
 class TransitionEventTypeDef(_RequiredTransitionEventTypeDef, _OptionalTransitionEventTypeDef):
     pass
 
-AlarmEventActionsOutputTypeDef = TypedDict(
-    "AlarmEventActionsOutputTypeDef",
-    {
-        "alarmActions": List[AlarmActionTypeDef],
-    },
-    total=False,
-)
 
 AlarmEventActionsTypeDef = TypedDict(
     "AlarmEventActionsTypeDef",
     {
         "alarmActions": Sequence[AlarmActionTypeDef],
     },
     total=False,
 )
 
-_RequiredNotificationActionOutputTypeDef = TypedDict(
-    "_RequiredNotificationActionOutputTypeDef",
-    {
-        "action": NotificationTargetActionsTypeDef,
-    },
-)
-_OptionalNotificationActionOutputTypeDef = TypedDict(
-    "_OptionalNotificationActionOutputTypeDef",
-    {
-        "smsConfigurations": List[SMSConfigurationOutputTypeDef],
-        "emailConfigurations": List[EmailConfigurationOutputTypeDef],
-    },
-    total=False,
-)
-
-class NotificationActionOutputTypeDef(
-    _RequiredNotificationActionOutputTypeDef, _OptionalNotificationActionOutputTypeDef
-):
-    pass
-
 _RequiredNotificationActionTypeDef = TypedDict(
     "_RequiredNotificationActionTypeDef",
     {
         "action": NotificationTargetActionsTypeDef,
     },
 )
 _OptionalNotificationActionTypeDef = TypedDict(
@@ -1444,34 +1332,20 @@
     {
         "smsConfigurations": Sequence[SMSConfigurationTypeDef],
         "emailConfigurations": Sequence[EmailConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class NotificationActionTypeDef(
     _RequiredNotificationActionTypeDef, _OptionalNotificationActionTypeDef
 ):
     pass
 
-OnEnterLifecycleOutputTypeDef = TypedDict(
-    "OnEnterLifecycleOutputTypeDef",
-    {
-        "events": List[EventOutputTypeDef],
-    },
-    total=False,
-)
-
-OnExitLifecycleOutputTypeDef = TypedDict(
-    "OnExitLifecycleOutputTypeDef",
-    {
-        "events": List[EventOutputTypeDef],
-    },
-    total=False,
-)
 
 OnEnterLifecycleTypeDef = TypedDict(
     "OnEnterLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
     },
     total=False,
@@ -1481,68 +1355,31 @@
     "OnExitLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
     },
     total=False,
 )
 
-OnInputLifecycleOutputTypeDef = TypedDict(
-    "OnInputLifecycleOutputTypeDef",
-    {
-        "events": List[EventOutputTypeDef],
-        "transitionEvents": List[TransitionEventOutputTypeDef],
-    },
-    total=False,
-)
-
 OnInputLifecycleTypeDef = TypedDict(
     "OnInputLifecycleTypeDef",
     {
         "events": Sequence[EventTypeDef],
         "transitionEvents": Sequence[TransitionEventTypeDef],
     },
     total=False,
 )
 
-AlarmEventActionsUnionTypeDef = Union[AlarmEventActionsTypeDef, AlarmEventActionsOutputTypeDef]
-AlarmNotificationOutputTypeDef = TypedDict(
-    "AlarmNotificationOutputTypeDef",
-    {
-        "notificationActions": List[NotificationActionOutputTypeDef],
-    },
-    total=False,
-)
-
 AlarmNotificationTypeDef = TypedDict(
     "AlarmNotificationTypeDef",
     {
         "notificationActions": Sequence[NotificationActionTypeDef],
     },
     total=False,
 )
 
-_RequiredStateOutputTypeDef = TypedDict(
-    "_RequiredStateOutputTypeDef",
-    {
-        "stateName": str,
-    },
-)
-_OptionalStateOutputTypeDef = TypedDict(
-    "_OptionalStateOutputTypeDef",
-    {
-        "onInput": OnInputLifecycleOutputTypeDef,
-        "onEnter": OnEnterLifecycleOutputTypeDef,
-        "onExit": OnExitLifecycleOutputTypeDef,
-    },
-    total=False,
-)
-
-class StateOutputTypeDef(_RequiredStateOutputTypeDef, _OptionalStateOutputTypeDef):
-    pass
-
 _RequiredStateTypeDef = TypedDict(
     "_RequiredStateTypeDef",
     {
         "stateName": str,
     },
 )
 _OptionalStateTypeDef = TypedDict(
@@ -1551,40 +1388,19 @@
         "onInput": OnInputLifecycleTypeDef,
         "onEnter": OnEnterLifecycleTypeDef,
         "onExit": OnExitLifecycleTypeDef,
     },
     total=False,
 )
 
+
 class StateTypeDef(_RequiredStateTypeDef, _OptionalStateTypeDef):
     pass
 
-DescribeAlarmModelResponseTypeDef = TypedDict(
-    "DescribeAlarmModelResponseTypeDef",
-    {
-        "creationTime": datetime,
-        "alarmModelArn": str,
-        "alarmModelVersion": str,
-        "lastUpdateTime": datetime,
-        "status": AlarmModelVersionStatusType,
-        "statusMessage": str,
-        "alarmModelName": str,
-        "alarmModelDescription": str,
-        "roleArn": str,
-        "key": str,
-        "severity": int,
-        "alarmRule": AlarmRuleTypeDef,
-        "alarmNotification": AlarmNotificationOutputTypeDef,
-        "alarmEventActions": AlarmEventActionsOutputTypeDef,
-        "alarmCapabilities": AlarmCapabilitiesTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 
-AlarmNotificationUnionTypeDef = Union[AlarmNotificationTypeDef, AlarmNotificationOutputTypeDef]
 _RequiredCreateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
         "roleArn": str,
         "alarmRule": AlarmRuleTypeDef,
     },
@@ -1599,19 +1415,43 @@
         "alarmNotification": AlarmNotificationTypeDef,
         "alarmEventActions": AlarmEventActionsTypeDef,
         "alarmCapabilities": AlarmCapabilitiesTypeDef,
     },
     total=False,
 )
 
+
 class CreateAlarmModelRequestRequestTypeDef(
     _RequiredCreateAlarmModelRequestRequestTypeDef, _OptionalCreateAlarmModelRequestRequestTypeDef
 ):
     pass
 
+
+DescribeAlarmModelResponseTypeDef = TypedDict(
+    "DescribeAlarmModelResponseTypeDef",
+    {
+        "creationTime": datetime,
+        "alarmModelArn": str,
+        "alarmModelVersion": str,
+        "lastUpdateTime": datetime,
+        "status": AlarmModelVersionStatusType,
+        "statusMessage": str,
+        "alarmModelName": str,
+        "alarmModelDescription": str,
+        "roleArn": str,
+        "key": str,
+        "severity": int,
+        "alarmRule": AlarmRuleTypeDef,
+        "alarmNotification": AlarmNotificationTypeDef,
+        "alarmEventActions": AlarmEventActionsTypeDef,
+        "alarmCapabilities": AlarmCapabilitiesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredUpdateAlarmModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAlarmModelRequestRequestTypeDef",
     {
         "alarmModelName": str,
         "roleArn": str,
         "alarmRule": AlarmRuleTypeDef,
     },
@@ -1624,44 +1464,29 @@
         "alarmNotification": AlarmNotificationTypeDef,
         "alarmEventActions": AlarmEventActionsTypeDef,
         "alarmCapabilities": AlarmCapabilitiesTypeDef,
     },
     total=False,
 )
 
+
 class UpdateAlarmModelRequestRequestTypeDef(
     _RequiredUpdateAlarmModelRequestRequestTypeDef, _OptionalUpdateAlarmModelRequestRequestTypeDef
 ):
     pass
 
-DetectorModelDefinitionOutputTypeDef = TypedDict(
-    "DetectorModelDefinitionOutputTypeDef",
-    {
-        "states": List[StateOutputTypeDef],
-        "initialStateName": str,
-    },
-)
 
 DetectorModelDefinitionTypeDef = TypedDict(
     "DetectorModelDefinitionTypeDef",
     {
         "states": Sequence[StateTypeDef],
         "initialStateName": str,
     },
 )
 
-DetectorModelTypeDef = TypedDict(
-    "DetectorModelTypeDef",
-    {
-        "detectorModelDefinition": DetectorModelDefinitionOutputTypeDef,
-        "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
-    },
-    total=False,
-)
-
 _RequiredCreateDetectorModelRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDetectorModelRequestRequestTypeDef",
     {
         "detectorModelName": str,
         "detectorModelDefinition": DetectorModelDefinitionTypeDef,
         "roleArn": str,
     },
@@ -1673,23 +1498,31 @@
         "key": str,
         "tags": Sequence[TagTypeDef],
         "evaluationMethod": EvaluationMethodType,
     },
     total=False,
 )
 
+
 class CreateDetectorModelRequestRequestTypeDef(
     _RequiredCreateDetectorModelRequestRequestTypeDef,
     _OptionalCreateDetectorModelRequestRequestTypeDef,
 ):
     pass
 
-DetectorModelDefinitionUnionTypeDef = Union[
-    DetectorModelDefinitionTypeDef, DetectorModelDefinitionOutputTypeDef
-]
+
+DetectorModelTypeDef = TypedDict(
+    "DetectorModelTypeDef",
+    {
+        "detectorModelDefinition": DetectorModelDefinitionTypeDef,
+        "detectorModelConfiguration": DetectorModelConfigurationTypeDef,
+    },
+    total=False,
+)
+
 StartDetectorModelAnalysisRequestRequestTypeDef = TypedDict(
     "StartDetectorModelAnalysisRequestRequestTypeDef",
     {
         "detectorModelDefinition": DetectorModelDefinitionTypeDef,
     },
 )
 
@@ -1706,20 +1539,22 @@
     {
         "detectorModelDescription": str,
         "evaluationMethod": EvaluationMethodType,
     },
     total=False,
 )
 
+
 class UpdateDetectorModelRequestRequestTypeDef(
     _RequiredUpdateDetectorModelRequestRequestTypeDef,
     _OptionalUpdateDetectorModelRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeDetectorModelResponseTypeDef = TypedDict(
     "DescribeDetectorModelResponseTypeDef",
     {
         "detectorModel": DetectorModelTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iotevents-2.5.2.post1/types_aiobotocore_iotevents.egg-info/SOURCES.txt` & `types-aiobotocore-iotevents-2.5.2.post2/types_aiobotocore_iotevents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

