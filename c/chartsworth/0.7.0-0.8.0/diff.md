# Comparing `tmp/chartsworth-0.7.0.tar.gz` & `tmp/chartsworth-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chartsworth-0.7.0.tar", max compression
+gzip compressed data, was "chartsworth-0.8.0.tar", max compression
```

## Comparing `chartsworth-0.7.0.tar` & `chartsworth-0.8.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0        0 2023-08-03 01:38:46.233088 chartsworth-0.7.0/README.md
--rw-r--r--   0        0        0       59 2023-08-03 01:35:50.467539 chartsworth-0.7.0/chartsworth/__init__.py
--rw-r--r--   0        0        0     5079 2023-08-04 12:51:56.068389 chartsworth-0.7.0/chartsworth/client.py
--rw-r--r--   0        0        0      927 2023-08-04 12:27:58.005085 chartsworth-0.7.0/chartsworth/plot.py
--rw-r--r--   0        0        0      617 2023-08-04 12:52:16.886246 chartsworth-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 chartsworth-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-03 01:38:46.233088 chartsworth-0.8.0/README.md
+-rw-r--r--   0        0        0       59 2023-08-03 01:35:50.467539 chartsworth-0.8.0/chartsworth/__init__.py
+-rw-r--r--   0        0        0     5130 2023-08-04 19:13:44.647897 chartsworth-0.8.0/chartsworth/client.py
+-rw-r--r--   0        0        0      272 2023-08-04 13:10:22.655346 chartsworth-0.8.0/chartsworth/emojis.py
+-rw-r--r--   0        0        0     1000 2023-08-04 17:32:53.137895 chartsworth-0.8.0/chartsworth/plot.py
+-rw-r--r--   0        0        0      659 2023-08-04 19:18:40.250484 chartsworth-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 chartsworth-0.8.0/PKG-INFO
```

### Comparing `chartsworth-0.7.0/chartsworth/client.py` & `chartsworth-0.8.0/chartsworth/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import io
 import os
 from typing import Optional, Union
 
+import matplotlib.pyplot as plt
 import PIL.Image
 from matplotlib.figure import Figure
 from slack_sdk import WebClient
 
 from .plot import create_monster_plot
 
 
@@ -86,41 +87,42 @@
         if thread_ts is None:
             thread_ts = self.__begin_thread("Post :thread:", channel=channel)
 
         self.slack_client.reactions_add(channel=channel, timestamp=thread_ts, name=name)
 
     def post_image(
         self,
-        image: Union[io.IOBase, PIL.Image.Image, Figure],
+        image: Union[io.BytesIO, PIL.Image.Image, Figure],
         filename: str,
         channel: Optional[str] = None,
     ):
         """Posts an image to a thread."""
         channel = self.__determine_channel(channel)
         thread_ts = self.threads.get(channel, None)
         if thread_ts is None:
             thread_ts = self.__begin_thread("Image :thread:", channel=channel)
 
-        image_stream: io.IOBase = io.BytesIO()
+        image_stream = io.BytesIO()
 
         if isinstance(image, PIL.Image.Image):
             image.save(image_stream, format="PNG")
         elif isinstance(image, Figure):
+            plt.close(image)
             image.savefig(image_stream, format="PNG")
         else:
             image_stream = image
 
-        image_stream.seek(0)
-
         if filename is None:
             filename = "image.png"
         filename = filename[:160]
         if not filename.endswith(".png"):
             filename += ".png"
 
+        image_stream.seek(0)
+
         self.slack_client.files_upload_v2(
             channel=channel,
             thread_ts=thread_ts,
             file=image_stream,
             filename=filename,
         )
```

### Comparing `chartsworth-0.7.0/chartsworth/plot.py` & `chartsworth-0.8.0/chartsworth/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,8 +22,11 @@
     y = 0.2 + 0.1 * np.sin(np.random.uniform(1, 10) * x + np.random.uniform(0, 2 * np.pi))
     ax.plot(x, y, color="black", linewidth=2)
 
     # Set the aspect ratio of the plot to 1 so the monster looks dope
     ax.set_aspect("equal", adjustable="box")
     ax.set_ylim(0, 1)
 
+    # Don't let matplotlib show the plot immediately
+    plt.close(fig)
+
     return fig
```

### Comparing `chartsworth-0.7.0/pyproject.toml` & `chartsworth-0.8.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chartsworth"
-version = "0.7.0"
+version = "0.8.0"
 description = ""
 authors = ["Kyle Kelley <rgbkrk@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">3.9,<3.12"
 slack-sdk = "^3.21.3"
@@ -14,14 +14,16 @@
 pillow = ">=9.0"
 
 
 [tool.poetry.group.dev.dependencies]
 mypy = "^1.4.1"
 black = "^23.7.0"
 types-pillow = "^10.0.0.2"
+ipykernel = "^6.25.0"
+ipython = "^8.14.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `chartsworth-0.7.0/PKG-INFO` & `chartsworth-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chartsworth
-Version: 0.7.0
+Version: 0.8.0
 Summary: 
 Author: Kyle Kelley
 Author-email: rgbkrk@gmail.com
 Requires-Python: >3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

