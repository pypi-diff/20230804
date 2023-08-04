# Comparing `tmp/remotion_lambda-4.0.16.tar.gz` & `tmp/remotion_lambda-4.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotion_lambda-4.0.16.tar", last modified: Thu Aug  3 07:56:00 2023, max compression
+gzip compressed data, was "remotion_lambda-4.0.17.tar", last modified: Fri Aug  4 15:48:56 2023, max compression
```

## Comparing `remotion_lambda-4.0.16.tar` & `remotion_lambda-4.0.17.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-03 07:56:00.861702 remotion_lambda-4.0.16/
--rw-r--r--   0 jonathanburger   (501) staff       (20)     2512 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/LICENSE
--rw-r--r--   0 jonathanburger   (501) staff       (20)      427 2023-08-03 07:56:00.861584 remotion_lambda-4.0.16/PKG-INFO
--rw-r--r--   0 jonathanburger   (501) staff       (20)       26 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/README.md
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-03 07:56:00.860726 remotion_lambda-4.0.16/remotion_lambda/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      202 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/remotion_lambda/__init__.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)     5252 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/remotion_lambda/models.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)     6064 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/remotion_lambda/remotionclient.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)       84 2023-08-03 07:29:54.000000 remotion_lambda-4.0.16/remotion_lambda/version.py
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-03 07:56:00.861110 remotion_lambda-4.0.16/remotion_lambda.egg-info/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      427 2023-08-03 07:56:00.000000 remotion_lambda-4.0.16/remotion_lambda.egg-info/PKG-INFO
--rw-r--r--   0 jonathanburger   (501) staff       (20)      384 2023-08-03 07:56:00.000000 remotion_lambda-4.0.16/remotion_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)        1 2023-08-03 07:56:00.000000 remotion_lambda-4.0.16/remotion_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-03 07:56:00.000000 remotion_lambda-4.0.16/remotion_lambda.egg-info/top_level.txt
--rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-03 07:56:00.861823 remotion_lambda-4.0.16/setup.cfg
--rw-r--r--   0 jonathanburger   (501) staff       (20)      753 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/setup.py
-drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-03 07:56:00.861440 remotion_lambda-4.0.16/tests/
--rw-r--r--   0 jonathanburger   (501) staff       (20)      131 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/tests/__init__.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)      474 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/tests/test_get_render_progress_client.py
--rw-r--r--   0 jonathanburger   (501) staff       (20)      764 2023-07-31 17:59:07.000000 remotion_lambda-4.0.16/tests/test_render_client.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-04 15:48:56.161940 remotion_lambda-4.0.17/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     2512 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/LICENSE
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      391 2023-08-04 15:48:56.161777 remotion_lambda-4.0.17/PKG-INFO
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       26 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/README.md
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-04 15:48:56.160144 remotion_lambda-4.0.17/remotion_lambda/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      202 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/remotion_lambda/__init__.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     5252 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/remotion_lambda/models.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)     6064 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/remotion_lambda/remotionclient.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       84 2023-08-04 15:40:30.000000 remotion_lambda-4.0.17/remotion_lambda/version.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-04 15:48:56.160929 remotion_lambda-4.0.17/remotion_lambda.egg-info/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      391 2023-08-04 15:48:56.000000 remotion_lambda-4.0.17/remotion_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      384 2023-08-04 15:48:56.000000 remotion_lambda-4.0.17/remotion_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)        1 2023-08-04 15:48:56.000000 remotion_lambda-4.0.17/remotion_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-04 15:48:56.000000 remotion_lambda-4.0.17/remotion_lambda.egg-info/top_level.txt
+-rw-r--r--   0 jonathanburger   (501) staff       (20)       38 2023-08-04 15:48:56.161977 remotion_lambda-4.0.17/setup.cfg
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      753 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/setup.py
+drwxr-xr-x   0 jonathanburger   (501) staff       (20)        0 2023-08-04 15:48:56.161541 remotion_lambda-4.0.17/tests/
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      131 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/tests/__init__.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      474 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/tests/test_get_render_progress_client.py
+-rw-r--r--   0 jonathanburger   (501) staff       (20)      764 2023-08-02 10:09:30.000000 remotion_lambda-4.0.17/tests/test_render_client.py
```

### Comparing `remotion_lambda-4.0.16/LICENSE` & `remotion_lambda-4.0.17/LICENSE`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.16/remotion_lambda/models.py` & `remotion_lambda-4.0.17/remotion_lambda/models.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.16/remotion_lambda/remotionclient.py` & `remotion_lambda-4.0.17/remotion_lambda/remotionclient.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.16/setup.py` & `remotion_lambda-4.0.17/setup.py`

 * *Files identical despite different names*

### Comparing `remotion_lambda-4.0.16/tests/test_render_client.py` & `remotion_lambda-4.0.17/tests/test_render_client.py`

 * *Files identical despite different names*

