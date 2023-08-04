# Comparing `tmp/astro-seeing-1.0.tar.gz` & `tmp/astro-seeing-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-seeing-1.0.tar", last modified: Wed Apr  5 17:19:43 2023, max compression
+gzip compressed data, was "astro-seeing-1.1.tar", last modified: Fri Aug  4 09:57:36 2023, max compression
```

## Comparing `astro-seeing-1.0.tar` & `astro-seeing-1.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-05 17:19:43.393737 astro-seeing-1.0/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-05 17:19:43.387071 astro-seeing-1.0/.github/
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-05 17:19:43.390404 astro-seeing-1.0/.github/workflows/
--rw-r--r--   0 simon     (1000) simon     (1000)      923 2023-03-03 11:47:40.000000 astro-seeing-1.0/.github/workflows/publish.yml
--rw-r--r--   0 simon     (1000) simon     (1000)     1826 2023-03-03 11:47:40.000000 astro-seeing-1.0/.gitignore
--rw-r--r--   0 simon     (1000) simon     (1000)     1064 2023-03-31 16:17:35.000000 astro-seeing-1.0/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1000)     1261 2023-04-05 17:19:43.393737 astro-seeing-1.0/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)      907 2023-04-05 17:13:06.000000 astro-seeing-1.0/README.md
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-05 17:19:43.390404 astro-seeing-1.0/astro_seeing.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)     1261 2023-04-05 17:19:43.000000 astro-seeing-1.0/astro_seeing.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)      750 2023-04-05 17:19:43.000000 astro-seeing-1.0/astro_seeing.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2023-04-05 17:19:43.000000 astro-seeing-1.0/astro_seeing.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       41 2023-04-05 17:19:43.000000 astro-seeing-1.0/astro_seeing.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        7 2023-04-05 17:19:43.000000 astro-seeing-1.0/astro_seeing.egg-info/top_level.txt
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-05 17:19:43.393737 astro-seeing-1.0/astrobigne/
--rw-r--r--   0 simon     (1000) simon     (1000)   507120 2023-01-18 11:40:17.000000 astro-seeing-1.0/astrobigne/AstroBigneDemos.ipynb
--rw-r--r--   0 simon     (1000) simon     (1000)  1214723 2023-01-18 11:40:17.000000 astro-seeing-1.0/astrobigne/Astrobigne.html
--rw-r--r--   0 simon     (1000) simon     (1000)   589594 2023-01-18 11:40:17.000000 astro-seeing-1.0/astrobigne/Astrobigne.ipynb
--rw-r--r--   0 simon     (1000) simon     (1000)  1220785 2023-01-18 11:40:17.000000 astro-seeing-1.0/astrobigne/Astrobigne.slides.html
--rw-r--r--   0 simon     (1000) simon     (1000)    82408 2023-01-18 11:40:17.000000 astro-seeing-1.0/astrobigne/Astrobigne2020.jpg
--rw-r--r--   0 simon     (1000) simon     (1000)    68303 2023-01-18 11:40:17.000000 astro-seeing-1.0/astrobigne/Astrobigne2020_2.jpg
--rw-r--r--   0 simon     (1000) simon     (1000)    10981 2023-01-18 11:40:17.000000 astro-seeing-1.0/astrobigne/Mavis.frm
--rw-r--r--   0 simon     (1000) simon     (1000)     1911 2023-01-18 11:40:17.000000 astro-seeing-1.0/astrobigne/Propagation100.frm
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-05 17:19:43.393737 astro-seeing-1.0/examples/
--rw-r--r--   0 simon     (1000) simon     (1000)     1911 2023-01-18 11:40:17.000000 astro-seeing-1.0/examples/Propagation100.frm
--rw-r--r--   0 simon     (1000) simon     (1000)   570280 2023-01-18 11:40:17.000000 astro-seeing-1.0/examples/examples.ipynb
--rw-r--r--   0 simon     (1000) simon     (1000)      697 2023-04-05 16:59:11.000000 astro-seeing-1.0/pyproject.toml
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-05 17:19:43.393737 astro-seeing-1.0/seeing/
--rw-r--r--   0 simon     (1000) simon     (1000)      400 2023-03-03 11:47:40.000000 astro-seeing-1.0/seeing/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)      155 2023-04-05 17:19:43.000000 astro-seeing-1.0/seeing/_version.py
--rw-r--r--   0 simon     (1000) simon     (1000)     4891 2023-01-18 11:40:17.000000 astro-seeing-1.0/seeing/formulary.py
--rw-r--r--   0 simon     (1000) simon     (1000)    13669 2023-01-18 11:40:17.000000 astro-seeing-1.0/seeing/integrator.py
--rw-r--r--   0 simon     (1000) simon     (1000)      536 2023-01-18 11:40:17.000000 astro-seeing-1.0/seeing/lambdifyDictionaries.py
--rw-r--r--   0 simon     (1000) simon     (1000)     5687 2023-01-18 11:40:17.000000 astro-seeing-1.0/seeing/lambdifyDictionariesGPU.py
--rw-r--r--   0 simon     (1000) simon     (1000)     6158 2023-01-18 11:40:17.000000 astro-seeing-1.0/seeing/sympyHelpers.py
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-04-05 17:19:43.393737 astro-seeing-1.0/setup.cfg
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-04-05 17:19:43.393737 astro-seeing-1.0/tests/
--rw-r--r--   0 simon     (1000) simon     (1000)     2478 2023-01-18 11:40:17.000000 astro-seeing-1.0/tests/coreTests.py
--rw-r--r--   0 simon     (1000) simon     (1000)      919 2023-01-18 11:40:17.000000 astro-seeing-1.0/tests/integratorTests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:57:36.766313 astro-seeing-1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:57:36.750313 astro-seeing-1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:57:36.754313 astro-seeing-1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-08-04 09:57:20.000000 astro-seeing-1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-04 09:57:20.000000 astro-seeing-1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 09:57:20.000000 astro-seeing-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-04 09:57:36.766313 astro-seeing-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-08-04 09:57:20.000000 astro-seeing-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:57:36.754313 astro-seeing-1.1/astro_seeing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-08-04 09:57:36.000000 astro-seeing-1.1/astro_seeing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-04 09:57:36.000000 astro-seeing-1.1/astro_seeing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:57:36.000000 astro-seeing-1.1/astro_seeing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 09:57:36.000000 astro-seeing-1.1/astro_seeing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 09:57:36.000000 astro-seeing-1.1/astro_seeing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:57:36.762313 astro-seeing-1.1/astrobigne/
+-rw-r--r--   0 runner    (1001) docker     (123)   507120 2023-08-04 09:57:20.000000 astro-seeing-1.1/astrobigne/AstroBigneDemos.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1214723 2023-08-04 09:57:20.000000 astro-seeing-1.1/astrobigne/Astrobigne.html
+-rw-r--r--   0 runner    (1001) docker     (123)   589594 2023-08-04 09:57:20.000000 astro-seeing-1.1/astrobigne/Astrobigne.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1220785 2023-08-04 09:57:20.000000 astro-seeing-1.1/astrobigne/Astrobigne.slides.html
+-rw-r--r--   0 runner    (1001) docker     (123)    82408 2023-08-04 09:57:20.000000 astro-seeing-1.1/astrobigne/Astrobigne2020.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    68303 2023-08-04 09:57:20.000000 astro-seeing-1.1/astrobigne/Astrobigne2020_2.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-08-04 09:57:20.000000 astro-seeing-1.1/astrobigne/Mavis.frm
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-04 09:57:20.000000 astro-seeing-1.1/astrobigne/Propagation100.frm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:57:36.762313 astro-seeing-1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-08-04 09:57:20.000000 astro-seeing-1.1/examples/Propagation100.frm
+-rw-r--r--   0 runner    (1001) docker     (123)   570280 2023-08-04 09:57:20.000000 astro-seeing-1.1/examples/examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-08-04 09:57:20.000000 astro-seeing-1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:57:36.766313 astro-seeing-1.1/seeing/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-04 09:57:20.000000 astro-seeing-1.1/seeing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-04 09:57:36.000000 astro-seeing-1.1/seeing/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-08-04 09:57:20.000000 astro-seeing-1.1/seeing/formulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13669 2023-08-04 09:57:20.000000 astro-seeing-1.1/seeing/integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-04 09:57:20.000000 astro-seeing-1.1/seeing/lambdifyDictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-08-04 09:57:20.000000 astro-seeing-1.1/seeing/lambdifyDictionariesGPU.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-08-04 09:57:20.000000 astro-seeing-1.1/seeing/sympyHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 09:57:36.766313 astro-seeing-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:57:36.766313 astro-seeing-1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-08-04 09:57:20.000000 astro-seeing-1.1/tests/coreTests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-08-04 09:57:20.000000 astro-seeing-1.1/tests/integratorTests.py
```

### Comparing `astro-seeing-1.0/.github/workflows/publish.yml` & `astro-seeing-1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/.gitignore` & `astro-seeing-1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/LICENSE` & `astro-seeing-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/PKG-INFO` & `astro-seeing-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-seeing
-Version: 1.0
+Version: 1.1
 Summary: Sympy Expressions Evaluation Implemented oN the GPU
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/SEEING
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
```

### Comparing `astro-seeing-1.0/README.md` & `astro-seeing-1.1/README.md`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/astro_seeing.egg-info/PKG-INFO` & `astro-seeing-1.1/astro_seeing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-seeing
-Version: 1.0
+Version: 1.1
 Summary: Sympy Expressions Evaluation Implemented oN the GPU
 Author-email: Fabio Rossi <fabio.rossi@inaf.it>
 License: MIT License
 Project-URL: repository, https://github.com/astro-tiptop/SEEING
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: gpu
```

### Comparing `astro-seeing-1.0/astro_seeing.egg-info/SOURCES.txt` & `astro-seeing-1.1/astro_seeing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/astrobigne/AstroBigneDemos.ipynb` & `astro-seeing-1.1/astrobigne/AstroBigneDemos.ipynb`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/astrobigne/Astrobigne.html` & `astro-seeing-1.1/astrobigne/Astrobigne.html`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/astrobigne/Astrobigne.ipynb` & `astro-seeing-1.1/astrobigne/Astrobigne.ipynb`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/astrobigne/Astrobigne.slides.html` & `astro-seeing-1.1/astrobigne/Astrobigne.slides.html`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/astrobigne/Astrobigne2020.jpg` & `astro-seeing-1.1/astrobigne/Astrobigne2020.jpg`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/astrobigne/Astrobigne2020_2.jpg` & `astro-seeing-1.1/astrobigne/Astrobigne2020_2.jpg`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/astrobigne/Mavis.frm` & `astro-seeing-1.1/astrobigne/Mavis.frm`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/astrobigne/Propagation100.frm` & `astro-seeing-1.1/astrobigne/Propagation100.frm`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/examples/Propagation100.frm` & `astro-seeing-1.1/examples/Propagation100.frm`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/examples/examples.ipynb` & `astro-seeing-1.1/examples/examples.ipynb`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/pyproject.toml` & `astro-seeing-1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/seeing/formulary.py` & `astro-seeing-1.1/seeing/formulary.py`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/seeing/integrator.py` & `astro-seeing-1.1/seeing/integrator.py`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/seeing/lambdifyDictionaries.py` & `astro-seeing-1.1/seeing/lambdifyDictionaries.py`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/seeing/lambdifyDictionariesGPU.py` & `astro-seeing-1.1/seeing/lambdifyDictionariesGPU.py`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/seeing/sympyHelpers.py` & `astro-seeing-1.1/seeing/sympyHelpers.py`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/tests/coreTests.py` & `astro-seeing-1.1/tests/coreTests.py`

 * *Files identical despite different names*

### Comparing `astro-seeing-1.0/tests/integratorTests.py` & `astro-seeing-1.1/tests/integratorTests.py`

 * *Files identical despite different names*

