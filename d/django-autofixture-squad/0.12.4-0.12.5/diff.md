# Comparing `tmp/django-autofixture-squad-0.12.4.tar.gz` & `tmp/django-autofixture-squad-0.12.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-autofixture-squad-0.12.4.tar", last modified: Fri Aug  4 10:17:41 2023, max compression
+gzip compressed data, was "dist/django-autofixture-squad-0.12.5.tar", last modified: Fri Aug  4 10:23:11 2023, max compression
```

## Comparing `django-autofixture-squad-0.12.4.tar` & `django-autofixture-squad-0.12.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:17:41.000000 django-autofixture-squad-0.12.4/
--rw-r--r--   0 root         (0) root         (0)    18665 2023-08-04 10:17:41.000000 django-autofixture-squad-0.12.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       99 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:17:41.000000 django-autofixture-squad-0.12.4/autofixture/
--rw-r--r--   0 root         (0) root         (0)     1389 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/autofixture/placeholder.py
--rw-r--r--   0 root         (0) root         (0)      138 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/autofixture/signals.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/autofixture/values.py
--rw-r--r--   0 root         (0) root         (0)     1862 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/autofixture/compat.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 10:11:50.000000 django-autofixture-squad-0.12.4/autofixture/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 10:14:00.000000 django-autofixture-squad-0.12.4/autofixture/fields.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:17:41.000000 django-autofixture-squad-0.12.4/autofixture/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/autofixture/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:17:41.000000 django-autofixture-squad-0.12.4/autofixture/management/commands/
--rw-r--r--   0 root         (0) root         (0)     9757 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/autofixture/management/commands/loadtestdata.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/autofixture/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7966 2023-08-04 10:14:00.000000 django-autofixture-squad-0.12.4/autofixture/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21938 2023-08-04 08:10:24.000000 django-autofixture-squad-0.12.4/autofixture/generators.py
--rw-r--r--   0 root         (0) root         (0)     3399 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/autofixture/autofixtures.py
--rw-r--r--   0 root         (0) root         (0)     2130 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/autofixture/constraints.py
--rw-r--r--   0 root         (0) root         (0)    23073 2023-08-04 10:14:00.000000 django-autofixture-squad-0.12.4/autofixture/base.py
--rwxr-xr-x   0 root         (0) root         (0)     2384 2023-08-04 08:10:24.000000 django-autofixture-squad-0.12.4/setup.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 10:17:41.000000 django-autofixture-squad-0.12.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8857 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/README.rst
--rw-r--r--   0 root         (0) root         (0)     1515 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      810 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/AUTHORS.txt
--rw-r--r--   0 root         (0) root         (0)     5310 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.4/CHANGES.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:17:41.000000 django-autofixture-squad-0.12.4/django_autofixture_squad.egg-info/
--rw-r--r--   0 root         (0) root         (0)    18665 2023-08-04 10:17:41.000000 django-autofixture-squad-0.12.4/django_autofixture_squad.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      696 2023-08-04 10:17:41.000000 django-autofixture-squad-0.12.4/django_autofixture_squad.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-08-04 10:17:41.000000 django-autofixture-squad-0.12.4/django_autofixture_squad.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-08-04 10:17:41.000000 django-autofixture-squad-0.12.4/django_autofixture_squad.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 10:17:41.000000 django-autofixture-squad-0.12.4/django_autofixture_squad.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:23:11.000000 django-autofixture-squad-0.12.5/
+-rw-r--r--   0 root         (0) root         (0)    18665 2023-08-04 10:23:11.000000 django-autofixture-squad-0.12.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       99 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:23:11.000000 django-autofixture-squad-0.12.5/autofixture/
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/autofixture/placeholder.py
+-rw-r--r--   0 root         (0) root         (0)      138 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/autofixture/signals.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/autofixture/values.py
+-rw-r--r--   0 root         (0) root         (0)     1862 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/autofixture/compat.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 10:11:50.000000 django-autofixture-squad-0.12.5/autofixture/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 10:14:00.000000 django-autofixture-squad-0.12.5/autofixture/fields.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:23:11.000000 django-autofixture-squad-0.12.5/autofixture/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/autofixture/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:23:11.000000 django-autofixture-squad-0.12.5/autofixture/management/commands/
+-rw-r--r--   0 root         (0) root         (0)     9757 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/autofixture/management/commands/loadtestdata.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/autofixture/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7966 2023-08-04 10:23:09.000000 django-autofixture-squad-0.12.5/autofixture/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21938 2023-08-04 08:10:24.000000 django-autofixture-squad-0.12.5/autofixture/generators.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/autofixture/autofixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/autofixture/constraints.py
+-rw-r--r--   0 root         (0) root         (0)    23137 2023-08-04 10:22:55.000000 django-autofixture-squad-0.12.5/autofixture/base.py
+-rwxr-xr-x   0 root         (0) root         (0)     2384 2023-08-04 08:10:24.000000 django-autofixture-squad-0.12.5/setup.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 10:23:11.000000 django-autofixture-squad-0.12.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8857 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      810 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/AUTHORS.txt
+-rw-r--r--   0 root         (0) root         (0)     5310 2023-08-04 06:35:12.000000 django-autofixture-squad-0.12.5/CHANGES.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 10:23:11.000000 django-autofixture-squad-0.12.5/django_autofixture_squad.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    18665 2023-08-04 10:23:11.000000 django-autofixture-squad-0.12.5/django_autofixture_squad.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      696 2023-08-04 10:23:11.000000 django-autofixture-squad-0.12.5/django_autofixture_squad.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-04 10:23:11.000000 django-autofixture-squad-0.12.5/django_autofixture_squad.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-08-04 10:23:11.000000 django-autofixture-squad-0.12.5/django_autofixture_squad.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 10:23:11.000000 django-autofixture-squad-0.12.5/django_autofixture_squad.egg-info/dependency_links.txt
```

### Comparing `django-autofixture-squad-0.12.4/PKG-INFO` & `django-autofixture-squad-0.12.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-autofixture-squad
-Version: 0.12.4
+Version: 0.12.5
 Summary: Provides tools to auto generate test data.
 Home-page: https://github.com/squadrun/django-autofixture
 Author: Gregor Müllegger
 Author-email: gregor@muellegger.de
 License: BSD
 Description: ==================
         django-autofixture
```

### Comparing `django-autofixture-squad-0.12.4/autofixture/placeholder.py` & `django-autofixture-squad-0.12.5/autofixture/placeholder.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.4/autofixture/values.py` & `django-autofixture-squad-0.12.5/autofixture/values.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.4/autofixture/compat.py` & `django-autofixture-squad-0.12.5/autofixture/compat.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.4/autofixture/management/commands/loadtestdata.py` & `django-autofixture-squad-0.12.5/autofixture/management/commands/loadtestdata.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.4/autofixture/__init__.py` & `django-autofixture-squad-0.12.5/autofixture/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 if sys.version_info[0] < 3:
     string_types = basestring
 else:
     string_types = str
 
 
-__version__ = '0.12.4'
+__version__ = '0.12.5'
 
 
 REGISTRY = {}
 
 
 def register(model, autofixture, overwrite=False, fail_silently=False):
     '''
```

### Comparing `django-autofixture-squad-0.12.4/autofixture/generators.py` & `django-autofixture-squad-0.12.5/autofixture/generators.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.4/autofixture/autofixtures.py` & `django-autofixture-squad-0.12.5/autofixture/autofixtures.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.4/autofixture/constraints.py` & `django-autofixture-squad-0.12.5/autofixture/constraints.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.4/autofixture/base.py` & `django-autofixture-squad-0.12.5/autofixture/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,14 +271,17 @@
         if (
             field.default is not fields.NOT_PROVIDED and
             not self.overwrite_defaults and
             field.name not in self.field_values):
                 return None
         kwargs = {}
 
+        if "SRPatchedJSONField" in str(field.__class__):
+            return generators.SRPatchedJSONFieldGenerator()
+
         if field.name in self.field_values:
             value = self.field_values[field.name]
             if isinstance(value, generators.Generator):
                 return value
             elif isinstance(value, AutoFixture):
                 return generators.InstanceGenerator(autofixture=value)
             elif callable(value):
@@ -380,15 +383,15 @@
         if hasattr(fields, 'BigIntegerField'):
             if isinstance(field, fields.BigIntegerField):
                 return generators.IntegerGenerator(
                     min_value=-field.MAX_BIGINT - 1,
                     max_value=field.MAX_BIGINT,
                     **kwargs)
         if isinstance(field, ImageField):
-            return generators.ImageGenerator(storage=field.storage, **kwargs)
+            return None
         for field_class, generator in self.field_to_generator.items():
             if isinstance(field, field_class):
                 return generator(**kwargs)
         return None
 
     def get_value(self, field):
         '''
```

### Comparing `django-autofixture-squad-0.12.4/setup.py` & `django-autofixture-squad-0.12.5/setup.py`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.4/README.rst` & `django-autofixture-squad-0.12.5/README.rst`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.4/LICENSE.txt` & `django-autofixture-squad-0.12.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.4/AUTHORS.txt` & `django-autofixture-squad-0.12.5/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.4/CHANGES.rst` & `django-autofixture-squad-0.12.5/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `django-autofixture-squad-0.12.4/django_autofixture_squad.egg-info/PKG-INFO` & `django-autofixture-squad-0.12.5/django_autofixture_squad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: django-autofixture-squad
-Version: 0.12.4
+Version: 0.12.5
 Summary: Provides tools to auto generate test data.
 Home-page: https://github.com/squadrun/django-autofixture
 Author: Gregor Müllegger
 Author-email: gregor@muellegger.de
 License: BSD
 Description: ==================
         django-autofixture
```

### Comparing `django-autofixture-squad-0.12.4/django_autofixture_squad.egg-info/SOURCES.txt` & `django-autofixture-squad-0.12.5/django_autofixture_squad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

