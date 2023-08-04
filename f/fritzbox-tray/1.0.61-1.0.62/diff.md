# Comparing `tmp/fritzbox-tray-1.0.61.tar.gz` & `tmp/fritzbox-tray-1.0.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fritzbox-tray-1.0.61.tar", last modified: Tue Jul 11 17:58:40 2023, max compression
+gzip compressed data, was "fritzbox-tray-1.0.62.tar", last modified: Fri Aug  4 07:01:55 2023, max compression
```

## Comparing `fritzbox-tray-1.0.61.tar` & `fritzbox-tray-1.0.62.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 17:58:40.246251 fritzbox-tray-1.0.61/
--rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 fritzbox-tray-1.0.61/LICENSE
--rw-rw-rw-   0        0        0     3944 2023-07-11 17:58:40.239415 fritzbox-tray-1.0.61/PKG-INFO
--rw-rw-rw-   0        0        0     2881 2023-05-27 17:18:19.000000 fritzbox-tray-1.0.61/README.md
--rw-rw-rw-   0        0        0       42 2023-07-11 17:58:40.246251 fritzbox-tray-1.0.61/setup.cfg
--rw-rw-rw-   0        0        0     2637 2023-07-11 17:41:34.000000 fritzbox-tray-1.0.61/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:58:40.199970 fritzbox-tray-1.0.61/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 17:58:40.212778 fritzbox-tray-1.0.61/src/fritzbox_tray/
--rw-rw-rw-   0        0        0        0 2023-01-07 15:15:29.000000 fritzbox-tray-1.0.61/src/fritzbox_tray/__init__.py
--rw-rw-rw-   0        0        0     5007 2023-04-30 12:36:27.000000 fritzbox-tray-1.0.61/src/fritzbox_tray/__main__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:58:40.235458 fritzbox-tray-1.0.61/src/fritzbox_tray/resources/
--rw-rw-rw-   0        0        0   121004 2023-01-08 16:34:44.000000 fritzbox-tray-1.0.61/src/fritzbox_tray/resources/ft.ico
-drwxrwxrwx   0        0        0        0 2023-07-11 17:58:40.234456 fritzbox-tray-1.0.61/src/fritzbox_tray.egg-info/
--rw-rw-rw-   0        0        0     3944 2023-07-11 17:58:40.000000 fritzbox-tray-1.0.61/src/fritzbox_tray.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2023-07-11 17:58:40.000000 fritzbox-tray-1.0.61/src/fritzbox_tray.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 17:58:40.000000 fritzbox-tray-1.0.61/src/fritzbox_tray.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-11 17:58:40.000000 fritzbox-tray-1.0.61/src/fritzbox_tray.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      129 2023-07-11 17:58:40.000000 fritzbox-tray-1.0.61/src/fritzbox_tray.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-07-11 17:58:40.000000 fritzbox-tray-1.0.61/src/fritzbox_tray.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 07:01:55.801707 fritzbox-tray-1.0.62/
+-rw-rw-rw-   0        0        0    35823 2023-01-08 18:15:51.000000 fritzbox-tray-1.0.62/LICENSE
+-rw-rw-rw-   0        0        0     3944 2023-08-04 07:01:55.795706 fritzbox-tray-1.0.62/PKG-INFO
+-rw-rw-rw-   0        0        0     2881 2023-05-27 17:18:19.000000 fritzbox-tray-1.0.62/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 07:01:55.801707 fritzbox-tray-1.0.62/setup.cfg
+-rw-rw-rw-   0        0        0     2637 2023-08-04 06:45:53.000000 fritzbox-tray-1.0.62/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:01:55.754709 fritzbox-tray-1.0.62/src/
+drwxrwxrwx   0        0        0        0 2023-08-04 07:01:55.767707 fritzbox-tray-1.0.62/src/fritzbox_tray/
+-rw-rw-rw-   0        0        0        0 2023-01-07 15:15:29.000000 fritzbox-tray-1.0.62/src/fritzbox_tray/__init__.py
+-rw-rw-rw-   0        0        0     5007 2023-04-30 12:36:27.000000 fritzbox-tray-1.0.62/src/fritzbox_tray/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 07:01:55.791707 fritzbox-tray-1.0.62/src/fritzbox_tray/resources/
+-rw-rw-rw-   0        0        0   121004 2023-01-08 16:34:44.000000 fritzbox-tray-1.0.62/src/fritzbox_tray/resources/ft.ico
+drwxrwxrwx   0        0        0        0 2023-08-04 07:01:55.789707 fritzbox-tray-1.0.62/src/fritzbox_tray.egg-info/
+-rw-rw-rw-   0        0        0     3944 2023-08-04 07:01:55.000000 fritzbox-tray-1.0.62/src/fritzbox_tray.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2023-08-04 07:01:55.000000 fritzbox-tray-1.0.62/src/fritzbox_tray.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 07:01:55.000000 fritzbox-tray-1.0.62/src/fritzbox_tray.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-08-04 07:01:55.000000 fritzbox-tray-1.0.62/src/fritzbox_tray.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      130 2023-08-04 07:01:55.000000 fritzbox-tray-1.0.62/src/fritzbox_tray.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-04 07:01:55.000000 fritzbox-tray-1.0.62/src/fritzbox_tray.egg-info/top_level.txt
```

### Comparing `fritzbox-tray-1.0.61/LICENSE` & `fritzbox-tray-1.0.62/LICENSE`

 * *Files identical despite different names*

### Comparing `fritzbox-tray-1.0.61/PKG-INFO` & `fritzbox-tray-1.0.62/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fritzbox-tray
-Version: 1.0.61
+Version: 1.0.62
 Summary: A system tray application for interacting with FRITZ!Box devices.
 Home-page: https://github.com/aviolaris/fritzbox-tray
 Author: Andreas Violaris
 Keywords: fritz,fritzbox,fritz-box,fritzbox-tray,fritzbox_tray,avm-fritz,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `fritzbox-tray-1.0.61/README.md` & `fritzbox-tray-1.0.62/README.md`

 * *Files identical despite different names*

### Comparing `fritzbox-tray-1.0.61/setup.py` & `fritzbox-tray-1.0.62/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     long_description = f.read()
 
 with open('requirements.txt', encoding='utf-8') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='fritzbox-tray',
-    version='1.0.61',
+    version='1.0.62',
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     package_data={
         "fritzbox_tray": ["*.py"],
         "fritzbox_tray.resources": ["*.ico"],
     },
     description='A system tray application for interacting with FRITZ!Box devices.',
```

### Comparing `fritzbox-tray-1.0.61/src/fritzbox_tray/__main__.py` & `fritzbox-tray-1.0.62/src/fritzbox_tray/__main__.py`

 * *Files identical despite different names*

### Comparing `fritzbox-tray-1.0.61/src/fritzbox_tray/resources/ft.ico` & `fritzbox-tray-1.0.62/src/fritzbox_tray/resources/ft.ico`

 * *Files identical despite different names*

### Comparing `fritzbox-tray-1.0.61/src/fritzbox_tray.egg-info/PKG-INFO` & `fritzbox-tray-1.0.62/src/fritzbox_tray.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fritzbox-tray
-Version: 1.0.61
+Version: 1.0.62
 Summary: A system tray application for interacting with FRITZ!Box devices.
 Home-page: https://github.com/aviolaris/fritzbox-tray
 Author: Andreas Violaris
 Keywords: fritz,fritzbox,fritz-box,fritzbox-tray,fritzbox_tray,avm-fritz,tray,python,pypi,python3,tray,tray-application,pypi-package,tray-app
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: Microsoft :: Windows
```

