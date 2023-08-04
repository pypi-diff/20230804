# Comparing `tmp/wowipy-1.1.7.tar.gz` & `tmp/wowipy-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wowipy-1.1.7.tar", last modified: Thu Aug  3 09:20:42 2023, max compression
+gzip compressed data, was "wowipy-1.1.8.tar", last modified: Fri Aug  4 09:55:39 2023, max compression
```

## Comparing `wowipy-1.1.7.tar` & `wowipy-1.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 09:20:42.048510 wowipy-1.1.7/
--rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.7/COPYING
--rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.7/LICENSE
--rw-rw-rw-   0        0        0     1120 2023-08-03 09:20:42.047513 wowipy-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-03 09:20:42.048510 wowipy-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1317 2023-08-03 09:20:23.000000 wowipy-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 09:20:42.032552 wowipy-1.1.7/wowipy/
--rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.7/wowipy/__init__.py
--rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.7/wowipy/exceptions.py
--rw-rw-rw-   0        0        0    56035 2023-08-03 09:04:47.000000 wowipy-1.1.7/wowipy/models.py
--rw-rw-rw-   0        0        0     4577 2023-08-03 08:04:52.000000 wowipy-1.1.7/wowipy/rest_adapter.py
--rw-rw-rw-   0        0        0    48072 2023-08-03 08:25:40.000000 wowipy-1.1.7/wowipy/wowipy.py
-drwxrwxrwx   0        0        0        0 2023-08-03 09:20:42.046540 wowipy-1.1.7/wowipy.egg-info/
--rw-rw-rw-   0        0        0     1120 2023-08-03 09:20:41.000000 wowipy-1.1.7/wowipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-08-03 09:20:41.000000 wowipy-1.1.7/wowipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 09:20:41.000000 wowipy-1.1.7/wowipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-08-03 09:20:41.000000 wowipy-1.1.7/wowipy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-03 09:20:41.000000 wowipy-1.1.7/wowipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 09:55:39.842127 wowipy-1.1.8/
+-rw-rw-rw-   0        0        0    35817 2023-06-05 13:12:07.000000 wowipy-1.1.8/COPYING
+-rw-rw-rw-   0        0        0    35817 2023-06-09 09:15:36.000000 wowipy-1.1.8/LICENSE
+-rw-rw-rw-   0        0        0     1120 2023-08-04 09:55:39.842127 wowipy-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-04 09:55:39.842127 wowipy-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1317 2023-08-04 09:55:35.000000 wowipy-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:55:39.826161 wowipy-1.1.8/wowipy/
+-rw-rw-rw-   0        0        0      153 2023-06-09 09:33:03.000000 wowipy-1.1.8/wowipy/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-06-05 13:24:50.000000 wowipy-1.1.8/wowipy/exceptions.py
+-rw-rw-rw-   0        0        0    56035 2023-08-03 09:04:47.000000 wowipy-1.1.8/wowipy/models.py
+-rw-rw-rw-   0        0        0     4577 2023-08-03 08:04:52.000000 wowipy-1.1.8/wowipy/rest_adapter.py
+-rw-rw-rw-   0        0        0    48309 2023-08-04 09:55:35.000000 wowipy-1.1.8/wowipy/wowipy.py
+drwxrwxrwx   0        0        0        0 2023-08-04 09:55:39.841121 wowipy-1.1.8/wowipy.egg-info/
+-rw-rw-rw-   0        0        0     1120 2023-08-04 09:55:39.000000 wowipy-1.1.8/wowipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-08-04 09:55:39.000000 wowipy-1.1.8/wowipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 09:55:39.000000 wowipy-1.1.8/wowipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 09:55:39.000000 wowipy-1.1.8/wowipy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-04 09:55:39.000000 wowipy-1.1.8/wowipy.egg-info/top_level.txt
```

### Comparing `wowipy-1.1.7/COPYING` & `wowipy-1.1.8/COPYING`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.7/LICENSE` & `wowipy-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.7/PKG-INFO` & `wowipy-1.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.7
+Version: 1.1.8
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `wowipy-1.1.7/setup.py` & `wowipy-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='wowipy',
-    version='1.1.7',
+    version='1.1.8',
     description='OPENWOWI Wowiport API wrapper for python',
     url='https://github.com/seb-bau/WowiPy',
     author='Sebastian Bauhaus',
     author_email='sebastian@bytewish.de',
     license='GPL-3.0',
     packages=['wowipy'],
     install_requires=['requests>=2.0',
```

### Comparing `wowipy-1.1.7/wowipy/models.py` & `wowipy-1.1.8/wowipy/models.py`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.7/wowipy/rest_adapter.py` & `wowipy-1.1.8/wowipy/rest_adapter.py`

 * *Files identical despite different names*

### Comparing `wowipy-1.1.7/wowipy/wowipy.py` & `wowipy-1.1.8/wowipy/wowipy.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,21 +62,25 @@
             if len(res) >= max_results:
                 break
 
             if entry.person.id_ in person_ids:
                 continue
 
             if search_name is not None:
-                first_name = entry.person.natural_person.first_name.lower()
-                last_name = entry.person.natural_person.last_name.lower()
-                if self.search_string(first_name, search_name, search_mode) or \
-                        self.search_string(last_name, search_name, search_mode):
-                    res.append(entry)
-                    person_ids.append(entry.person.id_)
-                    continue
+                if entry.person.natural_person is not None:
+                    if entry.person.natural_person.first_name is not None:
+                        first_name = entry.person.natural_person.first_name.lower()
+                    else:
+                        first_name = ""
+                    last_name = entry.person.natural_person.last_name.lower()
+                    if self.search_string(first_name, search_name, search_mode) or \
+                            self.search_string(last_name, search_name, search_mode):
+                        res.append(entry)
+                        person_ids.append(entry.person.id_)
+                        continue
 
             if search_address is not None:
                 address: Address
                 address_found = False
                 for address in entry.person.addresses:
                     street = address.street_complete
                     if self.search_string(street, search_address, search_mode):
```

### Comparing `wowipy-1.1.7/wowipy.egg-info/PKG-INFO` & `wowipy-1.1.8/wowipy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wowipy
-Version: 1.1.7
+Version: 1.1.8
 Summary: OPENWOWI Wowiport API wrapper for python
 Home-page: https://github.com/seb-bau/WowiPy
 Author: Sebastian Bauhaus
 Author-email: sebastian@bytewish.de
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

