# Comparing `tmp/BloxPy-0.1.13.tar.gz` & `tmp/BloxPy-0.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BloxPy-0.1.13.tar", last modified: Thu Aug  3 22:53:35 2023, max compression
+gzip compressed data, was "BloxPy-0.1.14.tar", last modified: Thu Aug  3 22:59:23 2023, max compression
```

## Comparing `BloxPy-0.1.13.tar` & `BloxPy-0.1.14.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 22:53:35.222433 BloxPy-0.1.13/
-drwxrwxrwx   0        0        0        0 2023-08-03 22:53:35.211434 BloxPy-0.1.13/BloxPy/
--rw-rw-rw-   0        0        0     4009 2023-08-03 22:08:51.000000 BloxPy-0.1.13/BloxPy/Badges.py
--rw-rw-rw-   0        0        0    13520 2023-08-03 21:42:20.000000 BloxPy-0.1.13/BloxPy/Groups.py
--rw-rw-rw-   0        0        0     8146 2023-08-03 20:47:25.000000 BloxPy-0.1.13/BloxPy/Search.py
--rw-rw-rw-   0        0        0    29723 2023-08-03 22:52:06.000000 BloxPy-0.1.13/BloxPy/Users.py
--rw-rw-rw-   0        0        0        0 2023-07-28 21:18:45.000000 BloxPy-0.1.13/BloxPy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-03 22:53:35.217432 BloxPy-0.1.13/BloxPy.egg-info/
--rw-rw-rw-   0        0        0     3675 2023-08-03 22:53:34.000000 BloxPy-0.1.13/BloxPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-08-03 22:53:34.000000 BloxPy-0.1.13/BloxPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 22:53:34.000000 BloxPy-0.1.13/BloxPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-03 22:53:34.000000 BloxPy-0.1.13/BloxPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-08-03 22:53:34.000000 BloxPy-0.1.13/BloxPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1087 2023-08-03 20:13:02.000000 BloxPy-0.1.13/LICENSE
--rw-rw-rw-   0        0        0     3675 2023-08-03 22:53:35.221433 BloxPy-0.1.13/PKG-INFO
--rw-rw-rw-   0        0        0     2739 2023-08-03 20:15:33.000000 BloxPy-0.1.13/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 22:53:35.219433 BloxPy-0.1.13/_exceptions/
--rw-rw-rw-   0        0        0     1774 2023-07-30 22:02:04.000000 BloxPy-0.1.13/_exceptions/RobloxExceptions.py
--rw-rw-rw-   0        0        0      428 2023-07-30 22:03:36.000000 BloxPy-0.1.13/_exceptions/__init__.py
--rw-rw-rw-   0        0        0       42 2023-08-03 22:53:35.222433 BloxPy-0.1.13/setup.cfg
--rw-rw-rw-   0        0        0     1752 2023-08-03 22:52:59.000000 BloxPy-0.1.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:59:23.167670 BloxPy-0.1.14/
+drwxrwxrwx   0        0        0        0 2023-08-03 22:59:23.155673 BloxPy-0.1.14/BloxPy/
+-rw-rw-rw-   0        0        0     4009 2023-08-03 22:08:51.000000 BloxPy-0.1.14/BloxPy/Badges.py
+-rw-rw-rw-   0        0        0    13520 2023-08-03 21:42:20.000000 BloxPy-0.1.14/BloxPy/Groups.py
+-rw-rw-rw-   0        0        0     8146 2023-08-03 20:47:25.000000 BloxPy-0.1.14/BloxPy/Search.py
+-rw-rw-rw-   0        0        0    29753 2023-08-03 22:58:07.000000 BloxPy-0.1.14/BloxPy/Users.py
+-rw-rw-rw-   0        0        0        0 2023-07-28 21:18:45.000000 BloxPy-0.1.14/BloxPy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-03 22:59:23.163671 BloxPy-0.1.14/BloxPy.egg-info/
+-rw-rw-rw-   0        0        0     3675 2023-08-03 22:59:22.000000 BloxPy-0.1.14/BloxPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-08-03 22:59:22.000000 BloxPy-0.1.14/BloxPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 22:59:22.000000 BloxPy-0.1.14/BloxPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-03 22:59:22.000000 BloxPy-0.1.14/BloxPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-03 22:59:22.000000 BloxPy-0.1.14/BloxPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1087 2023-08-03 20:13:02.000000 BloxPy-0.1.14/LICENSE
+-rw-rw-rw-   0        0        0     3675 2023-08-03 22:59:23.167670 BloxPy-0.1.14/PKG-INFO
+-rw-rw-rw-   0        0        0     2739 2023-08-03 20:15:33.000000 BloxPy-0.1.14/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 22:59:23.165669 BloxPy-0.1.14/_exceptions/
+-rw-rw-rw-   0        0        0     1774 2023-07-30 22:02:04.000000 BloxPy-0.1.14/_exceptions/RobloxExceptions.py
+-rw-rw-rw-   0        0        0      428 2023-07-30 22:03:36.000000 BloxPy-0.1.14/_exceptions/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-08-03 22:59:23.168670 BloxPy-0.1.14/setup.cfg
+-rw-rw-rw-   0        0        0     1752 2023-08-03 22:58:56.000000 BloxPy-0.1.14/setup.py
```

### Comparing `BloxPy-0.1.13/BloxPy/Badges.py` & `BloxPy-0.1.14/BloxPy/Badges.py`

 * *Files identical despite different names*

### Comparing `BloxPy-0.1.13/BloxPy/Groups.py` & `BloxPy-0.1.14/BloxPy/Groups.py`

 * *Files identical despite different names*

### Comparing `BloxPy-0.1.13/BloxPy/Search.py` & `BloxPy-0.1.14/BloxPy/Search.py`

 * *Files identical despite different names*

### Comparing `BloxPy-0.1.13/BloxPy/Users.py` & `BloxPy-0.1.14/BloxPy/Users.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,20 +212,20 @@
         elif response.status_code != 200:
             raise RobloxUnexpectedError(f"Unexpected HTTP status code: {response.status_code}")
         else:
             data = response.json()
 
             scales_data = data['scales']
             scales = AvatarScales(
-                height=scales.get('height', None),
-                width=scales.get('width', None),
-                head=scales.get('head', None),
-                depth=scales.get('depth', None),
-                proportion=scales.get('proportion', None),
-                bodyType=scales.get('bodyType', None)
+                height=scales_data.get('height', None),
+                width=scales_data.get('width', None),
+                head=scales_data.get('head', None),
+                depth=scales_data.get('depth', None),
+                proportion=scales_data.get('proportion', None),
+                bodyType=scales_data.get('bodyType', None)
             )
 
             bodyColors_data = data['bodyColors']
             bodyColors = AvatarBodyColors(
                 headColorId=bodyColors_data.get('headColorId', None),
                 torsoColorId=bodyColors_data.get('torsoColorId', None),
                 rightArmColorId=bodyColors_data.get('rightArmColorId', None),
```

### Comparing `BloxPy-0.1.13/BloxPy.egg-info/PKG-INFO` & `BloxPy-0.1.14/BloxPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BloxPy
-Version: 0.1.13
+Version: 0.1.14
 Summary: BloxPy: Your All-in-One Python API wrapper for Roblox Development
 Home-page: https://github.com/Developer-X-0001/BloxPy
 Author: Developer X
 Author-email: developer.x.business@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BloxPy-0.1.13/LICENSE` & `BloxPy-0.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `BloxPy-0.1.13/PKG-INFO` & `BloxPy-0.1.14/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BloxPy
-Version: 0.1.13
+Version: 0.1.14
 Summary: BloxPy: Your All-in-One Python API wrapper for Roblox Development
 Home-page: https://github.com/Developer-X-0001/BloxPy
 Author: Developer X
 Author-email: developer.x.business@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `BloxPy-0.1.13/README.md` & `BloxPy-0.1.14/README.md`

 * *Files identical despite different names*

### Comparing `BloxPy-0.1.13/_exceptions/RobloxExceptions.py` & `BloxPy-0.1.14/_exceptions/RobloxExceptions.py`

 * *Files identical despite different names*

### Comparing `BloxPy-0.1.13/setup.py` & `BloxPy-0.1.14/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 NAME = 'BloxPy'
-VERSION = '0.1.13'
+VERSION = '0.1.14'
 DESCRIPTION = 'BloxPy: Your All-in-One Python API wrapper for Roblox Development'
 LONG_DESCRIPTION = 'BloxPy is the ultimate Python API wrapper for Roblox developers, offering an all-in-one solution to interact with Roblox Public APIs effortlessly. Whether you want to retrieve player data, manage groups, or create dynamic game interactions, BloxPy empowers you to build amazing Roblox experiences with ease.'
 AUTHOR = 'Developer X'
 EMAIL = 'developer.x.business@gmail.com'
 URL = 'https://github.com/Developer-X-0001/BloxPy'
 LICENSE = 'MIT'
 PYTHON_REQUIRES = '>=3.9'
```

