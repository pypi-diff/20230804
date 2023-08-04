# Comparing `tmp/chartsworth-0.3.0.tar.gz` & `tmp/chartsworth-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartsworth-0.3.0.tar", max compression
+gzip compressed data, was "chartsworth-0.4.0.tar", max compression
```

## Comparing `chartsworth-0.3.0.tar` & `chartsworth-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-08-03 01:38:46.233088 chartsworth-0.3.0/README.md
--rw-r--r--   0        0        0       59 2023-08-03 01:35:50.467539 chartsworth-0.3.0/chartsworth/__init__.py
--rw-r--r--   0        0        0     4181 2023-08-04 11:32:15.604618 chartsworth-0.3.0/chartsworth/client.py
--rw-r--r--   0        0        0     1456 2023-08-03 01:56:37.831353 chartsworth-0.3.0/chartsworth/plot.py
--rw-r--r--   0        0        0      572 2023-08-04 11:40:33.915865 chartsworth-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 chartsworth-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-03 01:38:46.233088 chartsworth-0.4.0/README.md
+-rw-r--r--   0        0        0       59 2023-08-03 01:35:50.467539 chartsworth-0.4.0/chartsworth/__init__.py
+-rw-r--r--   0        0        0     4553 2023-08-04 11:44:52.380213 chartsworth-0.4.0/chartsworth/client.py
+-rw-r--r--   0        0        0     1456 2023-08-03 01:56:37.831353 chartsworth-0.4.0/chartsworth/plot.py
+-rw-r--r--   0        0        0      572 2023-08-04 11:45:30.036332 chartsworth-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 chartsworth-0.4.0/PKG-INFO
```

### Comparing `chartsworth-0.3.0/chartsworth/client.py` & `chartsworth-0.4.0/chartsworth/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,20 +7,24 @@
 
 class Chartsworth:
     """Chartsworth is a Chart Monster for posting from notebooks to Slack.
 
     Chartsworth loves threads. Every new instance of chartsworth will try to
     reuse existing threads per channel."""
 
-    def __init__(self, default_channel=None):
+    def __init__(self, default_channel=None, base_deployment=None):
         # Set up Chartsworth
         slack_token = os.getenv("CHARTSWORTH_SLACK_TOKEN", None)
         if slack_token is None:
             raise ValueError("CHARTSWORTH_SLACK_TOKEN not set as an environment variable")
 
+        self.base_deployment = base_deployment
+        if self.base_deployment is None:
+            self.base_deployment = "app.noteable.io"
+
         self.slack_client = WebClient(token=slack_token)
         self.default_channel = default_channel
         self.threads = {}
 
     def __determine_channel(self, channel: Optional[str] = None) -> str:
         if channel is not None:
             return channel
@@ -110,7 +114,13 @@
 
         image_data = fig_to_bytes(figure)
         print(image_data[0])
 
         self.slack_client.files_upload_v2(
             channel=channel, thread_ts=thread_ts, filename="plot.png", file=image_data
         )
+
+    def get_current_notebook_id(self):
+        return os.environ["NTBL_FILE_ID"]
+
+    def get_current_notebook_link(self):
+        return f"https://{self.base_deployment}/f/{self.get_current_notebook_id()}"
```

### Comparing `chartsworth-0.3.0/chartsworth/plot.py` & `chartsworth-0.4.0/chartsworth/plot.py`

 * *Files identical despite different names*

### Comparing `chartsworth-0.3.0/pyproject.toml` & `chartsworth-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chartsworth"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.9,<3.12"
 slack-sdk = "^3.21.3"
```

