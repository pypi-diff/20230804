# Comparing `tmp/peek-field-service-3.4.8.tar.gz` & `tmp/peek-field-service-3.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-field-service-3.4.8.tar", last modified: Tue Jul 11 02:52:40 2023, max compression
+gzip compressed data, was "peek-field-service-3.4.9.tar", last modified: Wed Jul 19 06:51:22 2023, max compression
```

## Comparing `peek-field-service-3.4.8.tar` & `peek-field-service-3.4.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:40.539033 peek-field-service-3.4.8/
--rw-r--r--   0 root         (0) root         (0)      373 2023-07-11 02:52:40.538033 peek-field-service-3.4.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      245 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:40.537033 peek-field-service-3.4.8/peek_field_service/
--rw-r--r--   0 root         (0) root         (0)     1506 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/PeekClientConfig.py
--rw-r--r--   0 root         (0) root         (0)     1295 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/PeekClientConfigTest.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      146 2023-07-11 02:52:40.000000 peek-field-service-3.4.8/peek_field_service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:40.538033 peek-field-service-3.4.8/peek_field_service/backend/
--rw-r--r--   0 root         (0) root         (0)      448 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/backend/ClientObservable.py
--rw-r--r--   0 root         (0) root         (0)     2247 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/backend/SiteRootResource.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:40.538033 peek-field-service-3.4.8/peek_field_service/plugin/
--rw-r--r--   0 root         (0) root         (0)     1575 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/plugin/ClientFrontendBuildersMixin.py
--rw-r--r--   0 root         (0) root         (0)     2779 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/plugin/ClientPluginLoader.py
--rw-r--r--   0 root         (0) root         (0)     1629 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/plugin/ClientPluginLoaderTest.py
--rw-r--r--   0 root         (0) root         (0)     3107 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/plugin/PeekClientPlatformHook.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/plugin/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9797 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/run_peek_field_service.py
--rw-r--r--   0 root         (0) root         (0)      600 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/run_peek_field_service_build_only.py
--rw-r--r--   0 root         (0) root         (0)      646 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/run_peek_field_service_offline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:40.538033 peek-field-service-3.4.8/peek_field_service/sw_install/
--rw-r--r--   0 root         (0) root         (0)      792 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/sw_install/PeekSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      326 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/sw_install/PluginSwInstallManager.py
--rw-r--r--   0 root         (0) root         (0)      141 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/sw_install/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-07-11 02:51:11.000000 peek-field-service-3.4.8/peek_field_service/winsvc_peek_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 02:52:40.538033 peek-field-service-3.4.8/peek_field_service.egg-info/
--rw-r--r--   0 root         (0) root         (0)      373 2023-07-11 02:52:40.000000 peek-field-service-3.4.8/peek_field_service.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1199 2023-07-11 02:52:40.000000 peek-field-service-3.4.8/peek_field_service.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:52:40.000000 peek-field-service-3.4.8/peek_field_service.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      351 2023-07-11 02:52:40.000000 peek-field-service-3.4.8/peek_field_service.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 02:52:40.000000 peek-field-service-3.4.8/peek_field_service.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      121 2023-07-11 02:52:40.000000 peek-field-service-3.4.8/peek_field_service.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-07-11 02:52:40.000000 peek-field-service-3.4.8/peek_field_service.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-11 02:52:40.539033 peek-field-service-3.4.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3259 2023-07-11 02:52:40.000000 peek-field-service-3.4.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:22.049952 peek-field-service-3.4.9/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-07-19 06:51:22.048952 peek-field-service-3.4.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      245 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:22.047953 peek-field-service-3.4.9/peek_field_service/
+-rw-r--r--   0 root         (0) root         (0)     1506 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/PeekClientConfig.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/PeekClientConfigTest.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      146 2023-07-19 06:51:21.000000 peek-field-service-3.4.9/peek_field_service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:22.048952 peek-field-service-3.4.9/peek_field_service/backend/
+-rw-r--r--   0 root         (0) root         (0)      448 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/backend/ClientObservable.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/backend/SiteRootResource.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:22.048952 peek-field-service-3.4.9/peek_field_service/plugin/
+-rw-r--r--   0 root         (0) root         (0)     1575 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/plugin/ClientFrontendBuildersMixin.py
+-rw-r--r--   0 root         (0) root         (0)     2779 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/plugin/ClientPluginLoader.py
+-rw-r--r--   0 root         (0) root         (0)     1629 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/plugin/ClientPluginLoaderTest.py
+-rw-r--r--   0 root         (0) root         (0)     3107 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/plugin/PeekClientPlatformHook.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/plugin/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9797 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/run_peek_field_service.py
+-rw-r--r--   0 root         (0) root         (0)      600 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/run_peek_field_service_build_only.py
+-rw-r--r--   0 root         (0) root         (0)      646 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/run_peek_field_service_offline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:22.048952 peek-field-service-3.4.9/peek_field_service/sw_install/
+-rw-r--r--   0 root         (0) root         (0)      792 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/sw_install/PeekSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      326 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/sw_install/PluginSwInstallManager.py
+-rw-r--r--   0 root         (0) root         (0)      141 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/sw_install/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-07-19 06:49:47.000000 peek-field-service-3.4.9/peek_field_service/winsvc_peek_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-19 06:51:22.048952 peek-field-service-3.4.9/peek_field_service.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      373 2023-07-19 06:51:22.000000 peek-field-service-3.4.9/peek_field_service.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1199 2023-07-19 06:51:22.000000 peek-field-service-3.4.9/peek_field_service.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 06:51:22.000000 peek-field-service-3.4.9/peek_field_service.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      351 2023-07-19 06:51:22.000000 peek-field-service-3.4.9/peek_field_service.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-19 06:51:22.000000 peek-field-service-3.4.9/peek_field_service.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      121 2023-07-19 06:51:22.000000 peek-field-service-3.4.9/peek_field_service.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-07-19 06:51:22.000000 peek-field-service-3.4.9/peek_field_service.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-19 06:51:22.049952 peek-field-service-3.4.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-07-19 06:51:21.000000 peek-field-service-3.4.9/setup.py
```

### Comparing `peek-field-service-3.4.8/peek_field_service/PeekClientConfig.py` & `peek-field-service-3.4.9/peek_field_service/PeekClientConfig.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.8/peek_field_service/PeekClientConfigTest.py` & `peek-field-service-3.4.9/peek_field_service/PeekClientConfigTest.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.8/peek_field_service/backend/SiteRootResource.py` & `peek-field-service-3.4.9/peek_field_service/backend/SiteRootResource.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.8/peek_field_service/plugin/ClientFrontendBuildersMixin.py` & `peek-field-service-3.4.9/peek_field_service/plugin/ClientFrontendBuildersMixin.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.8/peek_field_service/plugin/ClientPluginLoader.py` & `peek-field-service-3.4.9/peek_field_service/plugin/ClientPluginLoader.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.8/peek_field_service/plugin/ClientPluginLoaderTest.py` & `peek-field-service-3.4.9/peek_field_service/plugin/ClientPluginLoaderTest.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.8/peek_field_service/plugin/PeekClientPlatformHook.py` & `peek-field-service-3.4.9/peek_field_service/plugin/PeekClientPlatformHook.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.8/peek_field_service/run_peek_field_service.py` & `peek-field-service-3.4.9/peek_field_service/run_peek_field_service.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.8/peek_field_service/run_peek_field_service_build_only.py` & `peek-field-service-3.4.9/peek_field_service/run_peek_field_service_build_only.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.8/peek_field_service/run_peek_field_service_offline.py` & `peek-field-service-3.4.9/peek_field_service/run_peek_field_service_offline.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.8/peek_field_service/sw_install/PeekSwInstallManager.py` & `peek-field-service-3.4.9/peek_field_service/sw_install/PeekSwInstallManager.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.8/peek_field_service/winsvc_peek_client.py` & `peek-field-service-3.4.9/peek_field_service/winsvc_peek_client.py`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.8/peek_field_service.egg-info/SOURCES.txt` & `peek-field-service-3.4.9/peek_field_service.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-field-service-3.4.8/setup.py` & `peek-field-service-3.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # Modify these values to fork a new plugin
 #
 
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_field_service"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.8"
+package_version = "3.4.9"
 description = "Peek Field Service."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 ###############################################################################
```

