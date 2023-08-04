# Comparing `tmp/metar2bufr-0.0.2.35.tar.gz` & `tmp/metar2bufr-0.0.2.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metar2bufr-0.0.2.35.tar", last modified: Thu Aug  3 22:39:57 2023, max compression
+gzip compressed data, was "metar2bufr-0.0.2.36.tar", last modified: Thu Aug  3 22:57:31 2023, max compression
```

## Comparing `metar2bufr-0.0.2.35.tar` & `metar2bufr-0.0.2.36.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.363705 metar2bufr-0.0.2.35/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1073 2023-07-13 16:23:37.000000 metar2bufr-0.0.2.35/LICENSE
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       39 2023-07-13 22:22:45.000000 metar2bufr-0.0.2.35/MANIFEST.in
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-08-03 22:39:57.362705 metar2bufr-0.0.2.35/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       85 2023-07-13 16:24:38.000000 metar2bufr-0.0.2.35/README.md
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      764 2023-08-03 22:39:25.000000 metar2bufr-0.0.2.35/pyproject.toml
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-08-03 22:39:57.363705 metar2bufr-0.0.2.35/setup.cfg
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.355704 metar2bufr-0.0.2.35/src/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.357704 metar2bufr-0.0.2.35/src/metar2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      164 2023-07-13 20:54:01.000000 metar2bufr-0.0.2.35/src/metar2bufr/__init__.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.358704 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.355704 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.355704 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.359705 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.360705 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/cli.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.356704 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/docs/
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.360705 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/docs/source/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3056 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/docs/source/conf.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3330 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/setup.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.360705 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/tests/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8502 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    26208 2023-07-26 21:53:12.000000 metar2bufr-0.0.2.35/src/metar2bufr/icao_bufr_encoder.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.361704 metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 17:15:28.000000 metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    59241 2023-07-13 20:20:04.000000 metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/metarDecoders.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    82209 2023-07-13 16:28:08.000000 metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/tpg.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8261 2023-07-13 16:28:19.000000 metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/xmlConfig.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     6620 2023-07-13 20:39:39.000000 metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/xmlUtilities.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    24100 2023-08-03 22:39:03.000000 metar2bufr-0.0.2.35/src/metar2bufr/metar_bufr_encoder.py
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.362705 metar2bufr-0.0.2.35/src/metar2bufr/resources/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 22:08:27.000000 metar2bufr-0.0.2.35/src/metar2bufr/resources/__init__.py
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2793 2023-07-20 23:18:14.000000 metar2bufr-0.0.2.35/src/metar2bufr/resources/icao-metar-mappings.json
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2825 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.35/src/metar2bufr/resources/metar-mappings.json
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3136 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.35/src/metar2bufr/resources/metar-mappings2.json
-drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:39:57.358704 metar2bufr-0.0.2.35/src/metar2bufr.egg-info/
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-08-03 22:39:57.000000 metar2bufr-0.0.2.35/src/metar2bufr.egg-info/PKG-INFO
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1107 2023-08-03 22:39:57.000000 metar2bufr-0.0.2.35/src/metar2bufr.egg-info/SOURCES.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-08-03 22:39:57.000000 metar2bufr-0.0.2.35/src/metar2bufr.egg-info/dependency_links.txt
--rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       11 2023-08-03 22:39:57.000000 metar2bufr-0.0.2.35/src/metar2bufr.egg-info/top_level.txt
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.113490 metar2bufr-0.0.2.36/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1073 2023-07-13 16:23:37.000000 metar2bufr-0.0.2.36/LICENSE
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       39 2023-07-13 22:22:45.000000 metar2bufr-0.0.2.36/MANIFEST.in
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-08-03 22:57:31.113490 metar2bufr-0.0.2.36/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       85 2023-07-13 16:24:38.000000 metar2bufr-0.0.2.36/README.md
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      764 2023-08-03 22:57:21.000000 metar2bufr-0.0.2.36/pyproject.toml
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       38 2023-08-03 22:57:31.113490 metar2bufr-0.0.2.36/setup.cfg
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.107490 metar2bufr-0.0.2.36/src/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.109490 metar2bufr-0.0.2.36/src/metar2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      164 2023-07-13 20:54:01.000000 metar2bufr-0.0.2.36/src/metar2bufr/__init__.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.110490 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.107490 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/build/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.107490 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/build/lib/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.110490 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/build/lib/csv2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.111490 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/csv2bufr/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    36767 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/csv2bufr/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     4621 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/csv2bufr/cli.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     7899 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.107490 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/docs/
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.111490 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/docs/source/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3056 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/docs/source/conf.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3330 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/setup.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.111490 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/tests/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8502 2023-07-13 16:27:31.000000 metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    26208 2023-07-26 21:53:12.000000 metar2bufr-0.0.2.36/src/metar2bufr/icao_bufr_encoder.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.112490 metar2bufr-0.0.2.36/src/metar2bufr/metarDecoder/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 17:15:28.000000 metar2bufr-0.0.2.36/src/metar2bufr/metarDecoder/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    59241 2023-07-13 20:20:04.000000 metar2bufr-0.0.2.36/src/metar2bufr/metarDecoder/metarDecoders.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    82209 2023-07-13 16:28:08.000000 metar2bufr-0.0.2.36/src/metar2bufr/metarDecoder/tpg.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     8261 2023-07-13 16:28:19.000000 metar2bufr-0.0.2.36/src/metar2bufr/metarDecoder/xmlConfig.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     6620 2023-07-13 20:39:39.000000 metar2bufr-0.0.2.36/src/metar2bufr/metarDecoder/xmlUtilities.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)    24305 2023-08-03 22:55:56.000000 metar2bufr-0.0.2.36/src/metar2bufr/metar_bufr_encoder.py
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.113490 metar2bufr-0.0.2.36/src/metar2bufr/resources/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-07-13 22:08:27.000000 metar2bufr-0.0.2.36/src/metar2bufr/resources/__init__.py
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2793 2023-07-20 23:18:14.000000 metar2bufr-0.0.2.36/src/metar2bufr/resources/icao-metar-mappings.json
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     2825 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.36/src/metar2bufr/resources/metar-mappings.json
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     3136 2023-07-13 16:29:37.000000 metar2bufr-0.0.2.36/src/metar2bufr/resources/metar-mappings2.json
+drwxr-x---   0 alexander.thompson  (1013) alexander.thompson  (1013)        0 2023-08-03 22:57:31.110490 metar2bufr-0.0.2.36/src/metar2bufr.egg-info/
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)      623 2023-08-03 22:57:31.000000 metar2bufr-0.0.2.36/src/metar2bufr.egg-info/PKG-INFO
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)     1107 2023-08-03 22:57:31.000000 metar2bufr-0.0.2.36/src/metar2bufr.egg-info/SOURCES.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)        1 2023-08-03 22:57:31.000000 metar2bufr-0.0.2.36/src/metar2bufr.egg-info/dependency_links.txt
+-rw-r-----   0 alexander.thompson  (1013) alexander.thompson  (1013)       11 2023-08-03 22:57:31.000000 metar2bufr-0.0.2.36/src/metar2bufr.egg-info/top_level.txt
```

### Comparing `metar2bufr-0.0.2.35/LICENSE` & `metar2bufr-0.0.2.36/LICENSE`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/PKG-INFO` & `metar2bufr-0.0.2.36/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar2bufr
-Version: 0.0.2.35
+Version: 0.0.2.36
 Summary: Package for converting METAR TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `metar2bufr-0.0.2.35/pyproject.toml` & `metar2bufr-0.0.2.36/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "metar2bufr"
-version = "0.0.2.35"
+version = "0.0.2.36"
 authors = [
   { name="Alexander Thompson", email="alexander.thompson@noaa.gov" },
 ]
 description = "Package for converting METAR TAC messages or an individual METAR message to BUFR4"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py` & `metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/build/lib/csv2bufr/__init__.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py` & `metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/build/lib/csv2bufr/cli.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py` & `metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/build/lib/csv2bufr/pygeoapi_plugin.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/__init__.py` & `metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/csv2bufr/__init__.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/cli.py` & `metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/csv2bufr/cli.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py` & `metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/csv2bufr/pygeoapi_plugin.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/docs/source/conf.py` & `metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/setup.py` & `metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/setup.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py` & `metar2bufr-0.0.2.36/src/metar2bufr/csv2bufr/tests/test_csv2bufr.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/icao_bufr_encoder.py` & `metar2bufr-0.0.2.36/src/metar2bufr/icao_bufr_encoder.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/metarDecoders.py` & `metar2bufr-0.0.2.36/src/metar2bufr/metarDecoder/metarDecoders.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/tpg.py` & `metar2bufr-0.0.2.36/src/metar2bufr/metarDecoder/tpg.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/xmlConfig.py` & `metar2bufr-0.0.2.36/src/metar2bufr/metarDecoder/xmlConfig.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/metarDecoder/xmlUtilities.py` & `metar2bufr-0.0.2.36/src/metar2bufr/metarDecoder/xmlUtilities.py`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/metar_bufr_encoder.py` & `metar2bufr-0.0.2.36/src/metar2bufr/metar_bufr_encoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,21 +300,25 @@
     #         if len(decoded['sky']['str'][i]) > 6:
     #             output['sig_convec_'+str(i+1)] = decoded['sky']['str'][i][6:]
 
     #         #  TODO need to incorporate NSC and NCD values as described in section 15.9.1.3 of FM-15 manual
 
     if 'temps' in decoded:
         if 'air' in decoded['temps']:
-            # metar records temperatures in Celsius. Need to convert to Kelvin for bufr
-            air_temp = float(decoded['temps']['air'])
-            output['air_temp'] = air_temp + 273.15
+            #   check for missing value
+            if decoded['temps']['air'] != '//':
+                # metar records temperatures in Celsius. Need to convert to Kelvin for bufr
+                air_temp = float(decoded['temps']['air'])
+                output['air_temp'] = air_temp + 273.15
         if 'dewpoint' in decoded['temps']:
-            # metar records temperatures in Celsius. Need to convert to Kelvin for bufr
-            dewpoint_temp = float(decoded['temps']['dewpoint'])
-            output['dew_point_temp'] = dewpoint_temp + 273.15
+            #   check for missing value
+            if decoded['temps']['dewpoint'] != '//':
+                # metar records temperatures in Celsius. Need to convert to Kelvin for bufr
+                dewpoint_temp = float(decoded['temps']['dewpoint'])
+                output['dew_point_temp'] = dewpoint_temp + 273.15
 
     if 'altimeter' in decoded:
         altimeter = float(decoded['altimeter']['value'])
         alt_uom = decoded['altimeter']['uom']
         if alt_uom == 'hPa':
             output['altimeter'] = altimeter*100
         elif alt_uom == "[in_i'Hg]":
```

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/resources/icao-metar-mappings.json` & `metar2bufr-0.0.2.36/src/metar2bufr/resources/icao-metar-mappings.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/resources/metar-mappings.json` & `metar2bufr-0.0.2.36/src/metar2bufr/resources/metar-mappings.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr/resources/metar-mappings2.json` & `metar2bufr-0.0.2.36/src/metar2bufr/resources/metar-mappings2.json`

 * *Files identical despite different names*

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr.egg-info/PKG-INFO` & `metar2bufr-0.0.2.36/src/metar2bufr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metar2bufr
-Version: 0.0.2.35
+Version: 0.0.2.36
 Summary: Package for converting METAR TAC messages or an individual METAR message to BUFR4
 Author-email: Alexander Thompson <alexander.thompson@noaa.gov>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: WMO,METAR,FM-15,BUFR,decoding,weather,observations
 Classifier: Development Status :: 1 - Planning
 Requires-Python: >=3.7
```

### Comparing `metar2bufr-0.0.2.35/src/metar2bufr.egg-info/SOURCES.txt` & `metar2bufr-0.0.2.36/src/metar2bufr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

