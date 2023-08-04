# Comparing `tmp/huhk-1.9.7.tar.gz` & `tmp/huhk-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huhk-1.9.7.tar", last modified: Fri Aug  4 06:33:09 2023, max compression
+gzip compressed data, was "huhk-1.9.8.tar", last modified: Fri Aug  4 06:49:08 2023, max compression
```

## Comparing `huhk-1.9.7.tar` & `huhk-1.9.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 06:33:09.486734 huhk-1.9.7/
--rw-rw-rw-   0        0        0      223 2023-08-04 06:33:09.485739 huhk-1.9.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-04 06:33:09.383516 huhk-1.9.7/huhk/
--rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.9.7/huhk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 06:33:09.425403 huhk-1.9.7/huhk/case_project/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/case_project/__init__.py
--rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/case_project/json_coder.py
--rw-rw-rw-   0        0        0     3253 2023-08-04 01:52:31.000000 huhk-1.9.7/huhk/case_project/main_fun.py
--rw-rw-rw-   0        0        0    21477 2023-08-04 01:53:28.000000 huhk-1.9.7/huhk/case_project/project_base.py
--rw-rw-rw-   0        0        0     1359 2023-08-04 01:36:40.000000 huhk-1.9.7/huhk/case_project/project_init.py
--rw-rw-rw-   0        0        0    18564 2023-08-04 01:53:28.000000 huhk-1.9.7/huhk/case_project/project_string.py
--rw-rw-rw-   0        0        0     1110 2023-08-04 02:28:29.000000 huhk-1.9.7/huhk/case_project/setup_set.py
--rw-rw-rw-   0        0        0       17 2023-08-04 06:33:08.000000 huhk-1.9.7/huhk/case_project/version.py
--rw-rw-rw-   0        0        0     9864 2023-08-04 01:53:28.000000 huhk-1.9.7/huhk/init_project.py
--rw-rw-rw-   0        0        0     1277 2023-08-04 01:51:34.000000 huhk-1.9.7/huhk/main.py
--rw-rw-rw-   0        0        0      338 2023-08-04 06:33:00.000000 huhk-1.9.7/huhk/setup_run.py
-drwxrwxrwx   0        0        0        0 2023-08-04 06:33:09.428395 huhk-1.9.7/huhk/testcase/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/testcase/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 06:33:09.479752 huhk-1.9.7/huhk/testcase/apache/
--rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/testcase/apache/__init__.py
--rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/testcase/apache/beam_class.py
--rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.9.7/huhk/testcase/apache/data.py
--rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/testcase/apache/par_do.py
--rw-rw-rw-   0        0        0     7252 2023-08-04 01:32:03.000000 huhk-1.9.7/huhk/testcase/apache/test_cogroupbykey.py
--rw-rw-rw-   0        0        0      471 2023-08-04 01:32:02.000000 huhk-1.9.7/huhk/testcase/apache/test_file.py
--rw-rw-rw-   0        0        0     1498 2023-08-04 01:32:02.000000 huhk-1.9.7/huhk/testcase/apache/test_fiter.py
--rw-rw-rw-   0        0        0     2098 2023-08-04 01:32:03.000000 huhk-1.9.7/huhk/testcase/apache/test_flatmap.py
--rw-rw-rw-   0        0        0      518 2023-08-04 01:32:03.000000 huhk-1.9.7/huhk/testcase/apache/test_map.py
--rw-rw-rw-   0        0        0     2627 2023-08-04 01:32:02.000000 huhk-1.9.7/huhk/testcase/apache/test_par_do.py
--rw-rw-rw-   0        0        0     1646 2023-08-04 01:32:03.000000 huhk-1.9.7/huhk/testcase/apache/test_regex.py
--rw-rw-rw-   0        0        0     1566 2023-08-04 01:32:02.000000 huhk-1.9.7/huhk/testcase/apache/test_time.py
--rw-rw-rw-   0        0        0      503 2023-08-04 01:32:03.000000 huhk-1.9.7/huhk/testcase/apache/test_to_string.py
--rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.9.7/huhk/unit_apache_beam.py
--rw-rw-rw-   0        0        0      352 2023-07-31 09:35:09.000000 huhk-1.9.7/huhk/unit_data.py
--rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/unit_dict.py
--rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/unit_encryption.py
--rw-rw-rw-   0        0        0    29677 2023-08-04 02:08:02.000000 huhk-1.9.7/huhk/unit_fun.py
--rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/unit_logger.py
--rw-rw-rw-   0        0        0    10048 2023-08-04 01:36:40.000000 huhk-1.9.7/huhk/unit_request.py
--rw-rw-rw-   0        0        0     2591 2023-08-04 05:24:53.000000 huhk-1.9.7/huhk/unit_tasks.py
--rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.9.7/huhk/常用命令.py
-drwxrwxrwx   0        0        0        0 2023-08-04 06:33:09.399501 huhk-1.9.7/huhk.egg-info/
--rw-rw-rw-   0        0        0      223 2023-08-04 06:33:09.000000 huhk-1.9.7/huhk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1156 2023-08-04 06:33:09.000000 huhk-1.9.7/huhk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 06:33:09.000000 huhk-1.9.7/huhk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-08-04 06:33:09.000000 huhk-1.9.7/huhk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      134 2023-08-04 06:33:09.000000 huhk-1.9.7/huhk.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-04 06:33:09.000000 huhk-1.9.7/huhk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 06:33:09.486734 huhk-1.9.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 06:49:08.259422 huhk-1.9.8/
+-rw-rw-rw-   0        0        0      223 2023-08-04 06:49:08.259422 huhk-1.9.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-04 06:49:08.192942 huhk-1.9.8/huhk/
+-rw-rw-rw-   0        0        0      772 2023-07-17 02:44:39.000000 huhk-1.9.8/huhk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:49:08.223971 huhk-1.9.8/huhk/case_project/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.8/huhk/case_project/__init__.py
+-rw-rw-rw-   0        0        0      639 2023-07-12 01:13:24.000000 huhk-1.9.8/huhk/case_project/json_coder.py
+-rw-rw-rw-   0        0        0     3253 2023-08-04 01:52:31.000000 huhk-1.9.8/huhk/case_project/main_fun.py
+-rw-rw-rw-   0        0        0    21492 2023-08-04 06:46:35.000000 huhk-1.9.8/huhk/case_project/project_base.py
+-rw-rw-rw-   0        0        0     1369 2023-08-04 06:46:35.000000 huhk-1.9.8/huhk/case_project/project_init.py
+-rw-rw-rw-   0        0        0    18569 2023-08-04 06:46:35.000000 huhk-1.9.8/huhk/case_project/project_string.py
+-rw-rw-rw-   0        0        0     1115 2023-08-04 06:46:35.000000 huhk-1.9.8/huhk/case_project/setup_set.py
+-rw-rw-rw-   0        0        0       17 2023-08-04 06:49:07.000000 huhk-1.9.8/huhk/case_project/version.py
+-rw-rw-rw-   0        0        0     9874 2023-08-04 06:46:35.000000 huhk-1.9.8/huhk/init_project.py
+-rw-rw-rw-   0        0        0     1277 2023-08-04 01:51:34.000000 huhk-1.9.8/huhk/main.py
+-rw-rw-rw-   0        0        0      338 2023-08-04 06:33:00.000000 huhk-1.9.8/huhk/setup_run.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:49:08.225509 huhk-1.9.8/huhk/testcase/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.8/huhk/testcase/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:49:08.257425 huhk-1.9.8/huhk/testcase/apache/
+-rw-rw-rw-   0        0        0        0 2023-07-12 01:13:24.000000 huhk-1.9.8/huhk/testcase/apache/__init__.py
+-rw-rw-rw-   0        0        0     3355 2023-07-12 01:13:24.000000 huhk-1.9.8/huhk/testcase/apache/beam_class.py
+-rw-rw-rw-   0        0        0     5523 2023-07-12 02:37:05.000000 huhk-1.9.8/huhk/testcase/apache/data.py
+-rw-rw-rw-   0        0        0     1764 2023-07-12 01:13:24.000000 huhk-1.9.8/huhk/testcase/apache/par_do.py
+-rw-rw-rw-   0        0        0     7257 2023-08-04 06:46:35.000000 huhk-1.9.8/huhk/testcase/apache/test_cogroupbykey.py
+-rw-rw-rw-   0        0        0      476 2023-08-04 06:46:35.000000 huhk-1.9.8/huhk/testcase/apache/test_file.py
+-rw-rw-rw-   0        0        0     1503 2023-08-04 06:46:35.000000 huhk-1.9.8/huhk/testcase/apache/test_fiter.py
+-rw-rw-rw-   0        0        0     2103 2023-08-04 06:46:35.000000 huhk-1.9.8/huhk/testcase/apache/test_flatmap.py
+-rw-rw-rw-   0        0        0      607 2023-08-04 06:46:35.000000 huhk-1.9.8/huhk/testcase/apache/test_map.py
+-rw-rw-rw-   0        0        0     2717 2023-08-04 06:48:16.000000 huhk-1.9.8/huhk/testcase/apache/test_par_do.py
+-rw-rw-rw-   0        0        0     1734 2023-08-04 06:48:23.000000 huhk-1.9.8/huhk/testcase/apache/test_regex.py
+-rw-rw-rw-   0        0        0     1639 2023-08-04 06:47:50.000000 huhk-1.9.8/huhk/testcase/apache/test_time.py
+-rw-rw-rw-   0        0        0      508 2023-08-04 06:47:50.000000 huhk-1.9.8/huhk/testcase/apache/test_to_string.py
+-rw-rw-rw-   0        0        0    22615 2023-07-14 06:52:17.000000 huhk-1.9.8/huhk/unit_apache_beam.py
+-rw-rw-rw-   0        0        0      352 2023-07-31 09:35:09.000000 huhk-1.9.8/huhk/unit_data.py
+-rw-rw-rw-   0        0        0     4508 2023-07-12 01:13:24.000000 huhk-1.9.8/huhk/unit_dict.py
+-rw-rw-rw-   0        0        0     3843 2023-07-12 01:13:24.000000 huhk-1.9.8/huhk/unit_encryption.py
+-rw-rw-rw-   0        0        0    29692 2023-08-04 06:47:05.000000 huhk-1.9.8/huhk/unit_fun.py
+-rw-rw-rw-   0        0        0     1242 2023-07-12 01:13:24.000000 huhk-1.9.8/huhk/unit_logger.py
+-rw-rw-rw-   0        0        0    10063 2023-08-04 06:47:50.000000 huhk-1.9.8/huhk/unit_request.py
+-rw-rw-rw-   0        0        0     2591 2023-08-04 05:24:53.000000 huhk-1.9.8/huhk/unit_tasks.py
+-rw-rw-rw-   0        0        0      733 2023-07-12 01:13:24.000000 huhk-1.9.8/huhk/常用命令.py
+drwxrwxrwx   0        0        0        0 2023-08-04 06:49:08.204908 huhk-1.9.8/huhk.egg-info/
+-rw-rw-rw-   0        0        0      223 2023-08-04 06:49:08.000000 huhk-1.9.8/huhk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1156 2023-08-04 06:49:08.000000 huhk-1.9.8/huhk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 06:49:08.000000 huhk-1.9.8/huhk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-08-04 06:49:08.000000 huhk-1.9.8/huhk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      134 2023-08-04 06:49:08.000000 huhk-1.9.8/huhk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-04 06:49:08.000000 huhk-1.9.8/huhk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 06:49:08.260418 huhk-1.9.8/setup.cfg
```

### Comparing `huhk-1.9.7/huhk/__init__.py` & `huhk-1.9.8/huhk/__init__.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.7/huhk/case_project/json_coder.py` & `huhk-1.9.8/huhk/case_project/json_coder.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.7/huhk/case_project/main_fun.py` & `huhk-1.9.8/huhk/case_project/main_fun.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.7/huhk/case_project/project_base.py` & `huhk-1.9.8/huhk/case_project/project_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import os.path
 import re
 import time
 
 import requests
 
 from huhk.case_project.project_string import ProjectString
-from unit_dict import Dict
-from unit_fun import FunBase
+from huhk.unit_dict import Dict
+from huhk.unit_fun import FunBase
 from huhk import projects_path
-from unit_logger import logger
+from huhk.unit_logger import logger
 
 
 class ProjectBase(ProjectString):
     def __init__(self, name=None, app_key=None, yapi_url=None, yapi_token=None, yapi_json_file=None, swagger_url=None):
         super().__init__(name, app_key, yapi_url, yapi_token, yapi_json_file, swagger_url)
         self.get_project()
```

### Comparing `huhk-1.9.7/huhk/case_project/project_init.py` & `huhk-1.9.8/huhk/case_project/project_init.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from huhk import projects_path, admin_host
-from unit_dict import Dict
-from unit_data import size_names, page_names, before_names, end_names, page_and_size
+from huhk.unit_dict import Dict
+from huhk.unit_data import size_names, page_names, before_names, end_names, page_and_size
 
 
 class ProjectInIt:
     def __init__(self, name=None, app_key=None, yapi_url=None, yapi_token=None, yapi_json_file=None, swagger_url=None):
         """api_type: 0时，value是swagger的api，json的url
                      1时，value值为yapi项目token,
                      2时，value是yapi下载的json文件名，文件放在file目录下,
```

### Comparing `huhk-1.9.7/huhk/case_project/project_string.py` & `huhk-1.9.8/huhk/case_project/project_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 import re
 
 import requests
 
 from huhk.case_project.project_init import ProjectInIt
-from unit_dict import Dict
+from huhk.unit_dict import Dict
 
 
 class ProjectString(ProjectInIt):
     def _get_description(self, req_body_other):
         try:
             if not req_body_other:
                 return []
```

### Comparing `huhk-1.9.7/huhk/case_project/setup_set.py` & `huhk-1.9.8/huhk/case_project/setup_set.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-from unit_fun import FunBase
+from huhk.unit_fun import FunBase
 
 
 def find_data_files(directory):
     pass
 
 
 setup(
```

### Comparing `huhk-1.9.7/huhk/init_project.py` & `huhk-1.9.8/huhk/init_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os.path
 import re
 
 from huhk.case_project.project_base import ProjectBase
-from unit_dict import Dict
-from unit_fun import FunBase
+from huhk.unit_dict import Dict
+from huhk.unit_fun import FunBase
 from huhk import projects_path
 
 
 class GetApi(ProjectBase):
     def __init__(self, name=None, app_key=None, yapi_url=None, yapi_token=None, yapi_json_file=None, swagger_url=None):
         """
         """
```

### Comparing `huhk-1.9.7/huhk/main.py` & `huhk-1.9.8/huhk/main.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.7/huhk/testcase/apache/beam_class.py` & `huhk-1.9.8/huhk/testcase/apache/beam_class.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.7/huhk/testcase/apache/data.py` & `huhk-1.9.8/huhk/testcase/apache/data.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.7/huhk/testcase/apache/par_do.py` & `huhk-1.9.8/huhk/testcase/apache/par_do.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.7/huhk/testcase/apache/test_cogroupbykey.py` & `huhk-1.9.8/huhk/testcase/apache/test_cogroupbykey.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from testcase.apache.beam_class import AverageFn, AverageFn2
-from unit_apache_beam import ApacheFun
+from huhk.unit_apache_beam import ApacheFun
 
 
 class TestPolymerization:
     # 通过键聚合所有输入元素，并允许下游处理使用与键关联的所有值
     def test_polymerization_001(self):
         ApacheFun(data_type=data_type).co_group_by_key(icons=data_list_tuple3, durations=data_list_tuple4).print()
```

### Comparing `huhk-1.9.7/huhk/testcase/apache/test_fiter.py` & `huhk-1.9.8/huhk/testcase/apache/test_fiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from unit_apache_beam import ApacheFun
+from huhk.unit_apache_beam import ApacheFun
 
 
 class TestFiter:
     def setup(self):
         self.af = ApacheFun(data_list_dict, data_type=data_type)
 
     # 使用函数过滤
```

### Comparing `huhk-1.9.7/huhk/testcase/apache/test_flatmap.py` & `huhk-1.9.8/huhk/testcase/apache/test_flatmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from unit_apache_beam import ApacheFun
+from huhk.unit_apache_beam import ApacheFun
 
 
 class TestFlatmap:
     def setup(self):
         self.af = ApacheFun(data_list_str, data_type=data_type)
 
     # 带有预定义函数的 FlatMap
```

### Comparing `huhk-1.9.7/huhk/testcase/apache/test_map.py` & `huhk-1.9.8/huhk/testcase/apache/test_map.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from unit_apache_beam import ApacheFun
+from huhk.testcase.apache.data import data_list_str3, data_type, data_list_tuple
+
+from huhk.unit_apache_beam import ApacheFun
 
 
 class TestMap:
     # 带有预定义函数的 FlatMap
     def test_map_001(self):
         ApacheFun(data_list_str3, data_type=data_type).map(str.strip).print()
```

### Comparing `huhk-1.9.7/huhk/testcase/apache/test_par_do.py` & `huhk-1.9.8/huhk/testcase/apache/test_par_do.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import random
-from unit_apache_beam import ApacheFun
+
+from huhk.testcase.apache.data import data_list_str2, data_type, data_list_dict
+
+from huhk.unit_apache_beam import ApacheFun
 from testcase.apache.beam_class import SplitWords, AnalyzeElement, DoFnMethods
 
 
 class TestParDo:
     # 有简单 DoFn 的 ParDo
     def test_par_do_001(self):
         ApacheFun(data_list_str2, data_type=data_type).par_do(SplitWords(',')).print()
```

### Comparing `huhk-1.9.7/huhk/testcase/apache/test_regex.py` & `huhk-1.9.8/huhk/testcase/apache/test_regex.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from unit_apache_beam import ApacheFun
+from huhk.testcase.apache.data import data_list_str4, data_type, data_list_str5
+
+from huhk.unit_apache_beam import ApacheFun
 
 
 class TestRegex:
     # 正则表达式匹配
     def test_regex_001(self):
         ApacheFun(data_list_str4, data_type=data_type).regex_matches(r'(?P<icon>[^\s,]+), *(\w+), *(\w+)').print()
```

### Comparing `huhk-1.9.7/huhk/testcase/apache/test_time.py` & `huhk-1.9.8/huhk/testcase/apache/test_time.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from unit_apache_beam import ApacheFun
+from huhk.testcase.apache.data import data_list_dict3, data_type
+
+from huhk.unit_apache_beam import ApacheFun
 
 
 class TestTimes:
     # 按事件时间标记时间戳
     def test_times_001(self):
         ApacheFun(data_list_dict3, data_type=data_type).timestamped_value("season").print()
```

### Comparing `huhk-1.9.7/huhk/unit_apache_beam.py` & `huhk-1.9.8/huhk/unit_apache_beam.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.7/huhk/unit_dict.py` & `huhk-1.9.8/huhk/unit_dict.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.7/huhk/unit_encryption.py` & `huhk-1.9.8/huhk/unit_encryption.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.7/huhk/unit_fun.py` & `huhk-1.9.8/huhk/unit_fun.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 import time
 import requests
 import datetime
 from pandas import DataFrame, ExcelWriter
 from typing import List
 from faker import Faker
 
-from unit_dict import Dict
-from unit_logger import logger
-from unit_data import page_and_size, before_and_end_re_str
+from huhk.unit_dict import Dict
+from huhk.unit_logger import logger
+from huhk.unit_data import page_and_size, before_and_end_re_str
 
 
 class FunBase:
     def __init__(self):
         self._time2 = 0
         self._time1 = 0
         self.sql_str = ""
```

### Comparing `huhk-1.9.7/huhk/unit_logger.py` & `huhk-1.9.8/huhk/unit_logger.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.7/huhk/unit_request.py` & `huhk-1.9.8/huhk/unit_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import requests
 import json
 import time
 import urllib
 import os
 import hashlib
 
-from unit_fun import FunBase
+from huhk.unit_fun import FunBase
 from requests import ReadTimeout, ConnectTimeout
 from requests.exceptions import MissingSchema
 from urllib.parse import urlencode
-from unit_dict import Dict
-from unit_logger import logger
+from huhk.unit_dict import Dict
+from huhk.unit_logger import logger
 from openpyxl.reader.excel import load_workbook
 from huhk import admin_host, projects_path
 
 
 class UnitRequest:
     def __init__(self, ZEST_ENV=None, APP_KEY=None, TIMEOUT=30000):
         self.ZEST_ENV = ZEST_ENV
```

### Comparing `huhk-1.9.7/huhk/unit_tasks.py` & `huhk-1.9.8/huhk/unit_tasks.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.7/huhk/常用命令.py` & `huhk-1.9.8/huhk/常用命令.py`

 * *Files identical despite different names*

### Comparing `huhk-1.9.7/huhk.egg-info/SOURCES.txt` & `huhk-1.9.8/huhk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

