# Comparing `tmp/roapipy-1.0.8.tar.gz` & `tmp/roapipy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\Code\roapipy\dist\tmpca88w5u7\roapipy-1.0.8.tar", last modified: Thu Oct 27 04:49:03 2022, max compression
+gzip compressed data, was "D:\Code\roapipy\dist\tmpyyg697qv\roapipy-1.0.9.tar", last modified: Thu Oct 27 05:12:39 2022, max compression
```

## Comparing `roapipy-1.0.8.tar` & `roapipy-1.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-10-27 04:49:03.633704 roapipy-1.0.8/
--rw-rw-rw-   0        0        0     1085 2022-10-05 15:28:08.000000 roapipy-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     5651 2022-10-27 04:49:03.633704 roapipy-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5201 2022-10-27 04:43:50.000000 roapipy-1.0.8/README.md
--rw-rw-rw-   0        0        0      572 2022-10-27 04:48:40.000000 roapipy-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-10-27 04:49:03.633704 roapipy-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-27 04:49:03.589841 roapipy-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-10-27 04:49:03.611764 roapipy-1.0.8/src/roapipy/
--rw-rw-rw-   0        0        0    18504 2022-10-27 04:28:43.000000 roapipy-1.0.8/src/roapipy/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-27 04:49:03.630714 roapipy-1.0.8/src/roapipy.egg-info/
--rw-rw-rw-   0        0        0     5651 2022-10-27 04:49:03.000000 roapipy-1.0.8/src/roapipy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2022-10-27 04:49:03.000000 roapipy-1.0.8/src/roapipy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-27 04:49:03.000000 roapipy-1.0.8/src/roapipy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2022-10-27 04:49:03.000000 roapipy-1.0.8/src/roapipy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-10-27 05:12:39.451300 roapipy-1.0.9/
+-rw-rw-rw-   0        0        0     1085 2022-10-05 15:28:08.000000 roapipy-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     5808 2022-10-27 05:12:39.450304 roapipy-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5358 2022-10-27 05:11:48.000000 roapipy-1.0.9/README.md
+-rw-rw-rw-   0        0        0      572 2022-10-27 05:11:58.000000 roapipy-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2022-10-27 05:12:39.452297 roapipy-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-10-27 05:12:39.406420 roapipy-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-10-27 05:12:39.429360 roapipy-1.0.9/src/roapipy/
+-rw-rw-rw-   0        0        0    18504 2022-10-27 04:28:43.000000 roapipy-1.0.9/src/roapipy/__init__.py
+drwxrwxrwx   0        0        0        0 2022-10-27 05:12:39.446314 roapipy-1.0.9/src/roapipy.egg-info/
+-rw-rw-rw-   0        0        0     5808 2022-10-27 05:12:39.000000 roapipy-1.0.9/src/roapipy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2022-10-27 05:12:39.000000 roapipy-1.0.9/src/roapipy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-27 05:12:39.000000 roapipy-1.0.9/src/roapipy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2022-10-27 05:12:39.000000 roapipy-1.0.9/src/roapipy.egg-info/top_level.txt
```

### Comparing `roapipy-1.0.8/LICENSE.txt` & `roapipy-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `roapipy-1.0.8/PKG-INFO` & `roapipy-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roapipy
-Version: 1.0.8
+Version: 1.0.9
 Summary: roapipy - A wrapper for the Roblox API built for Python
 Author: Gytis
 Project-URL: Developer, https://discord.com/users/301014178703998987
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -25,15 +25,16 @@
 ### class User()
 Used to interact with users
 #### Info(user)
 Returns information on the user with the given id
 **Parameters:**
 *  **user** ( Any[int(id), str(username)] ) - the user you wish to get information on
 #### Activity(user)
-Returns the activity of the user with the given id
+Returns the activity of the user with the given id.
+**A [roblosecurity](https://ro.py.jmk.gg/dev/roblosecurity/) is __optional__ within the Client’s parameters for this command to give extra information**
 **Parameters:**
 *  **user** ( Any[int(id), str(username)] ) - the user you wish to get the activity of
 #### Groups(user)
 Returns the groups the user with the given id is in
 **Parameters:**
 *  **user** ( Any[int(id), str(username)] ) - the user you wish to get the groups of
 ### class Group()
```

### Comparing `roapipy-1.0.8/README.md` & `roapipy-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 ### class User()
 Used to interact with users
 #### Info(user)
 Returns information on the user with the given id
 **Parameters:**
 *  **user** ( Any[int(id), str(username)] ) - the user you wish to get information on
 #### Activity(user)
-Returns the activity of the user with the given id
+Returns the activity of the user with the given id.
+**A [roblosecurity](https://ro.py.jmk.gg/dev/roblosecurity/) is __optional__ within the Client’s parameters for this command to give extra information**
 **Parameters:**
 *  **user** ( Any[int(id), str(username)] ) - the user you wish to get the activity of
 #### Groups(user)
 Returns the groups the user with the given id is in
 **Parameters:**
 *  **user** ( Any[int(id), str(username)] ) - the user you wish to get the groups of
 ### class Group()
```

### Comparing `roapipy-1.0.8/pyproject.toml` & `roapipy-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 40.0.4", "setuptools_scm >= 2.0.0", "requests"]
 build-backend="setuptools.build_meta"
 
 [project]
 name = "roapipy"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Gytis" },
 ]
 description = "roapipy - A wrapper for the Roblox API built for Python"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `roapipy-1.0.8/src/roapipy/__init__.py` & `roapipy-1.0.9/src/roapipy/__init__.py`

 * *Files identical despite different names*

### Comparing `roapipy-1.0.8/src/roapipy.egg-info/PKG-INFO` & `roapipy-1.0.9/src/roapipy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roapipy
-Version: 1.0.8
+Version: 1.0.9
 Summary: roapipy - A wrapper for the Roblox API built for Python
 Author: Gytis
 Project-URL: Developer, https://discord.com/users/301014178703998987
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
@@ -25,15 +25,16 @@
 ### class User()
 Used to interact with users
 #### Info(user)
 Returns information on the user with the given id
 **Parameters:**
 *  **user** ( Any[int(id), str(username)] ) - the user you wish to get information on
 #### Activity(user)
-Returns the activity of the user with the given id
+Returns the activity of the user with the given id.
+**A [roblosecurity](https://ro.py.jmk.gg/dev/roblosecurity/) is __optional__ within the Client’s parameters for this command to give extra information**
 **Parameters:**
 *  **user** ( Any[int(id), str(username)] ) - the user you wish to get the activity of
 #### Groups(user)
 Returns the groups the user with the given id is in
 **Parameters:**
 *  **user** ( Any[int(id), str(username)] ) - the user you wish to get the groups of
 ### class Group()
```

