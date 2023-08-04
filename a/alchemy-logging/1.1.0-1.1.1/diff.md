# Comparing `tmp/alchemy-logging-1.1.0.tar.gz` & `tmp/alchemy-logging-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alchemy-logging-1.1.0.tar", last modified: Thu Jun  2 17:29:12 2022, max compression
+gzip compressed data, was "dist/alchemy-logging-1.1.1.tar", last modified: Wed Oct 26 18:24:35 2022, max compression
```

## Comparing `alchemy-logging-1.1.0.tar` & `alchemy-logging-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 17:29:12.000000 alchemy-logging-1.1.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 17:29:12.000000 alchemy-logging-1.1.0/alog/
--rw-r--r--   0 root         (0) root         (0)     1698 2022-06-02 17:28:43.000000 alchemy-logging-1.1.0/alog/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29489 2022-06-02 17:28:43.000000 alchemy-logging-1.1.0/alog/alog.py
--rw-r--r--   0 root         (0) root         (0)     2605 2022-06-02 17:28:43.000000 alchemy-logging-1.1.0/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2022-06-02 17:29:12.000000 alchemy-logging-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8428 2022-06-02 17:28:43.000000 alchemy-logging-1.1.0/README.md
--rw-r--r--   0 root         (0) root         (0)     9228 2022-06-02 17:29:12.000000 alchemy-logging-1.1.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-06-02 17:29:12.000000 alchemy-logging-1.1.0/alchemy_logging.egg-info/
--rw-r--r--   0 root         (0) root         (0)        5 2022-06-02 17:29:12.000000 alchemy-logging-1.1.0/alchemy_logging.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-06-02 17:29:12.000000 alchemy-logging-1.1.0/alchemy_logging.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      204 2022-06-02 17:29:12.000000 alchemy-logging-1.1.0/alchemy_logging.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     9228 2022-06-02 17:29:12.000000 alchemy-logging-1.1.0/alchemy_logging.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 18:24:35.000000 alchemy-logging-1.1.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 18:24:35.000000 alchemy-logging-1.1.1/alchemy_logging.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        5 2022-10-26 18:24:35.000000 alchemy-logging-1.1.1/alchemy_logging.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-10-26 18:24:35.000000 alchemy-logging-1.1.1/alchemy_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      204 2022-10-26 18:24:35.000000 alchemy-logging-1.1.1/alchemy_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     9469 2022-10-26 18:24:35.000000 alchemy-logging-1.1.1/alchemy_logging.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2022-10-26 18:24:35.000000 alchemy-logging-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8669 2022-10-26 18:24:04.000000 alchemy-logging-1.1.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     2605 2022-10-26 18:24:04.000000 alchemy-logging-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-10-26 18:24:35.000000 alchemy-logging-1.1.1/alog/
+-rw-r--r--   0 root         (0) root         (0)    29824 2022-10-26 18:24:04.000000 alchemy-logging-1.1.1/alog/alog.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2022-10-26 18:24:04.000000 alchemy-logging-1.1.1/alog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9469 2022-10-26 18:24:35.000000 alchemy-logging-1.1.1/PKG-INFO
```

### Comparing `alchemy-logging-1.1.0/alog/__init__.py` & `alchemy-logging-1.1.1/alog/__init__.py`

 * *Files identical despite different names*

### Comparing `alchemy-logging-1.1.0/alog/alog.py` & `alchemy-logging-1.1.1/alog/alog.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,14 +164,23 @@
         # Add indent to all log records
         log_record['num_indent'] = self._indent.indent
 
         # If enabled, add thread id
         if g_thread_id_enabled:
             log_record['thread_id'] = threading.get_ident()
 
+        # Interpolate message and args if present
+        record_args = log_record.pop('args', None)
+        if record_args:
+            message = log_record.get('message')
+            if message:
+                log_record['message'] = message % record_args
+            else:
+                log_record['message'] = str(record_args)
+
         return json.dumps(log_record, sort_keys=True)
 
 class AlogPrettyFormatter(AlogFormatterBase):
     """Log formatter that pretty-prints lines for easy visibility.
     """
     _INDENT = "  "
     _LEVEL_MAP = {
```

### Comparing `alchemy-logging-1.1.0/setup.py` & `alchemy-logging-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `alchemy-logging-1.1.0/README.md` & `alchemy-logging-1.1.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -182,7 +182,10 @@
 foo()
 ```
 
 ```
 2021-07-29T19:19:47.468428 [DEMO :DBUG] This is a test
 2021-07-29T19:19:48.471788 [DEMO :TRCE] 0:00:01.003284
 ```
+
+## Tip
+- Visual Studio Code (VSCode) users can take advantage of [alchemy-logging extension](https://marketplace.visualstudio.com/items?itemName=Gaurav-Kumbhat.alog-code-generator) that provides automatic log code generation and insertion.
```

### Comparing `alchemy-logging-1.1.0/PKG-INFO` & `alchemy-logging-1.1.1/alchemy_logging.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemy-logging
-Version: 1.1.0
+Version: 1.1.1
 Summary: A wrapper around the logging package to provide Alchemy Logging functionality
 Home-page: https://github.com/IBM/alchemy-logging
 Author: Gabe Goodhart
 Author-email: gabe.l.hart@gmail.com
 License: MIT
 Keywords: logging
 Platform: UNKNOWN
@@ -204,8 +204,11 @@
 ```
 
 ```
 2021-07-29T19:19:47.468428 [DEMO :DBUG] This is a test
 2021-07-29T19:19:48.471788 [DEMO :TRCE] 0:00:01.003284
 ```
 
+## Tip
+- Visual Studio Code (VSCode) users can take advantage of [alchemy-logging extension](https://marketplace.visualstudio.com/items?itemName=Gaurav-Kumbhat.alog-code-generator) that provides automatic log code generation and insertion.
+
```

### Comparing `alchemy-logging-1.1.0/alchemy_logging.egg-info/PKG-INFO` & `alchemy-logging-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alchemy-logging
-Version: 1.1.0
+Version: 1.1.1
 Summary: A wrapper around the logging package to provide Alchemy Logging functionality
 Home-page: https://github.com/IBM/alchemy-logging
 Author: Gabe Goodhart
 Author-email: gabe.l.hart@gmail.com
 License: MIT
 Keywords: logging
 Platform: UNKNOWN
@@ -204,8 +204,11 @@
 ```
 
 ```
 2021-07-29T19:19:47.468428 [DEMO :DBUG] This is a test
 2021-07-29T19:19:48.471788 [DEMO :TRCE] 0:00:01.003284
 ```
 
+## Tip
+- Visual Studio Code (VSCode) users can take advantage of [alchemy-logging extension](https://marketplace.visualstudio.com/items?itemName=Gaurav-Kumbhat.alog-code-generator) that provides automatic log code generation and insertion.
+
```

