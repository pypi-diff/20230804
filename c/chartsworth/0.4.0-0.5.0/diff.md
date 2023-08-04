# Comparing `tmp/chartsworth-0.4.0.tar.gz` & `tmp/chartsworth-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartsworth-0.4.0.tar", max compression
+gzip compressed data, was "chartsworth-0.5.0.tar", max compression
```

## Comparing `chartsworth-0.4.0.tar` & `chartsworth-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-08-03 01:38:46.233088 chartsworth-0.4.0/README.md
--rw-r--r--   0        0        0       59 2023-08-03 01:35:50.467539 chartsworth-0.4.0/chartsworth/__init__.py
--rw-r--r--   0        0        0     4553 2023-08-04 11:44:52.380213 chartsworth-0.4.0/chartsworth/client.py
--rw-r--r--   0        0        0     1456 2023-08-03 01:56:37.831353 chartsworth-0.4.0/chartsworth/plot.py
--rw-r--r--   0        0        0      572 2023-08-04 11:45:30.036332 chartsworth-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 chartsworth-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-03 01:38:46.233088 chartsworth-0.5.0/README.md
+-rw-r--r--   0        0        0       59 2023-08-03 01:35:50.467539 chartsworth-0.5.0/chartsworth/__init__.py
+-rw-r--r--   0        0        0     4738 2023-08-04 11:53:32.145852 chartsworth-0.5.0/chartsworth/client.py
+-rw-r--r--   0        0        0     1456 2023-08-03 01:56:37.831353 chartsworth-0.5.0/chartsworth/plot.py
+-rw-r--r--   0        0        0      572 2023-08-04 11:54:49.546473 chartsworth-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 chartsworth-0.5.0/PKG-INFO
```

### Comparing `chartsworth-0.4.0/chartsworth/client.py` & `chartsworth-0.5.0/chartsworth/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         channel = self.__determine_channel(channel)
         thread_ts = self.threads.get(channel, None)
         if thread_ts is None:
             thread_ts = self.__begin_thread("Post :thread:", channel=channel)
 
         self.slack_client.reactions_add(channel=channel, timestamp=thread_ts, name=name)
 
-    def post_image(self, image_stream: IOBase, filename, channel: Optional[str] = None):
+    def post_image(self, image_stream: IOBase, filename: str, channel: Optional[str] = None):
         """Posts an image to a thread."""
         channel = self.__determine_channel(channel)
         thread_ts = self.threads.get(channel, None)
         if thread_ts is None:
             thread_ts = self.__begin_thread("Image :thread:", channel=channel)
 
         self.slack_client.files_upload(
@@ -120,7 +120,15 @@
         )
 
     def get_current_notebook_id(self):
         return os.environ["NTBL_FILE_ID"]
 
     def get_current_notebook_link(self):
         return f"https://{self.base_deployment}/f/{self.get_current_notebook_id()}"
+
+    @property
+    def notebook_link(self):
+        return self.get_current_notebook_link()
+
+    @property
+    def notebook_id(self):
+        return self.get_current_notebook_id()
```

### Comparing `chartsworth-0.4.0/chartsworth/plot.py` & `chartsworth-0.5.0/chartsworth/plot.py`

 * *Files identical despite different names*

### Comparing `chartsworth-0.4.0/pyproject.toml` & `chartsworth-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chartsworth"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.9,<3.12"
 slack-sdk = "^3.21.3"
```

