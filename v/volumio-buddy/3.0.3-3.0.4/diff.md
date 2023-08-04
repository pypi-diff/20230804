# Comparing `tmp/volumio-buddy-3.0.3.tar.gz` & `tmp/volumio-buddy-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/volumio-buddy/volumio-buddy/dist/.tmp-8gm_nrkf/volumio-buddy-3.0.3.tar", last modified: Sun Dec 18 10:09:53 2022, max compression
+gzip compressed data, was "/home/runner/work/volumio-buddy/volumio-buddy/dist/.tmp-da7ub6g2/volumio-buddy-3.0.4.tar", last modified: Fri Aug  4 20:36:49 2023, max compression
```

## Comparing `volumio-buddy-3.0.3.tar` & `volumio-buddy-3.0.4.tar`

### file list

```diff
@@ -1,28 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 10:09:53.000000 volumio-buddy-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    34502 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2022-12-18 10:09:53.000000 volumio-buddy-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2171 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2022-12-18 10:09:53.000000 volumio-buddy-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 10:09:53.000000 volumio-buddy-3.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 10:09:53.000000 volumio-buddy-3.0.3/src/vb3/
--rw-r--r--   0 runner    (1001) docker     (123)    65932 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/src/vb3/Vera.ttf
--rw-r--r--   0 runner    (1001) docker     (123)      595 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/src/vb3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/src/vb3/battery.py
--rw-r--r--   0 runner    (1001) docker     (123)    16436 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/src/vb3/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     7724 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/src/vb3/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/src/vb3/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    29964 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/src/vb3/pixChicago.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/src/vb3/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    24629 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/src/vb3/volumio.ppm
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/src/vb3/volumio_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8614 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/src/vbuddy
--rw-r--r--   0 runner    (1001) docker     (123)      317 2022-12-18 10:09:09.000000 volumio-buddy-3.0.3/src/vbuddy.service
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-18 10:09:53.000000 volumio-buddy-3.0.3/src/volumio_buddy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2022-12-18 10:09:53.000000 volumio-buddy-3.0.3/src/volumio_buddy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2022-12-18 10:09:53.000000 volumio-buddy-3.0.3/src/volumio_buddy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-18 10:09:53.000000 volumio-buddy-3.0.3/src/volumio_buddy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2022-12-18 10:09:53.000000 volumio-buddy-3.0.3/src/volumio_buddy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2022-12-18 10:09:53.000000 volumio-buddy-3.0.3/src/volumio_buddy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:36:49.000000 volumio-buddy-3.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    34502 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-04 20:36:49.000000 volumio-buddy-3.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-04 20:36:49.000000 volumio-buddy-3.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:36:49.000000 volumio-buddy-3.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:36:49.000000 volumio-buddy-3.0.4/src/vb3/
+-rw-r--r--   0 runner    (1001) docker     (123)    65932 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/src/vb3/Vera.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/src/vb3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/src/vb3/battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/src/vb3/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7724 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/src/vb3/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/src/vb3/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29964 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/src/vb3/pixChicago.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/src/vb3/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24629 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/src/vb3/volumio.ppm
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/src/vb3/volumio_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8614 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/src/vbuddy
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/src/vbuddy.service
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:36:49.000000 volumio-buddy-3.0.4/src/volumio_buddy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-08-04 20:36:49.000000 volumio-buddy-3.0.4/src/volumio_buddy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-08-04 20:36:49.000000 volumio-buddy-3.0.4/src/volumio_buddy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 20:36:49.000000 volumio-buddy-3.0.4/src/volumio_buddy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-04 20:36:49.000000 volumio-buddy-3.0.4/src/volumio_buddy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-04 20:36:49.000000 volumio-buddy-3.0.4/src/volumio_buddy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:36:49.000000 volumio-buddy-3.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/tests/test_battery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/tests/test_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-04 20:35:55.000000 volumio-buddy-3.0.4/tests/test_volumio_client.py
```

### Comparing `volumio-buddy-3.0.3/LICENSE` & `volumio-buddy-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `volumio-buddy-3.0.3/PKG-INFO` & `volumio-buddy-3.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volumio-buddy
-Version: 3.0.3
+Version: 3.0.4
 Summary: Hardware add-ons integration for Volumio 3
 Home-page: https://github.com/foxey/volumio-buddy
 Author: Michiel Fokke
 Author-email: michiel@fokke.org
 Project-URL: Bug Tracker, https://github.com/foxey/volumio-buddy/issues
 Keywords: Volumio,Volumio3,GPIO,SSD1306,OLED,Rotary Encoder,SocketIO
 Classifier: Programming Language :: Python :: 3
```

### Comparing `volumio-buddy-3.0.3/README.md` & `volumio-buddy-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `volumio-buddy-3.0.3/setup.cfg` & `volumio-buddy-3.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = volumio-buddy
-version = 3.0.3
+version = 3.0.4
 author = Michiel Fokke
 author_email = michiel@fokke.org
 description = Hardware add-ons integration for Volumio 3
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/foxey/volumio-buddy
 project_urls =
```

### Comparing `volumio-buddy-3.0.3/src/vb3/Vera.ttf` & `volumio-buddy-3.0.4/src/vb3/Vera.ttf`

 * *Files identical despite different names*

### Comparing `volumio-buddy-3.0.3/src/vb3/__init__.py` & `volumio-buddy-3.0.4/src/vb3/__init__.py`

 * *Files identical despite different names*

### Comparing `volumio-buddy-3.0.3/src/vb3/battery.py` & `volumio-buddy-3.0.4/src/vb3/battery.py`

 * *Files identical despite different names*

### Comparing `volumio-buddy-3.0.3/src/vb3/display.py` & `volumio-buddy-3.0.4/src/vb3/display.py`

 * *Files identical despite different names*

### Comparing `volumio-buddy-3.0.3/src/vb3/gpio.py` & `volumio-buddy-3.0.4/src/vb3/gpio.py`

 * *Files identical despite different names*

### Comparing `volumio-buddy-3.0.3/src/vb3/network.py` & `volumio-buddy-3.0.4/src/vb3/network.py`

 * *Files identical despite different names*

### Comparing `volumio-buddy-3.0.3/src/vb3/pixChicago.ttf` & `volumio-buddy-3.0.4/src/vb3/pixChicago.ttf`

 * *Files identical despite different names*

### Comparing `volumio-buddy-3.0.3/src/vb3/util.py` & `volumio-buddy-3.0.4/src/vb3/util.py`

 * *Files identical despite different names*

### Comparing `volumio-buddy-3.0.3/src/vb3/volumio.ppm` & `volumio-buddy-3.0.4/src/vb3/volumio.ppm`

 * *Files identical despite different names*

### Comparing `volumio-buddy-3.0.3/src/vb3/volumio_client.py` & `volumio-buddy-3.0.4/src/vb3/volumio_client.py`

 * *Files identical despite different names*

### Comparing `volumio-buddy-3.0.3/src/vbuddy` & `volumio-buddy-3.0.4/src/vbuddy`

 * *Files identical despite different names*

### Comparing `volumio-buddy-3.0.3/src/volumio_buddy.egg-info/PKG-INFO` & `volumio-buddy-3.0.4/src/volumio_buddy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volumio-buddy
-Version: 3.0.3
+Version: 3.0.4
 Summary: Hardware add-ons integration for Volumio 3
 Home-page: https://github.com/foxey/volumio-buddy
 Author: Michiel Fokke
 Author-email: michiel@fokke.org
 Project-URL: Bug Tracker, https://github.com/foxey/volumio-buddy/issues
 Keywords: Volumio,Volumio3,GPIO,SSD1306,OLED,Rotary Encoder,SocketIO
 Classifier: Programming Language :: Python :: 3
```

