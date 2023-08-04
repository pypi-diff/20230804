# Comparing `tmp/tybase-0.2.0.tar.gz` & `tmp/tybase-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.2.0.tar", last modified: Thu Jul 20 05:55:18 2023, max compression
+gzip compressed data, was "tybase-0.2.2.tar", last modified: Fri Aug  4 16:23:14 2023, max compression
```

## Comparing `tybase-0.2.0.tar` & `tybase-0.2.2.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-07-20 05:55:18.862044 tybase-0.2.0/
--rw-rw-rw-   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.2.0/MANIFEST.in
--rw-r--r--   0 zhangte    (501) staff       (20)      805 2023-07-20 05:55:18.861798 tybase-0.2.0/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.2.0/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-07-20 05:55:18.862136 tybase-0.2.0/setup.cfg
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1049 2023-07-20 05:55:02.000000 tybase-0.2.0/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-07-20 05:55:18.857476 tybase-0.2.0/tybase/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.2.0/tybase/__init__.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-07-20 05:55:18.858794 tybase-0.2.0/tybase/baidu/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.2.0/tybase/baidu/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.2.0/tybase/baidu/kw_tool.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.2.0/tybase/datatest.txt
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-07-20 05:55:18.859663 tybase-0.2.0/tybase/dbtool/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.2.0/tybase/dbtool/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.2.0/tybase/dbtool/data_import.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.2.0/tybase/dbtool/mysql.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-07-20 05:55:18.860114 tybase-0.2.0/tybase/lc/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.2.0/tybase/lc/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.2.0/tybase/lc/eg1.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-07-20 05:55:18.861530 tybase-0.2.0/tybase/tools/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.2.0/tybase/tools/__init__.py
--rw-r--r--   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.2.0/tybase/tools/ali_oss_tools.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.2.0/tybase/tools/qiniu_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.2.0/tybase/tools/riqit_tools.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.2.0/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-07-20 05:55:18.858536 tybase-0.2.0/tybase.egg-info/
--rw-rw-rw-   0 zhangte    (501) staff       (20)      805 2023-07-20 05:55:18.000000 tybase-0.2.0/tybase.egg-info/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      512 2023-07-20 05:55:18.000000 tybase-0.2.0/tybase.egg-info/SOURCES.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)        1 2023-07-20 05:55:18.000000 tybase-0.2.0/tybase.egg-info/dependency_links.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)      135 2023-07-20 05:55:18.000000 tybase-0.2.0/tybase.egg-info/requires.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)        7 2023-07-20 05:55:18.000000 tybase-0.2.0/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:23:14.523706 tybase-0.2.2/
+-rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.2.2/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      793 2023-08-04 16:23:14.523475 tybase-0.2.2/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.2.2/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-08-04 16:23:14.523805 tybase-0.2.2/setup.cfg
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1082 2023-08-04 16:22:44.000000 tybase-0.2.2/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:23:14.511828 tybase-0.2.2/tybase/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.2.2/tybase/__init__.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:23:14.514661 tybase-0.2.2/tybase/baidu/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.2.2/tybase/baidu/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.2.2/tybase/baidu/kw_tool.py
+-rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.2.2/tybase/datatest.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:23:14.516517 tybase-0.2.2/tybase/dbtool/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.2.2/tybase/dbtool/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.2.2/tybase/dbtool/data_import.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.2.2/tybase/dbtool/mysql.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:23:14.517597 tybase-0.2.2/tybase/lc/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.2.2/tybase/lc/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.2.2/tybase/lc/eg1.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:23:14.522710 tybase-0.2.2/tybase/tools/
+-rw-r--r--   0 zhangte    (501) staff       (20)     2831 2023-08-04 15:56:07.000000 tybase-0.2.2/tybase/tools/Task.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.2.2/tybase/tools/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.2.2/tybase/tools/ali_oss_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     2626 2023-08-04 16:22:30.000000 tybase-0.2.2/tybase/tools/image_utils.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.2.2/tybase/tools/qiniu_tools.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.2.2/tybase/tools/riqit_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.2.2/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:23:14.513911 tybase-0.2.2/tybase.egg-info/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      793 2023-08-04 16:23:14.000000 tybase-0.2.2/tybase.egg-info/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      561 2023-08-04 16:23:14.000000 tybase-0.2.2/tybase.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-08-04 16:23:14.000000 tybase-0.2.2/tybase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      158 2023-08-04 16:23:14.000000 tybase-0.2.2/tybase.egg-info/requires.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-08-04 16:23:14.000000 tybase-0.2.2/tybase.egg-info/top_level.txt
```

### Comparing `tybase-0.2.0/setup.py` & `tybase-0.2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tybase',
-    version='0.2.0',
+    version='0.2.2',
     include_package_data=True,
-    description='新增了阿里oss的操作,需要单独安装库',
+    description='图片裁剪,Task异步任务(简单)',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',  # 版本描述
     author='Tuya',
     author_email='353335447@qq.com',
     url='https://github.com/yourusername/your_package',
     packages=find_packages(),
     install_requires=[
         'setuptools',
+        "opencv-python",
         "loguru",
+        "openpyxl",
         'requests',
         "python-dotenv",
         "retrying",
         "pymysql",
         "mysql-connector-python",
         "sqlalchemy",
         "pandas",
```

### Comparing `tybase-0.2.0/tybase/baidu/kw_tool.py` & `tybase-0.2.2/tybase/baidu/kw_tool.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.0/tybase/dbtool/data_import.py` & `tybase-0.2.2/tybase/dbtool/data_import.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.0/tybase/dbtool/mysql.py` & `tybase-0.2.2/tybase/dbtool/mysql.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.0/tybase/lc/eg1.py` & `tybase-0.2.2/tybase/lc/eg1.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.0/tybase/tools/ali_oss_tools.py` & `tybase-0.2.2/tybase/tools/ali_oss_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.0/tybase/tools/qiniu_tools.py` & `tybase-0.2.2/tybase/tools/qiniu_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.0/tybase/tools/riqit_tools.py` & `tybase-0.2.2/tybase/tools/riqit_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.0/tybase.egg-info/SOURCES.txt` & `tybase-0.2.2/tybase.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -12,11 +12,13 @@
 tybase/baidu/__init__.py
 tybase/baidu/kw_tool.py
 tybase/dbtool/__init__.py
 tybase/dbtool/data_import.py
 tybase/dbtool/mysql.py
 tybase/lc/__init__.py
 tybase/lc/eg1.py
+tybase/tools/Task.py
 tybase/tools/__init__.py
 tybase/tools/ali_oss_tools.py
+tybase/tools/image_utils.py
 tybase/tools/qiniu_tools.py
 tybase/tools/riqit_tools.py
```

