# Comparing `tmp/types-aiobotocore-evidently-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-evidently-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-evidently-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-evidently-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:53 2023, max compression
```

## Comparing `types-aiobotocore-evidently-2.5.2.post1.tar` & `types-aiobotocore-evidently-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:17.153588 types-aiobotocore-evidently-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-08-02 14:52:17.153588 types-aiobotocore-evidently-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17154 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:17.153588 types-aiobotocore-evidently-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:17.153588 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32393 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-08-02 14:38:40.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-08-02 14:38:40.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    45742 2023-08-02 14:38:41.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    45657 2023-08-02 14:38:40.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:38.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:17.153588 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-08-02 14:52:16.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:17.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:16.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:16.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:16.000000 types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.188171 types-aiobotocore-evidently-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:46:08.000000 types-aiobotocore-evidently-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-08-04 12:00:53.184171 types-aiobotocore-evidently-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12262 2023-08-04 11:46:08.000000 types-aiobotocore-evidently-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:53.188171 types-aiobotocore-evidently-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-08-04 11:46:07.000000 types-aiobotocore-evidently-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.180170 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-08-04 11:46:08.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-08-04 11:46:08.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-04 11:46:08.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32446 2023-08-04 11:46:08.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32393 2023-08-04 11:46:08.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-08-04 11:46:08.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10277 2023-08-04 11:46:08.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-08-04 11:46:08.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-08-04 11:46:08.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:46:08.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    45515 2023-08-04 11:46:11.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45430 2023-08-04 11:46:10.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:46:08.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:53.184171 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-08-04 12:00:52.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-04 12:00:53.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:52.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:52.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 12:00:52.000000 types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-evidently-2.5.2.post1/LICENSE` & `types-aiobotocore-evidently-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post1/setup.py` & `types-aiobotocore-evidently-2.5.2.post2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-evidently",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_evidently"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudWatchEvidently 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/__init__.py` & `types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/__init__.pyi` & `types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/__main__.py` & `types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CloudWatchEvidently 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_evidently//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/evidently.html#CloudWatchEvidently\nOther"
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

### Comparing `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/client.py` & `types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/client.pyi` & `types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/literals.py` & `types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/literals.pyi` & `types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/paginator.py` & `types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/paginator.pyi` & `types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/type_defs.py` & `types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,14 @@
     "MetricDefinitionConfigTypeDef",
     "MetricDefinitionTypeDef",
     "ProjectAppConfigResourceTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "PutProjectEventsResultEntryTypeDef",
     "SegmentOverrideTypeDef",
-    "SegmentOverrideOutputTypeDef",
     "StartLaunchRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
     "StopLaunchRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSegmentPatternRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchEvaluateFeatureRequestRequestTypeDef",
@@ -814,23 +813,14 @@
     {
         "evaluationOrder": int,
         "segment": str,
         "weights": Mapping[str, int],
     },
 )
 
-SegmentOverrideOutputTypeDef = TypedDict(
-    "SegmentOverrideOutputTypeDef",
-    {
-        "evaluationOrder": int,
-        "segment": str,
-        "weights": Dict[str, int],
-    },
-)
-
 StartLaunchRequestRequestTypeDef = TypedDict(
     "StartLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -1393,15 +1383,15 @@
         "startTime": datetime,
     },
 )
 _OptionalScheduledSplitTypeDef = TypedDict(
     "_OptionalScheduledSplitTypeDef",
     {
         "groupWeights": Dict[str, int],
-        "segmentOverrides": List[SegmentOverrideOutputTypeDef],
+        "segmentOverrides": List[SegmentOverrideTypeDef],
     },
     total=False,
 )
 
 
 class ScheduledSplitTypeDef(_RequiredScheduledSplitTypeDef, _OptionalScheduledSplitTypeDef):
     pass
```

### Comparing `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently/type_defs.pyi` & `types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
     "MetricDefinitionConfigTypeDef",
     "MetricDefinitionTypeDef",
     "ProjectAppConfigResourceTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "PutProjectEventsResultEntryTypeDef",
     "SegmentOverrideTypeDef",
-    "SegmentOverrideOutputTypeDef",
     "StartLaunchRequestRequestTypeDef",
     "StopExperimentRequestRequestTypeDef",
     "StopLaunchRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TestSegmentPatternRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchEvaluateFeatureRequestRequestTypeDef",
@@ -781,23 +780,14 @@
     {
         "evaluationOrder": int,
         "segment": str,
         "weights": Mapping[str, int],
     },
 )
 
-SegmentOverrideOutputTypeDef = TypedDict(
-    "SegmentOverrideOutputTypeDef",
-    {
-        "evaluationOrder": int,
-        "segment": str,
-        "weights": Dict[str, int],
-    },
-)
-
 StartLaunchRequestRequestTypeDef = TypedDict(
     "StartLaunchRequestRequestTypeDef",
     {
         "launch": str,
         "project": str,
     },
 )
@@ -1332,15 +1322,15 @@
         "startTime": datetime,
     },
 )
 _OptionalScheduledSplitTypeDef = TypedDict(
     "_OptionalScheduledSplitTypeDef",
     {
         "groupWeights": Dict[str, int],
-        "segmentOverrides": List[SegmentOverrideOutputTypeDef],
+        "segmentOverrides": List[SegmentOverrideTypeDef],
     },
     total=False,
 )
 
 class ScheduledSplitTypeDef(_RequiredScheduledSplitTypeDef, _OptionalScheduledSplitTypeDef):
     pass
```

### Comparing `types-aiobotocore-evidently-2.5.2.post1/types_aiobotocore_evidently.egg-info/SOURCES.txt` & `types-aiobotocore-evidently-2.5.2.post2/types_aiobotocore_evidently.egg-info/SOURCES.txt`

 * *Files identical despite different names*

