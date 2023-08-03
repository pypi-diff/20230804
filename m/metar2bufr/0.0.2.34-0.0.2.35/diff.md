# Comparing `tmp/metar2bufr-0.0.2.34.tar.gz` & `tmp/metar2bufr-0.0.2.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metar2bufr-0.0.2.34.tar", last modified: Thu Aug  3 00:51:51 2023, max compression
+gzip compressed data, was "metar2bufr-0.0.2.35.tar", last modified: Thu Aug  3 22:39:57 2023, max compression
```

## Comparing `metar2bufr-0.0.2.34.tar` & `metar2bufr-0.0.2.35.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.728076 metar2bufr-0.0.2.34/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1073 2023-07-13 16:23:37.000000 metar2bufr-0.0.2.34/LICENSE
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       39 2023-07-13 22:22:45.000000 metar2bufr-0.0.2.34/MANIFEST.in
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-08-03 00:51:51.728076 metar2bufr-0.0.2.34/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       85 2023-07-13 16:24:38.000000 metar2bufr-0.0.2.34/README.md
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      764 2023-08-03 00:51:21.000000 metar2bufr-0.0.2.34/pyproject.toml
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-08-03 00:51:51.729076 metar2bufr-0.0.2.34/setup.cfg
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.721075 metar2bufr-0.0.2.34/src/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.724075 metar2bufr-0.0.2.34/src/metar2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      164 2023-07-13 20:54:01.000000 metar2bufr-0.0.2.34/src/metar2bufr/__init__.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.725075 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.722075 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/build/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.722075 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/build/lib/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.726076 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/build/lib/csv2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.726076 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/csv2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/csv2bufr/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/csv2bufr/cli.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.722075 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/docs/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.726076 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/docs/source/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3056 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/docs/source/conf.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3330 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/setup.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.726076 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/tests/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8502 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    26208 2023-07-26 21:53:12.000000 metar2bufr-0.0.2.34/src/metar2bufr/icao_bufr_encoder.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.727075 metar2bufr-0.0.2.34/src/metar2bufr/metarDecoder/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 17:15:28.000000 metar2bufr-0.0.2.34/src/metar2bufr/metarDecoder/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    59241 2023-07-13 20:20:04.000000 metar2bufr-0.0.2.34/src/metar2bufr/metarDecoder/metarDecoders.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    82209 2023-07-13 16:28:08.000000 metar2bufr-0.0.2.34/src/metar2bufr/metarDecoder/tpg.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8261 2023-07-13 16:28:19.000000 metar2bufr-0.0.2.34/src/metar2bufr/metarDecoder/xmlConfig.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     6620 2023-07-13 20:39:39.000000 metar2bufr-0.0.2.34/src/metar2bufr/metarDecoder/xmlUtilities.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    24148 2023-08-03 00:51:03.000000 metar2bufr-0.0.2.34/src/metar2bufr/metar_bufr_encoder.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.728076 metar2bufr-0.0.2.34/src/metar2bufr/resources/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 22:08:27.000000 metar2bufr-0.0.2.34/src/metar2bufr/resources/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2793 2023-07-20 23:18:14.000000 metar2bufr-0.0.2.34/src/metar2bufr/resources/icao-metar-mappings.json
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2825 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.34/src/metar2bufr/resources/metar-mappings.json
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3136 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.34/src/metar2bufr/resources/metar-mappings2.json
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 00:51:51.725075 metar2bufr-0.0.2.34/src/metar2bufr.egg-info/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-08-03 00:51:51.000000 metar2bufr-0.0.2.34/src/metar2bufr.egg-info/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1107 2023-08-03 00:51:51.000000 metar2bufr-0.0.2.34/src/metar2bufr.egg-info/SOURCES.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-08-03 00:51:51.000000 metar2bufr-0.0.2.34/src/metar2bufr.egg-info/dependency_links.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       11 2023-08-03 00:51:51.000000 metar2bufr-0.0.2.34/src/metar2bufr.egg-info/top_level.txt
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.363705 metar2bufr-0.0.2.35/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1073 2023-07-13 16:23:37.000000 metar2bufr-0.0.2.35/LICENSE
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       39 2023-07-13 22:22:45.000000 metar2bufr-0.0.2.35/MANIFEST.in
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-08-03 22:39:57.362705 metar2bufr-0.0.2.35/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       85 2023-07-13 16:24:38.000000 metar2bufr-0.0.2.35/README.md
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      764 2023-08-03 22:39:25.000000 metar2bufr-0.0.2.35/pyproject.toml
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-08-03 22:39:57.363705 metar2bufr-0.0.2.35/setup.cfg
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.355704 metar2bufr-0.0.2.35/src/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.357704 metar2bufr-0.0.2.35/src/metar2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      164 2023-07-13 20:54:01.000000 metar2bufr-0.0.2.35/src/metar2bufr/__init__.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.358704 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.355704 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.355704 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.359705 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.360705 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/cli.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.356704 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/docs/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.360705 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/docs/source/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3056 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/docs/source/conf.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3330 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/setup.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.360705 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/tests/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8502 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    26208 2023-07-26 21:53:12.000000 metar2bufr-0.0.2.35/src/metar2bufr/icao_bufr_encoder.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.361704 metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 17:15:28.000000 metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    59241 2023-07-13 20:20:04.000000 metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/metarDecoders.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    82209 2023-07-13 16:28:08.000000 metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/tpg.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8261 2023-07-13 16:28:19.000000 metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/xmlConfig.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     6620 2023-07-13 20:39:39.000000 metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/xmlUtilities.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    24100 2023-08-03 22:39:03.000000 metar2bufr-0.0.2.35/src/metar2bufr/metar_bufr_encoder.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.362705 metar2bufr-0.0.2.35/src/metar2bufr/resources/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 22:08:27.000000 metar2bufr-0.0.2.35/src/metar2bufr/resources/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2793 2023-07-20 23:18:14.000000 metar2bufr-0.0.2.35/src/metar2bufr/resources/icao-metar-mappings.json
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2825 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.35/src/metar2bufr/resources/metar-mappings.json
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3136 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.35/src/metar2bufr/resources/metar-mappings2.json
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.358704 metar2bufr-0.0.2.35/src/metar2bufr.egg-info/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-08-03 22:39:57.000000 metar2bufr-0.0.2.35/src/metar2bufr.egg-info/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1107 2023-08-03 22:39:57.000000 metar2bufr-0.0.2.35/src/metar2bufr.egg-info/SOURCES.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-08-03 22:39:57.000000 metar2bufr-0.0.2.35/src/metar2bufr.egg-info/dependency_links.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       11 2023-08-03 22:39:57.000000 metar2bufr-0.0.2.35/src/metar2bufr.egg-info/top_level.txt
```

### Comparing `metar2bufr-0.0.2.34/LICENSE` & `metar2bufr-0.0.2.35/LICENSE`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/PKG-INFO` & `metar2bufr-0.0.2.35/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar2bufr
-Version: 0.0.2.34
+Version: 0.0.2.35
 Summary: Package for converting METAR TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `metar2bufr-0.0.2.34/pyproject.toml` & `metar2bufr-0.0.2.35/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metar2bufr"
-version = "0.0.2.34"
+version = "0.0.2.35"
 authors = [
   { name="Alexander Thompson", email="alexander.thompson@noaa.gov" },
 ]
 description = "Package for converting METAR TAC messages or an individual METAR message to BUFR4"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py` & `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py` & `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py` & `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/csv2bufr/__init__.py` & `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/__init__.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/csv2bufr/cli.py` & `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/cli.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py` & `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/docs/source/conf.py` & `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/setup.py` & `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/setup.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py` & `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/icao_bufr_encoder.py` & `metar2bufr-0.0.2.35/src/metar2bufr/icao_bufr_encoder.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/metarDecoder/metarDecoders.py` & `metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/metarDecoders.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/metarDecoder/tpg.py` & `metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/tpg.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/metarDecoder/xmlConfig.py` & `metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/xmlConfig.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/metarDecoder/xmlUtilities.py` & `metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/xmlUtilities.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/metar_bufr_encoder.py` & `metar2bufr-0.0.2.35/src/metar2bufr/metar_bufr_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,23 +85,23 @@
     for i in range(len(data)):
         data[i] = data[i]+"="
 
     # print(data[:len(data)-1])
     return data[:len(data)-1]
 
 def parse_metar(message: str, year: int, month: int) -> dict:
-    message = message.strip()
-    print(f"Parsing message: {message}")
-    print(re_ID.match(message))
     icaoID = re_ID.match(message).group('id')
     if deu.isUSIdentifier(icaoID):
         decoded = fmh(message)
     else:
         decoded = annex3(message)
 
+    for key in decoded:
+        print(key, ': ', decoded[key])
+
     output = deepcopy(metar_template)
 
     output['report_type'] = message[0:5]
     output['year'] = year
     output['month'] = month
 
     if 'ident' in decoded:
@@ -115,15 +115,15 @@
         #     if f' {icao} ' in line:
         #         # print(line)
         #         # print(re.search('[0-9]{5}', line))
         #         tsi = str(re.search('[0-9]{5}', line).group())
         #         # print(f'Mapping {icao} to {tsi}')
         #         break
 
-        try:
+        try: 
             output['tsi'] = icao
             # output['block_no'] = tsi[0:2]
             # output['station_no'] = tsi[2:5]
         except Exception:
             # tsi = None
             output['tsi'] = None
             # output['block_no'] = None
@@ -140,22 +140,27 @@
     else:
         output['station_type'] = 1
 
     if 'wind' in decoded:
         wind_uom = decoded['wind']['uom']
         wind_speed = decoded['wind']['ff']
         #   this bufr template records wind speed in m/s
-        #   if wind speed reported in m/s, can copy directly to output
-        if wind_uom == 'm/s':
-            output['wind_speed'] = wind_speed
-        #   if wind speed report in knots, need to convert to m/s for bufr
-        elif wind_uom == '[kn_i]':
-            output['wind_speed'] = round(int(wind_speed)*0.514444, 2)
+
+        #   check for missing value
+        if wind_speed != '//':
+            #   if wind speed reported in m/s, can copy directly to output
+            if wind_uom == 'm/s':
+                output['wind_speed'] = wind_speed
+            #   if wind speed report in knots, need to convert to m/s for bufr
+            elif wind_uom == '[kn_i]':
+                output['wind_speed'] = round(int(wind_speed)*0.514444, 2)
         
-        output['wind_direction'] = decoded['wind']['dd']
+        #   check for missing value
+        if decoded['wind']['dd'] != '///':
+            output['wind_direction'] = decoded['wind']['dd']
 
         #   perform same unit conversions on gust speed if recorded
         if 'gg' in decoded['wind']:
             gust_speed = decoded['wind']['gg']
             if wind_uom == 'm/s':
                 output['gust_speed'] = gust_speed
             elif wind_uom == '[kn_i]':
@@ -163,23 +168,20 @@
         output['wind_uom'] = decoded['wind']['uom']
         if 'ccw' in decoded['wind']:
             output['variable_extreme_ccw'] = int(decoded['wind']['ccw'])
         if 'cw' in decoded['wind']:
             output['variable_extreme_cw'] = int(decoded['wind']['cw'])
 
     if 'vsby' in decoded:
-        vis_uom = decoded['vsby']['uom']
-        visibility = decoded['vsby']['value']
-        #   bufr uses meters for visibility. if reported in meters, just copy to output
-        if vis_uom == 'm':
-            output['visibility'] == visibility
-        #   if reported in Statute Miles (SM), convert to m/s
-        elif vis_uom == '[mi_i]':
-            output['visibility'] == math.floor(float(visibility)*1609.34)
-        output['visibility_uom'] = decoded['vsby']['uom']
+        #   check for missing value
+        if decoded['vsby']['value'] != '////':
+            # Metar reports visibility in statute miles. Need to convert value to meters to be bufr compatible
+            vis_miles = float(decoded['vsby']['value'])
+            output['visibility'] = math.floor(vis_miles * 1609.34)
+            output['visibility_uom'] = decoded['vsby']['uom']
 
     # TODO need to incorporate visibility variation as outlined in section 15.6.2 in FM-15 manual
 
     num_rvr = 0
     if 'rvr' in decoded:
         num_rvr = len(decoded['rvr']['str'])
         for i in range(num_rvr):
@@ -270,17 +272,22 @@
                 output[f'cloud_amount_{i+1}'] = 11
             elif cloud_amount == 'BKN':
                 # codes BROKEN clouds as 12
                 output[f'cloud_amount_{i+1}'] = 12
             elif cloud_amount == 'OVC':
                 # table 020011 lists two codes that might work for OVERCAST clouds, 9 and 10. Hard coding as 10 for now
                 output[f'cloud_amount_{i+1}'] = 10
+            elif cloud_amount == '///':
+                # codes undiscernable observation or observation not made as 15
+                output[f'cloud_amount_{i+1}'] = 15
             # convert reported cloud height from hundreds of ft. to meters for bufr
-            cloud_height_ft = float(decoded['sky']['str'][i][3:6]) * 100
-            output[f'cloud_height_{i+1}'] = math.floor(cloud_height_ft*0.3048)
+            # check for missing value
+            if decoded['sky']['str'][i][3:6] != '///':
+                cloud_height_ft = float(decoded['sky']['str'][i][3:6]) * 100
+                output[f'cloud_height_{i+1}'] = math.floor(cloud_height_ft*0.3048)
 
             # TODO: capture significant convective clouds, namely TCU OR CB using ecCodes
             if len(decoded['sky']['str'][i]) > 6:
                 output['sig_convec_'+str(i+1)] = decoded['sky']['str'][i][6:]
 
             #  TODO need to incorporate NSC and NCD values as described in section 15.9.1.3 of FM-15 manual
     # if 'sky' in decoded:
@@ -301,29 +308,23 @@
             air_temp = float(decoded['temps']['air'])
             output['air_temp'] = air_temp + 273.15
         if 'dewpoint' in decoded['temps']:
             # metar records temperatures in Celsius. Need to convert to Kelvin for bufr
             dewpoint_temp = float(decoded['temps']['dewpoint'])
             output['dew_point_temp'] = dewpoint_temp + 273.15
 
-    # if 'altimeter' in decoded:
-    #     altimeter = float(decoded['altimeter']['value'])
-    #     # metar records altimeter in inches of Mercury. need to convert to Pascals for bufr
-    #     output['altimeter'] = round(altimeter*3386.39, 2)
-    #     output['altimeter_uom'] = decoded['altimeter']['uom']
-    
     if 'altimeter' in decoded:
         altimeter = float(decoded['altimeter']['value'])
         alt_uom = decoded['altimeter']['uom']
-        #   if units of measurement are in hectopascals, hPa, multiply by 100 to convert to Pascals for bufr
         if alt_uom == 'hPa':
             output['altimeter'] = altimeter*100
         elif alt_uom == "[in_i'Hg]":
-            # if units of measurement is inches of Mercury. need to convert to Pascals for bufr
+            # if metar records altimeter in inches of Mercury. need to convert to Pascals for bufr
             output['altimeter'] = round(altimeter*3386.39, 2)
+        output['altimeter_uom'] = decoded['altimeter']['uom']
 
     return output, num_rvr, num_vrbrvr, num_pcp, num_obv, num_sky
 
 def transform(data: str, metadata: str, year: int, month: int) -> Iterator[dict]:
     # ===================
     # First parse metadata file
     # ===================
```

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/resources/icao-metar-mappings.json` & `metar2bufr-0.0.2.35/src/metar2bufr/resources/icao-metar-mappings.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/resources/metar-mappings.json` & `metar2bufr-0.0.2.35/src/metar2bufr/resources/metar-mappings.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr/resources/metar-mappings2.json` & `metar2bufr-0.0.2.35/src/metar2bufr/resources/metar-mappings2.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr.egg-info/PKG-INFO` & `metar2bufr-0.0.2.35/src/metar2bufr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar2bufr
-Version: 0.0.2.34
+Version: 0.0.2.35
 Summary: Package for converting METAR TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `metar2bufr-0.0.2.34/src/metar2bufr.egg-info/SOURCES.txt` & `metar2bufr-0.0.2.35/src/metar2bufr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

