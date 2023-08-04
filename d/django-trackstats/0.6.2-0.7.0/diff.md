# Comparing `tmp/django-trackstats-0.6.2.tar.gz` & `tmp/django-trackstats-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-trackstats-0.6.2.tar", last modified: Mon Mar 27 18:42:06 2023, max compression
+gzip compressed data, was "django-trackstats-0.7.0.tar", last modified: Fri Aug  4 12:20:26 2023, max compression
```

## Comparing `django-trackstats-0.6.2.tar` & `django-trackstats-0.7.0.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.495304 django-trackstats-0.6.2/
--rw-r--r--   0 pennersr  (1000) users      (100)      110 2023-02-15 15:08:14.000000 django-trackstats-0.6.2/AUTHORS
--rw-r--r--   0 pennersr  (1000) users      (100)     1098 2023-02-15 15:08:14.000000 django-trackstats-0.6.2/LICENSE
--rw-r--r--   0 pennersr  (1000) users      (100)       98 2023-02-15 15:08:14.000000 django-trackstats-0.6.2/MANIFEST.in
--rw-r--r--   0 pennersr  (1000) users      (100)     6633 2023-03-27 18:42:06.495304 django-trackstats-0.6.2/PKG-INFO
--rw-r--r--   0 pennersr  (1000) users      (100)     5745 2023-03-27 18:42:02.000000 django-trackstats-0.6.2/README.rst
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.494304 django-trackstats-0.6.2/django_trackstats.egg-info/
--rw-r--r--   0 pennersr  (1000) users      (100)     6633 2023-03-27 18:42:06.000000 django-trackstats-0.6.2/django_trackstats.egg-info/PKG-INFO
--rw-r--r--   0 pennersr  (1000) users      (100)     1162 2023-03-27 18:42:06.000000 django-trackstats-0.6.2/django_trackstats.egg-info/SOURCES.txt
--rw-r--r--   0 pennersr  (1000) users      (100)        1 2023-03-27 18:42:06.000000 django-trackstats-0.6.2/django_trackstats.egg-info/dependency_links.txt
--rw-r--r--   0 pennersr  (1000) users      (100)        1 2023-02-15 15:10:03.000000 django-trackstats-0.6.2/django_trackstats.egg-info/not-zip-safe
--rw-r--r--   0 pennersr  (1000) users      (100)       20 2023-03-27 18:42:06.000000 django-trackstats-0.6.2/django_trackstats.egg-info/requires.txt
--rw-r--r--   0 pennersr  (1000) users      (100)       11 2023-03-27 18:42:06.000000 django-trackstats-0.6.2/django_trackstats.egg-info/top_level.txt
--rw-r--r--   0 pennersr  (1000) users      (100)      110 2023-03-27 18:42:06.495304 django-trackstats-0.6.2/setup.cfg
--rw-r--r--   0 pennersr  (1000) users      (100)     2165 2023-03-27 18:42:02.000000 django-trackstats-0.6.2/setup.py
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.494304 django-trackstats-0.6.2/trackstats/
--rw-r--r--   0 pennersr  (1000) users      (100)      621 2023-03-27 18:42:02.000000 django-trackstats-0.6.2/trackstats/__init__.py
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.494304 django-trackstats-0.6.2/trackstats/admin/
--rw-r--r--   0 pennersr  (1000) users      (100)     3252 2023-03-27 18:42:02.000000 django-trackstats-0.6.2/trackstats/admin/__init__.py
--rw-r--r--   0 pennersr  (1000) users      (100)     1671 2023-02-15 15:24:07.000000 django-trackstats-0.6.2/trackstats/admin/forms.py
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.494304 django-trackstats-0.6.2/trackstats/migrations/
--rw-r--r--   0 pennersr  (1000) users      (100)     6004 2023-02-15 15:24:07.000000 django-trackstats-0.6.2/trackstats/migrations/0001_initial.py
--rw-r--r--   0 pennersr  (1000) users      (100)     1212 2023-02-15 15:22:17.000000 django-trackstats-0.6.2/trackstats/migrations/0002_alter_domain_id_alter_metric_id_and_more.py
--rw-r--r--   0 pennersr  (1000) users      (100)     1234 2023-03-27 18:42:02.000000 django-trackstats-0.6.2/trackstats/migrations/0003_alter_model_fields.py
--rw-r--r--   0 pennersr  (1000) users      (100)        0 2023-02-15 15:08:14.000000 django-trackstats-0.6.2/trackstats/migrations/__init__.py
--rw-r--r--   0 pennersr  (1000) users      (100)     7813 2023-03-27 18:42:02.000000 django-trackstats-0.6.2/trackstats/models.py
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.493304 django-trackstats-0.6.2/trackstats/static/
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.493304 django-trackstats-0.6.2/trackstats/static/trackstats/
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.494304 django-trackstats-0.6.2/trackstats/static/trackstats/css/
--rw-r--r--   0 pennersr  (1000) users      (100)       92 2023-02-15 15:08:14.000000 django-trackstats-0.6.2/trackstats/static/trackstats/css/admin.css
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.494304 django-trackstats-0.6.2/trackstats/static/trackstats/js/
--rw-r--r--   0 pennersr  (1000) users      (100)      636 2023-02-15 15:08:14.000000 django-trackstats-0.6.2/trackstats/static/trackstats/js/graphs.js
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.493304 django-trackstats-0.6.2/trackstats/templates/
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.493304 django-trackstats-0.6.2/trackstats/templates/trackstats/
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.494304 django-trackstats-0.6.2/trackstats/templates/trackstats/admin/
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.494304 django-trackstats-0.6.2/trackstats/templates/trackstats/admin/by_date/
--rw-r--r--   0 pennersr  (1000) users      (100)      220 2023-02-15 15:08:14.000000 django-trackstats-0.6.2/trackstats/templates/trackstats/admin/by_date/change_list.html
--rw-r--r--   0 pennersr  (1000) users      (100)       44 2023-02-15 15:08:14.000000 django-trackstats-0.6.2/trackstats/templates/trackstats/admin/by_date/graph.html
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.494304 django-trackstats-0.6.2/trackstats/templates/trackstats/admin/by_date_and_object/
--rw-r--r--   0 pennersr  (1000) users      (100)      231 2023-02-15 15:08:14.000000 django-trackstats-0.6.2/trackstats/templates/trackstats/admin/by_date_and_object/change_list.html
--rw-r--r--   0 pennersr  (1000) users      (100)      226 2023-02-15 15:08:14.000000 django-trackstats-0.6.2/trackstats/templates/trackstats/admin/by_date_and_object/graph.html
--rw-r--r--   0 pennersr  (1000) users      (100)     1298 2023-02-15 15:08:14.000000 django-trackstats-0.6.2/trackstats/templates/trackstats/admin/graph.html
-drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-03-27 18:42:06.495304 django-trackstats-0.6.2/trackstats/tests/
--rw-r--r--   0 pennersr  (1000) users      (100)        0 2023-02-15 15:08:14.000000 django-trackstats-0.6.2/trackstats/tests/__init__.py
--rw-r--r--   0 pennersr  (1000) users      (100)      221 2023-02-15 15:22:17.000000 django-trackstats-0.6.2/trackstats/tests/models.py
--rw-r--r--   0 pennersr  (1000) users      (100)      997 2023-02-15 15:21:52.000000 django-trackstats-0.6.2/trackstats/tests/settings.py
--rw-r--r--   0 pennersr  (1000) users      (100)     3130 2023-03-27 18:42:02.000000 django-trackstats-0.6.2/trackstats/tests/test_models.py
--rw-r--r--   0 pennersr  (1000) users      (100)     5028 2023-03-27 18:42:02.000000 django-trackstats-0.6.2/trackstats/tests/test_trackers.py
--rw-r--r--   0 pennersr  (1000) users      (100)     6987 2023-03-27 18:42:02.000000 django-trackstats-0.6.2/trackstats/trackers.py
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.674818 django-trackstats-0.7.0/
+-rw-r--r--   0 pennersr  (1000) users      (100)      110 2023-02-15 15:08:14.000000 django-trackstats-0.7.0/AUTHORS
+-rw-r--r--   0 pennersr  (1000) users      (100)     1098 2023-02-15 15:08:14.000000 django-trackstats-0.7.0/LICENSE
+-rw-r--r--   0 pennersr  (1000) users      (100)       98 2023-02-15 15:08:14.000000 django-trackstats-0.7.0/MANIFEST.in
+-rw-r--r--   0 pennersr  (1000) users      (100)     6633 2023-08-04 12:20:26.674818 django-trackstats-0.7.0/PKG-INFO
+-rw-r--r--   0 pennersr  (1000) users      (100)     5745 2023-03-27 18:42:02.000000 django-trackstats-0.7.0/README.rst
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.673818 django-trackstats-0.7.0/django_trackstats.egg-info/
+-rw-r--r--   0 pennersr  (1000) users      (100)     6633 2023-08-04 12:20:26.000000 django-trackstats-0.7.0/django_trackstats.egg-info/PKG-INFO
+-rw-r--r--   0 pennersr  (1000) users      (100)     1236 2023-08-04 12:20:26.000000 django-trackstats-0.7.0/django_trackstats.egg-info/SOURCES.txt
+-rw-r--r--   0 pennersr  (1000) users      (100)        1 2023-08-04 12:20:26.000000 django-trackstats-0.7.0/django_trackstats.egg-info/dependency_links.txt
+-rw-r--r--   0 pennersr  (1000) users      (100)        1 2023-02-15 15:10:03.000000 django-trackstats-0.7.0/django_trackstats.egg-info/not-zip-safe
+-rw-r--r--   0 pennersr  (1000) users      (100)       20 2023-08-04 12:20:26.000000 django-trackstats-0.7.0/django_trackstats.egg-info/requires.txt
+-rw-r--r--   0 pennersr  (1000) users      (100)       11 2023-08-04 12:20:26.000000 django-trackstats-0.7.0/django_trackstats.egg-info/top_level.txt
+-rw-r--r--   0 pennersr  (1000) users      (100)      110 2023-08-04 12:20:26.675818 django-trackstats-0.7.0/setup.cfg
+-rw-r--r--   0 pennersr  (1000) users      (100)     2165 2023-03-27 18:42:02.000000 django-trackstats-0.7.0/setup.py
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.673818 django-trackstats-0.7.0/trackstats/
+-rw-r--r--   0 pennersr  (1000) users      (100)      621 2023-08-04 12:18:12.000000 django-trackstats-0.7.0/trackstats/__init__.py
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.673818 django-trackstats-0.7.0/trackstats/admin/
+-rw-r--r--   0 pennersr  (1000) users      (100)     3252 2023-03-27 18:42:02.000000 django-trackstats-0.7.0/trackstats/admin/__init__.py
+-rw-r--r--   0 pennersr  (1000) users      (100)     1671 2023-02-15 15:24:07.000000 django-trackstats-0.7.0/trackstats/admin/forms.py
+-rw-r--r--   0 pennersr  (1000) users      (100)      184 2023-08-04 12:16:21.000000 django-trackstats-0.7.0/trackstats/apps.py
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.673818 django-trackstats-0.7.0/trackstats/migrations/
+-rw-r--r--   0 pennersr  (1000) users      (100)     6004 2023-02-15 15:24:07.000000 django-trackstats-0.7.0/trackstats/migrations/0001_initial.py
+-rw-r--r--   0 pennersr  (1000) users      (100)     1212 2023-02-15 15:22:17.000000 django-trackstats-0.7.0/trackstats/migrations/0002_alter_domain_id_alter_metric_id_and_more.py
+-rw-r--r--   0 pennersr  (1000) users      (100)     1234 2023-03-27 18:42:02.000000 django-trackstats-0.7.0/trackstats/migrations/0003_alter_model_fields.py
+-rw-r--r--   0 pennersr  (1000) users      (100)     1222 2023-08-04 12:16:21.000000 django-trackstats-0.7.0/trackstats/migrations/0004_alter_default_auto_field.py
+-rw-r--r--   0 pennersr  (1000) users      (100)        0 2023-02-15 15:08:14.000000 django-trackstats-0.7.0/trackstats/migrations/__init__.py
+-rw-r--r--   0 pennersr  (1000) users      (100)     7813 2023-03-27 18:42:02.000000 django-trackstats-0.7.0/trackstats/models.py
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.672818 django-trackstats-0.7.0/trackstats/static/
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.672818 django-trackstats-0.7.0/trackstats/static/trackstats/
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.673818 django-trackstats-0.7.0/trackstats/static/trackstats/css/
+-rw-r--r--   0 pennersr  (1000) users      (100)       92 2023-02-15 15:08:14.000000 django-trackstats-0.7.0/trackstats/static/trackstats/css/admin.css
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.673818 django-trackstats-0.7.0/trackstats/static/trackstats/js/
+-rw-r--r--   0 pennersr  (1000) users      (100)      636 2023-02-15 15:08:14.000000 django-trackstats-0.7.0/trackstats/static/trackstats/js/graphs.js
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.672818 django-trackstats-0.7.0/trackstats/templates/
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.672818 django-trackstats-0.7.0/trackstats/templates/trackstats/
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.674818 django-trackstats-0.7.0/trackstats/templates/trackstats/admin/
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.674818 django-trackstats-0.7.0/trackstats/templates/trackstats/admin/by_date/
+-rw-r--r--   0 pennersr  (1000) users      (100)      220 2023-02-15 15:08:14.000000 django-trackstats-0.7.0/trackstats/templates/trackstats/admin/by_date/change_list.html
+-rw-r--r--   0 pennersr  (1000) users      (100)       44 2023-02-15 15:08:14.000000 django-trackstats-0.7.0/trackstats/templates/trackstats/admin/by_date/graph.html
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.674818 django-trackstats-0.7.0/trackstats/templates/trackstats/admin/by_date_and_object/
+-rw-r--r--   0 pennersr  (1000) users      (100)      231 2023-02-15 15:08:14.000000 django-trackstats-0.7.0/trackstats/templates/trackstats/admin/by_date_and_object/change_list.html
+-rw-r--r--   0 pennersr  (1000) users      (100)      226 2023-02-15 15:08:14.000000 django-trackstats-0.7.0/trackstats/templates/trackstats/admin/by_date_and_object/graph.html
+-rw-r--r--   0 pennersr  (1000) users      (100)     1298 2023-02-15 15:08:14.000000 django-trackstats-0.7.0/trackstats/templates/trackstats/admin/graph.html
+drwxr-xr-x   0 pennersr  (1000) users      (100)        0 2023-08-04 12:20:26.674818 django-trackstats-0.7.0/trackstats/tests/
+-rw-r--r--   0 pennersr  (1000) users      (100)        0 2023-02-15 15:08:14.000000 django-trackstats-0.7.0/trackstats/tests/__init__.py
+-rw-r--r--   0 pennersr  (1000) users      (100)      221 2023-02-15 15:22:17.000000 django-trackstats-0.7.0/trackstats/tests/models.py
+-rw-r--r--   0 pennersr  (1000) users      (100)      997 2023-02-15 15:21:52.000000 django-trackstats-0.7.0/trackstats/tests/settings.py
+-rw-r--r--   0 pennersr  (1000) users      (100)     3130 2023-03-27 18:42:02.000000 django-trackstats-0.7.0/trackstats/tests/test_models.py
+-rw-r--r--   0 pennersr  (1000) users      (100)     5028 2023-03-27 18:42:02.000000 django-trackstats-0.7.0/trackstats/tests/test_trackers.py
+-rw-r--r--   0 pennersr  (1000) users      (100)     6987 2023-03-27 18:42:02.000000 django-trackstats-0.7.0/trackstats/trackers.py
```

### Comparing `django-trackstats-0.6.2/LICENSE` & `django-trackstats-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/PKG-INFO` & `django-trackstats-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-trackstats
-Version: 0.6.2
+Version: 0.7.0
 Summary: Statistics storage for Django
 Home-page: http://github.com/pennersr/django-trackstats
 Author: Raymond Penners
 Author-email: raymond.penners@intenct.nl
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-trackstats-0.6.2/README.rst` & `django-trackstats-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/django_trackstats.egg-info/PKG-INFO` & `django-trackstats-0.7.0/django_trackstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-trackstats
-Version: 0.6.2
+Version: 0.7.0
 Summary: Statistics storage for Django
 Home-page: http://github.com/pennersr/django-trackstats
 Author: Raymond Penners
 Author-email: raymond.penners@intenct.nl
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `django-trackstats-0.6.2/django_trackstats.egg-info/SOURCES.txt` & `django-trackstats-0.7.0/django_trackstats.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 django_trackstats.egg-info/PKG-INFO
 django_trackstats.egg-info/SOURCES.txt
 django_trackstats.egg-info/dependency_links.txt
 django_trackstats.egg-info/not-zip-safe
 django_trackstats.egg-info/requires.txt
 django_trackstats.egg-info/top_level.txt
 trackstats/__init__.py
+trackstats/apps.py
 trackstats/models.py
 trackstats/trackers.py
 trackstats/admin/__init__.py
 trackstats/admin/forms.py
 trackstats/migrations/0001_initial.py
 trackstats/migrations/0002_alter_domain_id_alter_metric_id_and_more.py
 trackstats/migrations/0003_alter_model_fields.py
+trackstats/migrations/0004_alter_default_auto_field.py
 trackstats/migrations/__init__.py
 trackstats/static/trackstats/css/admin.css
 trackstats/static/trackstats/js/graphs.js
 trackstats/templates/trackstats/admin/graph.html
 trackstats/templates/trackstats/admin/by_date/change_list.html
 trackstats/templates/trackstats/admin/by_date/graph.html
 trackstats/templates/trackstats/admin/by_date_and_object/change_list.html
```

### Comparing `django-trackstats-0.6.2/setup.py` & `django-trackstats-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/trackstats/__init__.py` & `django-trackstats-0.7.0/trackstats/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
   ______                __   _____ __        __
  /_  __/________ ______/ /__/ ___// /_____ _/ /______
   / / / ___/ __ `/ ___/ //_/\__ \/ __/ __ `/ __/ ___/
  / / / /  / /_/ / /__/ ,<  ___/ / /_/ /_/ / /_(__  )
 /_/ /_/   \__,_/\___/_/|_|/____/\__/\__,_/\__/____/
 
 """  # noqa
-VERSION = (0, 6, 2, "final", 0)
+VERSION = (0, 7, 0, "final", 0)
 
 __title__ = "django-trackstats"
 __version_info__ = VERSION
 __version__ = ".".join(map(str, VERSION[:3])) + (
     "-{}{}".format(VERSION[3], VERSION[4] or "") if VERSION[3] != "final" else ""
 )
 __author__ = "Raymond Penners"
```

### Comparing `django-trackstats-0.6.2/trackstats/admin/__init__.py` & `django-trackstats-0.7.0/trackstats/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/trackstats/admin/forms.py` & `django-trackstats-0.7.0/trackstats/admin/forms.py`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/trackstats/migrations/0001_initial.py` & `django-trackstats-0.7.0/trackstats/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/trackstats/migrations/0002_alter_domain_id_alter_metric_id_and_more.py` & `django-trackstats-0.7.0/trackstats/migrations/0002_alter_domain_id_alter_metric_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/trackstats/migrations/0003_alter_model_fields.py` & `django-trackstats-0.7.0/trackstats/migrations/0003_alter_model_fields.py`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/trackstats/models.py` & `django-trackstats-0.7.0/trackstats/models.py`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/trackstats/static/trackstats/js/graphs.js` & `django-trackstats-0.7.0/trackstats/static/trackstats/js/graphs.js`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/trackstats/templates/trackstats/admin/graph.html` & `django-trackstats-0.7.0/trackstats/templates/trackstats/admin/graph.html`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/trackstats/tests/settings.py` & `django-trackstats-0.7.0/trackstats/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/trackstats/tests/test_models.py` & `django-trackstats-0.7.0/trackstats/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/trackstats/tests/test_trackers.py` & `django-trackstats-0.7.0/trackstats/tests/test_trackers.py`

 * *Files identical despite different names*

### Comparing `django-trackstats-0.6.2/trackstats/trackers.py` & `django-trackstats-0.7.0/trackstats/trackers.py`

 * *Files identical despite different names*

