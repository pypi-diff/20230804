# Comparing `tmp/peek-worker-service-3.4.8.tar.gz` & `tmp/peek-worker-service-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-worker-service-3.4.8.tar", last modified: Tue Jul 11 02:53:13 2023, max compression
+gzip compressed data, was "peek-worker-service-3.4.9.tar", last modified: Wed Jul 19 06:51:53 2023, max compression
```

## Comparing `peek-worker-service-3.4.8.tar` & `peek-worker-service-3.4.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:13.859971 peek-worker-service-3.4.8/
--rw-r--r--   0 root         (0) root         (0)      377 2023-07-11 02:53:13.859971 peek-worker-service-3.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      418 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:13.858971 peek-worker-service-3.4.8/peek_worker_service/
--rw-r--r--   0 root         (0) root         (0)     1922 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/CeleryApp.py
--rw-r--r--   0 root         (0) root         (0)     1321 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/PeekWorkerConfig.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/PeekWorkerConfigTest.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      271 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/TempUnitTest.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-07-11 02:53:13.000000 peek-worker-service-3.4.8/peek_worker_service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:13.859971 peek-worker-service-3.4.8/peek_worker_service/plugin/
--rw-r--r--   0 root         (0) root         (0)     2155 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/plugin/PeekWorkerPlatformHook.py
--rw-r--r--   0 root         (0) root         (0)     1996 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/plugin/WorkerPluginLoader.py
--rw-r--r--   0 root         (0) root         (0)     1482 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/plugin/WorkerPluginLoaderTest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/plugin/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     8906 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/run_peek_worker_service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:13.859971 peek-worker-service-3.4.8/peek_worker_service/sw_install/
--rw-r--r--   0 root         (0) root         (0)     1080 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/sw_install/PeekSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      526 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/sw_install/PluginSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/sw_install/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1673 2023-07-11 02:51:12.000000 peek-worker-service-3.4.8/peek_worker_service/winsvc_peek_worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:53:13.859971 peek-worker-service-3.4.8/peek_worker_service.egg-info/
--rw-r--r--   0 root         (0) root         (0)      377 2023-07-11 02:53:13.000000 peek-worker-service-3.4.8/peek_worker_service.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1000 2023-07-11 02:53:13.000000 peek-worker-service-3.4.8/peek_worker_service.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:53:13.000000 peek-worker-service-3.4.8/peek_worker_service.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      175 2023-07-11 02:53:13.000000 peek-worker-service-3.4.8/peek_worker_service.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:53:13.000000 peek-worker-service-3.4.8/peek_worker_service.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       61 2023-07-11 02:53:13.000000 peek-worker-service-3.4.8/peek_worker_service.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-07-11 02:53:13.000000 peek-worker-service-3.4.8/peek_worker_service.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       80 2023-07-11 02:53:13.868971 peek-worker-service-3.4.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2925 2023-07-11 02:53:13.000000 peek-worker-service-3.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:53.765018 peek-worker-service-3.4.9/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-07-19 06:51:53.765018 peek-worker-service-3.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      418 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:53.764018 peek-worker-service-3.4.9/peek_worker_service/
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/CeleryApp.py
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/PeekWorkerConfig.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/PeekWorkerConfigTest.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      271 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/TempUnitTest.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-07-19 06:51:53.000000 peek-worker-service-3.4.9/peek_worker_service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:53.765018 peek-worker-service-3.4.9/peek_worker_service/plugin/
+-rw-r--r--   0 root         (0) root         (0)     2155 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/plugin/PeekWorkerPlatformHook.py
+-rw-r--r--   0 root         (0) root         (0)     1996 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/plugin/WorkerPluginLoader.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/plugin/WorkerPluginLoaderTest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/plugin/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8906 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/run_peek_worker_service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:53.765018 peek-worker-service-3.4.9/peek_worker_service/sw_install/
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/sw_install/PeekSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      526 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/sw_install/PluginSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/sw_install/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1673 2023-07-19 06:49:48.000000 peek-worker-service-3.4.9/peek_worker_service/winsvc_peek_worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:53.764018 peek-worker-service-3.4.9/peek_worker_service.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      377 2023-07-19 06:51:53.000000 peek-worker-service-3.4.9/peek_worker_service.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1000 2023-07-19 06:51:53.000000 peek-worker-service-3.4.9/peek_worker_service.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 06:51:53.000000 peek-worker-service-3.4.9/peek_worker_service.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      175 2023-07-19 06:51:53.000000 peek-worker-service-3.4.9/peek_worker_service.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 06:51:53.000000 peek-worker-service-3.4.9/peek_worker_service.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       61 2023-07-19 06:51:53.000000 peek-worker-service-3.4.9/peek_worker_service.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-07-19 06:51:53.000000 peek-worker-service-3.4.9/peek_worker_service.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       80 2023-07-19 06:51:53.765018 peek-worker-service-3.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2925 2023-07-19 06:51:53.000000 peek-worker-service-3.4.9/setup.py
```

### Comparing `peek-worker-service-3.4.8/peek_worker_service/CeleryApp.py` & `peek-worker-service-3.4.9/peek_worker_service/CeleryApp.py`

 * *Files identical despite different names*

### Comparing `peek-worker-service-3.4.8/peek_worker_service/PeekWorkerConfig.py` & `peek-worker-service-3.4.9/peek_worker_service/PeekWorkerConfig.py`

 * *Files identical despite different names*

### Comparing `peek-worker-service-3.4.8/peek_worker_service/PeekWorkerConfigTest.py` & `peek-worker-service-3.4.9/peek_worker_service/PeekWorkerConfigTest.py`

 * *Files identical despite different names*

### Comparing `peek-worker-service-3.4.8/peek_worker_service/plugin/PeekWorkerPlatformHook.py` & `peek-worker-service-3.4.9/peek_worker_service/plugin/PeekWorkerPlatformHook.py`

 * *Files identical despite different names*

### Comparing `peek-worker-service-3.4.8/peek_worker_service/plugin/WorkerPluginLoader.py` & `peek-worker-service-3.4.9/peek_worker_service/plugin/WorkerPluginLoader.py`

 * *Files identical despite different names*

### Comparing `peek-worker-service-3.4.8/peek_worker_service/plugin/WorkerPluginLoaderTest.py` & `peek-worker-service-3.4.9/peek_worker_service/plugin/WorkerPluginLoaderTest.py`

 * *Files identical despite different names*

### Comparing `peek-worker-service-3.4.8/peek_worker_service/run_peek_worker_service.py` & `peek-worker-service-3.4.9/peek_worker_service/run_peek_worker_service.py`

 * *Files identical despite different names*

### Comparing `peek-worker-service-3.4.8/peek_worker_service/sw_install/PeekSwInstallManager.py` & `peek-worker-service-3.4.9/peek_worker_service/sw_install/PeekSwInstallManager.py`

 * *Files identical despite different names*

### Comparing `peek-worker-service-3.4.8/peek_worker_service/sw_install/PluginSwInstallManager.py` & `peek-worker-service-3.4.9/peek_worker_service/sw_install/PluginSwInstallManager.py`

 * *Files identical despite different names*

### Comparing `peek-worker-service-3.4.8/peek_worker_service/winsvc_peek_worker.py` & `peek-worker-service-3.4.9/peek_worker_service/winsvc_peek_worker.py`

 * *Files identical despite different names*

### Comparing `peek-worker-service-3.4.8/peek_worker_service.egg-info/SOURCES.txt` & `peek-worker-service-3.4.9/peek_worker_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-worker-service-3.4.8/setup.py` & `peek-worker-service-3.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_worker_service"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.8"
+package_version = "3.4.9"
 description = "Peek Worker Service."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

