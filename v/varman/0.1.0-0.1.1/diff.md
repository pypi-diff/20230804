# Comparing `tmp/varman-0.1.0.tar.gz` & `tmp/varman-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "varman-0.1.0.tar", last modified: Fri Aug  4 02:51:23 2023, max compression
+gzip compressed data, was "varman-0.1.1.tar", last modified: Fri Aug  4 03:50:40 2023, max compression
```

## Comparing `varman-0.1.0.tar` & `varman-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 02:51:23.017953 varman-0.1.0/
--rw-rw-rw-   0        0        0     1084 2023-08-03 04:17:23.000000 varman-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3018 2023-08-04 02:51:23.016969 varman-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2578 2023-08-04 02:50:05.000000 varman-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-08-04 02:51:23.017953 varman-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      630 2023-08-04 02:48:54.000000 varman-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:51:22.998817 varman-0.1.0/varman/
--rw-rw-rw-   0        0        0     4168 2023-08-04 02:43:45.000000 varman-0.1.0/varman/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 02:51:23.015964 varman-0.1.0/varman.egg-info/
--rw-rw-rw-   0        0        0     3018 2023-08-04 02:51:22.000000 varman-0.1.0/varman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      165 2023-08-04 02:51:22.000000 varman-0.1.0/varman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 02:51:22.000000 varman-0.1.0/varman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-08-04 02:51:22.000000 varman-0.1.0/varman.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 03:50:40.118948 varman-0.1.1/
+-rw-rw-rw-   0        0        0     1084 2023-08-03 04:17:23.000000 varman-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2977 2023-08-04 03:50:40.117949 varman-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2578 2023-08-04 02:50:05.000000 varman-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 03:50:40.118948 varman-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      638 2023-08-04 03:50:26.000000 varman-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 03:50:40.106955 varman-0.1.1/varman/
+-rw-rw-rw-   0        0        0     4168 2023-08-04 02:43:45.000000 varman-0.1.1/varman/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 03:50:40.116949 varman-0.1.1/varman.egg-info/
+-rw-rw-rw-   0        0        0     2977 2023-08-04 03:50:39.000000 varman-0.1.1/varman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      165 2023-08-04 03:50:39.000000 varman-0.1.1/varman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 03:50:39.000000 varman-0.1.1/varman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-08-04 03:50:39.000000 varman-0.1.1/varman.egg-info/top_level.txt
```

### Comparing `varman-0.1.0/LICENSE` & `varman-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `varman-0.1.0/PKG-INFO` & `varman-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: varman
-Version: 0.1.0
-Summary: A dict like variable container, listen for variable changes.
+Version: 0.1.1
+Summary: A dict like variable manager, listen for variable changes.
 Home-page: https://github.com/zlolss/VarMan.py.git
 Author: zloss
-Author-email: zlos@foxmail.com
-Classifier: Programming Language :: Python :: 3
+Author-email: zlols@foxmail.com
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VarMan
 
 一个辅助监听变量赋值变化的类，基本用法类似dict类型
```

### Comparing `varman-0.1.0/README.md` & `varman-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `varman-0.1.0/setup.py` & `varman-0.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="varman",
-  version="0.1.0",
+  version="0.1.1",
   author="zloss",
-  author_email="zlos@foxmail.com",
-  description="A dict like variable container, listen for variable changes.",
+  author_email="zlols@foxmail.com",
+  description="A dict like variable manager, listen for variable changes.",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/zlolss/VarMan.py.git",
   packages=setuptools.find_packages(),
   classifiers=[
-  "Programming Language :: Python :: 3",
+  "Programming Language :: Python :: 3 :: Only",
   "License :: OSI Approved :: MIT License",
-  "Operating System :: OS Independent",
+  #"Operating System :: OS Independent",
   ],
 )
```

### Comparing `varman-0.1.0/varman/__init__.py` & `varman-0.1.1/varman/__init__.py`

 * *Files identical despite different names*

### Comparing `varman-0.1.0/varman.egg-info/PKG-INFO` & `varman-0.1.1/varman.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: varman
-Version: 0.1.0
-Summary: A dict like variable container, listen for variable changes.
+Version: 0.1.1
+Summary: A dict like variable manager, listen for variable changes.
 Home-page: https://github.com/zlolss/VarMan.py.git
 Author: zloss
-Author-email: zlos@foxmail.com
-Classifier: Programming Language :: Python :: 3
+Author-email: zlols@foxmail.com
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VarMan
 
 一个辅助监听变量赋值变化的类，基本用法类似dict类型
```

