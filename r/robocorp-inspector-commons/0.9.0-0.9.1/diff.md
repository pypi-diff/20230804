# Comparing `tmp/robocorp_inspector_commons-0.9.0.tar.gz` & `tmp/robocorp_inspector_commons-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_inspector_commons-0.9.0.tar", max compression
+gzip compressed data, was "robocorp_inspector_commons-0.9.1.tar", max compression
```

## Comparing `robocorp_inspector_commons-0.9.0.tar` & `robocorp_inspector_commons-0.9.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    17242 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/LICENSE
--rw-r--r--   0        0        0     1592 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/README.md
--rw-r--r--   0        0        0      105 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/__init__.py
--rw-r--r--   0        0        0      249 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/api/__init__.py
--rw-r--r--   0        0        0     1242 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/api/bridge_interface.py
--rw-r--r--   0        0        0      197 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/api/database_interface.py
--rw-r--r--   0        0        0        0 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/bridge/__init__.py
--rw-r--r--   0        0        0     1116 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/bridge/base.py
--rw-r--r--   0        0        0     7080 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/bridge/bridge_browser.py
--rw-r--r--   0        0        0     7195 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/bridge/bridge_recorder.py
--rw-r--r--   0        0        0     2263 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/bridge/bridge_windows.py
--rw-r--r--   0        0        0      782 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/bridge/mixin.py
--rw-r--r--   0        0        0      846 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/config.py
--rw-r--r--   0        0        0     1800 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/context.py
--rw-r--r--   0        0        0     6925 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/database.py
--rw-r--r--   0        0        0    17336 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/driver_web.py
--rw-r--r--   0        0        0    10917 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/driver_windows.py
--rw-r--r--   0        0        0     1121 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/metric.py
--rw-r--r--   0        0        0     7239 2023-03-09 10:07:18.566096 robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/browser-recording-guide.html
--rw-r--r--   0        0        0    27050 2023-03-09 10:07:18.566096 robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/builder.js
--rw-r--r--   0        0        0       59 2023-03-09 10:07:18.566096 robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/builder.js.LICENSE.txt
--rw-r--r--   0        0        0     5942 2023-03-09 10:07:18.566096 robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/guide.html
--rw-r--r--   0        0        0     2456 2023-03-09 10:07:18.566096 robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/inspector.css
--rw-r--r--   0        0        0    27053 2023-03-09 10:07:18.566096 robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/inspector.js
--rw-r--r--   0        0        0       59 2023-03-09 10:07:18.566096 robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/inspector.js.LICENSE.txt
--rw-r--r--   0        0        0    27055 2023-03-09 10:07:18.566096 robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/webRecorder.js
--rw-r--r--   0        0        0       59 2023-03-09 10:07:18.566096 robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/webRecorder.js.LICENSE.txt
--rw-r--r--   0        0        0     3460 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/telemetry.py
--rw-r--r--   0        0        0     3890 2023-03-09 10:04:39.707760 robocorp_inspector_commons-0.9.0/inspector_commons/utils.py
--rw-r--r--   0        0        0     1329 2023-03-09 10:04:39.715760 robocorp_inspector_commons-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     2741 1970-01-01 00:00:00.000000 robocorp_inspector_commons-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    17242 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/LICENSE
+-rw-r--r--   0        0        0     1592 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/README.md
+-rw-r--r--   0        0        0      105 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/__init__.py
+-rw-r--r--   0        0        0      249 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/api/__init__.py
+-rw-r--r--   0        0        0     1242 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/api/bridge_interface.py
+-rw-r--r--   0        0        0      197 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/api/database_interface.py
+-rw-r--r--   0        0        0        0 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/bridge/__init__.py
+-rw-r--r--   0        0        0     1116 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/bridge/base.py
+-rw-r--r--   0        0        0     6992 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/bridge/bridge_browser.py
+-rw-r--r--   0        0        0     7195 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/bridge/bridge_recorder.py
+-rw-r--r--   0        0        0     2263 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/bridge/bridge_windows.py
+-rw-r--r--   0        0        0      782 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/bridge/mixin.py
+-rw-r--r--   0        0        0      846 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/config.py
+-rw-r--r--   0        0        0     1800 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/context.py
+-rw-r--r--   0        0        0     6925 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/database.py
+-rw-r--r--   0        0        0    17318 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/driver_web.py
+-rw-r--r--   0        0        0    10917 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/driver_windows.py
+-rw-r--r--   0        0        0     1121 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/metric.py
+-rw-r--r--   0        0        0     7239 2023-03-13 15:03:33.521134 robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/browser-recording-guide.html
+-rw-r--r--   0        0        0    27050 2023-03-13 15:03:33.521134 robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/builder.js
+-rw-r--r--   0        0        0       59 2023-03-13 15:03:33.521134 robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/builder.js.LICENSE.txt
+-rw-r--r--   0        0        0     5942 2023-03-13 15:03:33.521134 robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/guide.html
+-rw-r--r--   0        0        0     2456 2023-03-13 15:03:33.521134 robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/inspector.css
+-rw-r--r--   0        0        0    27053 2023-03-13 15:03:33.521134 robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/inspector.js
+-rw-r--r--   0        0        0       59 2023-03-13 15:03:33.521134 robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/inspector.js.LICENSE.txt
+-rw-r--r--   0        0        0    27055 2023-03-13 15:03:33.521134 robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/webRecorder.js
+-rw-r--r--   0        0        0       59 2023-03-13 15:03:33.521134 robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/webRecorder.js.LICENSE.txt
+-rw-r--r--   0        0        0     3460 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/telemetry.py
+-rw-r--r--   0        0        0     3972 2023-03-13 15:01:16.915144 robocorp_inspector_commons-0.9.1/inspector_commons/utils.py
+-rw-r--r--   0        0        0     1329 2023-03-13 15:01:16.919144 robocorp_inspector_commons-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     2741 1970-01-01 00:00:00.000000 robocorp_inspector_commons-0.9.1/PKG-INFO
```

### Comparing `robocorp_inspector_commons-0.9.0/LICENSE` & `robocorp_inspector_commons-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/README.md` & `robocorp_inspector_commons-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/api/bridge_interface.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/api/bridge_interface.py`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/bridge/base.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/bridge/base.py`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/bridge/bridge_browser.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/bridge/bridge_browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import os
 import sys
 import time
 import traceback as tb
 from typing import Optional
 
 import requests
 
 from inspector_commons.bridge.base import Bridge, traceback
 from inspector_commons.bridge.mixin import DatabaseMixin
 from inspector_commons.driver_web import WebDriver, WebDriverError
-from inspector_commons.utils import force_kill_process_children
+from inspector_commons.utils import force_kill_process
 
 
 class BrowserBridge(DatabaseMixin, Bridge):
     """Javascript API bridge for browser locators."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -105,16 +104,15 @@
         self,
         only_kill_app: bool = False,
         only_kill_browser: bool = False,
     ):
         kill_all = only_kill_browser is False and only_kill_app is False
         if kill_all:
             self.logger.warning("Using force kill to close the app window")
-            force_kill_process_children(logger=self.logger)
-            os._exit(0)  # pylint: disable=protected-access
+            force_kill_process(logger=self.logger)
         if only_kill_app:
             self.logger.debug("Destroying app window...")
             self.close()
         if only_kill_browser and self.web_driver:
             self.logger.debug("Destroying web driver...")
             self.web_driver.stop()
```

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/bridge/bridge_recorder.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/bridge/bridge_recorder.py`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/bridge/bridge_windows.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/bridge/bridge_windows.py`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/bridge/mixin.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/bridge/mixin.py`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/config.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/config.py`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/context.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/context.py`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/database.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/database.py`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/driver_web.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/driver_web.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     StaleElementReferenceException,
     TimeoutException,
     WebDriverException,
 )
 from selenium.webdriver import ActionChains, ChromeOptions, Remote  # type: ignore
 from selenium.webdriver.common.by import By  # type: ignore
 
-from inspector_commons.utils import force_kill_process_children  # type: ignore
+from inspector_commons.utils import force_kill_process  # type: ignore
 
 
 class WebDriverExceptions(Exception):
     def __init__(
         self,
         msg: Optional[str] = None,
         errors: Optional[Dict[str, WebDriverException]] = None,
@@ -342,15 +342,15 @@
 
         if self.is_remote:
             self.logger.debug("Skipping close for remote browser")
             return
 
         try:
             if self.selenium:
-                force_kill_process_children(
+                force_kill_process(
                     logger=self.logger, pid=self.selenium.service.process.pid
                 )
                 self.logger.debug("Finished stopping browser child processes!")
             else:
                 self.logger.debug("Skipped force stopping browser.")
         except Exception as ex:  # pylint: disable=W0703
             self.logger.error("There was an error while stopping driver: %s", ex)
```

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/driver_windows.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/driver_windows.py`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/metric.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/metric.py`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/browser-recording-guide.html` & `robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/browser-recording-guide.html`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/builder.js` & `robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/builder.js`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/guide.html` & `robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/guide.html`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/inspector.css` & `robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/inspector.css`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/inspector.js` & `robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/inspector.js`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/static/resources/webRecorder.js` & `robocorp_inspector_commons-0.9.1/inspector_commons/static/resources/webRecorder.js`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/telemetry.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/telemetry.py`

 * *Files identical despite different names*

### Comparing `robocorp_inspector_commons-0.9.0/inspector_commons/utils.py` & `robocorp_inspector_commons-0.9.1/inspector_commons/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
             return stop
 
         return wrapper
 
     return decorator
 
 
-def force_kill_process_children(logger, pid=None, suspend=False):
+def force_kill_process(logger, pid=None, suspend=False):
     try:
         # if pid is None will kill all children of current process
         current_proc = psutil.Process(pid)
         _suspend_process(logger=logger, proc=current_proc, suspend=suspend)
 
         if current_proc.is_running():
             logger.debug("Stopping children of process: %s", current_proc.pid)
@@ -62,28 +62,31 @@
 
             # go through the children and try to kill each one
             for child in children:
                 try:
                     # if the child process has children, we go through those first
                     grandchildren = _get_process_children(logger=logger, proc=child)
                     if len(grandchildren) > 0:
-                        force_kill_process_children(logger=logger, pid=child.pid)
+                        force_kill_process(logger=logger, pid=child.pid)
 
                     # attempt to kill the child process
                     logger.debug("Stopping child process: %s", child.pid)
                     _send_kill_to_process(logger=logger, proc=child)
                 except Exception as error:  # pylint: disable=W0703
                     logger.debug(
                         f"Continuing, but there was an error killing process: {error}"
                     )
             # check if there are any processes left (zombies) that we should kill
             _, alive = psutil.wait_procs(children, timeout=2)
             for child in alive:
                 logger.debug(f"Killing process still alive: {child}")
                 _send_kill_to_process(logger=logger, proc=child)
+
+            # kill the process
+            _send_kill_to_process(logger=logger, proc=current_proc)
         else:
             logger.debug("Process not running: %s", pid)
     except Exception as error:  # pylint: disable=W0703
         logger.debug(f"There was an error while killing process: {error}")
 
 
 def _send_kill_to_process(logger, proc):
```

### Comparing `robocorp_inspector_commons-0.9.0/pyproject.toml` & `robocorp_inspector_commons-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-inspector-commons"
-version = "0.9.0"
+version = "0.9.1"
 description = "Robocorp Inspector Commons"
 
 authors = ["Robocorp <dev@robocorp.com>"]
 repository = "https://github.com/robocorp/inspector"
 license = "Proprietary"
 readme = "README.md"
```

### Comparing `robocorp_inspector_commons-0.9.0/PKG-INFO` & `robocorp_inspector_commons-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robocorp-inspector-commons
-Version: 0.9.0
+Version: 0.9.1
 Summary: Robocorp Inspector Commons
 Home-page: https://github.com/robocorp/inspector
 License: Proprietary
 Author: Robocorp
 Author-email: dev@robocorp.com
 Requires-Python: >=3.7,<3.11
 Classifier: License :: Other/Proprietary License
```

