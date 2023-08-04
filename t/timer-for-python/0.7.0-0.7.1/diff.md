# Comparing `tmp/timer-for-python-0.7.0.tar.gz` & `tmp/timer-for-python-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timer-for-python-0.7.0.tar", last modified: Sat Jan 28 00:03:52 2023, max compression
+gzip compressed data, was "timer-for-python-0.7.1.tar", last modified: Fri Aug  4 08:06:49 2023, max compression
```

## Comparing `timer-for-python-0.7.0.tar` & `timer-for-python-0.7.1.tar`

### file list

```diff
@@ -1,44 +1,60 @@
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-01-28 00:03:52.391368 timer-for-python-0.7.0/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1084 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/LICENSE.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      193 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/MANIFEST.in
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     7626 2023-01-28 00:03:52.391421 timer-for-python-0.7.0/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     5753 2023-01-27 23:59:31.000000 timer-for-python-0.7.0/README.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      109 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/pyproject.toml
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1484 2023-01-28 00:03:52.391724 timer-for-python-0.7.0/setup.cfg
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-01-28 00:03:52.387235 timer-for-python-0.7.0/src/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-01-28 00:03:52.387979 timer-for-python-0.7.0/src/timer/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      161 2023-01-27 23:59:28.000000 timer-for-python-0.7.0/src/timer/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-01-28 00:03:52.388662 timer-for-python-0.7.0/src/timer/constant/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       67 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/constant/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       53 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/constant/decimals.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      117 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/constant/various.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-01-28 00:03:52.388795 timer-for-python-0.7.0/src/timer/controller/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1662 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/controller/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-01-28 00:03:52.388912 timer-for-python-0.7.0/src/timer/decorator/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      378 2023-01-27 23:59:28.000000 timer-for-python-0.7.0/src/timer/decorator/benchmark.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-01-28 00:03:52.389010 timer-for-python-0.7.0/src/timer/error/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1185 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/error/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-01-28 00:03:52.389541 timer-for-python-0.7.0/src/timer/helper/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      117 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/helper/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1568 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/helper/decimals.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1641 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/helper/output.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-01-28 00:03:52.389782 timer-for-python-0.7.0/src/timer/helper/thread/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      471 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/helper/thread/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1474 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/helper/thread/list.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1083 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/helper/time_fractions.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-01-28 00:03:52.390486 timer-for-python-0.7.0/src/timer/model/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      145 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/model/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      282 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/model/elapsed_time_fractions.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      212 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/model/thread_item.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1298 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/model/time_fractions.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2617 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/model/timer.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      557 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/model/timer_base.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 13:59:39.000000 timer-for-python-0.7.0/src/timer/py.typed
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       80 2023-01-27 23:59:31.000000 timer-for-python-0.7.0/src/timer/version.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-01-28 00:03:52.391229 timer-for-python-0.7.0/src/timer_for_python.egg-info/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     7626 2023-01-28 00:03:52.000000 timer-for-python-0.7.0/src/timer_for_python.egg-info/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      945 2023-01-28 00:03:52.000000 timer-for-python-0.7.0/src/timer_for_python.egg-info/SOURCES.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-28 00:03:52.000000 timer-for-python-0.7.0/src/timer_for_python.egg-info/dependency_links.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-26 21:26:38.000000 timer-for-python-0.7.0/src/timer_for_python.egg-info/not-zip-safe
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      126 2023-01-28 00:03:52.000000 timer-for-python-0.7.0/src/timer_for_python.egg-info/requires.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        6 2023-01-28 00:03:52.000000 timer-for-python-0.7.0/src/timer_for_python.egg-info/top_level.txt
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.397688 timer-for-python-0.7.1/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1085 2023-06-27 14:27:46.000000 timer-for-python-0.7.1/LICENSE.md
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      193 2023-08-03 22:19:33.000000 timer-for-python-0.7.1/MANIFEST.in
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     6396 2023-08-04 08:06:49.397904 timer-for-python-0.7.1/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     4136 2023-08-04 08:03:15.000000 timer-for-python-0.7.1/README.md
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      109 2023-01-03 20:49:05.000000 timer-for-python-0.7.1/pyproject.toml
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1818 2023-08-04 08:06:49.399310 timer-for-python-0.7.1/setup.cfg
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.242407 timer-for-python-0.7.1/src/
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.248949 timer-for-python-0.7.1/src/timer/
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.253199 timer-for-python-0.7.1/src/timer/.pytest_cache/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       37 2022-05-08 17:22:45.000000 timer-for-python-0.7.1/src/timer/.pytest_cache/.gitignore
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      191 2022-05-08 17:22:45.000000 timer-for-python-0.7.1/src/timer/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      302 2022-05-08 17:22:45.000000 timer-for-python-0.7.1/src/timer/.pytest_cache/README.md
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.237539 timer-for-python-0.7.1/src/timer/.pytest_cache/v/
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.258609 timer-for-python-0.7.1/src/timer/.pytest_cache/v/cache/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        2 2022-05-08 17:22:45.000000 timer-for-python-0.7.1/src/timer/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        2 2022-05-08 17:22:45.000000 timer-for-python-0.7.1/src/timer/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      161 2023-03-13 10:40:21.000000 timer-for-python-0.7.1/src/timer/__init__.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.262631 timer-for-python-0.7.1/src/timer/constant/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       67 2022-04-27 16:25:41.000000 timer-for-python-0.7.1/src/timer/constant/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       53 2022-04-27 16:25:41.000000 timer-for-python-0.7.1/src/timer/constant/decimals.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      117 2022-04-27 16:25:41.000000 timer-for-python-0.7.1/src/timer/constant/various.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.263446 timer-for-python-0.7.1/src/timer/controller/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1662 2022-05-08 17:31:17.000000 timer-for-python-0.7.1/src/timer/controller/__init__.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.264102 timer-for-python-0.7.1/src/timer/decorator/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      378 2023-08-03 14:43:30.000000 timer-for-python-0.7.1/src/timer/decorator/benchmark.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.265493 timer-for-python-0.7.1/src/timer/error/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1185 2022-04-27 16:25:41.000000 timer-for-python-0.7.1/src/timer/error/__init__.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.267878 timer-for-python-0.7.1/src/timer/helper/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      117 2022-04-27 16:25:41.000000 timer-for-python-0.7.1/src/timer/helper/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1568 2022-04-27 16:25:41.000000 timer-for-python-0.7.1/src/timer/helper/decimals.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1641 2022-05-08 17:31:17.000000 timer-for-python-0.7.1/src/timer/helper/output.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.273275 timer-for-python-0.7.1/src/timer/helper/thread/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      471 2022-04-27 16:25:41.000000 timer-for-python-0.7.1/src/timer/helper/thread/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1474 2022-04-27 16:25:41.000000 timer-for-python-0.7.1/src/timer/helper/thread/list.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1083 2022-05-08 17:31:17.000000 timer-for-python-0.7.1/src/timer/helper/time_fractions.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.303635 timer-for-python-0.7.1/src/timer/model/
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.341813 timer-for-python-0.7.1/src/timer/model/.pytest_cache/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       37 2022-05-08 17:22:29.000000 timer-for-python-0.7.1/src/timer/model/.pytest_cache/.gitignore
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      191 2022-05-08 17:22:29.000000 timer-for-python-0.7.1/src/timer/model/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      302 2022-05-08 17:22:29.000000 timer-for-python-0.7.1/src/timer/model/.pytest_cache/README.md
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.242146 timer-for-python-0.7.1/src/timer/model/.pytest_cache/v/
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.384046 timer-for-python-0.7.1/src/timer/model/.pytest_cache/v/cache/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        2 2022-05-08 17:22:29.000000 timer-for-python-0.7.1/src/timer/model/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        2 2022-05-08 17:22:29.000000 timer-for-python-0.7.1/src/timer/model/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      145 2022-04-27 16:25:41.000000 timer-for-python-0.7.1/src/timer/model/__init__.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      282 2022-05-08 08:29:07.000000 timer-for-python-0.7.1/src/timer/model/elapsed_time_fractions.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      212 2022-05-08 08:29:07.000000 timer-for-python-0.7.1/src/timer/model/thread_item.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1298 2022-05-08 17:31:17.000000 timer-for-python-0.7.1/src/timer/model/time_fractions.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     4950 2023-08-04 06:36:28.000000 timer-for-python-0.7.1/src/timer/model/timer.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      557 2022-05-08 08:29:07.000000 timer-for-python-0.7.1/src/timer/model/timer_base.py
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        0 2022-04-27 16:25:41.000000 timer-for-python-0.7.1/src/timer/py.typed
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)       80 2023-08-04 08:03:57.000000 timer-for-python-0.7.1/src/timer/version.py
+drwxr-xr-x   0 jakobbagterp   (502) staff       (20)        0 2023-08-04 08:06:49.396913 timer-for-python-0.7.1/src/timer_for_python.egg-info/
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     6396 2023-08-04 08:06:48.000000 timer-for-python-0.7.1/src/timer_for_python.egg-info/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)     1349 2023-08-04 08:06:49.000000 timer-for-python-0.7.1/src/timer_for_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        1 2023-08-04 08:06:48.000000 timer-for-python-0.7.1/src/timer_for_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        1 2022-05-08 08:41:50.000000 timer-for-python-0.7.1/src/timer_for_python.egg-info/not-zip-safe
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)      126 2023-08-04 08:06:49.000000 timer-for-python-0.7.1/src/timer_for_python.egg-info/requires.txt
+-rw-r--r--   0 jakobbagterp   (502) staff       (20)        6 2023-08-04 08:06:49.000000 timer-for-python-0.7.1/src/timer_for_python.egg-info/top_level.txt
```

### Comparing `timer-for-python-0.7.0/LICENSE.md` & `timer-for-python-0.7.1/LICENSE.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MIT License
 
-Copyright (c) 2020 – present Jakob Bagterp
+Copyright (c) 2020 – present, Jakob Bagterp
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `timer-for-python-0.7.0/PKG-INFO` & `timer-for-python-0.7.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,132 +1,105 @@
 Metadata-Version: 2.1
 Name: timer-for-python
-Version: 0.7.0
+Version: 0.7.1
 Summary: Timer for Python
-Home-page: https://github.com/jakob-bagterp/timer-for-python
+Home-page: https://jakob-bagterp.github.io/timer-for-python/
+Download-URL: https://pypi.org/project/timer-for-python/
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/jakob-bagterp/timer-for-python/issues
+Project-URL: Documentation, https://jakob-bagterp.github.io/timer-for-python/
+Project-URL: API Reference, https://jakob-bagterp.github.io/timer-for-python/reference/
+Project-URL: Source Code, https://github.com/jakob-bagterp/timer-for-python
+Project-URL: Release Notes, https://github.com/jakob-bagterp/timer-for-python/releases
 Keywords: python,timer
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=0.7.0&color=yellowgreen)](https://github.com/jakob-bagterp/timer-for-python/releases/latest)
-![Python >=3.10](https://img.shields.io/static/v1?label=python&message=>=3.10&color=blueviolet)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=0.7.1&color=yellowgreen)](https://github.com/jakob-bagterp/timer-for-python/releases/latest)
+![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![MIT license](https://img.shields.io/static/v1?label=license&message=MIT&color=blue)](https://github.com/jakob-bagterp/timer-for-python/blob/master/LICENSE.md)
+[![Codecov](https://codecov.io/gh/jakob-bagterp/timer-for-python/branch/master/graph/badge.svg?token=P4IT8WQO0R)](https://codecov.io/gh/jakob-bagterp/timer-for-python)
+[![CodeQL](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/timer-for-python)](https://pepy.tech/project/timer-for-python)
 
 # ⏳ Timer for Python ⌛️
 Lightweight Python package that makes it easy to measure how much time it takes to run Python programs and gauge performance of multiple, smaller bits of code.
 
-## Prerequisites
-* Python 3.10 or higher
-
-## Installation
-### PyPI
-Assuming that Python is installed already, execute this command in the terminal:
-
-```shell
-pip3 install timer-for-python
-```
-
-If you already have installed Timer for Python, use this command to upgrade to latest version:
-
-```shell
-pip3 install --upgrade timer-for-python
-```
-
-### Homebrew
-If you already have installed the [Homebrew](https://brew.sh) package manager for Mac and Linux, execute this terminal command to tap Timer for Python:
-
-```shell
-brew tap jakob-bagterp/timer-for-python
-```
-
-And then install:
-
-```shell
-brew install timer-for-python
-```
-
-### NuGet
-TBC
+Ready to try? Learn [how to install](https://jakob-bagterp.github.io/timer-for-python/getting-started/installation/) and find tutorials in the [user guide](https://jakob-bagterp.github.io/timer-for-python/user-guide/).
 
 ## Getting Started
-### Basic
-Firstly, add the Timer to your imports:
+### Basics
+Simply add the Timer to your imports, and then wrap the Timer function around your code to measure the performance of the executed block of code:
 
 ```python
 from timer import Timer
-```
 
-Wrap the Timer function around your code to measure performance of the executed block of code:
-
-```python
 timer = Timer()
 timer.start()
 
 # Insert your code here
 
 timer.stop() # Output example: 12.34 seconds
 ```
 
-#### With Statement
-Alternatively, use the `with` statement, which automatically will stop the Timer. Same result with less code:
+#### Context Manager
+Alternatively, use the with statement. This will automatically start and stop the Timer – and so no need to declare `timer.start()` and `timer.stop()`. Same result as before, but less code:
 
 ```python
 with Timer():
     # Insert your code here
 
-# Output example: 12.34 seconds
+    # Output example: 12.34 seconds
 ```
 
 #### Decorator
-Or use the `benchmark_timer` as function decorator:
+Or use the `benchmark_timer` as a function decorator:
 
 ```python
 from timer import benchmark_timer
 
 @benchmark_timer
 def test_function():
     # Insert your code here
 
 test_function()
 
 # Output example: 12.34 seconds for thread TEST_FUNCTION
 ```
 
-### Advanced
+### Core Features
 #### Decimals
-Instead of the default value `2` for `decimals`, you can set the output precision up to `9` in the `decimals` argument:
+Instead of the default value of `2` for `decimals``, you can set the output precision up to `9` in the `decimals` argument:
 
 ```python
 timer = Timer()
 timer.start(decimals=5)
 
 # Insert your code here
 
 timer.stop() # Output example: 0.12345 seconds
 ```
 
 #### Multiple Threads
-Imagine that you want to troubleshoot which parts of your code are performing better or worse? Or you want to split test the performance of different methods? Timer for Python is a quick, easy way to get the job done.
+Imagine that you want to troubleshoot which parts of your code are performing better or worse. Or do you want to split-test the performance of different methods? Timer for Python is a quick, easy way to get the job done.
 
-To measure performance of multiple blocks of code, use the `thread` argument to name different threads:
+To measure the performance of multiple blocks of code, use the `thread` argument to name different threads:
 
 ```python
 timer = Timer()
 timer.start(thread="A")
 
 # Insert your code here
 
@@ -145,86 +118,34 @@
 ```python
 with Timer(thread="A")
     # Insert your code here
 
     with Timer(thread="B", decimals=5):
         # Insert more code here
 
-    # Output example: 0.12345 seconds for thread B
+        # Output example: 0.12345 seconds for thread B
 
-# Insert even more code here
+    # Insert even more code here
 
-# Output example: 6.78 seconds for thread A
+    # Output example: 6.78 seconds for thread A
 ```
 
-## Documentation and Other Features
-### Precision in Nanoseconds
-Timer for Python uses the native `time.perf_counter_ns()` function for maximum resolution in nanoseconds.
-
-### Decimals in Output
-To set the number of decimals in the output (only if less than an hour), use the `decimals` argument.
-
-Either, set the general precision of decimals when initiating the Timer:
-
-```python
-timer = Timer(decimals=5)
-timer.start()
-
-# Insert your code here
-
-timer.stop() # Output example: 0.12345 seconds
-```
-
-Or set the decimals when starting a new thread, which will also override the general decimals defined when initiating the Timer:
-
-```python
-timer = Timer(decimals=5)
-timer.start(decimals=9)
-
-# Insert your code here
-
-timer.stop() # Output example: 0.123456789 seconds
-```
-
-#### Default Decimals and Supported Interval
-Default value for `decimals` is `2`. The range is minimum `0` (for no decimals) and up to `9`.
-
-### Humanised Output
-Timer for Python supports time measurement from nanoseconds to days.
-
-But. If the Timer runs for several minutes, it doesn't make sense to display the output time in milliseconds. And similarly if it runs for hours, it doesn't make sense to display the output time in seconds.
-
-Therefore, the output is "humanised" so it's easier to read. Examples:
-
-```
-Elapsed time: 123 nanoseconds
-Elapsed time: 4.56 microseconds
-Elapsed time: 56.78 milliseconds
-Elapsed time: 7.89 seconds
-Elapsed time: 67.89 seconds (1m 8s)
-Elapsed time: 3m 4s
-Elapsed time: 2h 3m 4s
-Elapsed time: 1d 2h 3m 4s
-```
-
-### Graceful Error Handling
-Timer for Python is designed with several nested `try/catch` clauses so it handles exceptions gracefully and therefore shouldn't break your application while running. However, if you find a bug, please [report it](https://github.com/jakob-bagterp/timer-for-python/issues).
-
+# Thank You for Supporting
 ## Donate
 This module is free to use. And if you like it, feel free to [buy me a coffee](https://github.com/sponsors/jakob-bagterp).
 
 ## Contribute
 If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/timer-for-python/pulls).
 
 ## Report Bugs
 Report bugs and issues [here](https://github.com/jakob-bagterp/timer-for-python/issues).
 
 # MIT License
 
-Copyright (c) 2020 – present Jakob Bagterp
+Copyright (c) 2020 – present, Jakob Bagterp
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `timer-for-python-0.7.0/README.md` & `timer-for-python-0.7.1/src/timer_for_python.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,109 +1,105 @@
-[![Latest version](https://img.shields.io/static/v1?label=version&message=0.7.0&color=yellowgreen)](https://github.com/jakob-bagterp/timer-for-python/releases/latest)
-![Python >=3.10](https://img.shields.io/static/v1?label=python&message=>=3.10&color=blueviolet)
+Metadata-Version: 2.1
+Name: timer-for-python
+Version: 0.7.1
+Summary: Timer for Python
+Home-page: https://jakob-bagterp.github.io/timer-for-python/
+Download-URL: https://pypi.org/project/timer-for-python/
+Author: Jakob Bagterp
+Author-email: jakob_bagterp@hotmail.com
+Maintainer: Jakob Bagterp
+Maintainer-email: jakob_bagterp@hotmail.com
+License: MIT License
+Project-URL: Bug Tracker, https://github.com/jakob-bagterp/timer-for-python/issues
+Project-URL: Documentation, https://jakob-bagterp.github.io/timer-for-python/
+Project-URL: API Reference, https://jakob-bagterp.github.io/timer-for-python/reference/
+Project-URL: Source Code, https://github.com/jakob-bagterp/timer-for-python
+Project-URL: Release Notes, https://github.com/jakob-bagterp/timer-for-python/releases
+Keywords: python,timer
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE.md
+
+[![Latest version](https://img.shields.io/static/v1?label=version&message=0.7.1&color=yellowgreen)](https://github.com/jakob-bagterp/timer-for-python/releases/latest)
+![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![MIT license](https://img.shields.io/static/v1?label=license&message=MIT&color=blue)](https://github.com/jakob-bagterp/timer-for-python/blob/master/LICENSE.md)
+[![Codecov](https://codecov.io/gh/jakob-bagterp/timer-for-python/branch/master/graph/badge.svg?token=P4IT8WQO0R)](https://codecov.io/gh/jakob-bagterp/timer-for-python)
+[![CodeQL](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/codeql.yml/badge.svg)](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/codeql.yml)
 [![Test](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/timer-for-python/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/timer-for-python)](https://pepy.tech/project/timer-for-python)
 
 # ⏳ Timer for Python ⌛️
 Lightweight Python package that makes it easy to measure how much time it takes to run Python programs and gauge performance of multiple, smaller bits of code.
 
-## Prerequisites
-* Python 3.10 or higher
-
-## Installation
-### PyPI
-Assuming that Python is installed already, execute this command in the terminal:
-
-```shell
-pip3 install timer-for-python
-```
-
-If you already have installed Timer for Python, use this command to upgrade to latest version:
-
-```shell
-pip3 install --upgrade timer-for-python
-```
-
-### Homebrew
-If you already have installed the [Homebrew](https://brew.sh) package manager for Mac and Linux, execute this terminal command to tap Timer for Python:
-
-```shell
-brew tap jakob-bagterp/timer-for-python
-```
-
-And then install:
-
-```shell
-brew install timer-for-python
-```
-
-### NuGet
-TBC
+Ready to try? Learn [how to install](https://jakob-bagterp.github.io/timer-for-python/getting-started/installation/) and find tutorials in the [user guide](https://jakob-bagterp.github.io/timer-for-python/user-guide/).
 
 ## Getting Started
-### Basic
-Firstly, add the Timer to your imports:
+### Basics
+Simply add the Timer to your imports, and then wrap the Timer function around your code to measure the performance of the executed block of code:
 
 ```python
 from timer import Timer
-```
-
-Wrap the Timer function around your code to measure performance of the executed block of code:
 
-```python
 timer = Timer()
 timer.start()
 
 # Insert your code here
 
 timer.stop() # Output example: 12.34 seconds
 ```
 
-#### With Statement
-Alternatively, use the `with` statement, which automatically will stop the Timer. Same result with less code:
+#### Context Manager
+Alternatively, use the with statement. This will automatically start and stop the Timer – and so no need to declare `timer.start()` and `timer.stop()`. Same result as before, but less code:
 
 ```python
 with Timer():
     # Insert your code here
 
-# Output example: 12.34 seconds
+    # Output example: 12.34 seconds
 ```
 
 #### Decorator
-Or use the `benchmark_timer` as function decorator:
+Or use the `benchmark_timer` as a function decorator:
 
 ```python
 from timer import benchmark_timer
 
 @benchmark_timer
 def test_function():
     # Insert your code here
 
 test_function()
 
 # Output example: 12.34 seconds for thread TEST_FUNCTION
 ```
 
-### Advanced
+### Core Features
 #### Decimals
-Instead of the default value `2` for `decimals`, you can set the output precision up to `9` in the `decimals` argument:
+Instead of the default value of `2` for `decimals``, you can set the output precision up to `9` in the `decimals` argument:
 
 ```python
 timer = Timer()
 timer.start(decimals=5)
 
 # Insert your code here
 
 timer.stop() # Output example: 0.12345 seconds
 ```
 
 #### Multiple Threads
-Imagine that you want to troubleshoot which parts of your code are performing better or worse? Or you want to split test the performance of different methods? Timer for Python is a quick, easy way to get the job done.
+Imagine that you want to troubleshoot which parts of your code are performing better or worse. Or do you want to split-test the performance of different methods? Timer for Python is a quick, easy way to get the job done.
 
-To measure performance of multiple blocks of code, use the `thread` argument to name different threads:
+To measure the performance of multiple blocks of code, use the `thread` argument to name different threads:
 
 ```python
 timer = Timer()
 timer.start(thread="A")
 
 # Insert your code here
 
@@ -122,75 +118,35 @@
 ```python
 with Timer(thread="A")
     # Insert your code here
 
     with Timer(thread="B", decimals=5):
         # Insert more code here
 
-    # Output example: 0.12345 seconds for thread B
+        # Output example: 0.12345 seconds for thread B
 
-# Insert even more code here
+    # Insert even more code here
 
-# Output example: 6.78 seconds for thread A
+    # Output example: 6.78 seconds for thread A
 ```
 
-## Documentation and Other Features
-### Precision in Nanoseconds
-Timer for Python uses the native `time.perf_counter_ns()` function for maximum resolution in nanoseconds.
-
-### Decimals in Output
-To set the number of decimals in the output (only if less than an hour), use the `decimals` argument.
-
-Either, set the general precision of decimals when initiating the Timer:
-
-```python
-timer = Timer(decimals=5)
-timer.start()
-
-# Insert your code here
-
-timer.stop() # Output example: 0.12345 seconds
-```
-
-Or set the decimals when starting a new thread, which will also override the general decimals defined when initiating the Timer:
-
-```python
-timer = Timer(decimals=5)
-timer.start(decimals=9)
-
-# Insert your code here
-
-timer.stop() # Output example: 0.123456789 seconds
-```
+# Thank You for Supporting
+## Donate
+This module is free to use. And if you like it, feel free to [buy me a coffee](https://github.com/sponsors/jakob-bagterp).
 
-#### Default Decimals and Supported Interval
-Default value for `decimals` is `2`. The range is minimum `0` (for no decimals) and up to `9`.
+## Contribute
+If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/timer-for-python/pulls).
 
-### Humanised Output
-Timer for Python supports time measurement from nanoseconds to days.
+## Report Bugs
+Report bugs and issues [here](https://github.com/jakob-bagterp/timer-for-python/issues).
 
-But. If the Timer runs for several minutes, it doesn't make sense to display the output time in milliseconds. And similarly if it runs for hours, it doesn't make sense to display the output time in seconds.
+# MIT License
 
-Therefore, the output is "humanised" so it's easier to read. Examples:
+Copyright (c) 2020 – present, Jakob Bagterp
 
-```
-Elapsed time: 123 nanoseconds
-Elapsed time: 4.56 microseconds
-Elapsed time: 56.78 milliseconds
-Elapsed time: 7.89 seconds
-Elapsed time: 67.89 seconds (1m 8s)
-Elapsed time: 3m 4s
-Elapsed time: 2h 3m 4s
-Elapsed time: 1d 2h 3m 4s
-```
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-### Graceful Error Handling
-Timer for Python is designed with several nested `try/catch` clauses so it handles exceptions gracefully and therefore shouldn't break your application while running. However, if you find a bug, please [report it](https://github.com/jakob-bagterp/timer-for-python/issues).
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-## Donate
-This module is free to use. And if you like it, feel free to [buy me a coffee](https://github.com/sponsors/jakob-bagterp).
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
-## Contribute
-If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/timer-for-python/pulls).
 
-## Report Bugs
-Report bugs and issues [here](https://github.com/jakob-bagterp/timer-for-python/issues).
```

### Comparing `timer-for-python-0.7.0/setup.cfg` & `timer-for-python-0.7.1/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -7,17 +7,22 @@
 maintainer_email = jakob_bagterp@hotmail.com
 description = Timer for Python
 long_description = file: README.md, LICENSE.md
 long_description_content_type = text/markdown
 keywords = 
 	python
 	timer
-url = https://github.com/jakob-bagterp/timer-for-python
+url = https://jakob-bagterp.github.io/timer-for-python/
+download_url = https://pypi.org/project/timer-for-python/
 project_urls = 
 	Bug Tracker = https://github.com/jakob-bagterp/timer-for-python/issues
+	Documentation = https://jakob-bagterp.github.io/timer-for-python/
+	API Reference = https://jakob-bagterp.github.io/timer-for-python/reference/
+	Source Code = https://github.com/jakob-bagterp/timer-for-python
+	Release Notes = https://github.com/jakob-bagterp/timer-for-python/releases
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 license = MIT License
@@ -25,29 +30,29 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
 setup_requires = 
-	colorist ==1.2.3
+	colorist==1.6.0
 install_requires = 
-	colorist ==1.2.3
+	colorist==1.6.0
 zip_safe = no
 include_package_data = True
 
 [options.extras_require]
 testing = 
-	coverage ==7.1.0
-	flake8 ==6.0.0
-	mypy ==0.991
-	numpy ==1.24.1
-	pytest ==7.2.1
-	pytest-cov ==4.0.0
-	tox ==4.4.2
+	coverage==7.2.7
+	flake8==6.1.0
+	mypy==1.4.1
+	numpy==1.25.1
+	pytest==7.4.0
+	pytest-cov==4.1.0
+	tox==4.6.4
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 colorist = py.typed
```

### Comparing `timer-for-python-0.7.0/src/timer/controller/__init__.py` & `timer-for-python-0.7.1/src/timer/controller/__init__.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.0/src/timer/error/__init__.py` & `timer-for-python-0.7.1/src/timer/error/__init__.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.0/src/timer/helper/decimals.py` & `timer-for-python-0.7.1/src/timer/helper/decimals.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.0/src/timer/helper/output.py` & `timer-for-python-0.7.1/src/timer/helper/output.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.0/src/timer/helper/thread/list.py` & `timer-for-python-0.7.1/src/timer/helper/thread/list.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.0/src/timer/helper/time_fractions.py` & `timer-for-python-0.7.1/src/timer/helper/time_fractions.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.0/src/timer/model/time_fractions.py` & `timer-for-python-0.7.1/src/timer/model/time_fractions.py`

 * *Files identical despite different names*

### Comparing `timer-for-python-0.7.0/src/timer/model/timer_base.py` & `timer-for-python-0.7.1/src/timer/model/timer_base.py`

 * *Files identical despite different names*

