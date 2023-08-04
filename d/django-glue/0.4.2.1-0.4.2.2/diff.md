# Comparing `tmp/django-glue-0.4.2.1.tar.gz` & `tmp/django-glue-0.4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-glue-0.4.2.1.tar", last modified: Thu Aug  3 16:58:27 2023, max compression
+gzip compressed data, was "django-glue-0.4.2.2.tar", last modified: Fri Aug  4 18:23:43 2023, max compression
```

## Comparing `django-glue-0.4.2.1.tar` & `django-glue-0.4.2.2.tar`

### file list

```diff
@@ -1,76 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.960915 django-glue-0.4.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/CONTRIBUTORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-03 16:58:27.960915 django-glue-0.4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.952915 django-glue-0.4.2.1/django_glue/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.956915 django-glue-0.4.2.1/django_glue/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/responses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.956915 django-glue-0.4.2.1/django_glue/services/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/services/model_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/services/query_sets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/services/services.py
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/services/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     5738 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.948915 django-glue-0.4.2.1/django_glue/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.948915 django-glue-0.4.2.1/django_glue/static/django_glue/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.956915 django-glue-0.4.2.1/django_glue/static/django_glue/js/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_ajax.js
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_csrf.js
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_event.js
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_keep_live.js
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_message.js
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_model_object.js
--rw-r--r--   0 runner    (1001) docker     (123)     4182 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_query_set.js
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_response.js
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_shortcuts.js
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_template.js
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_utils.js
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_view.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.948915 django-glue-0.4.2.1/django_glue/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.956915 django-glue-0.4.2.1/django_glue/templates/django_glue/
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/templates/django_glue/django_glue.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.956915 django-glue-0.4.2.1/django_glue/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/templatetags/django_glue.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/django_glue/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.952915 django-glue-0.4.2.1/django_glue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-03 16:58:27.000000 django-glue-0.4.2.1/django_glue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-08-03 16:58:27.000000 django-glue-0.4.2.1/django_glue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:58:27.000000 django-glue-0.4.2.1/django_glue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 16:58:27.000000 django-glue-0.4.2.1/django_glue.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 16:58:27.000000 django-glue-0.4.2.1/django_glue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-03 16:58:27.000000 django-glue-0.4.2.1/django_glue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-03 16:58:27.960915 django-glue-0.4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.960915 django-glue-0.4.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:27.960915 django-glue-0.4.2.1/tests/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-03 16:58:17.000000 django-glue-0.4.2.1/tests/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.483816 django-glue-0.4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/CONTRIBUTORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-04 18:23:43.483816 django-glue-0.4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3026 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/responses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/services/model_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/services/query_sets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/services/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.475816 django-glue-0.4.2.2/django_glue/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.475816 django-glue-0.4.2.2/django_glue/static/django_glue/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue/static/django_glue/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_ajax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_csrf.js
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_event.js
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_keep_live.js
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_message.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_model_object.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_query_set.js
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_response.js
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_shortcuts.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_template.js
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_utils.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_view.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.475816 django-glue-0.4.2.2/django_glue/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue/templates/django_glue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/templates/django_glue/django_glue.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/templatetags/django_glue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/django_glue/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/django_glue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-08-04 18:23:43.000000 django-glue-0.4.2.2/django_glue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-08-04 18:23:43.000000 django-glue-0.4.2.2/django_glue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 18:23:43.000000 django-glue-0.4.2.2/django_glue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 18:23:43.000000 django-glue-0.4.2.2/django_glue.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 18:23:43.000000 django-glue-0.4.2.2/django_glue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 18:23:43.000000 django-glue-0.4.2.2/django_glue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-04 18:23:43.483816 django-glue-0.4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:43.479816 django-glue-0.4.2.2/tests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-04 18:23:34.000000 django-glue-0.4.2.2/tests/wsgi.py
```

### Comparing `django-glue-0.4.2.1/CHANGELOG.md` & `django-glue-0.4.2.2/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 # Changelog for Django Glue
 
+## 0.4.2.2
+
+### Changes
+- Foreign Key fields now work with glue.
+- Move validation logic from Glue Request Handler to View.  
+
+
+
 ## 0.4.2.1
 
 ### Changes
 - Model default values now work with glue.
 
 ## 0.4.2
```

### Comparing `django-glue-0.4.2.1/LICENSE.md` & `django-glue-0.4.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/PKG-INFO` & `django-glue-0.4.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.4.2.1
+Version: 0.4.2.2
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-glue-0.4.2.1/README.md` & `django-glue-0.4.2.2/README.md`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/django_glue/context_processors.py` & `django-glue-0.4.2.2/django_glue/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/django_glue/data_classes.py` & `django-glue-0.4.2.2/django_glue/data_classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -85,14 +85,18 @@
 
     def to_dict(self) -> dict:
         return asdict(self)
 
 
 @dataclass
 class GlueMetaData:
+    """
+        # Todo: Should this handle both queryset and models? Should this be split into two classes?
+        This class is used to store meta data about the model or query set.
+    """
     app_label: str = None
     model: str = None
     object_pk: int = None
     query_set_str: str = None
     template: str = None
     fields: Union[list, tuple] = None
     exclude: Union[list, tuple] = None
```

### Comparing `django-glue-0.4.2.1/django_glue/enums.py` & `django-glue-0.4.2.2/django_glue/enums.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/django_glue/glue.py` & `django-glue-0.4.2.2/django_glue/glue.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/django_glue/handlers.py` & `django-glue-0.4.2.2/django_glue/handlers.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,71 +4,53 @@
 from django_glue.responses import generate_json_404_response
 from django_glue.services.templates import GlueTemplateService
 from django_glue.sessions import GlueSession
 from django_glue.data_classes import GlueMetaData, GlueBodyData
 from django_glue.enums import GlueConnection, GlueAccess
 
 
-class GlueDataRequestHandler:
-    def __init__(self, request):
-        self.request = request
-
-        self.is_valid_request = True
-
-        if request.content_type == 'application/json' or request.content_type == 'text/html':
-            logging.warning(request.body.decode('utf-8'))
-            self.body_data = GlueBodyData(request.body)
-        else:
-            self.is_valid_request = False
-
-        self.unique_name = self.body_data['unique_name']
+class GlueRequestHandler:
+    """
+        This class parses the request, determines the type of request, and then calls the appropriate service.
+    """
+    def __init__(self, glue_session: GlueSession, glue_body_data: GlueBodyData):
+        self.glue_session = glue_session
+        self.glue_body_data = glue_body_data
 
-        self.glue_session = GlueSession(request)
+        self.unique_name = self.glue_body_data['unique_name']
         self.context = self.glue_session['context']
-        self.method = request.method
 
-        if self.unique_name in self.context:
+        self.meta_data: GlueMetaData = GlueMetaData(
+            **self.glue_session['meta'][self.unique_name]
+        )
 
-            self.meta_data: GlueMetaData = GlueMetaData(
-                **self.glue_session['meta'][self.unique_name]
-            )
+        self.connection = GlueConnection(self.context[self.unique_name]['connection'])
+        self.access = GlueAccess(self.context[self.unique_name]['access'])
 
-            self.connection = GlueConnection(self.context[self.unique_name]['connection'])
+    def process_response(self):
 
-            self.access = GlueAccess(self.context[self.unique_name]['access'])
+        if self.connection == GlueConnection.MODEL_OBJECT:
+            glue_model_object_service = GlueModelObjectService(
+                self.meta_data,
+            )
 
-        else:
-            self.is_valid_request = False
+            json_response_data = glue_model_object_service.process_body_data(self.access, self.glue_body_data)
+            return json_response_data.to_django_json_response()
 
-        logging.warning(f'{self.is_valid_request = }')
+        elif self.connection == GlueConnection.QUERY_SET:
+            glue_query_set_service = GlueQuerySetService(
+                self.meta_data,
+            )
 
-    def process_response(self):
-        if self.method == 'QUERY' and self.is_valid_request:
-            if self.connection == GlueConnection.MODEL_OBJECT:
-                glue_model_object_service = GlueModelObjectService(
-                    self.meta_data,
-                )
-
-                json_response_data = glue_model_object_service.process_body_data(self.access, self.body_data)
-                return json_response_data.to_django_json_response()
-
-            elif self.connection == GlueConnection.QUERY_SET:
-                glue_query_set_service = GlueQuerySetService(
-                    self.meta_data,
-                )
-
-                json_response_data = glue_query_set_service.process_body_data(self.access, self.body_data)
-                return json_response_data.to_django_json_response()
-
-            elif self.connection == GlueConnection.TEMPLATE:
-                glue_template_service = GlueTemplateService(
-                    self.meta_data,
-                )
+            json_response_data = glue_query_set_service.process_body_data(self.access, self.glue_body_data)
+            return json_response_data.to_django_json_response()
 
-                html_response_data = glue_template_service.process_body_data(self.access, self.body_data)
-                return html_response_data
+        elif self.connection == GlueConnection.TEMPLATE:
+            glue_template_service = GlueTemplateService(
+                self.meta_data,
+            )
 
-            else:
-                return generate_json_404_response()
+            html_response_data = glue_template_service.process_body_data(self.access, self.glue_body_data)
+            return html_response_data
 
         else:
             return generate_json_404_response()
```

### Comparing `django-glue-0.4.2.1/django_glue/middleware.py` & `django-glue-0.4.2.2/django_glue/middleware.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/django_glue/responses.py` & `django-glue-0.4.2.2/django_glue/responses.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/django_glue/services/model_objects.py` & `django-glue-0.4.2.2/django_glue/services/model_objects.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import inspect
 from typing import Optional
 
 from django.contrib.contenttypes.models import ContentType
 from django.db.models import Model
 
 from django_glue.data_classes import GlueJsonResponseData, GlueJsonData, GlueBodyData, GlueMetaData
 from django_glue.responses import generate_json_200_response_data, generate_json_404_response_data
 from django_glue.services.services import Service
-from django_glue.utils import generate_simple_field_dict, get_fields_from_model, check_valid_method_kwargs, \
-    type_set_method_kwargs, field_name_included
+from django_glue.utils import generate_simple_field_dict, get_field_names_from_model, check_valid_method_kwargs, \
+    type_set_method_kwargs, generate_field_dict
 
 
 class GlueModelObjectService(Service):
     def __init__(self, meta_data: GlueMetaData) -> None:
         self.meta_data = meta_data
         self.model_class = None
         self.object: Optional[Model] = None
@@ -44,17 +43,18 @@
         )
 
     def process_create_action(self, body_data: GlueBodyData) -> GlueJsonResponseData:
         self.load_model_class()
 
         model_object = self.model_class()
 
-        for field in get_fields_from_model(model_object):
-            if field.name in body_data['data'] and field.name != 'id':
-                model_object.__dict__[field.name] = body_data['data'][field.name]
+        # Todo: This is duplicated code
+        for field_name in get_field_names_from_model(model_object):
+            if field_name in body_data['data'] and field_name != 'id':
+                model_object.__dict__[field_name] = body_data['data'][field_name]
 
         model_object.save()
 
         json_data = GlueJsonData()
 
         json_data.simple_fields = generate_simple_field_dict(
             model_object,
@@ -67,17 +67,17 @@
             'this is a response from an model object create action!',
             json_data
         )
 
     def process_update_action(self, body_data: GlueBodyData) -> GlueJsonResponseData:
         self.load_object()
 
-        for field in get_fields_from_model(self.object):
-            if field.name in body_data['data'] and field.name != 'id' and field_name_included(field.name, self.meta_data.fields, self.meta_data.exclude):
-                self.object.__dict__[field.name] = body_data['data'][field.name]
+        field_dict = generate_field_dict(self.object, self.meta_data.fields, self.meta_data.exclude)
+        for field_name in field_dict.keys():
+            self.object.__dict__[field_name] = body_data['data'][field_name]
 
         self.object.save()
 
         return generate_json_200_response_data(
             'THE UPDATE ACTION',
             'this is a response from an model object update action!'
         )
```

### Comparing `django-glue-0.4.2.1/django_glue/services/query_sets.py` & `django-glue-0.4.2.2/django_glue/services/query_sets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Optional
 
 from django.db.models import QuerySet
 
 from django_glue.data_classes import GlueJsonResponseData, GlueBodyData, GlueMetaData, GlueJsonData
 from django_glue.responses import generate_json_200_response_data, generate_json_404_response_data
 from django_glue.services.services import Service
-from django_glue.utils import decode_query_set_from_str, generate_simple_field_dict, get_fields_from_model, \
+from django_glue.utils import decode_query_set_from_str, generate_simple_field_dict, get_field_names_from_model, \
     check_valid_method_kwargs, type_set_method_kwargs, field_name_included
 
 
 class GlueQuerySetService(Service):
     def __init__(self, meta_data: GlueMetaData) -> None:
         self.meta_data = meta_data
         self.query_set: Optional[QuerySet] = None
@@ -44,17 +44,18 @@
         )
 
     def process_create_action(self, body_data: GlueBodyData) -> GlueJsonResponseData:
         self.load_query_set()
 
         model_object = self.meta_data.model_class()
 
-        for field in get_fields_from_model(self.meta_data.model_class):
-            if field.name in body_data['data'] and field.name != 'id':
-                setattr(model_object, field.name, body_data['data'][field.name])
+        # Todo: This is duplicated code
+        for field_name in get_field_names_from_model(self.meta_data.model_class):
+            if field_name in body_data['data'] and field_name != 'id':
+                setattr(model_object, field_name, body_data['data'][field_name])
 
         model_object.save()
 
         json_data = GlueJsonData()
 
         json_data.simple_fields = generate_simple_field_dict(
             model_object,
@@ -69,17 +70,18 @@
         )
 
     def process_update_action(self, body_data: GlueBodyData) -> GlueJsonResponseData:
         self.load_query_set()
 
         model_object = self.meta_data.model_class.objects.get(id=body_data['data']['id'])
 
-        for field in get_fields_from_model(self.meta_data.model_class):
-            if field.name in body_data['data'] and field.name != 'id' and field_name_included(field.name, self.meta_data.fields, self.meta_data.exclude):
-                model_object.__dict__[field.name] = body_data['data'][field.name]
+        # Todo: This is duplicated code
+        for field_name in get_field_names_from_model(self.meta_data.model_class):
+            if field_name in body_data['data'] and field_name != 'id' and field_name_included(field_name, self.meta_data.fields, self.meta_data.exclude):
+                model_object.__dict__[field_name] = body_data['data'][field_name]
 
         model_object.save()
 
         return generate_json_200_response_data(
             'THE QUERY UPDATE ACTION',
             'this is a response from an query set update action!'
         )
```

### Comparing `django-glue-0.4.2.1/django_glue/services/services.py` & `django-glue-0.4.2.2/django_glue/services/services.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/django_glue/services/templates.py` & `django-glue-0.4.2.2/django_glue/services/templates.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/django_glue/sessions.py` & `django-glue-0.4.2.2/django_glue/sessions.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 GLUE_SESSION_TYPES = (
     'context',
     'meta',
 )
 
 
 class GlueSession:
+    """
+        Used to add models, query sets, and other objects to the session.
+        Todo: What is context?
+    """
     def __init__(self, request):
         self.request = request
 
         self.request.session.setdefault(settings.DJANGO_GLUE_SESSION_NAME, dict())
 
         for session_type in GLUE_SESSION_TYPES:
             self.request.session[settings.DJANGO_GLUE_SESSION_NAME].setdefault(session_type, dict())
@@ -123,30 +127,35 @@
 
     def clean(self, removable_unique_names):
         for unique_name in removable_unique_names:
             self.purge_unique_name(unique_name)
 
         self.set_modified()
 
+    def has_unique_name(self, unique_name):
+        return unique_name in self.session['context']
+
     def purge_unique_name(self, unique_name):
         for session_type in GLUE_SESSION_TYPES:
             if unique_name in self.session[session_type]:
                 self.session[session_type].pop(unique_name)
 
     def set_modified(self):
         self.request.session.modified = True
 
     def unique_name_unused(self, unique_name):
-        if unique_name in self.session['context']:
-            return False
-        else:
-            return True
+        return unique_name in self.session['context']
+
 
 
 class GlueKeepLiveSession:
+    """
+        Used to keep glue session data live for a set amount of time.
+        Functionality to handle multiple windows/tabs.
+    """
     def __init__(self, request):
         self.request = request
         self.session = request.session.setdefault(settings.DJANGO_GLUE_KEEP_LIVE_SESSION_NAME, dict())
 
     def __getitem__(self, key):
         return self.session[key]
```

### Comparing `django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_ajax.js` & `django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_ajax.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_keep_live.js` & `django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_keep_live.js`

 * *Files 18% similar despite different names*

#### js-beautify {}

```diff
@@ -17,11 +17,10 @@
                 'Content-Type': 'application/json',
                 'X-CSRFToken': glue_get_cookie('csrftoken'),
             },
             body: JSON.stringify({
                 'unique_names': window.glue_keep_live_unique_names,
             }),
         }
-        const response = await fetch(keep_live_url, request_options)
-        window.glue_session_data = await response.json()
+        await fetch(keep_live_url, request_options)
     }
 }
```

### Comparing `django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_model_object.js` & `django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_model_object.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,17 +1,18 @@
 class GlueModelObject {
-    constructor(unique_name) {
-        this.glue_unique_name = unique_name
+    constructor(glue_unique_name) {
+        // Needs to be named glue_unique_name to avoid overriding the unique_name property
+        this.glue_unique_name = glue_unique_name
 
-        for (let key in window.glue_session_data['context'][unique_name].fields) {
-            this[key] = window.glue_session_data['context'][unique_name].fields[key].value
+        for (let key in window.glue_session_data['context'][glue_unique_name].fields) {
+            this[key] = window.glue_session_data['context'][glue_unique_name].fields[key].value
             console.log(key, this[key])
         }
 
-        window.glue_keep_live.add_unique_name(unique_name)
+        window.glue_keep_live.add_unique_name(glue_unique_name)
     }
 
     async create() {
         return await glue_ajax_request(
             this.glue_unique_name,
             'create',
             this.get_properties()
@@ -70,17 +71,15 @@
             console.log(response)
         })
     }
 
     get_properties() {
         let properties = {}
         Object.entries(this).forEach(([key, value]) => {
-            if (!key.startsWith('glue')) {
-                properties[key] = value
-            }
+            properties[key] = value
         });
         return properties
     }
 
     set_properties(properties) {
         for (let key in properties) {
             this[key] = properties[key]
```

### Comparing `django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_query_set.js` & `django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_query_set.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 class GlueQuerySet {
-    constructor(unique_name) {
-        this.glue_unique_name = unique_name
+    constructor(glue_unique_name) {
+        this.glue_unique_name = glue_unique_name
 
-        for (let key in window.glue_session_data['context'][unique_name].fields) {
-            this[key] = window.glue_session_data['context'][unique_name].fields[key].value
+        for (let key in window.glue_session_data['context'][glue_unique_name].fields) {
+            this[key] = window.glue_session_data['context'][glue_unique_name].fields[key].value
         }
 
-        window.glue_keep_live.add_unique_name(unique_name)
+        window.glue_keep_live.add_unique_name(glue_unique_name)
     }
 
     async all() {
         let model_object_list = []
 
         return await glue_ajax_request(this.glue_unique_name, 'get', {
                 'all': true
```

### Comparing `django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_template.js` & `django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_template.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/django_glue/static/django_glue/js/django_glue_view.js` & `django-glue-0.4.2.2/django_glue/static/django_glue/js/django_glue_view.js`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/django_glue/templates/django_glue/django_glue.html` & `django-glue-0.4.2.2/django_glue/templates/django_glue/django_glue.html`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/django_glue/templatetags/django_glue.py` & `django-glue-0.4.2.2/django_glue/templatetags/django_glue.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/django_glue/utils.py` & `django-glue-0.4.2.2/django_glue/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import inspect
 import logging, pickle, base64, json
-from typing import Optional, Callable
+from typing import Optional, Callable, Union
 
 from django.core import exceptions
+from django.db.models import Model
 
 from django_glue.core.utils import serialize_object_to_json
 from django_glue.data_classes import GlueModelFieldData
 
 
 def decode_query_set_from_str(query_set_string):
     query = pickle.loads(base64.b64decode(query_set_string))
@@ -29,15 +30,15 @@
 
 
 def generate_field_attr_dict(field):
     form_field = field.formfield()
     return form_field.widget_attrs(form_field.widget)
 
 
-def generate_field_dict(model_object, fields, exclude):
+def generate_field_dict(model_object: Model, fields: [list, tuple], exclude: Union[list, tuple]):
     fields_dict = dict()
 
     model = type(model_object)
     json_model = json.loads(serialize_object_to_json(model_object))[0]
 
     for field in model._meta.fields:
         try:
@@ -46,15 +47,21 @@
                     if field.name == 'id':
                         field_value = json_model['pk']
                         field_attr = ''
                     else:
                         field_value = json_model['fields'][field.name]
                         field_attr = generate_field_attr_dict(field)
 
-                    fields_dict[field.name] = GlueModelFieldData(
+                    # Todo: Field name logic is duplicated
+                    if field.attname == 'foreign_key_id':
+                        field_name = field.name + '_id'
+                    else:
+                        field_name = field.name
+
+                    fields_dict[field_name] = GlueModelFieldData(
                         type=field.get_internal_type(),
                         value=field_value,
                         html_attr=field_attr,
                     ).to_dict()
 
         except:
             raise f'Field "{field.name}" is invalid field or exclude for model type "{model.__class__.__name__}"'
@@ -83,16 +90,25 @@
 
     for key, val in fields_dict.items():
         simple_fields_dict[key] = val['value']
 
     return simple_fields_dict
 
 
-def get_fields_from_model(model):
-    return [field for field in model._meta.fields]
+# Todo: Field name logic is duplicated
+def get_field_names_from_model(model) -> list:
+    field_names = []
+
+    for field in model._meta.fields:
+        if field.attname == 'foreign_key_id':
+            field_names.append(field.name + '_id')
+        else:
+            field_names.append(field.name)
+
+    return field_names
 
 
 def check_valid_method_kwargs(method: Callable, kwargs: Optional[dict]):
     for kwarg in kwargs:
         if kwarg not in inspect.signature(method).parameters.keys():
             return False
     return True
```

### Comparing `django-glue-0.4.2.1/django_glue.egg-info/PKG-INFO` & `django-glue-0.4.2.2/django_glue.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-glue
-Version: 0.4.2.1
+Version: 0.4.2.2
 Summary: Industrial Strength Glue for Django Backends and Frontends!
 Home-page: https://github.com/stratusadv/django-glue
 Author: Nathan Johnson, Austin Sauer & Wesley Howery
 Author-email: info@stratusadv.com
 License: MIT
 Keywords: glue,django,backend,frontend,javascript,active server pages
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-glue-0.4.2.1/django_glue.egg-info/SOURCES.txt` & `django-glue-0.4.2.2/django_glue.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 django_glue.egg-info/PKG-INFO
 django_glue.egg-info/SOURCES.txt
 django_glue.egg-info/dependency_links.txt
 django_glue.egg-info/not-zip-safe
 django_glue.egg-info/requires.txt
 django_glue.egg-info/top_level.txt
 django_glue/core/__init__.py
+django_glue/core/decorators.py
 django_glue/core/utils.py
 django_glue/services/__init__.py
 django_glue/services/model_objects.py
 django_glue/services/query_sets.py
 django_glue/services/services.py
 django_glue/services/templates.py
 django_glue/static/django_glue/js/django_glue_ajax.js
@@ -55,8 +56,9 @@
 tests/settings.py
 tests/test_core.py
 tests/urls.py
 tests/utils.py
 tests/views.py
 tests/wsgi.py
 tests/migrations/0001_initial.py
+tests/migrations/0002_bigtestmodel_foreign_key_alter_testmodel_birth_date.py
 tests/migrations/__init__.py
```

### Comparing `django-glue-0.4.2.1/setup.py` & `django-glue-0.4.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/tests/manage.py` & `django-glue-0.4.2.2/tests/manage.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/tests/migrations/0001_initial.py` & `django-glue-0.4.2.2/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/tests/models.py` & `django-glue-0.4.2.2/tests/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from django.db import models
 from django.utils.timezone import now, localdate
 
-from django_glue.data_classes import GlueJsonResponseData
 
 
 class TestModel(models.Model):
     first_name = models.CharField(max_length=32)
     last_name = models.CharField(max_length=32)
     description = models.TextField()
     favorite_number = models.IntegerField()
@@ -33,14 +32,15 @@
     date_field = models.DateField()
     date_time_field = models.DateTimeField()
     decimal_field = models.DecimalField(decimal_places=2, max_digits=6)
     duration_field = models.DurationField()
     email_field = models.EmailField()
     file_path_field = models.FilePathField(path='/static')
     float_field = models.FloatField()
+    foreign_key = models.ForeignKey(TestModel, on_delete=models.CASCADE)
     generic_ip_address_field = models.GenericIPAddressField()
     ip_address_field = models.GenericIPAddressField()
     integer_field = models.IntegerField()
     positive_big_integer_field = models.PositiveBigIntegerField()
     positive_integer_field = models.PositiveIntegerField()
     positive_small_integer_field = models.PositiveSmallIntegerField()
     slug_field = models.SlugField()
```

### Comparing `django-glue-0.4.2.1/tests/settings.py` & `django-glue-0.4.2.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-glue-0.4.2.1/tests/urls.py` & `django-glue-0.4.2.2/tests/urls.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from django.urls import path, include
 from django.views.generic import TemplateView
 
 from tests import views
 
 urlpatterns = [
     path("", views.ModelObjectView.as_view(), name="model_object"),
+    path("big_model", views.big_model_object_view, name="big_model"),
     path("query_set/", views.QuerySetView.as_view(), name="query_set"),
     path("query_set/list/", views.query_set_list_view, name="query_set_list"),
     path("other/", views.OtherView.as_view(), name="other_glue"),
     path("no_glue/", TemplateView.as_view(template_name='page/no_glue_page.html'), name="no_glue"),
     path("benchmark/", views.benchmark_view, name="benchmark"),
     path("django_glue/", include('django_glue.urls', namespace='django_glue')),
     path("template/", views.template_view, name="template"),
```

### Comparing `django-glue-0.4.2.1/tests/utils.py` & `django-glue-0.4.2.2/tests/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,14 +117,15 @@
         char_field='Word',
         date_field=now(),
         date_time_field=now(),
         decimal_field=19.88,
         duration_field=datetime.timedelta(days=1, minutes=60),
         email_field='me@here.com',
         file_path_field='static.css',
+        foreign_key=TestModel.objects.first(),
         float_field=88.19,
         generic_ip_address_field='127.0.01',
         ip_address_field='0.0.0.0',
         integer_field=-23,
         positive_big_integer_field=3247238947238,
         positive_integer_field=1312321,
         positive_small_integer_field=9,
```

### Comparing `django-glue-0.4.2.1/tests/views.py` & `django-glue-0.4.2.2/tests/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,23 @@
 import logging
 
 from django.template.response import TemplateResponse
 from django.views.generic import TemplateView
 
-from tests.models import TestModel
+from tests.models import TestModel, BigTestModel
 from tests.utils import generate_randomized_test_model, generate_big_test_model
 from django_glue.glue import add_glue
 
 
+def big_model_object_view(request):
+    big_model = BigTestModel.objects.first()
+    add_glue(request, 'big_model', big_model, 'delete', fields=('foreign_key',))
+    return TemplateResponse(request, template='page/big_model_object_page.html')
+
+
 class ModelObjectView(TemplateView):
     template_name = 'page/model_object_page.html'
 
     def get_context_data(self, **kwargs):
         context_data = super().get_context_data(**kwargs)
 
         test_model_object = generate_randomized_test_model()
```

