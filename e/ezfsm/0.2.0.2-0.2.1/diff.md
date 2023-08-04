# Comparing `tmp/ezfsm-0.2.0.2.tar.gz` & `tmp/ezfsm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ezfsm-0.2.0.2.tar", last modified: Wed Dec  1 04:15:04 2021, max compression
+gzip compressed data, was "ezfsm-0.2.1.tar", last modified: Fri Aug  4 13:16:14 2023, max compression
```

## Comparing `ezfsm-0.2.0.2.tar` & `ezfsm-0.2.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2021-12-01 04:15:04.000000 ezfsm-0.2.0.2/
--rw-rw-rw-   0        0        0      460 2021-12-01 04:15:04.000000 ezfsm-0.2.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2021-12-01 04:15:04.000000 ezfsm-0.2.0.2/ezfsm/
--rw-rw-rw-   0        0        0      366 2021-11-11 15:18:50.000000 ezfsm-0.2.0.2/ezfsm/DataArea.py
--rw-rw-rw-   0        0        0    22224 2021-12-01 02:47:13.000000 ezfsm-0.2.0.2/ezfsm/StateMachine.py
--rw-rw-rw-   0        0        0       29 2021-11-11 15:18:50.000000 ezfsm-0.2.0.2/ezfsm/StateNode.py
--rw-rw-rw-   0        0        0     1243 2021-11-11 15:18:50.000000 ezfsm-0.2.0.2/ezfsm/StateSet.py
--rw-rw-rw-   0        0        0     5816 2021-12-01 04:14:10.000000 ezfsm-0.2.0.2/ezfsm/TimingSeriesFunction.py
--rw-rw-rw-   0        0        0     4574 2021-11-11 15:18:50.000000 ezfsm-0.2.0.2/ezfsm/TransFunction.py
--rw-rw-rw-   0        0        0     1096 2021-12-01 02:53:16.000000 ezfsm-0.2.0.2/ezfsm/__init__.py
--rw-rw-rw-   0        0        0      751 2021-12-01 02:44:36.000000 ezfsm-0.2.0.2/ezfsm/unit_test.py
--rw-rw-rw-   0        0        0     4782 2021-11-11 15:18:50.000000 ezfsm-0.2.0.2/ezfsm/vessel.py
-drwxrwxrwx   0        0        0        0 2021-12-01 04:15:04.000000 ezfsm-0.2.0.2/ezfsm.egg-info/
--rw-rw-rw-   0        0        0      460 2021-12-01 04:15:04.000000 ezfsm-0.2.0.2/ezfsm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2021-12-01 04:15:04.000000 ezfsm-0.2.0.2/ezfsm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-01 04:15:04.000000 ezfsm-0.2.0.2/ezfsm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2021-12-01 04:15:04.000000 ezfsm-0.2.0.2/ezfsm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2021-12-01 04:15:04.000000 ezfsm-0.2.0.2/ezfsm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-12-01 04:15:04.000000 ezfsm-0.2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      616 2021-12-01 04:14:56.000000 ezfsm-0.2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:16:14.490907 ezfsm-0.2.1/
+-rw-rw-rw-   0        0        0    20161 2023-08-04 13:16:14.489899 ezfsm-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-04 13:16:14.459913 ezfsm-0.2.1/ezfsm/
+-rw-rw-rw-   0        0        0      366 2023-07-30 06:24:30.000000 ezfsm-0.2.1/ezfsm/DataArea.py
+-rw-rw-rw-   0        0        0    22334 2023-08-04 13:08:49.000000 ezfsm-0.2.1/ezfsm/StateMachine.py
+-rw-rw-rw-   0        0        0       29 2023-07-30 06:24:30.000000 ezfsm-0.2.1/ezfsm/StateNode.py
+-rw-rw-rw-   0        0        0     1243 2023-07-30 06:24:30.000000 ezfsm-0.2.1/ezfsm/StateSet.py
+-rw-rw-rw-   0        0        0     5816 2023-07-30 06:24:30.000000 ezfsm-0.2.1/ezfsm/TimingSeriesFunction.py
+-rw-rw-rw-   0        0        0     4574 2023-07-30 06:24:30.000000 ezfsm-0.2.1/ezfsm/TransFunction.py
+-rw-rw-rw-   0        0        0     1096 2023-07-30 06:24:30.000000 ezfsm-0.2.1/ezfsm/__init__.py
+-rw-rw-rw-   0        0        0      751 2023-07-30 06:24:30.000000 ezfsm-0.2.1/ezfsm/unit_test.py
+-rw-rw-rw-   0        0        0     4782 2023-07-30 06:24:30.000000 ezfsm-0.2.1/ezfsm/vessel.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:16:14.484901 ezfsm-0.2.1/ezfsm.egg-info/
+-rw-rw-rw-   0        0        0    20161 2023-08-04 13:16:14.000000 ezfsm-0.2.1/ezfsm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      307 2023-08-04 13:16:14.000000 ezfsm-0.2.1/ezfsm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 13:16:14.000000 ezfsm-0.2.1/ezfsm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-04 13:16:14.000000 ezfsm-0.2.1/ezfsm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 13:16:14.491897 ezfsm-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      798 2023-08-04 13:15:52.000000 ezfsm-0.2.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ezfsm-0.2.0.2/ezfsm/StateMachine.py` & `ezfsm-0.2.1/ezfsm/StateMachine.py`

 * *Files 0% similar despite different names*

```diff
@@ -405,14 +405,18 @@
                             added_flag = True
 
                 if not added_flag:  # 在排序中没有添加此项，那么应当在末尾添加此项
                     self.st[srt] += [(srt, dst, tf)]
 
 
 
+        # 移除重复项
+        for sta in self.st:
+            self.st[sta] = list(set(self.st[sta]))
+
         # Build完成
         self.ready = self.READY
 
         self.ResetAreas()  # 重置各级运行环境
 
 
 class StateMachine(StateMachine_cb, StateMachine_area, StateMachine_data):  # 状态机
```

### Comparing `ezfsm-0.2.0.2/ezfsm/StateSet.py` & `ezfsm-0.2.1/ezfsm/StateSet.py`

 * *Files identical despite different names*

### Comparing `ezfsm-0.2.0.2/ezfsm/TimingSeriesFunction.py` & `ezfsm-0.2.1/ezfsm/TimingSeriesFunction.py`

 * *Files identical despite different names*

### Comparing `ezfsm-0.2.0.2/ezfsm/TransFunction.py` & `ezfsm-0.2.1/ezfsm/TransFunction.py`

 * *Files identical despite different names*

### Comparing `ezfsm-0.2.0.2/ezfsm/__init__.py` & `ezfsm-0.2.1/ezfsm/__init__.py`

 * *Files identical despite different names*

### Comparing `ezfsm-0.2.0.2/ezfsm/unit_test.py` & `ezfsm-0.2.1/ezfsm/unit_test.py`

 * *Files identical despite different names*

### Comparing `ezfsm-0.2.0.2/ezfsm/vessel.py` & `ezfsm-0.2.1/ezfsm/vessel.py`

 * *Files identical despite different names*

