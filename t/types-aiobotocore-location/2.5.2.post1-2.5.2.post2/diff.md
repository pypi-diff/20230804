# Comparing `tmp/types-aiobotocore-location-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-location-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-location-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-location-2.5.2.post2.tar", last modified: Fri Aug  4 13:59:15 2023, max compression
```

## Comparing `types-aiobotocore-location-2.5.2.post1.tar` & `types-aiobotocore-location-2.5.2.post2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.633534 types-aiobotocore-location-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-08-02 14:52:35.629534 types-aiobotocore-location-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20050 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:35.633534 types-aiobotocore-location-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.625534 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47996 2023-08-02 14:42:26.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    47919 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-08-02 14:42:26.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-08-02 14:42:26.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12337 2023-08-02 14:42:26.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12325 2023-08-02 14:42:26.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    66009 2023-08-02 14:42:27.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65896 2023-08-02 14:42:26.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:25.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.629534 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21579 2023-08-02 14:52:35.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:52:35.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:35.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:35.000000 types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/top_level.txt
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.956643 types-aiobotocore-location-2.5.2.post2/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/LICENSE
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14372 2023-08-04 13:59:15.956643 types-aiobotocore-location-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12843 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/README.md
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-08-04 13:59:15.956643 types-aiobotocore-location-2.5.2.post2/setup.cfg
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2086 2023-08-04 13:43:15.000000 types-aiobotocore-location-2.5.2.post2/setup.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.946643 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2576 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/__init__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)     2575 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/__init__.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      961 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/__main__.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    48161 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/client.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    48084 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/client.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10376 2023-08-04 13:43:17.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/literals.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    10374 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/literals.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12337 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/paginator.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    12325 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/paginator.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/py.typed
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    65015 2023-08-04 13:43:18.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/type_defs.py
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    64904 2023-08-04 13:43:17.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/type_defs.pyi
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       65 2023-08-04 13:43:16.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/version.py
+drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-08-04 13:59:15.946643 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/
+-rw-r--r--   0 vlad      (1000) vlad      (1000)    14372 2023-08-04 13:59:15.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/PKG-INFO
+-rw-r--r--   0 vlad      (1000) vlad      (1000)      832 2023-08-04 13:59:15.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/SOURCES.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/dependency_links.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-08-04 13:59:15.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/not-zip-safe
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-08-04 13:59:15.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/requires.txt
+-rw-r--r--   0 vlad      (1000) vlad      (1000)       27 2023-08-04 13:59:15.000000 types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-location-2.5.2.post1/LICENSE` & `types-aiobotocore-location-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post1/setup.py` & `types-aiobotocore-location-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-location",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_location"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LocationService 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/__init__.py` & `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/__init__.pyi` & `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/__main__.py` & `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.LocationService 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService\nOther"
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

### Comparing `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/client.py` & `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     ListPlaceIndexesPaginator,
     ListRouteCalculatorsPaginator,
     ListTrackerConsumersPaginator,
     ListTrackersPaginator,
 )
 from .type_defs import (
     ApiKeyFilterTypeDef,
-    ApiKeyRestrictionsUnionTypeDef,
+    ApiKeyRestrictionsTypeDef,
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
@@ -57,15 +57,15 @@
     DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyResponseTypeDef,
     DescribeMapResponseTypeDef,
     DescribePlaceIndexResponseTypeDef,
     DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerResponseTypeDef,
     DevicePositionUpdateTypeDef,
-    GeofenceGeometryUnionTypeDef,
+    GeofenceGeometryTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     GetDevicePositionResponseTypeDef,
     GetGeofenceResponseTypeDef,
     GetMapGlyphsResponseTypeDef,
     GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorResponseTypeDef,
     GetMapTileResponseTypeDef,
@@ -221,14 +221,15 @@
         DeparturePosition: Sequence[float],
         DestinationPosition: Sequence[float],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
         DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         IncludeLegGeometry: bool = ...,
+        Key: str = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,
         WaypointPositions: Sequence[Sequence[float]] = ...
     ) -> CalculateRouteResponseTypeDef:
         """
         [Calculates a
         route](https://docs.aws.amazon.com/location/latest/developerguide/calculate-
@@ -245,14 +246,15 @@
         CalculatorName: str,
         DeparturePositions: Sequence[Sequence[float]],
         DestinationPositions: Sequence[Sequence[float]],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
         DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
+        Key: str = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...
     ) -> CalculateRouteMatrixResponseTypeDef:
         """
         [Calculates a route
         matrix](https://docs.aws.amazon.com/location/latest/developerguide/calculate-
         route-matrix.html)_ given the following required parameters:
@@ -295,24 +297,23 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#create_geofence_collection)
         """
 
     async def create_key(
         self,
         *,
         KeyName: str,
-        Restrictions: ApiKeyRestrictionsUnionTypeDef,
+        Restrictions: ApiKeyRestrictionsTypeDef,
         Description: str = ...,
         ExpireTime: TimestampTypeDef = ...,
         NoExpiry: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateKeyResponseTypeDef:
         """
         Creates an API key resource in your Amazon Web Services account, which lets you
-        grant `geo:GetMap*` actions for Amazon Location Map resources to the API key
-        bearer.
+        grant actions for Amazon Location resources to the API key bearer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#create_key)
         """
 
     async def create_map(
         self,
@@ -365,14 +366,15 @@
         """
 
     async def create_tracker(
         self,
         *,
         TrackerName: str,
         Description: str = ...,
+        EventBridgeEnabled: bool = ...,
         KmsKeyId: str = ...,
         PositionFiltering: PositionFilteringType = ...,
         PricingPlan: PricingPlanType = ...,
         PricingPlanDataSource: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateTrackerResponseTypeDef:
         """
@@ -582,15 +584,15 @@
         Retrieves a vector data tile from the map resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_map_tile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#get_map_tile)
         """
 
     async def get_place(
-        self, *, IndexName: str, PlaceId: str, Language: str = ...
+        self, *, IndexName: str, PlaceId: str, Key: str = ..., Language: str = ...
     ) -> GetPlaceResponseTypeDef:
         """
         Finds a place by its unique ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_place)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#get_place)
         """
@@ -697,15 +699,15 @@
         """
 
     async def put_geofence(
         self,
         *,
         CollectionName: str,
         GeofenceId: str,
-        Geometry: GeofenceGeometryUnionTypeDef,
+        Geometry: GeofenceGeometryTypeDef,
         GeofenceProperties: Mapping[str, str] = ...
     ) -> PutGeofenceResponseTypeDef:
         """
         Stores a geofence geometry in a given geofence collection, or updates the
         geometry of an existing geofence if a geofence ID is included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.put_geofence)
@@ -713,14 +715,15 @@
         """
 
     async def search_place_index_for_position(
         self,
         *,
         IndexName: str,
         Position: Sequence[float],
+        Key: str = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForPositionResponseTypeDef:
         """
         Reverse geocodes a given coordinate and returns a legible address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.search_place_index_for_position)
@@ -732,14 +735,15 @@
         *,
         IndexName: str,
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
         FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
+        Key: str = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForSuggestionsResponseTypeDef:
         """
         Generates suggestions for addresses and points of interest based on partial or
         misspelled free-form text.
 
@@ -752,14 +756,15 @@
         *,
         IndexName: str,
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
         FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
+        Key: str = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForTextResponseTypeDef:
         """
         Geocodes free-form text, such as an address, name, city, or region to allow you
         to search for Places or points of interest.
 
@@ -803,15 +808,15 @@
         self,
         *,
         KeyName: str,
         Description: str = ...,
         ExpireTime: TimestampTypeDef = ...,
         ForceUpdate: bool = ...,
         NoExpiry: bool = ...,
-        Restrictions: ApiKeyRestrictionsUnionTypeDef = ...
+        Restrictions: ApiKeyRestrictionsTypeDef = ...
     ) -> UpdateKeyResponseTypeDef:
         """
         Updates the specified properties of a given API key resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_key)
         """
@@ -857,14 +862,15 @@
         """
 
     async def update_tracker(
         self,
         *,
         TrackerName: str,
         Description: str = ...,
+        EventBridgeEnabled: bool = ...,
         PositionFiltering: PositionFilteringType = ...,
         PricingPlan: PricingPlanType = ...,
         PricingPlanDataSource: str = ...
     ) -> UpdateTrackerResponseTypeDef:
         """
         Updates the specified properties of a given tracker resource.
```

### Comparing `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/client.pyi` & `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     ListPlaceIndexesPaginator,
     ListRouteCalculatorsPaginator,
     ListTrackerConsumersPaginator,
     ListTrackersPaginator,
 )
 from .type_defs import (
     ApiKeyFilterTypeDef,
-    ApiKeyRestrictionsUnionTypeDef,
+    ApiKeyRestrictionsTypeDef,
     BatchDeleteDevicePositionHistoryResponseTypeDef,
     BatchDeleteGeofenceResponseTypeDef,
     BatchEvaluateGeofencesResponseTypeDef,
     BatchGetDevicePositionResponseTypeDef,
     BatchPutGeofenceRequestEntryTypeDef,
     BatchPutGeofenceResponseTypeDef,
     BatchUpdateDevicePositionResponseTypeDef,
@@ -57,15 +57,15 @@
     DescribeGeofenceCollectionResponseTypeDef,
     DescribeKeyResponseTypeDef,
     DescribeMapResponseTypeDef,
     DescribePlaceIndexResponseTypeDef,
     DescribeRouteCalculatorResponseTypeDef,
     DescribeTrackerResponseTypeDef,
     DevicePositionUpdateTypeDef,
-    GeofenceGeometryUnionTypeDef,
+    GeofenceGeometryTypeDef,
     GetDevicePositionHistoryResponseTypeDef,
     GetDevicePositionResponseTypeDef,
     GetGeofenceResponseTypeDef,
     GetMapGlyphsResponseTypeDef,
     GetMapSpritesResponseTypeDef,
     GetMapStyleDescriptorResponseTypeDef,
     GetMapTileResponseTypeDef,
@@ -209,14 +209,15 @@
         DeparturePosition: Sequence[float],
         DestinationPosition: Sequence[float],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
         DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
         IncludeLegGeometry: bool = ...,
+        Key: str = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...,
         WaypointPositions: Sequence[Sequence[float]] = ...
     ) -> CalculateRouteResponseTypeDef:
         """
         [Calculates a
         route](https://docs.aws.amazon.com/location/latest/developerguide/calculate-
@@ -232,14 +233,15 @@
         CalculatorName: str,
         DeparturePositions: Sequence[Sequence[float]],
         DestinationPositions: Sequence[Sequence[float]],
         CarModeOptions: CalculateRouteCarModeOptionsTypeDef = ...,
         DepartNow: bool = ...,
         DepartureTime: TimestampTypeDef = ...,
         DistanceUnit: DistanceUnitType = ...,
+        Key: str = ...,
         TravelMode: TravelModeType = ...,
         TruckModeOptions: CalculateRouteTruckModeOptionsTypeDef = ...
     ) -> CalculateRouteMatrixResponseTypeDef:
         """
         [Calculates a route
         matrix](https://docs.aws.amazon.com/location/latest/developerguide/calculate-
         route-matrix.html)_ given the following required parameters:
@@ -278,24 +280,23 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_geofence_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#create_geofence_collection)
         """
     async def create_key(
         self,
         *,
         KeyName: str,
-        Restrictions: ApiKeyRestrictionsUnionTypeDef,
+        Restrictions: ApiKeyRestrictionsTypeDef,
         Description: str = ...,
         ExpireTime: TimestampTypeDef = ...,
         NoExpiry: bool = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateKeyResponseTypeDef:
         """
         Creates an API key resource in your Amazon Web Services account, which lets you
-        grant `geo:GetMap*` actions for Amazon Location Map resources to the API key
-        bearer.
+        grant actions for Amazon Location resources to the API key bearer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.create_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#create_key)
         """
     async def create_map(
         self,
         *,
@@ -344,14 +345,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#create_route_calculator)
         """
     async def create_tracker(
         self,
         *,
         TrackerName: str,
         Description: str = ...,
+        EventBridgeEnabled: bool = ...,
         KmsKeyId: str = ...,
         PositionFiltering: PositionFilteringType = ...,
         PricingPlan: PricingPlanType = ...,
         PricingPlanDataSource: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateTrackerResponseTypeDef:
         """
@@ -539,15 +541,15 @@
         """
         Retrieves a vector data tile from the map resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_map_tile)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#get_map_tile)
         """
     async def get_place(
-        self, *, IndexName: str, PlaceId: str, Language: str = ...
+        self, *, IndexName: str, PlaceId: str, Key: str = ..., Language: str = ...
     ) -> GetPlaceResponseTypeDef:
         """
         Finds a place by its unique ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.get_place)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#get_place)
         """
@@ -643,29 +645,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#list_trackers)
         """
     async def put_geofence(
         self,
         *,
         CollectionName: str,
         GeofenceId: str,
-        Geometry: GeofenceGeometryUnionTypeDef,
+        Geometry: GeofenceGeometryTypeDef,
         GeofenceProperties: Mapping[str, str] = ...
     ) -> PutGeofenceResponseTypeDef:
         """
         Stores a geofence geometry in a given geofence collection, or updates the
         geometry of an existing geofence if a geofence ID is included in the request.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.put_geofence)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#put_geofence)
         """
     async def search_place_index_for_position(
         self,
         *,
         IndexName: str,
         Position: Sequence[float],
+        Key: str = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForPositionResponseTypeDef:
         """
         Reverse geocodes a given coordinate and returns a legible address.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.search_place_index_for_position)
@@ -676,14 +679,15 @@
         *,
         IndexName: str,
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
         FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
+        Key: str = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForSuggestionsResponseTypeDef:
         """
         Generates suggestions for addresses and points of interest based on partial or
         misspelled free-form text.
 
@@ -695,14 +699,15 @@
         *,
         IndexName: str,
         Text: str,
         BiasPosition: Sequence[float] = ...,
         FilterBBox: Sequence[float] = ...,
         FilterCategories: Sequence[str] = ...,
         FilterCountries: Sequence[str] = ...,
+        Key: str = ...,
         Language: str = ...,
         MaxResults: int = ...
     ) -> SearchPlaceIndexForTextResponseTypeDef:
         """
         Geocodes free-form text, such as an address, name, city, or region to allow you
         to search for Places or points of interest.
 
@@ -742,15 +747,15 @@
         self,
         *,
         KeyName: str,
         Description: str = ...,
         ExpireTime: TimestampTypeDef = ...,
         ForceUpdate: bool = ...,
         NoExpiry: bool = ...,
-        Restrictions: ApiKeyRestrictionsUnionTypeDef = ...
+        Restrictions: ApiKeyRestrictionsTypeDef = ...
     ) -> UpdateKeyResponseTypeDef:
         """
         Updates the specified properties of a given API key resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/location.html#LocationService.Client.update_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_key)
         """
@@ -792,14 +797,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_location/client/#update_route_calculator)
         """
     async def update_tracker(
         self,
         *,
         TrackerName: str,
         Description: str = ...,
+        EventBridgeEnabled: bool = ...,
         PositionFiltering: PositionFilteringType = ...,
         PricingPlan: PricingPlanType = ...,
         PricingPlanDataSource: str = ...
     ) -> UpdateTrackerResponseTypeDef:
         """
         Updates the specified properties of a given tracker resource.
```

### Comparing `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/literals.py` & `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,14 +94,15 @@
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
@@ -197,14 +198,15 @@
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
@@ -283,26 +285,28 @@
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

### Comparing `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/literals.pyi` & `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/literals.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -92,14 +92,15 @@
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
@@ -195,14 +196,15 @@
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
@@ -281,26 +283,28 @@
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

### Comparing `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/paginator.py` & `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/paginator.pyi` & `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/type_defs.py` & `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,30 +34,28 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ApiKeyFilterTypeDef",
-    "ApiKeyRestrictionsOutputTypeDef",
     "ApiKeyRestrictionsTypeDef",
     "AssociateTrackerConsumerRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionRequestRequestTypeDef",
     "BatchPutGeofenceSuccessTypeDef",
     "CalculateRouteCarModeOptionsTypeDef",
     "TimestampTypeDef",
     "CalculateRouteMatrixSummaryTypeDef",
     "CalculateRouteSummaryTypeDef",
     "TruckDimensionsTypeDef",
     "TruckWeightTypeDef",
-    "CircleOutputTypeDef",
     "CircleTypeDef",
     "CreateGeofenceCollectionRequestRequestTypeDef",
     "MapConfigurationTypeDef",
     "DataSourceConfigurationTypeDef",
     "CreateRouteCalculatorRequestRequestTypeDef",
     "CreateTrackerRequestRequestTypeDef",
     "DeleteGeofenceCollectionRequestRequestTypeDef",
@@ -112,15 +110,14 @@
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGeofenceCollectionRequestRequestTypeDef",
     "UpdateRouteCalculatorRequestRequestTypeDef",
     "UpdateTrackerRequestRequestTypeDef",
     "ListKeysRequestRequestTypeDef",
     "ListKeysResponseEntryTypeDef",
-    "ApiKeyRestrictionsUnionTypeDef",
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     "BatchDeleteGeofenceErrorTypeDef",
     "BatchEvaluateGeofencesErrorTypeDef",
     "BatchGetDevicePositionErrorTypeDef",
     "BatchPutGeofenceErrorTypeDef",
     "BatchUpdateDevicePositionErrorTypeDef",
     "CreateGeofenceCollectionResponseTypeDef",
@@ -146,15 +143,14 @@
     "UpdatePlaceIndexResponseTypeDef",
     "UpdateRouteCalculatorResponseTypeDef",
     "UpdateTrackerResponseTypeDef",
     "CreateKeyRequestRequestTypeDef",
     "GetDevicePositionHistoryRequestRequestTypeDef",
     "UpdateKeyRequestRequestTypeDef",
     "CalculateRouteTruckModeOptionsTypeDef",
-    "GeofenceGeometryOutputTypeDef",
     "GeofenceGeometryTypeDef",
     "CreateMapRequestRequestTypeDef",
     "DescribeMapResponseTypeDef",
     "CreatePlaceIndexRequestRequestTypeDef",
     "DescribePlaceIndexResponseTypeDef",
     "UpdatePlaceIndexRequestRequestTypeDef",
     "DevicePositionTypeDef",
@@ -185,65 +181,42 @@
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     "BatchDeleteGeofenceResponseTypeDef",
     "BatchEvaluateGeofencesResponseTypeDef",
     "BatchPutGeofenceResponseTypeDef",
     "BatchUpdateDevicePositionResponseTypeDef",
     "CalculateRouteMatrixRequestRequestTypeDef",
     "CalculateRouteRequestRequestTypeDef",
+    "BatchPutGeofenceRequestEntryTypeDef",
     "GetGeofenceResponseTypeDef",
     "ListGeofenceResponseEntryTypeDef",
-    "BatchPutGeofenceRequestEntryTypeDef",
-    "GeofenceGeometryUnionTypeDef",
     "PutGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionResponseTypeDef",
     "GetDevicePositionHistoryResponseTypeDef",
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     "BatchUpdateDevicePositionRequestRequestTypeDef",
     "ListDevicePositionsResponseTypeDef",
     "CalculateRouteResponseTypeDef",
     "GetPlaceResponseTypeDef",
     "SearchForPositionResultTypeDef",
     "SearchForTextResultTypeDef",
     "CalculateRouteMatrixResponseTypeDef",
-    "ListGeofencesResponseTypeDef",
     "BatchPutGeofenceRequestRequestTypeDef",
+    "ListGeofencesResponseTypeDef",
     "SearchPlaceIndexForPositionResponseTypeDef",
     "SearchPlaceIndexForTextResponseTypeDef",
 )
 
 ApiKeyFilterTypeDef = TypedDict(
     "ApiKeyFilterTypeDef",
     {
         "KeyStatus": StatusType,
     },
     total=False,
 )
 
-_RequiredApiKeyRestrictionsOutputTypeDef = TypedDict(
-    "_RequiredApiKeyRestrictionsOutputTypeDef",
-    {
-        "AllowActions": List[str],
-        "AllowResources": List[str],
-    },
-)
-_OptionalApiKeyRestrictionsOutputTypeDef = TypedDict(
-    "_OptionalApiKeyRestrictionsOutputTypeDef",
-    {
-        "AllowReferers": List[str],
-    },
-    total=False,
-)
-
-
-class ApiKeyRestrictionsOutputTypeDef(
-    _RequiredApiKeyRestrictionsOutputTypeDef, _OptionalApiKeyRestrictionsOutputTypeDef
-):
-    pass
-
-
 _RequiredApiKeyRestrictionsTypeDef = TypedDict(
     "_RequiredApiKeyRestrictionsTypeDef",
     {
         "AllowActions": Sequence[str],
         "AllowResources": Sequence[str],
     },
 )
@@ -370,22 +343,14 @@
     {
         "Total": float,
         "Unit": VehicleWeightUnitType,
     },
     total=False,
 )
 
-CircleOutputTypeDef = TypedDict(
-    "CircleOutputTypeDef",
-    {
-        "Center": List[float],
-        "Radius": float,
-    },
-)
-
 CircleTypeDef = TypedDict(
     "CircleTypeDef",
     {
         "Center": Sequence[float],
         "Radius": float,
     },
 )
@@ -474,14 +439,15 @@
         "TrackerName": str,
     },
 )
 _OptionalCreateTrackerRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTrackerRequestRequestTypeDef",
     {
         "Description": str,
+        "EventBridgeEnabled": bool,
         "KmsKeyId": str,
         "PositionFiltering": PositionFilteringType,
         "PricingPlan": PricingPlanType,
         "PricingPlanDataSource": str,
         "Tags": Mapping[str, str],
     },
     total=False,
@@ -716,14 +682,15 @@
         "IndexName": str,
         "PlaceId": str,
     },
 )
 _OptionalGetPlaceRequestRequestTypeDef = TypedDict(
     "_OptionalGetPlaceRequestRequestTypeDef",
     {
+        "Key": str,
         "Language": str,
     },
     total=False,
 )
 
 
 class GetPlaceRequestRequestTypeDef(
@@ -1094,14 +1061,15 @@
         "IndexName": str,
         "Position": Sequence[float],
     },
 )
 _OptionalSearchPlaceIndexForPositionRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForPositionRequestRequestTypeDef",
     {
+        "Key": str,
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 
@@ -1146,14 +1114,15 @@
 _OptionalSearchPlaceIndexForSuggestionsRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForSuggestionsRequestRequestTypeDef",
     {
         "BiasPosition": Sequence[float],
         "FilterBBox": Sequence[float],
         "FilterCategories": Sequence[str],
         "FilterCountries": Sequence[str],
+        "Key": str,
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 
@@ -1202,14 +1171,15 @@
 _OptionalSearchPlaceIndexForTextRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForTextRequestRequestTypeDef",
     {
         "BiasPosition": Sequence[float],
         "FilterBBox": Sequence[float],
         "FilterCategories": Sequence[str],
         "FilterCountries": Sequence[str],
+        "Key": str,
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 
@@ -1317,14 +1287,15 @@
         "TrackerName": str,
     },
 )
 _OptionalUpdateTrackerRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTrackerRequestRequestTypeDef",
     {
         "Description": str,
+        "EventBridgeEnabled": bool,
         "PositionFiltering": PositionFilteringType,
         "PricingPlan": PricingPlanType,
         "PricingPlanDataSource": str,
     },
     total=False,
 )
 
@@ -1347,15 +1318,15 @@
 
 _RequiredListKeysResponseEntryTypeDef = TypedDict(
     "_RequiredListKeysResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "ExpireTime": datetime,
         "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
         "UpdateTime": datetime,
     },
 )
 _OptionalListKeysResponseEntryTypeDef = TypedDict(
     "_OptionalListKeysResponseEntryTypeDef",
     {
         "Description": str,
@@ -1366,15 +1337,14 @@
 
 class ListKeysResponseEntryTypeDef(
     _RequiredListKeysResponseEntryTypeDef, _OptionalListKeysResponseEntryTypeDef
 ):
     pass
 
 
-ApiKeyRestrictionsUnionTypeDef = Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef]
 BatchDeleteDevicePositionHistoryErrorTypeDef = TypedDict(
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     {
         "DeviceId": str,
         "Error": BatchItemErrorTypeDef,
     },
 )
@@ -1503,15 +1473,15 @@
     {
         "CreateTime": datetime,
         "Description": str,
         "ExpireTime": datetime,
         "Key": str,
         "KeyArn": str,
         "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
         "Tags": Dict[str, str],
         "UpdateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRouteCalculatorResponseTypeDef = TypedDict(
@@ -1530,14 +1500,15 @@
 )
 
 DescribeTrackerResponseTypeDef = TypedDict(
     "DescribeTrackerResponseTypeDef",
     {
         "CreateTime": datetime,
         "Description": str,
+        "EventBridgeEnabled": bool,
         "KmsKeyId": str,
         "PositionFiltering": PositionFilteringType,
         "PricingPlan": PricingPlanType,
         "PricingPlanDataSource": str,
         "Tags": Dict[str, str],
         "TrackerArn": str,
         "TrackerName": str,
@@ -1756,23 +1727,14 @@
         "AvoidTolls": bool,
         "Dimensions": TruckDimensionsTypeDef,
         "Weight": TruckWeightTypeDef,
     },
     total=False,
 )
 
-GeofenceGeometryOutputTypeDef = TypedDict(
-    "GeofenceGeometryOutputTypeDef",
-    {
-        "Circle": CircleOutputTypeDef,
-        "Polygon": List[List[List[float]]],
-    },
-    total=False,
-)
-
 GeofenceGeometryTypeDef = TypedDict(
     "GeofenceGeometryTypeDef",
     {
         "Circle": CircleTypeDef,
         "Polygon": Sequence[Sequence[Sequence[float]]],
     },
     total=False,
@@ -2311,14 +2273,15 @@
 _OptionalCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_OptionalCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
         "DepartureTime": TimestampTypeDef,
         "DistanceUnit": DistanceUnitType,
+        "Key": str,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
     },
     total=False,
 )
 
 
@@ -2341,47 +2304,70 @@
     "_OptionalCalculateRouteRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
         "DepartureTime": TimestampTypeDef,
         "DistanceUnit": DistanceUnitType,
         "IncludeLegGeometry": bool,
+        "Key": str,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
         "WaypointPositions": Sequence[Sequence[float]],
     },
     total=False,
 )
 
 
 class CalculateRouteRequestRequestTypeDef(
     _RequiredCalculateRouteRequestRequestTypeDef, _OptionalCalculateRouteRequestRequestTypeDef
 ):
     pass
 
 
+_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceId": str,
+        "Geometry": GeofenceGeometryTypeDef,
+    },
+)
+_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class BatchPutGeofenceRequestEntryTypeDef(
+    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
+):
+    pass
+
+
 GetGeofenceResponseTypeDef = TypedDict(
     "GetGeofenceResponseTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
         "GeofenceProperties": Dict[str, str],
-        "Geometry": GeofenceGeometryOutputTypeDef,
+        "Geometry": GeofenceGeometryTypeDef,
         "Status": str,
         "UpdateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListGeofenceResponseEntryTypeDef = TypedDict(
     "_RequiredListGeofenceResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
-        "Geometry": GeofenceGeometryOutputTypeDef,
+        "Geometry": GeofenceGeometryTypeDef,
         "Status": str,
         "UpdateTime": datetime,
     },
 )
 _OptionalListGeofenceResponseEntryTypeDef = TypedDict(
     "_OptionalListGeofenceResponseEntryTypeDef",
     {
@@ -2393,37 +2379,14 @@
 
 class ListGeofenceResponseEntryTypeDef(
     _RequiredListGeofenceResponseEntryTypeDef, _OptionalListGeofenceResponseEntryTypeDef
 ):
     pass
 
 
-_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
-    {
-        "GeofenceId": str,
-        "Geometry": GeofenceGeometryTypeDef,
-    },
-)
-_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
-    {
-        "GeofenceProperties": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class BatchPutGeofenceRequestEntryTypeDef(
-    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
-):
-    pass
-
-
-GeofenceGeometryUnionTypeDef = Union[GeofenceGeometryTypeDef, GeofenceGeometryOutputTypeDef]
 _RequiredPutGeofenceRequestRequestTypeDef = TypedDict(
     "_RequiredPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
     },
@@ -2555,31 +2518,31 @@
         "SnappedDeparturePositions": List[List[float]],
         "SnappedDestinationPositions": List[List[float]],
         "Summary": CalculateRouteMatrixSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchPutGeofenceRequestRequestTypeDef = TypedDict(
+    "BatchPutGeofenceRequestRequestTypeDef",
+    {
+        "CollectionName": str,
+        "Entries": Sequence[BatchPutGeofenceRequestEntryTypeDef],
+    },
+)
+
 ListGeofencesResponseTypeDef = TypedDict(
     "ListGeofencesResponseTypeDef",
     {
         "Entries": List[ListGeofenceResponseEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutGeofenceRequestRequestTypeDef = TypedDict(
-    "BatchPutGeofenceRequestRequestTypeDef",
-    {
-        "CollectionName": str,
-        "Entries": Sequence[BatchPutGeofenceRequestEntryTypeDef],
-    },
-)
-
 SearchPlaceIndexForPositionResponseTypeDef = TypedDict(
     "SearchPlaceIndexForPositionResponseTypeDef",
     {
         "Results": List[SearchForPositionResultTypeDef],
         "Summary": SearchPlaceIndexForPositionSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location/type_defs.pyi` & `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -33,30 +33,28 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ApiKeyFilterTypeDef",
-    "ApiKeyRestrictionsOutputTypeDef",
     "ApiKeyRestrictionsTypeDef",
     "AssociateTrackerConsumerRequestRequestTypeDef",
     "BatchItemErrorTypeDef",
     "BatchDeleteDevicePositionHistoryRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "BatchDeleteGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionRequestRequestTypeDef",
     "BatchPutGeofenceSuccessTypeDef",
     "CalculateRouteCarModeOptionsTypeDef",
     "TimestampTypeDef",
     "CalculateRouteMatrixSummaryTypeDef",
     "CalculateRouteSummaryTypeDef",
     "TruckDimensionsTypeDef",
     "TruckWeightTypeDef",
-    "CircleOutputTypeDef",
     "CircleTypeDef",
     "CreateGeofenceCollectionRequestRequestTypeDef",
     "MapConfigurationTypeDef",
     "DataSourceConfigurationTypeDef",
     "CreateRouteCalculatorRequestRequestTypeDef",
     "CreateTrackerRequestRequestTypeDef",
     "DeleteGeofenceCollectionRequestRequestTypeDef",
@@ -111,15 +109,14 @@
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateGeofenceCollectionRequestRequestTypeDef",
     "UpdateRouteCalculatorRequestRequestTypeDef",
     "UpdateTrackerRequestRequestTypeDef",
     "ListKeysRequestRequestTypeDef",
     "ListKeysResponseEntryTypeDef",
-    "ApiKeyRestrictionsUnionTypeDef",
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     "BatchDeleteGeofenceErrorTypeDef",
     "BatchEvaluateGeofencesErrorTypeDef",
     "BatchGetDevicePositionErrorTypeDef",
     "BatchPutGeofenceErrorTypeDef",
     "BatchUpdateDevicePositionErrorTypeDef",
     "CreateGeofenceCollectionResponseTypeDef",
@@ -145,15 +142,14 @@
     "UpdatePlaceIndexResponseTypeDef",
     "UpdateRouteCalculatorResponseTypeDef",
     "UpdateTrackerResponseTypeDef",
     "CreateKeyRequestRequestTypeDef",
     "GetDevicePositionHistoryRequestRequestTypeDef",
     "UpdateKeyRequestRequestTypeDef",
     "CalculateRouteTruckModeOptionsTypeDef",
-    "GeofenceGeometryOutputTypeDef",
     "GeofenceGeometryTypeDef",
     "CreateMapRequestRequestTypeDef",
     "DescribeMapResponseTypeDef",
     "CreatePlaceIndexRequestRequestTypeDef",
     "DescribePlaceIndexResponseTypeDef",
     "UpdatePlaceIndexRequestRequestTypeDef",
     "DevicePositionTypeDef",
@@ -184,63 +180,42 @@
     "BatchDeleteDevicePositionHistoryResponseTypeDef",
     "BatchDeleteGeofenceResponseTypeDef",
     "BatchEvaluateGeofencesResponseTypeDef",
     "BatchPutGeofenceResponseTypeDef",
     "BatchUpdateDevicePositionResponseTypeDef",
     "CalculateRouteMatrixRequestRequestTypeDef",
     "CalculateRouteRequestRequestTypeDef",
+    "BatchPutGeofenceRequestEntryTypeDef",
     "GetGeofenceResponseTypeDef",
     "ListGeofenceResponseEntryTypeDef",
-    "BatchPutGeofenceRequestEntryTypeDef",
-    "GeofenceGeometryUnionTypeDef",
     "PutGeofenceRequestRequestTypeDef",
     "BatchGetDevicePositionResponseTypeDef",
     "GetDevicePositionHistoryResponseTypeDef",
     "BatchEvaluateGeofencesRequestRequestTypeDef",
     "BatchUpdateDevicePositionRequestRequestTypeDef",
     "ListDevicePositionsResponseTypeDef",
     "CalculateRouteResponseTypeDef",
     "GetPlaceResponseTypeDef",
     "SearchForPositionResultTypeDef",
     "SearchForTextResultTypeDef",
     "CalculateRouteMatrixResponseTypeDef",
-    "ListGeofencesResponseTypeDef",
     "BatchPutGeofenceRequestRequestTypeDef",
+    "ListGeofencesResponseTypeDef",
     "SearchPlaceIndexForPositionResponseTypeDef",
     "SearchPlaceIndexForTextResponseTypeDef",
 )
 
 ApiKeyFilterTypeDef = TypedDict(
     "ApiKeyFilterTypeDef",
     {
         "KeyStatus": StatusType,
     },
     total=False,
 )
 
-_RequiredApiKeyRestrictionsOutputTypeDef = TypedDict(
-    "_RequiredApiKeyRestrictionsOutputTypeDef",
-    {
-        "AllowActions": List[str],
-        "AllowResources": List[str],
-    },
-)
-_OptionalApiKeyRestrictionsOutputTypeDef = TypedDict(
-    "_OptionalApiKeyRestrictionsOutputTypeDef",
-    {
-        "AllowReferers": List[str],
-    },
-    total=False,
-)
-
-class ApiKeyRestrictionsOutputTypeDef(
-    _RequiredApiKeyRestrictionsOutputTypeDef, _OptionalApiKeyRestrictionsOutputTypeDef
-):
-    pass
-
 _RequiredApiKeyRestrictionsTypeDef = TypedDict(
     "_RequiredApiKeyRestrictionsTypeDef",
     {
         "AllowActions": Sequence[str],
         "AllowResources": Sequence[str],
     },
 )
@@ -365,22 +340,14 @@
     {
         "Total": float,
         "Unit": VehicleWeightUnitType,
     },
     total=False,
 )
 
-CircleOutputTypeDef = TypedDict(
-    "CircleOutputTypeDef",
-    {
-        "Center": List[float],
-        "Radius": float,
-    },
-)
-
 CircleTypeDef = TypedDict(
     "CircleTypeDef",
     {
         "Center": Sequence[float],
         "Radius": float,
     },
 )
@@ -463,14 +430,15 @@
         "TrackerName": str,
     },
 )
 _OptionalCreateTrackerRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTrackerRequestRequestTypeDef",
     {
         "Description": str,
+        "EventBridgeEnabled": bool,
         "KmsKeyId": str,
         "PositionFiltering": PositionFilteringType,
         "PricingPlan": PricingPlanType,
         "PricingPlanDataSource": str,
         "Tags": Mapping[str, str],
     },
     total=False,
@@ -695,14 +663,15 @@
         "IndexName": str,
         "PlaceId": str,
     },
 )
 _OptionalGetPlaceRequestRequestTypeDef = TypedDict(
     "_OptionalGetPlaceRequestRequestTypeDef",
     {
+        "Key": str,
         "Language": str,
     },
     total=False,
 )
 
 class GetPlaceRequestRequestTypeDef(
     _RequiredGetPlaceRequestRequestTypeDef, _OptionalGetPlaceRequestRequestTypeDef
@@ -1047,14 +1016,15 @@
         "IndexName": str,
         "Position": Sequence[float],
     },
 )
 _OptionalSearchPlaceIndexForPositionRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForPositionRequestRequestTypeDef",
     {
+        "Key": str,
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 class SearchPlaceIndexForPositionRequestRequestTypeDef(
@@ -1095,14 +1065,15 @@
 _OptionalSearchPlaceIndexForSuggestionsRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForSuggestionsRequestRequestTypeDef",
     {
         "BiasPosition": Sequence[float],
         "FilterBBox": Sequence[float],
         "FilterCategories": Sequence[str],
         "FilterCountries": Sequence[str],
+        "Key": str,
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 class SearchPlaceIndexForSuggestionsRequestRequestTypeDef(
@@ -1147,14 +1118,15 @@
 _OptionalSearchPlaceIndexForTextRequestRequestTypeDef = TypedDict(
     "_OptionalSearchPlaceIndexForTextRequestRequestTypeDef",
     {
         "BiasPosition": Sequence[float],
         "FilterBBox": Sequence[float],
         "FilterCategories": Sequence[str],
         "FilterCountries": Sequence[str],
+        "Key": str,
         "Language": str,
         "MaxResults": int,
     },
     total=False,
 )
 
 class SearchPlaceIndexForTextRequestRequestTypeDef(
@@ -1254,14 +1226,15 @@
         "TrackerName": str,
     },
 )
 _OptionalUpdateTrackerRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTrackerRequestRequestTypeDef",
     {
         "Description": str,
+        "EventBridgeEnabled": bool,
         "PositionFiltering": PositionFilteringType,
         "PricingPlan": PricingPlanType,
         "PricingPlanDataSource": str,
     },
     total=False,
 )
 
@@ -1282,15 +1255,15 @@
 
 _RequiredListKeysResponseEntryTypeDef = TypedDict(
     "_RequiredListKeysResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "ExpireTime": datetime,
         "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
         "UpdateTime": datetime,
     },
 )
 _OptionalListKeysResponseEntryTypeDef = TypedDict(
     "_OptionalListKeysResponseEntryTypeDef",
     {
         "Description": str,
@@ -1299,15 +1272,14 @@
 )
 
 class ListKeysResponseEntryTypeDef(
     _RequiredListKeysResponseEntryTypeDef, _OptionalListKeysResponseEntryTypeDef
 ):
     pass
 
-ApiKeyRestrictionsUnionTypeDef = Union[ApiKeyRestrictionsTypeDef, ApiKeyRestrictionsOutputTypeDef]
 BatchDeleteDevicePositionHistoryErrorTypeDef = TypedDict(
     "BatchDeleteDevicePositionHistoryErrorTypeDef",
     {
         "DeviceId": str,
         "Error": BatchItemErrorTypeDef,
     },
 )
@@ -1436,15 +1408,15 @@
     {
         "CreateTime": datetime,
         "Description": str,
         "ExpireTime": datetime,
         "Key": str,
         "KeyArn": str,
         "KeyName": str,
-        "Restrictions": ApiKeyRestrictionsOutputTypeDef,
+        "Restrictions": ApiKeyRestrictionsTypeDef,
         "Tags": Dict[str, str],
         "UpdateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRouteCalculatorResponseTypeDef = TypedDict(
@@ -1463,14 +1435,15 @@
 )
 
 DescribeTrackerResponseTypeDef = TypedDict(
     "DescribeTrackerResponseTypeDef",
     {
         "CreateTime": datetime,
         "Description": str,
+        "EventBridgeEnabled": bool,
         "KmsKeyId": str,
         "PositionFiltering": PositionFilteringType,
         "PricingPlan": PricingPlanType,
         "PricingPlanDataSource": str,
         "Tags": Dict[str, str],
         "TrackerArn": str,
         "TrackerName": str,
@@ -1683,23 +1656,14 @@
         "AvoidTolls": bool,
         "Dimensions": TruckDimensionsTypeDef,
         "Weight": TruckWeightTypeDef,
     },
     total=False,
 )
 
-GeofenceGeometryOutputTypeDef = TypedDict(
-    "GeofenceGeometryOutputTypeDef",
-    {
-        "Circle": CircleOutputTypeDef,
-        "Polygon": List[List[List[float]]],
-    },
-    total=False,
-)
-
 GeofenceGeometryTypeDef = TypedDict(
     "GeofenceGeometryTypeDef",
     {
         "Circle": CircleTypeDef,
         "Polygon": Sequence[Sequence[Sequence[float]]],
     },
     total=False,
@@ -2212,14 +2176,15 @@
 _OptionalCalculateRouteMatrixRequestRequestTypeDef = TypedDict(
     "_OptionalCalculateRouteMatrixRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
         "DepartureTime": TimestampTypeDef,
         "DistanceUnit": DistanceUnitType,
+        "Key": str,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
     },
     total=False,
 )
 
 class CalculateRouteMatrixRequestRequestTypeDef(
@@ -2240,45 +2205,66 @@
     "_OptionalCalculateRouteRequestRequestTypeDef",
     {
         "CarModeOptions": CalculateRouteCarModeOptionsTypeDef,
         "DepartNow": bool,
         "DepartureTime": TimestampTypeDef,
         "DistanceUnit": DistanceUnitType,
         "IncludeLegGeometry": bool,
+        "Key": str,
         "TravelMode": TravelModeType,
         "TruckModeOptions": CalculateRouteTruckModeOptionsTypeDef,
         "WaypointPositions": Sequence[Sequence[float]],
     },
     total=False,
 )
 
 class CalculateRouteRequestRequestTypeDef(
     _RequiredCalculateRouteRequestRequestTypeDef, _OptionalCalculateRouteRequestRequestTypeDef
 ):
     pass
 
+_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceId": str,
+        "Geometry": GeofenceGeometryTypeDef,
+    },
+)
+_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
+    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
+    {
+        "GeofenceProperties": Mapping[str, str],
+    },
+    total=False,
+)
+
+class BatchPutGeofenceRequestEntryTypeDef(
+    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
+):
+    pass
+
 GetGeofenceResponseTypeDef = TypedDict(
     "GetGeofenceResponseTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
         "GeofenceProperties": Dict[str, str],
-        "Geometry": GeofenceGeometryOutputTypeDef,
+        "Geometry": GeofenceGeometryTypeDef,
         "Status": str,
         "UpdateTime": datetime,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListGeofenceResponseEntryTypeDef = TypedDict(
     "_RequiredListGeofenceResponseEntryTypeDef",
     {
         "CreateTime": datetime,
         "GeofenceId": str,
-        "Geometry": GeofenceGeometryOutputTypeDef,
+        "Geometry": GeofenceGeometryTypeDef,
         "Status": str,
         "UpdateTime": datetime,
     },
 )
 _OptionalListGeofenceResponseEntryTypeDef = TypedDict(
     "_OptionalListGeofenceResponseEntryTypeDef",
     {
@@ -2288,35 +2274,14 @@
 )
 
 class ListGeofenceResponseEntryTypeDef(
     _RequiredListGeofenceResponseEntryTypeDef, _OptionalListGeofenceResponseEntryTypeDef
 ):
     pass
 
-_RequiredBatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "_RequiredBatchPutGeofenceRequestEntryTypeDef",
-    {
-        "GeofenceId": str,
-        "Geometry": GeofenceGeometryTypeDef,
-    },
-)
-_OptionalBatchPutGeofenceRequestEntryTypeDef = TypedDict(
-    "_OptionalBatchPutGeofenceRequestEntryTypeDef",
-    {
-        "GeofenceProperties": Mapping[str, str],
-    },
-    total=False,
-)
-
-class BatchPutGeofenceRequestEntryTypeDef(
-    _RequiredBatchPutGeofenceRequestEntryTypeDef, _OptionalBatchPutGeofenceRequestEntryTypeDef
-):
-    pass
-
-GeofenceGeometryUnionTypeDef = Union[GeofenceGeometryTypeDef, GeofenceGeometryOutputTypeDef]
 _RequiredPutGeofenceRequestRequestTypeDef = TypedDict(
     "_RequiredPutGeofenceRequestRequestTypeDef",
     {
         "CollectionName": str,
         "GeofenceId": str,
         "Geometry": GeofenceGeometryTypeDef,
     },
@@ -2442,31 +2407,31 @@
         "SnappedDeparturePositions": List[List[float]],
         "SnappedDestinationPositions": List[List[float]],
         "Summary": CalculateRouteMatrixSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+BatchPutGeofenceRequestRequestTypeDef = TypedDict(
+    "BatchPutGeofenceRequestRequestTypeDef",
+    {
+        "CollectionName": str,
+        "Entries": Sequence[BatchPutGeofenceRequestEntryTypeDef],
+    },
+)
+
 ListGeofencesResponseTypeDef = TypedDict(
     "ListGeofencesResponseTypeDef",
     {
         "Entries": List[ListGeofenceResponseEntryTypeDef],
         "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchPutGeofenceRequestRequestTypeDef = TypedDict(
-    "BatchPutGeofenceRequestRequestTypeDef",
-    {
-        "CollectionName": str,
-        "Entries": Sequence[BatchPutGeofenceRequestEntryTypeDef],
-    },
-)
-
 SearchPlaceIndexForPositionResponseTypeDef = TypedDict(
     "SearchPlaceIndexForPositionResponseTypeDef",
     {
         "Results": List[SearchForPositionResultTypeDef],
         "Summary": SearchPlaceIndexForPositionSummaryTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
```

### Comparing `types-aiobotocore-location-2.5.2.post1/types_aiobotocore_location.egg-info/SOURCES.txt` & `types-aiobotocore-location-2.5.2.post2/types_aiobotocore_location.egg-info/SOURCES.txt`

 * *Files identical despite different names*

