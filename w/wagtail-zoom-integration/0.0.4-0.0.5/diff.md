# Comparing `tmp/wagtail-zoom-integration-0.0.4.tar.gz` & `tmp/wagtail-zoom-integration-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-zoom-integration-0.0.4.tar", last modified: Thu May 25 20:14:20 2023, max compression
+gzip compressed data, was "wagtail-zoom-integration-0.0.5.tar", last modified: Fri Aug  4 14:46:36 2023, max compression
```

## Comparing `wagtail-zoom-integration-0.0.4.tar` & `wagtail-zoom-integration-0.0.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:20.097210 wagtail-zoom-integration-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-25 20:14:20.097210 wagtail-zoom-integration-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:20.093210 wagtail-zoom-integration-0.0.4/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:20.093210 wagtail-zoom-integration-0.0.4/sandbox/home/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/home/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:20.093210 wagtail-zoom-integration-0.0.4/sandbox/home/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/home/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/home/migrations/0002_create_homepage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/home/migrations/0003_eventregistrationpage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/home/migrations/0004_formfield.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/home/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/home/models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:20.093210 wagtail-zoom-integration-0.0.4/sandbox/sandbox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:20.093210 wagtail-zoom-integration-0.0.4/sandbox/sandbox/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/sandbox/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/sandbox/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/sandbox/settings/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/sandbox/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/sandbox/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/sandbox/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:20.093210 wagtail-zoom-integration-0.0.4/sandbox/search/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/sandbox/search/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-25 20:14:20.097210 wagtail-zoom-integration-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:20.093210 wagtail-zoom-integration-0.0.4/wagtail_zoom_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-25 20:14:20.000000 wagtail-zoom-integration-0.0.4/wagtail_zoom_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-05-25 20:14:20.000000 wagtail-zoom-integration-0.0.4/wagtail_zoom_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:14:20.000000 wagtail-zoom-integration-0.0.4/wagtail_zoom_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 20:14:20.000000 wagtail-zoom-integration-0.0.4/wagtail_zoom_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 20:14:20.000000 wagtail-zoom-integration-0.0.4/wagtail_zoom_integration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:20.097210 wagtail-zoom-integration-0.0.4/wagtailzoom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:20.097210 wagtail-zoom-integration-0.0.4/wagtailzoom/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:20.089210 wagtail-zoom-integration-0.0.4/wagtailzoom/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:20.097210 wagtail-zoom-integration-0.0.4/wagtailzoom/templates/wagtailzoom/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:14:20.097210 wagtail-zoom-integration-0.0.4/wagtailzoom/templates/wagtailzoom/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-05-25 20:14:04.000000 wagtail-zoom-integration-0.0.4/wagtailzoom/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.858104 wagtail-zoom-integration-0.0.5/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.858104 wagtail-zoom-integration-0.0.5/sandbox/home/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.858104 wagtail-zoom-integration-0.0.5/sandbox/home/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0002_create_homepage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0003_eventregistrationpage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0004_formfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/home/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      254 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.858104 wagtail-zoom-integration-0.0.5/sandbox/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/sandbox/sandbox/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/settings/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/sandbox/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/sandbox/search/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/sandbox/search/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-08-04 14:46:36.000000 wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-08-04 14:46:36.000000 wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:46:36.000000 wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-04 14:46:36.000000 wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-04 14:46:36.000000 wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/wagtailzoom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/wagtailzoom/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.858104 wagtail-zoom-integration-0.0.5/wagtailzoom/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:46:36.862104 wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-08-04 14:46:21.000000 wagtail-zoom-integration-0.0.5/wagtailzoom/widgets.py
```

### Comparing `wagtail-zoom-integration-0.0.4/PKG-INFO` & `wagtail-zoom-integration-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-zoom-integration
-Version: 0.0.4
+Version: 0.0.5
 Summary: Integrate Zoom Event registration registration in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/wagtail-zoom-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-zoom-integration-0.0.4/README.md` & `wagtail-zoom-integration-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/sandbox/home/migrations/0001_initial.py` & `wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/sandbox/home/migrations/0002_create_homepage.py` & `wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/sandbox/home/migrations/0003_eventregistrationpage.py` & `wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0003_eventregistrationpage.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/sandbox/home/migrations/0004_formfield.py` & `wagtail-zoom-integration-0.0.5/sandbox/home/migrations/0004_formfield.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/sandbox/home/models.py` & `wagtail-zoom-integration-0.0.5/sandbox/home/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/sandbox/sandbox/settings/base.py` & `wagtail-zoom-integration-0.0.5/sandbox/sandbox/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/sandbox/sandbox/urls.py` & `wagtail-zoom-integration-0.0.5/sandbox/sandbox/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/sandbox/search/views.py` & `wagtail-zoom-integration-0.0.5/sandbox/search/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/setup.cfg` & `wagtail-zoom-integration-0.0.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-zoom-integration
-version = 0.0.4
+version = 0.0.5
 description = Integrate Zoom Event registration registration in Wagtail Projects.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/wmo-raf/wagtail-zoom-integration
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
```

### Comparing `wagtail-zoom-integration-0.0.4/wagtail_zoom_integration.egg-info/PKG-INFO` & `wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-zoom-integration
-Version: 0.0.4
+Version: 0.0.5
 Summary: Integrate Zoom Event registration registration in Wagtail Projects.
 Home-page: https://github.com/wmo-raf/wagtail-zoom-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `wagtail-zoom-integration-0.0.4/wagtail_zoom_integration.egg-info/SOURCES.txt` & `wagtail-zoom-integration-0.0.5/wagtail_zoom_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/wagtailzoom/api.py` & `wagtail-zoom-integration-0.0.5/wagtailzoom/api.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/wagtailzoom/forms.py` & `wagtail-zoom-integration-0.0.5/wagtailzoom/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/wagtailzoom/migrations/0001_initial.py` & `wagtail-zoom-integration-0.0.5/wagtailzoom/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/wagtailzoom/models.py` & `wagtail-zoom-integration-0.0.5/wagtailzoom/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 import json
 
 from django.core.mail import mail_admins
 from django.db import models
 from django.template import Context, Template
-from django.template.response import TemplateResponse
-from django.utils.decorators import method_decorator
 from django.utils.translation import gettext as _
-from django.views.decorators.csrf import csrf_exempt
 from wagtail.admin.panels import FieldPanel
 from wagtail.contrib.forms.models import AbstractForm
 from wagtail.contrib.settings.models import BaseSiteSetting
 from wagtail.contrib.settings.registry import register_setting
 
 from .api import ZoomApi
 from .widgets import ZoomEventSelectWidget
@@ -50,30 +47,30 @@
     is_zoom_integration = True
 
     class Meta:
         abstract = True
 
     @property
     def zoom_event_id(self):
-        return self.get_data().get("event_id")
+        return self.get_zoom_data().get("event_id")
 
     @property
     def zoom_event_type(self):
-        return self.get_data().get("event_type")
+        return self.get_zoom_data().get("event_type")
 
     @property
     def zoom_merge_fields(self):
         if self.zoom_reg_fields_mapping:
             try:
                 return json.loads(self.zoom_reg_fields_mapping)
             except Exception:
                 pass
         return {}
 
-    def get_data(self):
+    def get_zoom_data(self):
         data = {}
         if self.zoom_event:
             try:
                 event = json.loads(self.zoom_event)
 
                 if event:
                     data.update({
@@ -82,56 +79,35 @@
                         "event_topic": event.get("event_topic")
                     })
             except Exception:
                 pass
 
         return data
 
-    def post_process_submission(self, form, form_submission):
-        pass
-
-    def process_form_submission(self, form, request=None):
+    def process_form_submission(self, form):
         form_submission = super(AbstractZoomIntegrationForm, self).process_form_submission(form)
-        try:
-            self.post_process_submission(form, form_submission)
-        except Exception as e:
-            pass
 
-        return form_submission
+        if self.request:
+            self.zoom_integration_operation(self, form=form, request=self.request)
 
-    def should_process_form(self, request, form_data):
-        return True
+        return form_submission
 
-    @method_decorator(csrf_exempt)
     def serve(self, request, *args, **kwargs):
-        if request.method == 'POST':
-            form = self.get_form(request.POST, request.FILES, page=self, user=request.user)
-
-            if form.is_valid():
-                form_submission = None
-                if self.should_process_form(request, form.cleaned_data):
-                    form_submission = self.process_form_submission(form)
-                    self.integration_operation(self, form=form, request=request)
-
-                # render landing page
-                return self.render_landing_page(request, form_submission, *args, **kwargs)
-
-        form = self.get_form(page=self, user=request.user)
-        context = self.get_context(request)
-        context['form'] = form
+        # We need to access the request later on in integration operation
+        self.request = request
 
-        return TemplateResponse(request, self.get_template(request), context)
+        return super(AbstractZoomIntegrationForm, self).serve(request, *args, **kwargs)
 
     def format_zoom_form_submission(self, form):
         formatted_form_data = {}
         for k, v in form.cleaned_data.items():
             formatted_form_data[k.replace('-', '_')] = v
         return formatted_form_data
 
-    def integration_operation(self, instance, **kwargs):
+    def zoom_integration_operation(self, instance, **kwargs):
         success = False
         response = None
         request = kwargs.get('request', None)
 
         if self.zoom_event_id and self.zoom_merge_fields:
             try:
                 zoom_settings = ZoomSettings.for_request(request)
@@ -149,34 +125,34 @@
                     response = zoom.add_webinar_registrant(self.zoom_event_id, dict_data)
                 # mark as success
                 success = True
             except Exception as e:
                 # mark as failed
                 success = False
 
-                data = json.dumps(self.get_data())
+                data = json.dumps(self.get_zoom_data())
 
                 message = "Error \n {}\n  Rendered \n {}\n Zoom Form Data\n {}".format(str(e),
                                                                                        str(rendered_dictionary),
                                                                                        str(data))
                 mail_admins(subject="Error adding user to zoom event", message=message)
 
         return success, response
 
-    def get_merge_fields_template(self):
+    def get_zoom_fields_template(self):
         fields = self.zoom_merge_fields
 
         for key, value in fields.items():
             if value:
                 fields[key] = "{}{}{}".format("{{", value, "}}")
         return fields
 
     def render_zoom_dictionary(self, form_submission):
 
-        merge_fields_templates = self.get_merge_fields_template()
+        fields_templates = self.get_zoom_fields_template()
 
         rendered_dictionary_template = json.dumps({
-            **merge_fields_templates,
+            **fields_templates,
         })
 
         rendered_dictionary = Template(rendered_dictionary_template).render(Context(form_submission))
         return rendered_dictionary
```

### Comparing `wagtail-zoom-integration-0.0.4/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html` & `wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html` & `wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html` & `wagtail-zoom-integration-0.0.5/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/wagtailzoom/views.py` & `wagtail-zoom-integration-0.0.5/wagtailzoom/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/wagtailzoom/wagtail_hooks.py` & `wagtail-zoom-integration-0.0.5/wagtailzoom/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-zoom-integration-0.0.4/wagtailzoom/widgets.py` & `wagtail-zoom-integration-0.0.5/wagtailzoom/widgets.py`

 * *Files identical despite different names*

