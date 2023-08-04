# Comparing `tmp/topobank-statistics-1.1.0.tar.gz` & `tmp/topobank-statistics-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topobank-statistics-1.1.0.tar", last modified: Sun Jun 11 21:45:16 2023, max compression
+gzip compressed data, was "topobank-statistics-1.1.1.tar", last modified: Fri Aug  4 19:30:05 2023, max compression
```

## Comparing `topobank-statistics-1.1.0.tar` & `topobank-statistics-1.1.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.215458 topobank-statistics-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.207458 topobank-statistics-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-11 21:45:16.215458 topobank-statistics-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-11 21:45:16.215458 topobank-statistics-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/topobank_statistics/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/downloads.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/topobank_statistics/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/frontend/RoughnessParametersCard.vue
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/frontend/roughness_parameters_card.js
--rw-r--r--   0 runner    (1001) docker     (123)    33625 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/topobank_statistics/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/topobank_statistics/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/topobank_statistics/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/static/images/ce_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.215458 topobank-statistics-1.1.0/topobank_statistics/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26939 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/tests/test_reentrant.py
--rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/tests/test_results_view.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-06-11 21:45:05.000000 topobank-statistics-1.1.0/topobank_statistics/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 21:45:16.211458 topobank-statistics-1.1.0/topobank_statistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-06-11 21:45:16.000000 topobank-statistics-1.1.0/topobank_statistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-11 21:45:16.000000 topobank-statistics-1.1.0/topobank_statistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 21:45:16.000000 topobank-statistics-1.1.0/topobank_statistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-11 21:45:16.000000 topobank-statistics-1.1.0/topobank_statistics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-11 21:45:16.000000 topobank-statistics-1.1.0/topobank_statistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-11 21:45:16.000000 topobank-statistics-1.1.0/topobank_statistics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:05.833963 topobank-statistics-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:05.829963 topobank-statistics-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:05.829963 topobank-statistics-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-08-04 19:30:05.833963 topobank-statistics-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-04 19:30:05.833963 topobank-statistics-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:05.829963 topobank-statistics-1.1.1/topobank_statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/downloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:05.833963 topobank-statistics-1.1.1/topobank_statistics/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     7882 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/frontend/RoughnessParametersCard.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/frontend/roughness_parameters_card.js
+-rw-r--r--   0 runner    (1001) docker     (123)    33604 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:05.833963 topobank-statistics-1.1.1/topobank_statistics/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:05.829963 topobank-statistics-1.1.1/topobank_statistics/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:05.833963 topobank-statistics-1.1.1/topobank_statistics/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/static/images/ce_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:05.833963 topobank-statistics-1.1.1/topobank_statistics/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26939 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/tests/test_reentrant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7314 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/tests/test_results_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-08-04 19:29:53.000000 topobank-statistics-1.1.1/topobank_statistics/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:05.833963 topobank-statistics-1.1.1/topobank_statistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-08-04 19:30:05.000000 topobank-statistics-1.1.1/topobank_statistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 19:30:05.000000 topobank-statistics-1.1.1/topobank_statistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:30:05.000000 topobank-statistics-1.1.1/topobank_statistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-04 19:30:05.000000 topobank-statistics-1.1.1/topobank_statistics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 19:30:05.000000 topobank-statistics-1.1.1/topobank_statistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-04 19:30:05.000000 topobank-statistics-1.1.1/topobank_statistics.egg-info/top_level.txt
```

### Comparing `topobank-statistics-1.1.0/.github/workflows/publish.yml` & `topobank-statistics-1.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/.github/workflows/test.yml` & `topobank-statistics-1.1.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/.gitignore` & `topobank-statistics-1.1.1/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -320,19 +320,14 @@
 # Auto-generated tag files
 tags
 
 
 ### VirtualEnv template
 # Virtualenv
 # http://iamzed.com/2009/05/07/a-primer-on-virtualenv/
-[Bb]in
-[Ii]nclude
-[Ll]ib
-[Ll]ib64
-[Ss]cripts
 pyvenv.cfg
 pip-selfcheck.json
 
 #Celery_Created
 celerybeat-schedule.bak
 celerybeat-schedule.dat
 celerybeat-schedule.dir
@@ -342,23 +337,28 @@
 ### Project template
 
 MailHog
 topobank/media/
 topobank.db
 .pytest_cache/
 
-# The following files contain password and should be generated manally from .template files
+# The following files contain password and should be generated manully from .template files or commands
 .envs/.local/.django
+.envs/.local/.pypi-authfile
 .envs/.production/.django
 .envs/.production/.django.testserver
 .envs/.production/.postgres
 orcid.yaml
 
+# Locally generated pip packages
+docker/local/django/pip-packages/*
+
 # temporary files from soffice
 .~lock.*#
 
 # Some stuff which may appear during development
 .ipynb_checkpoints/
 /media/**/*
 !/stuff/usage_statistics.xlsx
 data/
+.envs/.local/.pypi-authfile
```

### Comparing `topobank-statistics-1.1.0/CHANGELOG.md` & `topobank-statistics-1.1.1/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Changelog for plugin *topobank-statistics*
 
+## 1.1.1 (2023-08-04)
+
+- MAINT: Unified CSRF injection
+
 ## 1.1.0 (2023-06-11)
 
 - ENH: Unified single page application for analyses, including rewritten
   task status
 - ENH: Webpack based bundling (for the analysis app)
 - ENH: Upgrade to Vue 3
 - MAINT: Easier to use download format for roughness parameters (#4)
```

### Comparing `topobank-statistics-1.1.0/LICENSE` & `topobank-statistics-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/PKG-INFO` & `topobank-statistics-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topobank-statistics
-Version: 1.1.0
+Version: 1.1.1
 Summary: This is a plugin for "topobank" for statistical analysis of measurements and digital surface twins.
 Author-email: Michael Röttger <info@michael-roettger.de>, Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
 License: 
         The MIT License (MIT)
         Copyright (c) 2018-2019, Simulation Group, IMTEK, University of Freiburg, Germany
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `topobank-statistics-1.1.0/README.rst` & `topobank-statistics-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/pyproject.toml` & `topobank-statistics-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/topobank_statistics/apps.py` & `topobank-statistics-1.1.1/topobank_statistics/apps.py`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/topobank_statistics/downloads.py` & `topobank-statistics-1.1.1/topobank_statistics/downloads.py`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/topobank_statistics/frontend/RoughnessParametersCard.vue` & `topobank-statistics-1.1.1/topobank_statistics/frontend/RoughnessParametersCard.vue`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         TasksButton
     },
     props: {
         apiUrl: {
             type: String,
             default: '/plugins/topobank_statistics/card/roughness-parameters'
         },
-        csrfToken: String,
         detailUrl: {
             type: String,
             default: '/analysis/html/detail/'
         },
         enlarged: {
             type: Boolean,
             default: false
@@ -43,14 +42,15 @@
             type: String,
             default() {
                 return uuid4();
             }
         },
         xlsxDownloadUrl: String
     },
+    inject: ['csrfToken'],
     data() {
         return {
             _analyses: null,
             _columnDefs: [
                 // Indicate that first column contains HTML
                 // to have HTML tags removed for sorting/filtering
                 {targets: 0, type: 'html'}
```

### Comparing `topobank-statistics-1.1.0/topobank_statistics/functions.py` & `topobank-statistics-1.1.1/topobank_statistics/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -587,17 +587,17 @@
 
 @register_implementation(APP_NAME, VIZ_ROUGHNESS_PARAMETERS, "Roughness parameters")
 def roughness_parameters(topography, progress_recorder=None, storage_prefix=None):
     """Calculate roughness parameters for given topography.
 
     Parameters
     ----------
-    topography: topobank.manager.models.Topography
-    progress_recorder: celery_progress.backend.ProgressRecorder or None
-    storage_prefix: str or None
+    topography : topobank.manager.models.Topography
+    progress_recorder : ProgressRecorder or None
+    storage_prefix : str or None
 
     Returns
     -------
     list of dicts where each dict has keys
 
      quantity, e.g. 'RMS height' or 'RMS gradient'
      direction, e.g. 'x' or None
```

### Comparing `topobank-statistics-1.1.0/topobank_statistics/static/images/ce_logo.svg` & `topobank-statistics-1.1.1/topobank_statistics/static/images/ce_logo.svg`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/topobank_statistics/tests/test_functions.py` & `topobank-statistics-1.1.1/topobank_statistics/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/topobank_statistics/tests/test_reentrant.py` & `topobank-statistics-1.1.1/topobank_statistics/tests/test_reentrant.py`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/topobank_statistics/tests/test_results_view.py` & `topobank-statistics-1.1.1/topobank_statistics/tests/test_results_view.py`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/topobank_statistics/tests/urls.py` & `topobank-statistics-1.1.1/topobank_statistics/tests/urls.py`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/topobank_statistics/tests.py` & `topobank-statistics-1.1.1/topobank_statistics/tests.py`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/topobank_statistics/urls.py` & `topobank-statistics-1.1.1/topobank_statistics/urls.py`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/topobank_statistics/views.py` & `topobank-statistics-1.1.1/topobank_statistics/views.py`

 * *Files identical despite different names*

### Comparing `topobank-statistics-1.1.0/topobank_statistics.egg-info/PKG-INFO` & `topobank-statistics-1.1.1/topobank_statistics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topobank-statistics
-Version: 1.1.0
+Version: 1.1.1
 Summary: This is a plugin for "topobank" for statistical analysis of measurements and digital surface twins.
 Author-email: Michael Röttger <info@michael-roettger.de>, Lars Pastewka <lars.pastewka@imtek.uni-freiburg.de>
 License: 
         The MIT License (MIT)
         Copyright (c) 2018-2019, Simulation Group, IMTEK, University of Freiburg, Germany
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `topobank-statistics-1.1.0/topobank_statistics.egg-info/SOURCES.txt` & `topobank-statistics-1.1.1/topobank_statistics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

