# Comparing `tmp/metar2bufr-0.0.2.37.tar.gz` & `tmp/metar2bufr-0.0.2.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metar2bufr-0.0.2.37.tar", last modified: Fri Aug  4 16:00:14 2023, max compression
+gzip compressed data, was "metar2bufr-0.0.2.38.tar", last modified: Fri Aug  4 19:00:38 2023, max compression
```

## Comparing `metar2bufr-0.0.2.37.tar` & `metar2bufr-0.0.2.38.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.321038 metar2bufr-0.0.2.37/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1073 2023-07-13 16:23:37.000000 metar2bufr-0.0.2.37/LICENSE
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       39 2023-07-13 22:22:45.000000 metar2bufr-0.0.2.37/MANIFEST.in
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-08-04 16:00:14.321038 metar2bufr-0.0.2.37/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       85 2023-07-13 16:24:38.000000 metar2bufr-0.0.2.37/README.md
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      764 2023-08-04 15:59:35.000000 metar2bufr-0.0.2.37/pyproject.toml
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-08-04 16:00:14.321038 metar2bufr-0.0.2.37/setup.cfg
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.314038 metar2bufr-0.0.2.37/src/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.316038 metar2bufr-0.0.2.37/src/metar2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      164 2023-07-13 20:54:01.000000 metar2bufr-0.0.2.37/src/metar2bufr/__init__.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.317038 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.314038 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/build/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.314038 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/build/lib/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.318038 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/build/lib/csv2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.318038 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/csv2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/csv2bufr/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/csv2bufr/cli.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.315038 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/docs/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.319038 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/docs/source/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3056 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/docs/source/conf.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3330 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/setup.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.319038 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/tests/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8502 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    26208 2023-07-26 21:53:12.000000 metar2bufr-0.0.2.37/src/metar2bufr/icao_bufr_encoder.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.320038 metar2bufr-0.0.2.37/src/metar2bufr/metarDecoder/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 17:15:28.000000 metar2bufr-0.0.2.37/src/metar2bufr/metarDecoder/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    59241 2023-07-13 20:20:04.000000 metar2bufr-0.0.2.37/src/metar2bufr/metarDecoder/metarDecoders.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    82209 2023-07-13 16:28:08.000000 metar2bufr-0.0.2.37/src/metar2bufr/metarDecoder/tpg.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8261 2023-07-13 16:28:19.000000 metar2bufr-0.0.2.37/src/metar2bufr/metarDecoder/xmlConfig.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     6620 2023-07-13 20:39:39.000000 metar2bufr-0.0.2.37/src/metar2bufr/metarDecoder/xmlUtilities.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    24305 2023-08-03 22:55:56.000000 metar2bufr-0.0.2.37/src/metar2bufr/metar_bufr_encoder.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.320038 metar2bufr-0.0.2.37/src/metar2bufr/resources/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 22:08:27.000000 metar2bufr-0.0.2.37/src/metar2bufr/resources/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2793 2023-07-20 23:18:14.000000 metar2bufr-0.0.2.37/src/metar2bufr/resources/icao-metar-mappings.json
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2825 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.37/src/metar2bufr/resources/metar-mappings.json
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3136 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.37/src/metar2bufr/resources/metar-mappings2.json
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 16:00:14.317038 metar2bufr-0.0.2.37/src/metar2bufr.egg-info/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-08-04 16:00:14.000000 metar2bufr-0.0.2.37/src/metar2bufr.egg-info/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1107 2023-08-04 16:00:14.000000 metar2bufr-0.0.2.37/src/metar2bufr.egg-info/SOURCES.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-08-04 16:00:14.000000 metar2bufr-0.0.2.37/src/metar2bufr.egg-info/dependency_links.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       11 2023-08-04 16:00:14.000000 metar2bufr-0.0.2.37/src/metar2bufr.egg-info/top_level.txt
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.412572 metar2bufr-0.0.2.38/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1073 2023-07-13 16:23:37.000000 metar2bufr-0.0.2.38/LICENSE
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       39 2023-07-13 22:22:45.000000 metar2bufr-0.0.2.38/MANIFEST.in
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-08-04 19:00:38.412572 metar2bufr-0.0.2.38/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       85 2023-07-13 16:24:38.000000 metar2bufr-0.0.2.38/README.md
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      764 2023-08-04 18:58:37.000000 metar2bufr-0.0.2.38/pyproject.toml
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-08-04 19:00:38.412572 metar2bufr-0.0.2.38/setup.cfg
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.405572 metar2bufr-0.0.2.38/src/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.408572 metar2bufr-0.0.2.38/src/metar2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      164 2023-07-13 20:54:01.000000 metar2bufr-0.0.2.38/src/metar2bufr/__init__.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.409572 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.406572 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/build/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.406572 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/build/lib/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.409572 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/build/lib/csv2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.410572 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/csv2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/csv2bufr/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/csv2bufr/cli.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.406572 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/docs/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.410572 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/docs/source/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3056 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/docs/source/conf.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3330 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/setup.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.410572 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/tests/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8502 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    26208 2023-07-26 21:53:12.000000 metar2bufr-0.0.2.38/src/metar2bufr/icao_bufr_encoder.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.411572 metar2bufr-0.0.2.38/src/metar2bufr/metarDecoder/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 17:15:28.000000 metar2bufr-0.0.2.38/src/metar2bufr/metarDecoder/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    59241 2023-07-13 20:20:04.000000 metar2bufr-0.0.2.38/src/metar2bufr/metarDecoder/metarDecoders.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    82209 2023-07-13 16:28:08.000000 metar2bufr-0.0.2.38/src/metar2bufr/metarDecoder/tpg.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8261 2023-07-13 16:28:19.000000 metar2bufr-0.0.2.38/src/metar2bufr/metarDecoder/xmlConfig.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     6620 2023-07-13 20:39:39.000000 metar2bufr-0.0.2.38/src/metar2bufr/metarDecoder/xmlUtilities.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    25055 2023-08-04 18:59:50.000000 metar2bufr-0.0.2.38/src/metar2bufr/metar_bufr_encoder.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.412572 metar2bufr-0.0.2.38/src/metar2bufr/resources/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 22:08:27.000000 metar2bufr-0.0.2.38/src/metar2bufr/resources/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2793 2023-07-20 23:18:14.000000 metar2bufr-0.0.2.38/src/metar2bufr/resources/icao-metar-mappings.json
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2825 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.38/src/metar2bufr/resources/metar-mappings.json
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3136 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.38/src/metar2bufr/resources/metar-mappings2.json
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-04 19:00:38.408572 metar2bufr-0.0.2.38/src/metar2bufr.egg-info/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-08-04 19:00:38.000000 metar2bufr-0.0.2.38/src/metar2bufr.egg-info/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1107 2023-08-04 19:00:38.000000 metar2bufr-0.0.2.38/src/metar2bufr.egg-info/SOURCES.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-08-04 19:00:38.000000 metar2bufr-0.0.2.38/src/metar2bufr.egg-info/dependency_links.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       11 2023-08-04 19:00:38.000000 metar2bufr-0.0.2.38/src/metar2bufr.egg-info/top_level.txt
```

### Comparing `metar2bufr-0.0.2.37/LICENSE` & `metar2bufr-0.0.2.38/LICENSE`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/PKG-INFO` & `metar2bufr-0.0.2.38/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar2bufr
-Version: 0.0.2.37
+Version: 0.0.2.38
 Summary: Package for converting METAR TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `metar2bufr-0.0.2.37/pyproject.toml` & `metar2bufr-0.0.2.38/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metar2bufr"
-version = "0.0.2.37"
+version = "0.0.2.38"
 authors = [
   { name="Alexander Thompson", email="alexander.thompson@noaa.gov" },
 ]
 description = "Package for converting METAR TAC messages or an individual METAR message to BUFR4"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py` & `metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py` & `metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py` & `metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/csv2bufr/__init__.py` & `metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/csv2bufr/__init__.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/csv2bufr/cli.py` & `metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/csv2bufr/cli.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py` & `metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/docs/source/conf.py` & `metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/setup.py` & `metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/setup.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py` & `metar2bufr-0.0.2.38/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/icao_bufr_encoder.py` & `metar2bufr-0.0.2.38/src/metar2bufr/icao_bufr_encoder.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/metarDecoder/metarDecoders.py` & `metar2bufr-0.0.2.38/src/metar2bufr/metarDecoder/metarDecoders.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/metarDecoder/tpg.py` & `metar2bufr-0.0.2.38/src/metar2bufr/metarDecoder/tpg.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/metarDecoder/xmlConfig.py` & `metar2bufr-0.0.2.38/src/metar2bufr/metarDecoder/xmlConfig.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/metarDecoder/xmlUtilities.py` & `metar2bufr-0.0.2.38/src/metar2bufr/metarDecoder/xmlUtilities.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/metar_bufr_encoder.py` & `metar2bufr-0.0.2.38/src/metar2bufr/metar_bufr_encoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,15 @@
     for i in range(len(data)):
         data[i] = data[i]+"="
 
     # print(data[:len(data)-1])
     return data[:len(data)-1]
 
 def parse_metar(message: str, year: int, month: int) -> dict:
+    print(f"Parsing message: {message}")
     icaoID = re_ID.match(message).group('id')
     if deu.isUSIdentifier(icaoID):
         decoded = fmh(message)
     else:
         decoded = annex3(message)
 
     for key in decoded:
@@ -386,14 +387,19 @@
 
         try:
             wsi = tsi_mapping[tsi]
         except Exception:
             conversion_success[tsi] = False
             LOGGER.warning(f"Station {tsi} not found in station file")
 
+            #   Question for Tom on how wigos mapping is resulting in conversion success being set even though station
+            #   is not present
+            #   suspect stale data in wsi is retained from previous iteration
+            continue
+
         # parse WSI to get sections
         try:
             wsi_series, wsi_issuer, wsi_issue_number, wsi_local = wsi.split("-")   # noqa
             # get other required metadata
             latitude = metadata_dict[wsi]["latitude"]
             longitude = metadata_dict[wsi]["longitude"]
             station_height = metadata_dict[wsi]["elevation"]
@@ -409,14 +415,18 @@
         except Exception:
             conversion_success[tsi] = False
             if wsi == "":
                 LOGGER.warning(f"Missing WSI for station {tsi}")
             else:
                 LOGGER.warning((f"Invalid WSI ({wsi}) found in station file,"
                                 " unable to parse"))
+            #   Question for Tom on how wigos mapping is resulting in conversion success being set even though station
+            #   is not present
+            #   suspect stale data in wsi is retained from previous iteration
+            continue
 
         # TODO: update mappings based on number of precipitation observations and observed phenomena
 
         # for idx in range(num_rvr):
         #     rvr_mappings = [
         #         {"eccodes_key": f"#{idx+1}#runwayDesignator", "value": f"data:rvr_{idx+1}_designator"},
         #         {"eccodes_key": f"#{idx+1}#qualifierForRunwayVisualRange", "value": f"data:rvr_{idx+1}_qualifier"},
@@ -468,24 +478,28 @@
                 delayed_replications,
                 extended_delayed_replications,
                 table_version)
         except Exception as e:
             LOGGER.error(e)
             LOGGER.error("Error creating BUFRMessage")
             conversion_success[tsi] = False
+            #   Question for Tom on how wigos mapping is resulting in conversion success being set even though station
+            #   is not present
+            #   suspect stale data in wsi is retained from previous iteration
+            continue
 
         # parse
         if conversion_success[tsi]:
             try:
                 message.parse(msg, mapping)
             except Exception as e:
                 LOGGER.error(e)
                 LOGGER.error("Error parsing message")
                 conversion_success[tsi] = False
-            message.parse(msg, mapping)
+
         # Only convert to BUFR if there's no errors so far
         if conversion_success[tsi]:
             try:
                 result["bufr4"] = message.as_bufr()  # encode to BUFR
                 status = {"code": PASSED}
             except Exception as e:
                 LOGGER.error("Error encoding BUFR, null returned")
```

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/resources/icao-metar-mappings.json` & `metar2bufr-0.0.2.38/src/metar2bufr/resources/icao-metar-mappings.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/resources/metar-mappings.json` & `metar2bufr-0.0.2.38/src/metar2bufr/resources/metar-mappings.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr/resources/metar-mappings2.json` & `metar2bufr-0.0.2.38/src/metar2bufr/resources/metar-mappings2.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr.egg-info/PKG-INFO` & `metar2bufr-0.0.2.38/src/metar2bufr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar2bufr
-Version: 0.0.2.37
+Version: 0.0.2.38
 Summary: Package for converting METAR TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `metar2bufr-0.0.2.37/src/metar2bufr.egg-info/SOURCES.txt` & `metar2bufr-0.0.2.38/src/metar2bufr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

