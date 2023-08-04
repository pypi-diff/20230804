# Comparing `tmp/proctracer-0.0.23.tar.gz` & `tmp/proctracer-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proctracer-0.0.23.tar", last modified: Fri Jul 28 11:09:25 2023, max compression
+gzip compressed data, was "proctracer-0.0.25.tar", last modified: Fri Aug  4 09:52:22 2023, max compression
```

## Comparing `proctracer-0.0.23.tar` & `proctracer-0.0.25.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:09:25.930890 proctracer-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-28 11:09:16.000000 proctracer-0.0.23/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-28 11:09:16.000000 proctracer-0.0.23/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-28 11:09:25.930890 proctracer-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-28 11:09:16.000000 proctracer-0.0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:09:25.926890 proctracer-0.0.23/proctracer/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:09:25.930890 proctracer-0.0.23/proctracer/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/net_dev.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/net_snmp_udp.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/net_udpX.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/pid_stat.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/plugin_proc_tracer_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/pressure_X.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/stat.plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/plugins/text_pipe.plugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5153 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/proctracer.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-28 11:09:16.000000 proctracer-0.0.23/proctracer/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 11:09:25.926890 proctracer-0.0.23/proctracer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-28 11:09:25.000000 proctracer-0.0.23/proctracer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-28 11:09:25.000000 proctracer-0.0.23/proctracer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 11:09:25.000000 proctracer-0.0.23/proctracer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-28 11:09:25.000000 proctracer-0.0.23/proctracer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-28 11:09:25.000000 proctracer-0.0.23/proctracer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-28 11:09:25.000000 proctracer-0.0.23/proctracer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-28 11:09:25.930890 proctracer-0.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-07-28 11:09:16.000000 proctracer-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:52:22.061479 proctracer-0.0.25/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-04 09:52:07.000000 proctracer-0.0.25/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 09:52:07.000000 proctracer-0.0.25/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-04 09:52:22.061479 proctracer-0.0.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-08-04 09:52:07.000000 proctracer-0.0.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:52:22.057479 proctracer-0.0.25/proctracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:52:22.061479 proctracer-0.0.25/proctracer/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/net_dev.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/net_snmp_udp.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/net_udpX.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/pid_stat.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/plugin_proc_tracer_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/pressure_X.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/stat.plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/plugins/text_pipe.plugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5322 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/proctracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-04 09:52:07.000000 proctracer-0.0.25/proctracer/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:52:22.057479 proctracer-0.0.25/proctracer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-08-04 09:52:22.000000 proctracer-0.0.25/proctracer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-08-04 09:52:22.000000 proctracer-0.0.25/proctracer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:52:22.000000 proctracer-0.0.25/proctracer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-04 09:52:22.000000 proctracer-0.0.25/proctracer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-04 09:52:22.000000 proctracer-0.0.25/proctracer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-04 09:52:22.000000 proctracer-0.0.25/proctracer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-04 09:52:22.061479 proctracer-0.0.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4895 2023-08-04 09:52:07.000000 proctracer-0.0.25/setup.py
```

### Comparing `proctracer-0.0.23/LICENSE.md` & `proctracer-0.0.25/LICENSE.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.23/PKG-INFO` & `proctracer-0.0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.23
+Version: 0.0.25
 Summary: /proc Tracer
 Home-page: https://github.com/david-kracht/proctracer
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.23/README.md` & `proctracer-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.23/proctracer/plugins/__init__.py` & `proctracer-0.0.25/proctracer/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.23/proctracer/plugins/net_dev.plugin.py` & `proctracer-0.0.25/proctracer/plugins/net_dev.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.23/proctracer/plugins/net_snmp_udp.plugin.py` & `proctracer-0.0.25/proctracer/plugins/net_snmp_udp.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.23/proctracer/plugins/net_udpX.plugin.py` & `proctracer-0.0.25/proctracer/plugins/net_udpX.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.23/proctracer/plugins/pid_stat.plugin.py` & `proctracer-0.0.25/proctracer/plugins/pid_stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.23/proctracer/plugins/plugin_base.py` & `proctracer-0.0.25/proctracer/plugins/plugin_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.23/proctracer/plugins/plugin_proc_tracer_base.py` & `proctracer-0.0.25/proctracer/plugins/plugin_proc_tracer_base.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.23/proctracer/plugins/pressure_X.plugin.py` & `proctracer-0.0.25/proctracer/plugins/pressure_X.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.23/proctracer/plugins/stat.plugin.py` & `proctracer-0.0.25/proctracer/plugins/stat.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.23/proctracer/plugins/text_pipe.plugin.py` & `proctracer-0.0.25/proctracer/plugins/text_pipe.plugin.py`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.23/proctracer/proctracer.py` & `proctracer-0.0.25/proctracer/proctracer.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,14 +92,17 @@
 
     parser.add_argument('-c', '--config', type=str, required=False, default=DEFAULT_CONFIG_YAML_PATH , help='Path to /proc Tracer config yaml.')
     parser.add_argument('-o', '--output_path', type=str, required=False, default='' , help='Output path for report.')
     parser.add_argument('-n', '--report_name', type=str, required=False, default='' , help='Name of the report file.')
     parser.add_argument('-f', '--foreground', action='store_true', help='Start Tracer in foreground, not daemonized.')
 
     sp = parser.add_subparsers()
+    sp_configure = sp.add_parser('configure', help='Configure Tracer (default: %s)' % DEFAULT_CONFIG_YAML_PATH)
+    sp_configure.set_defaults(task='configure')    
+    
     sp_start = sp.add_parser('start', help='Start Tracer')
     sp_start.set_defaults(task='start')
 
     sp_stop = sp.add_parser('stop', help='Stop Tracer')
     sp_stop.set_defaults(task='stop')
 
     sp_restart = sp.add_parser('restart', help='Restart Tracer')
```

### Comparing `proctracer-0.0.23/proctracer.egg-info/PKG-INFO` & `proctracer-0.0.25/proctracer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proctracer
-Version: 0.0.23
+Version: 0.0.25
 Summary: /proc Tracer
 Home-page: https://github.com/david-kracht/proctracer
 Author: David Kracht
 Author-email: dave.kracht@gmail.com
 License: BSD-3
 Project-URL: Documentation, https://github.com/david-kracht/proctracer
 Project-URL: Source, https://github.com/david-kracht/proctracer.git
```

### Comparing `proctracer-0.0.23/proctracer.egg-info/SOURCES.txt` & `proctracer-0.0.25/proctracer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proctracer-0.0.23/setup.py` & `proctracer-0.0.25/setup.py`

 * *Files identical despite different names*

