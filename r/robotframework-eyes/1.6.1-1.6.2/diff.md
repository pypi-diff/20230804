# Comparing `tmp/robotframework-eyes-1.6.1.tar.gz` & `tmp/robotframework-eyes-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-eyes-1.6.1.tar", last modified: Sun Mar 26 19:47:39 2023, max compression
+gzip compressed data, was "robotframework-eyes-1.6.2.tar", last modified: Fri Aug  4 17:42:38 2023, max compression
```

## Comparing `robotframework-eyes-1.6.1.tar` & `robotframework-eyes-1.6.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:47:39.234975 robotframework-eyes-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-26 19:47:39.230975 robotframework-eyes-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:47:39.230975 robotframework-eyes-1.6.1/RobotEyes/
--rw-r--r--   0 runner    (1001) docker     (123)    11600 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/imagemagick.py
--rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/report_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/report_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/reportgen.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/selenium_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:47:39.230975 robotframework-eyes-1.6.1/RobotEyes/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/templates/failed.html
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/templates/overview.html
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/templates/passed.html
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/templates/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/templates/test.html
--rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/RobotEyes/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 19:47:39.230975 robotframework-eyes-1.6.1/robotframework_eyes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-26 19:47:39.000000 robotframework-eyes-1.6.1/robotframework_eyes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-26 19:47:39.000000 robotframework-eyes-1.6.1/robotframework_eyes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 19:47:39.000000 robotframework-eyes-1.6.1/robotframework_eyes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-26 19:47:39.000000 robotframework-eyes-1.6.1/robotframework_eyes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 19:47:39.000000 robotframework-eyes-1.6.1/robotframework_eyes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-26 19:47:39.000000 robotframework-eyes-1.6.1/robotframework_eyes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-26 19:47:39.000000 robotframework-eyes-1.6.1/robotframework_eyes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 19:47:39.234975 robotframework-eyes-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-03-26 19:47:29.000000 robotframework-eyes-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:42:38.960980 robotframework-eyes-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-04 17:42:38.956979 robotframework-eyes-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14031 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:42:38.956979 robotframework-eyes-1.6.2/RobotEyes/
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/imagemagick.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/report_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6455 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/reportgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13246 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/selenium_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:42:38.956979 robotframework-eyes-1.6.2/RobotEyes/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/templates/failed.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/templates/overview.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/templates/passed.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/templates/test.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8042 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/RobotEyes/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 17:42:38.956979 robotframework-eyes-1.6.2/robotframework_eyes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-04 17:42:38.000000 robotframework-eyes-1.6.2/robotframework_eyes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-08-04 17:42:38.000000 robotframework-eyes-1.6.2/robotframework_eyes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:42:38.000000 robotframework-eyes-1.6.2/robotframework_eyes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-04 17:42:38.000000 robotframework-eyes-1.6.2/robotframework_eyes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 17:42:38.000000 robotframework-eyes-1.6.2/robotframework_eyes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 17:42:38.000000 robotframework-eyes-1.6.2/robotframework_eyes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 17:42:38.000000 robotframework-eyes-1.6.2/robotframework_eyes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 17:42:38.960980 robotframework-eyes-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-08-04 17:42:29.000000 robotframework-eyes-1.6.2/setup.py
```

### Comparing `robotframework-eyes-1.6.1/LICENSE` & `robotframework-eyes-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/PKG-INFO` & `robotframework-eyes-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-eyes
-Version: 1.6.1
+Version: 1.6.2
 Summary: Visual regression library and report generator for robot framework
 Home-page: https://github.com/jz-jess/RobotEyes
 Author: Jesse Zacharias
 Author-email: iamjess988@gmail.com
 License: MIT
 Keywords: visual-regression image-comparison robotframework robot-eyes
 Classifier: Framework :: Robot Framework
```

### Comparing `robotframework-eyes-1.6.1/README.md` & `robotframework-eyes-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/RobotEyes/__init__.py` & `robotframework-eyes-1.6.2/RobotEyes/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,29 +191,29 @@
 
         if not os.path.exists(self.path):
             os.makedirs(self.path)
 
     def _resize(self, *args):
         for arg in args:
             img = Image.open(arg)
-            img = img.resize((1024, 700), Image.ANTIALIAS)
+            img = img.resize((1024, 700), Image.LANCZOS)
             img.save(arg)
 
     def _fix_base_image_size(self, path, image_name):
         test_name = self.test_name.replace(' ', '_')
         base_image = os.path.join(self.baseline_dir, test_name, image_name)
         if os.path.exists(base_image):
             im = Image.open(path)
             width, height = im.size
             im.close()
 
             im = Image.open(base_image)
             b_width, b_height = im.size
             if width != b_width or height != b_height:
-                im = im.resize((width, height), Image.ANTIALIAS)
+                im = im.resize((width, height), Image.LANCZOS)
                 im.save(base_image)
 
     def _delete_report_if_old(self, path):
         t1 = datetime.fromtimestamp(os.path.getmtime(path))
         t2 = datetime.now()
         diff = (t2 - t1).seconds
         os.remove(path) if diff > REPORT_EXPIRATION_THRESHOLD else ''
```

### Comparing `robotframework-eyes-1.6.1/RobotEyes/imagemagick.py` & `robotframework-eyes-1.6.2/RobotEyes/imagemagick.py`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/RobotEyes/report_generator.py` & `robotframework-eyes-1.6.2/RobotEyes/report_generator.py`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/RobotEyes/report_utils.py` & `robotframework-eyes-1.6.2/RobotEyes/report_utils.py`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/RobotEyes/reportgen.py` & `robotframework-eyes-1.6.2/RobotEyes/reportgen.py`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/RobotEyes/runner.py` & `robotframework-eyes-1.6.2/RobotEyes/runner.py`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/RobotEyes/selenium_hooks.py` & `robotframework-eyes-1.6.2/RobotEyes/selenium_hooks.py`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/RobotEyes/templates/base.html` & `robotframework-eyes-1.6.2/RobotEyes/templates/base.html`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/RobotEyes/templates/failed.html` & `robotframework-eyes-1.6.2/RobotEyes/templates/failed.html`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/RobotEyes/templates/overview.html` & `robotframework-eyes-1.6.2/RobotEyes/templates/overview.html`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/RobotEyes/templates/passed.html` & `robotframework-eyes-1.6.2/RobotEyes/templates/passed.html`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/RobotEyes/templates/report.html` & `robotframework-eyes-1.6.2/RobotEyes/templates/report.html`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/RobotEyes/templates/test.html` & `robotframework-eyes-1.6.2/RobotEyes/templates/test.html`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/RobotEyes/web.py` & `robotframework-eyes-1.6.2/RobotEyes/web.py`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/robotframework_eyes.egg-info/PKG-INFO` & `robotframework-eyes-1.6.2/robotframework_eyes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-eyes
-Version: 1.6.1
+Version: 1.6.2
 Summary: Visual regression library and report generator for robot framework
 Home-page: https://github.com/jz-jess/RobotEyes
 Author: Jesse Zacharias
 Author-email: iamjess988@gmail.com
 License: MIT
 Keywords: visual-regression image-comparison robotframework robot-eyes
 Classifier: Framework :: Robot Framework
```

### Comparing `robotframework-eyes-1.6.1/robotframework_eyes.egg-info/SOURCES.txt` & `robotframework-eyes-1.6.2/robotframework_eyes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-eyes-1.6.1/setup.py` & `robotframework-eyes-1.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-version = '1.6.1'
+version = '1.6.2'
 
 setup(name='robotframework-eyes',
       version=version,
       description="Visual regression library and report generator for robot framework",
       long_description="""\
 Visual regression library and report generator for robot framework. Capture elements, fullscreens and compare them against baseline images. Extends Selenium2Libary. Visit https://github.com/jz-jess/RobotEyes for documentation.""",
       classifiers=[
```

