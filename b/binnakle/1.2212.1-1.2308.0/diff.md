# Comparing `tmp/binnakle-1.2212.1-py3-none-any.whl.zip` & `tmp/binnakle-1.2308.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 15533 bytes, number of entries: 8
--rw-rw-r--  2.0 unx      117 b- defN 22-Dec-28 23:46 binnakle/__init__.py
--rw-rw-r--  2.0 unx     4168 b- defN 22-Dec-28 23:45 binnakle/binnakle.py
--rw-rw-r--  2.0 unx      153 b- defN 22-Dec-14 16:38 binnakle/utils.py
--rw-rw-r--  2.0 unx    35149 b- defN 22-Dec-28 23:46 binnakle-1.2212.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx      776 b- defN 22-Dec-28 23:46 binnakle-1.2212.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Dec-28 23:46 binnakle-1.2212.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 22-Dec-28 23:46 binnakle-1.2212.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      631 b- defN 22-Dec-28 23:46 binnakle-1.2212.1.dist-info/RECORD
-8 files, 41095 bytes uncompressed, 14431 bytes compressed:  64.9%
+Zip file size: 15553 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      117 b- defN 23-Aug-04 14:13 binnakle/__init__.py
+-rw-r--r--  2.0 unx     4306 b- defN 23-Aug-04 14:12 binnakle/binnakle.py
+-rw-r--r--  2.0 unx      153 b- defN 23-Aug-04 13:58 binnakle/utils.py
+-rw-r--r--  2.0 unx    35149 b- defN 23-Aug-04 14:14 binnakle-1.2308.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      776 b- defN 23-Aug-04 14:14 binnakle-1.2308.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 14:14 binnakle-1.2308.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Aug-04 14:14 binnakle-1.2308.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      631 b- defN 23-Aug-04 14:14 binnakle-1.2308.0.dist-info/RECORD
+8 files, 41233 bytes uncompressed, 14451 bytes compressed:  65.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: binnakle/binnakle.py
 Comment: 
 
 Filename: binnakle/utils.py
 Comment: 
 
-Filename: binnakle-1.2212.1.dist-info/LICENSE
+Filename: binnakle-1.2308.0.dist-info/LICENSE
 Comment: 
 
-Filename: binnakle-1.2212.1.dist-info/METADATA
+Filename: binnakle-1.2308.0.dist-info/METADATA
 Comment: 
 
-Filename: binnakle-1.2212.1.dist-info/WHEEL
+Filename: binnakle-1.2308.0.dist-info/WHEEL
 Comment: 
 
-Filename: binnakle-1.2212.1.dist-info/top_level.txt
+Filename: binnakle-1.2308.0.dist-info/top_level.txt
 Comment: 
 
-Filename: binnakle-1.2212.1.dist-info/RECORD
+Filename: binnakle-1.2308.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## binnakle/__init__.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from .binnakle import *  # noqa: F401, F403
 
-__version__ = '1.2212.1'
+__version__ = '1.2308.0'
```

## binnakle/binnakle.py

```diff
@@ -78,23 +78,26 @@
 
     def wrapped(method):
 
         def _wrapped(
             self,
             message=None,
             error: Exception = None,
+            stack_depth=None,
             **kwargs,
         ):
             if isinstance(message, bytes):
                 message = message.decode('utf-8')
 
             if message is not None and self._prefix is not None:
                 message = self._prefix + message
 
-            inspection = inspect.stack()[1]
+            if stack_depth is None:
+                stack_depth = 1
+            inspection = inspect.stack()[stack_depth]
 
             level = method.__name__.upper()
             if method.__name__ == 'exception':
                 level = 'ERROR'
                 error_message = traceback.format_exc()
             else:
                 error_message = self._get_error_message(error)
@@ -103,15 +106,17 @@
                 'level': level,
                 'env': self._env,
                 'timestamp': get_timestamp_ms(),
                 'filepath': inspection.filename,
                 'function': inspection.function,
                 'line': inspection.lineno,
                 'error': error_message,
-            } | kwargs | { 'message': message }
+            } | kwargs | {
+                'message': message
+            }
             message_dict = remove_empty_keys(payload)
 
             modified_message = json.dumps(
                 message_dict,
                 indent=4 if self._pretty else None,
                 separators=None if self._pretty else (',', ':'),
                 ensure_ascii=False,
@@ -143,21 +148,23 @@
     @wrapped
     def info(self, message):
         self._logger.info(message)
 
     @wrapped
     def warning(self, message):
         self._logger.warning(message)
+
     warn = warning
 
     @wrapped
     def error(self, message):
         self._logger.error(message)
 
     @wrapped
     def critical(self, message):
         self._logger.critical(message)
+
     fatal = critical
 
     @wrapped
     def exception(self, message):
         self._logger.error(message)
```

## Comparing `binnakle-1.2212.1.dist-info/LICENSE` & `binnakle-1.2308.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `binnakle-1.2212.1.dist-info/METADATA` & `binnakle-1.2308.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binnakle
-Version: 1.2212.1
+Version: 1.2308.0
 Summary: Contextualized logging library for Python.
 Home-page: https://github.com/councilbox/binnakle-python
 Author: Rodrigo Martínez Castaño
 Author-email: rodrigo.martinez@councilbox.com
 License: GNU General Public License v3 (GPLv3)
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

