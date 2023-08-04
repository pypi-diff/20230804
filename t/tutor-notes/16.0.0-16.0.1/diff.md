# Comparing `tmp/tutor-notes-16.0.0.tar.gz` & `tmp/tutor-notes-16.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutor-notes-16.0.0.tar", last modified: Wed Jun 14 23:42:28 2023, max compression
+gzip compressed data, was "tutor-notes-16.0.1.tar", last modified: Fri Aug  4 13:21:40 2023, max compression
```

## Comparing `tutor-notes-16.0.0.tar` & `tutor-notes-16.0.1.tar`

### file list

```diff
@@ -1,47 +1,49 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/
--rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/LICENSE.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)     4305 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     3306 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/pyproject.toml
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1642 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.932627 tutor-notes-16.0.0/tutor_notes.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)     4305 2023-06-14 23:42:28.000000 tutor-notes-16.0.0/tutor_notes.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1093 2023-06-14 23:42:28.000000 tutor-notes-16.0.0/tutor_notes.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-06-14 23:42:28.000000 tutor-notes-16.0.0/tutor_notes.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-06-14 23:42:28.000000 tutor-notes-16.0.0/tutor_notes.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-06-14 23:42:28.000000 tutor-notes-16.0.0/tutor_notes.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-06-14 23:42:28.000000 tutor-notes-16.0.0/tutor_notes.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.932627 tutor-notes-16.0.0/tutornotes/
--rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/tutornotes/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)      903 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      606 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/k8s-jobs
--rw-r--r--   0 ci        (1000) ci        (1000)      217 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)       74 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/kustomization-configmapgenerator
--rw-r--r--   0 ci        (1000) ci        (1000)      111 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      275 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/local-docker-compose-jobs-services
--rw-r--r--   0 ci        (1000) ci        (1000)      576 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/local-docker-compose-services
--rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/openedx-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)       47 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/openedx-lms-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      111 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/openedx-lms-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      143 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/patches/openedx-lms-production-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     3930 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.929294 tutor-notes-16.0.0/tutornotes/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.929294 tutor-notes-16.0.0/tutornotes/templates/notes/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.929294 tutor-notes-16.0.0/tutornotes/templates/notes/apps/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/tutornotes/templates/notes/apps/settings/
--rw-r--r--   0 ci        (1000) ci        (1000)     1073 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/templates/notes/apps/settings/tutor.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.929294 tutor-notes-16.0.0/tutornotes/templates/notes/build/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/tutornotes/templates/notes/build/notes/
--rw-r--r--   0 ci        (1000) ci        (1000)     1364 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/templates/notes/build/notes/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.929294 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)      574 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/lms/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/mysql/
--rw-r--r--   0 ci        (1000) ci        (1000)      797 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/mysql/init
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-06-14 23:42:28.939294 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/notes/
--rw-r--r--   0 ci        (1000) ci        (1000)       58 2023-06-14 23:42:22.000000 tutor-notes-16.0.0/tutornotes/templates/notes/tasks/notes/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.551104 tutor-notes-16.0.1/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)     4305 2023-08-04 13:21:40.551104 tutor-notes-16.0.1/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     3306 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       50 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/pyproject.toml
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-08-04 13:21:40.551104 tutor-notes-16.0.1/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1642 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.541104 tutor-notes-16.0.1/tutor_notes.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)     4305 2023-08-04 13:21:40.000000 tutor-notes-16.0.1/tutor_notes.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1213 2023-08-04 13:21:40.000000 tutor-notes-16.0.1/tutor_notes.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-08-04 13:21:40.000000 tutor-notes-16.0.1/tutor_notes.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       44 2023-08-04 13:21:40.000000 tutor-notes-16.0.1/tutor_notes.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-08-04 13:21:40.000000 tutor-notes-16.0.1/tutor_notes.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       11 2023-08-04 13:21:40.000000 tutor-notes-16.0.1/tutor_notes.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.544437 tutor-notes-16.0.1/tutornotes/
+-rw-r--r--   0 ci        (1000) ci        (1000)      175 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.547771 tutor-notes-16.0.1/tutornotes/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)       79 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      903 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      606 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/k8s-jobs
+-rw-r--r--   0 ci        (1000) ci        (1000)      217 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       74 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/kustomization-configmapgenerator
+-rw-r--r--   0 ci        (1000) ci        (1000)      111 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      275 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/local-docker-compose-jobs-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       28 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/local-docker-compose-permissions-command
+-rw-r--r--   0 ci        (1000) ci        (1000)       33 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/local-docker-compose-permissions-volumes
+-rw-r--r--   0 ci        (1000) ci        (1000)      387 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/local-docker-compose-services
+-rw-r--r--   0 ci        (1000) ci        (1000)       51 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/openedx-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)       47 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/openedx-lms-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      111 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/openedx-lms-development-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      143 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/patches/openedx-lms-production-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     3930 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.537771 tutor-notes-16.0.1/tutornotes/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.537771 tutor-notes-16.0.1/tutornotes/templates/notes/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.537771 tutor-notes-16.0.1/tutornotes/templates/notes/apps/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.551104 tutor-notes-16.0.1/tutornotes/templates/notes/apps/settings/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1073 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/templates/notes/apps/settings/tutor.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.537771 tutor-notes-16.0.1/tutornotes/templates/notes/build/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.551104 tutor-notes-16.0.1/tutornotes/templates/notes/build/notes/
+-rw-r--r--   0 ci        (1000) ci        (1000)     1364 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/templates/notes/build/notes/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.537771 tutor-notes-16.0.1/tutornotes/templates/notes/tasks/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.551104 tutor-notes-16.0.1/tutornotes/templates/notes/tasks/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)      574 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/templates/notes/tasks/lms/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.551104 tutor-notes-16.0.1/tutornotes/templates/notes/tasks/mysql/
+-rw-r--r--   0 ci        (1000) ci        (1000)      797 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/templates/notes/tasks/mysql/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-08-04 13:21:40.551104 tutor-notes-16.0.1/tutornotes/templates/notes/tasks/notes/
+-rw-r--r--   0 ci        (1000) ci        (1000)       58 2023-08-04 13:21:34.000000 tutor-notes-16.0.1/tutornotes/templates/notes/tasks/notes/init
```

### Comparing `tutor-notes-16.0.0/LICENSE.txt` & `tutor-notes-16.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tutor-notes-16.0.0/PKG-INFO` & `tutor-notes-16.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-notes
-Version: 16.0.0
+Version: 16.0.1
 Summary: A Tutor plugin for student notes
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: eduNEXT
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
```

### Comparing `tutor-notes-16.0.0/README.rst` & `tutor-notes-16.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `tutor-notes-16.0.0/setup.py` & `tutor-notes-16.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-notes-16.0.0/tutor_notes.egg-info/PKG-INFO` & `tutor-notes-16.0.1/tutor_notes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-notes
-Version: 16.0.0
+Version: 16.0.1
 Summary: A Tutor plugin for student notes
 Home-page: https://docs.tutor.overhang.io/
 Author: Overhang.IO
 Author-email: contact@overhang.io
 Maintainer: eduNEXT
 License: AGPLv3
 Project-URL: Documentation, https://docs.tutor.overhang.io/
```

### Comparing `tutor-notes-16.0.0/tutor_notes.egg-info/SOURCES.txt` & `tutor-notes-16.0.1/tutor_notes.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 tutornotes/patches/caddyfile
 tutornotes/patches/k8s-deployments
 tutornotes/patches/k8s-jobs
 tutornotes/patches/k8s-services
 tutornotes/patches/kustomization-configmapgenerator
 tutornotes/patches/local-docker-compose-dev-services
 tutornotes/patches/local-docker-compose-jobs-services
+tutornotes/patches/local-docker-compose-permissions-command
+tutornotes/patches/local-docker-compose-permissions-volumes
 tutornotes/patches/local-docker-compose-services
 tutornotes/patches/openedx-common-settings
 tutornotes/patches/openedx-lms-common-settings
 tutornotes/patches/openedx-lms-development-settings
 tutornotes/patches/openedx-lms-production-settings
 tutornotes/templates/notes/apps/settings/tutor.py
 tutornotes/templates/notes/build/notes/Dockerfile
```

### Comparing `tutor-notes-16.0.0/tutornotes/patches/k8s-deployments` & `tutor-notes-16.0.1/tutornotes/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-notes-16.0.0/tutornotes/patches/k8s-jobs` & `tutor-notes-16.0.1/tutornotes/patches/k8s-jobs`

 * *Files identical despite different names*

### Comparing `tutor-notes-16.0.0/tutornotes/plugin.py` & `tutor-notes-16.0.1/tutornotes/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-notes-16.0.0/tutornotes/templates/notes/apps/settings/tutor.py` & `tutor-notes-16.0.1/tutornotes/templates/notes/apps/settings/tutor.py`

 * *Files identical despite different names*

### Comparing `tutor-notes-16.0.0/tutornotes/templates/notes/build/notes/Dockerfile` & `tutor-notes-16.0.1/tutornotes/templates/notes/build/notes/Dockerfile`

 * *Files identical despite different names*

### Comparing `tutor-notes-16.0.0/tutornotes/templates/notes/tasks/lms/init` & `tutor-notes-16.0.1/tutornotes/templates/notes/tasks/lms/init`

 * *Files identical despite different names*

### Comparing `tutor-notes-16.0.0/tutornotes/templates/notes/tasks/mysql/init` & `tutor-notes-16.0.1/tutornotes/templates/notes/tasks/mysql/init`

 * *Files identical despite different names*

