# Comparing `tmp/webmeter-1.0.2.tar.gz` & `tmp/webmeter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/webmeter/webmeter/dist/.tmp-s4jvp3g7/webmeter-1.0.2.tar", last modified: Thu Aug  3 10:06:19 2023, max compression
+gzip compressed data, was "/home/runner/work/webmeter/webmeter/dist/.tmp-ffgk5c64/webmeter-1.0.3.tar", last modified: Fri Aug  4 00:31:28 2023, max compression
```

## Comparing `webmeter-1.0.2.tar` & `webmeter-1.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 10:06:10.000000 webmeter-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-08-03 10:06:10.000000 webmeter-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-03 10:06:19.000000 webmeter-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-03 10:06:10.000000 webmeter-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-03 10:06:19.000000 webmeter-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-03 10:06:10.000000 webmeter-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter/
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter/public/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/public/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter/static/image/
--rw-r--r--   0 runner    (1001) docker     (123)   126687 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/static/image/empty.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    29743 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/templates/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter/view/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/view/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/view/page.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-08-03 10:06:10.000000 webmeter-1.0.2/webmeter/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-03 10:06:19.000000 webmeter-1.0.2/webmeter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:31:28.000000 webmeter-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-04 00:31:15.000000 webmeter-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-04 00:31:15.000000 webmeter-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-04 00:31:28.000000 webmeter-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-04 00:31:15.000000 webmeter-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-08-04 00:31:28.000000 webmeter-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-08-04 00:31:15.000000 webmeter-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:31:28.000000 webmeter-1.0.3/webmeter/
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-08-04 00:31:15.000000 webmeter-1.0.3/webmeter/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:31:28.000000 webmeter-1.0.3/webmeter/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-08-04 00:31:15.000000 webmeter-1.0.3/webmeter/public/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:31:28.000000 webmeter-1.0.3/webmeter/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:31:28.000000 webmeter-1.0.3/webmeter/static/image/
+-rw-r--r--   0 runner    (1001) docker     (123)   126687 2023-08-04 00:31:15.000000 webmeter-1.0.3/webmeter/static/image/empty.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:31:28.000000 webmeter-1.0.3/webmeter/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    29743 2023-08-04 00:31:15.000000 webmeter-1.0.3/webmeter/templates/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:31:28.000000 webmeter-1.0.3/webmeter/view/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-08-04 00:31:15.000000 webmeter-1.0.3/webmeter/view/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-04 00:31:15.000000 webmeter-1.0.3/webmeter/view/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-08-04 00:31:15.000000 webmeter-1.0.3/webmeter/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 00:31:28.000000 webmeter-1.0.3/webmeter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-04 00:31:28.000000 webmeter-1.0.3/webmeter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-08-04 00:31:28.000000 webmeter-1.0.3/webmeter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 00:31:28.000000 webmeter-1.0.3/webmeter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-04 00:31:28.000000 webmeter-1.0.3/webmeter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 00:31:28.000000 webmeter-1.0.3/webmeter.egg-info/top_level.txt
```

### Comparing `webmeter-1.0.2/LICENSE` & `webmeter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `webmeter-1.0.2/PKG-INFO` & `webmeter-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webmeter
-Version: 1.0.2
+Version: 1.0.3
 Summary: WebMeter - A web api-performance tool based on jmeter.
 Home-page: https://github.com/rafa0128/webmeter
 Author: Rafa Chen
 Author-email: laoqi1988_f1@126.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `webmeter-1.0.2/setup.py` & `webmeter-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     install_requires=['fastapi','uvicorn', 'requests', 'logzero', 'fire','pyfiglet','psutil'],
-    version='1.0.2',
+    version='1.0.3',
     long_description=long_description,
     long_description_content_type="text/markdown",
     description="WebMeter - A web api-performance tool based on jmeter.",
     packages=setuptools.find_namespace_packages(include=["webmeter", "webmeter.*"], ),
     include_package_data=True
 )
```

### Comparing `webmeter-1.0.2/webmeter/main.py` & `webmeter-1.0.3/webmeter/__main__.py`

 * *Files identical despite different names*

### Comparing `webmeter-1.0.2/webmeter/static/image/empty.png` & `webmeter-1.0.3/webmeter/static/image/empty.png`

 * *Files identical despite different names*

### Comparing `webmeter-1.0.2/webmeter/templates/index.html` & `webmeter-1.0.3/webmeter/templates/index.html`

 * *Files identical despite different names*

### Comparing `webmeter-1.0.2/webmeter/web.py` & `webmeter-1.0.3/webmeter/web.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 def status(host: str, port: int):
     r = requests.get('http://{}:{}/plan'.format(host, port), timeout=2.0)
     flag = (True, False)[r.status_code == 200]
     return flag
 
 def start(host: str, port: int):
-    uvicorn.run("main:app", host=host, port=port, reload=False)
+    uvicorn.run("__main__:app", host=host, port=port, reload=False)
 
 def open(host: str, port: int):
     flag = True
     while flag:
         flag = status(host, port)
     webbrowser.open('http://{}:{}/plan'.format(host, port), new=2)
```

### Comparing `webmeter-1.0.2/webmeter.egg-info/PKG-INFO` & `webmeter-1.0.3/webmeter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webmeter
-Version: 1.0.2
+Version: 1.0.3
 Summary: WebMeter - A web api-performance tool based on jmeter.
 Home-page: https://github.com/rafa0128/webmeter
 Author: Rafa Chen
 Author-email: laoqi1988_f1@126.com
 License: MIT
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

