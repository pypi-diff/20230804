# Comparing `tmp/MoreApi-0.4.tar.gz` & `tmp/MoreApi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MoreApi-0.4.tar", last modified: Fri Aug  4 03:37:33 2023, max compression
+gzip compressed data, was "MoreApi-0.4.1.tar", last modified: Fri Aug  4 03:43:23 2023, max compression
```

## Comparing `MoreApi-0.4.tar` & `MoreApi-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-08-04 03:37:33.857868 MoreApi-0.4/
--rw-r--r--   0 liulu      (501) staff       (20)    11357 2023-07-29 03:24:25.000000 MoreApi-0.4/LICENSE
-drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-08-04 03:37:33.855151 MoreApi-0.4/MoreAPI/
--rw-r--r--   0 liulu      (501) staff       (20)      696 2023-08-04 03:35:20.000000 MoreApi-0.4/MoreAPI/Auth.py
--rw-r--r--   0 liulu      (501) staff       (20)     1861 2023-08-04 03:35:20.000000 MoreApi-0.4/MoreAPI/DouYin.py
--rw-r--r--   0 liulu      (501) staff       (20)     2359 2023-08-04 03:33:57.000000 MoreApi-0.4/MoreAPI/KS.py
--rw-r--r--   0 liulu      (501) staff       (20)     1093 2023-08-04 03:35:20.000000 MoreApi-0.4/MoreAPI/KuWo.py
--rw-r--r--   0 liulu      (501) staff       (20)      656 2023-08-04 03:35:20.000000 MoreApi-0.4/MoreAPI/Video.py
--rw-r--r--   0 liulu      (501) staff       (20)     3781 2023-08-04 03:35:20.000000 MoreApi-0.4/MoreAPI/XHS.py
--rw-r--r--   0 liulu      (501) staff       (20)      126 2023-07-29 06:46:10.000000 MoreApi-0.4/MoreAPI/__init__.py
-drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-08-04 03:37:33.857097 MoreApi-0.4/MoreApi.egg-info/
--rw-r--r--   0 liulu      (501) staff       (20)     2494 2023-08-04 03:37:33.000000 MoreApi-0.4/MoreApi.egg-info/PKG-INFO
--rw-r--r--   0 liulu      (501) staff       (20)      296 2023-08-04 03:37:33.000000 MoreApi-0.4/MoreApi.egg-info/SOURCES.txt
--rw-r--r--   0 liulu      (501) staff       (20)        1 2023-08-04 03:37:33.000000 MoreApi-0.4/MoreApi.egg-info/dependency_links.txt
--rw-r--r--   0 liulu      (501) staff       (20)        9 2023-08-04 03:37:33.000000 MoreApi-0.4/MoreApi.egg-info/requires.txt
--rw-r--r--   0 liulu      (501) staff       (20)        8 2023-08-04 03:37:33.000000 MoreApi-0.4/MoreApi.egg-info/top_level.txt
--rw-r--r--   0 liulu      (501) staff       (20)     2494 2023-08-04 03:37:33.857586 MoreApi-0.4/PKG-INFO
--rw-r--r--   0 liulu      (501) staff       (20)     2152 2023-07-29 07:28:57.000000 MoreApi-0.4/README.md
--rw-r--r--   0 liulu      (501) staff       (20)       38 2023-08-04 03:37:33.857995 MoreApi-0.4/setup.cfg
--rw-r--r--   0 liulu      (501) staff       (20)      715 2023-08-04 03:35:20.000000 MoreApi-0.4/setup.py
+drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-08-04 03:43:23.939297 MoreApi-0.4.1/
+-rw-r--r--   0 liulu      (501) staff       (20)    11357 2023-07-29 03:24:25.000000 MoreApi-0.4.1/LICENSE
+drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-08-04 03:43:23.936324 MoreApi-0.4.1/MoreAPI/
+-rw-r--r--   0 liulu      (501) staff       (20)      696 2023-08-04 03:35:20.000000 MoreApi-0.4.1/MoreAPI/Auth.py
+-rw-r--r--   0 liulu      (501) staff       (20)     1861 2023-08-04 03:35:20.000000 MoreApi-0.4.1/MoreAPI/DouYin.py
+-rw-r--r--   0 liulu      (501) staff       (20)     2359 2023-08-04 03:33:57.000000 MoreApi-0.4.1/MoreAPI/KS.py
+-rw-r--r--   0 liulu      (501) staff       (20)     1093 2023-08-04 03:35:20.000000 MoreApi-0.4.1/MoreAPI/KuWo.py
+-rw-r--r--   0 liulu      (501) staff       (20)      656 2023-08-04 03:35:20.000000 MoreApi-0.4.1/MoreAPI/Video.py
+-rw-r--r--   0 liulu      (501) staff       (20)     3781 2023-08-04 03:35:20.000000 MoreApi-0.4.1/MoreAPI/XHS.py
+-rw-r--r--   0 liulu      (501) staff       (20)      152 2023-08-04 03:42:09.000000 MoreApi-0.4.1/MoreAPI/__init__.py
+drwxr-xr-x   0 liulu      (501) staff       (20)        0 2023-08-04 03:43:23.938412 MoreApi-0.4.1/MoreApi.egg-info/
+-rw-r--r--   0 liulu      (501) staff       (20)     2496 2023-08-04 03:43:23.000000 MoreApi-0.4.1/MoreApi.egg-info/PKG-INFO
+-rw-r--r--   0 liulu      (501) staff       (20)      296 2023-08-04 03:43:23.000000 MoreApi-0.4.1/MoreApi.egg-info/SOURCES.txt
+-rw-r--r--   0 liulu      (501) staff       (20)        1 2023-08-04 03:43:23.000000 MoreApi-0.4.1/MoreApi.egg-info/dependency_links.txt
+-rw-r--r--   0 liulu      (501) staff       (20)        9 2023-08-04 03:43:23.000000 MoreApi-0.4.1/MoreApi.egg-info/requires.txt
+-rw-r--r--   0 liulu      (501) staff       (20)        8 2023-08-04 03:43:23.000000 MoreApi-0.4.1/MoreApi.egg-info/top_level.txt
+-rw-r--r--   0 liulu      (501) staff       (20)     2496 2023-08-04 03:43:23.938910 MoreApi-0.4.1/PKG-INFO
+-rw-r--r--   0 liulu      (501) staff       (20)     2152 2023-07-29 07:28:57.000000 MoreApi-0.4.1/README.md
+-rw-r--r--   0 liulu      (501) staff       (20)       38 2023-08-04 03:43:23.939447 MoreApi-0.4.1/setup.cfg
+-rw-r--r--   0 liulu      (501) staff       (20)      717 2023-08-04 03:43:00.000000 MoreApi-0.4.1/setup.py
```

### Comparing `MoreApi-0.4/LICENSE` & `MoreApi-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MoreApi-0.4/MoreAPI/Auth.py` & `MoreApi-0.4.1/MoreAPI/Auth.py`

 * *Files identical despite different names*

### Comparing `MoreApi-0.4/MoreAPI/DouYin.py` & `MoreApi-0.4.1/MoreAPI/DouYin.py`

 * *Files identical despite different names*

### Comparing `MoreApi-0.4/MoreAPI/KS.py` & `MoreApi-0.4.1/MoreAPI/KS.py`

 * *Files identical despite different names*

### Comparing `MoreApi-0.4/MoreAPI/KuWo.py` & `MoreApi-0.4.1/MoreAPI/KuWo.py`

 * *Files identical despite different names*

### Comparing `MoreApi-0.4/MoreAPI/Video.py` & `MoreApi-0.4.1/MoreAPI/Video.py`

 * *Files identical despite different names*

### Comparing `MoreApi-0.4/MoreAPI/XHS.py` & `MoreApi-0.4.1/MoreAPI/XHS.py`

 * *Files identical despite different names*

### Comparing `MoreApi-0.4/MoreApi.egg-info/PKG-INFO` & `MoreApi-0.4.1/MoreApi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MoreApi
-Version: 0.4
+Version: 0.4.1
 Summary: MoreAPI是抖音/酷我/小红书/快手等各视频平台非官方的RESTful API平台。
 Home-page: https://github.com/liulu1550/MoreAPI.git
 Author: MoreCoding
 Author-email: wouldmissyou@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `MoreApi-0.4/PKG-INFO` & `MoreApi-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MoreApi
-Version: 0.4
+Version: 0.4.1
 Summary: MoreAPI是抖音/酷我/小红书/快手等各视频平台非官方的RESTful API平台。
 Home-page: https://github.com/liulu1550/MoreAPI.git
 Author: MoreCoding
 Author-email: wouldmissyou@163.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `MoreApi-0.4/README.md` & `MoreApi-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `MoreApi-0.4/setup.py` & `MoreApi-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import (setup, find_packages)
 
 setup(
 
     name="MoreApi",  # 包名
     author='MoreCoding',  #作者
-    version="0.4",  # 版本
+    version="0.4.1",  # 版本
     url='https://github.com/liulu1550/MoreAPI.git',  # github地址
     description='MoreAPI是抖音/酷我/小红书/快手等各视频平台非官方的RESTful API平台。',  #包的简述
     long_description=open('README.md', encoding='utf-8').read(),  # #包的详细介绍
     long_description_content_type="text/markdown",
     # 需要包含的子包列表
     packages=find_packages(),
     author_email='wouldmissyou@163.com',
```

