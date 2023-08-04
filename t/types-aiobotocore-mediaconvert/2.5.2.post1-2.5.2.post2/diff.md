# Comparing `tmp/types-aiobotocore-mediaconvert-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-mediaconvert-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediaconvert-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:38 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediaconvert-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:17 2023, max compression
```

## Comparing `types-aiobotocore-mediaconvert-2.5.2.post1.tar` & `types-aiobotocore-mediaconvert-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.269527 types-aiobotocore-mediaconvert-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    35083 2023-08-02 14:52:38.269527 types-aiobotocore-mediaconvert-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33545 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:38.269527 types-aiobotocore-mediaconvert-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.269527 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24316 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24274 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    55531 2023-08-02 14:43:06.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    55529 2023-08-02 14:43:05.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   127164 2023-08-02 14:43:08.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   127139 2023-08-02 14:43:07.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:04.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.269527 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    35083 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:38.000000 types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.286643 types-aiobotocore-mediaconvert-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13737 2023-08-04 13:59:17.286643 types-aiobotocore-mediaconvert-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12199 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:17.286643 types-aiobotocore-mediaconvert-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2107 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.286643 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1425 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1424 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      963 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24276 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    24234 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    55626 2023-08-04 13:44:13.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    55624 2023-08-04 13:44:12.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6982 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     6975 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   103337 2023-08-04 13:44:16.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)   103312 2023-08-04 13:44:15.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:11.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:17.286643 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    13737 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      908 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       31 2023-08-04 13:59:17.000000 types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/LICENSE` & `types-aiobotocore-mediaconvert-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/setup.py` & `types-aiobotocore-mediaconvert-2.5.2.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediaconvert",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_mediaconvert"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MediaConvert 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/__init__.py` & `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/__init__.pyi` & `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/__main__.py` & `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaConvert 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.MediaConvert 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert\nOther"
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

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/client.py` & `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,23 +49,23 @@
     DescribeEndpointsResponseTypeDef,
     GetJobResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetPresetResponseTypeDef,
     GetQueueResponseTypeDef,
     HopDestinationTypeDef,
-    JobSettingsUnionTypeDef,
-    JobTemplateSettingsUnionTypeDef,
+    JobSettingsTypeDef,
+    JobTemplateSettingsTypeDef,
     ListJobsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListPresetsResponseTypeDef,
     ListQueuesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PolicyTypeDef,
-    PresetSettingsUnionTypeDef,
+    PresetSettingsTypeDef,
     PutPolicyResponseTypeDef,
     ReservationPlanSettingsTypeDef,
     UpdateJobTemplateResponseTypeDef,
     UpdatePresetResponseTypeDef,
     UpdateQueueResponseTypeDef,
 )
 
@@ -146,15 +146,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#close)
         """
 
     async def create_job(
         self,
         *,
         Role: str,
-        Settings: JobSettingsUnionTypeDef,
+        Settings: JobSettingsTypeDef,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         BillingTagsSource: BillingTagsSourceType = ...,
         ClientRequestToken: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         JobTemplate: str = ...,
         Priority: int = ...,
         Queue: str = ...,
@@ -170,15 +170,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_job)
         """
 
     async def create_job_template(
         self,
         *,
         Name: str,
-        Settings: JobTemplateSettingsUnionTypeDef,
+        Settings: JobTemplateSettingsTypeDef,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...,
@@ -191,15 +191,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_job_template)
         """
 
     async def create_preset(
         self,
         *,
         Name: str,
-        Settings: PresetSettingsUnionTypeDef,
+        Settings: PresetSettingsTypeDef,
         Category: str = ...,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreatePresetResponseTypeDef:
         """
         Create a new preset.
 
@@ -432,15 +432,15 @@
         Name: str,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
-        Settings: JobTemplateSettingsUnionTypeDef = ...,
+        Settings: JobTemplateSettingsTypeDef = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...
     ) -> UpdateJobTemplateResponseTypeDef:
         """
         Modify one of your existing job templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_job_template)
@@ -448,15 +448,15 @@
 
     async def update_preset(
         self,
         *,
         Name: str,
         Category: str = ...,
         Description: str = ...,
-        Settings: PresetSettingsUnionTypeDef = ...
+        Settings: PresetSettingsTypeDef = ...
     ) -> UpdatePresetResponseTypeDef:
         """
         Modify one of your existing presets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_preset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_preset)
         """
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/client.pyi` & `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -49,23 +49,23 @@
     DescribeEndpointsResponseTypeDef,
     GetJobResponseTypeDef,
     GetJobTemplateResponseTypeDef,
     GetPolicyResponseTypeDef,
     GetPresetResponseTypeDef,
     GetQueueResponseTypeDef,
     HopDestinationTypeDef,
-    JobSettingsUnionTypeDef,
-    JobTemplateSettingsUnionTypeDef,
+    JobSettingsTypeDef,
+    JobTemplateSettingsTypeDef,
     ListJobsResponseTypeDef,
     ListJobTemplatesResponseTypeDef,
     ListPresetsResponseTypeDef,
     ListQueuesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PolicyTypeDef,
-    PresetSettingsUnionTypeDef,
+    PresetSettingsTypeDef,
     PutPolicyResponseTypeDef,
     ReservationPlanSettingsTypeDef,
     UpdateJobTemplateResponseTypeDef,
     UpdatePresetResponseTypeDef,
     UpdateQueueResponseTypeDef,
 )
 
@@ -137,15 +137,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#close)
         """
     async def create_job(
         self,
         *,
         Role: str,
-        Settings: JobSettingsUnionTypeDef,
+        Settings: JobSettingsTypeDef,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         BillingTagsSource: BillingTagsSourceType = ...,
         ClientRequestToken: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         JobTemplate: str = ...,
         Priority: int = ...,
         Queue: str = ...,
@@ -160,15 +160,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_job)
         """
     async def create_job_template(
         self,
         *,
         Name: str,
-        Settings: JobTemplateSettingsUnionTypeDef,
+        Settings: JobTemplateSettingsTypeDef,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...,
@@ -180,15 +180,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.create_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#create_job_template)
         """
     async def create_preset(
         self,
         *,
         Name: str,
-        Settings: PresetSettingsUnionTypeDef,
+        Settings: PresetSettingsTypeDef,
         Category: str = ...,
         Description: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreatePresetResponseTypeDef:
         """
         Create a new preset.
 
@@ -399,30 +399,30 @@
         Name: str,
         AccelerationSettings: AccelerationSettingsTypeDef = ...,
         Category: str = ...,
         Description: str = ...,
         HopDestinations: Sequence[HopDestinationTypeDef] = ...,
         Priority: int = ...,
         Queue: str = ...,
-        Settings: JobTemplateSettingsUnionTypeDef = ...,
+        Settings: JobTemplateSettingsTypeDef = ...,
         StatusUpdateInterval: StatusUpdateIntervalType = ...
     ) -> UpdateJobTemplateResponseTypeDef:
         """
         Modify one of your existing job templates.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_job_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_job_template)
         """
     async def update_preset(
         self,
         *,
         Name: str,
         Category: str = ...,
         Description: str = ...,
-        Settings: PresetSettingsUnionTypeDef = ...
+        Settings: PresetSettingsTypeDef = ...
     ) -> UpdatePresetResponseTypeDef:
         """
         Modify one of your existing presets.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediaconvert.html#MediaConvert.Client.update_preset)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediaconvert/client/#update_preset)
         """
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/literals.py` & `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -1309,14 +1309,15 @@
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
@@ -1412,14 +1413,15 @@
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
@@ -1498,26 +1500,28 @@
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

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/literals.pyi` & `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1307,14 +1307,15 @@
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
@@ -1410,14 +1411,15 @@
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
@@ -1496,26 +1498,28 @@
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

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/paginator.py` & `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/paginator.pyi` & `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/type_defs.py` & `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_mediaconvert.type_defs import AacSettingsTypeDef
 
     data: AacSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AacAudioDescriptionBroadcasterMixType,
     AacCodecProfileType,
     AacCodingModeType,
     AacRateControlModeType,
     AacRawFormatType,
@@ -426,15 +426,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AacSettingsTypeDef",
     "Ac3SettingsTypeDef",
     "AccelerationSettingsTypeDef",
     "AdvancedInputFilterSettingsTypeDef",
     "AiffSettingsTypeDef",
     "AllowedRenditionSizeTypeDef",
@@ -445,15 +444,14 @@
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
     "Mp3SettingsTypeDef",
     "OpusSettingsTypeDef",
     "VorbisSettingsTypeDef",
     "WavSettingsTypeDef",
     "AudioNormalizationSettingsTypeDef",
-    "AudioSelectorGroupOutputTypeDef",
     "AudioSelectorGroupTypeDef",
     "HlsRenditionGroupSettingsTypeDef",
     "ForceIncludeRenditionSizeTypeDef",
     "MinBottomRenditionSizeTypeDef",
     "MinTopRenditionSizeTypeDef",
     "Av1QvbrSettingsTypeDef",
     "AvailBlankingTypeDef",
@@ -462,47 +460,40 @@
     "BurninDestinationSettingsTypeDef",
     "CancelJobRequestRequestTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "EmbeddedDestinationSettingsTypeDef",
     "ImscDestinationSettingsTypeDef",
     "SccDestinationSettingsTypeDef",
     "SrtDestinationSettingsTypeDef",
-    "TeletextDestinationSettingsOutputTypeDef",
+    "TeletextDestinationSettingsTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
-    "TeletextDestinationSettingsTypeDef",
     "CaptionSourceFramerateTypeDef",
     "DvbSubSourceSettingsTypeDef",
     "EmbeddedSourceSettingsTypeDef",
     "TeletextSourceSettingsTypeDef",
     "TrackSourceSettingsTypeDef",
     "WebvttHlsSourceSettingsTypeDef",
-    "OutputChannelMappingOutputTypeDef",
     "OutputChannelMappingTypeDef",
     "ClipLimitsTypeDef",
-    "CmafAdditionalManifestOutputTypeDef",
     "CmafAdditionalManifestTypeDef",
-    "SpekeKeyProviderCmafOutputTypeDef",
-    "StaticKeyProviderTypeDef",
     "SpekeKeyProviderCmafTypeDef",
+    "StaticKeyProviderTypeDef",
     "CmafImageBasedTrickPlaySettingsTypeDef",
     "CmfcSettingsTypeDef",
     "Hdr10MetadataTypeDef",
     "F4vSettingsTypeDef",
-    "M3u8SettingsOutputTypeDef",
+    "M3u8SettingsTypeDef",
     "MovSettingsTypeDef",
     "Mp4SettingsTypeDef",
     "MpdSettingsTypeDef",
-    "M3u8SettingsTypeDef",
     "HopDestinationTypeDef",
     "ResponseMetadataTypeDef",
     "ReservationPlanSettingsTypeDef",
-    "DashAdditionalManifestOutputTypeDef",
     "DashAdditionalManifestTypeDef",
-    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     "DeinterlacerTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -521,25 +512,24 @@
     "GetJobTemplateRequestRequestTypeDef",
     "PolicyTypeDef",
     "GetPresetRequestRequestTypeDef",
     "GetQueueRequestRequestTypeDef",
     "H264QvbrSettingsTypeDef",
     "H265QvbrSettingsTypeDef",
     "Hdr10PlusTypeDef",
-    "HlsAdditionalManifestOutputTypeDef",
     "HlsAdditionalManifestTypeDef",
     "HlsCaptionLanguageMappingTypeDef",
     "HlsImageBasedTrickPlaySettingsTypeDef",
     "HlsSettingsTypeDef",
     "Id3InsertionTypeDef",
     "InsertableImageTypeDef",
     "InputClippingTypeDef",
     "InputDecryptionSettingsTypeDef",
-    "InputVideoGeneratorTypeDef",
     "RectangleTypeDef",
+    "InputVideoGeneratorTypeDef",
     "JobMessagesTypeDef",
     "KantarWatermarkSettingsTypeDef",
     "NielsenConfigurationTypeDef",
     "NielsenNonLinearWatermarkSettingsTypeDef",
     "TimecodeConfigTypeDef",
     "QueueTransitionTypeDef",
     "TimingTypeDef",
@@ -550,15 +540,14 @@
     "ListQueuesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagsTypeDef",
     "M2tsScte35EsamTypeDef",
     "MotionImageInsertionFramerateTypeDef",
     "MotionImageInsertionOffsetTypeDef",
     "Mpeg2SettingsTypeDef",
-    "MsSmoothAdditionalManifestOutputTypeDef",
     "MsSmoothAdditionalManifestTypeDef",
     "MxfXavcProfileSettingsTypeDef",
     "NexGuardFileMarkerSettingsTypeDef",
     "NoiseReducerFilterSettingsTypeDef",
     "NoiseReducerSpatialFilterSettingsTypeDef",
     "NoiseReducerTemporalFilterSettingsTypeDef",
     "VideoDetailTypeDef",
@@ -574,32 +563,25 @@
     "Vp9SettingsTypeDef",
     "Xavc4kIntraCbgProfileSettingsTypeDef",
     "Xavc4kIntraVbrProfileSettingsTypeDef",
     "Xavc4kProfileSettingsTypeDef",
     "XavcHdIntraCbgProfileSettingsTypeDef",
     "XavcHdProfileSettingsTypeDef",
     "AudioCodecSettingsTypeDef",
-    "AutomatedAbrRuleOutputTypeDef",
     "AutomatedAbrRuleTypeDef",
     "Av1SettingsTypeDef",
     "AvcIntraSettingsTypeDef",
-    "CaptionDestinationSettingsOutputTypeDef",
     "CaptionDestinationSettingsTypeDef",
     "FileSourceSettingsTypeDef",
-    "ChannelMappingOutputTypeDef",
     "ChannelMappingTypeDef",
-    "CmafEncryptionSettingsOutputTypeDef",
     "CmafEncryptionSettingsTypeDef",
     "ColorCorrectorTypeDef",
     "VideoSelectorTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "UpdateQueueRequestRequestTypeDef",
-    "DashIsoEncryptionSettingsOutputTypeDef",
-    "HlsEncryptionSettingsOutputTypeDef",
-    "MsSmoothEncryptionSettingsOutputTypeDef",
     "DashIsoEncryptionSettingsTypeDef",
     "HlsEncryptionSettingsTypeDef",
     "MsSmoothEncryptionSettingsTypeDef",
     "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListPresetsRequestListPresetsPaginateTypeDef",
@@ -609,95 +591,69 @@
     "EsamSettingsTypeDef",
     "GetPolicyResponseTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
     "H264SettingsTypeDef",
     "H265SettingsTypeDef",
     "OutputSettingsTypeDef",
-    "TimedMetadataInsertionOutputTypeDef",
     "TimedMetadataInsertionTypeDef",
-    "ImageInserterOutputTypeDef",
     "ImageInserterTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "M2tsSettingsOutputTypeDef",
     "M2tsSettingsTypeDef",
     "MotionImageInserterTypeDef",
     "MxfSettingsTypeDef",
     "PartnerWatermarkingTypeDef",
     "NoiseReducerTypeDef",
     "OutputDetailTypeDef",
     "QueueTypeDef",
     "S3DestinationSettingsTypeDef",
     "XavcSettingsTypeDef",
-    "AutomatedAbrSettingsOutputTypeDef",
     "AutomatedAbrSettingsTypeDef",
-    "CaptionDescriptionPresetOutputTypeDef",
     "CaptionDescriptionPresetTypeDef",
     "CaptionDescriptionTypeDef",
     "CaptionSourceSettingsTypeDef",
-    "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
-    "ContainerSettingsOutputTypeDef",
     "ContainerSettingsTypeDef",
-    "VideoPreprocessorOutputTypeDef",
     "VideoPreprocessorTypeDef",
     "OutputGroupDetailTypeDef",
     "CreateQueueResponseTypeDef",
     "GetQueueResponseTypeDef",
     "ListQueuesResponseTypeDef",
     "UpdateQueueResponseTypeDef",
     "DestinationSettingsTypeDef",
     "VideoCodecSettingsTypeDef",
-    "AutomatedEncodingSettingsOutputTypeDef",
     "AutomatedEncodingSettingsTypeDef",
     "CaptionSelectorTypeDef",
-    "AudioDescriptionOutputTypeDef",
-    "AudioSelectorOutputTypeDef",
     "AudioDescriptionTypeDef",
     "AudioSelectorTypeDef",
-    "CmafGroupSettingsOutputTypeDef",
     "CmafGroupSettingsTypeDef",
-    "DashIsoGroupSettingsOutputTypeDef",
     "DashIsoGroupSettingsTypeDef",
     "FileGroupSettingsTypeDef",
-    "HlsGroupSettingsOutputTypeDef",
     "HlsGroupSettingsTypeDef",
-    "MsSmoothGroupSettingsOutputTypeDef",
     "MsSmoothGroupSettingsTypeDef",
-    "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
-    "InputOutputTypeDef",
-    "InputTemplateOutputTypeDef",
     "InputTemplateTypeDef",
     "InputTypeDef",
-    "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
-    "PresetSettingsOutputTypeDef",
     "OutputTypeDef",
     "PresetSettingsTypeDef",
-    "PresetTypeDef",
-    "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
     "CreatePresetRequestRequestTypeDef",
-    "PresetSettingsUnionTypeDef",
+    "PresetTypeDef",
     "UpdatePresetRequestRequestTypeDef",
+    "JobSettingsTypeDef",
+    "JobTemplateSettingsTypeDef",
     "CreatePresetResponseTypeDef",
     "GetPresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "UpdatePresetResponseTypeDef",
-    "JobSettingsOutputTypeDef",
-    "JobTemplateSettingsOutputTypeDef",
-    "JobSettingsTypeDef",
-    "JobTemplateSettingsTypeDef",
-    "JobTypeDef",
-    "JobTemplateTypeDef",
     "CreateJobRequestRequestTypeDef",
-    "JobSettingsUnionTypeDef",
+    "JobTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
-    "JobTemplateSettingsUnionTypeDef",
+    "JobTemplateTypeDef",
     "UpdateJobTemplateRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
     "ListJobsResponseTypeDef",
     "CreateJobTemplateResponseTypeDef",
     "GetJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
@@ -913,22 +869,14 @@
         "PeakCalculation": AudioNormalizationPeakCalculationType,
         "TargetLkfs": float,
         "TruePeakLimiterThreshold": float,
     },
     total=False,
 )
 
-AudioSelectorGroupOutputTypeDef = TypedDict(
-    "AudioSelectorGroupOutputTypeDef",
-    {
-        "AudioSelectorNames": List[str],
-    },
-    total=False,
-)
-
 AudioSelectorGroupTypeDef = TypedDict(
     "AudioSelectorGroupTypeDef",
     {
         "AudioSelectorNames": Sequence[str],
     },
     total=False,
 )
@@ -1103,19 +1051,19 @@
     "SrtDestinationSettingsTypeDef",
     {
         "StylePassthrough": SrtStylePassthroughType,
     },
     total=False,
 )
 
-TeletextDestinationSettingsOutputTypeDef = TypedDict(
-    "TeletextDestinationSettingsOutputTypeDef",
+TeletextDestinationSettingsTypeDef = TypedDict(
+    "TeletextDestinationSettingsTypeDef",
     {
         "PageNumber": str,
-        "PageTypes": List[TeletextPageTypeType],
+        "PageTypes": Sequence[TeletextPageTypeType],
     },
     total=False,
 )
 
 TtmlDestinationSettingsTypeDef = TypedDict(
     "TtmlDestinationSettingsTypeDef",
     {
@@ -1129,23 +1077,14 @@
     {
         "Accessibility": WebvttAccessibilitySubsType,
         "StylePassthrough": WebvttStylePassthroughType,
     },
     total=False,
 )
 
-TeletextDestinationSettingsTypeDef = TypedDict(
-    "TeletextDestinationSettingsTypeDef",
-    {
-        "PageNumber": str,
-        "PageTypes": Sequence[TeletextPageTypeType],
-    },
-    total=False,
-)
-
 CaptionSourceFramerateTypeDef = TypedDict(
     "CaptionSourceFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
     total=False,
@@ -1192,23 +1131,14 @@
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
     total=False,
 )
 
-OutputChannelMappingOutputTypeDef = TypedDict(
-    "OutputChannelMappingOutputTypeDef",
-    {
-        "InputChannels": List[int],
-        "InputChannelsFineTune": List[float],
-    },
-    total=False,
-)
-
 OutputChannelMappingTypeDef = TypedDict(
     "OutputChannelMappingTypeDef",
     {
         "InputChannels": Sequence[int],
         "InputChannelsFineTune": Sequence[float],
     },
     total=False,
@@ -1221,38 +1151,29 @@
         "MaximumYUV": int,
         "MinimumRGBTolerance": int,
         "MinimumYUV": int,
     },
     total=False,
 )
 
-CmafAdditionalManifestOutputTypeDef = TypedDict(
-    "CmafAdditionalManifestOutputTypeDef",
-    {
-        "ManifestNameModifier": str,
-        "SelectedOutputs": List[str],
-    },
-    total=False,
-)
-
 CmafAdditionalManifestTypeDef = TypedDict(
     "CmafAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
-SpekeKeyProviderCmafOutputTypeDef = TypedDict(
-    "SpekeKeyProviderCmafOutputTypeDef",
+SpekeKeyProviderCmafTypeDef = TypedDict(
+    "SpekeKeyProviderCmafTypeDef",
     {
         "CertificateArn": str,
-        "DashSignaledSystemIds": List[str],
-        "HlsSignaledSystemIds": List[str],
+        "DashSignaledSystemIds": Sequence[str],
+        "HlsSignaledSystemIds": Sequence[str],
         "ResourceId": str,
         "Url": str,
     },
     total=False,
 )
 
 StaticKeyProviderTypeDef = TypedDict(
@@ -1262,26 +1183,14 @@
         "KeyFormatVersions": str,
         "StaticKeyValue": str,
         "Url": str,
     },
     total=False,
 )
 
-SpekeKeyProviderCmafTypeDef = TypedDict(
-    "SpekeKeyProviderCmafTypeDef",
-    {
-        "CertificateArn": str,
-        "DashSignaledSystemIds": Sequence[str],
-        "HlsSignaledSystemIds": Sequence[str],
-        "ResourceId": str,
-        "Url": str,
-    },
-    total=False,
-)
-
 CmafImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "CmafImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": CmafIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
@@ -1335,20 +1244,20 @@
     "F4vSettingsTypeDef",
     {
         "MoovPlacement": F4vMoovPlacementType,
     },
     total=False,
 )
 
-M3u8SettingsOutputTypeDef = TypedDict(
-    "M3u8SettingsOutputTypeDef",
+M3u8SettingsTypeDef = TypedDict(
+    "M3u8SettingsTypeDef",
     {
         "AudioDuration": M3u8AudioDurationType,
         "AudioFramesPerPes": int,
-        "AudioPids": List[int],
+        "AudioPids": Sequence[int],
         "DataPTSControl": M3u8DataPtsControlType,
         "MaxPcrInterval": int,
         "NielsenId3": M3u8NielsenId3Type,
         "PatInterval": int,
         "PcrControl": M3u8PcrControlType,
         "PcrPid": int,
         "PmtInterval": int,
@@ -1404,40 +1313,14 @@
         "TimedMetadataBoxVersion": MpdTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
     total=False,
 )
 
-M3u8SettingsTypeDef = TypedDict(
-    "M3u8SettingsTypeDef",
-    {
-        "AudioDuration": M3u8AudioDurationType,
-        "AudioFramesPerPes": int,
-        "AudioPids": Sequence[int],
-        "DataPTSControl": M3u8DataPtsControlType,
-        "MaxPcrInterval": int,
-        "NielsenId3": M3u8NielsenId3Type,
-        "PatInterval": int,
-        "PcrControl": M3u8PcrControlType,
-        "PcrPid": int,
-        "PmtInterval": int,
-        "PmtPid": int,
-        "PrivateMetadataPid": int,
-        "ProgramNumber": int,
-        "Scte35Pid": int,
-        "Scte35Source": M3u8Scte35SourceType,
-        "TimedMetadata": TimedMetadataType,
-        "TimedMetadataPid": int,
-        "TransportStreamId": int,
-        "VideoPid": int,
-    },
-    total=False,
-)
-
 HopDestinationTypeDef = TypedDict(
     "HopDestinationTypeDef",
     {
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
     },
@@ -1460,43 +1343,23 @@
     {
         "Commitment": Literal["ONE_YEAR"],
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
     },
 )
 
-DashAdditionalManifestOutputTypeDef = TypedDict(
-    "DashAdditionalManifestOutputTypeDef",
-    {
-        "ManifestNameModifier": str,
-        "SelectedOutputs": List[str],
-    },
-    total=False,
-)
-
 DashAdditionalManifestTypeDef = TypedDict(
     "DashAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
-SpekeKeyProviderOutputTypeDef = TypedDict(
-    "SpekeKeyProviderOutputTypeDef",
-    {
-        "CertificateArn": str,
-        "ResourceId": str,
-        "SystemIds": List[str],
-        "Url": str,
-    },
-    total=False,
-)
-
 SpekeKeyProviderTypeDef = TypedDict(
     "SpekeKeyProviderTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
         "SystemIds": Sequence[str],
         "Url": str,
@@ -1720,23 +1583,14 @@
     {
         "MasteringMonitorNits": int,
         "TargetMonitorNits": int,
     },
     total=False,
 )
 
-HlsAdditionalManifestOutputTypeDef = TypedDict(
-    "HlsAdditionalManifestOutputTypeDef",
-    {
-        "ManifestNameModifier": str,
-        "SelectedOutputs": List[str],
-    },
-    total=False,
-)
-
 HlsAdditionalManifestTypeDef = TypedDict(
     "HlsAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
@@ -1823,33 +1677,33 @@
         "EncryptedDecryptionKey": str,
         "InitializationVector": str,
         "KmsKeyRegion": str,
     },
     total=False,
 )
 
-InputVideoGeneratorTypeDef = TypedDict(
-    "InputVideoGeneratorTypeDef",
-    {
-        "Duration": int,
-    },
-    total=False,
-)
-
 RectangleTypeDef = TypedDict(
     "RectangleTypeDef",
     {
         "Height": int,
         "Width": int,
         "X": int,
         "Y": int,
     },
     total=False,
 )
 
+InputVideoGeneratorTypeDef = TypedDict(
+    "InputVideoGeneratorTypeDef",
+    {
+        "Duration": int,
+    },
+    total=False,
+)
+
 JobMessagesTypeDef = TypedDict(
     "JobMessagesTypeDef",
     {
         "Info": List[str],
         "Warning": List[str],
     },
     total=False,
@@ -2066,23 +1920,14 @@
         "Syntax": Mpeg2SyntaxType,
         "Telecine": Mpeg2TelecineType,
         "TemporalAdaptiveQuantization": Mpeg2TemporalAdaptiveQuantizationType,
     },
     total=False,
 )
 
-MsSmoothAdditionalManifestOutputTypeDef = TypedDict(
-    "MsSmoothAdditionalManifestOutputTypeDef",
-    {
-        "ManifestNameModifier": str,
-        "SelectedOutputs": List[str],
-    },
-    total=False,
-)
-
 MsSmoothAdditionalManifestTypeDef = TypedDict(
     "MsSmoothAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
@@ -2226,21 +2071,19 @@
     "_OptionalUntagResourceRequestRequestTypeDef",
     {
         "TagKeys": Sequence[str],
     },
     total=False,
 )
 
-
 class UntagResourceRequestRequestTypeDef(
     _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
 ):
     pass
 
-
 Vc3SettingsTypeDef = TypedDict(
     "Vc3SettingsTypeDef",
     {
         "FramerateControl": Vc3FramerateControlType,
         "FramerateConversionAlgorithm": Vc3FramerateConversionAlgorithmType,
         "FramerateDenominator": int,
         "FramerateNumerator": int,
@@ -2362,26 +2205,14 @@
         "OpusSettings": OpusSettingsTypeDef,
         "VorbisSettings": VorbisSettingsTypeDef,
         "WavSettings": WavSettingsTypeDef,
     },
     total=False,
 )
 
-AutomatedAbrRuleOutputTypeDef = TypedDict(
-    "AutomatedAbrRuleOutputTypeDef",
-    {
-        "AllowedRenditions": List[AllowedRenditionSizeTypeDef],
-        "ForceIncludeRenditions": List[ForceIncludeRenditionSizeTypeDef],
-        "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
-        "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
-        "Type": RuleTypeType,
-    },
-    total=False,
-)
-
 AutomatedAbrRuleTypeDef = TypedDict(
     "AutomatedAbrRuleTypeDef",
     {
         "AllowedRenditions": Sequence[AllowedRenditionSizeTypeDef],
         "ForceIncludeRenditions": Sequence[ForceIncludeRenditionSizeTypeDef],
         "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
         "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
@@ -2423,31 +2254,14 @@
         "ScanTypeConversionMode": AvcIntraScanTypeConversionModeType,
         "SlowPal": AvcIntraSlowPalType,
         "Telecine": AvcIntraTelecineType,
     },
     total=False,
 )
 
-CaptionDestinationSettingsOutputTypeDef = TypedDict(
-    "CaptionDestinationSettingsOutputTypeDef",
-    {
-        "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
-        "DestinationType": CaptionDestinationTypeType,
-        "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
-        "EmbeddedDestinationSettings": EmbeddedDestinationSettingsTypeDef,
-        "ImscDestinationSettings": ImscDestinationSettingsTypeDef,
-        "SccDestinationSettings": SccDestinationSettingsTypeDef,
-        "SrtDestinationSettings": SrtDestinationSettingsTypeDef,
-        "TeletextDestinationSettings": TeletextDestinationSettingsOutputTypeDef,
-        "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
-        "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
-    },
-    total=False,
-)
-
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
         "DestinationType": CaptionDestinationTypeType,
         "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
         "EmbeddedDestinationSettings": EmbeddedDestinationSettingsTypeDef,
@@ -2470,43 +2284,22 @@
         "SourceFile": str,
         "TimeDelta": int,
         "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
     },
     total=False,
 )
 
-ChannelMappingOutputTypeDef = TypedDict(
-    "ChannelMappingOutputTypeDef",
-    {
-        "OutputChannels": List[OutputChannelMappingOutputTypeDef],
-    },
-    total=False,
-)
-
 ChannelMappingTypeDef = TypedDict(
     "ChannelMappingTypeDef",
     {
         "OutputChannels": Sequence[OutputChannelMappingTypeDef],
     },
     total=False,
 )
 
-CmafEncryptionSettingsOutputTypeDef = TypedDict(
-    "CmafEncryptionSettingsOutputTypeDef",
-    {
-        "ConstantInitializationVector": str,
-        "EncryptionMethod": CmafEncryptionTypeType,
-        "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
-        "SpekeKeyProvider": SpekeKeyProviderCmafOutputTypeDef,
-        "StaticKeyProvider": StaticKeyProviderTypeDef,
-        "Type": CmafKeyProviderTypeType,
-    },
-    total=False,
-)
-
 CmafEncryptionSettingsTypeDef = TypedDict(
     "CmafEncryptionSettingsTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
         "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
         "SpekeKeyProvider": SpekeKeyProviderCmafTypeDef,
@@ -2564,21 +2357,19 @@
         "ReservationPlanSettings": ReservationPlanSettingsTypeDef,
         "Status": QueueStatusType,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateQueueRequestRequestTypeDef(
     _RequiredCreateQueueRequestRequestTypeDef, _OptionalCreateQueueRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateQueueRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateQueueRequestRequestTypeDef = TypedDict(
@@ -2587,52 +2378,19 @@
         "Description": str,
         "ReservationPlanSettings": ReservationPlanSettingsTypeDef,
         "Status": QueueStatusType,
     },
     total=False,
 )
 
-
 class UpdateQueueRequestRequestTypeDef(
     _RequiredUpdateQueueRequestRequestTypeDef, _OptionalUpdateQueueRequestRequestTypeDef
 ):
     pass
 
-
-DashIsoEncryptionSettingsOutputTypeDef = TypedDict(
-    "DashIsoEncryptionSettingsOutputTypeDef",
-    {
-        "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-    total=False,
-)
-
-HlsEncryptionSettingsOutputTypeDef = TypedDict(
-    "HlsEncryptionSettingsOutputTypeDef",
-    {
-        "ConstantInitializationVector": str,
-        "EncryptionMethod": HlsEncryptionTypeType,
-        "InitializationVectorInManifest": HlsInitializationVectorInManifestType,
-        "OfflineEncrypted": HlsOfflineEncryptedType,
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-        "StaticKeyProvider": StaticKeyProviderTypeDef,
-        "Type": HlsKeyProviderTypeType,
-    },
-    total=False,
-)
-
-MsSmoothEncryptionSettingsOutputTypeDef = TypedDict(
-    "MsSmoothEncryptionSettingsOutputTypeDef",
-    {
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-    total=False,
-)
-
 DashIsoEncryptionSettingsTypeDef = TypedDict(
     "DashIsoEncryptionSettingsTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
     total=False,
@@ -2867,39 +2625,22 @@
     "OutputSettingsTypeDef",
     {
         "HlsSettings": HlsSettingsTypeDef,
     },
     total=False,
 )
 
-TimedMetadataInsertionOutputTypeDef = TypedDict(
-    "TimedMetadataInsertionOutputTypeDef",
-    {
-        "Id3Insertions": List[Id3InsertionTypeDef],
-    },
-    total=False,
-)
-
 TimedMetadataInsertionTypeDef = TypedDict(
     "TimedMetadataInsertionTypeDef",
     {
         "Id3Insertions": Sequence[Id3InsertionTypeDef],
     },
     total=False,
 )
 
-ImageInserterOutputTypeDef = TypedDict(
-    "ImageInserterOutputTypeDef",
-    {
-        "InsertableImages": List[InsertableImageTypeDef],
-        "SdrReferenceWhiteLevel": int,
-    },
-    total=False,
-)
-
 ImageInserterTypeDef = TypedDict(
     "ImageInserterTypeDef",
     {
         "InsertableImages": Sequence[InsertableImageTypeDef],
         "SdrReferenceWhiteLevel": int,
     },
     total=False,
@@ -2909,60 +2650,14 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": ResourceTagsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-M2tsSettingsOutputTypeDef = TypedDict(
-    "M2tsSettingsOutputTypeDef",
-    {
-        "AudioBufferModel": M2tsAudioBufferModelType,
-        "AudioDuration": M2tsAudioDurationType,
-        "AudioFramesPerPes": int,
-        "AudioPids": List[int],
-        "Bitrate": int,
-        "BufferModel": M2tsBufferModelType,
-        "DataPTSControl": M2tsDataPtsControlType,
-        "DvbNitSettings": DvbNitSettingsTypeDef,
-        "DvbSdtSettings": DvbSdtSettingsTypeDef,
-        "DvbSubPids": List[int],
-        "DvbTdtSettings": DvbTdtSettingsTypeDef,
-        "DvbTeletextPid": int,
-        "EbpAudioInterval": M2tsEbpAudioIntervalType,
-        "EbpPlacement": M2tsEbpPlacementType,
-        "EsRateInPes": M2tsEsRateInPesType,
-        "ForceTsVideoEbpOrder": M2tsForceTsVideoEbpOrderType,
-        "FragmentTime": float,
-        "KlvMetadata": M2tsKlvMetadataType,
-        "MaxPcrInterval": int,
-        "MinEbpInterval": int,
-        "NielsenId3": M2tsNielsenId3Type,
-        "NullPacketBitrate": float,
-        "PatInterval": int,
-        "PcrControl": M2tsPcrControlType,
-        "PcrPid": int,
-        "PmtInterval": int,
-        "PmtPid": int,
-        "PrivateMetadataPid": int,
-        "ProgramNumber": int,
-        "RateMode": M2tsRateModeType,
-        "Scte35Esam": M2tsScte35EsamTypeDef,
-        "Scte35Pid": int,
-        "Scte35Source": M2tsScte35SourceType,
-        "SegmentationMarkers": M2tsSegmentationMarkersType,
-        "SegmentationStyle": M2tsSegmentationStyleType,
-        "SegmentationTime": float,
-        "TimedMetadataPid": int,
-        "TransportStreamId": int,
-        "VideoPid": int,
-    },
-    total=False,
-)
-
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioDuration": M2tsAudioDurationType,
         "AudioFramesPerPes": int,
         "AudioPids": Sequence[int],
@@ -3075,19 +2770,17 @@
         "Status": QueueStatusType,
         "SubmittedJobsCount": int,
         "Type": TypeType,
     },
     total=False,
 )
 
-
 class QueueTypeDef(_RequiredQueueTypeDef, _OptionalQueueTypeDef):
     pass
 
-
 S3DestinationSettingsTypeDef = TypedDict(
     "S3DestinationSettingsTypeDef",
     {
         "AccessControl": S3DestinationAccessControlTypeDef,
         "Encryption": S3EncryptionSettingsTypeDef,
     },
     total=False,
@@ -3112,47 +2805,25 @@
         "Xavc4kProfileSettings": Xavc4kProfileSettingsTypeDef,
         "XavcHdIntraCbgProfileSettings": XavcHdIntraCbgProfileSettingsTypeDef,
         "XavcHdProfileSettings": XavcHdProfileSettingsTypeDef,
     },
     total=False,
 )
 
-AutomatedAbrSettingsOutputTypeDef = TypedDict(
-    "AutomatedAbrSettingsOutputTypeDef",
-    {
-        "MaxAbrBitrate": int,
-        "MaxRenditions": int,
-        "MinAbrBitrate": int,
-        "Rules": List[AutomatedAbrRuleOutputTypeDef],
-    },
-    total=False,
-)
-
 AutomatedAbrSettingsTypeDef = TypedDict(
     "AutomatedAbrSettingsTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
         "MinAbrBitrate": int,
         "Rules": Sequence[AutomatedAbrRuleTypeDef],
     },
     total=False,
 )
 
-CaptionDescriptionPresetOutputTypeDef = TypedDict(
-    "CaptionDescriptionPresetOutputTypeDef",
-    {
-        "CustomLanguageCode": str,
-        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "LanguageDescription": str,
-    },
-    total=False,
-)
-
 CaptionDescriptionPresetTypeDef = TypedDict(
     "CaptionDescriptionPresetTypeDef",
     {
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
@@ -3183,50 +2854,24 @@
         "TeletextSourceSettings": TeletextSourceSettingsTypeDef,
         "TrackSourceSettings": TrackSourceSettingsTypeDef,
         "WebvttHlsSourceSettings": WebvttHlsSourceSettingsTypeDef,
     },
     total=False,
 )
 
-RemixSettingsOutputTypeDef = TypedDict(
-    "RemixSettingsOutputTypeDef",
-    {
-        "ChannelMapping": ChannelMappingOutputTypeDef,
-        "ChannelsIn": int,
-        "ChannelsOut": int,
-    },
-    total=False,
-)
-
 RemixSettingsTypeDef = TypedDict(
     "RemixSettingsTypeDef",
     {
         "ChannelMapping": ChannelMappingTypeDef,
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
     total=False,
 )
 
-ContainerSettingsOutputTypeDef = TypedDict(
-    "ContainerSettingsOutputTypeDef",
-    {
-        "CmfcSettings": CmfcSettingsTypeDef,
-        "Container": ContainerTypeType,
-        "F4vSettings": F4vSettingsTypeDef,
-        "M2tsSettings": M2tsSettingsOutputTypeDef,
-        "M3u8Settings": M3u8SettingsOutputTypeDef,
-        "MovSettings": MovSettingsTypeDef,
-        "Mp4Settings": Mp4SettingsTypeDef,
-        "MpdSettings": MpdSettingsTypeDef,
-        "MxfSettings": MxfSettingsTypeDef,
-    },
-    total=False,
-)
-
 ContainerSettingsTypeDef = TypedDict(
     "ContainerSettingsTypeDef",
     {
         "CmfcSettings": CmfcSettingsTypeDef,
         "Container": ContainerTypeType,
         "F4vSettings": F4vSettingsTypeDef,
         "M2tsSettings": M2tsSettingsTypeDef,
@@ -3235,29 +2880,14 @@
         "Mp4Settings": Mp4SettingsTypeDef,
         "MpdSettings": MpdSettingsTypeDef,
         "MxfSettings": MxfSettingsTypeDef,
     },
     total=False,
 )
 
-VideoPreprocessorOutputTypeDef = TypedDict(
-    "VideoPreprocessorOutputTypeDef",
-    {
-        "ColorCorrector": ColorCorrectorTypeDef,
-        "Deinterlacer": DeinterlacerTypeDef,
-        "DolbyVision": DolbyVisionTypeDef,
-        "Hdr10Plus": Hdr10PlusTypeDef,
-        "ImageInserter": ImageInserterOutputTypeDef,
-        "NoiseReducer": NoiseReducerTypeDef,
-        "PartnerWatermarking": PartnerWatermarkingTypeDef,
-        "TimecodeBurnin": TimecodeBurninTypeDef,
-    },
-    total=False,
-)
-
 VideoPreprocessorTypeDef = TypedDict(
     "VideoPreprocessorTypeDef",
     {
         "ColorCorrector": ColorCorrectorTypeDef,
         "Deinterlacer": DeinterlacerTypeDef,
         "DolbyVision": DolbyVisionTypeDef,
         "Hdr10Plus": Hdr10PlusTypeDef,
@@ -3333,22 +2963,14 @@
         "Vp8Settings": Vp8SettingsTypeDef,
         "Vp9Settings": Vp9SettingsTypeDef,
         "XavcSettings": XavcSettingsTypeDef,
     },
     total=False,
 )
 
-AutomatedEncodingSettingsOutputTypeDef = TypedDict(
-    "AutomatedEncodingSettingsOutputTypeDef",
-    {
-        "AbrSettings": AutomatedAbrSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 AutomatedEncodingSettingsTypeDef = TypedDict(
     "AutomatedEncodingSettingsTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsTypeDef,
     },
     total=False,
 )
@@ -3359,51 +2981,14 @@
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "SourceSettings": CaptionSourceSettingsTypeDef,
     },
     total=False,
 )
 
-AudioDescriptionOutputTypeDef = TypedDict(
-    "AudioDescriptionOutputTypeDef",
-    {
-        "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
-        "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
-        "AudioSourceName": str,
-        "AudioType": int,
-        "AudioTypeControl": AudioTypeControlType,
-        "CodecSettings": AudioCodecSettingsTypeDef,
-        "CustomLanguageCode": str,
-        "LanguageCode": LanguageCodeType,
-        "LanguageCodeControl": AudioLanguageCodeControlType,
-        "RemixSettings": RemixSettingsOutputTypeDef,
-        "StreamName": str,
-    },
-    total=False,
-)
-
-AudioSelectorOutputTypeDef = TypedDict(
-    "AudioSelectorOutputTypeDef",
-    {
-        "AudioDurationCorrection": AudioDurationCorrectionType,
-        "CustomLanguageCode": str,
-        "DefaultSelection": AudioDefaultSelectionType,
-        "ExternalAudioFileInput": str,
-        "HlsRenditionGroupSettings": HlsRenditionGroupSettingsTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "Offset": int,
-        "Pids": List[int],
-        "ProgramSelection": int,
-        "RemixSettings": RemixSettingsOutputTypeDef,
-        "SelectorType": AudioSelectorTypeType,
-        "Tracks": List[int],
-    },
-    total=False,
-)
-
 AudioDescriptionTypeDef = TypedDict(
     "AudioDescriptionTypeDef",
     {
         "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
         "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
         "AudioSourceName": str,
         "AudioType": int,
@@ -3433,48 +3018,14 @@
         "RemixSettings": RemixSettingsTypeDef,
         "SelectorType": AudioSelectorTypeType,
         "Tracks": Sequence[int],
     },
     total=False,
 )
 
-CmafGroupSettingsOutputTypeDef = TypedDict(
-    "CmafGroupSettingsOutputTypeDef",
-    {
-        "AdditionalManifests": List[CmafAdditionalManifestOutputTypeDef],
-        "BaseUrl": str,
-        "ClientCache": CmafClientCacheType,
-        "CodecSpecification": CmafCodecSpecificationType,
-        "DashManifestStyle": DashManifestStyleType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "Encryption": CmafEncryptionSettingsOutputTypeDef,
-        "FragmentLength": int,
-        "ImageBasedTrickPlay": CmafImageBasedTrickPlayType,
-        "ImageBasedTrickPlaySettings": CmafImageBasedTrickPlaySettingsTypeDef,
-        "ManifestCompression": CmafManifestCompressionType,
-        "ManifestDurationFormat": CmafManifestDurationFormatType,
-        "MinBufferTime": int,
-        "MinFinalSegmentLength": float,
-        "MpdManifestBandwidthType": CmafMpdManifestBandwidthTypeType,
-        "MpdProfile": CmafMpdProfileType,
-        "PtsOffsetHandlingForBFrames": CmafPtsOffsetHandlingForBFramesType,
-        "SegmentControl": CmafSegmentControlType,
-        "SegmentLength": int,
-        "SegmentLengthControl": CmafSegmentLengthControlType,
-        "StreamInfResolution": CmafStreamInfResolutionType,
-        "TargetDurationCompatibilityMode": CmafTargetDurationCompatibilityModeType,
-        "VideoCompositionOffsets": CmafVideoCompositionOffsetsType,
-        "WriteDashManifest": CmafWriteDASHManifestType,
-        "WriteHlsManifest": CmafWriteHLSManifestType,
-        "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
-    },
-    total=False,
-)
-
 CmafGroupSettingsTypeDef = TypedDict(
     "CmafGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[CmafAdditionalManifestTypeDef],
         "BaseUrl": str,
         "ClientCache": CmafClientCacheType,
         "CodecSpecification": CmafCodecSpecificationType,
@@ -3501,42 +3052,14 @@
         "WriteDashManifest": CmafWriteDASHManifestType,
         "WriteHlsManifest": CmafWriteHLSManifestType,
         "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
     },
     total=False,
 )
 
-DashIsoGroupSettingsOutputTypeDef = TypedDict(
-    "DashIsoGroupSettingsOutputTypeDef",
-    {
-        "AdditionalManifests": List[DashAdditionalManifestOutputTypeDef],
-        "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
-        "BaseUrl": str,
-        "DashManifestStyle": DashManifestStyleType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "Encryption": DashIsoEncryptionSettingsOutputTypeDef,
-        "FragmentLength": int,
-        "HbbtvCompliance": DashIsoHbbtvComplianceType,
-        "ImageBasedTrickPlay": DashIsoImageBasedTrickPlayType,
-        "ImageBasedTrickPlaySettings": DashIsoImageBasedTrickPlaySettingsTypeDef,
-        "MinBufferTime": int,
-        "MinFinalSegmentLength": float,
-        "MpdManifestBandwidthType": DashIsoMpdManifestBandwidthTypeType,
-        "MpdProfile": DashIsoMpdProfileType,
-        "PtsOffsetHandlingForBFrames": DashIsoPtsOffsetHandlingForBFramesType,
-        "SegmentControl": DashIsoSegmentControlType,
-        "SegmentLength": int,
-        "SegmentLengthControl": DashIsoSegmentLengthControlType,
-        "VideoCompositionOffsets": DashIsoVideoCompositionOffsetsType,
-        "WriteSegmentTimelineInRepresentation": DashIsoWriteSegmentTimelineInRepresentationType,
-    },
-    total=False,
-)
-
 DashIsoGroupSettingsTypeDef = TypedDict(
     "DashIsoGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[DashAdditionalManifestTypeDef],
         "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
         "BaseUrl": str,
         "DashManifestStyle": DashManifestStyleType,
@@ -3566,53 +3089,14 @@
     {
         "Destination": str,
         "DestinationSettings": DestinationSettingsTypeDef,
     },
     total=False,
 )
 
-HlsGroupSettingsOutputTypeDef = TypedDict(
-    "HlsGroupSettingsOutputTypeDef",
-    {
-        "AdMarkers": List[HlsAdMarkersType],
-        "AdditionalManifests": List[HlsAdditionalManifestOutputTypeDef],
-        "AudioOnlyHeader": HlsAudioOnlyHeaderType,
-        "BaseUrl": str,
-        "CaptionLanguageMappings": List[HlsCaptionLanguageMappingTypeDef],
-        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
-        "CaptionSegmentLengthControl": HlsCaptionSegmentLengthControlType,
-        "ClientCache": HlsClientCacheType,
-        "CodecSpecification": HlsCodecSpecificationType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "DirectoryStructure": HlsDirectoryStructureType,
-        "Encryption": HlsEncryptionSettingsOutputTypeDef,
-        "ImageBasedTrickPlay": HlsImageBasedTrickPlayType,
-        "ImageBasedTrickPlaySettings": HlsImageBasedTrickPlaySettingsTypeDef,
-        "ManifestCompression": HlsManifestCompressionType,
-        "ManifestDurationFormat": HlsManifestDurationFormatType,
-        "MinFinalSegmentLength": float,
-        "MinSegmentLength": int,
-        "OutputSelection": HlsOutputSelectionType,
-        "ProgramDateTime": HlsProgramDateTimeType,
-        "ProgramDateTimePeriod": int,
-        "ProgressiveWriteHlsManifest": HlsProgressiveWriteHlsManifestType,
-        "SegmentControl": HlsSegmentControlType,
-        "SegmentLength": int,
-        "SegmentLengthControl": HlsSegmentLengthControlType,
-        "SegmentsPerSubdirectory": int,
-        "StreamInfResolution": HlsStreamInfResolutionType,
-        "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
-        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
-        "TimedMetadataId3Period": int,
-        "TimestampDeltaMilliseconds": int,
-    },
-    total=False,
-)
-
 HlsGroupSettingsTypeDef = TypedDict(
     "HlsGroupSettingsTypeDef",
     {
         "AdMarkers": Sequence[HlsAdMarkersType],
         "AdditionalManifests": Sequence[HlsAdditionalManifestTypeDef],
         "AudioOnlyHeader": HlsAudioOnlyHeaderType,
         "BaseUrl": str,
@@ -3644,29 +3128,14 @@
         "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
         "TimestampDeltaMilliseconds": int,
     },
     total=False,
 )
 
-MsSmoothGroupSettingsOutputTypeDef = TypedDict(
-    "MsSmoothGroupSettingsOutputTypeDef",
-    {
-        "AdditionalManifests": List[MsSmoothAdditionalManifestOutputTypeDef],
-        "AudioDeduplication": MsSmoothAudioDeduplicationType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "Encryption": MsSmoothEncryptionSettingsOutputTypeDef,
-        "FragmentLength": int,
-        "FragmentLengthControl": MsSmoothFragmentLengthControlType,
-        "ManifestEncoding": MsSmoothManifestEncodingType,
-    },
-    total=False,
-)
-
 MsSmoothGroupSettingsTypeDef = TypedDict(
     "MsSmoothGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[MsSmoothAdditionalManifestTypeDef],
         "AudioDeduplication": MsSmoothAudioDeduplicationType,
         "Destination": str,
         "DestinationSettings": DestinationSettingsTypeDef,
@@ -3674,36 +3143,14 @@
         "FragmentLength": int,
         "FragmentLengthControl": MsSmoothFragmentLengthControlType,
         "ManifestEncoding": MsSmoothManifestEncodingType,
     },
     total=False,
 )
 
-VideoDescriptionOutputTypeDef = TypedDict(
-    "VideoDescriptionOutputTypeDef",
-    {
-        "AfdSignaling": AfdSignalingType,
-        "AntiAlias": AntiAliasType,
-        "CodecSettings": VideoCodecSettingsTypeDef,
-        "ColorMetadata": ColorMetadataType,
-        "Crop": RectangleTypeDef,
-        "DropFrameTimecode": DropFrameTimecodeType,
-        "FixedAfd": int,
-        "Height": int,
-        "Position": RectangleTypeDef,
-        "RespondToAfd": RespondToAfdType,
-        "ScalingBehavior": ScalingBehaviorType,
-        "Sharpness": int,
-        "TimecodeInsertion": VideoTimecodeInsertionType,
-        "VideoPreprocessors": VideoPreprocessorOutputTypeDef,
-        "Width": int,
-    },
-    total=False,
-)
-
 VideoDescriptionTypeDef = TypedDict(
     "VideoDescriptionTypeDef",
     {
         "AfdSignaling": AfdSignalingType,
         "AntiAlias": AntiAliasType,
         "CodecSettings": VideoCodecSettingsTypeDef,
         "ColorMetadata": ColorMetadataType,
@@ -3718,72 +3165,14 @@
         "TimecodeInsertion": VideoTimecodeInsertionType,
         "VideoPreprocessors": VideoPreprocessorTypeDef,
         "Width": int,
     },
     total=False,
 )
 
-InputOutputTypeDef = TypedDict(
-    "InputOutputTypeDef",
-    {
-        "AdvancedInputFilter": AdvancedInputFilterType,
-        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
-        "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
-        "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
-        "CaptionSelectors": Dict[str, CaptionSelectorTypeDef],
-        "Crop": RectangleTypeDef,
-        "DeblockFilter": InputDeblockFilterType,
-        "DecryptionSettings": InputDecryptionSettingsTypeDef,
-        "DenoiseFilter": InputDenoiseFilterType,
-        "DolbyVisionMetadataXml": str,
-        "FileInput": str,
-        "FilterEnable": InputFilterEnableType,
-        "FilterStrength": int,
-        "ImageInserter": ImageInserterOutputTypeDef,
-        "InputClippings": List[InputClippingTypeDef],
-        "InputScanType": InputScanTypeType,
-        "Position": RectangleTypeDef,
-        "ProgramNumber": int,
-        "PsiControl": InputPsiControlType,
-        "SupplementalImps": List[str],
-        "TimecodeSource": InputTimecodeSourceType,
-        "TimecodeStart": str,
-        "VideoGenerator": InputVideoGeneratorTypeDef,
-        "VideoSelector": VideoSelectorTypeDef,
-    },
-    total=False,
-)
-
-InputTemplateOutputTypeDef = TypedDict(
-    "InputTemplateOutputTypeDef",
-    {
-        "AdvancedInputFilter": AdvancedInputFilterType,
-        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
-        "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
-        "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
-        "CaptionSelectors": Dict[str, CaptionSelectorTypeDef],
-        "Crop": RectangleTypeDef,
-        "DeblockFilter": InputDeblockFilterType,
-        "DenoiseFilter": InputDenoiseFilterType,
-        "DolbyVisionMetadataXml": str,
-        "FilterEnable": InputFilterEnableType,
-        "FilterStrength": int,
-        "ImageInserter": ImageInserterOutputTypeDef,
-        "InputClippings": List[InputClippingTypeDef],
-        "InputScanType": InputScanTypeType,
-        "Position": RectangleTypeDef,
-        "ProgramNumber": int,
-        "PsiControl": InputPsiControlType,
-        "TimecodeSource": InputTimecodeSourceType,
-        "TimecodeStart": str,
-        "VideoSelector": VideoSelectorTypeDef,
-    },
-    total=False,
-)
-
 InputTemplateTypeDef = TypedDict(
     "InputTemplateTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
         "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
         "AudioSelectorGroups": Mapping[str, AudioSelectorGroupTypeDef],
         "AudioSelectors": Mapping[str, AudioSelectorTypeDef],
@@ -3834,51 +3223,27 @@
         "TimecodeStart": str,
         "VideoGenerator": InputVideoGeneratorTypeDef,
         "VideoSelector": VideoSelectorTypeDef,
     },
     total=False,
 )
 
-OutputGroupSettingsOutputTypeDef = TypedDict(
-    "OutputGroupSettingsOutputTypeDef",
-    {
-        "CmafGroupSettings": CmafGroupSettingsOutputTypeDef,
-        "DashIsoGroupSettings": DashIsoGroupSettingsOutputTypeDef,
-        "FileGroupSettings": FileGroupSettingsTypeDef,
-        "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
-        "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
-        "Type": OutputGroupTypeType,
-    },
-    total=False,
-)
-
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "CmafGroupSettings": CmafGroupSettingsTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsTypeDef,
         "FileGroupSettings": FileGroupSettingsTypeDef,
         "HlsGroupSettings": HlsGroupSettingsTypeDef,
         "MsSmoothGroupSettings": MsSmoothGroupSettingsTypeDef,
         "Type": OutputGroupTypeType,
     },
     total=False,
 )
 
-PresetSettingsOutputTypeDef = TypedDict(
-    "PresetSettingsOutputTypeDef",
-    {
-        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
-        "CaptionDescriptions": List[CaptionDescriptionPresetOutputTypeDef],
-        "ContainerSettings": ContainerSettingsOutputTypeDef,
-        "VideoDescription": VideoDescriptionOutputTypeDef,
-    },
-    total=False,
-)
-
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "CaptionDescriptions": Sequence[CaptionDescriptionTypeDef],
         "ContainerSettings": ContainerSettingsTypeDef,
         "Extension": str,
@@ -3897,51 +3262,14 @@
         "CaptionDescriptions": Sequence[CaptionDescriptionPresetTypeDef],
         "ContainerSettings": ContainerSettingsTypeDef,
         "VideoDescription": VideoDescriptionTypeDef,
     },
     total=False,
 )
 
-_RequiredPresetTypeDef = TypedDict(
-    "_RequiredPresetTypeDef",
-    {
-        "Name": str,
-        "Settings": PresetSettingsOutputTypeDef,
-    },
-)
-_OptionalPresetTypeDef = TypedDict(
-    "_OptionalPresetTypeDef",
-    {
-        "Arn": str,
-        "Category": str,
-        "CreatedAt": datetime,
-        "Description": str,
-        "LastUpdated": datetime,
-        "Type": TypeType,
-    },
-    total=False,
-)
-
-
-class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
-    pass
-
-
-OutputGroupOutputTypeDef = TypedDict(
-    "OutputGroupOutputTypeDef",
-    {
-        "AutomatedEncodingSettings": AutomatedEncodingSettingsOutputTypeDef,
-        "CustomName": str,
-        "Name": str,
-        "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
-        "Outputs": List[OutputTypeDef],
-    },
-    total=False,
-)
-
 OutputGroupTypeDef = TypedDict(
     "OutputGroupTypeDef",
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
@@ -3963,22 +3291,42 @@
         "Category": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
+_RequiredPresetTypeDef = TypedDict(
+    "_RequiredPresetTypeDef",
+    {
+        "Name": str,
+        "Settings": PresetSettingsTypeDef,
+    },
+)
+_OptionalPresetTypeDef = TypedDict(
+    "_OptionalPresetTypeDef",
+    {
+        "Arn": str,
+        "Category": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "LastUpdated": datetime,
+        "Type": TypeType,
+    },
+    total=False,
+)
+
+class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
+    pass
 
-PresetSettingsUnionTypeDef = Union[PresetSettingsTypeDef, PresetSettingsOutputTypeDef]
 _RequiredUpdatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePresetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdatePresetRequestRequestTypeDef = TypedDict(
@@ -3987,20 +3335,56 @@
         "Category": str,
         "Description": str,
         "Settings": PresetSettingsTypeDef,
     },
     total=False,
 )
 
-
 class UpdatePresetRequestRequestTypeDef(
     _RequiredUpdatePresetRequestRequestTypeDef, _OptionalUpdatePresetRequestRequestTypeDef
 ):
     pass
 
+JobSettingsTypeDef = TypedDict(
+    "JobSettingsTypeDef",
+    {
+        "AdAvailOffset": int,
+        "AvailBlanking": AvailBlankingTypeDef,
+        "Esam": EsamSettingsTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesTypeDef,
+        "Inputs": Sequence[InputTypeDef],
+        "KantarWatermark": KantarWatermarkSettingsTypeDef,
+        "MotionImageInserter": MotionImageInserterTypeDef,
+        "NielsenConfiguration": NielsenConfigurationTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
+        "OutputGroups": Sequence[OutputGroupTypeDef],
+        "TimecodeConfig": TimecodeConfigTypeDef,
+        "TimedMetadataInsertion": TimedMetadataInsertionTypeDef,
+    },
+    total=False,
+)
+
+JobTemplateSettingsTypeDef = TypedDict(
+    "JobTemplateSettingsTypeDef",
+    {
+        "AdAvailOffset": int,
+        "AvailBlanking": AvailBlankingTypeDef,
+        "Esam": EsamSettingsTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesTypeDef,
+        "Inputs": Sequence[InputTemplateTypeDef],
+        "KantarWatermark": KantarWatermarkSettingsTypeDef,
+        "MotionImageInserter": MotionImageInserterTypeDef,
+        "NielsenConfiguration": NielsenConfigurationTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
+        "OutputGroups": Sequence[OutputGroupTypeDef],
+        "TimecodeConfig": TimecodeConfigTypeDef,
+        "TimedMetadataInsertion": TimedMetadataInsertionTypeDef,
+    },
+    total=False,
+)
 
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -4027,95 +3411,49 @@
     "UpdatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JobSettingsOutputTypeDef = TypedDict(
-    "JobSettingsOutputTypeDef",
-    {
-        "AdAvailOffset": int,
-        "AvailBlanking": AvailBlankingTypeDef,
-        "Esam": EsamSettingsTypeDef,
-        "ExtendedDataServices": ExtendedDataServicesTypeDef,
-        "Inputs": List[InputOutputTypeDef],
-        "KantarWatermark": KantarWatermarkSettingsTypeDef,
-        "MotionImageInserter": MotionImageInserterTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
-        "OutputGroups": List[OutputGroupOutputTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
-        "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
-    },
-    total=False,
-)
-
-JobTemplateSettingsOutputTypeDef = TypedDict(
-    "JobTemplateSettingsOutputTypeDef",
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
     {
-        "AdAvailOffset": int,
-        "AvailBlanking": AvailBlankingTypeDef,
-        "Esam": EsamSettingsTypeDef,
-        "ExtendedDataServices": ExtendedDataServicesTypeDef,
-        "Inputs": List[InputTemplateOutputTypeDef],
-        "KantarWatermark": KantarWatermarkSettingsTypeDef,
-        "MotionImageInserter": MotionImageInserterTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
-        "OutputGroups": List[OutputGroupOutputTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
-        "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
+        "Role": str,
+        "Settings": JobSettingsTypeDef,
     },
-    total=False,
 )
-
-JobSettingsTypeDef = TypedDict(
-    "JobSettingsTypeDef",
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
     {
-        "AdAvailOffset": int,
-        "AvailBlanking": AvailBlankingTypeDef,
-        "Esam": EsamSettingsTypeDef,
-        "ExtendedDataServices": ExtendedDataServicesTypeDef,
-        "Inputs": Sequence[InputTypeDef],
-        "KantarWatermark": KantarWatermarkSettingsTypeDef,
-        "MotionImageInserter": MotionImageInserterTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
-        "OutputGroups": Sequence[OutputGroupTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
-        "TimedMetadataInsertion": TimedMetadataInsertionTypeDef,
+        "AccelerationSettings": AccelerationSettingsTypeDef,
+        "BillingTagsSource": BillingTagsSourceType,
+        "ClientRequestToken": str,
+        "HopDestinations": Sequence[HopDestinationTypeDef],
+        "JobTemplate": str,
+        "Priority": int,
+        "Queue": str,
+        "SimulateReservedQueue": SimulateReservedQueueType,
+        "StatusUpdateInterval": StatusUpdateIntervalType,
+        "Tags": Mapping[str, str],
+        "UserMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-JobTemplateSettingsTypeDef = TypedDict(
-    "JobTemplateSettingsTypeDef",
-    {
-        "AdAvailOffset": int,
-        "AvailBlanking": AvailBlankingTypeDef,
-        "Esam": EsamSettingsTypeDef,
-        "ExtendedDataServices": ExtendedDataServicesTypeDef,
-        "Inputs": Sequence[InputTemplateTypeDef],
-        "KantarWatermark": KantarWatermarkSettingsTypeDef,
-        "MotionImageInserter": MotionImageInserterTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
-        "OutputGroups": Sequence[OutputGroupTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
-        "TimedMetadataInsertion": TimedMetadataInsertionTypeDef,
-    },
-    total=False,
-)
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
+):
+    pass
 
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
         "Role": str,
-        "Settings": JobSettingsOutputTypeDef,
+        "Settings": JobSettingsTypeDef,
     },
 )
 _OptionalJobTypeDef = TypedDict(
     "_OptionalJobTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
         "AccelerationStatus": AccelerationStatusType,
@@ -4142,114 +3480,72 @@
         "Timing": TimingTypeDef,
         "UserMetadata": Dict[str, str],
         "Warnings": List[WarningGroupTypeDef],
     },
     total=False,
 )
 
-
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
 
-
-_RequiredJobTemplateTypeDef = TypedDict(
-    "_RequiredJobTemplateTypeDef",
+_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
-        "Settings": JobTemplateSettingsOutputTypeDef,
+        "Settings": JobTemplateSettingsTypeDef,
     },
 )
-_OptionalJobTemplateTypeDef = TypedDict(
-    "_OptionalJobTemplateTypeDef",
+_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobTemplateRequestRequestTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
-        "Arn": str,
         "Category": str,
-        "CreatedAt": datetime,
         "Description": str,
-        "HopDestinations": List[HopDestinationTypeDef],
-        "LastUpdated": datetime,
-        "Priority": int,
-        "Queue": str,
-        "StatusUpdateInterval": StatusUpdateIntervalType,
-        "Type": TypeType,
-    },
-    total=False,
-)
-
-
-class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
-    pass
-
-
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "Role": str,
-        "Settings": JobSettingsTypeDef,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "AccelerationSettings": AccelerationSettingsTypeDef,
-        "BillingTagsSource": BillingTagsSourceType,
-        "ClientRequestToken": str,
         "HopDestinations": Sequence[HopDestinationTypeDef],
-        "JobTemplate": str,
         "Priority": int,
         "Queue": str,
-        "SimulateReservedQueue": SimulateReservedQueueType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Tags": Mapping[str, str],
-        "UserMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
+class CreateJobTemplateRequestRequestTypeDef(
+    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
-
-JobSettingsUnionTypeDef = Union[JobSettingsTypeDef, JobSettingsOutputTypeDef]
-_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobTemplateRequestRequestTypeDef",
+_RequiredJobTemplateTypeDef = TypedDict(
+    "_RequiredJobTemplateTypeDef",
     {
         "Name": str,
         "Settings": JobTemplateSettingsTypeDef,
     },
 )
-_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobTemplateRequestRequestTypeDef",
+_OptionalJobTemplateTypeDef = TypedDict(
+    "_OptionalJobTemplateTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
+        "Arn": str,
         "Category": str,
+        "CreatedAt": datetime,
         "Description": str,
-        "HopDestinations": Sequence[HopDestinationTypeDef],
+        "HopDestinations": List[HopDestinationTypeDef],
+        "LastUpdated": datetime,
         "Priority": int,
         "Queue": str,
         "StatusUpdateInterval": StatusUpdateIntervalType,
-        "Tags": Mapping[str, str],
+        "Type": TypeType,
     },
     total=False,
 )
 
-
-class CreateJobTemplateRequestRequestTypeDef(
-    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
-):
+class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
     pass
 
-
-JobTemplateSettingsUnionTypeDef = Union[
-    JobTemplateSettingsTypeDef, JobTemplateSettingsOutputTypeDef
-]
 _RequiredUpdateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateJobTemplateRequestRequestTypeDef = TypedDict(
@@ -4263,21 +3559,19 @@
         "Queue": str,
         "Settings": JobTemplateSettingsTypeDef,
         "StatusUpdateInterval": StatusUpdateIntervalType,
     },
     total=False,
 )
 
-
 class UpdateJobTemplateRequestRequestTypeDef(
     _RequiredUpdateJobTemplateRequestRequestTypeDef, _OptionalUpdateJobTemplateRequestRequestTypeDef
 ):
     pass
 
-
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert/type_defs.pyi` & `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert/type_defs.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     from types_aiobotocore_mediaconvert.type_defs import AacSettingsTypeDef
 
     data: AacSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence, Union
+from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
     AacAudioDescriptionBroadcasterMixType,
     AacCodecProfileType,
     AacCodingModeType,
     AacRateControlModeType,
     AacRawFormatType,
@@ -426,14 +426,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AacSettingsTypeDef",
     "Ac3SettingsTypeDef",
     "AccelerationSettingsTypeDef",
     "AdvancedInputFilterSettingsTypeDef",
     "AiffSettingsTypeDef",
     "AllowedRenditionSizeTypeDef",
@@ -444,15 +445,14 @@
     "Eac3SettingsTypeDef",
     "Mp2SettingsTypeDef",
     "Mp3SettingsTypeDef",
     "OpusSettingsTypeDef",
     "VorbisSettingsTypeDef",
     "WavSettingsTypeDef",
     "AudioNormalizationSettingsTypeDef",
-    "AudioSelectorGroupOutputTypeDef",
     "AudioSelectorGroupTypeDef",
     "HlsRenditionGroupSettingsTypeDef",
     "ForceIncludeRenditionSizeTypeDef",
     "MinBottomRenditionSizeTypeDef",
     "MinTopRenditionSizeTypeDef",
     "Av1QvbrSettingsTypeDef",
     "AvailBlankingTypeDef",
@@ -461,47 +461,40 @@
     "BurninDestinationSettingsTypeDef",
     "CancelJobRequestRequestTypeDef",
     "DvbSubDestinationSettingsTypeDef",
     "EmbeddedDestinationSettingsTypeDef",
     "ImscDestinationSettingsTypeDef",
     "SccDestinationSettingsTypeDef",
     "SrtDestinationSettingsTypeDef",
-    "TeletextDestinationSettingsOutputTypeDef",
+    "TeletextDestinationSettingsTypeDef",
     "TtmlDestinationSettingsTypeDef",
     "WebvttDestinationSettingsTypeDef",
-    "TeletextDestinationSettingsTypeDef",
     "CaptionSourceFramerateTypeDef",
     "DvbSubSourceSettingsTypeDef",
     "EmbeddedSourceSettingsTypeDef",
     "TeletextSourceSettingsTypeDef",
     "TrackSourceSettingsTypeDef",
     "WebvttHlsSourceSettingsTypeDef",
-    "OutputChannelMappingOutputTypeDef",
     "OutputChannelMappingTypeDef",
     "ClipLimitsTypeDef",
-    "CmafAdditionalManifestOutputTypeDef",
     "CmafAdditionalManifestTypeDef",
-    "SpekeKeyProviderCmafOutputTypeDef",
-    "StaticKeyProviderTypeDef",
     "SpekeKeyProviderCmafTypeDef",
+    "StaticKeyProviderTypeDef",
     "CmafImageBasedTrickPlaySettingsTypeDef",
     "CmfcSettingsTypeDef",
     "Hdr10MetadataTypeDef",
     "F4vSettingsTypeDef",
-    "M3u8SettingsOutputTypeDef",
+    "M3u8SettingsTypeDef",
     "MovSettingsTypeDef",
     "Mp4SettingsTypeDef",
     "MpdSettingsTypeDef",
-    "M3u8SettingsTypeDef",
     "HopDestinationTypeDef",
     "ResponseMetadataTypeDef",
     "ReservationPlanSettingsTypeDef",
-    "DashAdditionalManifestOutputTypeDef",
     "DashAdditionalManifestTypeDef",
-    "SpekeKeyProviderOutputTypeDef",
     "SpekeKeyProviderTypeDef",
     "DashIsoImageBasedTrickPlaySettingsTypeDef",
     "DeinterlacerTypeDef",
     "DeleteJobTemplateRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DeleteQueueRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
@@ -520,25 +513,24 @@
     "GetJobTemplateRequestRequestTypeDef",
     "PolicyTypeDef",
     "GetPresetRequestRequestTypeDef",
     "GetQueueRequestRequestTypeDef",
     "H264QvbrSettingsTypeDef",
     "H265QvbrSettingsTypeDef",
     "Hdr10PlusTypeDef",
-    "HlsAdditionalManifestOutputTypeDef",
     "HlsAdditionalManifestTypeDef",
     "HlsCaptionLanguageMappingTypeDef",
     "HlsImageBasedTrickPlaySettingsTypeDef",
     "HlsSettingsTypeDef",
     "Id3InsertionTypeDef",
     "InsertableImageTypeDef",
     "InputClippingTypeDef",
     "InputDecryptionSettingsTypeDef",
-    "InputVideoGeneratorTypeDef",
     "RectangleTypeDef",
+    "InputVideoGeneratorTypeDef",
     "JobMessagesTypeDef",
     "KantarWatermarkSettingsTypeDef",
     "NielsenConfigurationTypeDef",
     "NielsenNonLinearWatermarkSettingsTypeDef",
     "TimecodeConfigTypeDef",
     "QueueTransitionTypeDef",
     "TimingTypeDef",
@@ -549,15 +541,14 @@
     "ListQueuesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ResourceTagsTypeDef",
     "M2tsScte35EsamTypeDef",
     "MotionImageInsertionFramerateTypeDef",
     "MotionImageInsertionOffsetTypeDef",
     "Mpeg2SettingsTypeDef",
-    "MsSmoothAdditionalManifestOutputTypeDef",
     "MsSmoothAdditionalManifestTypeDef",
     "MxfXavcProfileSettingsTypeDef",
     "NexGuardFileMarkerSettingsTypeDef",
     "NoiseReducerFilterSettingsTypeDef",
     "NoiseReducerSpatialFilterSettingsTypeDef",
     "NoiseReducerTemporalFilterSettingsTypeDef",
     "VideoDetailTypeDef",
@@ -573,32 +564,25 @@
     "Vp9SettingsTypeDef",
     "Xavc4kIntraCbgProfileSettingsTypeDef",
     "Xavc4kIntraVbrProfileSettingsTypeDef",
     "Xavc4kProfileSettingsTypeDef",
     "XavcHdIntraCbgProfileSettingsTypeDef",
     "XavcHdProfileSettingsTypeDef",
     "AudioCodecSettingsTypeDef",
-    "AutomatedAbrRuleOutputTypeDef",
     "AutomatedAbrRuleTypeDef",
     "Av1SettingsTypeDef",
     "AvcIntraSettingsTypeDef",
-    "CaptionDestinationSettingsOutputTypeDef",
     "CaptionDestinationSettingsTypeDef",
     "FileSourceSettingsTypeDef",
-    "ChannelMappingOutputTypeDef",
     "ChannelMappingTypeDef",
-    "CmafEncryptionSettingsOutputTypeDef",
     "CmafEncryptionSettingsTypeDef",
     "ColorCorrectorTypeDef",
     "VideoSelectorTypeDef",
     "CreateQueueRequestRequestTypeDef",
     "UpdateQueueRequestRequestTypeDef",
-    "DashIsoEncryptionSettingsOutputTypeDef",
-    "HlsEncryptionSettingsOutputTypeDef",
-    "MsSmoothEncryptionSettingsOutputTypeDef",
     "DashIsoEncryptionSettingsTypeDef",
     "HlsEncryptionSettingsTypeDef",
     "MsSmoothEncryptionSettingsTypeDef",
     "DescribeEndpointsRequestDescribeEndpointsPaginateTypeDef",
     "ListJobTemplatesRequestListJobTemplatesPaginateTypeDef",
     "ListJobsRequestListJobsPaginateTypeDef",
     "ListPresetsRequestListPresetsPaginateTypeDef",
@@ -608,95 +592,69 @@
     "EsamSettingsTypeDef",
     "GetPolicyResponseTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
     "H264SettingsTypeDef",
     "H265SettingsTypeDef",
     "OutputSettingsTypeDef",
-    "TimedMetadataInsertionOutputTypeDef",
     "TimedMetadataInsertionTypeDef",
-    "ImageInserterOutputTypeDef",
     "ImageInserterTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "M2tsSettingsOutputTypeDef",
     "M2tsSettingsTypeDef",
     "MotionImageInserterTypeDef",
     "MxfSettingsTypeDef",
     "PartnerWatermarkingTypeDef",
     "NoiseReducerTypeDef",
     "OutputDetailTypeDef",
     "QueueTypeDef",
     "S3DestinationSettingsTypeDef",
     "XavcSettingsTypeDef",
-    "AutomatedAbrSettingsOutputTypeDef",
     "AutomatedAbrSettingsTypeDef",
-    "CaptionDescriptionPresetOutputTypeDef",
     "CaptionDescriptionPresetTypeDef",
     "CaptionDescriptionTypeDef",
     "CaptionSourceSettingsTypeDef",
-    "RemixSettingsOutputTypeDef",
     "RemixSettingsTypeDef",
-    "ContainerSettingsOutputTypeDef",
     "ContainerSettingsTypeDef",
-    "VideoPreprocessorOutputTypeDef",
     "VideoPreprocessorTypeDef",
     "OutputGroupDetailTypeDef",
     "CreateQueueResponseTypeDef",
     "GetQueueResponseTypeDef",
     "ListQueuesResponseTypeDef",
     "UpdateQueueResponseTypeDef",
     "DestinationSettingsTypeDef",
     "VideoCodecSettingsTypeDef",
-    "AutomatedEncodingSettingsOutputTypeDef",
     "AutomatedEncodingSettingsTypeDef",
     "CaptionSelectorTypeDef",
-    "AudioDescriptionOutputTypeDef",
-    "AudioSelectorOutputTypeDef",
     "AudioDescriptionTypeDef",
     "AudioSelectorTypeDef",
-    "CmafGroupSettingsOutputTypeDef",
     "CmafGroupSettingsTypeDef",
-    "DashIsoGroupSettingsOutputTypeDef",
     "DashIsoGroupSettingsTypeDef",
     "FileGroupSettingsTypeDef",
-    "HlsGroupSettingsOutputTypeDef",
     "HlsGroupSettingsTypeDef",
-    "MsSmoothGroupSettingsOutputTypeDef",
     "MsSmoothGroupSettingsTypeDef",
-    "VideoDescriptionOutputTypeDef",
     "VideoDescriptionTypeDef",
-    "InputOutputTypeDef",
-    "InputTemplateOutputTypeDef",
     "InputTemplateTypeDef",
     "InputTypeDef",
-    "OutputGroupSettingsOutputTypeDef",
     "OutputGroupSettingsTypeDef",
-    "PresetSettingsOutputTypeDef",
     "OutputTypeDef",
     "PresetSettingsTypeDef",
-    "PresetTypeDef",
-    "OutputGroupOutputTypeDef",
     "OutputGroupTypeDef",
     "CreatePresetRequestRequestTypeDef",
-    "PresetSettingsUnionTypeDef",
+    "PresetTypeDef",
     "UpdatePresetRequestRequestTypeDef",
+    "JobSettingsTypeDef",
+    "JobTemplateSettingsTypeDef",
     "CreatePresetResponseTypeDef",
     "GetPresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "UpdatePresetResponseTypeDef",
-    "JobSettingsOutputTypeDef",
-    "JobTemplateSettingsOutputTypeDef",
-    "JobSettingsTypeDef",
-    "JobTemplateSettingsTypeDef",
-    "JobTypeDef",
-    "JobTemplateTypeDef",
     "CreateJobRequestRequestTypeDef",
-    "JobSettingsUnionTypeDef",
+    "JobTypeDef",
     "CreateJobTemplateRequestRequestTypeDef",
-    "JobTemplateSettingsUnionTypeDef",
+    "JobTemplateTypeDef",
     "UpdateJobTemplateRequestRequestTypeDef",
     "CreateJobResponseTypeDef",
     "GetJobResponseTypeDef",
     "ListJobsResponseTypeDef",
     "CreateJobTemplateResponseTypeDef",
     "GetJobTemplateResponseTypeDef",
     "ListJobTemplatesResponseTypeDef",
@@ -912,22 +870,14 @@
         "PeakCalculation": AudioNormalizationPeakCalculationType,
         "TargetLkfs": float,
         "TruePeakLimiterThreshold": float,
     },
     total=False,
 )
 
-AudioSelectorGroupOutputTypeDef = TypedDict(
-    "AudioSelectorGroupOutputTypeDef",
-    {
-        "AudioSelectorNames": List[str],
-    },
-    total=False,
-)
-
 AudioSelectorGroupTypeDef = TypedDict(
     "AudioSelectorGroupTypeDef",
     {
         "AudioSelectorNames": Sequence[str],
     },
     total=False,
 )
@@ -1102,19 +1052,19 @@
     "SrtDestinationSettingsTypeDef",
     {
         "StylePassthrough": SrtStylePassthroughType,
     },
     total=False,
 )
 
-TeletextDestinationSettingsOutputTypeDef = TypedDict(
-    "TeletextDestinationSettingsOutputTypeDef",
+TeletextDestinationSettingsTypeDef = TypedDict(
+    "TeletextDestinationSettingsTypeDef",
     {
         "PageNumber": str,
-        "PageTypes": List[TeletextPageTypeType],
+        "PageTypes": Sequence[TeletextPageTypeType],
     },
     total=False,
 )
 
 TtmlDestinationSettingsTypeDef = TypedDict(
     "TtmlDestinationSettingsTypeDef",
     {
@@ -1128,23 +1078,14 @@
     {
         "Accessibility": WebvttAccessibilitySubsType,
         "StylePassthrough": WebvttStylePassthroughType,
     },
     total=False,
 )
 
-TeletextDestinationSettingsTypeDef = TypedDict(
-    "TeletextDestinationSettingsTypeDef",
-    {
-        "PageNumber": str,
-        "PageTypes": Sequence[TeletextPageTypeType],
-    },
-    total=False,
-)
-
 CaptionSourceFramerateTypeDef = TypedDict(
     "CaptionSourceFramerateTypeDef",
     {
         "FramerateDenominator": int,
         "FramerateNumerator": int,
     },
     total=False,
@@ -1191,23 +1132,14 @@
         "RenditionGroupId": str,
         "RenditionLanguageCode": LanguageCodeType,
         "RenditionName": str,
     },
     total=False,
 )
 
-OutputChannelMappingOutputTypeDef = TypedDict(
-    "OutputChannelMappingOutputTypeDef",
-    {
-        "InputChannels": List[int],
-        "InputChannelsFineTune": List[float],
-    },
-    total=False,
-)
-
 OutputChannelMappingTypeDef = TypedDict(
     "OutputChannelMappingTypeDef",
     {
         "InputChannels": Sequence[int],
         "InputChannelsFineTune": Sequence[float],
     },
     total=False,
@@ -1220,38 +1152,29 @@
         "MaximumYUV": int,
         "MinimumRGBTolerance": int,
         "MinimumYUV": int,
     },
     total=False,
 )
 
-CmafAdditionalManifestOutputTypeDef = TypedDict(
-    "CmafAdditionalManifestOutputTypeDef",
-    {
-        "ManifestNameModifier": str,
-        "SelectedOutputs": List[str],
-    },
-    total=False,
-)
-
 CmafAdditionalManifestTypeDef = TypedDict(
     "CmafAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
-SpekeKeyProviderCmafOutputTypeDef = TypedDict(
-    "SpekeKeyProviderCmafOutputTypeDef",
+SpekeKeyProviderCmafTypeDef = TypedDict(
+    "SpekeKeyProviderCmafTypeDef",
     {
         "CertificateArn": str,
-        "DashSignaledSystemIds": List[str],
-        "HlsSignaledSystemIds": List[str],
+        "DashSignaledSystemIds": Sequence[str],
+        "HlsSignaledSystemIds": Sequence[str],
         "ResourceId": str,
         "Url": str,
     },
     total=False,
 )
 
 StaticKeyProviderTypeDef = TypedDict(
@@ -1261,26 +1184,14 @@
         "KeyFormatVersions": str,
         "StaticKeyValue": str,
         "Url": str,
     },
     total=False,
 )
 
-SpekeKeyProviderCmafTypeDef = TypedDict(
-    "SpekeKeyProviderCmafTypeDef",
-    {
-        "CertificateArn": str,
-        "DashSignaledSystemIds": Sequence[str],
-        "HlsSignaledSystemIds": Sequence[str],
-        "ResourceId": str,
-        "Url": str,
-    },
-    total=False,
-)
-
 CmafImageBasedTrickPlaySettingsTypeDef = TypedDict(
     "CmafImageBasedTrickPlaySettingsTypeDef",
     {
         "IntervalCadence": CmafIntervalCadenceType,
         "ThumbnailHeight": int,
         "ThumbnailInterval": float,
         "ThumbnailWidth": int,
@@ -1334,20 +1245,20 @@
     "F4vSettingsTypeDef",
     {
         "MoovPlacement": F4vMoovPlacementType,
     },
     total=False,
 )
 
-M3u8SettingsOutputTypeDef = TypedDict(
-    "M3u8SettingsOutputTypeDef",
+M3u8SettingsTypeDef = TypedDict(
+    "M3u8SettingsTypeDef",
     {
         "AudioDuration": M3u8AudioDurationType,
         "AudioFramesPerPes": int,
-        "AudioPids": List[int],
+        "AudioPids": Sequence[int],
         "DataPTSControl": M3u8DataPtsControlType,
         "MaxPcrInterval": int,
         "NielsenId3": M3u8NielsenId3Type,
         "PatInterval": int,
         "PcrControl": M3u8PcrControlType,
         "PcrPid": int,
         "PmtInterval": int,
@@ -1403,40 +1314,14 @@
         "TimedMetadataBoxVersion": MpdTimedMetadataBoxVersionType,
         "TimedMetadataSchemeIdUri": str,
         "TimedMetadataValue": str,
     },
     total=False,
 )
 
-M3u8SettingsTypeDef = TypedDict(
-    "M3u8SettingsTypeDef",
-    {
-        "AudioDuration": M3u8AudioDurationType,
-        "AudioFramesPerPes": int,
-        "AudioPids": Sequence[int],
-        "DataPTSControl": M3u8DataPtsControlType,
-        "MaxPcrInterval": int,
-        "NielsenId3": M3u8NielsenId3Type,
-        "PatInterval": int,
-        "PcrControl": M3u8PcrControlType,
-        "PcrPid": int,
-        "PmtInterval": int,
-        "PmtPid": int,
-        "PrivateMetadataPid": int,
-        "ProgramNumber": int,
-        "Scte35Pid": int,
-        "Scte35Source": M3u8Scte35SourceType,
-        "TimedMetadata": TimedMetadataType,
-        "TimedMetadataPid": int,
-        "TransportStreamId": int,
-        "VideoPid": int,
-    },
-    total=False,
-)
-
 HopDestinationTypeDef = TypedDict(
     "HopDestinationTypeDef",
     {
         "Priority": int,
         "Queue": str,
         "WaitMinutes": int,
     },
@@ -1459,43 +1344,23 @@
     {
         "Commitment": Literal["ONE_YEAR"],
         "RenewalType": RenewalTypeType,
         "ReservedSlots": int,
     },
 )
 
-DashAdditionalManifestOutputTypeDef = TypedDict(
-    "DashAdditionalManifestOutputTypeDef",
-    {
-        "ManifestNameModifier": str,
-        "SelectedOutputs": List[str],
-    },
-    total=False,
-)
-
 DashAdditionalManifestTypeDef = TypedDict(
     "DashAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
 )
 
-SpekeKeyProviderOutputTypeDef = TypedDict(
-    "SpekeKeyProviderOutputTypeDef",
-    {
-        "CertificateArn": str,
-        "ResourceId": str,
-        "SystemIds": List[str],
-        "Url": str,
-    },
-    total=False,
-)
-
 SpekeKeyProviderTypeDef = TypedDict(
     "SpekeKeyProviderTypeDef",
     {
         "CertificateArn": str,
         "ResourceId": str,
         "SystemIds": Sequence[str],
         "Url": str,
@@ -1719,23 +1584,14 @@
     {
         "MasteringMonitorNits": int,
         "TargetMonitorNits": int,
     },
     total=False,
 )
 
-HlsAdditionalManifestOutputTypeDef = TypedDict(
-    "HlsAdditionalManifestOutputTypeDef",
-    {
-        "ManifestNameModifier": str,
-        "SelectedOutputs": List[str],
-    },
-    total=False,
-)
-
 HlsAdditionalManifestTypeDef = TypedDict(
     "HlsAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
@@ -1822,33 +1678,33 @@
         "EncryptedDecryptionKey": str,
         "InitializationVector": str,
         "KmsKeyRegion": str,
     },
     total=False,
 )
 
-InputVideoGeneratorTypeDef = TypedDict(
-    "InputVideoGeneratorTypeDef",
-    {
-        "Duration": int,
-    },
-    total=False,
-)
-
 RectangleTypeDef = TypedDict(
     "RectangleTypeDef",
     {
         "Height": int,
         "Width": int,
         "X": int,
         "Y": int,
     },
     total=False,
 )
 
+InputVideoGeneratorTypeDef = TypedDict(
+    "InputVideoGeneratorTypeDef",
+    {
+        "Duration": int,
+    },
+    total=False,
+)
+
 JobMessagesTypeDef = TypedDict(
     "JobMessagesTypeDef",
     {
         "Info": List[str],
         "Warning": List[str],
     },
     total=False,
@@ -2065,23 +1921,14 @@
         "Syntax": Mpeg2SyntaxType,
         "Telecine": Mpeg2TelecineType,
         "TemporalAdaptiveQuantization": Mpeg2TemporalAdaptiveQuantizationType,
     },
     total=False,
 )
 
-MsSmoothAdditionalManifestOutputTypeDef = TypedDict(
-    "MsSmoothAdditionalManifestOutputTypeDef",
-    {
-        "ManifestNameModifier": str,
-        "SelectedOutputs": List[str],
-    },
-    total=False,
-)
-
 MsSmoothAdditionalManifestTypeDef = TypedDict(
     "MsSmoothAdditionalManifestTypeDef",
     {
         "ManifestNameModifier": str,
         "SelectedOutputs": Sequence[str],
     },
     total=False,
@@ -2225,19 +2072,21 @@
     "_OptionalUntagResourceRequestRequestTypeDef",
     {
         "TagKeys": Sequence[str],
     },
     total=False,
 )
 
+
 class UntagResourceRequestRequestTypeDef(
     _RequiredUntagResourceRequestRequestTypeDef, _OptionalUntagResourceRequestRequestTypeDef
 ):
     pass
 
+
 Vc3SettingsTypeDef = TypedDict(
     "Vc3SettingsTypeDef",
     {
         "FramerateControl": Vc3FramerateControlType,
         "FramerateConversionAlgorithm": Vc3FramerateConversionAlgorithmType,
         "FramerateDenominator": int,
         "FramerateNumerator": int,
@@ -2359,26 +2208,14 @@
         "OpusSettings": OpusSettingsTypeDef,
         "VorbisSettings": VorbisSettingsTypeDef,
         "WavSettings": WavSettingsTypeDef,
     },
     total=False,
 )
 
-AutomatedAbrRuleOutputTypeDef = TypedDict(
-    "AutomatedAbrRuleOutputTypeDef",
-    {
-        "AllowedRenditions": List[AllowedRenditionSizeTypeDef],
-        "ForceIncludeRenditions": List[ForceIncludeRenditionSizeTypeDef],
-        "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
-        "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
-        "Type": RuleTypeType,
-    },
-    total=False,
-)
-
 AutomatedAbrRuleTypeDef = TypedDict(
     "AutomatedAbrRuleTypeDef",
     {
         "AllowedRenditions": Sequence[AllowedRenditionSizeTypeDef],
         "ForceIncludeRenditions": Sequence[ForceIncludeRenditionSizeTypeDef],
         "MinBottomRenditionSize": MinBottomRenditionSizeTypeDef,
         "MinTopRenditionSize": MinTopRenditionSizeTypeDef,
@@ -2420,31 +2257,14 @@
         "ScanTypeConversionMode": AvcIntraScanTypeConversionModeType,
         "SlowPal": AvcIntraSlowPalType,
         "Telecine": AvcIntraTelecineType,
     },
     total=False,
 )
 
-CaptionDestinationSettingsOutputTypeDef = TypedDict(
-    "CaptionDestinationSettingsOutputTypeDef",
-    {
-        "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
-        "DestinationType": CaptionDestinationTypeType,
-        "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
-        "EmbeddedDestinationSettings": EmbeddedDestinationSettingsTypeDef,
-        "ImscDestinationSettings": ImscDestinationSettingsTypeDef,
-        "SccDestinationSettings": SccDestinationSettingsTypeDef,
-        "SrtDestinationSettings": SrtDestinationSettingsTypeDef,
-        "TeletextDestinationSettings": TeletextDestinationSettingsOutputTypeDef,
-        "TtmlDestinationSettings": TtmlDestinationSettingsTypeDef,
-        "WebvttDestinationSettings": WebvttDestinationSettingsTypeDef,
-    },
-    total=False,
-)
-
 CaptionDestinationSettingsTypeDef = TypedDict(
     "CaptionDestinationSettingsTypeDef",
     {
         "BurninDestinationSettings": BurninDestinationSettingsTypeDef,
         "DestinationType": CaptionDestinationTypeType,
         "DvbSubDestinationSettings": DvbSubDestinationSettingsTypeDef,
         "EmbeddedDestinationSettings": EmbeddedDestinationSettingsTypeDef,
@@ -2467,43 +2287,22 @@
         "SourceFile": str,
         "TimeDelta": int,
         "TimeDeltaUnits": FileSourceTimeDeltaUnitsType,
     },
     total=False,
 )
 
-ChannelMappingOutputTypeDef = TypedDict(
-    "ChannelMappingOutputTypeDef",
-    {
-        "OutputChannels": List[OutputChannelMappingOutputTypeDef],
-    },
-    total=False,
-)
-
 ChannelMappingTypeDef = TypedDict(
     "ChannelMappingTypeDef",
     {
         "OutputChannels": Sequence[OutputChannelMappingTypeDef],
     },
     total=False,
 )
 
-CmafEncryptionSettingsOutputTypeDef = TypedDict(
-    "CmafEncryptionSettingsOutputTypeDef",
-    {
-        "ConstantInitializationVector": str,
-        "EncryptionMethod": CmafEncryptionTypeType,
-        "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
-        "SpekeKeyProvider": SpekeKeyProviderCmafOutputTypeDef,
-        "StaticKeyProvider": StaticKeyProviderTypeDef,
-        "Type": CmafKeyProviderTypeType,
-    },
-    total=False,
-)
-
 CmafEncryptionSettingsTypeDef = TypedDict(
     "CmafEncryptionSettingsTypeDef",
     {
         "ConstantInitializationVector": str,
         "EncryptionMethod": CmafEncryptionTypeType,
         "InitializationVectorInManifest": CmafInitializationVectorInManifestType,
         "SpekeKeyProvider": SpekeKeyProviderCmafTypeDef,
@@ -2561,19 +2360,21 @@
         "ReservationPlanSettings": ReservationPlanSettingsTypeDef,
         "Status": QueueStatusType,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateQueueRequestRequestTypeDef(
     _RequiredCreateQueueRequestRequestTypeDef, _OptionalCreateQueueRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateQueueRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateQueueRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateQueueRequestRequestTypeDef = TypedDict(
@@ -2582,49 +2383,20 @@
         "Description": str,
         "ReservationPlanSettings": ReservationPlanSettingsTypeDef,
         "Status": QueueStatusType,
     },
     total=False,
 )
 
+
 class UpdateQueueRequestRequestTypeDef(
     _RequiredUpdateQueueRequestRequestTypeDef, _OptionalUpdateQueueRequestRequestTypeDef
 ):
     pass
 
-DashIsoEncryptionSettingsOutputTypeDef = TypedDict(
-    "DashIsoEncryptionSettingsOutputTypeDef",
-    {
-        "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-    total=False,
-)
-
-HlsEncryptionSettingsOutputTypeDef = TypedDict(
-    "HlsEncryptionSettingsOutputTypeDef",
-    {
-        "ConstantInitializationVector": str,
-        "EncryptionMethod": HlsEncryptionTypeType,
-        "InitializationVectorInManifest": HlsInitializationVectorInManifestType,
-        "OfflineEncrypted": HlsOfflineEncryptedType,
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-        "StaticKeyProvider": StaticKeyProviderTypeDef,
-        "Type": HlsKeyProviderTypeType,
-    },
-    total=False,
-)
-
-MsSmoothEncryptionSettingsOutputTypeDef = TypedDict(
-    "MsSmoothEncryptionSettingsOutputTypeDef",
-    {
-        "SpekeKeyProvider": SpekeKeyProviderOutputTypeDef,
-    },
-    total=False,
-)
 
 DashIsoEncryptionSettingsTypeDef = TypedDict(
     "DashIsoEncryptionSettingsTypeDef",
     {
         "PlaybackDeviceCompatibility": DashIsoPlaybackDeviceCompatibilityType,
         "SpekeKeyProvider": SpekeKeyProviderTypeDef,
     },
@@ -2860,39 +2632,22 @@
     "OutputSettingsTypeDef",
     {
         "HlsSettings": HlsSettingsTypeDef,
     },
     total=False,
 )
 
-TimedMetadataInsertionOutputTypeDef = TypedDict(
-    "TimedMetadataInsertionOutputTypeDef",
-    {
-        "Id3Insertions": List[Id3InsertionTypeDef],
-    },
-    total=False,
-)
-
 TimedMetadataInsertionTypeDef = TypedDict(
     "TimedMetadataInsertionTypeDef",
     {
         "Id3Insertions": Sequence[Id3InsertionTypeDef],
     },
     total=False,
 )
 
-ImageInserterOutputTypeDef = TypedDict(
-    "ImageInserterOutputTypeDef",
-    {
-        "InsertableImages": List[InsertableImageTypeDef],
-        "SdrReferenceWhiteLevel": int,
-    },
-    total=False,
-)
-
 ImageInserterTypeDef = TypedDict(
     "ImageInserterTypeDef",
     {
         "InsertableImages": Sequence[InsertableImageTypeDef],
         "SdrReferenceWhiteLevel": int,
     },
     total=False,
@@ -2902,60 +2657,14 @@
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": ResourceTagsTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-M2tsSettingsOutputTypeDef = TypedDict(
-    "M2tsSettingsOutputTypeDef",
-    {
-        "AudioBufferModel": M2tsAudioBufferModelType,
-        "AudioDuration": M2tsAudioDurationType,
-        "AudioFramesPerPes": int,
-        "AudioPids": List[int],
-        "Bitrate": int,
-        "BufferModel": M2tsBufferModelType,
-        "DataPTSControl": M2tsDataPtsControlType,
-        "DvbNitSettings": DvbNitSettingsTypeDef,
-        "DvbSdtSettings": DvbSdtSettingsTypeDef,
-        "DvbSubPids": List[int],
-        "DvbTdtSettings": DvbTdtSettingsTypeDef,
-        "DvbTeletextPid": int,
-        "EbpAudioInterval": M2tsEbpAudioIntervalType,
-        "EbpPlacement": M2tsEbpPlacementType,
-        "EsRateInPes": M2tsEsRateInPesType,
-        "ForceTsVideoEbpOrder": M2tsForceTsVideoEbpOrderType,
-        "FragmentTime": float,
-        "KlvMetadata": M2tsKlvMetadataType,
-        "MaxPcrInterval": int,
-        "MinEbpInterval": int,
-        "NielsenId3": M2tsNielsenId3Type,
-        "NullPacketBitrate": float,
-        "PatInterval": int,
-        "PcrControl": M2tsPcrControlType,
-        "PcrPid": int,
-        "PmtInterval": int,
-        "PmtPid": int,
-        "PrivateMetadataPid": int,
-        "ProgramNumber": int,
-        "RateMode": M2tsRateModeType,
-        "Scte35Esam": M2tsScte35EsamTypeDef,
-        "Scte35Pid": int,
-        "Scte35Source": M2tsScte35SourceType,
-        "SegmentationMarkers": M2tsSegmentationMarkersType,
-        "SegmentationStyle": M2tsSegmentationStyleType,
-        "SegmentationTime": float,
-        "TimedMetadataPid": int,
-        "TransportStreamId": int,
-        "VideoPid": int,
-    },
-    total=False,
-)
-
 M2tsSettingsTypeDef = TypedDict(
     "M2tsSettingsTypeDef",
     {
         "AudioBufferModel": M2tsAudioBufferModelType,
         "AudioDuration": M2tsAudioDurationType,
         "AudioFramesPerPes": int,
         "AudioPids": Sequence[int],
@@ -3068,17 +2777,19 @@
         "Status": QueueStatusType,
         "SubmittedJobsCount": int,
         "Type": TypeType,
     },
     total=False,
 )
 
+
 class QueueTypeDef(_RequiredQueueTypeDef, _OptionalQueueTypeDef):
     pass
 
+
 S3DestinationSettingsTypeDef = TypedDict(
     "S3DestinationSettingsTypeDef",
     {
         "AccessControl": S3DestinationAccessControlTypeDef,
         "Encryption": S3EncryptionSettingsTypeDef,
     },
     total=False,
@@ -3103,47 +2814,25 @@
         "Xavc4kProfileSettings": Xavc4kProfileSettingsTypeDef,
         "XavcHdIntraCbgProfileSettings": XavcHdIntraCbgProfileSettingsTypeDef,
         "XavcHdProfileSettings": XavcHdProfileSettingsTypeDef,
     },
     total=False,
 )
 
-AutomatedAbrSettingsOutputTypeDef = TypedDict(
-    "AutomatedAbrSettingsOutputTypeDef",
-    {
-        "MaxAbrBitrate": int,
-        "MaxRenditions": int,
-        "MinAbrBitrate": int,
-        "Rules": List[AutomatedAbrRuleOutputTypeDef],
-    },
-    total=False,
-)
-
 AutomatedAbrSettingsTypeDef = TypedDict(
     "AutomatedAbrSettingsTypeDef",
     {
         "MaxAbrBitrate": int,
         "MaxRenditions": int,
         "MinAbrBitrate": int,
         "Rules": Sequence[AutomatedAbrRuleTypeDef],
     },
     total=False,
 )
 
-CaptionDescriptionPresetOutputTypeDef = TypedDict(
-    "CaptionDescriptionPresetOutputTypeDef",
-    {
-        "CustomLanguageCode": str,
-        "DestinationSettings": CaptionDestinationSettingsOutputTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "LanguageDescription": str,
-    },
-    total=False,
-)
-
 CaptionDescriptionPresetTypeDef = TypedDict(
     "CaptionDescriptionPresetTypeDef",
     {
         "CustomLanguageCode": str,
         "DestinationSettings": CaptionDestinationSettingsTypeDef,
         "LanguageCode": LanguageCodeType,
         "LanguageDescription": str,
@@ -3174,50 +2863,24 @@
         "TeletextSourceSettings": TeletextSourceSettingsTypeDef,
         "TrackSourceSettings": TrackSourceSettingsTypeDef,
         "WebvttHlsSourceSettings": WebvttHlsSourceSettingsTypeDef,
     },
     total=False,
 )
 
-RemixSettingsOutputTypeDef = TypedDict(
-    "RemixSettingsOutputTypeDef",
-    {
-        "ChannelMapping": ChannelMappingOutputTypeDef,
-        "ChannelsIn": int,
-        "ChannelsOut": int,
-    },
-    total=False,
-)
-
 RemixSettingsTypeDef = TypedDict(
     "RemixSettingsTypeDef",
     {
         "ChannelMapping": ChannelMappingTypeDef,
         "ChannelsIn": int,
         "ChannelsOut": int,
     },
     total=False,
 )
 
-ContainerSettingsOutputTypeDef = TypedDict(
-    "ContainerSettingsOutputTypeDef",
-    {
-        "CmfcSettings": CmfcSettingsTypeDef,
-        "Container": ContainerTypeType,
-        "F4vSettings": F4vSettingsTypeDef,
-        "M2tsSettings": M2tsSettingsOutputTypeDef,
-        "M3u8Settings": M3u8SettingsOutputTypeDef,
-        "MovSettings": MovSettingsTypeDef,
-        "Mp4Settings": Mp4SettingsTypeDef,
-        "MpdSettings": MpdSettingsTypeDef,
-        "MxfSettings": MxfSettingsTypeDef,
-    },
-    total=False,
-)
-
 ContainerSettingsTypeDef = TypedDict(
     "ContainerSettingsTypeDef",
     {
         "CmfcSettings": CmfcSettingsTypeDef,
         "Container": ContainerTypeType,
         "F4vSettings": F4vSettingsTypeDef,
         "M2tsSettings": M2tsSettingsTypeDef,
@@ -3226,29 +2889,14 @@
         "Mp4Settings": Mp4SettingsTypeDef,
         "MpdSettings": MpdSettingsTypeDef,
         "MxfSettings": MxfSettingsTypeDef,
     },
     total=False,
 )
 
-VideoPreprocessorOutputTypeDef = TypedDict(
-    "VideoPreprocessorOutputTypeDef",
-    {
-        "ColorCorrector": ColorCorrectorTypeDef,
-        "Deinterlacer": DeinterlacerTypeDef,
-        "DolbyVision": DolbyVisionTypeDef,
-        "Hdr10Plus": Hdr10PlusTypeDef,
-        "ImageInserter": ImageInserterOutputTypeDef,
-        "NoiseReducer": NoiseReducerTypeDef,
-        "PartnerWatermarking": PartnerWatermarkingTypeDef,
-        "TimecodeBurnin": TimecodeBurninTypeDef,
-    },
-    total=False,
-)
-
 VideoPreprocessorTypeDef = TypedDict(
     "VideoPreprocessorTypeDef",
     {
         "ColorCorrector": ColorCorrectorTypeDef,
         "Deinterlacer": DeinterlacerTypeDef,
         "DolbyVision": DolbyVisionTypeDef,
         "Hdr10Plus": Hdr10PlusTypeDef,
@@ -3324,22 +2972,14 @@
         "Vp8Settings": Vp8SettingsTypeDef,
         "Vp9Settings": Vp9SettingsTypeDef,
         "XavcSettings": XavcSettingsTypeDef,
     },
     total=False,
 )
 
-AutomatedEncodingSettingsOutputTypeDef = TypedDict(
-    "AutomatedEncodingSettingsOutputTypeDef",
-    {
-        "AbrSettings": AutomatedAbrSettingsOutputTypeDef,
-    },
-    total=False,
-)
-
 AutomatedEncodingSettingsTypeDef = TypedDict(
     "AutomatedEncodingSettingsTypeDef",
     {
         "AbrSettings": AutomatedAbrSettingsTypeDef,
     },
     total=False,
 )
@@ -3350,51 +2990,14 @@
         "CustomLanguageCode": str,
         "LanguageCode": LanguageCodeType,
         "SourceSettings": CaptionSourceSettingsTypeDef,
     },
     total=False,
 )
 
-AudioDescriptionOutputTypeDef = TypedDict(
-    "AudioDescriptionOutputTypeDef",
-    {
-        "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
-        "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
-        "AudioSourceName": str,
-        "AudioType": int,
-        "AudioTypeControl": AudioTypeControlType,
-        "CodecSettings": AudioCodecSettingsTypeDef,
-        "CustomLanguageCode": str,
-        "LanguageCode": LanguageCodeType,
-        "LanguageCodeControl": AudioLanguageCodeControlType,
-        "RemixSettings": RemixSettingsOutputTypeDef,
-        "StreamName": str,
-    },
-    total=False,
-)
-
-AudioSelectorOutputTypeDef = TypedDict(
-    "AudioSelectorOutputTypeDef",
-    {
-        "AudioDurationCorrection": AudioDurationCorrectionType,
-        "CustomLanguageCode": str,
-        "DefaultSelection": AudioDefaultSelectionType,
-        "ExternalAudioFileInput": str,
-        "HlsRenditionGroupSettings": HlsRenditionGroupSettingsTypeDef,
-        "LanguageCode": LanguageCodeType,
-        "Offset": int,
-        "Pids": List[int],
-        "ProgramSelection": int,
-        "RemixSettings": RemixSettingsOutputTypeDef,
-        "SelectorType": AudioSelectorTypeType,
-        "Tracks": List[int],
-    },
-    total=False,
-)
-
 AudioDescriptionTypeDef = TypedDict(
     "AudioDescriptionTypeDef",
     {
         "AudioChannelTaggingSettings": AudioChannelTaggingSettingsTypeDef,
         "AudioNormalizationSettings": AudioNormalizationSettingsTypeDef,
         "AudioSourceName": str,
         "AudioType": int,
@@ -3424,48 +3027,14 @@
         "RemixSettings": RemixSettingsTypeDef,
         "SelectorType": AudioSelectorTypeType,
         "Tracks": Sequence[int],
     },
     total=False,
 )
 
-CmafGroupSettingsOutputTypeDef = TypedDict(
-    "CmafGroupSettingsOutputTypeDef",
-    {
-        "AdditionalManifests": List[CmafAdditionalManifestOutputTypeDef],
-        "BaseUrl": str,
-        "ClientCache": CmafClientCacheType,
-        "CodecSpecification": CmafCodecSpecificationType,
-        "DashManifestStyle": DashManifestStyleType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "Encryption": CmafEncryptionSettingsOutputTypeDef,
-        "FragmentLength": int,
-        "ImageBasedTrickPlay": CmafImageBasedTrickPlayType,
-        "ImageBasedTrickPlaySettings": CmafImageBasedTrickPlaySettingsTypeDef,
-        "ManifestCompression": CmafManifestCompressionType,
-        "ManifestDurationFormat": CmafManifestDurationFormatType,
-        "MinBufferTime": int,
-        "MinFinalSegmentLength": float,
-        "MpdManifestBandwidthType": CmafMpdManifestBandwidthTypeType,
-        "MpdProfile": CmafMpdProfileType,
-        "PtsOffsetHandlingForBFrames": CmafPtsOffsetHandlingForBFramesType,
-        "SegmentControl": CmafSegmentControlType,
-        "SegmentLength": int,
-        "SegmentLengthControl": CmafSegmentLengthControlType,
-        "StreamInfResolution": CmafStreamInfResolutionType,
-        "TargetDurationCompatibilityMode": CmafTargetDurationCompatibilityModeType,
-        "VideoCompositionOffsets": CmafVideoCompositionOffsetsType,
-        "WriteDashManifest": CmafWriteDASHManifestType,
-        "WriteHlsManifest": CmafWriteHLSManifestType,
-        "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
-    },
-    total=False,
-)
-
 CmafGroupSettingsTypeDef = TypedDict(
     "CmafGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[CmafAdditionalManifestTypeDef],
         "BaseUrl": str,
         "ClientCache": CmafClientCacheType,
         "CodecSpecification": CmafCodecSpecificationType,
@@ -3492,42 +3061,14 @@
         "WriteDashManifest": CmafWriteDASHManifestType,
         "WriteHlsManifest": CmafWriteHLSManifestType,
         "WriteSegmentTimelineInRepresentation": CmafWriteSegmentTimelineInRepresentationType,
     },
     total=False,
 )
 
-DashIsoGroupSettingsOutputTypeDef = TypedDict(
-    "DashIsoGroupSettingsOutputTypeDef",
-    {
-        "AdditionalManifests": List[DashAdditionalManifestOutputTypeDef],
-        "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
-        "BaseUrl": str,
-        "DashManifestStyle": DashManifestStyleType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "Encryption": DashIsoEncryptionSettingsOutputTypeDef,
-        "FragmentLength": int,
-        "HbbtvCompliance": DashIsoHbbtvComplianceType,
-        "ImageBasedTrickPlay": DashIsoImageBasedTrickPlayType,
-        "ImageBasedTrickPlaySettings": DashIsoImageBasedTrickPlaySettingsTypeDef,
-        "MinBufferTime": int,
-        "MinFinalSegmentLength": float,
-        "MpdManifestBandwidthType": DashIsoMpdManifestBandwidthTypeType,
-        "MpdProfile": DashIsoMpdProfileType,
-        "PtsOffsetHandlingForBFrames": DashIsoPtsOffsetHandlingForBFramesType,
-        "SegmentControl": DashIsoSegmentControlType,
-        "SegmentLength": int,
-        "SegmentLengthControl": DashIsoSegmentLengthControlType,
-        "VideoCompositionOffsets": DashIsoVideoCompositionOffsetsType,
-        "WriteSegmentTimelineInRepresentation": DashIsoWriteSegmentTimelineInRepresentationType,
-    },
-    total=False,
-)
-
 DashIsoGroupSettingsTypeDef = TypedDict(
     "DashIsoGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[DashAdditionalManifestTypeDef],
         "AudioChannelConfigSchemeIdUri": DashIsoGroupAudioChannelConfigSchemeIdUriType,
         "BaseUrl": str,
         "DashManifestStyle": DashManifestStyleType,
@@ -3557,53 +3098,14 @@
     {
         "Destination": str,
         "DestinationSettings": DestinationSettingsTypeDef,
     },
     total=False,
 )
 
-HlsGroupSettingsOutputTypeDef = TypedDict(
-    "HlsGroupSettingsOutputTypeDef",
-    {
-        "AdMarkers": List[HlsAdMarkersType],
-        "AdditionalManifests": List[HlsAdditionalManifestOutputTypeDef],
-        "AudioOnlyHeader": HlsAudioOnlyHeaderType,
-        "BaseUrl": str,
-        "CaptionLanguageMappings": List[HlsCaptionLanguageMappingTypeDef],
-        "CaptionLanguageSetting": HlsCaptionLanguageSettingType,
-        "CaptionSegmentLengthControl": HlsCaptionSegmentLengthControlType,
-        "ClientCache": HlsClientCacheType,
-        "CodecSpecification": HlsCodecSpecificationType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "DirectoryStructure": HlsDirectoryStructureType,
-        "Encryption": HlsEncryptionSettingsOutputTypeDef,
-        "ImageBasedTrickPlay": HlsImageBasedTrickPlayType,
-        "ImageBasedTrickPlaySettings": HlsImageBasedTrickPlaySettingsTypeDef,
-        "ManifestCompression": HlsManifestCompressionType,
-        "ManifestDurationFormat": HlsManifestDurationFormatType,
-        "MinFinalSegmentLength": float,
-        "MinSegmentLength": int,
-        "OutputSelection": HlsOutputSelectionType,
-        "ProgramDateTime": HlsProgramDateTimeType,
-        "ProgramDateTimePeriod": int,
-        "ProgressiveWriteHlsManifest": HlsProgressiveWriteHlsManifestType,
-        "SegmentControl": HlsSegmentControlType,
-        "SegmentLength": int,
-        "SegmentLengthControl": HlsSegmentLengthControlType,
-        "SegmentsPerSubdirectory": int,
-        "StreamInfResolution": HlsStreamInfResolutionType,
-        "TargetDurationCompatibilityMode": HlsTargetDurationCompatibilityModeType,
-        "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
-        "TimedMetadataId3Period": int,
-        "TimestampDeltaMilliseconds": int,
-    },
-    total=False,
-)
-
 HlsGroupSettingsTypeDef = TypedDict(
     "HlsGroupSettingsTypeDef",
     {
         "AdMarkers": Sequence[HlsAdMarkersType],
         "AdditionalManifests": Sequence[HlsAdditionalManifestTypeDef],
         "AudioOnlyHeader": HlsAudioOnlyHeaderType,
         "BaseUrl": str,
@@ -3635,29 +3137,14 @@
         "TimedMetadataId3Frame": HlsTimedMetadataId3FrameType,
         "TimedMetadataId3Period": int,
         "TimestampDeltaMilliseconds": int,
     },
     total=False,
 )
 
-MsSmoothGroupSettingsOutputTypeDef = TypedDict(
-    "MsSmoothGroupSettingsOutputTypeDef",
-    {
-        "AdditionalManifests": List[MsSmoothAdditionalManifestOutputTypeDef],
-        "AudioDeduplication": MsSmoothAudioDeduplicationType,
-        "Destination": str,
-        "DestinationSettings": DestinationSettingsTypeDef,
-        "Encryption": MsSmoothEncryptionSettingsOutputTypeDef,
-        "FragmentLength": int,
-        "FragmentLengthControl": MsSmoothFragmentLengthControlType,
-        "ManifestEncoding": MsSmoothManifestEncodingType,
-    },
-    total=False,
-)
-
 MsSmoothGroupSettingsTypeDef = TypedDict(
     "MsSmoothGroupSettingsTypeDef",
     {
         "AdditionalManifests": Sequence[MsSmoothAdditionalManifestTypeDef],
         "AudioDeduplication": MsSmoothAudioDeduplicationType,
         "Destination": str,
         "DestinationSettings": DestinationSettingsTypeDef,
@@ -3665,36 +3152,14 @@
         "FragmentLength": int,
         "FragmentLengthControl": MsSmoothFragmentLengthControlType,
         "ManifestEncoding": MsSmoothManifestEncodingType,
     },
     total=False,
 )
 
-VideoDescriptionOutputTypeDef = TypedDict(
-    "VideoDescriptionOutputTypeDef",
-    {
-        "AfdSignaling": AfdSignalingType,
-        "AntiAlias": AntiAliasType,
-        "CodecSettings": VideoCodecSettingsTypeDef,
-        "ColorMetadata": ColorMetadataType,
-        "Crop": RectangleTypeDef,
-        "DropFrameTimecode": DropFrameTimecodeType,
-        "FixedAfd": int,
-        "Height": int,
-        "Position": RectangleTypeDef,
-        "RespondToAfd": RespondToAfdType,
-        "ScalingBehavior": ScalingBehaviorType,
-        "Sharpness": int,
-        "TimecodeInsertion": VideoTimecodeInsertionType,
-        "VideoPreprocessors": VideoPreprocessorOutputTypeDef,
-        "Width": int,
-    },
-    total=False,
-)
-
 VideoDescriptionTypeDef = TypedDict(
     "VideoDescriptionTypeDef",
     {
         "AfdSignaling": AfdSignalingType,
         "AntiAlias": AntiAliasType,
         "CodecSettings": VideoCodecSettingsTypeDef,
         "ColorMetadata": ColorMetadataType,
@@ -3709,72 +3174,14 @@
         "TimecodeInsertion": VideoTimecodeInsertionType,
         "VideoPreprocessors": VideoPreprocessorTypeDef,
         "Width": int,
     },
     total=False,
 )
 
-InputOutputTypeDef = TypedDict(
-    "InputOutputTypeDef",
-    {
-        "AdvancedInputFilter": AdvancedInputFilterType,
-        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
-        "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
-        "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
-        "CaptionSelectors": Dict[str, CaptionSelectorTypeDef],
-        "Crop": RectangleTypeDef,
-        "DeblockFilter": InputDeblockFilterType,
-        "DecryptionSettings": InputDecryptionSettingsTypeDef,
-        "DenoiseFilter": InputDenoiseFilterType,
-        "DolbyVisionMetadataXml": str,
-        "FileInput": str,
-        "FilterEnable": InputFilterEnableType,
-        "FilterStrength": int,
-        "ImageInserter": ImageInserterOutputTypeDef,
-        "InputClippings": List[InputClippingTypeDef],
-        "InputScanType": InputScanTypeType,
-        "Position": RectangleTypeDef,
-        "ProgramNumber": int,
-        "PsiControl": InputPsiControlType,
-        "SupplementalImps": List[str],
-        "TimecodeSource": InputTimecodeSourceType,
-        "TimecodeStart": str,
-        "VideoGenerator": InputVideoGeneratorTypeDef,
-        "VideoSelector": VideoSelectorTypeDef,
-    },
-    total=False,
-)
-
-InputTemplateOutputTypeDef = TypedDict(
-    "InputTemplateOutputTypeDef",
-    {
-        "AdvancedInputFilter": AdvancedInputFilterType,
-        "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
-        "AudioSelectorGroups": Dict[str, AudioSelectorGroupOutputTypeDef],
-        "AudioSelectors": Dict[str, AudioSelectorOutputTypeDef],
-        "CaptionSelectors": Dict[str, CaptionSelectorTypeDef],
-        "Crop": RectangleTypeDef,
-        "DeblockFilter": InputDeblockFilterType,
-        "DenoiseFilter": InputDenoiseFilterType,
-        "DolbyVisionMetadataXml": str,
-        "FilterEnable": InputFilterEnableType,
-        "FilterStrength": int,
-        "ImageInserter": ImageInserterOutputTypeDef,
-        "InputClippings": List[InputClippingTypeDef],
-        "InputScanType": InputScanTypeType,
-        "Position": RectangleTypeDef,
-        "ProgramNumber": int,
-        "PsiControl": InputPsiControlType,
-        "TimecodeSource": InputTimecodeSourceType,
-        "TimecodeStart": str,
-        "VideoSelector": VideoSelectorTypeDef,
-    },
-    total=False,
-)
-
 InputTemplateTypeDef = TypedDict(
     "InputTemplateTypeDef",
     {
         "AdvancedInputFilter": AdvancedInputFilterType,
         "AdvancedInputFilterSettings": AdvancedInputFilterSettingsTypeDef,
         "AudioSelectorGroups": Mapping[str, AudioSelectorGroupTypeDef],
         "AudioSelectors": Mapping[str, AudioSelectorTypeDef],
@@ -3825,51 +3232,27 @@
         "TimecodeStart": str,
         "VideoGenerator": InputVideoGeneratorTypeDef,
         "VideoSelector": VideoSelectorTypeDef,
     },
     total=False,
 )
 
-OutputGroupSettingsOutputTypeDef = TypedDict(
-    "OutputGroupSettingsOutputTypeDef",
-    {
-        "CmafGroupSettings": CmafGroupSettingsOutputTypeDef,
-        "DashIsoGroupSettings": DashIsoGroupSettingsOutputTypeDef,
-        "FileGroupSettings": FileGroupSettingsTypeDef,
-        "HlsGroupSettings": HlsGroupSettingsOutputTypeDef,
-        "MsSmoothGroupSettings": MsSmoothGroupSettingsOutputTypeDef,
-        "Type": OutputGroupTypeType,
-    },
-    total=False,
-)
-
 OutputGroupSettingsTypeDef = TypedDict(
     "OutputGroupSettingsTypeDef",
     {
         "CmafGroupSettings": CmafGroupSettingsTypeDef,
         "DashIsoGroupSettings": DashIsoGroupSettingsTypeDef,
         "FileGroupSettings": FileGroupSettingsTypeDef,
         "HlsGroupSettings": HlsGroupSettingsTypeDef,
         "MsSmoothGroupSettings": MsSmoothGroupSettingsTypeDef,
         "Type": OutputGroupTypeType,
     },
     total=False,
 )
 
-PresetSettingsOutputTypeDef = TypedDict(
-    "PresetSettingsOutputTypeDef",
-    {
-        "AudioDescriptions": List[AudioDescriptionOutputTypeDef],
-        "CaptionDescriptions": List[CaptionDescriptionPresetOutputTypeDef],
-        "ContainerSettings": ContainerSettingsOutputTypeDef,
-        "VideoDescription": VideoDescriptionOutputTypeDef,
-    },
-    total=False,
-)
-
 OutputTypeDef = TypedDict(
     "OutputTypeDef",
     {
         "AudioDescriptions": Sequence[AudioDescriptionTypeDef],
         "CaptionDescriptions": Sequence[CaptionDescriptionTypeDef],
         "ContainerSettings": ContainerSettingsTypeDef,
         "Extension": str,
@@ -3888,49 +3271,14 @@
         "CaptionDescriptions": Sequence[CaptionDescriptionPresetTypeDef],
         "ContainerSettings": ContainerSettingsTypeDef,
         "VideoDescription": VideoDescriptionTypeDef,
     },
     total=False,
 )
 
-_RequiredPresetTypeDef = TypedDict(
-    "_RequiredPresetTypeDef",
-    {
-        "Name": str,
-        "Settings": PresetSettingsOutputTypeDef,
-    },
-)
-_OptionalPresetTypeDef = TypedDict(
-    "_OptionalPresetTypeDef",
-    {
-        "Arn": str,
-        "Category": str,
-        "CreatedAt": datetime,
-        "Description": str,
-        "LastUpdated": datetime,
-        "Type": TypeType,
-    },
-    total=False,
-)
-
-class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
-    pass
-
-OutputGroupOutputTypeDef = TypedDict(
-    "OutputGroupOutputTypeDef",
-    {
-        "AutomatedEncodingSettings": AutomatedEncodingSettingsOutputTypeDef,
-        "CustomName": str,
-        "Name": str,
-        "OutputGroupSettings": OutputGroupSettingsOutputTypeDef,
-        "Outputs": List[OutputTypeDef],
-    },
-    total=False,
-)
-
 OutputGroupTypeDef = TypedDict(
     "OutputGroupTypeDef",
     {
         "AutomatedEncodingSettings": AutomatedEncodingSettingsTypeDef,
         "CustomName": str,
         "Name": str,
         "OutputGroupSettings": OutputGroupSettingsTypeDef,
@@ -3952,20 +3300,46 @@
         "Category": str,
         "Description": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
-PresetSettingsUnionTypeDef = Union[PresetSettingsTypeDef, PresetSettingsOutputTypeDef]
+
+_RequiredPresetTypeDef = TypedDict(
+    "_RequiredPresetTypeDef",
+    {
+        "Name": str,
+        "Settings": PresetSettingsTypeDef,
+    },
+)
+_OptionalPresetTypeDef = TypedDict(
+    "_OptionalPresetTypeDef",
+    {
+        "Arn": str,
+        "Category": str,
+        "CreatedAt": datetime,
+        "Description": str,
+        "LastUpdated": datetime,
+        "Type": TypeType,
+    },
+    total=False,
+)
+
+
+class PresetTypeDef(_RequiredPresetTypeDef, _OptionalPresetTypeDef):
+    pass
+
+
 _RequiredUpdatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePresetRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdatePresetRequestRequestTypeDef = TypedDict(
@@ -3974,19 +3348,59 @@
         "Category": str,
         "Description": str,
         "Settings": PresetSettingsTypeDef,
     },
     total=False,
 )
 
+
 class UpdatePresetRequestRequestTypeDef(
     _RequiredUpdatePresetRequestRequestTypeDef, _OptionalUpdatePresetRequestRequestTypeDef
 ):
     pass
 
+
+JobSettingsTypeDef = TypedDict(
+    "JobSettingsTypeDef",
+    {
+        "AdAvailOffset": int,
+        "AvailBlanking": AvailBlankingTypeDef,
+        "Esam": EsamSettingsTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesTypeDef,
+        "Inputs": Sequence[InputTypeDef],
+        "KantarWatermark": KantarWatermarkSettingsTypeDef,
+        "MotionImageInserter": MotionImageInserterTypeDef,
+        "NielsenConfiguration": NielsenConfigurationTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
+        "OutputGroups": Sequence[OutputGroupTypeDef],
+        "TimecodeConfig": TimecodeConfigTypeDef,
+        "TimedMetadataInsertion": TimedMetadataInsertionTypeDef,
+    },
+    total=False,
+)
+
+JobTemplateSettingsTypeDef = TypedDict(
+    "JobTemplateSettingsTypeDef",
+    {
+        "AdAvailOffset": int,
+        "AvailBlanking": AvailBlankingTypeDef,
+        "Esam": EsamSettingsTypeDef,
+        "ExtendedDataServices": ExtendedDataServicesTypeDef,
+        "Inputs": Sequence[InputTemplateTypeDef],
+        "KantarWatermark": KantarWatermarkSettingsTypeDef,
+        "MotionImageInserter": MotionImageInserterTypeDef,
+        "NielsenConfiguration": NielsenConfigurationTypeDef,
+        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
+        "OutputGroups": Sequence[OutputGroupTypeDef],
+        "TimecodeConfig": TimecodeConfigTypeDef,
+        "TimedMetadataInsertion": TimedMetadataInsertionTypeDef,
+    },
+    total=False,
+)
+
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -4012,95 +3426,51 @@
     "UpdatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-JobSettingsOutputTypeDef = TypedDict(
-    "JobSettingsOutputTypeDef",
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
     {
-        "AdAvailOffset": int,
-        "AvailBlanking": AvailBlankingTypeDef,
-        "Esam": EsamSettingsTypeDef,
-        "ExtendedDataServices": ExtendedDataServicesTypeDef,
-        "Inputs": List[InputOutputTypeDef],
-        "KantarWatermark": KantarWatermarkSettingsTypeDef,
-        "MotionImageInserter": MotionImageInserterTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
-        "OutputGroups": List[OutputGroupOutputTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
-        "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
+        "Role": str,
+        "Settings": JobSettingsTypeDef,
     },
-    total=False,
 )
-
-JobTemplateSettingsOutputTypeDef = TypedDict(
-    "JobTemplateSettingsOutputTypeDef",
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
     {
-        "AdAvailOffset": int,
-        "AvailBlanking": AvailBlankingTypeDef,
-        "Esam": EsamSettingsTypeDef,
-        "ExtendedDataServices": ExtendedDataServicesTypeDef,
-        "Inputs": List[InputTemplateOutputTypeDef],
-        "KantarWatermark": KantarWatermarkSettingsTypeDef,
-        "MotionImageInserter": MotionImageInserterTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
-        "OutputGroups": List[OutputGroupOutputTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
-        "TimedMetadataInsertion": TimedMetadataInsertionOutputTypeDef,
+        "AccelerationSettings": AccelerationSettingsTypeDef,
+        "BillingTagsSource": BillingTagsSourceType,
+        "ClientRequestToken": str,
+        "HopDestinations": Sequence[HopDestinationTypeDef],
+        "JobTemplate": str,
+        "Priority": int,
+        "Queue": str,
+        "SimulateReservedQueue": SimulateReservedQueueType,
+        "StatusUpdateInterval": StatusUpdateIntervalType,
+        "Tags": Mapping[str, str],
+        "UserMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-JobSettingsTypeDef = TypedDict(
-    "JobSettingsTypeDef",
-    {
-        "AdAvailOffset": int,
-        "AvailBlanking": AvailBlankingTypeDef,
-        "Esam": EsamSettingsTypeDef,
-        "ExtendedDataServices": ExtendedDataServicesTypeDef,
-        "Inputs": Sequence[InputTypeDef],
-        "KantarWatermark": KantarWatermarkSettingsTypeDef,
-        "MotionImageInserter": MotionImageInserterTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
-        "OutputGroups": Sequence[OutputGroupTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
-        "TimedMetadataInsertion": TimedMetadataInsertionTypeDef,
-    },
-    total=False,
-)
 
-JobTemplateSettingsTypeDef = TypedDict(
-    "JobTemplateSettingsTypeDef",
-    {
-        "AdAvailOffset": int,
-        "AvailBlanking": AvailBlankingTypeDef,
-        "Esam": EsamSettingsTypeDef,
-        "ExtendedDataServices": ExtendedDataServicesTypeDef,
-        "Inputs": Sequence[InputTemplateTypeDef],
-        "KantarWatermark": KantarWatermarkSettingsTypeDef,
-        "MotionImageInserter": MotionImageInserterTypeDef,
-        "NielsenConfiguration": NielsenConfigurationTypeDef,
-        "NielsenNonLinearWatermark": NielsenNonLinearWatermarkSettingsTypeDef,
-        "OutputGroups": Sequence[OutputGroupTypeDef],
-        "TimecodeConfig": TimecodeConfigTypeDef,
-        "TimedMetadataInsertion": TimedMetadataInsertionTypeDef,
-    },
-    total=False,
-)
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
+):
+    pass
+
 
 _RequiredJobTypeDef = TypedDict(
     "_RequiredJobTypeDef",
     {
         "Role": str,
-        "Settings": JobSettingsOutputTypeDef,
+        "Settings": JobSettingsTypeDef,
     },
 )
 _OptionalJobTypeDef = TypedDict(
     "_OptionalJobTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
         "AccelerationStatus": AccelerationStatusType,
@@ -4127,106 +3497,78 @@
         "Timing": TimingTypeDef,
         "UserMetadata": Dict[str, str],
         "Warnings": List[WarningGroupTypeDef],
     },
     total=False,
 )
 
+
 class JobTypeDef(_RequiredJobTypeDef, _OptionalJobTypeDef):
     pass
 
-_RequiredJobTemplateTypeDef = TypedDict(
-    "_RequiredJobTemplateTypeDef",
+
+_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
-        "Settings": JobTemplateSettingsOutputTypeDef,
+        "Settings": JobTemplateSettingsTypeDef,
     },
 )
-_OptionalJobTemplateTypeDef = TypedDict(
-    "_OptionalJobTemplateTypeDef",
+_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobTemplateRequestRequestTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
-        "Arn": str,
         "Category": str,
-        "CreatedAt": datetime,
         "Description": str,
-        "HopDestinations": List[HopDestinationTypeDef],
-        "LastUpdated": datetime,
-        "Priority": int,
-        "Queue": str,
-        "StatusUpdateInterval": StatusUpdateIntervalType,
-        "Type": TypeType,
-    },
-    total=False,
-)
-
-class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
-    pass
-
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "Role": str,
-        "Settings": JobSettingsTypeDef,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "AccelerationSettings": AccelerationSettingsTypeDef,
-        "BillingTagsSource": BillingTagsSourceType,
-        "ClientRequestToken": str,
         "HopDestinations": Sequence[HopDestinationTypeDef],
-        "JobTemplate": str,
         "Priority": int,
         "Queue": str,
-        "SimulateReservedQueue": SimulateReservedQueueType,
         "StatusUpdateInterval": StatusUpdateIntervalType,
         "Tags": Mapping[str, str],
-        "UserMetadata": Mapping[str, str],
     },
     total=False,
 )
 
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
+
+class CreateJobTemplateRequestRequestTypeDef(
+    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
 ):
     pass
 
-JobSettingsUnionTypeDef = Union[JobSettingsTypeDef, JobSettingsOutputTypeDef]
-_RequiredCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobTemplateRequestRequestTypeDef",
+
+_RequiredJobTemplateTypeDef = TypedDict(
+    "_RequiredJobTemplateTypeDef",
     {
         "Name": str,
         "Settings": JobTemplateSettingsTypeDef,
     },
 )
-_OptionalCreateJobTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobTemplateRequestRequestTypeDef",
+_OptionalJobTemplateTypeDef = TypedDict(
+    "_OptionalJobTemplateTypeDef",
     {
         "AccelerationSettings": AccelerationSettingsTypeDef,
+        "Arn": str,
         "Category": str,
+        "CreatedAt": datetime,
         "Description": str,
-        "HopDestinations": Sequence[HopDestinationTypeDef],
+        "HopDestinations": List[HopDestinationTypeDef],
+        "LastUpdated": datetime,
         "Priority": int,
         "Queue": str,
         "StatusUpdateInterval": StatusUpdateIntervalType,
-        "Tags": Mapping[str, str],
+        "Type": TypeType,
     },
     total=False,
 )
 
-class CreateJobTemplateRequestRequestTypeDef(
-    _RequiredCreateJobTemplateRequestRequestTypeDef, _OptionalCreateJobTemplateRequestRequestTypeDef
-):
+
+class JobTemplateTypeDef(_RequiredJobTemplateTypeDef, _OptionalJobTemplateTypeDef):
     pass
 
-JobTemplateSettingsUnionTypeDef = Union[
-    JobTemplateSettingsTypeDef, JobTemplateSettingsOutputTypeDef
-]
+
 _RequiredUpdateJobTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateJobTemplateRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalUpdateJobTemplateRequestRequestTypeDef = TypedDict(
@@ -4240,19 +3582,21 @@
         "Queue": str,
         "Settings": JobTemplateSettingsTypeDef,
         "StatusUpdateInterval": StatusUpdateIntervalType,
     },
     total=False,
 )
 
+
 class UpdateJobTemplateRequestRequestTypeDef(
     _RequiredUpdateJobTemplateRequestRequestTypeDef, _OptionalUpdateJobTemplateRequestRequestTypeDef
 ):
     pass
 
+
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-mediaconvert-2.5.2.post1/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt` & `types-aiobotocore-mediaconvert-2.5.2.post2/types_aiobotocore_mediaconvert.egg-info/SOURCES.txt`

 * *Files identical despite different names*

