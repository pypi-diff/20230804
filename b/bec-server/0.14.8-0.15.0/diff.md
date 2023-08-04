# Comparing `tmp/bec-server-0.14.8.tar.gz` & `tmp/bec-server-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bec-server-0.14.8.tar", last modified: Wed Jul 26 19:23:55 2023, max compression
+gzip compressed data, was "bec-server-0.15.0.tar", last modified: Thu Aug  3 19:22:59 2023, max compression
```

## Comparing `bec-server-0.14.8.tar` & `bec-server-0.15.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 19:23:55.170905 bec-server-0.14.8/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-26 19:23:55.170905 bec-server-0.14.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 19:23:55.169905 bec-server-0.14.8/bec_server/
--rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.14.8/bec_server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-21 18:30:48.000000 bec-server-0.14.8/bec_server/launch.py
--rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.14.8/bec_server/service_handler.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2023-07-21 18:30:48.000000 bec-server-0.14.8/bec_server/tmux_launch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 19:23:55.170905 bec-server-0.14.8/bec_server.egg-info/
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-26 19:23:55.000000 bec-server-0.14.8/bec_server.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2023-07-26 19:23:55.000000 bec-server-0.14.8/bec_server.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 19:23:55.000000 bec-server-0.14.8/bec_server.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-07-26 19:23:55.000000 bec-server-0.14.8/bec_server.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      192 2023-07-26 19:23:55.000000 bec-server-0.14.8/bec_server.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-26 19:23:55.000000 bec-server-0.14.8/bec_server.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      503 2023-07-26 19:23:55.171905 bec-server-0.14.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2167 2023-07-26 19:23:48.000000 bec-server-0.14.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:22:59.516906 bec-server-0.15.0/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-08-03 19:22:59.516906 bec-server-0.15.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:22:59.515906 bec-server-0.15.0/bec_server/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-07-08 15:33:35.000000 bec-server-0.15.0/bec_server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-07-21 18:30:48.000000 bec-server-0.15.0/bec_server/launch.py
+-rw-r--r--   0 root         (0) root         (0)     3075 2023-07-08 15:33:35.000000 bec-server-0.15.0/bec_server/service_handler.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-07-21 18:30:48.000000 bec-server-0.15.0/bec_server/tmux_launch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-03 19:22:59.516906 bec-server-0.15.0/bec_server.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      443 2023-08-03 19:22:59.000000 bec-server-0.15.0/bec_server.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      332 2023-08-03 19:22:59.000000 bec-server-0.15.0/bec_server.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-03 19:22:59.000000 bec-server-0.15.0/bec_server.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-08-03 19:22:59.000000 bec-server-0.15.0/bec_server.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      192 2023-08-03 19:22:59.000000 bec-server-0.15.0/bec_server.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-03 19:22:59.000000 bec-server-0.15.0/bec_server.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      503 2023-08-03 19:22:59.516906 bec-server-0.15.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2023-08-03 19:22:53.000000 bec-server-0.15.0/setup.py
```

### Comparing `bec-server-0.14.8/bec_server/launch.py` & `bec-server-0.15.0/bec_server/launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.8/bec_server/service_handler.py` & `bec-server-0.15.0/bec_server/service_handler.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.8/bec_server/tmux_launch.py` & `bec-server-0.15.0/bec_server/tmux_launch.py`

 * *Files identical despite different names*

### Comparing `bec-server-0.14.8/setup.py` & `bec-server-0.15.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import subprocess
 import sys
 
 from setuptools import setup
 
 current_path = pathlib.Path(__file__).parent.resolve()
 
-__version__ = "0.14.8"
+__version__ = "0.15.0"
 
 
 def run_install(setup_args: dict, bec_deps: list, editable=False):
     """
     Run the setup function with the given arguments.
 
     Args:
```
