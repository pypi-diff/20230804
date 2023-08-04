# Comparing `tmp/rogue_tools-1.1.1.tar.gz` & `tmp/rogue_tools-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rogue_tools-1.1.1.tar", last modified: Thu Aug  3 02:25:56 2023, max compression
+gzip compressed data, was "rogue_tools-1.1.2.tar", last modified: Fri Aug  4 04:07:16 2023, max compression
```

## Comparing `rogue_tools-1.1.1.tar` & `rogue_tools-1.1.2.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 02:25:56.388913 rogue_tools-1.1.1/
--rw-rw-rw-   0        0        0      517 2023-08-03 02:25:56.387935 rogue_tools-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-03 02:25:56.377199 rogue_tools-1.1.1/rogue_tools/
--rw-rw-rw-   0        0        0        0 2023-04-12 11:49:44.000000 rogue_tools-1.1.1/rogue_tools/__init__.py
--rw-rw-rw-   0        0        0     7903 2023-07-28 08:16:04.000000 rogue_tools-1.1.1/rogue_tools/android_tool.py
--rw-rw-rw-   0        0        0     6558 2023-07-19 04:12:11.000000 rogue_tools-1.1.1/rogue_tools/excel_tool.py
--rw-rw-rw-   0        0        0     4070 2023-07-27 12:24:15.000000 rogue_tools-1.1.1/rogue_tools/file_tool.py
--rw-rw-rw-   0        0        0     1157 2023-07-19 04:12:11.000000 rogue_tools-1.1.1/rogue_tools/filter_tool.py
--rw-rw-rw-   0        0        0     2353 2023-07-19 04:12:11.000000 rogue_tools-1.1.1/rogue_tools/ini_tool.py
--rw-rw-rw-   0        0        0    13293 2023-07-31 06:11:18.000000 rogue_tools-1.1.1/rogue_tools/path_tool.py
--rw-rw-rw-   0        0        0     3380 2023-07-19 04:12:11.000000 rogue_tools-1.1.1/rogue_tools/robot_tool.py
--rw-rw-rw-   0        0        0     4064 2023-07-19 04:12:11.000000 rogue_tools-1.1.1/rogue_tools/show_tool.py
--rw-rw-rw-   0        0        0      147 2023-07-19 04:12:11.000000 rogue_tools-1.1.1/rogue_tools/string_tool.py
--rw-rw-rw-   0        0        0     1287 2023-07-31 09:35:35.000000 rogue_tools-1.1.1/rogue_tools/thread_tool.py
--rw-rw-rw-   0        0        0     2087 2023-08-01 03:05:11.000000 rogue_tools-1.1.1/rogue_tools/time_tool.py
--rw-rw-rw-   0        0        0     5052 2023-08-02 08:56:19.000000 rogue_tools-1.1.1/rogue_tools/ui_tool.py
--rw-rw-rw-   0        0        0     2300 2023-07-19 04:12:11.000000 rogue_tools-1.1.1/rogue_tools/web_tool.py
--rw-rw-rw-   0        0        0    17995 2023-07-19 04:12:11.000000 rogue_tools-1.1.1/rogue_tools/win_tool.py
--rw-rw-rw-   0        0        0     3860 2023-07-19 04:12:11.000000 rogue_tools-1.1.1/rogue_tools/yaml_tool.py
--rw-rw-rw-   0        0        0     1260 2023-07-19 04:12:11.000000 rogue_tools-1.1.1/rogue_tools/zip_tool.py
-drwxrwxrwx   0        0        0        0 2023-08-03 02:25:56.385984 rogue_tools-1.1.1/rogue_tools.egg-info/
--rw-rw-rw-   0        0        0      517 2023-08-03 02:25:56.000000 rogue_tools-1.1.1/rogue_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      641 2023-08-03 02:25:56.000000 rogue_tools-1.1.1/rogue_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 02:25:56.000000 rogue_tools-1.1.1/rogue_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-08-03 02:25:56.000000 rogue_tools-1.1.1/rogue_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-03 02:25:56.000000 rogue_tools-1.1.1/rogue_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2023-08-03 02:25:56.000000 rogue_tools-1.1.1/rogue_tools.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2023-08-03 02:25:56.389889 rogue_tools-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1749 2023-08-03 02:25:37.000000 rogue_tools-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:07:16.043119 rogue_tools-1.1.2/
+-rw-rw-rw-   0        0        0      517 2023-08-04 04:07:16.042142 rogue_tools-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-04 04:07:16.031407 rogue_tools-1.1.2/rogue_tools/
+-rw-rw-rw-   0        0        0        0 2023-04-12 11:49:44.000000 rogue_tools-1.1.2/rogue_tools/__init__.py
+-rw-rw-rw-   0        0        0     7903 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/android_tool.py
+-rw-rw-rw-   0        0        0     6558 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/excel_tool.py
+-rw-rw-rw-   0        0        0     4070 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/file_tool.py
+-rw-rw-rw-   0        0        0     1157 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/filter_tool.py
+-rw-rw-rw-   0        0        0     2353 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/ini_tool.py
+-rw-rw-rw-   0        0        0     2620 2023-08-04 03:23:20.000000 rogue_tools-1.1.2/rogue_tools/install_tools.py
+-rw-rw-rw-   0        0        0    13293 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/path_tool.py
+-rw-rw-rw-   0        0        0     3380 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/robot_tool.py
+-rw-rw-rw-   0        0        0     4064 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/show_tool.py
+-rw-rw-rw-   0        0        0      147 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/string_tool.py
+-rw-rw-rw-   0        0        0     1287 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/thread_tool.py
+-rw-rw-rw-   0        0        0     2087 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/time_tool.py
+-rw-rw-rw-   0        0        0     5052 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/ui_tool.py
+-rw-rw-rw-   0        0        0     2300 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/web_tool.py
+-rw-rw-rw-   0        0        0    17995 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/win_tool.py
+-rw-rw-rw-   0        0        0     3860 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/yaml_tool.py
+-rw-rw-rw-   0        0        0     1260 2023-08-04 04:04:12.000000 rogue_tools-1.1.2/rogue_tools/zip_tool.py
+drwxrwxrwx   0        0        0        0 2023-08-04 04:07:16.040190 rogue_tools-1.1.2/rogue_tools.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-08-04 04:07:15.000000 rogue_tools-1.1.2/rogue_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      670 2023-08-04 04:07:15.000000 rogue_tools-1.1.2/rogue_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 04:07:15.000000 rogue_tools-1.1.2/rogue_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-08-04 04:07:15.000000 rogue_tools-1.1.2/rogue_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-04 04:07:15.000000 rogue_tools-1.1.2/rogue_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-08-04 04:07:15.000000 rogue_tools-1.1.2/rogue_tools.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2023-08-04 04:07:16.043119 rogue_tools-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1749 2023-08-04 04:05:42.000000 rogue_tools-1.1.2/setup.py
```

### Comparing `rogue_tools-1.1.1/PKG-INFO` & `rogue_tools-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue_tools
-Version: 1.1.1
+Version: 1.1.2
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.1.1/rogue_tools/android_tool.py` & `rogue_tools-1.1.2/rogue_tools/android_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/excel_tool.py` & `rogue_tools-1.1.2/rogue_tools/excel_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/file_tool.py` & `rogue_tools-1.1.2/rogue_tools/file_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/filter_tool.py` & `rogue_tools-1.1.2/rogue_tools/filter_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/ini_tool.py` & `rogue_tools-1.1.2/rogue_tools/ini_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/path_tool.py` & `rogue_tools-1.1.2/rogue_tools/path_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/robot_tool.py` & `rogue_tools-1.1.2/rogue_tools/robot_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/show_tool.py` & `rogue_tools-1.1.2/rogue_tools/show_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/thread_tool.py` & `rogue_tools-1.1.2/rogue_tools/thread_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/time_tool.py` & `rogue_tools-1.1.2/rogue_tools/time_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/ui_tool.py` & `rogue_tools-1.1.2/rogue_tools/ui_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/web_tool.py` & `rogue_tools-1.1.2/rogue_tools/web_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/win_tool.py` & `rogue_tools-1.1.2/rogue_tools/win_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/yaml_tool.py` & `rogue_tools-1.1.2/rogue_tools/yaml_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools/zip_tool.py` & `rogue_tools-1.1.2/rogue_tools/zip_tool.py`

 * *Files identical despite different names*

### Comparing `rogue_tools-1.1.1/rogue_tools.egg-info/PKG-INFO` & `rogue_tools-1.1.2/rogue_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rogue-tools
-Version: 1.1.1
+Version: 1.1.2
 Summary: private tools
 Home-page: 
 Author: luohao
 Author-email: luohao@aobi.com
 License: MIT
 Classifier: Operating System :: Microsoft
 Classifier: Intended Audience :: Developers
```

### Comparing `rogue_tools-1.1.1/rogue_tools.egg-info/SOURCES.txt` & `rogue_tools-1.1.2/rogue_tools.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 setup.py
 rogue_tools/__init__.py
 rogue_tools/android_tool.py
 rogue_tools/excel_tool.py
 rogue_tools/file_tool.py
 rogue_tools/filter_tool.py
 rogue_tools/ini_tool.py
+rogue_tools/install_tools.py
 rogue_tools/path_tool.py
 rogue_tools/robot_tool.py
 rogue_tools/show_tool.py
 rogue_tools/string_tool.py
 rogue_tools/thread_tool.py
 rogue_tools/time_tool.py
 rogue_tools/ui_tool.py
```

### Comparing `rogue_tools-1.1.1/setup.py` & `rogue_tools-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 path_tool.del_('rogue_tools.egg-info')
 time.sleep(3)
 
 
 setup(
     name='rogue_tools',  # 包的名字
     author='luohao',  # 作者
-    version='1.1.1',  # 版本号
+    version='1.1.2',  # 版本号
     license='MIT',
 
     description='private tools',  # 描述
     long_description='''long description''',
     author_email='luohao@aobi.com',  # 你的邮箱**
     url='',  # 可以写github上的地址，或者其他地址
     # 包内需要引用的文件夹
```

