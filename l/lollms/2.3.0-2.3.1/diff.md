# Comparing `tmp/lollms-2.3.0.tar.gz` & `tmp/lollms-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lollms-2.3.0.tar", last modified: Wed Aug  2 23:06:32 2023, max compression
+gzip compressed data, was "lollms-2.3.1.tar", last modified: Fri Aug  4 08:28:27 2023, max compression
```

## Comparing `lollms-2.3.0.tar` & `lollms-2.3.1.tar`

### file list

```diff
@@ -1,50 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 23:06:32.052549 lollms-2.3.0/
--rw-rw-rw-   0        0        0    11558 2023-06-03 19:43:42.000000 lollms-2.3.0/LICENSE
--rw-rw-rw-   0        0        0      269 2023-07-19 17:46:44.000000 lollms-2.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11076 2023-08-02 23:06:32.051540 lollms-2.3.0/PKG-INFO
--rw-rw-rw-   0        0        0    10600 2023-06-18 10:10:09.000000 lollms-2.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 23:06:31.962833 lollms-2.3.0/lollms/
--rw-rw-rw-   0        0        0      146 2023-06-21 07:49:26.000000 lollms-2.3.0/lollms/__init__.py
--rw-rw-rw-   0        0        0     9679 2023-07-31 20:58:01.000000 lollms-2.3.0/lollms/app.py
-drwxrwxrwx   0        0        0        0 2023-08-02 23:06:31.986271 lollms-2.3.0/lollms/apps/
--rw-rw-rw-   0        0        0        0 2023-07-19 16:50:10.000000 lollms-2.3.0/lollms/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 23:06:31.987273 lollms-2.3.0/lollms/apps/console/
--rw-rw-rw-   0        0        0    14754 2023-07-27 19:45:11.000000 lollms-2.3.0/lollms/apps/console/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 23:06:31.988269 lollms-2.3.0/lollms/apps/playground/
--rw-rw-rw-   0        0        0      398 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 23:06:32.038199 lollms-2.3.0/lollms/apps/playground/static/
--rw-rw-rw-   0        0        0    11558 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/static/LICENSE
--rw-rw-rw-   0        0        0     3900 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/static/README.md
--rw-rw-rw-   0        0        0      566 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/static/index.html
--rw-rw-rw-   0        0        0   470378 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/static/logo.png
--rw-rw-rw-   0        0        0    16548 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/static/lollms_playground.html
--rw-rw-rw-   0        0        0       62 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/apps/playground/static/package.json
-drwxrwxrwx   0        0        0        0 2023-08-02 23:06:32.040229 lollms-2.3.0/lollms/apps/server/
--rw-rw-rw-   0        0        0    34757 2023-07-31 12:14:38.000000 lollms-2.3.0/lollms/apps/server/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 23:06:32.041241 lollms-2.3.0/lollms/apps/settings/
--rw-rw-rw-   0        0        0     7710 2023-07-31 12:14:48.000000 lollms-2.3.0/lollms/apps/settings/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 23:06:32.043239 lollms-2.3.0/lollms/assets/
--rw-rw-rw-   0        0        0   470378 2023-06-12 16:11:49.000000 lollms-2.3.0/lollms/assets/logo.png
--rw-rw-rw-   0        0        0    11094 2023-07-31 22:09:20.000000 lollms-2.3.0/lollms/binding.py
--rw-rw-rw-   0        0        0    21426 2023-07-02 17:51:25.000000 lollms-2.3.0/lollms/config.py
-drwxrwxrwx   0        0        0        0 2023-08-02 23:06:32.050270 lollms-2.3.0/lollms/configs/
--rw-rw-rw-   0        0        0      881 2023-07-19 16:42:16.000000 lollms-2.3.0/lollms/configs/config.yaml
--rw-rw-rw-   0        0        0     4418 2023-07-02 12:47:59.000000 lollms-2.3.0/lollms/data.py
--rw-rw-rw-   0        0        0     1357 2023-07-03 19:35:14.000000 lollms-2.3.0/lollms/extension.py
--rw-rw-rw-   0        0        0     3027 2023-07-16 00:19:49.000000 lollms-2.3.0/lollms/helpers.py
--rw-rw-rw-   0        0        0     9348 2023-06-12 16:11:49.000000 lollms-2.3.0/lollms/langchain_integration.py
--rw-rw-rw-   0        0        0     7239 2023-07-03 22:53:18.000000 lollms-2.3.0/lollms/main_config.py
--rw-rw-rw-   0        0        0    13693 2023-07-20 17:32:43.000000 lollms-2.3.0/lollms/paths.py
--rw-rw-rw-   0        0        0    50389 2023-08-02 20:41:38.000000 lollms-2.3.0/lollms/personality.py
--rw-rw-rw-   0        0        0    22076 2023-07-30 22:49:52.000000 lollms-2.3.0/lollms/terminal.py
--rw-rw-rw-   0        0        0     2811 2023-08-02 11:44:56.000000 lollms-2.3.0/lollms/types.py
--rw-rw-rw-   0        0        0    28641 2023-08-01 19:44:49.000000 lollms-2.3.0/lollms/utilities.py
-drwxrwxrwx   0        0        0        0 2023-08-02 23:06:31.985255 lollms-2.3.0/lollms.egg-info/
--rw-rw-rw-   0        0        0    11076 2023-08-02 23:06:31.000000 lollms-2.3.0/lollms.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      947 2023-08-02 23:06:31.000000 lollms-2.3.0/lollms.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 23:06:31.000000 lollms-2.3.0/lollms.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      192 2023-08-02 23:06:31.000000 lollms-2.3.0/lollms.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      245 2023-08-02 23:06:31.000000 lollms-2.3.0/lollms.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-02 23:06:31.000000 lollms-2.3.0/lollms.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 23:06:32.052549 lollms-2.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1870 2023-08-02 23:06:07.000000 lollms-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 08:28:27.085233 lollms-2.3.1/
+-rw-rw-rw-   0        0        0    11558 2023-06-13 07:51:48.000000 lollms-2.3.1/LICENSE
+-rw-rw-rw-   0        0        0      269 2023-07-20 07:07:55.000000 lollms-2.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    11076 2023-08-04 08:28:27.084233 lollms-2.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10600 2023-06-19 06:38:19.000000 lollms-2.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 08:28:27.046233 lollms-2.3.1/lollms/
+-rw-rw-rw-   0        0        0      146 2023-06-21 11:55:03.000000 lollms-2.3.1/lollms/__init__.py
+-rw-rw-rw-   0        0        0     9679 2023-08-03 06:57:52.000000 lollms-2.3.1/lollms/app.py
+drwxrwxrwx   0        0        0        0 2023-08-04 08:28:27.058232 lollms-2.3.1/lollms/apps/
+-rw-rw-rw-   0        0        0        0 2023-07-20 07:07:55.000000 lollms-2.3.1/lollms/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 08:28:27.060231 lollms-2.3.1/lollms/apps/console/
+-rw-rw-rw-   0        0        0    14754 2023-07-27 11:31:56.000000 lollms-2.3.1/lollms/apps/console/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 08:28:27.062232 lollms-2.3.1/lollms/apps/playground/
+-rw-rw-rw-   0        0        0      398 2023-07-19 13:43:20.000000 lollms-2.3.1/lollms/apps/playground/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 08:28:27.075231 lollms-2.3.1/lollms/apps/playground/static/
+-rw-rw-rw-   0        0        0    11558 2023-07-19 06:49:31.000000 lollms-2.3.1/lollms/apps/playground/static/LICENSE
+-rw-rw-rw-   0        0        0     3900 2023-07-19 06:49:31.000000 lollms-2.3.1/lollms/apps/playground/static/README.md
+-rw-rw-rw-   0        0        0      566 2023-07-19 06:49:31.000000 lollms-2.3.1/lollms/apps/playground/static/index.html
+-rw-rw-rw-   0        0        0   470378 2023-07-19 06:49:31.000000 lollms-2.3.1/lollms/apps/playground/static/logo.png
+-rw-rw-rw-   0        0        0    16548 2023-07-27 09:45:58.000000 lollms-2.3.1/lollms/apps/playground/static/lollms_playground.html
+-rw-rw-rw-   0        0        0       57 2023-07-19 13:38:20.000000 lollms-2.3.1/lollms/apps/playground/static/package.json
+drwxrwxrwx   0        0        0        0 2023-08-04 08:28:27.077257 lollms-2.3.1/lollms/apps/server/
+-rw-rw-rw-   0        0        0    34757 2023-08-03 06:57:52.000000 lollms-2.3.1/lollms/apps/server/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 08:28:27.078235 lollms-2.3.1/lollms/apps/settings/
+-rw-rw-rw-   0        0        0     7710 2023-08-03 06:57:52.000000 lollms-2.3.1/lollms/apps/settings/__init__.py
+-rw-rw-rw-   0        0        0    11094 2023-08-03 06:57:52.000000 lollms-2.3.1/lollms/binding.py
+-rw-rw-rw-   0        0        0    21426 2023-07-04 06:37:19.000000 lollms-2.3.1/lollms/config.py
+drwxrwxrwx   0        0        0        0 2023-08-04 08:28:27.082233 lollms-2.3.1/lollms/configs/
+-rw-rw-rw-   0        0        0      881 2023-07-19 12:34:44.000000 lollms-2.3.1/lollms/configs/config.yaml
+-rw-rw-rw-   0        0        0     4418 2023-07-04 06:37:19.000000 lollms-2.3.1/lollms/data.py
+-rw-rw-rw-   0        0        0     1357 2023-07-04 06:37:19.000000 lollms-2.3.1/lollms/extension.py
+-rw-rw-rw-   0        0        0     3027 2023-07-19 06:49:31.000000 lollms-2.3.1/lollms/helpers.py
+-rw-rw-rw-   0        0        0     9348 2023-06-13 07:51:48.000000 lollms-2.3.1/lollms/langchain_integration.py
+-rw-rw-rw-   0        0        0     7330 2023-08-04 07:49:45.000000 lollms-2.3.1/lollms/main_config.py
+-rw-rw-rw-   0        0        0    13693 2023-07-20 07:10:22.000000 lollms-2.3.1/lollms/paths.py
+-rw-rw-rw-   0        0        0    50414 2023-08-03 12:17:14.000000 lollms-2.3.1/lollms/personality.py
+-rw-rw-rw-   0        0        0    22076 2023-08-03 06:57:52.000000 lollms-2.3.1/lollms/terminal.py
+-rw-rw-rw-   0        0        0     2811 2023-08-03 06:57:52.000000 lollms-2.3.1/lollms/types.py
+-rw-rw-rw-   0        0        0    30044 2023-08-04 07:40:27.000000 lollms-2.3.1/lollms/utilities.py
+drwxrwxrwx   0        0        0        0 2023-08-04 08:28:27.057231 lollms-2.3.1/lollms.egg-info/
+-rw-rw-rw-   0        0        0    11076 2023-08-04 08:28:26.000000 lollms-2.3.1/lollms.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      924 2023-08-04 08:28:26.000000 lollms-2.3.1/lollms.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 08:28:26.000000 lollms-2.3.1/lollms.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      192 2023-08-04 08:28:26.000000 lollms-2.3.1/lollms.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      245 2023-08-04 08:28:26.000000 lollms-2.3.1/lollms.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-04 08:28:26.000000 lollms-2.3.1/lollms.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 08:28:27.086233 lollms-2.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1870 2023-08-04 08:28:07.000000 lollms-2.3.1/setup.py
```

### Comparing `lollms-2.3.0/LICENSE` & `lollms-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/PKG-INFO` & `lollms-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.3.0
+Version: 2.3.1
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.3.0/README.md` & `lollms-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/app.py` & `lollms-2.3.1/lollms/app.py`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/apps/console/__init__.py` & `lollms-2.3.1/lollms/apps/console/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/apps/playground/static/LICENSE` & `lollms-2.3.1/lollms/apps/playground/static/LICENSE`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/apps/playground/static/README.md` & `lollms-2.3.1/lollms/apps/playground/static/README.md`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/apps/playground/static/index.html` & `lollms-2.3.1/lollms/apps/playground/static/index.html`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/apps/playground/static/logo.png` & `lollms-2.3.1/lollms/apps/playground/static/logo.png`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/apps/playground/static/lollms_playground.html` & `lollms-2.3.1/lollms/apps/playground/static/lollms_playground.html`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/apps/server/__init__.py` & `lollms-2.3.1/lollms/apps/server/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/apps/settings/__init__.py` & `lollms-2.3.1/lollms/apps/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/binding.py` & `lollms-2.3.1/lollms/binding.py`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/config.py` & `lollms-2.3.1/lollms/config.py`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/configs/config.yaml` & `lollms-2.3.1/lollms/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/data.py` & `lollms-2.3.1/lollms/data.py`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/extension.py` & `lollms-2.3.1/lollms/extension.py`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/helpers.py` & `lollms-2.3.1/lollms/helpers.py`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/langchain_integration.py` & `lollms-2.3.1/lollms/langchain_integration.py`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/main_config.py` & `lollms-2.3.1/lollms/main_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,14 +171,15 @@
         folder_path = self.lollms_paths.personal_models_path/self.binding_name
         model_name  = path.split("/")[-1]+".reference"
         model_full_path = (folder_path / model_name)
 
         # Check if file already exists in folder
         if model_full_path.exists():
             print("File already exists in folder")
+            return False
         else:
             # Create folder if it doesn't exist
             folder_path.mkdir(parents=True, exist_ok=True)
             with open(model_full_path,"w") as f:
                 f.write(path)
-            print("Reference created, please make sure you don't delete the file or you will have broken link")
-
+            ASCIIColors.warning("Reference created, please make sure you don't delete or move the referenced file. This can cause the link to be broken")
+            return True
```

### Comparing `lollms-2.3.0/lollms/paths.py` & `lollms-2.3.1/lollms/paths.py`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/personality.py` & `lollms-2.3.1/lollms/personality.py`

 * *Files 0% similar despite different names*

```diff
@@ -1189,23 +1189,23 @@
         Args:
             inf (str): The information to be sent
             callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the step to. Defaults to None.
         """
         if callback:
             callback(info, MSG_TYPE.MSG_TYPE_INFO)
 
-    def json(self, json_infos:dict, callback: Callable[[str, int, dict], bool]=None):
+    def json(self, json_infos:dict, callback: Callable[[str, int, dict], bool]=None, indent=4):
         """This sends json data to front end
 
         Args:
             step_text (dict): The step text
             callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the step to. Defaults to None.
         """
         if callback:
-            callback(json.dumps(json_infos), MSG_TYPE.MSG_TYPE_JSON_INFOS)
+            callback(json.dumps(json_infos, indent=indent), MSG_TYPE.MSG_TYPE_JSON_INFOS)
 
     def ui(self, html_ui:str, callback: Callable[[str, int, dict], bool]=None):
         """This sends ui elements to front end
 
         Args:
             step_text (dict): The step text
             callback (callable, optional): A callable with this signature (str, MSG_TYPE) to send the step to. Defaults to None.
```

### Comparing `lollms-2.3.0/lollms/terminal.py` & `lollms-2.3.1/lollms/terminal.py`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/types.py` & `lollms-2.3.1/lollms/types.py`

 * *Files identical despite different names*

### Comparing `lollms-2.3.0/lollms/utilities.py` & `lollms-2.3.1/lollms/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,53 @@
 from lollms.paths import LollmsPaths
 from sklearn.feature_extraction.text import TfidfVectorizer
 import numpy as np
 from pathlib import Path
 import json
 import re
 import subprocess
+import gc
+
+class AdvancedGarbageCollector:
+    @staticmethod
+    def hardCollect(obj):
+        all_referrers = gc.get_referrers(obj)
+        for referrer in all_referrers:
+            if not isinstance(referrer, (list, tuple, dict, set)):
+                referrer = None
+        del obj
+
+    @staticmethod
+    def safeHardCollect(variable_name, instance=None):
+        if instance is not None:
+            if hasattr(instance, variable_name):
+                obj = getattr(instance, variable_name)
+                AdvancedGarbageCollector.hardCollect(obj)
+            else:
+                print(f"The variable '{variable_name}' does not exist in the instance.")
+        else:
+            if variable_name in locals():
+                obj = locals()[variable_name]
+                AdvancedGarbageCollector.hardCollect(obj)
+            elif variable_name in globals():
+                obj = globals()[variable_name]
+                AdvancedGarbageCollector.hardCollect(obj)
+            else:
+                print(f"The variable '{variable_name}' does not exist in the local or global namespace.")
+
+    @staticmethod
+    def safeHardCollectMultiple(variable_names, instance=None):
+        for variable_name in variable_names:
+            AdvancedGarbageCollector.safeHardCollect(variable_name, instance)
+
+    @staticmethod
+    def collect():
+        gc.collect()
+
+
 class PackageManager:
     @staticmethod
     def install_package(package_name):
         import subprocess
         import sys
         subprocess.check_call([sys.executable, "-m", "pip", "install", package_name])
```

### Comparing `lollms-2.3.0/lollms.egg-info/PKG-INFO` & `lollms-2.3.1/lollms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lollms
-Version: 2.3.0
+Version: 2.3.1
 Summary: A python library for AI personality definition
 Home-page: https://github.com/ParisNeo/lollms
 Author: Saifeddine ALOUI
 Author-email: aloui.saifeddine@gmail.com
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `lollms-2.3.0/lollms.egg-info/SOURCES.txt` & `lollms-2.3.1/lollms.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,9 +29,8 @@
 lollms/apps/playground/static/README.md
 lollms/apps/playground/static/index.html
 lollms/apps/playground/static/logo.png
 lollms/apps/playground/static/lollms_playground.html
 lollms/apps/playground/static/package.json
 lollms/apps/server/__init__.py
 lollms/apps/settings/__init__.py
-lollms/assets/logo.png
 lollms/configs/config.yaml
```

### Comparing `lollms-2.3.0/setup.py` & `lollms-2.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if file_path.is_file():
             if file_path.name != "__pycache__" and file_path.suffix !=".pyc" and  file_path.name!="local_config.yaml" and file_path.name!=".installed" and file_path.name!=".git" and file_path.name!=".gitignore":
                 file_list.append("/".join(str(file_path).replace("\\","/").split("/")[1:]))
     return file_list
 
 setuptools.setup(
     name="lollms",
-    version="2.3.0",
+    version="2.3.1",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/lollms",
     packages=setuptools.find_packages(),
```

