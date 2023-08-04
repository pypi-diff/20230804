# Comparing `tmp/ptmethods-1.0.0.tar.gz` & `tmp/ptmethods-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptmethods-1.0.0.tar", last modified: Mon Jul 31 19:00:18 2023, max compression
+gzip compressed data, was "ptmethods-1.0.1.tar", last modified: Fri Aug  4 11:21:12 2023, max compression
```

## Comparing `ptmethods-1.0.0.tar` & `ptmethods-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-31 19:00:18.162987 ptmethods-1.0.0/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35823 2023-02-16 20:42:08.000000 ptmethods-1.0.0/LICENSE
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3909 2023-07-31 19:00:18.162987 ptmethods-1.0.0/PKG-INFO
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3453 2023-07-31 18:59:07.000000 ptmethods-1.0.0/README.md
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-31 19:00:18.158987 ptmethods-1.0.0/ptmethods/
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-16 20:42:08.000000 ptmethods-1.0.0/ptmethods/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-04-14 08:08:26.000000 ptmethods-1.0.0/ptmethods/_version.py
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)    14643 2023-07-31 18:56:57.000000 ptmethods-1.0.0/ptmethods/ptmethods.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-07-31 19:00:18.162987 ptmethods-1.0.0/ptmethods.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     3909 2023-07-31 19:00:18.000000 ptmethods-1.0.0/ptmethods.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      293 2023-07-31 19:00:18.000000 ptmethods-1.0.0/ptmethods.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-07-31 19:00:18.000000 ptmethods-1.0.0/ptmethods.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       55 2023-07-31 19:00:18.000000 ptmethods-1.0.0/ptmethods.egg-info/entry_points.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       22 2023-07-31 19:00:18.000000 ptmethods-1.0.0/ptmethods.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       10 2023-07-31 19:00:18.000000 ptmethods-1.0.0/ptmethods.egg-info/top_level.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-07-31 19:00:18.162987 ptmethods-1.0.0/setup.cfg
--rwxr-xr-x   0 daniel    (1000) daniel    (1000)      973 2023-04-17 09:01:26.000000 ptmethods-1.0.0/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:21:12.462381 ptmethods-1.0.1/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    35823 2023-02-16 20:42:08.000000 ptmethods-1.0.1/LICENSE
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3939 2023-08-04 11:21:12.462381 ptmethods-1.0.1/PKG-INFO
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)     3485 2023-08-04 11:17:17.000000 ptmethods-1.0.1/README.md
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:21:12.462381 ptmethods-1.0.1/ptmethods/
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-02-16 20:42:08.000000 ptmethods-1.0.1/ptmethods/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-07-31 19:38:27.000000 ptmethods-1.0.1/ptmethods/_version.py
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)    14564 2023-07-31 19:38:43.000000 ptmethods-1.0.1/ptmethods/ptmethods.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-08-04 11:21:12.462381 ptmethods-1.0.1/ptmethods.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     3939 2023-08-04 11:21:12.000000 ptmethods-1.0.1/ptmethods.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      293 2023-08-04 11:21:12.000000 ptmethods-1.0.1/ptmethods.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-08-04 11:21:12.000000 ptmethods-1.0.1/ptmethods.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       55 2023-08-04 11:21:12.000000 ptmethods-1.0.1/ptmethods.egg-info/entry_points.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       22 2023-08-04 11:21:12.000000 ptmethods-1.0.1/ptmethods.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       10 2023-08-04 11:21:12.000000 ptmethods-1.0.1/ptmethods.egg-info/top_level.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       38 2023-08-04 11:21:12.462381 ptmethods-1.0.1/setup.cfg
+-rwxr-xr-x   0 daniel    (1000) daniel    (1000)      973 2023-04-17 09:01:26.000000 ptmethods-1.0.1/setup.py
```

### Comparing `ptmethods-1.0.0/LICENSE` & `ptmethods-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ptmethods-1.0.0/PKG-INFO` & `ptmethods-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptmethods
-Version: 1.0.0
+Version: 1.0.1
 Summary: HTTP methods testing tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -78,14 +78,16 @@
 ```
 requests
 ptlibs
 ```
 
 ## Version History
 ```
+1.0.1
+    - Fix urllib3 error
 1.0.0
     - Support for ptlibs v1.0.0
     - Code refactorization
 0.0.2 - 0.0.4
     - Implemented proxy and connect tests
 0.0.1 - 0.0.3
     Alpha releases
```

### Comparing `ptmethods-1.0.0/README.md` & `ptmethods-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 ```
 requests
 ptlibs
 ```
 
 ## Version History
 ```
+1.0.1
+    - Fix urllib3 error
 1.0.0
     - Support for ptlibs v1.0.0
     - Code refactorization
 0.0.2 - 0.0.4
     - Implemented proxy and connect tests
 0.0.1 - 0.0.3
     Alpha releases
```

### Comparing `ptmethods-1.0.0/ptmethods/ptmethods.py` & `ptmethods-1.0.1/ptmethods/ptmethods.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,14 @@
     return args
 
 
 def main():
     global SCRIPTNAME
     SCRIPTNAME = "ptmethods"
     requests.packages.urllib3.disable_warnings()
-    requests.packages.urllib3.util.ssl_.DEFAULT_CIPHERS += ':HIGH:!DH:!aNULL'
     args = parse_args()
     script = PtMethods(args)
     script.run()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ptmethods-1.0.0/ptmethods.egg-info/PKG-INFO` & `ptmethods-1.0.1/ptmethods.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptmethods
-Version: 1.0.0
+Version: 1.0.1
 Summary: HTTP methods testing tool
 Home-page: https://www.penterep.com/
 Author: Penterep
 Author-email: info@penterep.com
 License: GPLv3+
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -78,14 +78,16 @@
 ```
 requests
 ptlibs
 ```
 
 ## Version History
 ```
+1.0.1
+    - Fix urllib3 error
 1.0.0
     - Support for ptlibs v1.0.0
     - Code refactorization
 0.0.2 - 0.0.4
     - Implemented proxy and connect tests
 0.0.1 - 0.0.3
     Alpha releases
```

### Comparing `ptmethods-1.0.0/setup.py` & `ptmethods-1.0.1/setup.py`

 * *Files identical despite different names*

