# Comparing `tmp/dedust-0.0.4.tar.gz` & `tmp/dedust-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dedust-0.0.4.tar", last modified: Fri Aug  4 21:07:38 2023, max compression
+gzip compressed data, was "dedust-0.0.5.tar", last modified: Fri Aug  4 21:09:18 2023, max compression
```

## Comparing `dedust-0.0.4.tar` & `dedust-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     6148 2023-08-04 12:38:31.476509 dedust-0.0.4/.DS_Store
--rw-r--r--   0        0        0       26 2023-08-04 21:07:12.827629 dedust-0.0.4/.gitignore
--rw-r--r--   0        0        0    11350 2023-04-20 20:08:32.030831 dedust-0.0.4/LICENSE.md
--rw-r--r--   0        0        0     1363 2023-08-04 21:06:55.812898 dedust-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-04-20 20:25:11.314002 dedust-0.0.4/dedust/__init__.py
--rw-r--r--   0        0        0      275 2023-04-20 20:28:32.619931 dedust-0.0.4/dedust/api.py
--rw-r--r--   0        0        0     1553 2023-06-11 09:24:19.451717 dedust-0.0.4/dedust/functions.py
--rw-r--r--   0        0        0      998 2023-06-11 09:24:41.554230 dedust-0.0.4/dedust/tokens.py
--rw-r--r--   0        0        0      580 2023-08-04 21:05:40.414918 dedust-0.0.4/examples/full.py
--rw-r--r--   0        0        0      286 2023-08-04 21:07:35.967648 dedust-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 dedust-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     6148 2023-08-04 12:38:31.476509 dedust-0.0.5/.DS_Store
+-rw-r--r--   0        0        0       26 2023-08-04 21:07:12.827629 dedust-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1076 2023-08-04 21:08:32.854532 dedust-0.0.5/LICENSE.md
+-rw-r--r--   0        0        0     1385 2023-08-04 21:08:49.437048 dedust-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-04-20 20:25:11.314002 dedust-0.0.5/dedust/__init__.py
+-rw-r--r--   0        0        0      275 2023-04-20 20:28:32.619931 dedust-0.0.5/dedust/api.py
+-rw-r--r--   0        0        0     1553 2023-06-11 09:24:19.451717 dedust-0.0.5/dedust/functions.py
+-rw-r--r--   0        0        0      998 2023-06-11 09:24:41.554230 dedust-0.0.5/dedust/tokens.py
+-rw-r--r--   0        0        0      580 2023-08-04 21:05:40.414918 dedust-0.0.5/examples/full.py
+-rw-r--r--   0        0        0      286 2023-08-04 21:08:58.977038 dedust-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1581 1970-01-01 00:00:00.000000 dedust-0.0.5/PKG-INFO
```

### Comparing `dedust-0.0.4/.DS_Store` & `dedust-0.0.5/.DS_Store`

 * *Files identical despite different names*

### Comparing `dedust-0.0.4/README.md` & `dedust-0.0.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -47,26 +47,28 @@
 
 ## Authors
 
 [@Vlad10081](https://t.me/dalvgames)
 
 ## Version History
 
+* 0.0.5
+    * License change
 * 0.0.4
     * Dependecies fix
 * 0.0.3
     * Examples fix
 * 0.0.2
     * LP token address getting
 * 0.0.1
     * Initial Beta
 
 ## License
 
-This project is licensed under the Apache License 2.0 - see the LICENSE.md file for details
+This project is licensed under the MIT License - see the LICENSE.md file for details
 
 ## Donate
 
 If you like the bot, I will be glad to accept donations.
 
 * TON: EQCgphx8rTI0PukwmgpVqiPgqguTujhQscg2h7jgc4U0t347
```

### Comparing `dedust-0.0.4/dedust/functions.py` & `dedust-0.0.5/dedust/functions.py`

 * *Files identical despite different names*

### Comparing `dedust-0.0.4/dedust/tokens.py` & `dedust-0.0.5/dedust/tokens.py`

 * *Files identical despite different names*

### Comparing `dedust-0.0.4/examples/full.py` & `dedust-0.0.5/examples/full.py`

 * *Files identical despite different names*

### Comparing `dedust-0.0.4/PKG-INFO` & `dedust-0.0.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dedust
-Version: 0.0.4
+Version: 0.0.5
 Summary: DeDust - DeDust v2 API for Python.
 Author: Vlad100
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: flask
 
 # DeDust API for Python
@@ -56,26 +56,28 @@
 
 ## Authors
 
 [@Vlad10081](https://t.me/dalvgames)
 
 ## Version History
 
+* 0.0.5
+    * License change
 * 0.0.4
     * Dependecies fix
 * 0.0.3
     * Examples fix
 * 0.0.2
     * LP token address getting
 * 0.0.1
     * Initial Beta
 
 ## License
 
-This project is licensed under the Apache License 2.0 - see the LICENSE.md file for details
+This project is licensed under the MIT License - see the LICENSE.md file for details
 
 ## Donate
 
 If you like the bot, I will be glad to accept donations.
 
 * TON: EQCgphx8rTI0PukwmgpVqiPgqguTujhQscg2h7jgc4U0t347
```

