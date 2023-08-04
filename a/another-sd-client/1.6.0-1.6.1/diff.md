# Comparing `tmp/another_sd_client-1.6.0.tar.gz` & `tmp/another_sd_client-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "another_sd_client-1.6.0.tar", max compression
+gzip compressed data, was "another_sd_client-1.6.1.tar", max compression
```

## Comparing `another_sd_client-1.6.0.tar` & `another_sd_client-1.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     6296 2023-08-03 14:25:11.395404 another_sd_client-1.6.0/README.md
--rw-r--r--   0        0        0      950 2023-08-03 14:25:12.592508 another_sd_client-1.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-03 14:25:11.437407 another_sd_client-1.6.0/sdclient/__init__.py
--rw-r--r--   0        0        0     5018 2023-08-03 14:25:11.396404 another_sd_client-1.6.0/sdclient/client.py
--rw-r--r--   0        0        0     1017 2023-08-03 14:25:11.396404 another_sd_client-1.6.0/sdclient/exceptions.py
--rw-r--r--   0        0        0        0 2023-08-03 14:25:11.438408 another_sd_client-1.6.0/sdclient/py.typed
--rw-r--r--   0        0        0     4937 2023-08-03 14:25:11.396404 another_sd_client-1.6.0/sdclient/requests.py
--rw-r--r--   0        0        0     3024 2023-08-03 14:25:11.397404 another_sd_client-1.6.0/sdclient/responses.py
--rw-r--r--   0        0        0     6982 1970-01-01 00:00:00.000000 another_sd_client-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     6296 2023-08-04 08:34:25.777069 another_sd_client-1.6.1/README.md
+-rw-r--r--   0        0        0      950 2023-08-04 08:34:26.960173 another_sd_client-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-04 08:34:25.817073 another_sd_client-1.6.1/sdclient/__init__.py
+-rw-r--r--   0        0        0     5018 2023-08-04 08:34:25.778070 another_sd_client-1.6.1/sdclient/client.py
+-rw-r--r--   0        0        0     1017 2023-08-04 08:34:25.778070 another_sd_client-1.6.1/sdclient/exceptions.py
+-rw-r--r--   0        0        0        0 2023-08-04 08:34:25.818073 another_sd_client-1.6.1/sdclient/py.typed
+-rw-r--r--   0        0        0     4937 2023-08-04 08:34:25.778070 another_sd_client-1.6.1/sdclient/requests.py
+-rw-r--r--   0        0        0     3086 2023-08-04 08:34:25.778070 another_sd_client-1.6.1/sdclient/responses.py
+-rw-r--r--   0        0        0     6982 1970-01-01 00:00:00.000000 another_sd_client-1.6.1/PKG-INFO
```

### Comparing `another_sd_client-1.6.0/README.md` & `another_sd_client-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.6.0/pyproject.toml` & `another_sd_client-1.6.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2022 Magenta ApS <https://magenta.dk>
 # SPDX-License-Identifier: MPL-2.0
 [tool.poetry]
 name = "another-sd-client"
-version = "1.6.0"
+version = "1.6.1"
 description = "Client for communicating with SD Løn"
 authors = ["Magenta ApS <info@magenta.dk>"]
 readme = "README.md"
 packages = [{include = "sdclient"}]
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/another-sd-client"
 keywords = ["os2mo", "sd"]
```

### Comparing `another_sd_client-1.6.0/sdclient/client.py` & `another_sd_client-1.6.1/sdclient/client.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.6.0/sdclient/exceptions.py` & `another_sd_client-1.6.1/sdclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.6.0/sdclient/requests.py` & `another_sd_client-1.6.1/sdclient/requests.py`

 * *Files identical despite different names*

### Comparing `another_sd_client-1.6.0/sdclient/responses.py` & `another_sd_client-1.6.1/sdclient/responses.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,16 @@
     ny2_niveau = "NY2-niveau"
     ny3_niveau = "NY3-niveau"
     ny4_niveau = "NY4-niveau"
     ny5_niveau = "NY5-niveau"
     ny6_niveau = "NY6-niveau"
     ny7_niveau = "NY7-niveau"
     ny8_niveau = "NY8-niveau"
+    ny9_niveau = "NY9-niveau"
+    ny10_niveau = "NY10-niveau"
 
 
 class DepartmentLevelReference(BaseModel):
     DepartmentLevelIdentifier: DepartmentLevelIdentifierEnum | None = None
     DepartmentLevelReference: DepartmentLevelReference | None = None
     # TODO: add validator?
```

### Comparing `another_sd_client-1.6.0/PKG-INFO` & `another_sd_client-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: another-sd-client
-Version: 1.6.0
+Version: 1.6.1
 Summary: Client for communicating with SD Løn
 Home-page: https://magenta.dk/
 Keywords: os2mo,sd
 Author: Magenta ApS
 Author-email: info@magenta.dk
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
```

