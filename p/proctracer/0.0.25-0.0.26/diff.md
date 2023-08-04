# Comparing `tmp/proctracer-0.0.25.tar.gz` & `tmp/proctracer-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proctracer-0.0.25.tar", last modified: Fri Aug  4 09:52:22 2023, max compression
+gzip compressed data, was "proctracer-0.0.26.tar", last modified: Fri Aug  4 15:19:48 2023, max compression
```

## Comparing `proctracer-0.0.25.tar` & `proctracer-0.0.26.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:52:22.061479 proctracer-0.0.25/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-04 09:52:07.000000 proctracer-0.0.25/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 09:52:07.000000 proctracer-0.0.25/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-04 09:52:22.061479 proctracer-0.0.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-04 09:52:07.000000 proctracer-0.0.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:52:22.057479 proctracer-0.0.25/proctracer/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:52:22.061479 proctracer-0.0.25/proctracer/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/net_dev.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/net_snmp_udp.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/net_udpX.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/pid_stat.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/plugin_proc_tracer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/pressure_X.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/stat.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/text_pipe.plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5322 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/proctracer.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:52:22.057479 proctracer-0.0.25/proctracer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-04 09:52:22.000000 proctracer-0.0.25/proctracer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-04 09:52:22.000000 proctracer-0.0.25/proctracer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:52:22.000000 proctracer-0.0.25/proctracer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 09:52:22.000000 proctracer-0.0.25/proctracer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-04 09:52:22.000000 proctracer-0.0.25/proctracer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 09:52:22.000000 proctracer-0.0.25/proctracer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-04 09:52:22.061479 proctracer-0.0.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-08-04 09:52:07.000000 proctracer-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:19:48.889909 proctracer-0.0.26/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-04 15:19:38.000000 proctracer-0.0.26/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 15:19:38.000000 proctracer-0.0.26/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-04 15:19:48.889909 proctracer-0.0.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-04 15:19:38.000000 proctracer-0.0.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:19:48.889909 proctracer-0.0.26/proctracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:19:48.889909 proctracer-0.0.26/proctracer/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/plugins/net_dev.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/plugins/net_snmp_udp.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5361 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/plugins/net_softnet_stat.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/plugins/net_udpX.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/plugins/pid_stat.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/plugins/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/plugins/plugin_proc_tracer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/plugins/pressure_X.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/plugins/stat.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/plugins/text_pipe.plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5385 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/proctracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-04 15:19:38.000000 proctracer-0.0.26/proctracer/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:19:48.889909 proctracer-0.0.26/proctracer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-04 15:19:48.000000 proctracer-0.0.26/proctracer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-08-04 15:19:48.000000 proctracer-0.0.26/proctracer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:19:48.000000 proctracer-0.0.26/proctracer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 15:19:48.000000 proctracer-0.0.26/proctracer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-04 15:19:48.000000 proctracer-0.0.26/proctracer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 15:19:48.000000 proctracer-0.0.26/proctracer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-04 15:19:48.889909 proctracer-0.0.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-08-04 15:19:38.000000 proctracer-0.0.26/setup.py
```

### Comparing `proctracer-0.0.25/LICENSE.md` & `proctracer-0.0.26/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.25/PKG-INFO` & `proctracer-0.0.26/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.25
+Version: 0.0.26
 Summary: /proc Tracer
 Home-page: https://github.com/david-kracht/proctracer
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.25/README.md` & `proctracer-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.25/proctracer/plugins/__init__.py` & `proctracer-0.0.26/proctracer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.25/proctracer/plugins/net_dev.plugin.py` & `proctracer-0.0.26/proctracer/plugins/net_dev.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.25/proctracer/plugins/net_snmp_udp.plugin.py` & `proctracer-0.0.26/proctracer/plugins/net_snmp_udp.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.25/proctracer/plugins/net_udpX.plugin.py` & `proctracer-0.0.26/proctracer/plugins/net_udpX.plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
         kernel_parameter={'/proc/sys/net/ipv4/udp_mem': "N/A",    
                 '/proc/sys/net/ipv4/udp_rmem_min': "N/A",
                 '/proc/sys/net/ipv4/udp_wmem_min': "N/A",
                 '/proc/sys/net/core/rmem_default': "N/A",
                 '/proc/sys/net/core/rmem_max': "N/A",
                 '/proc/sys/net/core/wmem_default': "N/A",
                 '/proc/sys/net/core/wmem_max': "N/A",
+                '/proc/sys/net/core/netdev_max_backlog': "N/A",
                 }
         
         kernel_parameter_note=""
         for k,_ in kernel_parameter.items():
             result = self.proc_reader(k)
             if result:
                 kernel_parameter[k] = ' '.join(result.split())
```

### Comparing `proctracer-0.0.25/proctracer/plugins/pid_stat.plugin.py` & `proctracer-0.0.26/proctracer/plugins/pid_stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.25/proctracer/plugins/plugin_base.py` & `proctracer-0.0.26/proctracer/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.25/proctracer/plugins/plugin_proc_tracer_base.py` & `proctracer-0.0.26/proctracer/plugins/plugin_proc_tracer_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import copy
 
 import pandas as pd
 from matplotlib.backends.backend_pdf import PdfPages
 
 from plugin_base import PluginBase
 
+MAX_PROC_READ_RETRY=5
+
 class ProcTracerBase(PluginBase):
 
     t0=time.time()
 
     @classmethod
     def t(cls):
         return time.time()-cls.t0
@@ -57,14 +59,15 @@
 
     def proc_reader(self, file):
         result=""
 
         if file not in self.proc_fds:
             try:
                 self.proc_fds[file] = open(file, 'r')
+                self.retry_read_counter = MAX_PROC_READ_RETRY
             except FileNotFoundError:
                 self.retry_read_counter -= 1
                 time.sleep(1)
                 
                 if self.retry_read_counter == 0:
                     self.thread["pill2kill"].set()
                     self.file = "Not available: %s" % self.file
```

### Comparing `proctracer-0.0.25/proctracer/plugins/pressure_X.plugin.py` & `proctracer-0.0.26/proctracer/plugins/pressure_X.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.25/proctracer/plugins/stat.plugin.py` & `proctracer-0.0.26/proctracer/plugins/stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.25/proctracer/plugins/text_pipe.plugin.py` & `proctracer-0.0.26/proctracer/plugins/text_pipe.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.25/proctracer/proctracer.py` & `proctracer-0.0.26/proctracer/proctracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,17 @@
         period: 5.0
     net_dev:
         active: true
         period: 1.0
     net_snmp_udp:
         active: true
         period: 0.2
+    net_softnet_stat:
+        active: true
+        period: 0.2
     net_udp4:
         active: true
         period: 0.2
     net_udp6:
         active: false
         period: 0.2
 """
```

### Comparing `proctracer-0.0.25/proctracer.egg-info/PKG-INFO` & `proctracer-0.0.26/proctracer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.25
+Version: 0.0.26
 Summary: /proc Tracer
 Home-page: https://github.com/david-kracht/proctracer
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.25/proctracer.egg-info/SOURCES.txt` & `proctracer-0.0.26/proctracer.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 proctracer.egg-info/dependency_links.txt
 proctracer.egg-info/entry_points.txt
 proctracer.egg-info/requires.txt
 proctracer.egg-info/top_level.txt
 proctracer/plugins/__init__.py
 proctracer/plugins/net_dev.plugin.py
 proctracer/plugins/net_snmp_udp.plugin.py
+proctracer/plugins/net_softnet_stat.plugin.py
 proctracer/plugins/net_udpX.plugin.py
 proctracer/plugins/pid_stat.plugin.py
 proctracer/plugins/plugin_base.py
 proctracer/plugins/plugin_proc_tracer_base.py
 proctracer/plugins/pressure_X.plugin.py
 proctracer/plugins/stat.plugin.py
 proctracer/plugins/text_pipe.plugin.py
```

### Comparing `proctracer-0.0.25/setup.py` & `proctracer-0.0.26/setup.py`

 * *Files identical despite different names*

