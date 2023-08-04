# Comparing `tmp/PyLandslide-0.0.2.tar.gz` & `tmp/PyLandslide-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyLandslide-0.0.2.tar", last modified: Fri Aug  4 16:59:51 2023, max compression
+gzip compressed data, was "dist\PyLandslide-0.0.3.tar", last modified: Fri Aug  4 17:22:43 2023, max compression
```

## Comparing `PyLandslide-0.0.2.tar` & `PyLandslide-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 16:59:51.769129 PyLandslide-0.0.2/
--rw-rw-rw-   0        0        0    35823 2023-07-24 12:23:37.000000 PyLandslide-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      648 2023-08-04 16:59:51.769129 PyLandslide-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-04 16:59:51.753130 PyLandslide-0.0.2/PyLandslide/
--rw-rw-rw-   0        0        0      125 2023-07-25 14:20:54.000000 PyLandslide-0.0.2/PyLandslide/__init__.py
--rw-rw-rw-   0        0        0     2826 2023-07-29 22:57:27.000000 PyLandslide-0.0.2/PyLandslide/cli.py
--rw-rw-rw-   0        0        0        0 2023-07-25 14:20:54.000000 PyLandslide-0.0.2/PyLandslide/core.py
--rw-rw-rw-   0        0        0    13682 2023-07-29 23:25:30.000000 PyLandslide-0.0.2/PyLandslide/sensitivity.py
--rw-rw-rw-   0        0        0     8147 2023-07-29 21:05:23.000000 PyLandslide-0.0.2/PyLandslide/weightrange.py
--rw-rw-rw-   0        0        0     5549 2023-07-29 18:02:10.000000 PyLandslide-0.0.2/PyLandslide/weightrange_preparation.py
-drwxrwxrwx   0        0        0        0 2023-08-04 16:59:51.767130 PyLandslide-0.0.2/PyLandslide.egg-info/
--rw-rw-rw-   0        0        0      648 2023-08-04 16:59:50.000000 PyLandslide-0.0.2/PyLandslide.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-08-04 16:59:51.000000 PyLandslide-0.0.2/PyLandslide.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 16:59:50.000000 PyLandslide-0.0.2/PyLandslide.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-08-04 16:59:51.000000 PyLandslide-0.0.2/PyLandslide.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2023-08-04 16:59:51.000000 PyLandslide-0.0.2/PyLandslide.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-04 16:59:51.000000 PyLandslide-0.0.2/PyLandslide.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      386 2023-08-04 16:46:44.000000 PyLandslide-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 16:59:51.770129 PyLandslide-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-08-04 16:56:39.000000 PyLandslide-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:22:43.000000 PyLandslide-0.0.3/
+-rw-rw-rw-   0        0        0    35823 2023-07-24 12:23:37.000000 PyLandslide-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      680 2023-08-04 17:22:43.000000 PyLandslide-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-04 17:22:43.000000 PyLandslide-0.0.3/PyLandslide/
+-rw-rw-rw-   0        0        0     2826 2023-07-29 22:57:27.000000 PyLandslide-0.0.3/PyLandslide/cli.py
+-rw-rw-rw-   0        0        0        0 2023-07-25 14:20:54.000000 PyLandslide-0.0.3/PyLandslide/core.py
+-rw-rw-rw-   0        0        0    13682 2023-07-29 23:25:30.000000 PyLandslide-0.0.3/PyLandslide/sensitivity.py
+-rw-rw-rw-   0        0        0     8147 2023-07-29 21:05:23.000000 PyLandslide-0.0.3/PyLandslide/weightrange.py
+-rw-rw-rw-   0        0        0     5549 2023-07-29 18:02:10.000000 PyLandslide-0.0.3/PyLandslide/weightrange_preparation.py
+-rw-rw-rw-   0        0        0      125 2023-07-25 14:20:54.000000 PyLandslide-0.0.3/PyLandslide/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:22:43.000000 PyLandslide-0.0.3/PyLandslide.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-04 17:22:42.000000 PyLandslide-0.0.3/PyLandslide.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-08-04 17:22:42.000000 PyLandslide-0.0.3/PyLandslide.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      680 2023-08-04 17:22:42.000000 PyLandslide-0.0.3/PyLandslide.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-08-04 17:22:42.000000 PyLandslide-0.0.3/PyLandslide.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       12 2023-08-04 17:22:42.000000 PyLandslide-0.0.3/PyLandslide.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      386 2023-08-04 16:46:44.000000 PyLandslide-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 17:22:43.000000 PyLandslide-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      944 2023-08-04 17:22:28.000000 PyLandslide-0.0.3/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `PyLandslide-0.0.2/LICENSE` & `PyLandslide-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.0.2/PKG-INFO` & `PyLandslide-0.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: PyLandslide
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for landslide hazard uncertainty analysis.
 Home-page: https://github.com/IERRG/PyLandslide
 Author: Mohammed Basheer
 Author-email: mohammedadamabbaker@gmail.com
 License: GNU
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `PyLandslide-0.0.2/PyLandslide/cli.py` & `PyLandslide-0.0.3/PyLandslide/cli.py`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.0.2/PyLandslide/sensitivity.py` & `PyLandslide-0.0.3/PyLandslide/sensitivity.py`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.0.2/PyLandslide/weightrange.py` & `PyLandslide-0.0.3/PyLandslide/weightrange.py`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.0.2/PyLandslide/weightrange_preparation.py` & `PyLandslide-0.0.3/PyLandslide/weightrange_preparation.py`

 * *Files identical despite different names*

### Comparing `PyLandslide-0.0.2/PyLandslide.egg-info/PKG-INFO` & `PyLandslide-0.0.3/PyLandslide.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 Metadata-Version: 2.1
 Name: PyLandslide
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for landslide hazard uncertainty analysis.
 Home-page: https://github.com/IERRG/PyLandslide
 Author: Mohammed Basheer
 Author-email: mohammedadamabbaker@gmail.com
 License: GNU
+Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `PyLandslide-0.0.2/setup.py` & `PyLandslide-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='PyLandslide',
-    version='0.0.2',
+    version='0.0.3',
     description='Tools for landslide hazard uncertainty analysis.',
     url='https://github.com/IERRG/PyLandslide',
     author='Mohammed Basheer',
     author_email='mohammedadamabbaker@gmail.com',
     license='GNU',
-    install_requires=["gdal", "scikit-learn", "scipy", "pandas", "numpy", "click"],
+    install_requires=[],
     packages=find_packages(),
     package_data={
         'PyLandslide': ['json/*.json'],
     },
     entry_points={
         'console_scripts': ['PyLandslide=PyLandslide.cli:start_cli'],
     },
```

