# Comparing `tmp/django-tenants-celery-beat-0.2.0.tar.gz` & `tmp/django-tenants-celery-beat-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-tenants-celery-beat-0.2.0.tar", last modified: Thu Sep 22 08:54:14 2022, max compression
+gzip compressed data, was "django-tenants-celery-beat-0.2.1.tar", last modified: Fri Aug  4 09:35:16 2023, max compression
```

## Comparing `django-tenants-celery-beat-0.2.0.tar` & `django-tenants-celery-beat-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 08:54:14.403651 django-tenants-celery-beat-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-09-22 08:54:00.000000 django-tenants-celery-beat-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-09-22 08:54:00.000000 django-tenants-celery-beat-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9691 2022-09-22 08:54:14.403651 django-tenants-celery-beat-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8804 2022-09-22 08:54:00.000000 django-tenants-celery-beat-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 08:54:14.403651 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 08:54:00.000000 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2571 2022-09-22 08:54:00.000000 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-09-22 08:54:00.000000 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 08:54:14.403651 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-22 08:54:00.000000 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3881 2022-09-22 08:54:00.000000 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     3234 2022-09-22 08:54:00.000000 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-22 08:54:14.403651 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9691 2022-09-22 08:54:14.000000 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      520 2022-09-22 08:54:14.000000 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-22 08:54:14.000000 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-09-22 08:54:14.000000 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-09-22 08:54:14.000000 django-tenants-celery-beat-0.2.0/django_tenants_celery_beat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-22 08:54:14.403651 django-tenants-celery-beat-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1379 2022-09-22 08:54:00.000000 django-tenants-celery-beat-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:35:16.152179 django-tenants-celery-beat-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-04 09:35:05.000000 django-tenants-celery-beat-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-04 09:35:05.000000 django-tenants-celery-beat-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-08-04 09:35:16.152179 django-tenants-celery-beat-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-08-04 09:35:05.000000 django-tenants-celery-beat-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:35:16.148179 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:35:05.000000 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-08-04 09:35:05.000000 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-08-04 09:35:05.000000 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:35:16.148179 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:35:05.000000 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3946 2023-08-04 09:35:05.000000 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-08-04 09:35:05.000000 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:35:16.148179 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9691 2023-08-04 09:35:16.000000 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-08-04 09:35:16.000000 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:35:16.000000 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-04 09:35:16.000000 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 09:35:16.000000 django-tenants-celery-beat-0.2.1/django_tenants_celery_beat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 09:35:16.152179 django-tenants-celery-beat-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-04 09:35:05.000000 django-tenants-celery-beat-0.2.1/setup.py
```

### Comparing `django-tenants-celery-beat-0.2.0/LICENSE` & `django-tenants-celery-beat-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-tenants-celery-beat-0.2.0/PKG-INFO` & `django-tenants-celery-beat-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tenants-celery-beat
-Version: 0.2.0
+Version: 0.2.1
 Summary: Support for celery beat in multitenant Django projects
 Home-page: https://github.com/QuickRelease/django-tenants-celery-beat
 Author: David Vaughan
 Author-email: david.vaughan@quickrelease.co.uk
 Maintainer: Quick Release (Automotive) Ltd.
 License: MIT
 Keywords: django tenants celery beat multitenancy postgres postgresql
```

### Comparing `django-tenants-celery-beat-0.2.0/README.md` & `django-tenants-celery-beat-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `django-tenants-celery-beat-0.2.0/django_tenants_celery_beat/admin.py` & `django-tenants-celery-beat-0.2.1/django_tenants_celery_beat/admin.py`

 * *Files identical despite different names*

### Comparing `django-tenants-celery-beat-0.2.0/django_tenants_celery_beat/models.py` & `django-tenants-celery-beat-0.2.1/django_tenants_celery_beat/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 import timezone_field
 
 from django.conf import settings
 from django_tenants.utils import get_tenant_model, get_public_schema_name
 from django_tenants_celery_beat.utils import get_periodic_task_tenant_link_model
 
 
-class TenantTimezoneMixin(models.Model):
-    timezone = timezone_field.TimeZoneField(
-        default="UTC",
-        display_GMT_offset=getattr(
-            settings, "TENANT_TIMEZONE_DISPLAY_GMT_OFFSET", False
-        ),
-    )
 
+timezone_field_kwargs = {
+    "default": "UTC",
+}
+if getattr(settings, "TENANT_TIMEZONE_DISPLAY_GMT_OFFSET", False):
+    timezone_field_kwargs["choices_display"] = "WITH_GMT_OFFSET"
+
+class TenantTimezoneMixin(models.Model):
+    timezone = timezone_field.TimeZoneField(**timezone_field_kwargs)
     class Meta:
         abstract = True
 
 
 class PeriodicTaskTenantLinkMixin(models.Model):
     tenant = models.ForeignKey(
         settings.TENANT_MODEL,
```

### Comparing `django-tenants-celery-beat-0.2.0/django_tenants_celery_beat/utils.py` & `django-tenants-celery-beat-0.2.1/django_tenants_celery_beat/utils.py`

 * *Files identical despite different names*

### Comparing `django-tenants-celery-beat-0.2.0/django_tenants_celery_beat.egg-info/PKG-INFO` & `django-tenants-celery-beat-0.2.1/django_tenants_celery_beat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-tenants-celery-beat
-Version: 0.2.0
+Version: 0.2.1
 Summary: Support for celery beat in multitenant Django projects
 Home-page: https://github.com/QuickRelease/django-tenants-celery-beat
 Author: David Vaughan
 Author-email: david.vaughan@quickrelease.co.uk
 Maintainer: Quick Release (Automotive) Ltd.
 License: MIT
 Keywords: django tenants celery beat multitenancy postgres postgresql
```

### Comparing `django-tenants-celery-beat-0.2.0/django_tenants_celery_beat.egg-info/SOURCES.txt` & `django-tenants-celery-beat-0.2.1/django_tenants_celery_beat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-tenants-celery-beat-0.2.0/setup.py` & `django-tenants-celery-beat-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="django-tenants-celery-beat",
-    version="0.2.0",
+    version="0.2.1",
     author="David Vaughan",
     author_email="david.vaughan@quickrelease.co.uk",
     maintainer="Quick Release (Automotive) Ltd.",
     description="Support for celery beat in multitenant Django projects",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/QuickRelease/django-tenants-celery-beat",
```

