# Comparing `tmp/taku-0.3.0.tar.gz` & `tmp/taku-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taku-0.3.0.tar", last modified: Fri Aug  4 13:04:19 2023, max compression
+gzip compressed data, was "taku-0.7.0.tar", last modified: Fri Aug  4 13:16:55 2023, max compression
```

## Comparing `taku-0.3.0.tar` & `taku-0.7.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 huangjh   (1000) huangjh   (1000)        0 2023-08-04 13:04:19.678811 taku-0.3.0/
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)      937 2023-08-04 13:04:19.678811 taku-0.3.0/PKG-INFO
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)      509 2023-08-04 12:58:49.000000 taku-0.3.0/README.md
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)      442 2023-08-04 13:03:38.000000 taku-0.3.0/pyproject.toml
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)       38 2023-08-04 13:04:19.678811 taku-0.3.0/setup.cfg
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)      929 2023-08-04 12:56:58.000000 taku-0.3.0/setup.py
-drwxrwxr-x   0 huangjh   (1000) huangjh   (1000)        0 2023-08-04 13:04:19.678811 taku-0.3.0/taku/
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)      468 2023-08-04 13:03:38.000000 taku-0.3.0/taku/__init__.py
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)     1215 2023-08-04 12:57:18.000000 taku-0.3.0/taku/dataset.py
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)     5901 2023-08-04 12:57:23.000000 taku-0.3.0/taku/executors.py
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)    18787 2023-08-04 12:57:31.000000 taku-0.3.0/taku/pipeline.py
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)     4829 2023-08-04 12:57:37.000000 taku-0.3.0/taku/task.py
-drwxrwxr-x   0 huangjh   (1000) huangjh   (1000)        0 2023-08-04 13:04:19.678811 taku-0.3.0/taku.egg-info/
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)      937 2023-08-04 13:04:19.000000 taku-0.3.0/taku.egg-info/PKG-INFO
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)      272 2023-08-04 13:04:19.000000 taku-0.3.0/taku.egg-info/SOURCES.txt
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)        1 2023-08-04 13:04:19.000000 taku-0.3.0/taku.egg-info/dependency_links.txt
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)       22 2023-08-04 13:04:19.000000 taku-0.3.0/taku.egg-info/requires.txt
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)        5 2023-08-04 13:04:19.000000 taku-0.3.0/taku.egg-info/top_level.txt
-drwxrwxr-x   0 huangjh   (1000) huangjh   (1000)        0 2023-08-04 13:04:19.678811 taku-0.3.0/tests/
--rw-rw-r--   0 huangjh   (1000) huangjh   (1000)     3956 2023-08-04 12:57:44.000000 taku-0.3.0/tests/test_taku.py
+drwxrwxr-x   0 huangjh   (1000) huangjh   (1000)        0 2023-08-04 13:16:55.335558 taku-0.7.0/
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)     2087 2023-08-04 13:16:55.335558 taku-0.7.0/PKG-INFO
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)     1659 2023-08-04 13:16:52.000000 taku-0.7.0/README.md
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)      442 2023-08-04 13:16:53.000000 taku-0.7.0/pyproject.toml
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)       38 2023-08-04 13:16:55.335558 taku-0.7.0/setup.cfg
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)      930 2023-08-04 13:09:38.000000 taku-0.7.0/setup.py
+drwxrwxr-x   0 huangjh   (1000) huangjh   (1000)        0 2023-08-04 13:16:55.335558 taku-0.7.0/taku/
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)      468 2023-08-04 13:16:53.000000 taku-0.7.0/taku/__init__.py
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)     1215 2023-08-04 12:57:18.000000 taku-0.7.0/taku/dataset.py
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)     5901 2023-08-04 12:57:23.000000 taku-0.7.0/taku/executors.py
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)    18787 2023-08-04 12:57:31.000000 taku-0.7.0/taku/pipeline.py
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)     4829 2023-08-04 12:57:37.000000 taku-0.7.0/taku/task.py
+drwxrwxr-x   0 huangjh   (1000) huangjh   (1000)        0 2023-08-04 13:16:55.335558 taku-0.7.0/taku.egg-info/
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)     2087 2023-08-04 13:16:55.000000 taku-0.7.0/taku.egg-info/PKG-INFO
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)      272 2023-08-04 13:16:55.000000 taku-0.7.0/taku.egg-info/SOURCES.txt
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)        1 2023-08-04 13:16:55.000000 taku-0.7.0/taku.egg-info/dependency_links.txt
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)       23 2023-08-04 13:16:55.000000 taku-0.7.0/taku.egg-info/requires.txt
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)        5 2023-08-04 13:16:55.000000 taku-0.7.0/taku.egg-info/top_level.txt
+drwxrwxr-x   0 huangjh   (1000) huangjh   (1000)        0 2023-08-04 13:16:55.335558 taku-0.7.0/tests/
+-rw-rw-r--   0 huangjh   (1000) huangjh   (1000)     3956 2023-08-04 12:57:44.000000 taku-0.7.0/tests/test_taku.py
```

### Comparing `taku-0.3.0/setup.py` & `taku-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,12 @@
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3 :: Only"
     ],
     keywords=['task', 'manager'],
     python_requires='>=3.6',
     install_requires=[
         "logging",
-        "omegaconf"
+        "omegaconf",
         "rich",
     ],
     include_package_data=True,
 )
```

### Comparing `taku-0.3.0/taku/dataset.py` & `taku-0.7.0/taku/dataset.py`

 * *Files identical despite different names*

### Comparing `taku-0.3.0/taku/executors.py` & `taku-0.7.0/taku/executors.py`

 * *Files identical despite different names*

### Comparing `taku-0.3.0/taku/pipeline.py` & `taku-0.7.0/taku/pipeline.py`

 * *Files identical despite different names*

### Comparing `taku-0.3.0/taku/task.py` & `taku-0.7.0/taku/task.py`

 * *Files identical despite different names*

### Comparing `taku-0.3.0/tests/test_taku.py` & `taku-0.7.0/tests/test_taku.py`

 * *Files identical despite different names*

