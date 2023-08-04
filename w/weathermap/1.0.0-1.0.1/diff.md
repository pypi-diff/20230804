# Comparing `tmp/weathermap-1.0.0.tar.gz` & `tmp/weathermap-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weathermap-1.0.0.tar", last modified: Thu Aug  3 23:29:20 2023, max compression
+gzip compressed data, was "weathermap-1.0.1.tar", last modified: Fri Aug  4 00:33:20 2023, max compression
```

## Comparing `weathermap-1.0.0.tar` & `weathermap-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 23:29:20.707326 weathermap-1.0.0/
--rw-rw-rw-   0        0        0      660 2023-08-03 23:29:20.707326 weathermap-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-03 23:29:20.708323 weathermap-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      848 2023-08-03 23:22:48.000000 weathermap-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-03 23:29:20.694361 weathermap-1.0.0/weathermap/
--rw-rw-rw-   0        0        0       41 2023-08-03 23:11:08.000000 weathermap-1.0.0/weathermap/_init_.py
--rw-rw-rw-   0        0        0     3154 2023-08-03 22:55:34.000000 weathermap-1.0.0/weathermap/weathermap.py
-drwxrwxrwx   0        0        0        0 2023-08-03 23:29:20.705331 weathermap-1.0.0/weathermap.egg-info/
--rw-rw-rw-   0        0        0      660 2023-08-03 23:29:20.000000 weathermap-1.0.0/weathermap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      223 2023-08-03 23:29:20.000000 weathermap-1.0.0/weathermap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 23:29:20.000000 weathermap-1.0.0/weathermap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-08-03 23:29:20.000000 weathermap-1.0.0/weathermap.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-03 23:29:20.000000 weathermap-1.0.0/weathermap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 00:33:20.906709 weathermap-1.0.1/
+-rw-rw-rw-   0        0        0      660 2023-08-04 00:33:20.906709 weathermap-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-04 00:33:20.906709 weathermap-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      866 2023-08-04 00:33:06.000000 weathermap-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 00:33:20.887758 weathermap-1.0.1/weathermap/
+-rw-rw-rw-   0        0        0       41 2023-08-03 23:11:08.000000 weathermap-1.0.1/weathermap/_init_.py
+-rw-rw-rw-   0        0        0     2960 2023-08-03 23:54:04.000000 weathermap-1.0.1/weathermap/weathermap.py
+drwxrwxrwx   0        0        0        0 2023-08-04 00:33:20.905711 weathermap-1.0.1/weathermap.egg-info/
+-rw-rw-rw-   0        0        0      660 2023-08-04 00:33:20.000000 weathermap-1.0.1/weathermap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2023-08-04 00:33:20.000000 weathermap-1.0.1/weathermap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 00:33:20.000000 weathermap-1.0.1/weathermap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-04 00:33:20.000000 weathermap-1.0.1/weathermap.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 00:33:20.000000 weathermap-1.0.1/weathermap.egg-info/top_level.txt
```

### Comparing `weathermap-1.0.0/PKG-INFO` & `weathermap-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weathermap
-Version: 1.0.0
+Version: 1.0.1
 Summary: Openweathermap api simplified
 Home-page: https://github.com/savan2508/WeatherApp
 Author: Savan Patel
 Author-email: sawanpatel2508@gmail.com
 Keywords: weather,forecast,openweathermap,openweather
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `weathermap-1.0.0/setup.py` & `weathermap-1.0.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='weathermap',
-    version='1.0.0',
+    version='1.0.1',
     description='Openweathermap api simplified',
     author='Savan Patel',
     author_email='sawanpatel2508@gmail.com',
     url='https://github.com/savan2508/WeatherApp',
-    packages=['weathermap'],
+    packages=find_packages(exclude=['tests']),
     keywords=['weather', 'forecast', 'openweathermap', 'openweather'],
     install_requires=[
         'requests',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

### Comparing `weathermap-1.0.0/weathermap/weathermap.py` & `weathermap-1.0.1/weathermap/weathermap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,8 @@
 import requests
-import os
-import pprint
-from dotenv import load_dotenv
-
-# Load the contents of the .env file into the environment variables
-load_dotenv()
-
-openweather_api = os.getenv('OPENWEATHER_API')
 
 
 class Weather:
     """
     Weather Class:
 
     This class allows you to create a weather object by providing an API key along with either a city name or
```

### Comparing `weathermap-1.0.0/weathermap.egg-info/PKG-INFO` & `weathermap-1.0.1/weathermap.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weathermap
-Version: 1.0.0
+Version: 1.0.1
 Summary: Openweathermap api simplified
 Home-page: https://github.com/savan2508/WeatherApp
 Author: Savan Patel
 Author-email: sawanpatel2508@gmail.com
 Keywords: weather,forecast,openweathermap,openweather
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

