# Comparing `tmp/pykebab-0.9.0.tar.gz` & `tmp/pykebab-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykebab-0.9.0.tar", max compression
+gzip compressed data, was "pykebab-0.9.1.tar", max compression
```

## Comparing `pykebab-0.9.0.tar` & `pykebab-0.9.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      821 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/__init__.py
--rw-r--r--   0        0        0     3920 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/aws.py
--rw-r--r--   0        0        0       40 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/cli/__init__.py
--rw-r--r--   0        0        0     1801 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/cli/cli.py
--rw-r--r--   0        0        0      902 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/constants.py
--rw-r--r--   0        0        0       42 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/exceptions.py
--rw-r--r--   0        0        0     2586 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/k8s.py
--rw-r--r--   0        0        0      744 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/loaders.py
--rw-r--r--   0        0        0     2368 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/magic.py
--rw-r--r--   0        0        0     1575 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/openers.py
--rw-r--r--   0        0        0    22900 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/sources.py
--rw-r--r--   0        0        0     4825 2023-08-04 03:09:43.628775 pykebab-0.9.0/kebab/utils.py
--rw-r--r--   0        0        0      957 2023-08-04 03:09:43.628775 pykebab-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 pykebab-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      821 2023-08-04 11:04:34.602573 pykebab-0.9.1/kebab/__init__.py
+-rw-r--r--   0        0        0     3920 2023-08-04 11:04:34.602573 pykebab-0.9.1/kebab/aws.py
+-rw-r--r--   0        0        0       40 2023-08-04 11:04:34.602573 pykebab-0.9.1/kebab/cli/__init__.py
+-rw-r--r--   0        0        0     1801 2023-08-04 11:04:34.602573 pykebab-0.9.1/kebab/cli/cli.py
+-rw-r--r--   0        0        0      902 2023-08-04 11:04:34.602573 pykebab-0.9.1/kebab/constants.py
+-rw-r--r--   0        0        0       42 2023-08-04 11:04:34.602573 pykebab-0.9.1/kebab/exceptions.py
+-rw-r--r--   0        0        0     2586 2023-08-04 11:04:34.602573 pykebab-0.9.1/kebab/k8s.py
+-rw-r--r--   0        0        0      744 2023-08-04 11:04:34.602573 pykebab-0.9.1/kebab/loaders.py
+-rw-r--r--   0        0        0     2368 2023-08-04 11:04:34.602573 pykebab-0.9.1/kebab/magic.py
+-rw-r--r--   0        0        0     1575 2023-08-04 11:04:34.602573 pykebab-0.9.1/kebab/openers.py
+-rw-r--r--   0        0        0    23051 2023-08-04 11:04:34.602573 pykebab-0.9.1/kebab/sources.py
+-rw-r--r--   0        0        0     4825 2023-08-04 11:04:34.602573 pykebab-0.9.1/kebab/utils.py
+-rw-r--r--   0        0        0      957 2023-08-04 11:04:34.602573 pykebab-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      796 1970-01-01 00:00:00.000000 pykebab-0.9.1/PKG-INFO
```

### Comparing `pykebab-0.9.0/kebab/__init__.py` & `pykebab-0.9.1/kebab/__init__.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.0/kebab/aws.py` & `pykebab-0.9.1/kebab/aws.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.0/kebab/cli/cli.py` & `pykebab-0.9.1/kebab/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.0/kebab/constants.py` & `pykebab-0.9.1/kebab/constants.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.0/kebab/k8s.py` & `pykebab-0.9.1/kebab/k8s.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.0/kebab/loaders.py` & `pykebab-0.9.1/kebab/loaders.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.0/kebab/magic.py` & `pykebab-0.9.1/kebab/magic.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.0/kebab/openers.py` & `pykebab-0.9.1/kebab/openers.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.0/kebab/sources.py` & `pykebab-0.9.1/kebab/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import abc
 import copy
 import dataclasses
 import logging
 import os
 import queue  # using python-future for 2/3 compatibility
+import re
 import sys
 import threading
 import time
 from typing import Any, List, Dict, get_type_hints, Type, TypeVar, Callable
 from urllib.request import OpenerDirector, pathname2url
 
 import deprecation
@@ -21,15 +22,14 @@
 from kebab.utils import (
     update_recursively,
     lookup_recursively,
     fill_recursively,
     deprecated_alias,
 )
 
-
 _logger = logging.getLogger(__name__)
 
 
 class ContextExtension(object):
     @property
     @abc.abstractmethod
     def keyword(self):
@@ -477,26 +477,31 @@
     def __init__(self, url, opener=None, **kwargs):
         """
         :param str url: a url of supported protocols in openers.DEFAULT_OPENER
         """
         super(UrlSource, self).__init__(**kwargs)
         self._opener = opener or DEFAULT_OPENER
 
-        if ":\\" in url or ":" not in url:
-            url = UrlSource._path_to_url(url)
-
+        url = UrlSource._path_to_url(url)
         self._url = url
 
     @staticmethod
+    def _is_path(url):
+        return ":\\" in url or not re.match(r"^\w+:.*", url)
+
+    @staticmethod
     def _path_to_url(path):
-        path = os.path.abspath(os.path.expanduser(path))
+        if not UrlSource._is_path(path):
+            return path
         if sys.platform.startswith("win"):
             # path = "/" + path.replace("\\", "/")
             return f"file:{pathname2url(path)}"
-        return f"file://{path}"
+        else:
+            path = os.path.abspath(os.path.expanduser(path))
+            return f"file://{path}"
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self._url})"
 
     def _load_context(self):
         content = self._opener.open(self._url).read()
         return self.str_loader.load(content)
```

### Comparing `pykebab-0.9.0/kebab/utils.py` & `pykebab-0.9.1/kebab/utils.py`

 * *Files identical despite different names*

### Comparing `pykebab-0.9.0/pyproject.toml` & `pykebab-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pykebab"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = ["Yangming Huang <leonmax@gmail.com>"]
 packages = [
     { include = "kebab" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `pykebab-0.9.0/PKG-INFO` & `pykebab-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pykebab
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 Author: Yangming Huang
 Author-email: leonmax@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

