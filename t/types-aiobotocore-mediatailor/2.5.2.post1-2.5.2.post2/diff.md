# Comparing `tmp/types-aiobotocore-mediatailor-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-mediatailor-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-mediatailor-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:40 2023, max compression
+gzip compressed data, was "types-aiobotocore-mediatailor-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:18 2023, max compression
```

## Comparing `types-aiobotocore-mediatailor-2.5.2.post1.tar` & `types-aiobotocore-mediatailor-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.569521 types-aiobotocore-mediatailor-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:43:28.000000 types-aiobotocore-mediatailor-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19884 2023-08-02 14:52:40.561521 types-aiobotocore-mediatailor-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18350 2023-08-02 14:43:28.000000 types-aiobotocore-mediatailor-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:40.569521 types-aiobotocore-mediatailor-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-02 14:43:27.000000 types-aiobotocore-mediatailor-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.561521 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-08-02 14:43:28.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-08-02 14:43:28.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-02 14:43:28.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35861 2023-08-02 14:43:28.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35800 2023-08-02 14:43:28.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9807 2023-08-02 14:43:30.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-08-02 14:43:28.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10143 2023-08-02 14:43:28.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-08-02 14:43:28.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:43:28.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    54030 2023-08-02 14:43:31.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    53962 2023-08-02 14:43:31.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:43:28.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:40.561521 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19884 2023-08-02 14:52:40.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 14:52:40.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:40.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:40.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:40.000000 types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.296643 types-aiobotocore-mediatailor-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:44:43.000000 types-aiobotocore-mediatailor-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14242 2023-08-04 13:59:18.286643 types-aiobotocore-mediatailor-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12708 2023-08-04 13:44:43.000000 types-aiobotocore-mediatailor-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:18.296643 types-aiobotocore-mediatailor-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2100 2023-08-04 13:44:43.000000 types-aiobotocore-mediatailor-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.286643 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2183 2023-08-04 13:44:43.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2182 2023-08-04 13:44:43.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      959 2023-08-04 13:44:43.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    35826 2023-08-04 13:44:44.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    35765 2023-08-04 13:44:43.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10086 2023-08-04 13:44:44.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10084 2023-08-04 13:44:44.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10143 2023-08-04 13:44:44.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10133 2023-08-04 13:44:44.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:44:43.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    52454 2023-08-04 13:44:45.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    52387 2023-08-04 13:44:45.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:44:43.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:18.286643 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14242 2023-08-04 13:59:18.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      889 2023-08-04 13:59:18.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:18.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:18.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       30 2023-08-04 13:59:18.000000 types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/LICENSE` & `types-aiobotocore-mediatailor-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/setup.py` & `types-aiobotocore-mediatailor-2.5.2.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-mediatailor",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_mediatailor"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MediaTailor 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/__init__.py` & `types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/__init__.pyi` & `types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/__main__.py` & `types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MediaTailor 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.MediaTailor 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor\nOther"
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

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/client.py` & `types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ListPlaybackConfigurationsPaginator,
     ListPrefetchSchedulesPaginator,
     ListSourceLocationsPaginator,
     ListVodSourcesPaginator,
 )
 from .type_defs import (
     AccessConfigurationTypeDef,
-    AdBreakUnionTypeDef,
+    AdBreakTypeDef,
     AvailSuppressionTypeDef,
     BumperTypeDef,
     CdnConfigurationTypeDef,
     ConfigureLogsForChannelResponseTypeDef,
     ConfigureLogsForPlaybackConfigurationResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateLiveSourceResponseTypeDef,
@@ -65,16 +65,16 @@
     ListPlaybackConfigurationsResponseTypeDef,
     ListPrefetchSchedulesResponseTypeDef,
     ListSourceLocationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVodSourcesResponseTypeDef,
     LivePreRollConfigurationTypeDef,
     ManifestProcessingRulesTypeDef,
-    PrefetchConsumptionUnionTypeDef,
-    PrefetchRetrievalUnionTypeDef,
+    PrefetchConsumptionTypeDef,
+    PrefetchRetrievalTypeDef,
     PutPlaybackConfigurationResponseTypeDef,
     RequestOutputItemTypeDef,
     ScheduleConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     SlateSourceTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateLiveSourceResponseTypeDef,
@@ -190,18 +190,18 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_live_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_live_source)
         """
 
     async def create_prefetch_schedule(
         self,
         *,
-        Consumption: PrefetchConsumptionUnionTypeDef,
+        Consumption: PrefetchConsumptionTypeDef,
         Name: str,
         PlaybackConfigurationName: str,
-        Retrieval: PrefetchRetrievalUnionTypeDef,
+        Retrieval: PrefetchRetrievalTypeDef,
         StreamId: str = ...
     ) -> CreatePrefetchScheduleResponseTypeDef:
         """
         Creates a prefetch schedule for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_prefetch_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_prefetch_schedule)
@@ -210,15 +210,15 @@
     async def create_program(
         self,
         *,
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         SourceLocationName: str,
-        AdBreaks: Sequence[AdBreakUnionTypeDef] = ...,
+        AdBreaks: Sequence[AdBreakTypeDef] = ...,
         LiveSourceName: str = ...,
         VodSourceName: str = ...
     ) -> CreateProgramResponseTypeDef:
         """
         Creates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_program)
@@ -619,15 +619,15 @@
 
     async def update_program(
         self,
         *,
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: UpdateProgramScheduleConfigurationTypeDef,
-        AdBreaks: Sequence[AdBreakUnionTypeDef] = ...
+        AdBreaks: Sequence[AdBreakTypeDef] = ...
     ) -> UpdateProgramResponseTypeDef:
         """
         Updates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_program)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#update_program)
         """
```

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/client.pyi` & `types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     ListPlaybackConfigurationsPaginator,
     ListPrefetchSchedulesPaginator,
     ListSourceLocationsPaginator,
     ListVodSourcesPaginator,
 )
 from .type_defs import (
     AccessConfigurationTypeDef,
-    AdBreakUnionTypeDef,
+    AdBreakTypeDef,
     AvailSuppressionTypeDef,
     BumperTypeDef,
     CdnConfigurationTypeDef,
     ConfigureLogsForChannelResponseTypeDef,
     ConfigureLogsForPlaybackConfigurationResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateLiveSourceResponseTypeDef,
@@ -65,16 +65,16 @@
     ListPlaybackConfigurationsResponseTypeDef,
     ListPrefetchSchedulesResponseTypeDef,
     ListSourceLocationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListVodSourcesResponseTypeDef,
     LivePreRollConfigurationTypeDef,
     ManifestProcessingRulesTypeDef,
-    PrefetchConsumptionUnionTypeDef,
-    PrefetchRetrievalUnionTypeDef,
+    PrefetchConsumptionTypeDef,
+    PrefetchRetrievalTypeDef,
     PutPlaybackConfigurationResponseTypeDef,
     RequestOutputItemTypeDef,
     ScheduleConfigurationTypeDef,
     SegmentDeliveryConfigurationTypeDef,
     SlateSourceTypeDef,
     UpdateChannelResponseTypeDef,
     UpdateLiveSourceResponseTypeDef,
@@ -179,18 +179,18 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_live_source)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_live_source)
         """
     async def create_prefetch_schedule(
         self,
         *,
-        Consumption: PrefetchConsumptionUnionTypeDef,
+        Consumption: PrefetchConsumptionTypeDef,
         Name: str,
         PlaybackConfigurationName: str,
-        Retrieval: PrefetchRetrievalUnionTypeDef,
+        Retrieval: PrefetchRetrievalTypeDef,
         StreamId: str = ...
     ) -> CreatePrefetchScheduleResponseTypeDef:
         """
         Creates a prefetch schedule for a playback configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_prefetch_schedule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#create_prefetch_schedule)
@@ -198,15 +198,15 @@
     async def create_program(
         self,
         *,
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         SourceLocationName: str,
-        AdBreaks: Sequence[AdBreakUnionTypeDef] = ...,
+        AdBreaks: Sequence[AdBreakTypeDef] = ...,
         LiveSourceName: str = ...,
         VodSourceName: str = ...
     ) -> CreateProgramResponseTypeDef:
         """
         Creates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.create_program)
@@ -570,15 +570,15 @@
         """
     async def update_program(
         self,
         *,
         ChannelName: str,
         ProgramName: str,
         ScheduleConfiguration: UpdateProgramScheduleConfigurationTypeDef,
-        AdBreaks: Sequence[AdBreakUnionTypeDef] = ...
+        AdBreaks: Sequence[AdBreakTypeDef] = ...
     ) -> UpdateProgramResponseTypeDef:
         """
         Updates a program within a channel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mediatailor.html#MediaTailor.Client.update_program)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_mediatailor/client/#update_program)
         """
```

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/literals.py` & `types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 __all__ = (
     "AccessTypeType",
+    "AdMarkupTypeType",
+    "AlertCategoryType",
     "ChannelStateType",
     "FillPolicyType",
     "GetChannelSchedulePaginatorName",
     "ListAlertsPaginatorName",
     "ListChannelsPaginatorName",
     "ListLiveSourcesPaginatorName",
     "ListPlaybackConfigurationsPaginatorName",
@@ -46,14 +48,16 @@
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 
 AccessTypeType = Literal["S3_SIGV4", "SECRETS_MANAGER_ACCESS_TOKEN"]
+AdMarkupTypeType = Literal["DATERANGE", "SCTE35_ENHANCED"]
+AlertCategoryType = Literal["INFO", "PLAYBACK_WARNING", "SCHEDULING_ERROR"]
 ChannelStateType = Literal["RUNNING", "STOPPED"]
 FillPolicyType = Literal["FULL_AVAIL_ONLY", "PARTIAL_AVAIL"]
 GetChannelSchedulePaginatorName = Literal["get_channel_schedule"]
 ListAlertsPaginatorName = Literal["list_alerts"]
 ListChannelsPaginatorName = Literal["list_channels"]
 ListLiveSourcesPaginatorName = Literal["list_live_sources"]
 ListPlaybackConfigurationsPaginatorName = Literal["list_playback_configurations"]
@@ -82,14 +86,15 @@
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
@@ -185,14 +190,15 @@
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
@@ -271,26 +277,28 @@
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

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/literals.pyi` & `types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = (
     "AccessTypeType",
+    "AdMarkupTypeType",
+    "AlertCategoryType",
     "ChannelStateType",
     "FillPolicyType",
     "GetChannelSchedulePaginatorName",
     "ListAlertsPaginatorName",
     "ListChannelsPaginatorName",
     "ListLiveSourcesPaginatorName",
     "ListPlaybackConfigurationsPaginatorName",
@@ -44,14 +46,16 @@
     "ServiceName",
     "ResourceServiceName",
     "PaginatorName",
     "RegionName",
 )
 
 AccessTypeType = Literal["S3_SIGV4", "SECRETS_MANAGER_ACCESS_TOKEN"]
+AdMarkupTypeType = Literal["DATERANGE", "SCTE35_ENHANCED"]
+AlertCategoryType = Literal["INFO", "PLAYBACK_WARNING", "SCHEDULING_ERROR"]
 ChannelStateType = Literal["RUNNING", "STOPPED"]
 FillPolicyType = Literal["FULL_AVAIL_ONLY", "PARTIAL_AVAIL"]
 GetChannelSchedulePaginatorName = Literal["get_channel_schedule"]
 ListAlertsPaginatorName = Literal["list_alerts"]
 ListChannelsPaginatorName = Literal["list_channels"]
 ListLiveSourcesPaginatorName = Literal["list_live_sources"]
 ListPlaybackConfigurationsPaginatorName = Literal["list_playback_configurations"]
@@ -80,14 +84,15 @@
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
@@ -183,14 +188,15 @@
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
@@ -269,26 +275,28 @@
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

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/paginator.py` & `types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/paginator.pyi` & `types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/type_defs.py` & `types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessTypeType,
+    AdMarkupTypeType,
+    AlertCategoryType,
     ChannelStateType,
     FillPolicyType,
     MessageTypeType,
     ModeType,
     OriginManifestTypeType,
     PlaybackModeType,
     RelativePositionType,
@@ -34,32 +36,31 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "SecretsManagerAccessTokenConfigurationTypeDef",
+    "KeyValuePairTypeDef",
     "SlateSourceTypeDef",
     "SpliceInsertMessageTypeDef",
     "AdMarkerPassthroughTypeDef",
     "AlertTypeDef",
     "AvailMatchingCriteriaTypeDef",
     "AvailSuppressionTypeDef",
     "BumperTypeDef",
     "CdnConfigurationTypeDef",
     "LogConfigurationForChannelTypeDef",
     "ClipRangeTypeDef",
     "ConfigureLogsForChannelRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
     "HttpPackageConfigurationTypeDef",
-    "PrefetchRetrievalOutputTypeDef",
     "DefaultSegmentDeliveryConfigurationTypeDef",
     "HttpConfigurationTypeDef",
     "SegmentDeliveryConfigurationTypeDef",
     "DashConfigurationForPutTypeDef",
     "DashConfigurationTypeDef",
     "DashPlaylistSettingsTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
@@ -100,15 +101,14 @@
     "StartChannelRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProgramTransitionTypeDef",
     "AccessConfigurationTypeDef",
     "ManifestProcessingRulesTypeDef",
-    "PrefetchConsumptionOutputTypeDef",
     "ConfigureLogsForChannelResponseTypeDef",
     "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChannelPolicyResponseTypeDef",
     "ListAlertsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "CreateLiveSourceRequestRequestTypeDef",
@@ -133,66 +133,69 @@
     "ListVodSourcesRequestListVodSourcesPaginateTypeDef",
     "RequestOutputItemTypeDef",
     "ResponseOutputItemTypeDef",
     "PrefetchConsumptionTypeDef",
     "PrefetchRetrievalTypeDef",
     "ScheduleEntryTypeDef",
     "ScheduleConfigurationTypeDef",
-    "TimeSignalMessageOutputTypeDef",
     "TimeSignalMessageTypeDef",
     "UpdateProgramScheduleConfigurationTypeDef",
     "CreateSourceLocationRequestRequestTypeDef",
     "CreateSourceLocationResponseTypeDef",
     "DescribeSourceLocationResponseTypeDef",
     "SourceLocationTypeDef",
     "UpdateSourceLocationRequestRequestTypeDef",
     "UpdateSourceLocationResponseTypeDef",
     "GetPlaybackConfigurationResponseTypeDef",
     "PlaybackConfigurationTypeDef",
     "PutPlaybackConfigurationRequestRequestTypeDef",
     "PutPlaybackConfigurationResponseTypeDef",
-    "CreatePrefetchScheduleResponseTypeDef",
-    "GetPrefetchScheduleResponseTypeDef",
-    "PrefetchScheduleTypeDef",
     "ListLiveSourcesResponseTypeDef",
     "ListVodSourcesResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "ChannelTypeDef",
     "CreateChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "UpdateChannelResponseTypeDef",
-    "PrefetchConsumptionUnionTypeDef",
     "CreatePrefetchScheduleRequestRequestTypeDef",
-    "PrefetchRetrievalUnionTypeDef",
+    "CreatePrefetchScheduleResponseTypeDef",
+    "GetPrefetchScheduleResponseTypeDef",
+    "PrefetchScheduleTypeDef",
     "GetChannelScheduleResponseTypeDef",
-    "AdBreakOutputTypeDef",
     "AdBreakTypeDef",
     "ListSourceLocationsResponseTypeDef",
     "ListPlaybackConfigurationsResponseTypeDef",
-    "ListPrefetchSchedulesResponseTypeDef",
     "ListChannelsResponseTypeDef",
+    "ListPrefetchSchedulesResponseTypeDef",
+    "CreateProgramRequestRequestTypeDef",
     "CreateProgramResponseTypeDef",
     "DescribeProgramResponseTypeDef",
-    "UpdateProgramResponseTypeDef",
-    "AdBreakUnionTypeDef",
-    "CreateProgramRequestRequestTypeDef",
     "UpdateProgramRequestRequestTypeDef",
+    "UpdateProgramResponseTypeDef",
 )
 
 SecretsManagerAccessTokenConfigurationTypeDef = TypedDict(
     "SecretsManagerAccessTokenConfigurationTypeDef",
     {
         "HeaderName": str,
         "SecretArn": str,
         "SecretStringKey": str,
     },
     total=False,
 )
 
+KeyValuePairTypeDef = TypedDict(
+    "KeyValuePairTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 SlateSourceTypeDef = TypedDict(
     "SlateSourceTypeDef",
     {
         "SourceLocationName": str,
         "VodSourceName": str,
     },
     total=False,
@@ -213,24 +216,34 @@
     "AdMarkerPassthroughTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-AlertTypeDef = TypedDict(
-    "AlertTypeDef",
+_RequiredAlertTypeDef = TypedDict(
+    "_RequiredAlertTypeDef",
     {
         "AlertCode": str,
         "AlertMessage": str,
         "LastModifiedTime": datetime,
         "RelatedResourceArns": List[str],
         "ResourceArn": str,
     },
 )
+_OptionalAlertTypeDef = TypedDict(
+    "_OptionalAlertTypeDef",
+    {
+        "Category": AlertCategoryType,
+    },
+    total=False,
+)
+
+class AlertTypeDef(_RequiredAlertTypeDef, _OptionalAlertTypeDef):
+    pass
 
 AvailMatchingCriteriaTypeDef = TypedDict(
     "AvailMatchingCriteriaTypeDef",
     {
         "DynamicVariable": str,
         "Operator": Literal["EQUALS"],
     },
@@ -311,36 +324,14 @@
     {
         "Path": str,
         "SourceGroup": str,
         "Type": TypeType,
     },
 )
 
-_RequiredPrefetchRetrievalOutputTypeDef = TypedDict(
-    "_RequiredPrefetchRetrievalOutputTypeDef",
-    {
-        "EndTime": datetime,
-    },
-)
-_OptionalPrefetchRetrievalOutputTypeDef = TypedDict(
-    "_OptionalPrefetchRetrievalOutputTypeDef",
-    {
-        "DynamicVariables": Dict[str, str],
-        "StartTime": datetime,
-    },
-    total=False,
-)
-
-
-class PrefetchRetrievalOutputTypeDef(
-    _RequiredPrefetchRetrievalOutputTypeDef, _OptionalPrefetchRetrievalOutputTypeDef
-):
-    pass
-
-
 DefaultSegmentDeliveryConfigurationTypeDef = TypedDict(
     "DefaultSegmentDeliveryConfigurationTypeDef",
     {
         "BaseUrl": str,
     },
     total=False,
 )
@@ -518,22 +509,20 @@
         "DurationMinutes": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetChannelScheduleRequestRequestTypeDef(
     _RequiredGetChannelScheduleRequestRequestTypeDef,
     _OptionalGetChannelScheduleRequestRequestTypeDef,
 ):
     pass
 
-
 GetPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "GetPlaybackConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -568,14 +557,15 @@
         "PlaybackConfigurationName": str,
     },
 )
 
 HlsPlaylistSettingsTypeDef = TypedDict(
     "HlsPlaylistSettingsTypeDef",
     {
+        "AdMarkupType": Sequence[AdMarkupTypeType],
         "ManifestWindowSeconds": int,
     },
     total=False,
 )
 
 _RequiredListAlertsRequestRequestTypeDef = TypedDict(
     "_RequiredListAlertsRequestRequestTypeDef",
@@ -588,21 +578,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAlertsRequestRequestTypeDef(
     _RequiredListAlertsRequestRequestTypeDef, _OptionalListAlertsRequestRequestTypeDef
 ):
     pass
 
-
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -619,21 +607,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListLiveSourcesRequestRequestTypeDef(
     _RequiredListLiveSourcesRequestRequestTypeDef, _OptionalListLiveSourcesRequestRequestTypeDef
 ):
     pass
 
-
 ListPlaybackConfigurationsRequestRequestTypeDef = TypedDict(
     "ListPlaybackConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -651,22 +637,20 @@
         "MaxResults": int,
         "NextToken": str,
         "StreamId": str,
     },
     total=False,
 )
 
-
 class ListPrefetchSchedulesRequestRequestTypeDef(
     _RequiredListPrefetchSchedulesRequestRequestTypeDef,
     _OptionalListPrefetchSchedulesRequestRequestTypeDef,
 ):
     pass
 
-
 ListSourceLocationsRequestRequestTypeDef = TypedDict(
     "ListSourceLocationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -690,21 +674,19 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListVodSourcesRequestRequestTypeDef(
     _RequiredListVodSourcesRequestRequestTypeDef, _OptionalListVodSourcesRequestRequestTypeDef
 ):
     pass
 
-
 TimestampTypeDef = Union[datetime, str]
 PutChannelPolicyRequestRequestTypeDef = TypedDict(
     "PutChannelPolicyRequestRequestTypeDef",
     {
         "ChannelName": str,
         "Policy": str,
     },
@@ -734,19 +716,17 @@
         "DurationMillis": int,
         "RelativeProgram": str,
         "ScheduledStartTimeMillis": int,
     },
     total=False,
 )
 
-
 class TransitionTypeDef(_RequiredTransitionTypeDef, _OptionalTransitionTypeDef):
     pass
 
-
 SegmentationDescriptorTypeDef = TypedDict(
     "SegmentationDescriptorTypeDef",
     {
         "SegmentNum": int,
         "SegmentationEventId": int,
         "SegmentationTypeId": int,
         "SegmentationUpid": str,
@@ -810,36 +790,14 @@
     "ManifestProcessingRulesTypeDef",
     {
         "AdMarkerPassthrough": AdMarkerPassthroughTypeDef,
     },
     total=False,
 )
 
-_RequiredPrefetchConsumptionOutputTypeDef = TypedDict(
-    "_RequiredPrefetchConsumptionOutputTypeDef",
-    {
-        "EndTime": datetime,
-    },
-)
-_OptionalPrefetchConsumptionOutputTypeDef = TypedDict(
-    "_OptionalPrefetchConsumptionOutputTypeDef",
-    {
-        "AvailMatchingCriteria": List[AvailMatchingCriteriaTypeDef],
-        "StartTime": datetime,
-    },
-    total=False,
-)
-
-
-class PrefetchConsumptionOutputTypeDef(
-    _RequiredPrefetchConsumptionOutputTypeDef, _OptionalPrefetchConsumptionOutputTypeDef
-):
-    pass
-
-
 ConfigureLogsForChannelResponseTypeDef = TypedDict(
     "ConfigureLogsForChannelResponseTypeDef",
     {
         "ChannelName": str,
         "LogTypes": List[Literal["AS_RUN"]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -898,21 +856,19 @@
     "_OptionalCreateLiveSourceRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateLiveSourceRequestRequestTypeDef(
     _RequiredCreateLiveSourceRequestRequestTypeDef, _OptionalCreateLiveSourceRequestRequestTypeDef
 ):
     pass
 
-
 CreateLiveSourceResponseTypeDef = TypedDict(
     "CreateLiveSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
@@ -935,21 +891,19 @@
     "_OptionalCreateVodSourceRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateVodSourceRequestRequestTypeDef(
     _RequiredCreateVodSourceRequestRequestTypeDef, _OptionalCreateVodSourceRequestRequestTypeDef
 ):
     pass
 
-
 CreateVodSourceResponseTypeDef = TypedDict(
     "CreateVodSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
@@ -1003,19 +957,17 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class LiveSourceTypeDef(_RequiredLiveSourceTypeDef, _OptionalLiveSourceTypeDef):
     pass
 
-
 UpdateLiveSourceRequestRequestTypeDef = TypedDict(
     "UpdateLiveSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "LiveSourceName": str,
         "SourceLocationName": str,
     },
@@ -1073,19 +1025,17 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class VodSourceTypeDef(_RequiredVodSourceTypeDef, _OptionalVodSourceTypeDef):
     pass
 
-
 _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
     "_RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
     {
         "ChannelName": str,
     },
 )
 _OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
@@ -1093,44 +1043,40 @@
     {
         "DurationMinutes": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef(
     _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
     _OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
 ):
     pass
 
-
 _RequiredListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
     "_RequiredListAlertsRequestListAlertsPaginateTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
     "_OptionalListAlertsRequestListAlertsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListAlertsRequestListAlertsPaginateTypeDef(
     _RequiredListAlertsRequestListAlertsPaginateTypeDef,
     _OptionalListAlertsRequestListAlertsPaginateTypeDef,
 ):
     pass
 
-
 ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
     "ListChannelsRequestListChannelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1145,22 +1091,20 @@
     "_OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListLiveSourcesRequestListLiveSourcesPaginateTypeDef(
     _RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
     _OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
 ):
     pass
 
-
 ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef = TypedDict(
     "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1176,22 +1120,20 @@
     {
         "StreamId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef(
     _RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
     _OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
 ):
     pass
 
-
 ListSourceLocationsRequestListSourceLocationsPaginateTypeDef = TypedDict(
     "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1206,22 +1148,20 @@
     "_OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListVodSourcesRequestListVodSourcesPaginateTypeDef(
     _RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef,
     _OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredRequestOutputItemTypeDef = TypedDict(
     "_RequiredRequestOutputItemTypeDef",
     {
         "ManifestName": str,
         "SourceGroup": str,
     },
 )
@@ -1230,21 +1170,19 @@
     {
         "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
         "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
     },
     total=False,
 )
 
-
 class RequestOutputItemTypeDef(
     _RequiredRequestOutputItemTypeDef, _OptionalRequestOutputItemTypeDef
 ):
     pass
 
-
 _RequiredResponseOutputItemTypeDef = TypedDict(
     "_RequiredResponseOutputItemTypeDef",
     {
         "ManifestName": str,
         "PlaybackUrl": str,
         "SourceGroup": str,
     },
@@ -1254,21 +1192,19 @@
     {
         "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
         "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
     },
     total=False,
 )
 
-
 class ResponseOutputItemTypeDef(
     _RequiredResponseOutputItemTypeDef, _OptionalResponseOutputItemTypeDef
 ):
     pass
 
-
 _RequiredPrefetchConsumptionTypeDef = TypedDict(
     "_RequiredPrefetchConsumptionTypeDef",
     {
         "EndTime": TimestampTypeDef,
     },
 )
 _OptionalPrefetchConsumptionTypeDef = TypedDict(
@@ -1276,21 +1212,19 @@
     {
         "AvailMatchingCriteria": Sequence[AvailMatchingCriteriaTypeDef],
         "StartTime": TimestampTypeDef,
     },
     total=False,
 )
 
-
 class PrefetchConsumptionTypeDef(
     _RequiredPrefetchConsumptionTypeDef, _OptionalPrefetchConsumptionTypeDef
 ):
     pass
 
-
 _RequiredPrefetchRetrievalTypeDef = TypedDict(
     "_RequiredPrefetchRetrievalTypeDef",
     {
         "EndTime": TimestampTypeDef,
     },
 )
 _OptionalPrefetchRetrievalTypeDef = TypedDict(
@@ -1298,21 +1232,19 @@
     {
         "DynamicVariables": Mapping[str, str],
         "StartTime": TimestampTypeDef,
     },
     total=False,
 )
 
-
 class PrefetchRetrievalTypeDef(
     _RequiredPrefetchRetrievalTypeDef, _OptionalPrefetchRetrievalTypeDef
 ):
     pass
 
-
 _RequiredScheduleEntryTypeDef = TypedDict(
     "_RequiredScheduleEntryTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ProgramName": str,
         "SourceLocationName": str,
@@ -1327,48 +1259,36 @@
         "ScheduleAdBreaks": List[ScheduleAdBreakTypeDef],
         "ScheduleEntryType": ScheduleEntryTypeType,
         "VodSourceName": str,
     },
     total=False,
 )
 
-
 class ScheduleEntryTypeDef(_RequiredScheduleEntryTypeDef, _OptionalScheduleEntryTypeDef):
     pass
 
-
 _RequiredScheduleConfigurationTypeDef = TypedDict(
     "_RequiredScheduleConfigurationTypeDef",
     {
         "Transition": TransitionTypeDef,
     },
 )
 _OptionalScheduleConfigurationTypeDef = TypedDict(
     "_OptionalScheduleConfigurationTypeDef",
     {
         "ClipRange": ClipRangeTypeDef,
     },
     total=False,
 )
 
-
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
-
-TimeSignalMessageOutputTypeDef = TypedDict(
-    "TimeSignalMessageOutputTypeDef",
-    {
-        "SegmentationDescriptors": List[SegmentationDescriptorTypeDef],
-    },
-    total=False,
-)
-
 TimeSignalMessageTypeDef = TypedDict(
     "TimeSignalMessageTypeDef",
     {
         "SegmentationDescriptors": Sequence[SegmentationDescriptorTypeDef],
     },
     total=False,
 )
@@ -1396,22 +1316,20 @@
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "SegmentDeliveryConfigurations": Sequence[SegmentDeliveryConfigurationTypeDef],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateSourceLocationRequestRequestTypeDef(
     _RequiredCreateSourceLocationRequestRequestTypeDef,
     _OptionalCreateSourceLocationRequestRequestTypeDef,
 ):
     pass
 
-
 CreateSourceLocationResponseTypeDef = TypedDict(
     "CreateSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
@@ -1457,19 +1375,17 @@
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class SourceLocationTypeDef(_RequiredSourceLocationTypeDef, _OptionalSourceLocationTypeDef):
     pass
 
-
 _RequiredUpdateSourceLocationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSourceLocationRequestRequestTypeDef",
     {
         "HttpConfiguration": HttpConfigurationTypeDef,
         "SourceLocationName": str,
     },
 )
@@ -1479,22 +1395,20 @@
         "AccessConfiguration": AccessConfigurationTypeDef,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "SegmentDeliveryConfigurations": Sequence[SegmentDeliveryConfigurationTypeDef],
     },
     total=False,
 )
 
-
 class UpdateSourceLocationRequestRequestTypeDef(
     _RequiredUpdateSourceLocationRequestRequestTypeDef,
     _OptionalUpdateSourceLocationRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateSourceLocationResponseTypeDef = TypedDict(
     "UpdateSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
@@ -1581,22 +1495,20 @@
         "Tags": Mapping[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
     },
     total=False,
 )
 
-
 class PutPlaybackConfigurationRequestRequestTypeDef(
     _RequiredPutPlaybackConfigurationRequestRequestTypeDef,
     _OptionalPutPlaybackConfigurationRequestRequestTypeDef,
 ):
     pass
 
-
 PutPlaybackConfigurationResponseTypeDef = TypedDict(
     "PutPlaybackConfigurationResponseTypeDef",
     {
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionTypeDef,
         "Bumper": BumperTypeDef,
         "CdnConfiguration": CdnConfigurationTypeDef,
@@ -1615,63 +1527,14 @@
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreatePrefetchScheduleResponseTypeDef = TypedDict(
-    "CreatePrefetchScheduleResponseTypeDef",
-    {
-        "Arn": str,
-        "Consumption": PrefetchConsumptionOutputTypeDef,
-        "Name": str,
-        "PlaybackConfigurationName": str,
-        "Retrieval": PrefetchRetrievalOutputTypeDef,
-        "StreamId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPrefetchScheduleResponseTypeDef = TypedDict(
-    "GetPrefetchScheduleResponseTypeDef",
-    {
-        "Arn": str,
-        "Consumption": PrefetchConsumptionOutputTypeDef,
-        "Name": str,
-        "PlaybackConfigurationName": str,
-        "Retrieval": PrefetchRetrievalOutputTypeDef,
-        "StreamId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredPrefetchScheduleTypeDef = TypedDict(
-    "_RequiredPrefetchScheduleTypeDef",
-    {
-        "Arn": str,
-        "Consumption": PrefetchConsumptionOutputTypeDef,
-        "Name": str,
-        "PlaybackConfigurationName": str,
-        "Retrieval": PrefetchRetrievalOutputTypeDef,
-    },
-)
-_OptionalPrefetchScheduleTypeDef = TypedDict(
-    "_OptionalPrefetchScheduleTypeDef",
-    {
-        "StreamId": str,
-    },
-    total=False,
-)
-
-
-class PrefetchScheduleTypeDef(_RequiredPrefetchScheduleTypeDef, _OptionalPrefetchScheduleTypeDef):
-    pass
-
-
 ListLiveSourcesResponseTypeDef = TypedDict(
     "ListLiveSourcesResponseTypeDef",
     {
         "Items": List[LiveSourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1700,21 +1563,19 @@
         "FillerSlate": SlateSourceTypeDef,
         "Tags": Mapping[str, str],
         "Tier": TierType,
     },
     total=False,
 )
 
-
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
         "Outputs": Sequence[RequestOutputItemTypeDef],
     },
 )
@@ -1722,21 +1583,19 @@
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "FillerSlate": SlateSourceTypeDef,
     },
     total=False,
 )
 
-
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredChannelTypeDef = TypedDict(
     "_RequiredChannelTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": str,
         "LogConfiguration": LogConfigurationForChannelTypeDef,
@@ -1752,19 +1611,17 @@
         "FillerSlate": SlateSourceTypeDef,
         "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
     pass
 
-
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": ChannelStateType,
         "CreationTime": datetime,
@@ -1809,17 +1666,14 @@
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PrefetchConsumptionUnionTypeDef = Union[
-    PrefetchConsumptionTypeDef, PrefetchConsumptionOutputTypeDef
-]
 _RequiredCreatePrefetchScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePrefetchScheduleRequestRequestTypeDef",
     {
         "Consumption": PrefetchConsumptionTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalTypeDef,
@@ -1829,47 +1683,80 @@
     "_OptionalCreatePrefetchScheduleRequestRequestTypeDef",
     {
         "StreamId": str,
     },
     total=False,
 )
 
-
 class CreatePrefetchScheduleRequestRequestTypeDef(
     _RequiredCreatePrefetchScheduleRequestRequestTypeDef,
     _OptionalCreatePrefetchScheduleRequestRequestTypeDef,
 ):
     pass
 
+CreatePrefetchScheduleResponseTypeDef = TypedDict(
+    "CreatePrefetchScheduleResponseTypeDef",
+    {
+        "Arn": str,
+        "Consumption": PrefetchConsumptionTypeDef,
+        "Name": str,
+        "PlaybackConfigurationName": str,
+        "Retrieval": PrefetchRetrievalTypeDef,
+        "StreamId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-PrefetchRetrievalUnionTypeDef = Union[PrefetchRetrievalTypeDef, PrefetchRetrievalOutputTypeDef]
-GetChannelScheduleResponseTypeDef = TypedDict(
-    "GetChannelScheduleResponseTypeDef",
+GetPrefetchScheduleResponseTypeDef = TypedDict(
+    "GetPrefetchScheduleResponseTypeDef",
     {
-        "Items": List[ScheduleEntryTypeDef],
-        "NextToken": str,
+        "Arn": str,
+        "Consumption": PrefetchConsumptionTypeDef,
+        "Name": str,
+        "PlaybackConfigurationName": str,
+        "Retrieval": PrefetchRetrievalTypeDef,
+        "StreamId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdBreakOutputTypeDef = TypedDict(
-    "AdBreakOutputTypeDef",
+_RequiredPrefetchScheduleTypeDef = TypedDict(
+    "_RequiredPrefetchScheduleTypeDef",
     {
-        "MessageType": MessageTypeType,
-        "OffsetMillis": int,
-        "Slate": SlateSourceTypeDef,
-        "SpliceInsertMessage": SpliceInsertMessageTypeDef,
-        "TimeSignalMessage": TimeSignalMessageOutputTypeDef,
+        "Arn": str,
+        "Consumption": PrefetchConsumptionTypeDef,
+        "Name": str,
+        "PlaybackConfigurationName": str,
+        "Retrieval": PrefetchRetrievalTypeDef,
+    },
+)
+_OptionalPrefetchScheduleTypeDef = TypedDict(
+    "_OptionalPrefetchScheduleTypeDef",
+    {
+        "StreamId": str,
     },
     total=False,
 )
 
+class PrefetchScheduleTypeDef(_RequiredPrefetchScheduleTypeDef, _OptionalPrefetchScheduleTypeDef):
+    pass
+
+GetChannelScheduleResponseTypeDef = TypedDict(
+    "GetChannelScheduleResponseTypeDef",
+    {
+        "Items": List[ScheduleEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AdBreakTypeDef = TypedDict(
     "AdBreakTypeDef",
     {
+        "AdBreakMetadata": Sequence[KeyValuePairTypeDef],
         "MessageType": MessageTypeType,
         "OffsetMillis": int,
         "Slate": SlateSourceTypeDef,
         "SpliceInsertMessage": SpliceInsertMessageTypeDef,
         "TimeSignalMessage": TimeSignalMessageTypeDef,
     },
     total=False,
@@ -1889,127 +1776,123 @@
     {
         "Items": List[PlaybackConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListPrefetchSchedulesResponseTypeDef = TypedDict(
-    "ListPrefetchSchedulesResponseTypeDef",
+ListChannelsResponseTypeDef = TypedDict(
+    "ListChannelsResponseTypeDef",
     {
-        "Items": List[PrefetchScheduleTypeDef],
+        "Items": List[ChannelTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListChannelsResponseTypeDef = TypedDict(
-    "ListChannelsResponseTypeDef",
+ListPrefetchSchedulesResponseTypeDef = TypedDict(
+    "ListPrefetchSchedulesResponseTypeDef",
     {
-        "Items": List[ChannelTypeDef],
+        "Items": List[PrefetchScheduleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateProgramResponseTypeDef = TypedDict(
-    "CreateProgramResponseTypeDef",
+_RequiredCreateProgramRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProgramRequestRequestTypeDef",
     {
-        "AdBreaks": List[AdBreakOutputTypeDef],
-        "Arn": str,
         "ChannelName": str,
-        "ClipRange": ClipRangeTypeDef,
-        "CreationTime": datetime,
-        "DurationMillis": int,
-        "LiveSourceName": str,
         "ProgramName": str,
-        "ScheduledStartTime": datetime,
+        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "SourceLocationName": str,
+    },
+)
+_OptionalCreateProgramRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProgramRequestRequestTypeDef",
+    {
+        "AdBreaks": Sequence[AdBreakTypeDef],
+        "LiveSourceName": str,
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-DescribeProgramResponseTypeDef = TypedDict(
-    "DescribeProgramResponseTypeDef",
+class CreateProgramRequestRequestTypeDef(
+    _RequiredCreateProgramRequestRequestTypeDef, _OptionalCreateProgramRequestRequestTypeDef
+):
+    pass
+
+CreateProgramResponseTypeDef = TypedDict(
+    "CreateProgramResponseTypeDef",
     {
-        "AdBreaks": List[AdBreakOutputTypeDef],
+        "AdBreaks": List[AdBreakTypeDef],
         "Arn": str,
         "ChannelName": str,
         "ClipRange": ClipRangeTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateProgramResponseTypeDef = TypedDict(
-    "UpdateProgramResponseTypeDef",
+DescribeProgramResponseTypeDef = TypedDict(
+    "DescribeProgramResponseTypeDef",
     {
-        "AdBreaks": List[AdBreakOutputTypeDef],
+        "AdBreaks": List[AdBreakTypeDef],
         "Arn": str,
         "ChannelName": str,
         "ClipRange": ClipRangeTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdBreakUnionTypeDef = Union[AdBreakTypeDef, AdBreakOutputTypeDef]
-_RequiredCreateProgramRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProgramRequestRequestTypeDef",
-    {
-        "ChannelName": str,
-        "ProgramName": str,
-        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
-        "SourceLocationName": str,
-    },
-)
-_OptionalCreateProgramRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProgramRequestRequestTypeDef",
-    {
-        "AdBreaks": Sequence[AdBreakUnionTypeDef],
-        "LiveSourceName": str,
-        "VodSourceName": str,
-    },
-    total=False,
-)
-
-
-class CreateProgramRequestRequestTypeDef(
-    _RequiredCreateProgramRequestRequestTypeDef, _OptionalCreateProgramRequestRequestTypeDef
-):
-    pass
-
-
 _RequiredUpdateProgramRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProgramRequestRequestTypeDef",
     {
         "ChannelName": str,
         "ProgramName": str,
         "ScheduleConfiguration": UpdateProgramScheduleConfigurationTypeDef,
     },
 )
 _OptionalUpdateProgramRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateProgramRequestRequestTypeDef",
     {
-        "AdBreaks": Sequence[AdBreakUnionTypeDef],
+        "AdBreaks": Sequence[AdBreakTypeDef],
     },
     total=False,
 )
 
-
 class UpdateProgramRequestRequestTypeDef(
     _RequiredUpdateProgramRequestRequestTypeDef, _OptionalUpdateProgramRequestRequestTypeDef
 ):
     pass
+
+UpdateProgramResponseTypeDef = TypedDict(
+    "UpdateProgramResponseTypeDef",
+    {
+        "AdBreaks": List[AdBreakTypeDef],
+        "Arn": str,
+        "ChannelName": str,
+        "ClipRange": ClipRangeTypeDef,
+        "CreationTime": datetime,
+        "DurationMillis": int,
+        "LiveSourceName": str,
+        "ProgramName": str,
+        "ScheduledStartTime": datetime,
+        "SourceLocationName": str,
+        "VodSourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor/type_defs.pyi` & `types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccessTypeType,
+    AdMarkupTypeType,
+    AlertCategoryType,
     ChannelStateType,
     FillPolicyType,
     MessageTypeType,
     ModeType,
     OriginManifestTypeType,
     PlaybackModeType,
     RelativePositionType,
@@ -34,31 +36,32 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "SecretsManagerAccessTokenConfigurationTypeDef",
+    "KeyValuePairTypeDef",
     "SlateSourceTypeDef",
     "SpliceInsertMessageTypeDef",
     "AdMarkerPassthroughTypeDef",
     "AlertTypeDef",
     "AvailMatchingCriteriaTypeDef",
     "AvailSuppressionTypeDef",
     "BumperTypeDef",
     "CdnConfigurationTypeDef",
     "LogConfigurationForChannelTypeDef",
     "ClipRangeTypeDef",
     "ConfigureLogsForChannelRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ConfigureLogsForPlaybackConfigurationRequestRequestTypeDef",
     "HttpPackageConfigurationTypeDef",
-    "PrefetchRetrievalOutputTypeDef",
     "DefaultSegmentDeliveryConfigurationTypeDef",
     "HttpConfigurationTypeDef",
     "SegmentDeliveryConfigurationTypeDef",
     "DashConfigurationForPutTypeDef",
     "DashConfigurationTypeDef",
     "DashPlaylistSettingsTypeDef",
     "DeleteChannelPolicyRequestRequestTypeDef",
@@ -99,15 +102,14 @@
     "StartChannelRequestRequestTypeDef",
     "StopChannelRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateProgramTransitionTypeDef",
     "AccessConfigurationTypeDef",
     "ManifestProcessingRulesTypeDef",
-    "PrefetchConsumptionOutputTypeDef",
     "ConfigureLogsForChannelResponseTypeDef",
     "ConfigureLogsForPlaybackConfigurationResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetChannelPolicyResponseTypeDef",
     "ListAlertsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "CreateLiveSourceRequestRequestTypeDef",
@@ -132,66 +134,69 @@
     "ListVodSourcesRequestListVodSourcesPaginateTypeDef",
     "RequestOutputItemTypeDef",
     "ResponseOutputItemTypeDef",
     "PrefetchConsumptionTypeDef",
     "PrefetchRetrievalTypeDef",
     "ScheduleEntryTypeDef",
     "ScheduleConfigurationTypeDef",
-    "TimeSignalMessageOutputTypeDef",
     "TimeSignalMessageTypeDef",
     "UpdateProgramScheduleConfigurationTypeDef",
     "CreateSourceLocationRequestRequestTypeDef",
     "CreateSourceLocationResponseTypeDef",
     "DescribeSourceLocationResponseTypeDef",
     "SourceLocationTypeDef",
     "UpdateSourceLocationRequestRequestTypeDef",
     "UpdateSourceLocationResponseTypeDef",
     "GetPlaybackConfigurationResponseTypeDef",
     "PlaybackConfigurationTypeDef",
     "PutPlaybackConfigurationRequestRequestTypeDef",
     "PutPlaybackConfigurationResponseTypeDef",
-    "CreatePrefetchScheduleResponseTypeDef",
-    "GetPrefetchScheduleResponseTypeDef",
-    "PrefetchScheduleTypeDef",
     "ListLiveSourcesResponseTypeDef",
     "ListVodSourcesResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "ChannelTypeDef",
     "CreateChannelResponseTypeDef",
     "DescribeChannelResponseTypeDef",
     "UpdateChannelResponseTypeDef",
-    "PrefetchConsumptionUnionTypeDef",
     "CreatePrefetchScheduleRequestRequestTypeDef",
-    "PrefetchRetrievalUnionTypeDef",
+    "CreatePrefetchScheduleResponseTypeDef",
+    "GetPrefetchScheduleResponseTypeDef",
+    "PrefetchScheduleTypeDef",
     "GetChannelScheduleResponseTypeDef",
-    "AdBreakOutputTypeDef",
     "AdBreakTypeDef",
     "ListSourceLocationsResponseTypeDef",
     "ListPlaybackConfigurationsResponseTypeDef",
-    "ListPrefetchSchedulesResponseTypeDef",
     "ListChannelsResponseTypeDef",
+    "ListPrefetchSchedulesResponseTypeDef",
+    "CreateProgramRequestRequestTypeDef",
     "CreateProgramResponseTypeDef",
     "DescribeProgramResponseTypeDef",
-    "UpdateProgramResponseTypeDef",
-    "AdBreakUnionTypeDef",
-    "CreateProgramRequestRequestTypeDef",
     "UpdateProgramRequestRequestTypeDef",
+    "UpdateProgramResponseTypeDef",
 )
 
 SecretsManagerAccessTokenConfigurationTypeDef = TypedDict(
     "SecretsManagerAccessTokenConfigurationTypeDef",
     {
         "HeaderName": str,
         "SecretArn": str,
         "SecretStringKey": str,
     },
     total=False,
 )
 
+KeyValuePairTypeDef = TypedDict(
+    "KeyValuePairTypeDef",
+    {
+        "Key": str,
+        "Value": str,
+    },
+)
+
 SlateSourceTypeDef = TypedDict(
     "SlateSourceTypeDef",
     {
         "SourceLocationName": str,
         "VodSourceName": str,
     },
     total=False,
@@ -212,24 +217,36 @@
     "AdMarkerPassthroughTypeDef",
     {
         "Enabled": bool,
     },
     total=False,
 )
 
-AlertTypeDef = TypedDict(
-    "AlertTypeDef",
+_RequiredAlertTypeDef = TypedDict(
+    "_RequiredAlertTypeDef",
     {
         "AlertCode": str,
         "AlertMessage": str,
         "LastModifiedTime": datetime,
         "RelatedResourceArns": List[str],
         "ResourceArn": str,
     },
 )
+_OptionalAlertTypeDef = TypedDict(
+    "_OptionalAlertTypeDef",
+    {
+        "Category": AlertCategoryType,
+    },
+    total=False,
+)
+
+
+class AlertTypeDef(_RequiredAlertTypeDef, _OptionalAlertTypeDef):
+    pass
+
 
 AvailMatchingCriteriaTypeDef = TypedDict(
     "AvailMatchingCriteriaTypeDef",
     {
         "DynamicVariable": str,
         "Operator": Literal["EQUALS"],
     },
@@ -310,34 +327,14 @@
     {
         "Path": str,
         "SourceGroup": str,
         "Type": TypeType,
     },
 )
 
-_RequiredPrefetchRetrievalOutputTypeDef = TypedDict(
-    "_RequiredPrefetchRetrievalOutputTypeDef",
-    {
-        "EndTime": datetime,
-    },
-)
-_OptionalPrefetchRetrievalOutputTypeDef = TypedDict(
-    "_OptionalPrefetchRetrievalOutputTypeDef",
-    {
-        "DynamicVariables": Dict[str, str],
-        "StartTime": datetime,
-    },
-    total=False,
-)
-
-class PrefetchRetrievalOutputTypeDef(
-    _RequiredPrefetchRetrievalOutputTypeDef, _OptionalPrefetchRetrievalOutputTypeDef
-):
-    pass
-
 DefaultSegmentDeliveryConfigurationTypeDef = TypedDict(
     "DefaultSegmentDeliveryConfigurationTypeDef",
     {
         "BaseUrl": str,
     },
     total=False,
 )
@@ -515,20 +512,22 @@
         "DurationMinutes": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetChannelScheduleRequestRequestTypeDef(
     _RequiredGetChannelScheduleRequestRequestTypeDef,
     _OptionalGetChannelScheduleRequestRequestTypeDef,
 ):
     pass
 
+
 GetPlaybackConfigurationRequestRequestTypeDef = TypedDict(
     "GetPlaybackConfigurationRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -563,14 +562,15 @@
         "PlaybackConfigurationName": str,
     },
 )
 
 HlsPlaylistSettingsTypeDef = TypedDict(
     "HlsPlaylistSettingsTypeDef",
     {
+        "AdMarkupType": Sequence[AdMarkupTypeType],
         "ManifestWindowSeconds": int,
     },
     total=False,
 )
 
 _RequiredListAlertsRequestRequestTypeDef = TypedDict(
     "_RequiredListAlertsRequestRequestTypeDef",
@@ -583,19 +583,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAlertsRequestRequestTypeDef(
     _RequiredListAlertsRequestRequestTypeDef, _OptionalListAlertsRequestRequestTypeDef
 ):
     pass
 
+
 ListChannelsRequestRequestTypeDef = TypedDict(
     "ListChannelsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -612,19 +614,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListLiveSourcesRequestRequestTypeDef(
     _RequiredListLiveSourcesRequestRequestTypeDef, _OptionalListLiveSourcesRequestRequestTypeDef
 ):
     pass
 
+
 ListPlaybackConfigurationsRequestRequestTypeDef = TypedDict(
     "ListPlaybackConfigurationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -642,20 +646,22 @@
         "MaxResults": int,
         "NextToken": str,
         "StreamId": str,
     },
     total=False,
 )
 
+
 class ListPrefetchSchedulesRequestRequestTypeDef(
     _RequiredListPrefetchSchedulesRequestRequestTypeDef,
     _OptionalListPrefetchSchedulesRequestRequestTypeDef,
 ):
     pass
 
+
 ListSourceLocationsRequestRequestTypeDef = TypedDict(
     "ListSourceLocationsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -679,19 +685,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListVodSourcesRequestRequestTypeDef(
     _RequiredListVodSourcesRequestRequestTypeDef, _OptionalListVodSourcesRequestRequestTypeDef
 ):
     pass
 
+
 TimestampTypeDef = Union[datetime, str]
 PutChannelPolicyRequestRequestTypeDef = TypedDict(
     "PutChannelPolicyRequestRequestTypeDef",
     {
         "ChannelName": str,
         "Policy": str,
     },
@@ -721,17 +729,19 @@
         "DurationMillis": int,
         "RelativeProgram": str,
         "ScheduledStartTimeMillis": int,
     },
     total=False,
 )
 
+
 class TransitionTypeDef(_RequiredTransitionTypeDef, _OptionalTransitionTypeDef):
     pass
 
+
 SegmentationDescriptorTypeDef = TypedDict(
     "SegmentationDescriptorTypeDef",
     {
         "SegmentNum": int,
         "SegmentationEventId": int,
         "SegmentationTypeId": int,
         "SegmentationUpid": str,
@@ -795,34 +805,14 @@
     "ManifestProcessingRulesTypeDef",
     {
         "AdMarkerPassthrough": AdMarkerPassthroughTypeDef,
     },
     total=False,
 )
 
-_RequiredPrefetchConsumptionOutputTypeDef = TypedDict(
-    "_RequiredPrefetchConsumptionOutputTypeDef",
-    {
-        "EndTime": datetime,
-    },
-)
-_OptionalPrefetchConsumptionOutputTypeDef = TypedDict(
-    "_OptionalPrefetchConsumptionOutputTypeDef",
-    {
-        "AvailMatchingCriteria": List[AvailMatchingCriteriaTypeDef],
-        "StartTime": datetime,
-    },
-    total=False,
-)
-
-class PrefetchConsumptionOutputTypeDef(
-    _RequiredPrefetchConsumptionOutputTypeDef, _OptionalPrefetchConsumptionOutputTypeDef
-):
-    pass
-
 ConfigureLogsForChannelResponseTypeDef = TypedDict(
     "ConfigureLogsForChannelResponseTypeDef",
     {
         "ChannelName": str,
         "LogTypes": List[Literal["AS_RUN"]],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -881,19 +871,21 @@
     "_OptionalCreateLiveSourceRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateLiveSourceRequestRequestTypeDef(
     _RequiredCreateLiveSourceRequestRequestTypeDef, _OptionalCreateLiveSourceRequestRequestTypeDef
 ):
     pass
 
+
 CreateLiveSourceResponseTypeDef = TypedDict(
     "CreateLiveSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
@@ -916,19 +908,21 @@
     "_OptionalCreateVodSourceRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateVodSourceRequestRequestTypeDef(
     _RequiredCreateVodSourceRequestRequestTypeDef, _OptionalCreateVodSourceRequestRequestTypeDef
 ):
     pass
 
+
 CreateVodSourceResponseTypeDef = TypedDict(
     "CreateVodSourceResponseTypeDef",
     {
         "Arn": str,
         "CreationTime": datetime,
         "HttpPackageConfigurations": List[HttpPackageConfigurationTypeDef],
         "LastModifiedTime": datetime,
@@ -982,17 +976,19 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class LiveSourceTypeDef(_RequiredLiveSourceTypeDef, _OptionalLiveSourceTypeDef):
     pass
 
+
 UpdateLiveSourceRequestRequestTypeDef = TypedDict(
     "UpdateLiveSourceRequestRequestTypeDef",
     {
         "HttpPackageConfigurations": Sequence[HttpPackageConfigurationTypeDef],
         "LiveSourceName": str,
         "SourceLocationName": str,
     },
@@ -1050,17 +1046,19 @@
         "CreationTime": datetime,
         "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class VodSourceTypeDef(_RequiredVodSourceTypeDef, _OptionalVodSourceTypeDef):
     pass
 
+
 _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
     "_RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef",
     {
         "ChannelName": str,
     },
 )
 _OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef = TypedDict(
@@ -1068,40 +1066,44 @@
     {
         "DurationMinutes": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetChannelScheduleRequestGetChannelSchedulePaginateTypeDef(
     _RequiredGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
     _OptionalGetChannelScheduleRequestGetChannelSchedulePaginateTypeDef,
 ):
     pass
 
+
 _RequiredListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
     "_RequiredListAlertsRequestListAlertsPaginateTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListAlertsRequestListAlertsPaginateTypeDef = TypedDict(
     "_OptionalListAlertsRequestListAlertsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListAlertsRequestListAlertsPaginateTypeDef(
     _RequiredListAlertsRequestListAlertsPaginateTypeDef,
     _OptionalListAlertsRequestListAlertsPaginateTypeDef,
 ):
     pass
 
+
 ListChannelsRequestListChannelsPaginateTypeDef = TypedDict(
     "ListChannelsRequestListChannelsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1116,20 +1118,22 @@
     "_OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListLiveSourcesRequestListLiveSourcesPaginateTypeDef(
     _RequiredListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
     _OptionalListLiveSourcesRequestListLiveSourcesPaginateTypeDef,
 ):
     pass
 
+
 ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef = TypedDict(
     "ListPlaybackConfigurationsRequestListPlaybackConfigurationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1145,20 +1149,22 @@
     {
         "StreamId": str,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef(
     _RequiredListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
     _OptionalListPrefetchSchedulesRequestListPrefetchSchedulesPaginateTypeDef,
 ):
     pass
 
+
 ListSourceLocationsRequestListSourceLocationsPaginateTypeDef = TypedDict(
     "ListSourceLocationsRequestListSourceLocationsPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
@@ -1173,20 +1179,22 @@
     "_OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef",
     {
         "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListVodSourcesRequestListVodSourcesPaginateTypeDef(
     _RequiredListVodSourcesRequestListVodSourcesPaginateTypeDef,
     _OptionalListVodSourcesRequestListVodSourcesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredRequestOutputItemTypeDef = TypedDict(
     "_RequiredRequestOutputItemTypeDef",
     {
         "ManifestName": str,
         "SourceGroup": str,
     },
 )
@@ -1195,19 +1203,21 @@
     {
         "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
         "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
     },
     total=False,
 )
 
+
 class RequestOutputItemTypeDef(
     _RequiredRequestOutputItemTypeDef, _OptionalRequestOutputItemTypeDef
 ):
     pass
 
+
 _RequiredResponseOutputItemTypeDef = TypedDict(
     "_RequiredResponseOutputItemTypeDef",
     {
         "ManifestName": str,
         "PlaybackUrl": str,
         "SourceGroup": str,
     },
@@ -1217,19 +1227,21 @@
     {
         "DashPlaylistSettings": DashPlaylistSettingsTypeDef,
         "HlsPlaylistSettings": HlsPlaylistSettingsTypeDef,
     },
     total=False,
 )
 
+
 class ResponseOutputItemTypeDef(
     _RequiredResponseOutputItemTypeDef, _OptionalResponseOutputItemTypeDef
 ):
     pass
 
+
 _RequiredPrefetchConsumptionTypeDef = TypedDict(
     "_RequiredPrefetchConsumptionTypeDef",
     {
         "EndTime": TimestampTypeDef,
     },
 )
 _OptionalPrefetchConsumptionTypeDef = TypedDict(
@@ -1237,19 +1249,21 @@
     {
         "AvailMatchingCriteria": Sequence[AvailMatchingCriteriaTypeDef],
         "StartTime": TimestampTypeDef,
     },
     total=False,
 )
 
+
 class PrefetchConsumptionTypeDef(
     _RequiredPrefetchConsumptionTypeDef, _OptionalPrefetchConsumptionTypeDef
 ):
     pass
 
+
 _RequiredPrefetchRetrievalTypeDef = TypedDict(
     "_RequiredPrefetchRetrievalTypeDef",
     {
         "EndTime": TimestampTypeDef,
     },
 )
 _OptionalPrefetchRetrievalTypeDef = TypedDict(
@@ -1257,19 +1271,21 @@
     {
         "DynamicVariables": Mapping[str, str],
         "StartTime": TimestampTypeDef,
     },
     total=False,
 )
 
+
 class PrefetchRetrievalTypeDef(
     _RequiredPrefetchRetrievalTypeDef, _OptionalPrefetchRetrievalTypeDef
 ):
     pass
 
+
 _RequiredScheduleEntryTypeDef = TypedDict(
     "_RequiredScheduleEntryTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ProgramName": str,
         "SourceLocationName": str,
@@ -1284,43 +1300,39 @@
         "ScheduleAdBreaks": List[ScheduleAdBreakTypeDef],
         "ScheduleEntryType": ScheduleEntryTypeType,
         "VodSourceName": str,
     },
     total=False,
 )
 
+
 class ScheduleEntryTypeDef(_RequiredScheduleEntryTypeDef, _OptionalScheduleEntryTypeDef):
     pass
 
+
 _RequiredScheduleConfigurationTypeDef = TypedDict(
     "_RequiredScheduleConfigurationTypeDef",
     {
         "Transition": TransitionTypeDef,
     },
 )
 _OptionalScheduleConfigurationTypeDef = TypedDict(
     "_OptionalScheduleConfigurationTypeDef",
     {
         "ClipRange": ClipRangeTypeDef,
     },
     total=False,
 )
 
+
 class ScheduleConfigurationTypeDef(
     _RequiredScheduleConfigurationTypeDef, _OptionalScheduleConfigurationTypeDef
 ):
     pass
 
-TimeSignalMessageOutputTypeDef = TypedDict(
-    "TimeSignalMessageOutputTypeDef",
-    {
-        "SegmentationDescriptors": List[SegmentationDescriptorTypeDef],
-    },
-    total=False,
-)
 
 TimeSignalMessageTypeDef = TypedDict(
     "TimeSignalMessageTypeDef",
     {
         "SegmentationDescriptors": Sequence[SegmentationDescriptorTypeDef],
     },
     total=False,
@@ -1349,20 +1361,22 @@
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "SegmentDeliveryConfigurations": Sequence[SegmentDeliveryConfigurationTypeDef],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateSourceLocationRequestRequestTypeDef(
     _RequiredCreateSourceLocationRequestRequestTypeDef,
     _OptionalCreateSourceLocationRequestRequestTypeDef,
 ):
     pass
 
+
 CreateSourceLocationResponseTypeDef = TypedDict(
     "CreateSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
@@ -1408,17 +1422,19 @@
         "LastModifiedTime": datetime,
         "SegmentDeliveryConfigurations": List[SegmentDeliveryConfigurationTypeDef],
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class SourceLocationTypeDef(_RequiredSourceLocationTypeDef, _OptionalSourceLocationTypeDef):
     pass
 
+
 _RequiredUpdateSourceLocationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSourceLocationRequestRequestTypeDef",
     {
         "HttpConfiguration": HttpConfigurationTypeDef,
         "SourceLocationName": str,
     },
 )
@@ -1428,20 +1444,22 @@
         "AccessConfiguration": AccessConfigurationTypeDef,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
         "SegmentDeliveryConfigurations": Sequence[SegmentDeliveryConfigurationTypeDef],
     },
     total=False,
 )
 
+
 class UpdateSourceLocationRequestRequestTypeDef(
     _RequiredUpdateSourceLocationRequestRequestTypeDef,
     _OptionalUpdateSourceLocationRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateSourceLocationResponseTypeDef = TypedDict(
     "UpdateSourceLocationResponseTypeDef",
     {
         "AccessConfiguration": AccessConfigurationTypeDef,
         "Arn": str,
         "CreationTime": datetime,
         "DefaultSegmentDeliveryConfiguration": DefaultSegmentDeliveryConfigurationTypeDef,
@@ -1528,20 +1546,22 @@
         "Tags": Mapping[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
     },
     total=False,
 )
 
+
 class PutPlaybackConfigurationRequestRequestTypeDef(
     _RequiredPutPlaybackConfigurationRequestRequestTypeDef,
     _OptionalPutPlaybackConfigurationRequestRequestTypeDef,
 ):
     pass
 
+
 PutPlaybackConfigurationResponseTypeDef = TypedDict(
     "PutPlaybackConfigurationResponseTypeDef",
     {
         "AdDecisionServerUrl": str,
         "AvailSuppression": AvailSuppressionTypeDef,
         "Bumper": BumperTypeDef,
         "CdnConfiguration": CdnConfigurationTypeDef,
@@ -1560,61 +1580,14 @@
         "Tags": Dict[str, str],
         "TranscodeProfileName": str,
         "VideoContentSourceUrl": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreatePrefetchScheduleResponseTypeDef = TypedDict(
-    "CreatePrefetchScheduleResponseTypeDef",
-    {
-        "Arn": str,
-        "Consumption": PrefetchConsumptionOutputTypeDef,
-        "Name": str,
-        "PlaybackConfigurationName": str,
-        "Retrieval": PrefetchRetrievalOutputTypeDef,
-        "StreamId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-GetPrefetchScheduleResponseTypeDef = TypedDict(
-    "GetPrefetchScheduleResponseTypeDef",
-    {
-        "Arn": str,
-        "Consumption": PrefetchConsumptionOutputTypeDef,
-        "Name": str,
-        "PlaybackConfigurationName": str,
-        "Retrieval": PrefetchRetrievalOutputTypeDef,
-        "StreamId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
-_RequiredPrefetchScheduleTypeDef = TypedDict(
-    "_RequiredPrefetchScheduleTypeDef",
-    {
-        "Arn": str,
-        "Consumption": PrefetchConsumptionOutputTypeDef,
-        "Name": str,
-        "PlaybackConfigurationName": str,
-        "Retrieval": PrefetchRetrievalOutputTypeDef,
-    },
-)
-_OptionalPrefetchScheduleTypeDef = TypedDict(
-    "_OptionalPrefetchScheduleTypeDef",
-    {
-        "StreamId": str,
-    },
-    total=False,
-)
-
-class PrefetchScheduleTypeDef(_RequiredPrefetchScheduleTypeDef, _OptionalPrefetchScheduleTypeDef):
-    pass
-
 ListLiveSourcesResponseTypeDef = TypedDict(
     "ListLiveSourcesResponseTypeDef",
     {
         "Items": List[LiveSourceTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1643,19 +1616,21 @@
         "FillerSlate": SlateSourceTypeDef,
         "Tags": Mapping[str, str],
         "Tier": TierType,
     },
     total=False,
 )
 
+
 class CreateChannelRequestRequestTypeDef(
     _RequiredCreateChannelRequestRequestTypeDef, _OptionalCreateChannelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateChannelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateChannelRequestRequestTypeDef",
     {
         "ChannelName": str,
         "Outputs": Sequence[RequestOutputItemTypeDef],
     },
 )
@@ -1663,19 +1638,21 @@
     "_OptionalUpdateChannelRequestRequestTypeDef",
     {
         "FillerSlate": SlateSourceTypeDef,
     },
     total=False,
 )
 
+
 class UpdateChannelRequestRequestTypeDef(
     _RequiredUpdateChannelRequestRequestTypeDef, _OptionalUpdateChannelRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredChannelTypeDef = TypedDict(
     "_RequiredChannelTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": str,
         "LogConfiguration": LogConfigurationForChannelTypeDef,
@@ -1691,17 +1668,19 @@
         "FillerSlate": SlateSourceTypeDef,
         "LastModifiedTime": datetime,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class ChannelTypeDef(_RequiredChannelTypeDef, _OptionalChannelTypeDef):
     pass
 
+
 CreateChannelResponseTypeDef = TypedDict(
     "CreateChannelResponseTypeDef",
     {
         "Arn": str,
         "ChannelName": str,
         "ChannelState": ChannelStateType,
         "CreationTime": datetime,
@@ -1746,17 +1725,14 @@
         "PlaybackMode": str,
         "Tags": Dict[str, str],
         "Tier": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PrefetchConsumptionUnionTypeDef = Union[
-    PrefetchConsumptionTypeDef, PrefetchConsumptionOutputTypeDef
-]
 _RequiredCreatePrefetchScheduleRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePrefetchScheduleRequestRequestTypeDef",
     {
         "Consumption": PrefetchConsumptionTypeDef,
         "Name": str,
         "PlaybackConfigurationName": str,
         "Retrieval": PrefetchRetrievalTypeDef,
@@ -1766,45 +1742,84 @@
     "_OptionalCreatePrefetchScheduleRequestRequestTypeDef",
     {
         "StreamId": str,
     },
     total=False,
 )
 
+
 class CreatePrefetchScheduleRequestRequestTypeDef(
     _RequiredCreatePrefetchScheduleRequestRequestTypeDef,
     _OptionalCreatePrefetchScheduleRequestRequestTypeDef,
 ):
     pass
 
-PrefetchRetrievalUnionTypeDef = Union[PrefetchRetrievalTypeDef, PrefetchRetrievalOutputTypeDef]
-GetChannelScheduleResponseTypeDef = TypedDict(
-    "GetChannelScheduleResponseTypeDef",
+
+CreatePrefetchScheduleResponseTypeDef = TypedDict(
+    "CreatePrefetchScheduleResponseTypeDef",
     {
-        "Items": List[ScheduleEntryTypeDef],
-        "NextToken": str,
+        "Arn": str,
+        "Consumption": PrefetchConsumptionTypeDef,
+        "Name": str,
+        "PlaybackConfigurationName": str,
+        "Retrieval": PrefetchRetrievalTypeDef,
+        "StreamId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdBreakOutputTypeDef = TypedDict(
-    "AdBreakOutputTypeDef",
+GetPrefetchScheduleResponseTypeDef = TypedDict(
+    "GetPrefetchScheduleResponseTypeDef",
     {
-        "MessageType": MessageTypeType,
-        "OffsetMillis": int,
-        "Slate": SlateSourceTypeDef,
-        "SpliceInsertMessage": SpliceInsertMessageTypeDef,
-        "TimeSignalMessage": TimeSignalMessageOutputTypeDef,
+        "Arn": str,
+        "Consumption": PrefetchConsumptionTypeDef,
+        "Name": str,
+        "PlaybackConfigurationName": str,
+        "Retrieval": PrefetchRetrievalTypeDef,
+        "StreamId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPrefetchScheduleTypeDef = TypedDict(
+    "_RequiredPrefetchScheduleTypeDef",
+    {
+        "Arn": str,
+        "Consumption": PrefetchConsumptionTypeDef,
+        "Name": str,
+        "PlaybackConfigurationName": str,
+        "Retrieval": PrefetchRetrievalTypeDef,
+    },
+)
+_OptionalPrefetchScheduleTypeDef = TypedDict(
+    "_OptionalPrefetchScheduleTypeDef",
+    {
+        "StreamId": str,
     },
     total=False,
 )
 
+
+class PrefetchScheduleTypeDef(_RequiredPrefetchScheduleTypeDef, _OptionalPrefetchScheduleTypeDef):
+    pass
+
+
+GetChannelScheduleResponseTypeDef = TypedDict(
+    "GetChannelScheduleResponseTypeDef",
+    {
+        "Items": List[ScheduleEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AdBreakTypeDef = TypedDict(
     "AdBreakTypeDef",
     {
+        "AdBreakMetadata": Sequence[KeyValuePairTypeDef],
         "MessageType": MessageTypeType,
         "OffsetMillis": int,
         "Slate": SlateSourceTypeDef,
         "SpliceInsertMessage": SpliceInsertMessageTypeDef,
         "TimeSignalMessage": TimeSignalMessageTypeDef,
     },
     total=False,
@@ -1824,124 +1839,127 @@
     {
         "Items": List[PlaybackConfigurationTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListPrefetchSchedulesResponseTypeDef = TypedDict(
-    "ListPrefetchSchedulesResponseTypeDef",
+ListChannelsResponseTypeDef = TypedDict(
+    "ListChannelsResponseTypeDef",
     {
-        "Items": List[PrefetchScheduleTypeDef],
+        "Items": List[ChannelTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListChannelsResponseTypeDef = TypedDict(
-    "ListChannelsResponseTypeDef",
+ListPrefetchSchedulesResponseTypeDef = TypedDict(
+    "ListPrefetchSchedulesResponseTypeDef",
     {
-        "Items": List[ChannelTypeDef],
+        "Items": List[PrefetchScheduleTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateProgramResponseTypeDef = TypedDict(
-    "CreateProgramResponseTypeDef",
+_RequiredCreateProgramRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateProgramRequestRequestTypeDef",
     {
-        "AdBreaks": List[AdBreakOutputTypeDef],
-        "Arn": str,
         "ChannelName": str,
-        "ClipRange": ClipRangeTypeDef,
-        "CreationTime": datetime,
-        "DurationMillis": int,
-        "LiveSourceName": str,
         "ProgramName": str,
-        "ScheduledStartTime": datetime,
+        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "SourceLocationName": str,
+    },
+)
+_OptionalCreateProgramRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateProgramRequestRequestTypeDef",
+    {
+        "AdBreaks": Sequence[AdBreakTypeDef],
+        "LiveSourceName": str,
         "VodSourceName": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
     },
+    total=False,
 )
 
-DescribeProgramResponseTypeDef = TypedDict(
-    "DescribeProgramResponseTypeDef",
+
+class CreateProgramRequestRequestTypeDef(
+    _RequiredCreateProgramRequestRequestTypeDef, _OptionalCreateProgramRequestRequestTypeDef
+):
+    pass
+
+
+CreateProgramResponseTypeDef = TypedDict(
+    "CreateProgramResponseTypeDef",
     {
-        "AdBreaks": List[AdBreakOutputTypeDef],
+        "AdBreaks": List[AdBreakTypeDef],
         "Arn": str,
         "ChannelName": str,
         "ClipRange": ClipRangeTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateProgramResponseTypeDef = TypedDict(
-    "UpdateProgramResponseTypeDef",
+DescribeProgramResponseTypeDef = TypedDict(
+    "DescribeProgramResponseTypeDef",
     {
-        "AdBreaks": List[AdBreakOutputTypeDef],
+        "AdBreaks": List[AdBreakTypeDef],
         "Arn": str,
         "ChannelName": str,
         "ClipRange": ClipRangeTypeDef,
         "CreationTime": datetime,
         "DurationMillis": int,
         "LiveSourceName": str,
         "ProgramName": str,
         "ScheduledStartTime": datetime,
         "SourceLocationName": str,
         "VodSourceName": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdBreakUnionTypeDef = Union[AdBreakTypeDef, AdBreakOutputTypeDef]
-_RequiredCreateProgramRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateProgramRequestRequestTypeDef",
-    {
-        "ChannelName": str,
-        "ProgramName": str,
-        "ScheduleConfiguration": ScheduleConfigurationTypeDef,
-        "SourceLocationName": str,
-    },
-)
-_OptionalCreateProgramRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateProgramRequestRequestTypeDef",
-    {
-        "AdBreaks": Sequence[AdBreakUnionTypeDef],
-        "LiveSourceName": str,
-        "VodSourceName": str,
-    },
-    total=False,
-)
-
-class CreateProgramRequestRequestTypeDef(
-    _RequiredCreateProgramRequestRequestTypeDef, _OptionalCreateProgramRequestRequestTypeDef
-):
-    pass
-
 _RequiredUpdateProgramRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateProgramRequestRequestTypeDef",
     {
         "ChannelName": str,
         "ProgramName": str,
         "ScheduleConfiguration": UpdateProgramScheduleConfigurationTypeDef,
     },
 )
 _OptionalUpdateProgramRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateProgramRequestRequestTypeDef",
     {
-        "AdBreaks": Sequence[AdBreakUnionTypeDef],
+        "AdBreaks": Sequence[AdBreakTypeDef],
     },
     total=False,
 )
 
+
 class UpdateProgramRequestRequestTypeDef(
     _RequiredUpdateProgramRequestRequestTypeDef, _OptionalUpdateProgramRequestRequestTypeDef
 ):
     pass
+
+
+UpdateProgramResponseTypeDef = TypedDict(
+    "UpdateProgramResponseTypeDef",
+    {
+        "AdBreaks": List[AdBreakTypeDef],
+        "Arn": str,
+        "ChannelName": str,
+        "ClipRange": ClipRangeTypeDef,
+        "CreationTime": datetime,
+        "DurationMillis": int,
+        "LiveSourceName": str,
+        "ProgramName": str,
+        "ScheduledStartTime": datetime,
+        "SourceLocationName": str,
+        "VodSourceName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
```

### Comparing `types-aiobotocore-mediatailor-2.5.2.post1/types_aiobotocore_mediatailor.egg-info/SOURCES.txt` & `types-aiobotocore-mediatailor-2.5.2.post2/types_aiobotocore_mediatailor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

