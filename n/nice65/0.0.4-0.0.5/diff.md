# Comparing `tmp/nice65-0.0.4.tar.gz` & `tmp/nice65-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nice65-0.0.4.tar", last modified: Fri Aug  4 21:05:06 2023, max compression
+gzip compressed data, was "nice65-0.0.5.tar", last modified: Fri Aug  4 21:16:20 2023, max compression
```

## Comparing `nice65-0.0.4.tar` & `nice65-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-04 21:05:06.461229 nice65-0.0.4/
--rw-r--r--   0 anderson  (1000) anderson  (1000)     1069 2023-07-30 17:49:06.000000 nice65-0.0.4/LICENSE
--rw-r--r--   0 anderson  (1000) anderson  (1000)     3630 2023-08-04 21:05:06.461229 nice65-0.0.4/PKG-INFO
--rw-r--r--   0 anderson  (1000) anderson  (1000)     3210 2023-08-04 21:04:40.000000 nice65-0.0.4/README.md
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-04 21:05:06.461229 nice65-0.0.4/nice65/
--rw-r--r--   0 anderson  (1000) anderson  (1000)       22 2023-08-03 11:55:31.000000 nice65-0.0.4/nice65/__init__.py
--rw-r--r--   0 anderson  (1000) anderson  (1000)       27 2023-08-03 11:55:31.000000 nice65-0.0.4/nice65/__main__.py
--rwxr-xr-x   0 anderson  (1000) anderson  (1000)     7822 2023-08-04 20:52:14.000000 nice65-0.0.4/nice65/app.py
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-04 21:05:06.461229 nice65-0.0.4/nice65.egg-info/
--rw-r--r--   0 anderson  (1000) anderson  (1000)     3630 2023-08-04 21:05:06.000000 nice65-0.0.4/nice65.egg-info/PKG-INFO
--rw-r--r--   0 anderson  (1000) anderson  (1000)      266 2023-08-04 21:05:06.000000 nice65-0.0.4/nice65.egg-info/SOURCES.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-08-04 21:05:06.000000 nice65-0.0.4/nice65.egg-info/dependency_links.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)       39 2023-08-04 21:05:06.000000 nice65-0.0.4/nice65.egg-info/entry_points.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)       12 2023-08-04 21:05:06.000000 nice65-0.0.4/nice65.egg-info/requires.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        7 2023-08-04 21:05:06.000000 nice65-0.0.4/nice65.egg-info/top_level.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)      759 2023-08-04 20:46:54.000000 nice65-0.0.4/pyproject.toml
--rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-08-04 21:05:06.461229 nice65-0.0.4/setup.cfg
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-04 21:16:20.444564 nice65-0.0.5/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     1069 2023-07-30 17:49:06.000000 nice65-0.0.5/LICENSE
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3630 2023-08-04 21:16:20.444564 nice65-0.0.5/PKG-INFO
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3210 2023-08-04 21:04:40.000000 nice65-0.0.5/README.md
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-04 21:16:20.444564 nice65-0.0.5/nice65/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       22 2023-08-03 11:55:31.000000 nice65-0.0.5/nice65/__init__.py
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       27 2023-08-03 11:55:31.000000 nice65-0.0.5/nice65/__main__.py
+-rwxr-xr-x   0 anderson  (1000) anderson  (1000)     8163 2023-08-04 21:15:48.000000 nice65-0.0.5/nice65/app.py
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-04 21:16:20.444564 nice65-0.0.5/nice65.egg-info/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3630 2023-08-04 21:16:20.000000 nice65-0.0.5/nice65.egg-info/PKG-INFO
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      266 2023-08-04 21:16:20.000000 nice65-0.0.5/nice65.egg-info/SOURCES.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-08-04 21:16:20.000000 nice65-0.0.5/nice65.egg-info/dependency_links.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       39 2023-08-04 21:16:20.000000 nice65-0.0.5/nice65.egg-info/entry_points.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       12 2023-08-04 21:16:20.000000 nice65-0.0.5/nice65.egg-info/requires.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        7 2023-08-04 21:16:20.000000 nice65-0.0.5/nice65.egg-info/top_level.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      759 2023-08-04 21:14:03.000000 nice65-0.0.5/pyproject.toml
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-08-04 21:16:20.444564 nice65-0.0.5/setup.cfg
```

### Comparing `nice65-0.0.4/LICENSE` & `nice65-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nice65-0.0.4/PKG-INFO` & `nice65-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice65
-Version: 0.0.4
+Version: 0.0.5
 Summary: Code formatter for CC65 assembly
 Author-email: Andrew Dunai <a@dun.ai>
 Project-URL: Homepage, https://github.com/and3rson/nice65
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `nice65-0.0.4/README.md` & `nice65-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nice65-0.0.4/nice65/app.py` & `nice65-0.0.5/nice65/app.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 #!/usr/bin/python3
 
 from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
 import fnmatch
+try:
+    import importlib_metadata as metadata
+except ImportError:
+    from importlib import metadata
 import os
 import re
 import sys
 
 from lark import Lark, Token, Transformer, Discard
 
 # NMOS 6502 Opcodes
@@ -109,16 +113,26 @@
     )
     parser.add_argument(
         "-p",
         "--pattern",
         help="Match file names by Unix shell-style wildcard when used with -r",
         default='*.s',
     )
+    parser.add_argument(
+        "-v",
+        "--version",
+        help="Print version",
+        action="store_true",
+    )
     args = parser.parse_args()
 
+    if args.version:
+        print('nice65 version', metadata.version("nice65"), file=sys.stderr)
+        return
+
     if args.recursive:
         for root, _, files in os.walk(args.infile):
             for file in files:
                 if fnmatch.fnmatch(file, args.pattern):
                     path = os.path.join(root, file)
                     print("Fixing", path, file=sys.stderr)
                     fix(path, None, True)
```

### Comparing `nice65-0.0.4/nice65.egg-info/PKG-INFO` & `nice65-0.0.5/nice65.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice65
-Version: 0.0.4
+Version: 0.0.5
 Summary: Code formatter for CC65 assembly
 Author-email: Andrew Dunai <a@dun.ai>
 Project-URL: Homepage, https://github.com/and3rson/nice65
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `nice65-0.0.4/pyproject.toml` & `nice65-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nice65"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Andrew Dunai", email="a@dun.ai" },
 ]
 description = "Code formatter for CC65 assembly"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

