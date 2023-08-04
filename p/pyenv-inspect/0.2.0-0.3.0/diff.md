# Comparing `tmp/pyenv-inspect-0.2.0.tar.gz` & `tmp/pyenv-inspect-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenv-inspect-0.2.0.tar", max compression
+gzip compressed data, was "pyenv-inspect-0.3.0.tar", last modified: Fri Aug  4 13:52:12 2023, max compression
```

## Comparing `pyenv-inspect-0.2.0.tar` & `pyenv-inspect-0.3.0.tar`

### file list

```diff
@@ -1,11 +1,26 @@
--rw-r--r--   0        0        0     1093 2022-04-03 11:56:52.424813 pyenv-inspect-0.2.0/LICENSE
--rw-r--r--   0        0        0      314 2022-01-17 14:42:21.271860 pyenv-inspect-0.2.0/README.md
--rw-r--r--   0        0        0     1387 2022-04-03 11:56:17.448268 pyenv-inspect-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      134 2022-04-03 11:57:32.681440 pyenv-inspect-0.2.0/src/pyenv_inspect/__init__.py
--rw-r--r--   0        0        0      668 2022-01-17 11:29:37.190210 pyenv-inspect-0.2.0/src/pyenv_inspect/exceptions.py
--rw-r--r--   0        0        0     1675 2022-04-03 11:52:02.924308 pyenv-inspect-0.2.0/src/pyenv_inspect/inspect.py
--rw-r--r--   0        0        0     1384 2022-04-02 12:19:41.624897 pyenv-inspect-0.2.0/src/pyenv_inspect/path.py
--rw-r--r--   0        0        0     1540 2022-01-17 11:14:57.809420 pyenv-inspect-0.2.0/src/pyenv_inspect/spec.py
--rw-r--r--   0        0        0     4003 2022-01-17 11:48:18.720326 pyenv-inspect-0.2.0/src/pyenv_inspect/version.py
--rw-r--r--   0        0        0      986 2022-04-03 11:58:56.864338 pyenv-inspect-0.2.0/setup.py
--rw-r--r--   0        0        0     1183 2022-04-03 11:58:56.864483 pyenv-inspect-0.2.0/PKG-INFO
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-08-04 13:52:12.002101 pyenv-inspect-0.3.0/
+-rw-rw-r--   0 def       (1000) def       (1000)     1099 2023-08-03 08:04:36.000000 pyenv-inspect-0.3.0/LICENSE
+-rw-rw-r--   0 def       (1000) def       (1000)     2476 2023-08-04 13:52:12.002101 pyenv-inspect-0.3.0/PKG-INFO
+-rw-rw-r--   0 def       (1000) def       (1000)      314 2022-01-17 14:42:21.000000 pyenv-inspect-0.3.0/README.md
+-rw-rw-r--   0 def       (1000) def       (1000)     1780 2023-08-03 08:13:05.000000 pyenv-inspect-0.3.0/pyproject.toml
+-rw-rw-r--   0 def       (1000) def       (1000)       38 2023-08-04 13:52:12.002101 pyenv-inspect-0.3.0/setup.cfg
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-08-04 13:52:12.002101 pyenv-inspect-0.3.0/src/
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-08-04 13:52:12.002101 pyenv-inspect-0.3.0/src/pyenv_inspect/
+-rw-rw-r--   0 def       (1000) def       (1000)      134 2023-08-04 13:51:11.000000 pyenv-inspect-0.3.0/src/pyenv_inspect/__init__.py
+-rw-rw-r--   0 def       (1000) def       (1000)      668 2022-01-17 11:29:37.000000 pyenv-inspect-0.3.0/src/pyenv_inspect/exceptions.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1675 2022-04-03 11:52:02.000000 pyenv-inspect-0.3.0/src/pyenv_inspect/inspect.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1384 2022-04-02 12:19:41.000000 pyenv-inspect-0.3.0/src/pyenv_inspect/path.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1540 2022-01-17 11:14:57.000000 pyenv-inspect-0.3.0/src/pyenv_inspect/spec.py
+-rw-rw-r--   0 def       (1000) def       (1000)     4003 2023-08-02 15:20:01.000000 pyenv-inspect-0.3.0/src/pyenv_inspect/version.py
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-08-04 13:52:12.002101 pyenv-inspect-0.3.0/src/pyenv_inspect.egg-info/
+-rw-rw-r--   0 def       (1000) def       (1000)     2476 2023-08-04 13:52:11.000000 pyenv-inspect-0.3.0/src/pyenv_inspect.egg-info/PKG-INFO
+-rw-rw-r--   0 def       (1000) def       (1000)      503 2023-08-04 13:52:11.000000 pyenv-inspect-0.3.0/src/pyenv_inspect.egg-info/SOURCES.txt
+-rw-rw-r--   0 def       (1000) def       (1000)        1 2023-08-04 13:52:11.000000 pyenv-inspect-0.3.0/src/pyenv_inspect.egg-info/dependency_links.txt
+-rw-rw-r--   0 def       (1000) def       (1000)       14 2023-08-04 13:52:11.000000 pyenv-inspect-0.3.0/src/pyenv_inspect.egg-info/top_level.txt
+-rw-rw-r--   0 def       (1000) def       (1000)        1 2023-08-04 13:52:11.000000 pyenv-inspect-0.3.0/src/pyenv_inspect.egg-info/zip-safe
+drwxrwxr-x   0 def       (1000) def       (1000)        0 2023-08-04 13:52:12.002101 pyenv-inspect-0.3.0/tests/
+-rw-rw-r--   0 def       (1000) def       (1000)     1773 2023-08-02 15:28:52.000000 pyenv-inspect-0.3.0/tests/test_inspect.py
+-rw-rw-r--   0 def       (1000) def       (1000)     3882 2022-04-02 12:20:42.000000 pyenv-inspect-0.3.0/tests/test_path.py
+-rw-rw-r--   0 def       (1000) def       (1000)     1385 2023-08-01 08:14:44.000000 pyenv-inspect-0.3.0/tests/test_spec.py
+-rw-rw-r--   0 def       (1000) def       (1000)     3367 2023-08-02 15:22:45.000000 pyenv-inspect-0.3.0/tests/test_version.py
+-rw-rw-r--   0 def       (1000) def       (1000)      773 2022-04-02 11:14:20.000000 pyenv-inspect-0.3.0/tests/testlib.py
```

### Comparing `pyenv-inspect-0.2.0/LICENSE` & `pyenv-inspect-0.3.0/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2021, 2022 un.def <me@undef.im>
+Copyright (c) 2021, 2022, 2023 un.def <me@undef.im>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyenv-inspect-0.2.0/src/pyenv_inspect/exceptions.py` & `pyenv-inspect-0.3.0/src/pyenv_inspect/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyenv-inspect-0.2.0/src/pyenv_inspect/inspect.py` & `pyenv-inspect-0.3.0/src/pyenv_inspect/inspect.py`

 * *Files identical despite different names*

### Comparing `pyenv-inspect-0.2.0/src/pyenv_inspect/path.py` & `pyenv-inspect-0.3.0/src/pyenv_inspect/path.py`

 * *Files identical despite different names*

### Comparing `pyenv-inspect-0.2.0/src/pyenv_inspect/spec.py` & `pyenv-inspect-0.3.0/src/pyenv_inspect/spec.py`

 * *Files identical despite different names*

### Comparing `pyenv-inspect-0.2.0/src/pyenv_inspect/version.py` & `pyenv-inspect-0.3.0/src/pyenv_inspect/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from functools import partial
 from typing import Any, Optional, Tuple
 
 from .exceptions import VersionParseError
 
 
 VERSION_PATTERN = (
-    r'(?P<base>\d(?:\.\d+){1,2})(?:(?P<pre>(?:a|b|rc)\d+)?|-(?P<dev>dev))')
+    r'(?P<base>\d(?:\.\d+){0,2})(?:(?P<pre>(?:a|b|rc)\d+)?|-(?P<dev>dev))')
 VERSION_REGEX = re.compile(VERSION_PATTERN)
 
 
 class Readonly:
 
     def __set_name__(self, owner, name):
         self.private_name = f'_{name}'
```

