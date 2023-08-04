# Comparing `tmp/types-aiobotocore-cloudtrail-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-cloudtrail-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudtrail-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudtrail-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:36 2023, max compression
```

## Comparing `types-aiobotocore-cloudtrail-2.5.2.post1.tar` & `types-aiobotocore-cloudtrail-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.257627 types-aiobotocore-cloudtrail-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-08-02 14:52:02.257627 types-aiobotocore-cloudtrail-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16761 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.257627 types-aiobotocore-cloudtrail-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.253627 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41319 2023-08-02 14:34:45.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-08-02 14:34:45.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-08-02 14:34:45.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-02 14:34:45.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-08-02 14:34:45.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    41873 2023-08-02 14:34:46.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    41835 2023-08-02 14:34:45.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:44.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.257627 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18291 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:02.000000 types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.271525 types-aiobotocore-cloudtrail-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-08-04 12:00:36.263525 types-aiobotocore-cloudtrail-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:36.271525 types-aiobotocore-cloudtrail-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.263525 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41289 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41228 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10114 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10112 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7957 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39768 2023-08-04 11:42:01.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39733 2023-08-04 11:42:01.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:41:59.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:36.263525 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-08-04 12:00:36.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-04 12:00:36.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:36.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:36.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-04 12:00:36.000000 types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/LICENSE` & `types-aiobotocore-cloudtrail-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/setup.py` & `types-aiobotocore-cloudtrail-2.5.2.post2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudtrail",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_cloudtrail"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudTrail 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/__init__.py` & `types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/__init__.pyi` & `types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/__main__.py` & `types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudTrail 2.5.2\nVersion:         2.5.2.post1\nBuilder"
-        " version: 7.17.1\nDocs:           "
+        "Type annotations for aiobotocore.CloudTrail 2.5.2\nVersion:         2.5.2.post2\nBuilder"
+        " version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail\nOther"
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

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/client.py` & `types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     ListImportsPaginator,
     ListPublicKeysPaginator,
     ListTagsPaginator,
     ListTrailsPaginator,
     LookupEventsPaginator,
 )
 from .type_defs import (
-    AdvancedEventSelectorUnionTypeDef,
+    AdvancedEventSelectorTypeDef,
     CancelQueryResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateEventDataStoreResponseTypeDef,
     CreateTrailResponseTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     DestinationTypeDef,
-    EventSelectorUnionTypeDef,
+    EventSelectorTypeDef,
     GetChannelResponseTypeDef,
     GetEventDataStoreResponseTypeDef,
     GetEventSelectorsResponseTypeDef,
     GetImportResponseTypeDef,
     GetInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
@@ -243,15 +243,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#create_channel)
         """
 
     async def create_event_data_store(
         self,
         *,
         Name: str,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         TagsList: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         StartIngestion: bool = ...
@@ -571,16 +571,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#lookup_events)
         """
 
     async def put_event_selectors(
         self,
         *,
         TrailName: str,
-        EventSelectors: Sequence[EventSelectorUnionTypeDef] = ...,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...
+        EventSelectors: Sequence[EventSelectorTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...
     ) -> PutEventSelectorsResponseTypeDef:
         """
         Configures an event selector or advanced event selectors for your trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_event_selectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#put_event_selectors)
         """
@@ -726,15 +726,15 @@
         """
 
     async def update_event_data_store(
         self,
         *,
         EventDataStore: str,
         Name: str = ...,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         KmsKeyId: str = ...
     ) -> UpdateEventDataStoreResponseTypeDef:
         """
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/client.pyi` & `types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -26,23 +26,23 @@
     ListImportsPaginator,
     ListPublicKeysPaginator,
     ListTagsPaginator,
     ListTrailsPaginator,
     LookupEventsPaginator,
 )
 from .type_defs import (
-    AdvancedEventSelectorUnionTypeDef,
+    AdvancedEventSelectorTypeDef,
     CancelQueryResponseTypeDef,
     CreateChannelResponseTypeDef,
     CreateEventDataStoreResponseTypeDef,
     CreateTrailResponseTypeDef,
     DescribeQueryResponseTypeDef,
     DescribeTrailsResponseTypeDef,
     DestinationTypeDef,
-    EventSelectorUnionTypeDef,
+    EventSelectorTypeDef,
     GetChannelResponseTypeDef,
     GetEventDataStoreResponseTypeDef,
     GetEventSelectorsResponseTypeDef,
     GetImportResponseTypeDef,
     GetInsightSelectorsResponseTypeDef,
     GetQueryResultsResponseTypeDef,
     GetResourcePolicyResponseTypeDef,
@@ -233,15 +233,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.create_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#create_channel)
         """
     async def create_event_data_store(
         self,
         *,
         Name: str,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         TagsList: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...,
         StartIngestion: bool = ...
@@ -533,16 +533,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.lookup_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#lookup_events)
         """
     async def put_event_selectors(
         self,
         *,
         TrailName: str,
-        EventSelectors: Sequence[EventSelectorUnionTypeDef] = ...,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...
+        EventSelectors: Sequence[EventSelectorTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...
     ) -> PutEventSelectorsResponseTypeDef:
         """
         Configures an event selector or advanced event selectors for your trail.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudtrail.html#CloudTrail.Client.put_event_selectors)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#put_event_selectors)
         """
@@ -674,15 +674,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudtrail/client/#update_channel)
         """
     async def update_event_data_store(
         self,
         *,
         EventDataStore: str,
         Name: str = ...,
-        AdvancedEventSelectors: Sequence[AdvancedEventSelectorUnionTypeDef] = ...,
+        AdvancedEventSelectors: Sequence[AdvancedEventSelectorTypeDef] = ...,
         MultiRegionEnabled: bool = ...,
         OrganizationEnabled: bool = ...,
         RetentionPeriod: int = ...,
         TerminationProtectionEnabled: bool = ...,
         KmsKeyId: str = ...
     ) -> UpdateEventDataStoreResponseTypeDef:
         """
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/literals.py` & `types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/literals.pyi` & `types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/paginator.py` & `types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/paginator.pyi` & `types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/type_defs.py` & `types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,21 +35,19 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "AdvancedFieldSelectorOutputTypeDef",
     "AdvancedFieldSelectorTypeDef",
     "CancelQueryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ChannelTypeDef",
     "DestinationTypeDef",
-    "DataResourceOutputTypeDef",
     "DataResourceTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteEventDataStoreRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteTrailRequestRequestTypeDef",
     "DeregisterOrganizationDelegatedAdminRequestRequestTypeDef",
     "DescribeQueryRequestRequestTypeDef",
@@ -95,29 +93,27 @@
     "StopImportRequestRequestTypeDef",
     "StopLoggingRequestRequestTypeDef",
     "UpdateTrailRequestRequestTypeDef",
     "AddTagsRequestRequestTypeDef",
     "CreateTrailRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
     "ResourceTagTypeDef",
-    "AdvancedEventSelectorOutputTypeDef",
     "AdvancedEventSelectorTypeDef",
     "CancelQueryResponseTypeDef",
     "CreateTrailResponseTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "GetTrailStatusResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
     "StartQueryResponseTypeDef",
     "UpdateTrailResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
-    "EventSelectorOutputTypeDef",
     "EventSelectorTypeDef",
     "DescribeQueryResponseTypeDef",
     "DescribeTrailsResponseTypeDef",
     "GetTrailResponseTypeDef",
     "EventTypeDef",
     "GetInsightSelectorsResponseTypeDef",
     "PutInsightSelectorsRequestRequestTypeDef",
@@ -135,34 +131,32 @@
     "ListQueriesRequestRequestTypeDef",
     "ListPublicKeysResponseTypeDef",
     "ListQueriesResponseTypeDef",
     "ListTrailsResponseTypeDef",
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     "LookupEventsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
+    "CreateEventDataStoreRequestRequestTypeDef",
     "CreateEventDataStoreResponseTypeDef",
     "EventDataStoreTypeDef",
     "GetEventDataStoreResponseTypeDef",
     "RestoreEventDataStoreResponseTypeDef",
     "SourceConfigTypeDef",
+    "UpdateEventDataStoreRequestRequestTypeDef",
     "UpdateEventDataStoreResponseTypeDef",
-    "AdvancedEventSelectorUnionTypeDef",
     "GetEventSelectorsResponseTypeDef",
+    "PutEventSelectorsRequestRequestTypeDef",
     "PutEventSelectorsResponseTypeDef",
-    "EventSelectorUnionTypeDef",
     "LookupEventsResponseTypeDef",
     "GetImportResponseTypeDef",
     "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "StopImportResponseTypeDef",
     "ListEventDataStoresResponseTypeDef",
     "GetChannelResponseTypeDef",
-    "CreateEventDataStoreRequestRequestTypeDef",
-    "UpdateEventDataStoreRequestRequestTypeDef",
-    "PutEventSelectorsRequestRequestTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
@@ -176,40 +170,14 @@
 )
 
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
 
-_RequiredAdvancedFieldSelectorOutputTypeDef = TypedDict(
-    "_RequiredAdvancedFieldSelectorOutputTypeDef",
-    {
-        "Field": str,
-    },
-)
-_OptionalAdvancedFieldSelectorOutputTypeDef = TypedDict(
-    "_OptionalAdvancedFieldSelectorOutputTypeDef",
-    {
-        "Equals": List[str],
-        "StartsWith": List[str],
-        "EndsWith": List[str],
-        "NotEquals": List[str],
-        "NotStartsWith": List[str],
-        "NotEndsWith": List[str],
-    },
-    total=False,
-)
-
-
-class AdvancedFieldSelectorOutputTypeDef(
-    _RequiredAdvancedFieldSelectorOutputTypeDef, _OptionalAdvancedFieldSelectorOutputTypeDef
-):
-    pass
-
-
 _RequiredAdvancedFieldSelectorTypeDef = TypedDict(
     "_RequiredAdvancedFieldSelectorTypeDef",
     {
         "Field": str,
     },
 )
 _OptionalAdvancedFieldSelectorTypeDef = TypedDict(
@@ -277,28 +245,19 @@
     "DestinationTypeDef",
     {
         "Type": DestinationTypeType,
         "Location": str,
     },
 )
 
-DataResourceOutputTypeDef = TypedDict(
-    "DataResourceOutputTypeDef",
-    {
-        "Type": str,
-        "Values": List[str],
-    },
-    total=False,
-)
-
 DataResourceTypeDef = TypedDict(
     "DataResourceTypeDef",
     {
         "Type": str,
-        "Values": Sequence[str],
+        "Values": List[str],
     },
     total=False,
 )
 
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
@@ -832,35 +791,14 @@
     {
         "ResourceId": str,
         "TagsList": List[TagTypeDef],
     },
     total=False,
 )
 
-_RequiredAdvancedEventSelectorOutputTypeDef = TypedDict(
-    "_RequiredAdvancedEventSelectorOutputTypeDef",
-    {
-        "FieldSelectors": List[AdvancedFieldSelectorOutputTypeDef],
-    },
-)
-_OptionalAdvancedEventSelectorOutputTypeDef = TypedDict(
-    "_OptionalAdvancedEventSelectorOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-
-class AdvancedEventSelectorOutputTypeDef(
-    _RequiredAdvancedEventSelectorOutputTypeDef, _OptionalAdvancedEventSelectorOutputTypeDef
-):
-    pass
-
-
 _RequiredAdvancedEventSelectorTypeDef = TypedDict(
     "_RequiredAdvancedEventSelectorTypeDef",
     {
         "FieldSelectors": Sequence[AdvancedFieldSelectorTypeDef],
     },
 )
 _OptionalAdvancedEventSelectorTypeDef = TypedDict(
@@ -1050,32 +988,21 @@
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EventSelectorOutputTypeDef = TypedDict(
-    "EventSelectorOutputTypeDef",
-    {
-        "ReadWriteType": ReadWriteTypeType,
-        "IncludeManagementEvents": bool,
-        "DataResources": List[DataResourceOutputTypeDef],
-        "ExcludeManagementEventSources": List[str],
-    },
-    total=False,
-)
-
 EventSelectorTypeDef = TypedDict(
     "EventSelectorTypeDef",
     {
         "ReadWriteType": ReadWriteTypeType,
         "IncludeManagementEvents": bool,
-        "DataResources": Sequence[DataResourceTypeDef],
-        "ExcludeManagementEventSources": Sequence[str],
+        "DataResources": List[DataResourceTypeDef],
+        "ExcludeManagementEventSources": List[str],
     },
     total=False,
 )
 
 DescribeQueryResponseTypeDef = TypedDict(
     "DescribeQueryResponseTypeDef",
     {
@@ -1348,21 +1275,50 @@
     {
         "ResourceTagList": List[ResourceTagTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "TagsList": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "StartIngestion": bool,
+    },
+    total=False,
+)
+
+
+class CreateEventDataStoreRequestRequestTypeDef(
+    _RequiredCreateEventDataStoreRequestRequestTypeDef,
+    _OptionalCreateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
+
 CreateEventDataStoreResponseTypeDef = TypedDict(
     "CreateEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "TagsList": List[TagTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
@@ -1374,15 +1330,15 @@
 EventDataStoreTypeDef = TypedDict(
     "EventDataStoreTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "TerminationProtectionEnabled": bool,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
@@ -1390,15 +1346,15 @@
 
 GetEventDataStoreResponseTypeDef = TypedDict(
     "GetEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
@@ -1408,15 +1364,15 @@
 
 RestoreEventDataStoreResponseTypeDef = TypedDict(
     "RestoreEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
@@ -1424,61 +1380,107 @@
     },
 )
 
 SourceConfigTypeDef = TypedDict(
     "SourceConfigTypeDef",
     {
         "ApplyToAllRegions": bool,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
     },
     total=False,
 )
 
+_RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
+    },
+)
+_OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+
+class UpdateEventDataStoreRequestRequestTypeDef(
+    _RequiredUpdateEventDataStoreRequestRequestTypeDef,
+    _OptionalUpdateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
+
 UpdateEventDataStoreResponseTypeDef = TypedDict(
     "UpdateEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdvancedEventSelectorUnionTypeDef = Union[
-    AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef
-]
 GetEventSelectorsResponseTypeDef = TypedDict(
     "GetEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "EventSelectors": List[EventSelectorOutputTypeDef],
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "EventSelectors": List[EventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEventSelectorsRequestRequestTypeDef",
+    {
+        "TrailName": str,
+    },
+)
+_OptionalPutEventSelectorsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEventSelectorsRequestRequestTypeDef",
+    {
+        "EventSelectors": Sequence[EventSelectorTypeDef],
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
+    },
+    total=False,
+)
+
+
+class PutEventSelectorsRequestRequestTypeDef(
+    _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
+):
+    pass
+
+
 PutEventSelectorsResponseTypeDef = TypedDict(
     "PutEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "EventSelectors": List[EventSelectorOutputTypeDef],
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "EventSelectors": List[EventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EventSelectorUnionTypeDef = Union[EventSelectorTypeDef, EventSelectorOutputTypeDef]
 LookupEventsResponseTypeDef = TypedDict(
     "LookupEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1560,85 +1562,7 @@
         "Source": str,
         "SourceConfig": SourceConfigTypeDef,
         "Destinations": List[DestinationTypeDef],
         "IngestionStatus": IngestionStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "TagsList": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "StartIngestion": bool,
-    },
-    total=False,
-)
-
-
-class CreateEventDataStoreRequestRequestTypeDef(
-    _RequiredCreateEventDataStoreRequestRequestTypeDef,
-    _OptionalCreateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
-    {
-        "EventDataStore": str,
-    },
-)
-_OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-
-class UpdateEventDataStoreRequestRequestTypeDef(
-    _RequiredUpdateEventDataStoreRequestRequestTypeDef,
-    _OptionalUpdateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEventSelectorsRequestRequestTypeDef",
-    {
-        "TrailName": str,
-    },
-)
-_OptionalPutEventSelectorsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEventSelectorsRequestRequestTypeDef",
-    {
-        "EventSelectors": Sequence[EventSelectorUnionTypeDef],
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
-    },
-    total=False,
-)
-
-
-class PutEventSelectorsRequestRequestTypeDef(
-    _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail/type_defs.pyi` & `types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -34,21 +34,19 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "AdvancedFieldSelectorOutputTypeDef",
     "AdvancedFieldSelectorTypeDef",
     "CancelQueryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "ChannelTypeDef",
     "DestinationTypeDef",
-    "DataResourceOutputTypeDef",
     "DataResourceTypeDef",
     "DeleteChannelRequestRequestTypeDef",
     "DeleteEventDataStoreRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteTrailRequestRequestTypeDef",
     "DeregisterOrganizationDelegatedAdminRequestRequestTypeDef",
     "DescribeQueryRequestRequestTypeDef",
@@ -94,29 +92,27 @@
     "StopImportRequestRequestTypeDef",
     "StopLoggingRequestRequestTypeDef",
     "UpdateTrailRequestRequestTypeDef",
     "AddTagsRequestRequestTypeDef",
     "CreateTrailRequestRequestTypeDef",
     "RemoveTagsRequestRequestTypeDef",
     "ResourceTagTypeDef",
-    "AdvancedEventSelectorOutputTypeDef",
     "AdvancedEventSelectorTypeDef",
     "CancelQueryResponseTypeDef",
     "CreateTrailResponseTypeDef",
     "GetResourcePolicyResponseTypeDef",
     "GetTrailStatusResponseTypeDef",
     "PutResourcePolicyResponseTypeDef",
     "StartQueryResponseTypeDef",
     "UpdateTrailResponseTypeDef",
     "ListChannelsResponseTypeDef",
     "CreateChannelRequestRequestTypeDef",
     "CreateChannelResponseTypeDef",
     "UpdateChannelRequestRequestTypeDef",
     "UpdateChannelResponseTypeDef",
-    "EventSelectorOutputTypeDef",
     "EventSelectorTypeDef",
     "DescribeQueryResponseTypeDef",
     "DescribeTrailsResponseTypeDef",
     "GetTrailResponseTypeDef",
     "EventTypeDef",
     "GetInsightSelectorsResponseTypeDef",
     "PutInsightSelectorsRequestRequestTypeDef",
@@ -134,34 +130,32 @@
     "ListQueriesRequestRequestTypeDef",
     "ListPublicKeysResponseTypeDef",
     "ListQueriesResponseTypeDef",
     "ListTrailsResponseTypeDef",
     "LookupEventsRequestLookupEventsPaginateTypeDef",
     "LookupEventsRequestRequestTypeDef",
     "ListTagsResponseTypeDef",
+    "CreateEventDataStoreRequestRequestTypeDef",
     "CreateEventDataStoreResponseTypeDef",
     "EventDataStoreTypeDef",
     "GetEventDataStoreResponseTypeDef",
     "RestoreEventDataStoreResponseTypeDef",
     "SourceConfigTypeDef",
+    "UpdateEventDataStoreRequestRequestTypeDef",
     "UpdateEventDataStoreResponseTypeDef",
-    "AdvancedEventSelectorUnionTypeDef",
     "GetEventSelectorsResponseTypeDef",
+    "PutEventSelectorsRequestRequestTypeDef",
     "PutEventSelectorsResponseTypeDef",
-    "EventSelectorUnionTypeDef",
     "LookupEventsResponseTypeDef",
     "GetImportResponseTypeDef",
     "StartImportRequestRequestTypeDef",
     "StartImportResponseTypeDef",
     "StopImportResponseTypeDef",
     "ListEventDataStoresResponseTypeDef",
     "GetChannelResponseTypeDef",
-    "CreateEventDataStoreRequestRequestTypeDef",
-    "UpdateEventDataStoreRequestRequestTypeDef",
-    "PutEventSelectorsRequestRequestTypeDef",
 )
 
 _RequiredTagTypeDef = TypedDict(
     "_RequiredTagTypeDef",
     {
         "Key": str,
     },
@@ -173,38 +167,14 @@
     },
     total=False,
 )
 
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
     pass
 
-_RequiredAdvancedFieldSelectorOutputTypeDef = TypedDict(
-    "_RequiredAdvancedFieldSelectorOutputTypeDef",
-    {
-        "Field": str,
-    },
-)
-_OptionalAdvancedFieldSelectorOutputTypeDef = TypedDict(
-    "_OptionalAdvancedFieldSelectorOutputTypeDef",
-    {
-        "Equals": List[str],
-        "StartsWith": List[str],
-        "EndsWith": List[str],
-        "NotEquals": List[str],
-        "NotStartsWith": List[str],
-        "NotEndsWith": List[str],
-    },
-    total=False,
-)
-
-class AdvancedFieldSelectorOutputTypeDef(
-    _RequiredAdvancedFieldSelectorOutputTypeDef, _OptionalAdvancedFieldSelectorOutputTypeDef
-):
-    pass
-
 _RequiredAdvancedFieldSelectorTypeDef = TypedDict(
     "_RequiredAdvancedFieldSelectorTypeDef",
     {
         "Field": str,
     },
 )
 _OptionalAdvancedFieldSelectorTypeDef = TypedDict(
@@ -268,28 +238,19 @@
     "DestinationTypeDef",
     {
         "Type": DestinationTypeType,
         "Location": str,
     },
 )
 
-DataResourceOutputTypeDef = TypedDict(
-    "DataResourceOutputTypeDef",
-    {
-        "Type": str,
-        "Values": List[str],
-    },
-    total=False,
-)
-
 DataResourceTypeDef = TypedDict(
     "DataResourceTypeDef",
     {
         "Type": str,
-        "Values": Sequence[str],
+        "Values": List[str],
     },
     total=False,
 )
 
 DeleteChannelRequestRequestTypeDef = TypedDict(
     "DeleteChannelRequestRequestTypeDef",
     {
@@ -813,33 +774,14 @@
     {
         "ResourceId": str,
         "TagsList": List[TagTypeDef],
     },
     total=False,
 )
 
-_RequiredAdvancedEventSelectorOutputTypeDef = TypedDict(
-    "_RequiredAdvancedEventSelectorOutputTypeDef",
-    {
-        "FieldSelectors": List[AdvancedFieldSelectorOutputTypeDef],
-    },
-)
-_OptionalAdvancedEventSelectorOutputTypeDef = TypedDict(
-    "_OptionalAdvancedEventSelectorOutputTypeDef",
-    {
-        "Name": str,
-    },
-    total=False,
-)
-
-class AdvancedEventSelectorOutputTypeDef(
-    _RequiredAdvancedEventSelectorOutputTypeDef, _OptionalAdvancedEventSelectorOutputTypeDef
-):
-    pass
-
 _RequiredAdvancedEventSelectorTypeDef = TypedDict(
     "_RequiredAdvancedEventSelectorTypeDef",
     {
         "FieldSelectors": Sequence[AdvancedFieldSelectorTypeDef],
     },
 )
 _OptionalAdvancedEventSelectorTypeDef = TypedDict(
@@ -1023,32 +965,21 @@
         "Name": str,
         "Source": str,
         "Destinations": List[DestinationTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EventSelectorOutputTypeDef = TypedDict(
-    "EventSelectorOutputTypeDef",
-    {
-        "ReadWriteType": ReadWriteTypeType,
-        "IncludeManagementEvents": bool,
-        "DataResources": List[DataResourceOutputTypeDef],
-        "ExcludeManagementEventSources": List[str],
-    },
-    total=False,
-)
-
 EventSelectorTypeDef = TypedDict(
     "EventSelectorTypeDef",
     {
         "ReadWriteType": ReadWriteTypeType,
         "IncludeManagementEvents": bool,
-        "DataResources": Sequence[DataResourceTypeDef],
-        "ExcludeManagementEventSources": Sequence[str],
+        "DataResources": List[DataResourceTypeDef],
+        "ExcludeManagementEventSources": List[str],
     },
     total=False,
 )
 
 DescribeQueryResponseTypeDef = TypedDict(
     "DescribeQueryResponseTypeDef",
     {
@@ -1315,21 +1246,48 @@
     {
         "ResourceTagList": List[ResourceTagTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
+    {
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "TagsList": Sequence[TagTypeDef],
+        "KmsKeyId": str,
+        "StartIngestion": bool,
+    },
+    total=False,
+)
+
+class CreateEventDataStoreRequestRequestTypeDef(
+    _RequiredCreateEventDataStoreRequestRequestTypeDef,
+    _OptionalCreateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
 CreateEventDataStoreResponseTypeDef = TypedDict(
     "CreateEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "TagsList": List[TagTypeDef],
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
@@ -1341,15 +1299,15 @@
 EventDataStoreTypeDef = TypedDict(
     "EventDataStoreTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "TerminationProtectionEnabled": bool,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
     },
     total=False,
@@ -1357,15 +1315,15 @@
 
 GetEventDataStoreResponseTypeDef = TypedDict(
     "GetEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
@@ -1375,15 +1333,15 @@
 
 RestoreEventDataStoreResponseTypeDef = TypedDict(
     "RestoreEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
@@ -1391,61 +1349,103 @@
     },
 )
 
 SourceConfigTypeDef = TypedDict(
     "SourceConfigTypeDef",
     {
         "ApplyToAllRegions": bool,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
     },
     total=False,
 )
 
+_RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
+    {
+        "EventDataStore": str,
+    },
+)
+_OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateEventDataStoreRequestRequestTypeDef",
+    {
+        "Name": str,
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
+        "MultiRegionEnabled": bool,
+        "OrganizationEnabled": bool,
+        "RetentionPeriod": int,
+        "TerminationProtectionEnabled": bool,
+        "KmsKeyId": str,
+    },
+    total=False,
+)
+
+class UpdateEventDataStoreRequestRequestTypeDef(
+    _RequiredUpdateEventDataStoreRequestRequestTypeDef,
+    _OptionalUpdateEventDataStoreRequestRequestTypeDef,
+):
+    pass
+
 UpdateEventDataStoreResponseTypeDef = TypedDict(
     "UpdateEventDataStoreResponseTypeDef",
     {
         "EventDataStoreArn": str,
         "Name": str,
         "Status": EventDataStoreStatusType,
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "MultiRegionEnabled": bool,
         "OrganizationEnabled": bool,
         "RetentionPeriod": int,
         "TerminationProtectionEnabled": bool,
         "CreatedTimestamp": datetime,
         "UpdatedTimestamp": datetime,
         "KmsKeyId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AdvancedEventSelectorUnionTypeDef = Union[
-    AdvancedEventSelectorTypeDef, AdvancedEventSelectorOutputTypeDef
-]
 GetEventSelectorsResponseTypeDef = TypedDict(
     "GetEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "EventSelectors": List[EventSelectorOutputTypeDef],
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "EventSelectors": List[EventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEventSelectorsRequestRequestTypeDef",
+    {
+        "TrailName": str,
+    },
+)
+_OptionalPutEventSelectorsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEventSelectorsRequestRequestTypeDef",
+    {
+        "EventSelectors": Sequence[EventSelectorTypeDef],
+        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorTypeDef],
+    },
+    total=False,
+)
+
+class PutEventSelectorsRequestRequestTypeDef(
+    _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
+):
+    pass
+
 PutEventSelectorsResponseTypeDef = TypedDict(
     "PutEventSelectorsResponseTypeDef",
     {
         "TrailARN": str,
-        "EventSelectors": List[EventSelectorOutputTypeDef],
-        "AdvancedEventSelectors": List[AdvancedEventSelectorOutputTypeDef],
+        "EventSelectors": List[EventSelectorTypeDef],
+        "AdvancedEventSelectors": List[AdvancedEventSelectorTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EventSelectorUnionTypeDef = Union[EventSelectorTypeDef, EventSelectorOutputTypeDef]
 LookupEventsResponseTypeDef = TypedDict(
     "LookupEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -1527,80 +1527,7 @@
         "Source": str,
         "SourceConfig": SourceConfigTypeDef,
         "Destinations": List[DestinationTypeDef],
         "IngestionStatus": IngestionStatusTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-
-_RequiredCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalCreateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateEventDataStoreRequestRequestTypeDef",
-    {
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "TagsList": Sequence[TagTypeDef],
-        "KmsKeyId": str,
-        "StartIngestion": bool,
-    },
-    total=False,
-)
-
-class CreateEventDataStoreRequestRequestTypeDef(
-    _RequiredCreateEventDataStoreRequestRequestTypeDef,
-    _OptionalCreateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
-_RequiredUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateEventDataStoreRequestRequestTypeDef",
-    {
-        "EventDataStore": str,
-    },
-)
-_OptionalUpdateEventDataStoreRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateEventDataStoreRequestRequestTypeDef",
-    {
-        "Name": str,
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
-        "MultiRegionEnabled": bool,
-        "OrganizationEnabled": bool,
-        "RetentionPeriod": int,
-        "TerminationProtectionEnabled": bool,
-        "KmsKeyId": str,
-    },
-    total=False,
-)
-
-class UpdateEventDataStoreRequestRequestTypeDef(
-    _RequiredUpdateEventDataStoreRequestRequestTypeDef,
-    _OptionalUpdateEventDataStoreRequestRequestTypeDef,
-):
-    pass
-
-_RequiredPutEventSelectorsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEventSelectorsRequestRequestTypeDef",
-    {
-        "TrailName": str,
-    },
-)
-_OptionalPutEventSelectorsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEventSelectorsRequestRequestTypeDef",
-    {
-        "EventSelectors": Sequence[EventSelectorUnionTypeDef],
-        "AdvancedEventSelectors": Sequence[AdvancedEventSelectorUnionTypeDef],
-    },
-    total=False,
-)
-
-class PutEventSelectorsRequestRequestTypeDef(
-    _RequiredPutEventSelectorsRequestRequestTypeDef, _OptionalPutEventSelectorsRequestRequestTypeDef
-):
-    pass
```

### Comparing `types-aiobotocore-cloudtrail-2.5.2.post1/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt` & `types-aiobotocore-cloudtrail-2.5.2.post2/types_aiobotocore_cloudtrail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

