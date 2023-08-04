# Comparing `tmp/evodiff-0.0.4.tar.gz` & `tmp/evodiff-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evodiff-0.0.4.tar", last modified: Thu Aug  3 23:44:13 2023, max compression
+gzip compressed data, was "evodiff-0.0.5.tar", last modified: Fri Aug  4 17:20:10 2023, max compression
```

## Comparing `evodiff-0.0.4.tar` & `evodiff-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,29 @@
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 23:44:13.160400 evodiff-0.0.4/
--rw-r--r--   0 nityathakkar   (501) staff       (20)     1141 2023-07-27 13:33:47.000000 evodiff-0.0.4/LICENSE
--rw-r--r--   0 nityathakkar   (501) staff       (20)       29 2023-08-03 23:42:44.000000 evodiff-0.0.4/MANIFEST.in
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6883 2023-08-03 23:44:13.159973 evodiff-0.0.4/PKG-INFO
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6431 2023-08-03 15:34:17.000000 evodiff-0.0.4/README.md
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 23:44:13.078410 evodiff-0.0.4/evodiff/
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 23:44:13.085296 evodiff-0.0.4/evodiff/config/
--rw-r--r--   0 nityathakkar   (501) staff       (20)      417 2023-07-27 13:33:47.000000 evodiff-0.0.4/evodiff/config/config38M.json
--rw-r--r--   0 nityathakkar   (501) staff       (20)      398 2023-07-27 13:33:47.000000 evodiff-0.0.4/evodiff/config/config640M.json
--rw-r--r--   0 nityathakkar   (501) staff       (20)      352 2023-07-27 13:33:47.000000 evodiff-0.0.4/evodiff/config/configMSA-600M.json
--rw-r--r--   0 nityathakkar   (501) staff       (20)      348 2023-07-27 13:33:47.000000 evodiff-0.0.4/evodiff/config/configMSA.json
-drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-03 23:44:13.159350 evodiff-0.0.4/evodiff/evodiff.egg-info/
--rw-r--r--   0 nityathakkar   (501) staff       (20)     6883 2023-08-03 23:44:12.000000 evodiff-0.0.4/evodiff/evodiff.egg-info/PKG-INFO
--rw-r--r--   0 nityathakkar   (501) staff       (20)      335 2023-08-03 23:44:13.000000 evodiff-0.0.4/evodiff/evodiff.egg-info/SOURCES.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)        1 2023-08-03 23:44:12.000000 evodiff-0.0.4/evodiff/evodiff.egg-info/dependency_links.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)        1 2023-08-03 23:44:12.000000 evodiff-0.0.4/evodiff/evodiff.egg-info/top_level.txt
--rw-r--r--   0 nityathakkar   (501) staff       (20)      307 2023-08-03 23:42:53.000000 evodiff-0.0.4/pyproject.toml
--rw-r--r--   0 nityathakkar   (501) staff       (20)       38 2023-08-03 23:44:13.160529 evodiff-0.0.4/setup.cfg
--rw-r--r--   0 nityathakkar   (501) staff       (20)      814 2023-08-03 23:44:07.000000 evodiff-0.0.4/setup.py
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:20:10.232364 evodiff-0.0.5/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     1141 2023-07-27 13:33:47.000000 evodiff-0.0.5/LICENSE
+-rw-r--r--   0 nityathakkar   (501) staff       (20)       16 2023-08-04 17:18:36.000000 evodiff-0.0.5/MANIFEST.in
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6882 2023-08-04 17:20:10.231554 evodiff-0.0.5/PKG-INFO
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6431 2023-08-03 15:34:17.000000 evodiff-0.0.5/README.md
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:20:10.158344 evodiff-0.0.5/config/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      417 2023-07-27 13:33:47.000000 evodiff-0.0.5/config/config38M.json
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      398 2023-07-27 13:33:47.000000 evodiff-0.0.5/config/config640M.json
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      352 2023-07-27 13:33:47.000000 evodiff-0.0.5/config/configMSA-600M.json
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      348 2023-07-27 13:33:47.000000 evodiff-0.0.5/config/configMSA.json
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:20:10.165626 evodiff-0.0.5/evodiff/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      215 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/__init__.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    14694 2023-08-03 01:27:58.000000 evodiff-0.0.5/evodiff/collaters.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      406 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/constants.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    22358 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/data.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    12206 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/losses.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      914 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/metrics.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    12973 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/model.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    25379 2023-07-27 13:33:47.000000 evodiff-0.0.5/evodiff/plot.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    11829 2023-08-04 17:19:48.000000 evodiff-0.0.5/evodiff/pretrained.py
+-rw-r--r--   0 nityathakkar   (501) staff       (20)    16217 2023-08-03 01:27:58.000000 evodiff-0.0.5/evodiff/utils.py
+drwxr-xr-x   0 nityathakkar   (501) staff       (20)        0 2023-08-04 17:20:10.231102 evodiff-0.0.5/evodiff.egg-info/
+-rw-r--r--   0 nityathakkar   (501) staff       (20)     6882 2023-08-04 17:20:09.000000 evodiff-0.0.5/evodiff.egg-info/PKG-INFO
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      458 2023-08-04 17:20:10.000000 evodiff-0.0.5/evodiff.egg-info/SOURCES.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)        1 2023-08-04 17:20:09.000000 evodiff-0.0.5/evodiff.egg-info/dependency_links.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)        8 2023-08-04 17:20:09.000000 evodiff-0.0.5/evodiff.egg-info/top_level.txt
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      307 2023-08-04 17:18:33.000000 evodiff-0.0.5/pyproject.toml
+-rw-r--r--   0 nityathakkar   (501) staff       (20)       38 2023-08-04 17:20:10.232517 evodiff-0.0.5/setup.cfg
+-rw-r--r--   0 nityathakkar   (501) staff       (20)      799 2023-08-04 17:18:38.000000 evodiff-0.0.5/setup.py
```

### Comparing `evodiff-0.0.4/LICENSE` & `evodiff-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.4/PKG-INFO` & `evodiff-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: evodiff
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for generation of protein sequences and evolutionary alignments via discrete diffusion models
-Home-page: https://github.com/pypa/sampleproject
+Home-page: https://github.com/microsoft/evodiff
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `evodiff-0.0.4/README.md` & `evodiff-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `evodiff-0.0.4/evodiff/evodiff.egg-info/PKG-INFO` & `evodiff-0.0.5/evodiff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: evodiff
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for generation of protein sequences and evolutionary alignments via discrete diffusion models
-Home-page: https://github.com/pypa/sampleproject
+Home-page: https://github.com/microsoft/evodiff
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `evodiff-0.0.4/setup.py` & `evodiff-0.0.5/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="evodiff", # Replace with your own username
-    version="0.0.4",
+    version="0.0.5",
     description="Python package for generation of protein sequences and evolutionary alignments via discrete diffusion models",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/pypa/sampleproject",
-    packages=setuptools.find_packages(where="evodiff"),
+    url="https://github.com/microsoft/evodiff",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.8.5',
-    include_package_data=True,
-    package_dir = {"": "evodiff"},
-    # package_data={'evodiff': ['*.json']},
+    # include_package_data=True,
+    # package_dir = {"": "config"},
+    packages=setuptools.find_packages(),
+    package_data={'': ['config/*.json']},
 )
```

