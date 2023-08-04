# Comparing `tmp/multilogue-0.0.7.tar.gz` & `tmp/multilogue-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multilogue-0.0.7.tar", last modified: Thu Aug  3 14:11:24 2023, max compression
+gzip compressed data, was "multilogue-0.0.8.tar", last modified: Fri Aug  4 19:46:08 2023, max compression
```

## Comparing `multilogue-0.0.7.tar` & `multilogue-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-03 14:11:24.596764 multilogue-0.0.7/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1067 2023-07-02 15:37:04.000000 multilogue-0.0.7/LICENSE
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      604 2023-08-03 14:11:24.596764 multilogue-0.0.7/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       55 2023-07-02 15:37:04.000000 multilogue-0.0.7/README.md
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      738 2023-08-03 00:19:59.000000 multilogue-0.0.7/pyproject.toml
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-08-03 14:11:24.596764 multilogue-0.0.7/setup.cfg
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-03 14:11:24.592764 multilogue-0.0.7/src/
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-03 14:11:24.592764 multilogue-0.0.7/src/multilogue/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      101 2023-07-29 19:20:27.000000 multilogue-0.0.7/src/multilogue/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1244 2023-07-27 12:09:50.000000 multilogue-0.0.7/src/multilogue/entities.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-07-27 00:36:41.000000 multilogue-0.0.7/src/multilogue/participants.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-03 14:11:24.592764 multilogue-0.0.7/src/multilogue/utilities/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      439 2023-07-30 22:20:03.000000 multilogue-0.0.7/src/multilogue/utilities/__init__.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1849 2023-07-30 22:14:48.000000 multilogue-0.0.7/src/multilogue/utilities/chatgpt.py
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4562 2023-08-03 00:18:39.000000 multilogue-0.0.7/src/multilogue/utilities/githublog.py
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-03 14:11:24.592764 multilogue-0.0.7/src/multilogue.egg-info/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      604 2023-08-03 14:11:24.000000 multilogue-0.0.7/src/multilogue.egg-info/PKG-INFO
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      440 2023-08-03 14:11:24.000000 multilogue-0.0.7/src/multilogue.egg-info/SOURCES.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-08-03 14:11:24.000000 multilogue-0.0.7/src/multilogue.egg-info/dependency_links.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       49 2023-08-03 14:11:24.000000 multilogue-0.0.7/src/multilogue.egg-info/requires.txt
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-08-03 14:11:24.000000 multilogue-0.0.7/src/multilogue.egg-info/top_level.txt
-drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-03 14:11:24.592764 multilogue-0.0.7/tests/
--rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      345 2023-07-27 12:09:50.000000 multilogue-0.0.7/tests/test_entities.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-04 19:46:08.600914 multilogue-0.0.8/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1067 2023-07-02 15:37:04.000000 multilogue-0.0.8/LICENSE
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      763 2023-08-04 19:46:08.600914 multilogue-0.0.8/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      119 2023-08-04 19:43:07.000000 multilogue-0.0.8/README.md
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      833 2023-08-04 19:43:58.000000 multilogue-0.0.8/pyproject.toml
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       38 2023-08-04 19:46:08.600914 multilogue-0.0.8/setup.cfg
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-04 19:46:08.596914 multilogue-0.0.8/src/
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-04 19:46:08.596914 multilogue-0.0.8/src/multilogue/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      101 2023-07-29 19:20:27.000000 multilogue-0.0.8/src/multilogue/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1244 2023-07-27 12:09:50.000000 multilogue-0.0.8/src/multilogue/entities.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      190 2023-07-27 00:36:41.000000 multilogue-0.0.8/src/multilogue/participants.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-04 19:46:08.600914 multilogue-0.0.8/src/multilogue/utilities/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      439 2023-07-30 22:20:03.000000 multilogue-0.0.8/src/multilogue/utilities/__init__.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     1849 2023-07-30 22:14:48.000000 multilogue-0.0.8/src/multilogue/utilities/chatgpt.py
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)     4562 2023-08-04 19:38:14.000000 multilogue-0.0.8/src/multilogue/utilities/githublog.py
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-04 19:46:08.600914 multilogue-0.0.8/src/multilogue.egg-info/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      763 2023-08-04 19:46:08.000000 multilogue-0.0.8/src/multilogue.egg-info/PKG-INFO
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      440 2023-08-04 19:46:08.000000 multilogue-0.0.8/src/multilogue.egg-info/SOURCES.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)        1 2023-08-04 19:46:08.000000 multilogue-0.0.8/src/multilogue.egg-info/dependency_links.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       49 2023-08-04 19:46:08.000000 multilogue-0.0.8/src/multilogue.egg-info/requires.txt
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)       11 2023-08-04 19:46:08.000000 multilogue-0.0.8/src/multilogue.egg-info/top_level.txt
+drwxrwxr-x   0 alxfed    (1001) alxfed    (1001)        0 2023-08-04 19:46:08.600914 multilogue-0.0.8/tests/
+-rw-rw-r--   0 alxfed    (1001) alxfed    (1001)      345 2023-07-27 12:09:50.000000 multilogue-0.0.8/tests/test_entities.py
```

### Comparing `multilogue-0.0.7/LICENSE` & `multilogue-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `multilogue-0.0.7/pyproject.toml` & `multilogue-0.0.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "multilogue"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     {name="Alexander Fedotov", email="alex.fedotov@aol.com"},
 ]
-description = "Multilogue"
+description = "Multilogue is a cooperative game of reasoning entities against ignorance, confusion and misunderstanding."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
 ]
```

### Comparing `multilogue-0.0.7/src/multilogue/entities.py` & `multilogue-0.0.8/src/multilogue/entities.py`

 * *Files identical despite different names*

### Comparing `multilogue-0.0.7/src/multilogue/utilities/chatgpt.py` & `multilogue-0.0.8/src/multilogue/utilities/chatgpt.py`

 * *Files identical despite different names*

### Comparing `multilogue-0.0.7/src/multilogue/utilities/githublog.py` & `multilogue-0.0.8/src/multilogue/utilities/githublog.py`

 * *Files identical despite different names*

