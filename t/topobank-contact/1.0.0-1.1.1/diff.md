# Comparing `tmp/topobank-contact-1.0.0.tar.gz` & `tmp/topobank-contact-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topobank-contact-1.0.0.tar", last modified: Tue Jan 31 12:49:09 2023, max compression
+gzip compressed data, was "topobank-contact-1.1.1.tar", last modified: Fri Aug  4 19:30:34 2023, max compression
```

## Comparing `topobank-contact-1.0.0.tar` & `topobank-contact-1.1.1.tar`

### file list

```diff
@@ -1,56 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.154587 topobank-contact-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.150587 topobank-contact-1.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.150587 topobank-contact-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.150587 topobank-contact-1.0.0/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-01-31 12:49:09.154587 topobank-contact-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/README
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.150587 topobank-contact-1.0.0/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.150587 topobank-contact-1.0.0/config/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/config/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24190 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/config/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/config/settings/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-01-31 12:49:09.154587 topobank-contact-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.154587 topobank-contact-1.0.0/topobank_contact/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)    19964 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.154587 topobank-contact-1.0.0/topobank_contact/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.150587 topobank-contact-1.0.0/topobank_contact/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.154587 topobank-contact-1.0.0/topobank_contact/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/static/images/ce_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.150587 topobank-contact-1.0.0/topobank_contact/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.154587 topobank-contact-1.0.0/topobank_contact/templates/topobank_contact/
--rw-r--r--   0 runner    (1001) docker     (123)    24322 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/templates/topobank_contact/contact_mechanics_card_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/templates/topobank_contact/contact_mechanics_card_list.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.154587 topobank-contact-1.0.0/topobank_contact/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/tests/test_downloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-01-31 12:48:56.000000 topobank-contact-1.0.0/topobank_contact/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 12:49:09.154587 topobank-contact-1.0.0/topobank_contact.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-01-31 12:49:09.000000 topobank-contact-1.0.0/topobank_contact.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-01-31 12:49:09.000000 topobank-contact-1.0.0/topobank_contact.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 12:49:09.000000 topobank-contact-1.0.0/topobank_contact.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-01-31 12:49:09.000000 topobank-contact-1.0.0/topobank_contact.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-31 12:49:09.000000 topobank-contact-1.0.0/topobank_contact.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-31 12:49:09.000000 topobank-contact-1.0.0/topobank_contact.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:34.829253 topobank-contact-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:34.825253 topobank-contact-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:34.825253 topobank-contact-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:34.825253 topobank-contact-1.1.1/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-08-04 19:30:34.829253 topobank-contact-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-04 19:30:34.829253 topobank-contact-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:34.829253 topobank-contact-1.1.1/topobank_contact/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/downloads.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:34.829253 topobank-contact-1.1.1/topobank_contact/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)    20615 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/frontend/ContactMechanicsCard.vue
+-rw-r--r--   0 runner    (1001) docker     (123)    17255 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/frontend/ContactMechanicsParametersModal.vue
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/frontend/contact_mechanics_card.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19813 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:34.829253 topobank-contact-1.1.1/topobank_contact/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:34.825253 topobank-contact-1.1.1/topobank_contact/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:34.829253 topobank-contact-1.1.1/topobank_contact/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/static/images/ce_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:34.829253 topobank-contact-1.1.1/topobank_contact/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/tests/test_downloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-08-04 19:30:24.000000 topobank-contact-1.1.1/topobank_contact/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:30:34.829253 topobank-contact-1.1.1/topobank_contact.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-08-04 19:30:34.000000 topobank-contact-1.1.1/topobank_contact.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-04 19:30:34.000000 topobank-contact-1.1.1/topobank_contact.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:30:34.000000 topobank-contact-1.1.1/topobank_contact.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-04 19:30:34.000000 topobank-contact-1.1.1/topobank_contact.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 19:30:34.000000 topobank-contact-1.1.1/topobank_contact.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-04 19:30:34.000000 topobank-contact-1.1.1/topobank_contact.egg-info/top_level.txt
```

### Comparing `topobank-contact-1.0.0/.github/workflows/publish.yml` & `topobank-contact-1.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `topobank-contact-1.0.0/.github/workflows/test.yml` & `topobank-contact-1.1.1/.github/workflows/test.yml`

 * *Files 9% similar despite different names*

```diff
@@ -43,19 +43,20 @@
     - name: Set up python3 ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
 
     - name: Install
       run: |
-        pip install --upgrade pip
+        pip install --upgrade pip pip-tools
         pushd /tmp
-        git clone --branch develop https://github.com/ContactEngineering/topobank.git
-        cd topobank
-        pip install -q -r requirements/local.txt
-        pip install -e .[dev]
+        git clone https://github.com/ContactEngineering/topobank.git
+        popd
+        pip-compile --extra dev pyproject.toml /tmp/topobank/pyproject.toml
+        pip install -r requirements.txt
+        pushd /tmp/topobank
         USE_DOCKER=no python manage.py collectstatic
         popd
         pip install -e .[dev]
 
     - name: Test
-      run: pytest -v
+      run: PYTHONPATH=/tmp/topobank pytest -v
```

### Comparing `topobank-contact-1.0.0/.gitignore` & `topobank-contact-1.1.1/.gitignore`

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

### Comparing `topobank-contact-1.0.0/LICENSE` & `topobank-contact-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `topobank-contact-1.0.0/topobank_contact/apps.py` & `topobank-contact-1.1.1/topobank_contact/apps.py`

 * *Files identical despite different names*

### Comparing `topobank-contact-1.0.0/topobank_contact/downloads.py` & `topobank-contact-1.1.1/topobank_contact/downloads.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 import pandas as pd
 from django.core.files.storage import default_storage
 from django.http import HttpResponse
 
 from topobank.analysis.downloads import analysis_header_for_txt_file
 from topobank.analysis.registry import register_download_function
-from .functions import ART_CONTACT_MECHANICS
+from .functions import VIZ_CONTACT_MECHANICS
 
 
-@register_download_function(ART_CONTACT_MECHANICS, 'results', 'zip')
+@register_download_function(VIZ_CONTACT_MECHANICS, 'results', 'zip')
 def download_contact_mechanics_analyses_as_zip(request, analyses):
     """Provides a ZIP file with contact mechanics data.
 
     :param request: HTTPRequest
     :param analyses: sequence of Analysis instances
     :return: HTTP Response with file download
     """
@@ -73,15 +73,15 @@
                 zf.writestr("errors-{}.txt".format(dirname),
                             "Cannot save file {} in ZIP, reason: {}".format(filename_in_zip, str(exc)))
 
         #
         # Add a file with version information
         #
         zf.writestr(os.path.join(zip_dir, 'info.txt'),
-                    analysis_header_for_txt_file(analysis))
+                    analysis_header_for_txt_file(analysis, dois=True))
 
 
     #
     # Add a Readme file
     #
     zf.writestr("README.txt",
                 f"""
@@ -95,15 +95,16 @@
 - a simple CSV file ('plot.csv')
 - a couple of classical netCDF files (Extension '.nc')
 
 The file 'plot.csv' contains a table with the data used in the plot,
 one line for each calculation step. It has the following columns:
 
 - Zero-based index column
-- Normalized pressure in units of p/E*
+- Normalized mean pressure in units of p/E*. 
+  The mean pressure is the total force divided by the nominal area of contact A0. 
 - Fractional contact area in units of A/A0
 - Normalized mean gap in units of u/h_rms
 - A boolean flag (True/False) which indicates whether the calculation converged
   within the given limit
 - Filename of the NetCDF file (order of filenames may be different than index)
 
 So each line also refers to one NetCDF file in the directory, it corresponds to
```

### Comparing `topobank-contact-1.0.0/topobank_contact/functions.py` & `topobank-contact-1.1.1/topobank_contact/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 from SurfaceTopography.Uniform.GeometryAnalysis import patch_areas, assign_patch_numbers_area
 from ContactMechanics import PeriodicFFTElasticHalfSpace, FreeFFTElasticHalfSpace
 from ContactMechanics.Factory import make_system, make_plastic_system
 
 from topobank.analysis.functions import IncompatibleTopographyException
 from topobank.analysis.registry import register_implementation
 from topobank.manager.utils import default_storage_replace, make_dzi
-from topobank.utils import NumpyEncoder
+from topobank.supplib.json import ExtendedJSONEncoder
 
-ART_CONTACT_MECHANICS = "contact mechanics"
+APP_NAME = "topobank_contact"
+VIZ_CONTACT_MECHANICS = "contact-mechanics"
 
 CONTACT_MECHANICS_MAX_MB_GRID_PTS_PRODUCT = 100000000
 CONTACT_MECHANICS_MAX_MB_GRID_PTS_PER_DIM = 10000
 
 
 _log = logging.getLogger(__name__)
 
@@ -208,15 +209,15 @@
     contacting_points_xy = force_xy > 0
 
     return displacement_xy, gap_xy, pressure_xy, contacting_points_xy, \
            opt.offset, mean_load, total_contact_area, \
            (mean_displacements, mean_gaps, mean_pressures, total_contact_areas, converged)
 
 
-@register_implementation(art=ART_CONTACT_MECHANICS, name="Contact mechanics")
+@register_implementation(APP_NAME, VIZ_CONTACT_MECHANICS, "Contact mechanics")
 def contact_mechanics(topography, substrate_str="nonperiodic", hardness=None, nsteps=10,
                       pressures=None, maxiter=100, progress_recorder=None, storage_prefix=None):
     """
     Note that `loads` is a list of pressures if the substrate is periodic and a list of forces otherwise.
 
     :param topography:
     :param substrate_str: one of ['periodic', 'nonperiodic', None ]; if None, choose from topography's 'is_periodic' flag
@@ -410,15 +411,15 @@
             'clusterAreaProbabilityDensitySIScaleFactor': 1 / (fac * fac)
         })
 
         #
         # Write to storage
         #
         default_storage_replace(f'{storage_path}/json/distributions.json',
-                                io.BytesIO(json.dumps(data_dict, cls=NumpyEncoder).encode('utf-8')))
+                                io.BytesIO(json.dumps(data_dict, cls=ExtendedJSONEncoder).encode('utf-8')))
 
         #
         # Make Deep Zoom Images of pressure, contacting points, gap and displacement
         #
 
         make_dzi(pressure_xy.data, f'{storage_path}/dzi/pressure',
                  physical_sizes=topography.physical_sizes, unit=topography.unit,
@@ -457,16 +458,9 @@
         min_pentol=min_pentol,
         mean_pressures=mean_pressure[sort_order],
         total_contact_areas=total_contact_area[sort_order],
         mean_displacements=mean_displacement[sort_order] / rms_height,
         mean_gaps=mean_gap[sort_order] / rms_height,
         converged=converged[sort_order],
         data_paths=data_paths[sort_order],
-        effective_kwargs=dict(
-            substrate_str=substrate_str,
-            hardness=hardness,
-            nsteps=nsteps,
-            pressures=pressures,
-            maxiter=maxiter,
-        ),
         alerts=alerts,
     )
```

### Comparing `topobank-contact-1.0.0/topobank_contact/static/images/ce_logo.svg` & `topobank-contact-1.1.1/topobank_contact/static/images/ce_logo.svg`

 * *Files identical despite different names*

### Comparing `topobank-contact-1.0.0/topobank_contact/templates/topobank_contact/contact_mechanics_card_detail.html` & `topobank-contact-1.1.1/topobank_contact/frontend/ContactMechanicsCard.vue`

 * *Files 21% similar despite different names*

```diff
@@ -1,514 +1,445 @@
-{# Needs some keys in context. See AJAX view "PlotCardView" #}
-{% extends 'analysis/simple_card_detail.html' %}
-{% load analysis_tags %}
-{% load icon_tags %}
-{% load static %}
-
-{% block card_header %}
-  {% if not analyses_unready and analyses_success %}
-    <div class="btn-group btn-group-sm float-right dropdown">
-      <a type="button" class="btn btn-default"
-         href="{% url 'analysis:download' analyses_success|analyses_results_ids_list_str 'contact mechanics' 'zip' %}">
-        {% fa5_icon 'download' %} Download ZIP
-      </a>
-    </div>
-  {% endif %}
-  <div class="pull-left">
-    <h3>{{ title }}</h3>
-  </div>
-{% endblock card_header %}
-
-{% block card_body %}
-  <div class="row">
-    {% include 'analysis/analyses_alerts.html' %}
-  </div>
-  <div id="contact-mechanics-card" class="row">
-    <b-alert variant="error" :show="errorMessage !== null">[[ errorMessage ]]</b-alert>
-    {# Left side with simulation results #}
-    <div v-if="errorMessage === null" class="col-sm-5">
-      <div class="tab-pane show active" id="plot-{{ card_id }}" role="tabpanel" aria-labelledby="card-tab">
-        {% if analyses_success %}
-          {# Show all analyses for which we have results #}
-          <bokeh-plot
-            :plots="contactMechanicsPlots"
-            :categories="contactMechanicsCategories"
-            :data-sources='{{ data_sources|safe }}'
-            :selectable="true"
-            v-on:selected="onSelected"
-            :options-widgets="['layout', 'legend', 'lineWidth', 'symbolSize']"
-            output-backend="{{ output_backend }}">
-          </bokeh-plot>
-        {% endif %}
-      </div>
-    </div>
-
-    {% if not analyses_unready %}
-      {# Middle with group of tabs #}
-      <div class="col-2 col-sm-2 col-md-2 col-lg-2">
-
-        <div class="nav nav-pills nav-pills-custom flex-column" aria-orientation="vertical">
-          <a class="nav-link mb-3 p-3 shadow active" data-toggle="pill" href="#contacting-points-tab" role="tab"
-             aria-selected="true">
-            Contact geometry
-          </a>
-          <a class="nav-link mb-3 p-3 shadow" data-toggle="pill" href="#pressure-tab" role="tab" aria-selected="false">
-            Contact pressure
-          </a>
-          <a class="nav-link mb-3 p-3 shadow" data-toggle="pill" href="#displacement-tab" role="tab"
-             aria-selected="false">
-            Displacement
-          </a>
-          <a class="nav-link mb-3 p-3 shadow" data-toggle="pill" href="#gap-tab" role="tab" aria-selected="false">
-            Gap
-          </a>
-          <a class="nav-link mb-3 p-3 shadow" data-toggle="pill" href="#distribution-function-tab" role="tab"
-             aria-selected="false">
-            Distribution functions
-          </a>
-          <hr>
-          <a class="nav-link mb-3 p-3 shadow" data-toggle="pill" href="#actions-tab" role="tab" aria-selected="false">
-            Parameters
-          </a>
-          {% if analyses_failure or extra_warnings %}
-            <a class="nav-link mb-3 p-3 shadow" data-toggle="pill" href="#warnings-tab-{{ card_id }}" role="tab"
-               aria-selected="false">
-              Warnings
-            </a>
-          {% endif %}
-
-        </div>
-
-      </div>
-
-      {# Right with simulation details and actions #}
-      <div class="col-sm-5">
-        {# Tab contents on right side #}
-        <div class="tab-content">
-          <div class="tab-pane fade active show" id="contacting-points-tab">
-            <div v-if="selection === null" id="geometry" class="alert alert-info">For contact geometry, select a point
-              in the graphs on the left!
-            </div>
-            <deep-zoom-image v-if="selection !== null"
-                             :prefix-url="'{% url 'analysis:data' pk=123 location='step-456/dzi/contacting-points/' %}'.replace('123/step-456', selection.analysis_id + '/' + selection.data_path)"
-                             ref="contactingPoints">
-            </deep-zoom-image>
-            <div v-if="selection !== null" class="pull-right">
-              <a class="btn btn-default btn-block btn-lg mt-3" v-on:click="$refs.contactingPoints.download()">
-                {% fa5_icon 'download' %} Download PNG
-              </a>
-            </div>
-          </div>
-          <div class="tab-pane fade" id="pressure-tab">
-            <div v-if="selection === null" id="pressure" class="alert alert-info">For contact pressure, select a point
-              in the graphs on the left!
-            </div>
-            <deep-zoom-image v-if="selection !== null"
-                             :prefix-url="'{% url 'analysis:data' pk=123 location='step-456/dzi/pressure/' %}'.replace('123/step-456', selection.analysis_id + '/' + selection.data_path)"
-                             :colorbar="true"
-                             ref="pressure">
-            </deep-zoom-image>
-            <div v-if="selection !== null" class="pull-right">
-              <a class="btn btn-default btn-block btn-lg" v-on:click="$refs.pressure.download()">
-                {% fa5_icon 'download' %} Download PNG
-              </a>
-            </div>
-          </div>
-          <div class="tab-pane fade" id="displacement-tab">
-            <div v-if="selection === null" id="displacement" class="alert alert-info">For displacement, select a point
-              in the graphs on the left!
-            </div>
-            <deep-zoom-image v-if="selection !== null"
-                             :prefix-url="'{% url 'analysis:data' pk=123 location='step-456/dzi/displacement/' %}'.replace('123/step-456', selection.analysis_id + '/' + selection.data_path)"
-                             :colorbar="true"
-                             ref="displacement">
-            </deep-zoom-image>
-            <div v-if="selection !== null" class="pull-right">
-              <a class="btn btn-default btn-block btn-lg" v-on:click="$refs.displacement.download()">
-                {% fa5_icon 'download' %} Download PNG
-              </a>
-            </div>
-          </div>
-          <div class="tab-pane fade" id="gap-tab">
-            <div v-if="selection === null" id="gap" class="alert alert-info">For gap, select a point in the graphs on
-              the left!
-            </div>
-            <deep-zoom-image v-if="selection !== null"
-                             :prefix-url="'{% url 'analysis:data' pk=123 location='step-456/dzi/gap/' %}'.replace('123/step-456', selection.analysis_id + '/' + selection.data_path)"
-                             :colorbar="true"
-                             ref="gap">
-            </deep-zoom-image>
-            <div v-if="selection !== null" class="pull-right">
-              <a class="btn btn-default btn-block btn-lg" v-on:click="$refs.gap.download()">
-                {% fa5_icon 'download' %} Download PNG
-              </a>
-            </div>
-          </div>
-          <div class="tab-pane fade" id="distribution-function-tab">
-            <div v-if="selection === null" id="distribution-function" class="alert alert-info">For pressure
-              distribution, select a point in the graphs on the left!
-            </div>
-            <bokeh-plot
-              v-if="selection !== null"
-              :plots="distributionPlots"
-              :data-sources="distributionDataSources"
-              output-backend="{{ output_backend }}">
-            </bokeh-plot>
-          </div>
-          <div class="tab-pane fade" id="actions-tab">
-
-            {# BUTTON "TASK INFORMATION" #}
-            <div class="row p-3">
-              <div class="col-12">
-                {% if analyses_available and not analyses_unready %}
-                  <a class="btn btn-default btn-block btn-lg" href="#" data-toggle="modal"
-                     data-target="#statusesModal-{{ card_id }}">{% fa5_icon 'tasks' %} Tasks</a>
-                {% endif %}
-              </div>
-            </div>
-
-            {# ELEMENTS FOR TRIGGERING A CALCULATION #}
-            <div class="row p-3">
-              <div class="col-12">
-
-                <form>
-                  <div class="form-group row">
-
-                    {# Substrate selection #}
-
-                    <div class="input-group col-auto mb-3">
-                      <div class="input-group-prepend">
-                        <div class="input-group-text">
-                          Type
-                        </div>
-
-                      </div>
-                      <b-form-select v-model="periodicity" :options="periodicityOptions"></b-form-select>
-                      <div class="input-group-append">
-                        <div class="input-group-text">
-                          <b-icon-info-circle-fill
-                            title="Type of calculation"
-                            v-b-popover.hover="'This option determines how the elastic interactions are calculated. This affects edge effects that may show up in the results at large contact area. Calculations can assume that the surface repeats periodically or that it is pushing down on a nonperiodic, infinitely expanded half-space. The latter option corresponds to mapping the surface topography on a flat punch. If not given, this value is automatically chosen as periodic for periodic topographies, else non-periodic.'">
-                          </b-icon-info-circle-fill>
-                        </div>
-                      </div>
-                    </div>
-
-                    {# Hardness input #}
-                    <div class="input-group col-auto mb-3">
-
-                      <div class="input-group-prepend">
-                        <div class="input-group-text">
-                          Hardness
-                        </div>
-                        <div class="input-group-text">
-                          <input type="checkbox" v-model="enableHardness">
-                        </div>
-                      </div>
-                      <input id="hardness-input" type="number" min="0" step="0.1" class="form-control"
-                             v-model="hardness" :disabled="!enableHardness">
-                      <div class="input-group-append ">
-                        <div class="input-group-text">
-                          E<sup>*</sup>
-                        </div>
-                        <div class="input-group-text">
-                          <b-icon-info-circle-fill
-                            v-b-popover.hover="'Setting a hardness enables plastic calculations. Local pressure cannot exceed hardness value.'"
-                            title="Hardness">
-                          </b-icon-info-circle-fill>
-                        </div>
-                      </div>
-                    </div>
-
-                    {# Step selection #}
-                    <div class="input-group col-auto mb-3">
-                      {# Automatic #}
-                      <div class="input-group-prepend">
-                        <div class="input-group-text">
-                          <input type="radio"
-                                 name="pressure-selection"
-                                 value="automatic"
-                                 checked="checked"
-                                 v-model="pressureSelection"
-                                 aria-label="Radio button for automatic step selection">
-                        </div>
-                        <div class="input-group-text">
-                          Number of steps
-                        </div>
-                      </div>
-                      <input id='nsteps-input' type="number"
-                             min="{{ limits_calc_kwargs.nsteps.min }}"
-                             max="{{ limits_calc_kwargs.nsteps.max }}"
-                             step="1" class="form-control"
-                             v-model="nsteps"
-                             :disabled="pressureSelection != 'automatic'">
-                      <div class="input-group-append ">
-                        <div class="input-group-text">
-                          <b-icon-info-circle-fill
-                            title="Automatic step selection"
-                            v-b-popover.hover="'Number of pressure steps which are chosen automatically.'">
-                          </b-icon-info-circle-fill>
-                        </div>
-                      </div>
-                    </div>
-                    <div class="input-group col-auto mb-3">
-                      {# Fixed list #}
-                      <div class="input-group-prepend">
-                        <div class="input-group-text">
-                          <input type="radio"
-                                 name="pressure-selection"
-                                 value="manual"
-                                 v-model="pressureSelection"
-                                 aria-label="Radio button for list of values">
-                        </div>
-                        <div class="input-group-text">
-                          Pressures
-                        </div>
-                      </div>
-                      <b-form-tags class="form-control"
-                                   placeholder=""
-                                   separator=" ,;"
-                                   v-model="pressures"
-                                   :disabled="pressureSelection != 'manual'">
-                      </b-form-tags>
-                      <div class="input-group-append">
-                        <div class="input-group-text">
-                          E<sup>*</sup>
-                        </div>
-                        <div class="input-group-text">
-                          <b-icon-info-circle-fill
-                            title="Manual step selection"
-                            v-b-popover.hover="'Enter positive pressure values for which you need results. You can also copy/paste a comma-separated list of values with a comma after every number. Use dot as decimal separator. The maximum number of values is {{ limits_calc_kwargs.pressures.maxlen }}.'">
-                          </b-icon-info-circle-fill>
-                        </div>
-                      </div>
-                    </div>
+<script>
 
-                    {# Input of maximum number of iterations  #}
-                    <div class="input-group col-auto">
-                      {# Automatic #}
-                      <div class="input-group-prepend">
-                        <div class="input-group-text">
-                          Max. number of iterations
-                        </div>
-                      </div>
-                      <input id='maxiter-input' type="number"
-                             min="{{ limits_calc_kwargs.maxiter.min }}"
-                             max="{{ limits_calc_kwargs.maxiter.max }}"
-                             step="100" class="form-control"
-                             v-model="maxNbIter">
-                      <div class="input-group-append ">
-                        <div class="input-group-text">
-                          <b-icon-info-circle-fill
-                            title="Maximum number of iterations"
-                            v-b-popover.hover="'Maximum number of iterations (<={{ limits_calc_kwargs.maxiter.max }}).'">
-                          </b-icon-info-circle-fill>
-                        </div>
-                      </div>
-                    </div>
-                  </div>
-                </form>
-
-                {% if request.user.is_anonymous %}
-                  <button title="Please login for this feature"
-                          class="btn btn-primary btn-block btn-lg disabled" disabled>
-                    {% fa5_icon 'repeat' %} Recalculate
-                  </button>
-                {% else %}
-                  <b-alert variant="warning"
-                           :show="recalculateWarning"
-                           dismissible
-                           v-on:dismissed="recalculateWarning = false">
-                    Some of the input parameters were invalid. We have updated those parameters for you. Please
-                    double-check the parameters and click <b>Recalculate</b> when ready.
-                  </b-alert>
-                  <button title="Trigger calculation with given arguments"
-                          class="btn btn-primary btn-block btn-lg"
-                          v-on:click="recalculate">
-                    {% fa5_icon 'repeat' %} Recalculate
-                  </button>
-                {% endif %}
-              </div>
-            </div>
+import {v4 as uuid4} from 'uuid';
 
-          </div>
-          {% include 'analysis/analyses_warnings_tab_pane.html' %}
-        </div>
-      </div>
-    {% endif %}
-
-  </div>
-
-{% endblock card_body %}
-
-{% block card_javascript %}
-  <script>
-    new Vue({
-      delimiters: ['[[', ']]'],
-      el: "#contact-mechanics-card",
-      data: function () {
+import BokehPlot from 'topobank/components/BokehPlot.vue';
+import BibliographyModal from 'topobank/analysis/BibliographyModal.vue';
+import CardExpandButton from 'topobank/analysis/CardExpandButton.vue';
+import ContactMechanicsParametersModal from 'topobank_contact/ContactMechanicsParametersModal.vue';
+import DeepZoomImage from 'topobank/components/DeepZoomImage.vue';
+import TasksButton from 'topobank/analysis/TasksButton.vue';
+
+export default {
+    name: 'contact-mechanics-card',
+    components: {
+        CardExpandButton,
+        ContactMechanicsParametersModal,
+        BibliographyModal,
+        BokehPlot,
+        DeepZoomImage,
+        TasksButton
+    },
+    props: {
+        apiUrl: {
+            type: String,
+            default: '/plugins/topobank_contact/card/contact-mechanics'
+        },
+        detailUrl: {
+            type: String,
+            default: '/analysis/html/detail/'
+        },
+        enlarged: {
+            type: Boolean,
+            default: true
+        },
+        functionId: Number,
+        functionName: String,
+        subjects: String,
+        txtDownloadUrl: String,
+        uid: {
+            type: String,
+            default() {
+                return uuid4();
+            }
+        },
+        xlsxDownloadUrl: String
+    },
+    inject: ['csrfToken'],
+    data() {
         return {
-          errorMessage: null,
-          recalculateWarning: false,
-          selection: null,
-          periodicity: "{{ initial_calc_kwargs.substrate_str|default_if_none:"nonperiodic" }}",
-          nsteps: {{ initial_calc_kwargs.nsteps|default_if_none:10 }},
-          enableHardness: {% if initial_calc_kwargs.hardness %}1{% else %}0{% endif %},
-          pressureSelection: {% if initial_calc_kwargs.pressures %}"manual"{% else %}"automatic"{% endif %},
-          hardness: {{ initial_calc_kwargs.hardness|default_if_none:"undefined" }},
-          pressures: {{ initial_calc_kwargs.pressures|default_if_none:"[]" }},
-          maxNbIter: {{ initial_calc_kwargs.maxiter|default_if_none:100 }},
-          periodicityOptions: [
-            {value: "periodic", text: "Periodic (repeating array of the measurement)"},
-            {value: "nonperiodic", text: "Free boundaries (flat punch with measurement)"}
-          ]
+            _analyses: null,
+            _api: {},
+            _cardStatus: 'mounted',  // 'mounted', 'waiting-for-first-result', 'analyses-partially-available', 'analyses-finished'
+            _dois: [],
+            _dataSources: [],
+            _enable_hardness: 0,
+            _hardness: undefined,
+            _functionKwargs: null,
+            _limitsToFunctionKwargs: null,
+            _maxNbIter: 100,
+            _nbFailed: 0,
+            _nbRunningOrPending: 0,
+            _nbSteps: 10,
+            _nbSuccess: 0,
+            _outputBackend: "svg",
+            _periodicity: "nonperiodic",
+            _selection: null,
+            _sidebarVisible: false,
+            _periodicityOptions: [
+                {value: "periodic", text: "Periodic (repeating array of the measurement)"},
+                {value: "nonperiodic", text: "Free boundaries (flat punch with measurement)"}
+            ],
+            _pressureselection: "automatic",
+            _pressures: []
+        }
+    },
+    mounted() {
+        this.updateCard();
+    },
+    methods: {
+        updateCard() {
+            this.updateCardWithFunctionKwargs(this._functionKwargs);
+        },
+        updateCardWithFunctionKwargs(functionKwargs = null) {
+            this._functionKwargs = functionKwargs;
+
+            /* Fetch JSON describing the card */
+            console.log(functionKwargs);
+            let functionKwargsBase64 = btoa(JSON.stringify(functionKwargs));
+            fetch(`${this.apiUrl}/${this.functionId}?subjects=${this.subjects}&function_kwargs=${functionKwargsBase64}`, {
+                method: 'GET',
+                headers: {
+                    'Accept': 'application/json',
+                    'X-CSRFToken': this.csrfToken
+                }
+            })
+                .then(response => response.json())
+                .then(data => {
+                    this._analyses = data.analyses;
+                    this._dois = data.dois;
+                    if (this._functionKwargs === null) {
+                        this._functionKwargs = data.uniqueKwargs;
+                    } else {
+                        this._functionKwargs = {
+                            ...this._functionKwargs,
+                            ...data.uniqueKwargs  // override since the server may report changes
+                        };
+                    }
+                    this._limitsToFunctionKwargs = data.limitsToFunctionKwargs;
+                    this._api = data.api;
+
+                    if (data.plotConfiguration !== undefined) {
+                        if (this._analyses.map(a => a.task_state == 'pe' || a.task_state == 'st').some(v => v)) {
+                            this._cardStatus = 'analyses-partially-available';
+                        } else {
+                            this._cardStatus = 'analyses-finished';
+                        }
+                        this._dataSources = data.plotConfiguration.dataSources;
+                        this._outputBackend = data.plotConfiguration.outputBackend;
+                    } else {
+                        this._cardStatus = 'waiting-for-first-result';
+                    }
+                });
+        },
+        onSelected(obj, data) {
+            const name = data.source.name;
+            const path = data.source.data.dataPath[data.source.selected.indices[0]];
+            const splitPath = path.split('/');
+            this._selection = {
+                analysisId: name.split('-')[1],
+                dataPath: splitPath[splitPath.length - 1]  // We need to do some name mangling
+            };
+        },
+        taskStateChanged(nbRunningOrPending, nbSuccess, nbFailed) {
+            if (nbRunningOrPending == 0 && this._nbRunningOrPending > 0) {
+                // All tasks finished, reload card
+                this.updateCard();
+            }
+            this._nbRunningOrPending = nbRunningOrPending;
+            this._nbSuccess = nbSuccess;
+            this._nbFailed = nbFailed;
         }
-      },
-      computed: {
+    },
+    computed: {
         contactMechanicsPlots: function () {
-          return [{
-            title: "Contact area vs load",
-            xData: "data.mean_pressures",
-            yData: "data.total_contact_areas",
-            auxiliaryDataColumns: {dataPath: "data.data_paths"},
-            alphaData: "data.converged.map((value) => value ? 1.0 : 0.3)",
-            xAxisLabel: "Normalized pressure p/E*",
-            yAxisLabel: "Fractional contact area A/A0",
-            xAxisType: "log",
-            yAxisType: "log"
-          }, {
-            title: "Load vs displacement",
-            xData: "data.mean_gaps",
-            yData: "data.mean_pressures",
-            auxiliaryDataColumns: {dataPath: "data.data_paths"},
-            alphaData: "data.converged.map((value) => value ? 1.0 : 0.3)",
-            xAxisLabel: "Normalized mean gap u/h_rms",
-            yAxisLabel: "Normalized pressure p/E*",
-            xAxisType: "linear",
-            yAxisType: "log"
-          }]
+            return [{
+                title: "Contact area vs load",
+                xData: "data.mean_pressures",
+                yData: "data.total_contact_areas",
+                auxiliaryDataColumns: {
+                    dataPath: "data.data_paths"
+                },
+                alphaData: "data.converged.map((value) => value ? 1.0 : 0.3)",
+                xAxisLabel: "$$p/E^*$$",
+                yAxisLabel: "$$A/A_0$$",
+                xAxisType: "log",
+                yAxisType: "log"
+            }, {
+                title: "Load vs displacement",
+                xData: "data.mean_gaps",
+                yData: "data.mean_pressures",
+                auxiliaryDataColumns: {
+                    dataPath: "data.data_paths"
+                },
+                alphaData: "data.converged.map((value) => value ? 1.0 : 0.3)",
+                xAxisLabel: "$$u/h_\\text{rms}$$",
+                yAxisLabel: "$$p/E^*$$",
+                xAxisType: "linear",
+                yAxisType: "log"
+            }]
         },
         contactMechanicsCategories: function () {
-          return [{key: "subject_name", title: "Measurements"}];
+            return [{key: "subjectName", title: "Measurements"}];
         },
         distributionPlots: function () {
-          return [{
-            title: "Pressure",
-            xData: "data.pressure",
-            yData: "data.pressureProbabilityDensity",
-            xAxisLabel: "Pressure p (E*)",
-            yAxisLabel: "Probability density P(p) (E*⁻¹)"
-          }, {
-            title: "Gap",
-            xData: "data.gap.map((value) => data.gapSIScaleFactor * value)",
-            yData: "data.gapProbabilityDensity.map((value) => data.gapProbabilityDensitySIScaleFactor * value)",
-            xAxisLabel: "Gap g (m)",
-            yAxisLabel: "Probability density P(g) (m⁻¹)"
-          }, {
-            title: "Cluster area",
-            xData: "data.clusterArea.map((value) => data.clusterAreaSIScaleFactor * value)",
-            yData: "data.clusterAreaProbabilityDensity.map((value) => data.clusterAreaProbabilityDensitySIScaleFactor * value)",
-            xAxisLabel: "Cluster area A (m²)",
-            yAxisLabel: "Probability density P(A) (m⁻²)"
-          }];
+            return [{
+                title: "Pressure",
+                xData: "data.pressure",
+                yData: "data.pressureProbabilityDensity",
+                xAxisLabel: "$$p\\text{ (}E^*\\text{)}$$",
+                yAxisLabel: "$$P(p)\\text{ (}E^{*-1}\\text{)}$$"
+            }, {
+                title: "Gap",
+                xData: "data.gap.map((value) => data.gapSIScaleFactor * value)",
+                yData: "data.gapProbabilityDensity.map((value) => data.gapProbabilityDensitySIScaleFactor * value)",
+                xAxisLabel: "$$g\\text{ (m)}$$",
+                yAxisLabel: "$$P(g)\\text{ (m}^{-1}\\text{)}$$"
+            }, {
+                title: "Cluster area",
+                xData: "data.clusterArea.map((value) => data.clusterAreaSIScaleFactor * value)",
+                yData: "data.clusterAreaProbabilityDensity.map((value) => data.clusterAreaProbabilityDensitySIScaleFactor * value)",
+                xAxisLabel: "$$A\\text{ (m}^2\\text{)}$$",
+                yAxisLabel: "$$P(A)\\text{ (m}^{-2}\\text{)}$$"
+            }];
         },
         distributionDataSources: function () {
-          return [{
-            url: "{% url 'analysis:data' pk=123 location='step-456/json/distributions.json' %}".replace('123/step-456', this.selection.analysis_id + '/' + this.selection.data_path)
-          }];
-        }
-      },
-      methods: {
-        recalculate: function () {
-          this.recalculateWarning = false;
-
-          if (this.pressureSelection == "automatic") {
-            if (this.nsteps < {{ limits_calc_kwargs.nsteps.min }}) {
-              this.nsteps = {{ limits_calc_kwargs.nsteps.min }};
-              this.recalculateWarning = true;
-            }
-            if (this.nsteps > {{ limits_calc_kwargs.nsteps.max }}) {
-              this.nsteps = {{ limits_calc_kwargs.nsteps.max }};
-              this.recalculateWarning = true;
-            }
-          } else { // pressure_selection_mode == "manual"
-            const originalLength = this.pressures.length;
-            this.pressures = this.pressures.map(parseFloat);
-            this.pressures = this.pressures.filter((p) => {
-              return (p != null) && (p > 0)
-            });
-            if (originalLength > this.pressures.length) {
-              this.recalculateWarning = true;
-            }
-            if (this.pressures.length < 1) {
-              this.pressures = [1];
-              this.recalculateWarning = true;
-            } else if (this.pressures.length > {{ limits_calc_kwargs.pressures.maxlen }}) {
-              this.pressures.length = {{ limits_calc_kwargs.pressures.maxlen }};
-              this.recalculateWarning = true;
-            }
-          }
-
-          if (this.maxNbIter < {{ limits_calc_kwargs.maxiter.min }}) {
-            this.maxNbIter = {{ limits_calc_kwargs.maxiter.min }};
-            this.recalculateWarning = true;
-          }
-          if (this.maxNbIter > {{ limits_calc_kwargs.maxiter.max }}) {
-            this.maxNbIter = {{ limits_calc_kwargs.maxiter.max }};
-            this.recalculateWarning = true;
-          }
-
-          if (this.recalculateWarning) {
-            // Return here if some parameters were modified
-            return;
-          }
-
-          const function_kwargs = {
-            substrate_str: this.periodicity,
-            hardness: parseFloat(this.hardness),
-            nsteps: this.pressureSelection == "automatic" ? parseInt(this.nsteps) : null,
-            pressures: this.pressureSelection == "manual" ? this.pressures : null,
-            maxiter: parseInt(this.maxNbIter)
-          };
-
-          // FIXME! Switch to fetch API, but there is some weirdness with CSRF tokens going on
-          $.ajax({
-            type: "POST",
-            url: "{% url 'analysis:card-submit' %}",
-            timeout: 0,
-            data: {
-              function_id: {{ function.id }},
-              subjects_ids_json: JSON.stringify({{ subjects_ids_json|safe }}),
-              function_kwargs_json: JSON.stringify(function_kwargs),
-              csrfmiddlewaretoken: "{{csrf_token}}"
-            },
-            success: (data, textStatus, xhr) => {
-              // debug_msg("Job submission successful. Status: "+xhr.status+" textStatus: "+textStatus);
-              if (xhr.status == 200) {
-                submit_analyses_card_ajax(
-                    "{% url 'analysis:card' %}",
-                    "card-wrapper", "contact-mechanics-card",
-                    "detail", {{ function.id }}, {{ subjects_ids_json|safe }}, 0);
-                // debug_msg("Triggered card reload. Status: "+xhr.status+" textStatus: "+textStatus);
-              } else {
-                this.errorMessage = "Triggering calculation failed, status: " + xhr.status + " response:" + xhr.responseText;
-              }
-            },
-            error: (xhr, textStatus, errorThrown) => {
-              console.log("AJAX error when submitting jobs: errorThrown: " + errorThrown + " status: " + xhr.status + " responseText: " + xhr.responseText);
-              this.errorMessage = "Please report this error: " + errorThrown + xhr.status + xhr.responseText;
-            }
-          });
+            return [{
+                url: `/analysis/data/${this._selection.analysisId}/${this._selection.dataPath}/json/distributions.json`
+            }];
         },
-        onSelected: function (obj, data) {
-          const name = data.source.name;
-          const path = data.source.data.dataPath[data.source.selected.indices[0]];
-          const split_path = path.split('/');
-          this.selection = {
-            analysis_id: name.split('-')[1],
-            data_path: split_path[split_path.length - 1]  // We need to do some name mangling
-          };
+        analysisIds() {
+            return this._analyses.map(a => a.id).join();
         }
-      }
-    });
-  </script>
-{% endblock card_javascript %}
+    }
+};
+</script>
+
+<template>
+    <div class="card search-result-card">
+        <div class="card-header">
+            <div class="btn-group btn-group-sm float-right">
+                <tasks-button v-if="_analyses !== null && _analyses.length > 0"
+                              :analyses="_analyses"
+                              :csrf-token="csrfToken"
+                              @task-state-changed="taskStateChanged">
+                </tasks-button>
+                <button v-if="_analyses !== null && _analyses.length > 0"
+                        @click="updateCard"
+                        class="btn btn-default float-right ml-1">
+                    <i class="fa fa-redo"></i>
+                </button>
+                <card-expand-button v-if="!enlarged"
+                                    :detail-url="detailUrl"
+                                    :function-id="functionId"
+                                    :subjects="subjects"
+                                    class="btn-group btn-group-sm float-right">
+                </card-expand-button>
+            </div>
+            <h5 v-if="_analyses === null"
+                class="text-dark">
+                Contact mechanics
+            </h5>
+            <a v-if="_analyses !== null && _analyses.length > 0"
+               class="text-dark"
+               href="#"
+               @click="_sidebarVisible=true">
+                <h5><i class="fa fa-bars"></i> Contact mechanics</h5>
+            </a>
+        </div>
+        <div class="card-body">
+            <div v-if="_cardStatus == 'mounted'" class="tab-content">
+                <span class="spinner"></span>
+                <div>Please wait...</div>
+            </div>
+            <div v-if="_cardStatus == 'waiting-for-first-result'" class="tab-content">
+                <span class="spinner"></span>
+                <div>
+                    Analyses are not yet available, but tasks are scheduled or running.
+                    Please wait...
+                </div>
+            </div>
+
+            <div v-if="_cardStatus != 'waiting-for-first-result' && _dataSources.length > 0" class="tab-content row">
+                <div :class="{ 'col-sm-5': enlarged, 'col-sm-12': !enlarged }">
+                    <div class="tab-pane show active" id="plot-{{ card_id }}" role="tabpanel"
+                         aria-labelledby="card-tab">
+                        <bokeh-plot
+                            :plots="contactMechanicsPlots"
+                            :categories="contactMechanicsCategories"
+                            :data-sources="_dataSources"
+                            :selectable="enlarged"
+                            @selected="onSelected"
+                            :options-widgets="['layout', 'legend', 'lineWidth', 'symbolSize']"
+                            :output-backend="_outputBackend"
+                            ref="plot">
+                        </bokeh-plot>
+                    </div>
+                </div>
+
+                <!-- Middle with group of tabs -->
+                <div v-if="enlarged"
+                     class="col-2 col-sm-2 col-md-2 col-lg-2">
+
+                    <div class="nav nav-pills nav-pills-custom flex-column" aria-orientation="vertical">
+                        <a class="nav-link mb-3 p-3 shadow active" data-toggle="pill" href="#contacting-points-tab"
+                           role="tab"
+                           aria-selected="true">
+                            Contact geometry
+                        </a>
+                        <a class="nav-link mb-3 p-3 shadow" data-toggle="pill" href="#pressure-tab" role="tab"
+                           aria-selected="false">
+                            Contact pressure
+                        </a>
+                        <a class="nav-link mb-3 p-3 shadow" data-toggle="pill" href="#displacement-tab" role="tab"
+                           aria-selected="false">
+                            Displacement
+                        </a>
+                        <a class="nav-link mb-3 p-3 shadow" data-toggle="pill" href="#gap-tab" role="tab"
+                           aria-selected="false">
+                            Gap
+                        </a>
+                        <a class="nav-link mb-3 p-3 shadow" data-toggle="pill" href="#distribution-function-tab"
+                           role="tab"
+                           aria-selected="false">
+                            Distribution functions
+                        </a>
+                    </div>
+
+                </div>
+
+                <!-- Right with simulation details and actions -->
+                <div v-if="enlarged" class="col-sm-5">
+                    <!-- Tab contents on right side -->
+                    <div class="tab-content">
+                        <div class="tab-pane fade active show" id="contacting-points-tab">
+                            <div v-if="_selection === null" id="geometry" class="alert alert-info">For contact geometry,
+                                select a point
+                                in the graphs on the left!
+                            </div>
+                            <deep-zoom-image v-if="_selection !== null"
+                                             :prefix-url="`/analysis/data/${_selection.analysisId}/${_selection.dataPath}/dzi/contacting-points/`"
+                                             ref="contactingPoints">
+                            </deep-zoom-image>
+                            <div v-if="_selection !== null" class="pull-right">
+                                <a class="btn btn-default btn-block btn-lg mt-3"
+                                   v-on:click="$refs.contactingPoints.download()">
+                                    Download PNG
+                                </a>
+                            </div>
+                        </div>
+                        <div class="tab-pane fade" id="pressure-tab">
+                            <div v-if="_selection === null" id="pressure" class="alert alert-info">For contact pressure,
+                                select a point
+                                in the graphs on the left!
+                            </div>
+                            <deep-zoom-image v-if="_selection !== null"
+                                             :prefix-url="`/analysis/data/${_selection.analysisId}/${_selection.dataPath}/dzi/pressure/`"
+                                             :colorbar="true"
+                                             ref="pressure">
+                            </deep-zoom-image>
+                            <div v-if="_selection !== null" class="pull-right">
+                                <a class="btn btn-default btn-block btn-lg" v-on:click="$refs.pressure.download()">
+                                    Download PNG
+                                </a>
+                            </div>
+                        </div>
+                        <div class="tab-pane fade" id="displacement-tab">
+                            <div v-if="_selection === null" id="displacement" class="alert alert-info">For displacement,
+                                select a point
+                                in the graphs on the left!
+                            </div>
+                            <deep-zoom-image v-if="_selection !== null"
+                                             :prefix-url="`/analysis/data/${_selection.analysisId}/${_selection.dataPath}/dzi/displacement/`"
+                                             :colorbar="true"
+                                             ref="displacement">
+                            </deep-zoom-image>
+                            <div v-if="_selection !== null" class="pull-right">
+                                <a class="btn btn-default btn-block btn-lg" v-on:click="$refs.displacement.download()">
+                                    Download PNG
+                                </a>
+                            </div>
+                        </div>
+                        <div class="tab-pane fade" id="gap-tab">
+                            <div v-if="_selection === null" id="gap" class="alert alert-info">For gap, select a point in
+                                the graphs on
+                                the left!
+                            </div>
+                            <deep-zoom-image v-if="_selection !== null"
+                                             :prefix-url="`/analysis/data/${_selection.analysisId}/${_selection.dataPath}/dzi/gap/`"
+                                             :colorbar="true"
+                                             ref="gap">
+                            </deep-zoom-image>
+                            <div v-if="_selection !== null" class="pull-right">
+                                <a class="btn btn-default btn-block btn-lg" v-on:click="$refs.gap.download()">
+                                    Download PNG
+                                </a>
+                            </div>
+                        </div>
+                        <div class="tab-pane fade" id="distribution-function-tab">
+                            <div v-if="_selection === null" id="distribution-function" class="alert alert-info">For
+                                pressure
+                                distribution, select a point in the graphs on the left!
+                            </div>
+                            <bokeh-plot
+                                v-if="_selection !== null"
+                                :plots="distributionPlots"
+                                :data-sources="distributionDataSources"
+                                :output-backend="_outputBackend">
+                            </bokeh-plot>
+                        </div>
+                    </div>
+                </div>
+            </div>
+        </div>
+        <div v-if="_sidebarVisible"
+             class="position-absolute h-100">
+            <nav class="card-header navbar navbar-toggleable-xl bg-light flex-column align-items-start h-100">
+                <ul class="flex-column navbar-nav">
+                    <a class="text-dark"
+                       href="#"
+                       @click="_sidebarVisible=false">
+                        <h5><i class="fa fa-bars"></i> Contact mechanics</h5>
+                    </a>
+                    <li class="nav-item mb-1 mt-1">
+                        Download
+                        <div class="btn-group ml-1"
+                             role="group"
+                             aria-label="Download formats">
+                            <a class="btn btn-default"
+                               :href="`/analysis/download/${analysisIds}/zip`"
+                               @click="_sidebarVisible=false">
+                                ZIP
+                            </a>
+                            <a class="btn btn-default"
+                               @click="_sidebarVisible=false; $refs.plot.download()">
+                                SVG
+                            </a>
+                        </div>
+                    </li>
+                    <li class="nav-item mb-1 mt-1">
+                        <a class="btn btn-default w-100"
+                           href="#"
+                           data-toggle="modal"
+                           :data-target="`#bibliography-modal-${uid}`"
+                           @click="_sidebarVisible=false">
+                            Bibliography
+                        </a>
+                    </li>
+                    <hr>
+                    <li class="nav-item mb-1 mt-1">
+                        <a class="btn btn-primary w-100"
+                           href="#"
+                           data-toggle="modal"
+                           :data-target="`#contact-mechanics-parameters-modal-${uid}`"
+                           @click="_sidebarVisible=false">
+                            Parameters
+                        </a>
+                    </li>
+                </ul>
+            </nav>
+        </div>
+        <!-- card-header sets the margins identical to the card so the title appears at the same position -->
+    </div>
+    <bibliography-modal
+        :id="`bibliography-modal-${uid}`"
+        :dois="_dois">
+    </bibliography-modal>
+    <contact-mechanics-parameters-modal
+        v-if="_limitsToFunctionKwargs !== null && _functionKwargs !== null"
+        :id="`contact-mechanics-parameters-modal-${uid}`"
+        :limits-to-function-kwargs="_limitsToFunctionKwargs"
+        :function-kwargs="_functionKwargs"
+        @update-contact-kwargs="updateCardWithFunctionKwargs"
+        :csrf-token="csrfToken">
+    </contact-mechanics-parameters-modal>
+</template>
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `topobank-contact-1.0.0/topobank_contact/tests/test_downloads.py` & `topobank-contact-1.1.1/topobank_contact/tests/test_downloads.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import pytest
 import zipfile
 from io import BytesIO
 
 from django.shortcuts import reverse
 
 from ..downloads import download_contact_mechanics_analyses_as_zip
-from ..functions import ART_CONTACT_MECHANICS
 
 
 @pytest.mark.urls('topobank_contact.tests.urls')
 @pytest.mark.django_db
-def test_download_contact_analyses_to_zip(rf, example_contact_analysis):
-    request = rf.get(reverse('analysis:download',
-                             kwargs=dict(ids=str(example_contact_analysis.id),
-                                         art=ART_CONTACT_MECHANICS,
-                                         file_format='zip')))
+def test_download_contact_analyses_to_zip(api_rf, example_contact_analysis):
+    request = api_rf.get(reverse('analysis:download',
+                                 kwargs=dict(ids=str(example_contact_analysis.id),
+                                             file_format='zip')))
 
     response = download_contact_mechanics_analyses_as_zip(request, [example_contact_analysis])
 
     archive = zipfile.ZipFile(BytesIO(response.content))
 
     expected_filenames = [
         "README.txt",
@@ -28,20 +26,20 @@
         f"{example_contact_analysis.subject.name}/result-step-1.nc",
         f"{example_contact_analysis.subject.name}/result-step-2.nc",
         f"{example_contact_analysis.subject.name}/result-step-3.nc",
     ]
 
     assert sorted(expected_filenames) == sorted(archive.namelist())
 
-    exp_plot_content = ",Normalized pressure p/E*,Fractional contact area A/A0,Normalized mean gap u/h_rms,converged,filename\n"\
-            "0,1,2,4,True,result-step-0.nc\n"\
-            "1,2,4,6,True,result-step-1.nc\n"\
-            "2,3,6,8,False,result-step-2.nc\n"\
-            "3,4,8,10,True,result-step-3.nc\n"
+    exp_plot_content = ",Normalized pressure p/E*,Fractional contact area A/A0,Normalized mean gap u/h_rms,converged,filename\n" \
+                       "0,1,2,4,True,result-step-0.nc\n" \
+                       "1,2,4,6,True,result-step-1.nc\n" \
+                       "2,3,6,8,False,result-step-2.nc\n" \
+                       "3,4,8,10,True,result-step-3.nc\n"
 
     plot_content = archive.read(f"{example_contact_analysis.subject.name}/plot.csv")
     assert plot_content.decode('utf-8') == exp_plot_content
 
     # Howto test info.txt? Content is based on a function in topobank, so it should be tested there
 
     readme_content = archive.read(f"README.txt")
-    assert b"Accessing the CSV file" in readme_content
+    assert b"Accessing the CSV file" in readme_content
```

### Comparing `topobank-contact-1.0.0/topobank_contact/tests/test_functions.py` & `topobank-contact-1.1.1/topobank_contact/tests/test_functions.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,83 +1,56 @@
 import pytest
 import numpy as np
 
-from SurfaceTopography import Topography as STTopography, NonuniformLineScan as STNonuniformLineScan
+from SurfaceTopography import NonuniformLineScan as STNonuniformLineScan
 
 from topobank.analysis.functions import IncompatibleTopographyException
-from ..functions import contact_mechanics
 from topobank.analysis.tests.utils import FakeTopographyModel, DummyProgressRecorder, simple_linear_2d_topography
 
+from ..functions import contact_mechanics
 
 
 def test_contact_mechanics_incompatible_topography():
     x = np.arange(10)
     arr = 2 * x
     t = STNonuniformLineScan(x, arr, unit='nm').detrend("center")
     topography = FakeTopographyModel(t)
 
     with pytest.raises(IncompatibleTopographyException):
         contact_mechanics(topography)
 
 
 def test_contact_mechanics_whether_given_pressures_in_result(simple_linear_2d_topography):
-
     given_pressures = [2e-3, 1e-2]
     topography = FakeTopographyModel(simple_linear_2d_topography)
     result = contact_mechanics(topography,
                                nsteps=None, pressures=given_pressures, storage_prefix='test/',
                                progress_recorder=DummyProgressRecorder())
 
     np.testing.assert_almost_equal(result['mean_pressures'], given_pressures)
 
 
-@pytest.mark.parametrize('periodic', [True, False])
-def test_contact_mechanics_effective_kwargs_in_result(periodic):
-    y = np.arange(10).reshape((1, -1))
-    x = np.arange(5).reshape((-1, 1))
-
-    arr = -2 * y + 0 * x  # only slope in y direction
-
-    t = STTopography(arr, (10, 5), unit='nm', periodic=periodic).detrend('center')
-
-    topography = FakeTopographyModel(t)
-    result = contact_mechanics(topography, substrate_str=None, nsteps=10, storage_prefix='test/',
-                               progress_recorder=DummyProgressRecorder())
-
-    exp_effective_kwargs = dict(
-        substrate_str=('' if periodic else 'non') + 'periodic',
-        nsteps=10,
-        pressures=None,
-        hardness=None,
-        maxiter=100,
-    )
-    assert result['effective_kwargs'] == exp_effective_kwargs
-
-
-
 @pytest.mark.parametrize(["x_dim", "y_dim"], [[20000, 10000], [9999999, 3]])
 def test_exception_topography_too_large_for_contact_mechanics(x_dim, y_dim, mocker, simple_linear_2d_topography):
     topo = FakeTopographyModel(simple_linear_2d_topography)
 
     # patch raw topography in order to return a higher number of grid points
     m = mocker.patch("SurfaceTopography.Topography.nb_grid_pts", new_callable=mocker.PropertyMock)
     m.return_value = (x_dim, y_dim)  # this make the topography returning high numbers of grid points
 
     with pytest.raises(IncompatibleTopographyException):
         contact_mechanics(topo, storage_prefix='test')
 
 
-
 @pytest.mark.parametrize(["topo_is_periodic", "substrate_str", "exp_num_alerts"], [
     [False, 'nonperiodic', 0],
     [False, 'periodic', 1],
     [True, 'nonperiodic', 1],
     [True, 'periodic', 0],
 ])
 def test_alert_if_topographys_periodicity_does_not_match(simple_linear_2d_topography,
                                                          topo_is_periodic, substrate_str, exp_num_alerts):
     topo = FakeTopographyModel(simple_linear_2d_topography, is_periodic=topo_is_periodic)
     result = contact_mechanics(topo, substrate_str=substrate_str, storage_prefix='test',
                                progress_recorder=DummyProgressRecorder())
-    assert len(result['alerts']) == exp_num_alerts
-
 
+    assert len(result['alerts']) == exp_num_alerts
```

### Comparing `topobank-contact-1.0.0/topobank_contact/tests/urls.py` & `topobank-contact-1.1.1/topobank_contact/tests/urls.py`

 * *Files identical despite different names*

### Comparing `topobank-contact-1.0.0/topobank_contact/tests/utils.py` & `topobank-contact-1.1.1/topobank_contact/tests/utils.py`

 * *Files identical despite different names*

### Comparing `topobank-contact-1.0.0/topobank_contact.egg-info/SOURCES.txt` & `topobank-contact-1.1.1/topobank_contact.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 .gitignore
 CHANGELOG.md
 LICENSE
 MANIFEST.in
-README
+README.rst
 conftest.py
 pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
 .github/workflows/publish.yml
 .github/workflows/test.yml
 .idea/.gitignore
-config/__init__.py
-config/settings/__init__.py
-config/settings/base.py
-config/settings/test.py
 topobank_contact/__init__.py
 topobank_contact/apps.py
 topobank_contact/downloads.py
 topobank_contact/functions.py
 topobank_contact/models.py
 topobank_contact/signals.py
 topobank_contact/urls.py
 topobank_contact/views.py
 topobank_contact.egg-info/PKG-INFO
 topobank_contact.egg-info/SOURCES.txt
 topobank_contact.egg-info/dependency_links.txt
 topobank_contact.egg-info/entry_points.txt
 topobank_contact.egg-info/requires.txt
 topobank_contact.egg-info/top_level.txt
+topobank_contact/frontend/ContactMechanicsCard.vue
+topobank_contact/frontend/ContactMechanicsParametersModal.vue
+topobank_contact/frontend/contact_mechanics_card.js
 topobank_contact/migrations/__init__.py
 topobank_contact/static/images/ce_logo.svg
-topobank_contact/templates/topobank_contact/contact_mechanics_card_detail.html
-topobank_contact/templates/topobank_contact/contact_mechanics_card_list.html
 topobank_contact/tests/__init__.py
 topobank_contact/tests/test_downloads.py
 topobank_contact/tests/test_functions.py
 topobank_contact/tests/test_views.py
 topobank_contact/tests/urls.py
 topobank_contact/tests/utils.py
```

