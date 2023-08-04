# Comparing `tmp/detool-1.0.7.tar.gz` & `tmp/detool-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/detool-1.0.7.tar", last modified: Tue Aug  2 09:57:40 2022, max compression
+gzip compressed data, was "dist/detool-1.0.8.tar", last modified: Fri Aug  4 17:07:33 2023, max compression
```

## Comparing `detool-1.0.7.tar` & `detool-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-08-02 09:57:40.000000 detool-1.0.7/
--rw-r--r--   0 admin      (501) staff       (20)     1856 2022-08-02 09:57:40.000000 detool-1.0.7/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      664 2022-08-02 09:57:30.000000 detool-1.0.7/README.md
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-08-02 09:57:40.000000 detool-1.0.7/detool/
--rw-r--r--   0 admin      (501) staff       (20)      193 2022-07-01 06:30:59.000000 detool-1.0.7/detool/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)     3136 2022-08-02 09:56:30.000000 detool-1.0.7/detool/decr_reids_cache.py
--rw-r--r--   0 admin      (501) staff       (20)      653 2022-06-09 14:51:49.000000 detool-1.0.7/detool/decr_run_times.py
--rw-r--r--   0 admin      (501) staff       (20)      803 2022-06-07 15:08:29.000000 detool-1.0.7/detool/decr_timer.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2022-08-02 09:57:40.000000 detool-1.0.7/detool.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     1856 2022-08-02 09:57:39.000000 detool-1.0.7/detool.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      259 2022-08-02 09:57:39.000000 detool-1.0.7/detool.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2022-08-02 09:57:39.000000 detool-1.0.7/detool.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)       27 2022-08-02 09:57:39.000000 detool-1.0.7/detool.egg-info/requires.txt
--rw-r--r--   0 admin      (501) staff       (20)        7 2022-08-02 09:57:39.000000 detool-1.0.7/detool.egg-info/top_level.txt
--rw-r--r--   0 admin      (501) staff       (20)       38 2022-08-02 09:57:40.000000 detool-1.0.7/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1278 2022-08-02 09:55:59.000000 detool-1.0.7/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-04 17:07:33.000000 detool-1.0.8/
+-rw-r--r--   0 admin      (501) staff       (20)     2349 2023-08-04 17:07:33.000000 detool-1.0.8/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-04 17:07:33.000000 detool-1.0.8/detool.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     2349 2023-08-04 17:07:32.000000 detool-1.0.8/detool.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      284 2023-08-04 17:07:33.000000 detool-1.0.8/detool.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)       27 2023-08-04 17:07:32.000000 detool-1.0.8/detool.egg-info/requires.txt
+-rw-r--r--   0 admin      (501) staff       (20)        7 2023-08-04 17:07:32.000000 detool-1.0.8/detool.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-04 17:07:32.000000 detool-1.0.8/detool.egg-info/dependency_links.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-04 17:07:33.000000 detool-1.0.8/detool/
+-rw-r--r--   0 admin      (501) staff       (20)      653 2022-06-09 14:51:49.000000 detool-1.0.8/detool/decr_run_times.py
+-rw-r--r--   0 admin      (501) staff       (20)      803 2022-06-07 15:08:29.000000 detool-1.0.8/detool/decr_timer.py
+-rw-r--r--   0 admin      (501) staff       (20)      267 2023-08-04 17:06:57.000000 detool-1.0.8/detool/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1164 2023-08-04 17:06:57.000000 detool-1.0.8/detool/decr_class_log.py
+-rw-r--r--   0 admin      (501) staff       (20)     3136 2022-08-02 09:56:30.000000 detool-1.0.8/detool/decr_reids_cache.py
+-rw-r--r--   0 admin      (501) staff       (20)     1011 2023-08-04 17:06:57.000000 detool-1.0.8/README.md
+-rw-r--r--   0 admin      (501) staff       (20)     1288 2023-08-04 17:06:57.000000 detool-1.0.8/setup.py
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-08-04 17:07:33.000000 detool-1.0.8/setup.cfg
```

### Comparing `detool-1.0.7/PKG-INFO` & `detool-1.0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: detool
-Version: 1.0.7
+Version: 1.0.8
 Summary: decorator tool collection
 Home-page: UNKNOWN
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
-Maintainer: cc
+Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
 Description: [![Supported Versions](https://img.shields.io/pypi/pyversions/leek.svg)](https://pypi.org/project/leek)
         ### 常用装饰器工具集
                           
         #### pip安装
         ```shell
@@ -37,14 +37,31 @@
             def sum_t(a, b):
                 print(f'{a}+{b}={a + b}')
                 return a + b
         
             r = sum_t(1, 2)
             print(r)
         ```
+        #### 3.日志装饰器
+        ```python
+            from detool import class_log_decorator,log_decorator
+            
+            @class_log_decorator
+            class Cal(object):
+                def __init__(self, c):
+                    self.c = c
+        
+                def sum(self, a, b):
+                    return a + b
+            @log_decorator
+            def calculate(a, b):
+                return a + b
+        
+            Cal(3).sum(a=3, b=6)
+        ```
 Keywords: detool,decorators
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `detool-1.0.7/detool/decr_reids_cache.py` & `detool-1.0.8/detool/decr_reids_cache.py`

 * *Files identical despite different names*

### Comparing `detool-1.0.7/detool/decr_run_times.py` & `detool-1.0.8/detool/decr_run_times.py`

 * *Files identical despite different names*

### Comparing `detool-1.0.7/detool/decr_timer.py` & `detool-1.0.8/detool/decr_timer.py`

 * *Files identical despite different names*

### Comparing `detool-1.0.7/detool.egg-info/PKG-INFO` & `detool-1.0.8/detool.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: detool
-Version: 1.0.7
+Version: 1.0.8
 Summary: decorator tool collection
 Home-page: UNKNOWN
 Author: abo123456789
 Author-email: abcdef123456chen@sohu.com
-Maintainer: cc
+Maintainer: abo123456789
 Maintainer-email: abcdef123456chen@sohu.com
 License: MIT License
 Description: [![Supported Versions](https://img.shields.io/pypi/pyversions/leek.svg)](https://pypi.org/project/leek)
         ### 常用装饰器工具集
                           
         #### pip安装
         ```shell
@@ -37,14 +37,31 @@
             def sum_t(a, b):
                 print(f'{a}+{b}={a + b}')
                 return a + b
         
             r = sum_t(1, 2)
             print(r)
         ```
+        #### 3.日志装饰器
+        ```python
+            from detool import class_log_decorator,log_decorator
+            
+            @class_log_decorator
+            class Cal(object):
+                def __init__(self, c):
+                    self.c = c
+        
+                def sum(self, a, b):
+                    return a + b
+            @log_decorator
+            def calculate(a, b):
+                return a + b
+        
+            Cal(3).sum(a=3, b=6)
+        ```
 Keywords: detool,decorators
 Platform: all
 Classifier: Development Status :: 4 - Beta
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `detool-1.0.7/setup.py` & `detool-1.0.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 # @Author cc
 # @TIME 2019/5/25 23:26
 
 from setuptools import setup, find_packages
 
 setup(
     name='detool',
-    version='1.0.7',
+    version='1.0.8',
     description=(
         'decorator tool collection'
     ),
     keywords=("detool", "decorators"),
     long_description_content_type="text/markdown",
     long_description=open('README.md', encoding='utf-8').read(),
     author='abo123456789',
     author_email='abcdef123456chen@sohu.com',
-    maintainer='cc',
+    maintainer='abo123456789',
     maintainer_email='abcdef123456chen@sohu.com',
     license='MIT License',
     install_requires=[
         "loguru>=0.6.0",
         "redis>=3.0.0"
     ],
     packages=find_packages(),
```

