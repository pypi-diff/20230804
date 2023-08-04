# Comparing `tmp/chartsworth-0.6.0.tar.gz` & `tmp/chartsworth-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartsworth-0.6.0.tar", max compression
+gzip compressed data, was "chartsworth-0.7.0.tar", max compression
```

## Comparing `chartsworth-0.6.0.tar` & `chartsworth-0.7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-08-03 01:38:46.233088 chartsworth-0.6.0/README.md
--rw-r--r--   0        0        0       59 2023-08-03 01:35:50.467539 chartsworth-0.6.0/chartsworth/__init__.py
--rw-r--r--   0        0        0     4904 2023-08-04 12:32:30.491133 chartsworth-0.6.0/chartsworth/client.py
--rw-r--r--   0        0        0      927 2023-08-04 12:27:58.005085 chartsworth-0.6.0/chartsworth/plot.py
--rw-r--r--   0        0        0      617 2023-08-04 12:32:39.131521 chartsworth-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 chartsworth-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-03 01:38:46.233088 chartsworth-0.7.0/README.md
+-rw-r--r--   0        0        0       59 2023-08-03 01:35:50.467539 chartsworth-0.7.0/chartsworth/__init__.py
+-rw-r--r--   0        0        0     5079 2023-08-04 12:51:56.068389 chartsworth-0.7.0/chartsworth/client.py
+-rw-r--r--   0        0        0      927 2023-08-04 12:27:58.005085 chartsworth-0.7.0/chartsworth/plot.py
+-rw-r--r--   0        0        0      617 2023-08-04 12:52:16.886246 chartsworth-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 chartsworth-0.7.0/PKG-INFO
```

### Comparing `chartsworth-0.6.0/chartsworth/client.py` & `chartsworth-0.7.0/chartsworth/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,21 @@
         elif isinstance(image, Figure):
             image.savefig(image_stream, format="PNG")
         else:
             image_stream = image
 
         image_stream.seek(0)
 
-        self.slack_client.files_upload(
+        if filename is None:
+            filename = "image.png"
+        filename = filename[:160]
+        if not filename.endswith(".png"):
+            filename += ".png"
+
+        self.slack_client.files_upload_v2(
             channel=channel,
             thread_ts=thread_ts,
             file=image_stream,
             filename=filename,
         )
 
     def post_monster(self, text: str, channel: Optional[str] = None):
```

### Comparing `chartsworth-0.6.0/chartsworth/plot.py` & `chartsworth-0.7.0/chartsworth/plot.py`

 * *Files identical despite different names*

### Comparing `chartsworth-0.6.0/pyproject.toml` & `chartsworth-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chartsworth"
-version = "0.6.0"
+version = "0.7.0"
 description = ""
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.9,<3.12"
 slack-sdk = "^3.21.3"
```

### Comparing `chartsworth-0.6.0/PKG-INFO` & `chartsworth-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartsworth
-Version: 0.6.0
+Version: 0.7.0
 Summary: 
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
 Requires-Python: >3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

