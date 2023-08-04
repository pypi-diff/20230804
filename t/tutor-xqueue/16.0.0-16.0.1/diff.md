# Comparing `tmp/tutor-xqueue-16.0.0.tar.gz` & `tmp/tutor-xqueue-16.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-xqueue-16.0.0.tar", last modified: Thu Jun 15 00:19:06 2023, max compression
+gzip compressed data, was "tutor-xqueue-16.0.1.tar", last modified: Fri Aug  4 13:23:21 2023, max compression
```

## Comparing `tutor-xqueue-16.0.0.tar` & `tutor-xqueue-16.0.1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.507030 tutor-xqueue-16.0.0/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       81 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     6676 2023-06-15 00:19:06.507030 tutor-xqueue-16.0.0/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     5630 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/pyproject.toml
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-15 00:19:06.507030 tutor-xqueue-16.0.0/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1715 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.500363 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     6676 2023-06-15 00:19:06.000000 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)      929 2023-06-15 00:19:06.000000 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-15 00:19:06.000000 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       46 2023-06-15 00:19:06.000000 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       31 2023-06-15 00:19:06.000000 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       12 2023-06-15 00:19:06.000000 tutor-xqueue-16.0.0/tutor_xqueue.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.500363 tutor-xqueue-16.0.0/tutorxqueue/
--rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.503696 tutor-xqueue-16.0.0/tutorxqueue/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)       82 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)     1184 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      578 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/k8s-jobs
--rw-r--r--   0 ci        (1000) ci        (1000)      173 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)       76 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/kustomization-configmapgenerator
--rw-r--r--   0 ci        (1000) ci        (1000)       88 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      221 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      967 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)      204 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/patches/openedx-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     9235 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.493696 tutor-xqueue-16.0.0/tutorxqueue/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.493696 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.493696 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.503696 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/apps/settings/
--rw-r--r--   0 ci        (1000) ci        (1000)      956 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/apps/settings/tutor.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.493696 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.503696 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/build/xqueue/
--rw-r--r--   0 ci        (1000) ci        (1000)     1641 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/build/xqueue/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.497030 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/tasks/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.503696 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/tasks/mysql/
--rw-r--r--   0 ci        (1000) ci        (1000)      803 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/tasks/mysql/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-15 00:19:06.507030 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/tasks/xqueue/
--rw-r--r--   0 ci        (1000) ci        (1000)       45 2023-06-15 00:18:58.000000 tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/tasks/xqueue/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:21.421645 tutor-xqueue-16.0.1/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       81 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     6688 2023-08-04 13:23:21.421645 tutor-xqueue-16.0.1/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     5630 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-08-04 13:23:21.421645 tutor-xqueue-16.0.1/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1727 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:21.414978 tutor-xqueue-16.0.1/tutor_xqueue.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     6688 2023-08-04 13:23:21.000000 tutor-xqueue-16.0.1/tutor_xqueue.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1051 2023-08-04 13:23:21.000000 tutor-xqueue-16.0.1/tutor_xqueue.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-08-04 13:23:21.000000 tutor-xqueue-16.0.1/tutor_xqueue.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       46 2023-08-04 13:23:21.000000 tutor-xqueue-16.0.1/tutor_xqueue.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       31 2023-08-04 13:23:21.000000 tutor-xqueue-16.0.1/tutor_xqueue.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       12 2023-08-04 13:23:21.000000 tutor-xqueue-16.0.1/tutor_xqueue.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:21.414978 tutor-xqueue-16.0.1/tutorxqueue/
+-rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:21.418311 tutor-xqueue-16.0.1/tutorxqueue/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)       82 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)     1184 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      578 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      173 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       76 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/patches/kustomization-configmapgenerator
+-rw-r--r--   0 ci        (1000) ci        (1000)       88 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      221 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       29 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/patches/local-docker-compose-permissions-command
+-rw-r--r--   0 ci        (1000) ci        (1000)       41 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/patches/local-docker-compose-permissions-volumes
+-rw-r--r--   0 ci        (1000) ci        (1000)      788 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      204 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/patches/openedx-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     9235 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:21.408311 tutor-xqueue-16.0.1/tutorxqueue/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:21.408311 tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:21.408311 tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:21.418311 tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/apps/settings/
+-rw-r--r--   0 ci        (1000) ci        (1000)      956 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/apps/settings/tutor.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:21.408311 tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:21.418311 tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/build/xqueue/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1641 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/build/xqueue/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:21.411645 tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/tasks/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:21.421645 tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/tasks/mysql/
+-rw-r--r--   0 ci        (1000) ci        (1000)      803 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/tasks/mysql/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:23:21.421645 tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/tasks/xqueue/
+-rw-r--r--   0 ci        (1000) ci        (1000)       45 2023-08-04 13:23:16.000000 tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/tasks/xqueue/init
```

### Comparing `tutor-xqueue-16.0.0/LICENSE.txt` & `tutor-xqueue-16.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-xqueue-16.0.0/PKG-INFO` & `tutor-xqueue-16.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tutor-xqueue
-Version: 16.0.0
+Version: 16.0.1
 Summary: A Tutor plugin for Xqueue (external grading system)
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: eduNEXT
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor-xqueue
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-xqueue/issues
 Project-URL: Community, https://discuss.openedx.org
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tutor-xqueue-16.0.0/README.rst` & `tutor-xqueue-16.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-xqueue-16.0.0/setup.py` & `tutor-xqueue-16.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     long_description_content_type="text/x-rst",
     packages=find_packages(exclude=["tests*"]),
     include_package_data=True,
     python_requires=">=3.8",
     install_requires=["tutor>=16.0.0,<17.0.0", "requests"],
     entry_points={"tutor.plugin.v1": ["xqueue = tutorxqueue.plugin"]},
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
```

### Comparing `tutor-xqueue-16.0.0/tutor_xqueue.egg-info/PKG-INFO` & `tutor-xqueue-16.0.1/tutor_xqueue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: tutor-xqueue
-Version: 16.0.0
+Version: 16.0.1
 Summary: A Tutor plugin for Xqueue (external grading system)
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: eduNEXT
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
 Project-URL: Code, https://github.com/overhangio/tutor-xqueue
 Project-URL: Issue tracker, https://github.com/overhangio/tutor-xqueue/issues
 Project-URL: Community, https://discuss.openedx.org
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tutor-xqueue-16.0.0/tutor_xqueue.egg-info/SOURCES.txt` & `tutor-xqueue-16.0.1/tutor_xqueue.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -15,13 +15,15 @@
 tutorxqueue/patches/caddyfile
 tutorxqueue/patches/k8s-deployments
 tutorxqueue/patches/k8s-jobs
 tutorxqueue/patches/k8s-services
 tutorxqueue/patches/kustomization-configmapgenerator
 tutorxqueue/patches/local-docker-compose-dev-services
 tutorxqueue/patches/local-docker-compose-jobs-services
+tutorxqueue/patches/local-docker-compose-permissions-command
+tutorxqueue/patches/local-docker-compose-permissions-volumes
 tutorxqueue/patches/local-docker-compose-services
 tutorxqueue/patches/openedx-common-settings
 tutorxqueue/templates/xqueue/apps/settings/tutor.py
 tutorxqueue/templates/xqueue/build/xqueue/Dockerfile
 tutorxqueue/templates/xqueue/tasks/mysql/init
 tutorxqueue/templates/xqueue/tasks/xqueue/init
```

### Comparing `tutor-xqueue-16.0.0/tutorxqueue/patches/k8s-deployments` & `tutor-xqueue-16.0.1/tutorxqueue/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-xqueue-16.0.0/tutorxqueue/patches/k8s-jobs` & `tutor-xqueue-16.0.1/tutorxqueue/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-xqueue-16.0.0/tutorxqueue/plugin.py` & `tutor-xqueue-16.0.1/tutorxqueue/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/apps/settings/tutor.py` & `tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/apps/settings/tutor.py`

 * *Files identical despite different names*

### Comparing `tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/build/xqueue/Dockerfile` & `tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/build/xqueue/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-xqueue-16.0.0/tutorxqueue/templates/xqueue/tasks/mysql/init` & `tutor-xqueue-16.0.1/tutorxqueue/templates/xqueue/tasks/mysql/init`

 * *Files identical despite different names*

