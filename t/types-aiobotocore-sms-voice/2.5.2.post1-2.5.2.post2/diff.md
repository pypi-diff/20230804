# Comparing `tmp/types-aiobotocore-sms-voice-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-sms-voice-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sms-voice-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-sms-voice-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:26 2023, max compression
```

## Comparing `types-aiobotocore-sms-voice-2.5.2.post1.tar` & `types-aiobotocore-sms-voice-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.249454 types-aiobotocore-sms-voice-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-08-02 14:53:02.241454 types-aiobotocore-sms-voice-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11501 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:02.249454 types-aiobotocore-sms-voice-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.233454 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9585 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7659 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7657 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:52.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:02.241454 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13034 2023-08-02 14:53:02.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-02 14:53:02.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:02.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:02.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:02.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:53:02.000000 types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.886643 types-aiobotocore-sms-voice-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12373 2023-08-04 13:59:26.886643 types-aiobotocore-sms-voice-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10840 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:26.886643 types-aiobotocore-sms-voice-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2093 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.886643 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      493 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      492 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      965 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9601 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     9585 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7754 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7752 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7192 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     7187 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:53:49.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:26.886643 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12373 2023-08-04 13:59:26.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      768 2023-08-04 13:59:26.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:26.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:26.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       28 2023-08-04 13:59:26.000000 types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sms-voice-2.5.2.post1/LICENSE` & `types-aiobotocore-sms-voice-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-voice-2.5.2.post1/PKG-INFO` & `types-aiobotocore-sms-voice-2.5.2.post2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sms-voice
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.PinpointSMSVoice 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.PinpointSMSVoice 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-sms-voice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,58 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sms_voice.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `PinpointSMSVoice` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/literals/).
+
 ```python
-from types_aiobotocore_sms_voice.literals import (
-    EventTypeType,
-    PinpointSMSVoiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_sms_voice.literals import EventTypeType
 
 
 def check_value(value: EventTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sms_voice.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `PinpointSMSVoice` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/type_defs/).
+
 ```python
-from types_aiobotocore_sms_voice.type_defs import (
-    CallInstructionsMessageTypeTypeDef,
-    CloudWatchLogsDestinationTypeDef,
-    CreateConfigurationSetRequestRequestTypeDef,
-    DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
-    DeleteConfigurationSetRequestRequestTypeDef,
-    KinesisFirehoseDestinationTypeDef,
-    SnsDestinationTypeDef,
-    GetConfigurationSetEventDestinationsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ListConfigurationSetsRequestRequestTypeDef,
-    PlainTextMessageTypeTypeDef,
-    SSMLMessageTypeTypeDef,
-    EventDestinationDefinitionTypeDef,
-    EventDestinationTypeDef,
-    ListConfigurationSetsResponseTypeDef,
-    SendVoiceMessageResponseTypeDef,
-    VoiceMessageContentTypeDef,
-    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
-    UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
-    GetConfigurationSetEventDestinationsResponseTypeDef,
-    SendVoiceMessageRequestRequestTypeDef,
-)
+from types_aiobotocore_sms_voice.type_defs import CallInstructionsMessageTypeTypeDef
 
 
 def get_value() -> CallInstructionsMessageTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sms-voice-2.5.2.post1/README.md` & `types-aiobotocore-sms-voice-2.5.2.post2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-sms-voice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -234,58 +234,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sms_voice.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `PinpointSMSVoice` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/literals/).
+
 ```python
-from types_aiobotocore_sms_voice.literals import (
-    EventTypeType,
-    PinpointSMSVoiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_sms_voice.literals import EventTypeType
 
 
 def check_value(value: EventTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sms_voice.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `PinpointSMSVoice` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/type_defs/).
+
 ```python
-from types_aiobotocore_sms_voice.type_defs import (
-    CallInstructionsMessageTypeTypeDef,
-    CloudWatchLogsDestinationTypeDef,
-    CreateConfigurationSetRequestRequestTypeDef,
-    DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
-    DeleteConfigurationSetRequestRequestTypeDef,
-    KinesisFirehoseDestinationTypeDef,
-    SnsDestinationTypeDef,
-    GetConfigurationSetEventDestinationsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ListConfigurationSetsRequestRequestTypeDef,
-    PlainTextMessageTypeTypeDef,
-    SSMLMessageTypeTypeDef,
-    EventDestinationDefinitionTypeDef,
-    EventDestinationTypeDef,
-    ListConfigurationSetsResponseTypeDef,
-    SendVoiceMessageResponseTypeDef,
-    VoiceMessageContentTypeDef,
-    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
-    UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
-    GetConfigurationSetEventDestinationsResponseTypeDef,
-    SendVoiceMessageRequestRequestTypeDef,
-)
+from types_aiobotocore_sms_voice.type_defs import CallInstructionsMessageTypeTypeDef
 
 
 def get_value() -> CallInstructionsMessageTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sms-voice-2.5.2.post1/setup.py` & `types-aiobotocore-sms-voice-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sms-voice",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_sms_voice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.PinpointSMSVoice 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/__main__.py` & `types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.PinpointSMSVoice 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sms-voice.html#PinpointSMSVoice\nOther"
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

### Comparing `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/client.py` & `types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/client.pyi` & `types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/literals.py` & `types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
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
@@ -140,14 +141,15 @@
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
@@ -226,26 +228,28 @@
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

### Comparing `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/literals.pyi` & `types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
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
@@ -138,14 +139,15 @@
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
@@ -224,26 +226,28 @@
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

### Comparing `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/type_defs.py` & `types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice/type_defs.pyi` & `types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/PKG-INFO` & `types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sms-voice
-Version: 2.5.2.post1
-Summary: Type annotations for aiobotocore.PinpointSMSVoice 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Version: 2.5.2.post2
+Summary: Type annotations for aiobotocore.PinpointSMSVoice 2.5.2 service generated with mypy-boto3-builder 7.17.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-sms-voice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -266,58 +266,37 @@
 <a id="literals"></a>
 
 ### Literals
 
 `types_aiobotocore_sms_voice.literals` module contains literals extracted from
 shapes that can be used in user code for type checking.
 
+Full list of `PinpointSMSVoice` Literals can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/literals/).
+
 ```python
-from types_aiobotocore_sms_voice.literals import (
-    EventTypeType,
-    PinpointSMSVoiceServiceName,
-    ServiceName,
-    ResourceServiceName,
-)
+from types_aiobotocore_sms_voice.literals import EventTypeType
 
 
 def check_value(value: EventTypeType) -> bool:
     ...
 ```
 
 <a id="type-definitions"></a>
 
 ### Type definitions
 
 `types_aiobotocore_sms_voice.type_defs` module contains structures and shapes
 assembled to typed dictionaries and unions for additional type checking.
 
+Full list of `PinpointSMSVoice` TypeDefs can be found in
+[docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sms_voice/type_defs/).
+
 ```python
-from types_aiobotocore_sms_voice.type_defs import (
-    CallInstructionsMessageTypeTypeDef,
-    CloudWatchLogsDestinationTypeDef,
-    CreateConfigurationSetRequestRequestTypeDef,
-    DeleteConfigurationSetEventDestinationRequestRequestTypeDef,
-    DeleteConfigurationSetRequestRequestTypeDef,
-    KinesisFirehoseDestinationTypeDef,
-    SnsDestinationTypeDef,
-    GetConfigurationSetEventDestinationsRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    ListConfigurationSetsRequestRequestTypeDef,
-    PlainTextMessageTypeTypeDef,
-    SSMLMessageTypeTypeDef,
-    EventDestinationDefinitionTypeDef,
-    EventDestinationTypeDef,
-    ListConfigurationSetsResponseTypeDef,
-    SendVoiceMessageResponseTypeDef,
-    VoiceMessageContentTypeDef,
-    CreateConfigurationSetEventDestinationRequestRequestTypeDef,
-    UpdateConfigurationSetEventDestinationRequestRequestTypeDef,
-    GetConfigurationSetEventDestinationsResponseTypeDef,
-    SendVoiceMessageRequestRequestTypeDef,
-)
+from types_aiobotocore_sms_voice.type_defs import CallInstructionsMessageTypeTypeDef
 
 
 def get_value() -> CallInstructionsMessageTypeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
```

### Comparing `types-aiobotocore-sms-voice-2.5.2.post1/types_aiobotocore_sms_voice.egg-info/SOURCES.txt` & `types-aiobotocore-sms-voice-2.5.2.post2/types_aiobotocore_sms_voice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

