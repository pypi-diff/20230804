# Comparing `tmp/django-autofixture-squad-0.12.2.dev1.tar.gz` & `tmp/django-autofixture-squad-0.12.3.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-autofixture-squad-0.12.2.dev1.tar", last modified: Fri Aug  4 08:09:10 2023, max compression
+gzip compressed data, was "dist/django-autofixture-squad-0.12.3.dev1.tar", last modified: Fri Aug  4 08:37:05 2023, max compression
```

## Comparing `django-autofixture-squad-0.12.2.dev1.tar` & `django-autofixture-squad-0.12.3.dev1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 08:09:10.000000 django-autofixture-squad-0.12.2.dev1/
--rw-r--r--   0 root         (0) root         (0)    18670 2023-08-04 08:09:10.000000 django-autofixture-squad-0.12.2.dev1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       99 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 08:09:10.000000 django-autofixture-squad-0.12.2.dev1/autofixture/
--rw-r--r--   0 root         (0) root         (0)     1389 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/autofixture/placeholder.py
--rw-r--r--   0 root         (0) root         (0)      138 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/autofixture/signals.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/autofixture/values.py
--rw-r--r--   0 root         (0) root         (0)     1862 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/autofixture/compat.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 07:51:12.000000 django-autofixture-squad-0.12.2.dev1/autofixture/models.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-08-04 07:39:51.000000 django-autofixture-squad-0.12.2.dev1/autofixture/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 08:09:10.000000 django-autofixture-squad-0.12.2.dev1/autofixture/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/autofixture/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 08:09:10.000000 django-autofixture-squad-0.12.2.dev1/autofixture/management/commands/
--rw-r--r--   0 root         (0) root         (0)     9757 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/autofixture/management/commands/loadtestdata.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/autofixture/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7971 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/autofixture/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21938 2023-08-04 07:22:49.000000 django-autofixture-squad-0.12.2.dev1/autofixture/generators.py
--rw-r--r--   0 root         (0) root         (0)     3399 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/autofixture/autofixtures.py
--rw-r--r--   0 root         (0) root         (0)     2130 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/autofixture/constraints.py
--rw-r--r--   0 root         (0) root         (0)    23157 2023-08-04 07:43:06.000000 django-autofixture-squad-0.12.2.dev1/autofixture/base.py
--rwxr-xr-x   0 root         (0) root         (0)     2384 2023-08-04 08:07:46.000000 django-autofixture-squad-0.12.2.dev1/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 08:09:10.000000 django-autofixture-squad-0.12.2.dev1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8857 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/README.rst
--rw-r--r--   0 root         (0) root         (0)     1515 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      810 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/AUTHORS.txt
--rw-r--r--   0 root         (0) root         (0)     5310 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.2.dev1/CHANGES.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 08:09:10.000000 django-autofixture-squad-0.12.2.dev1/django_autofixture_squad.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18670 2023-08-04 08:09:10.000000 django-autofixture-squad-0.12.2.dev1/django_autofixture_squad.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      696 2023-08-04 08:09:10.000000 django-autofixture-squad-0.12.2.dev1/django_autofixture_squad.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-08-04 08:09:10.000000 django-autofixture-squad-0.12.2.dev1/django_autofixture_squad.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-08-04 08:09:10.000000 django-autofixture-squad-0.12.2.dev1/django_autofixture_squad.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 08:09:10.000000 django-autofixture-squad-0.12.2.dev1/django_autofixture_squad.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 08:37:05.000000 django-autofixture-squad-0.12.3.dev1/
+-rw-r--r--   0 root         (0) root         (0)    18670 2023-08-04 08:37:05.000000 django-autofixture-squad-0.12.3.dev1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       99 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 08:37:05.000000 django-autofixture-squad-0.12.3.dev1/autofixture/
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/autofixture/placeholder.py
+-rw-r--r--   0 root         (0) root         (0)      138 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/autofixture/signals.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/autofixture/values.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/autofixture/compat.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 07:51:12.000000 django-autofixture-squad-0.12.3.dev1/autofixture/models.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-08-04 08:10:24.000000 django-autofixture-squad-0.12.3.dev1/autofixture/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 08:37:05.000000 django-autofixture-squad-0.12.3.dev1/autofixture/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/autofixture/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 08:37:05.000000 django-autofixture-squad-0.12.3.dev1/autofixture/management/commands/
+-rw-r--r--   0 root         (0) root         (0)     9757 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/autofixture/management/commands/loadtestdata.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/autofixture/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7971 2023-08-04 08:36:45.000000 django-autofixture-squad-0.12.3.dev1/autofixture/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21938 2023-08-04 08:10:24.000000 django-autofixture-squad-0.12.3.dev1/autofixture/generators.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/autofixture/autofixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/autofixture/constraints.py
+-rw-r--r--   0 root         (0) root         (0)    23157 2023-08-04 08:10:24.000000 django-autofixture-squad-0.12.3.dev1/autofixture/base.py
+-rwxr-xr-x   0 root         (0) root         (0)     2384 2023-08-04 08:10:24.000000 django-autofixture-squad-0.12.3.dev1/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 08:37:05.000000 django-autofixture-squad-0.12.3.dev1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8857 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      810 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/AUTHORS.txt
+-rw-r--r--   0 root         (0) root         (0)     5310 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.3.dev1/CHANGES.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 08:37:05.000000 django-autofixture-squad-0.12.3.dev1/django_autofixture_squad.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18670 2023-08-04 08:37:05.000000 django-autofixture-squad-0.12.3.dev1/django_autofixture_squad.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      696 2023-08-04 08:37:05.000000 django-autofixture-squad-0.12.3.dev1/django_autofixture_squad.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-04 08:37:05.000000 django-autofixture-squad-0.12.3.dev1/django_autofixture_squad.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-08-04 08:37:05.000000 django-autofixture-squad-0.12.3.dev1/django_autofixture_squad.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 08:37:05.000000 django-autofixture-squad-0.12.3.dev1/django_autofixture_squad.egg-info/dependency_links.txt
```

### Comparing `django-autofixture-squad-0.12.2.dev1/PKG-INFO` & `django-autofixture-squad-0.12.3.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-autofixture-squad
-Version: 0.12.2.dev1
+Version: 0.12.3.dev1
 Summary: Provides tools to auto generate test data.
 Home-page: https://github.com/squadrun/django-autofixture
 Author: Gregor Müllegger
 Author-email: gregor@muellegger.de
 License: BSD
 Description: ==================
         django-autofixture
```

### Comparing `django-autofixture-squad-0.12.2.dev1/autofixture/placeholder.py` & `django-autofixture-squad-0.12.3.dev1/autofixture/placeholder.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/autofixture/values.py` & `django-autofixture-squad-0.12.3.dev1/autofixture/values.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/autofixture/compat.py` & `django-autofixture-squad-0.12.3.dev1/autofixture/compat.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/autofixture/fields.py` & `django-autofixture-squad-0.12.3.dev1/autofixture/fields.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/autofixture/management/commands/loadtestdata.py` & `django-autofixture-squad-0.12.3.dev1/autofixture/management/commands/loadtestdata.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/autofixture/__init__.py` & `django-autofixture-squad-0.12.3.dev1/autofixture/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 if sys.version_info[0] < 3:
     string_types = basestring
 else:
     string_types = str
 
 
-__version__ = '0.12.2.dev1'
+__version__ = '0.12.3.dev1'
 
 
 REGISTRY = {}
 
 
 def register(model, autofixture, overwrite=False, fail_silently=False):
     '''
```

### Comparing `django-autofixture-squad-0.12.2.dev1/autofixture/generators.py` & `django-autofixture-squad-0.12.3.dev1/autofixture/generators.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/autofixture/autofixtures.py` & `django-autofixture-squad-0.12.3.dev1/autofixture/autofixtures.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/autofixture/constraints.py` & `django-autofixture-squad-0.12.3.dev1/autofixture/constraints.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/autofixture/base.py` & `django-autofixture-squad-0.12.3.dev1/autofixture/base.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/setup.py` & `django-autofixture-squad-0.12.3.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/README.rst` & `django-autofixture-squad-0.12.3.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/LICENSE.txt` & `django-autofixture-squad-0.12.3.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/AUTHORS.txt` & `django-autofixture-squad-0.12.3.dev1/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/CHANGES.rst` & `django-autofixture-squad-0.12.3.dev1/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.2.dev1/django_autofixture_squad.egg-info/PKG-INFO` & `django-autofixture-squad-0.12.3.dev1/django_autofixture_squad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-autofixture-squad
-Version: 0.12.2.dev1
+Version: 0.12.3.dev1
 Summary: Provides tools to auto generate test data.
 Home-page: https://github.com/squadrun/django-autofixture
 Author: Gregor Müllegger
 Author-email: gregor@muellegger.de
 License: BSD
 Description: ==================
         django-autofixture
```

### Comparing `django-autofixture-squad-0.12.2.dev1/django_autofixture_squad.egg-info/SOURCES.txt` & `django-autofixture-squad-0.12.3.dev1/django_autofixture_squad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

