# Comparing `tmp/django-pygwalker-0.0.2.tar.gz` & `tmp/django-pygwalker-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pygwalker-0.0.2.tar", last modified: Tue Aug  1 02:14:12 2023, max compression
+gzip compressed data, was "django-pygwalker-0.0.3.tar", last modified: Fri Aug  4 05:09:13 2023, max compression
```

## Comparing `django-pygwalker-0.0.2.tar` & `django-pygwalker-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    46845 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.706181 django-pygwalker-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-01 02:14:12.000000 django-pygwalker-0.0.2/src/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/src/django_pygwalker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    46845 2023-08-01 02:14:12.000000 django-pygwalker-0.0.2/src/django_pygwalker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-08-01 02:14:12.000000 django-pygwalker-0.0.2/src/django_pygwalker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 02:14:12.000000 django-pygwalker-0.0.2/src/django_pygwalker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-01 02:14:12.000000 django-pygwalker-0.0.2/src/django_pygwalker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 02:14:12.000000 django-pygwalker-0.0.2/src/django_pygwalker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/src/djangoaddicts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/src/djangoaddicts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.706181 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.706181 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/templates/pygwalker/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 02:14:12.710181 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pygwalker.html
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-08-01 02:13:55.000000 django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:09:13.051446 django-pygwalker-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    47320 2023-08-04 05:09:13.051446 django-pygwalker-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 05:09:13.051446 django-pygwalker-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:09:13.051446 django-pygwalker-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 05:09:12.000000 django-pygwalker-0.0.3/src/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:09:13.051446 django-pygwalker-0.0.3/src/django_pygwalker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47320 2023-08-04 05:09:13.000000 django-pygwalker-0.0.3/src/django_pygwalker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-08-04 05:09:13.000000 django-pygwalker-0.0.3/src/django_pygwalker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 05:09:13.000000 django-pygwalker-0.0.3/src/django_pygwalker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-04 05:09:13.000000 django-pygwalker-0.0.3/src/django_pygwalker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 05:09:13.000000 django-pygwalker-0.0.3/src/django_pygwalker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:09:13.051446 django-pygwalker-0.0.3/src/djangoaddicts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/djangoaddicts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:09:13.051446 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:09:13.047446 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:09:13.047446 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/templates/pygwalker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:09:13.051446 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 05:09:13.051446 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/partials/file_upload.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/partials/footer.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/partials/header.htm
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/partials/pyg.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/partials/pygwalker_nav_menu.htm
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pygwalker.html
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/templates/pygwalker/bs5/pygwalker_dynamic.html
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-08-04 05:08:55.000000 django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/views.py
```

### Comparing `django-pygwalker-0.0.2/LICENSE` & `django-pygwalker-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pygwalker-0.0.2/PKG-INFO` & `django-pygwalker-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: django-pygwalker
-Version: 0.0.2
+Version: 0.0.3
+Summary: PyGWalker views for Django projects
 Author-email: David Slusser <dbslusser@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -673,14 +674,16 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
+Project-URL: homepage, https://github.com/djangoaddicts/django-pygwalker
+Project-URL: repository, https://github.com/djangoaddicts/django-pygwalker
 Keywords: django,visualization,data-analysis,data-exploration,tableau,tableau-alternative
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
@@ -703,17 +706,16 @@
 # django-pygwalker
 [![Downloads](https://static.pepy.tech/badge/django-pygwalker)](https://pepy.tech/project/django-pygwalker)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7682/badge)](https://bestpractices.coreinfrastructure.org/projects/7682)
 
 ![PyPI - Python](https://img.shields.io/pypi/pyversions/django-pygwalker)
 ![PyPI - Django](https://img.shields.io/pypi/djversions/django-pygwalker)
 
-Turn your Django querysets into user interfaces for visual analysis with PyGWalker.
+This utility creates user interfaces for visual analysis using PyGWalker in your django application. A PyGWalker page can be created from a Django queryset, a static csv file, or an uploaded csv file.
 
-This utility creates user interfaces based on your Django querysets for visual analysis using PyGwalker. 
 For more information on PyGWalker see the github repo available here: https://github.com/Kanaries/pygwalker 
 
 
 <br/>
 
 ## Code Quality
 | Workflow | Description             | Status                                                                       |
@@ -763,15 +765,22 @@
     ```
 - add the following to your INSTALLED_APPS in settings.py:
 
     ```python 
     djangoaddicts.pygwalker
     ```
 
-    ***NOTE:*** *adding djangoaddicts.pygwalker to INSTALLED_APPS is only required if you intend to use the built-in templates.* 
+    ***NOTE:*** *adding djangoaddicts.pygwalker to INSTALLED_APPS is only required if you intend to use the built-in templates or the 'generic' PyGWalker view.* 
+
+- to include the generic PyGWalker view (creates the PyGWalker page from an upload of a csv file) add the following to your project-level urls.py:
+
+    ```python
+    path("pygwalker/", include("djangoaddicts.pygwalker.urls"), ),
+    ```
+
 
 <br/>
 
 ## Features
 
 ### PygWalkerView
 The PygWalkerView renders a page containing PyGWalker html. This view takes a queryset parameter and includes all data in the queryset for visualizations. By default fields defined in the model will be included. To exclude fields or include additional fields (such as related fields), use the field_list parameter to specify exact fields desired for visualizations.
```

### Comparing `django-pygwalker-0.0.2/README.md` & `django-pygwalker-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # django-pygwalker
 [![Downloads](https://static.pepy.tech/badge/django-pygwalker)](https://pepy.tech/project/django-pygwalker)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7682/badge)](https://bestpractices.coreinfrastructure.org/projects/7682)
 
 ![PyPI - Python](https://img.shields.io/pypi/pyversions/django-pygwalker)
 ![PyPI - Django](https://img.shields.io/pypi/djversions/django-pygwalker)
 
-Turn your Django querysets into user interfaces for visual analysis with PyGWalker.
+This utility creates user interfaces for visual analysis using PyGWalker in your django application. A PyGWalker page can be created from a Django queryset, a static csv file, or an uploaded csv file.
 
-This utility creates user interfaces based on your Django querysets for visual analysis using PyGwalker. 
 For more information on PyGWalker see the github repo available here: https://github.com/Kanaries/pygwalker 
 
 
 <br/>
 
 ## Code Quality
 | Workflow | Description             | Status                                                                       |
@@ -61,15 +60,22 @@
     ```
 - add the following to your INSTALLED_APPS in settings.py:
 
     ```python 
     djangoaddicts.pygwalker
     ```
 
-    ***NOTE:*** *adding djangoaddicts.pygwalker to INSTALLED_APPS is only required if you intend to use the built-in templates.* 
+    ***NOTE:*** *adding djangoaddicts.pygwalker to INSTALLED_APPS is only required if you intend to use the built-in templates or the 'generic' PyGWalker view.* 
+
+- to include the generic PyGWalker view (creates the PyGWalker page from an upload of a csv file) add the following to your project-level urls.py:
+
+    ```python
+    path("pygwalker/", include("djangoaddicts.pygwalker.urls"), ),
+    ```
+
 
 <br/>
 
 ## Features
 
 ### PygWalkerView
 The PygWalkerView renders a page containing PyGWalker html. This view takes a queryset parameter and includes all data in the queryset for visualizations. By default fields defined in the model will be included. To exclude fields or include additional fields (such as related fields), use the field_list parameter to specify exact fields desired for visualizations.
```

### Comparing `django-pygwalker-0.0.2/pyproject.toml` & `django-pygwalker-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
     "django",
     "pandas",
     "pygwalker",
 ]
-description = ""
+description = "PyGWalker views for Django projects"
 dynamic = ["version"]
 keywords = ["django", "visualization", "data-analysis", "data-exploration", "tableau", "tableau-alternative",]
 license = {file = "LICENSE"}
 name = "django-pygwalker"
 readme = "README.md"
 requires-python = ">=3.8"
 
@@ -71,14 +71,19 @@
 docs = [
     "sphinx",
     "sphinx-rtd-theme",
     "myst-parser",
 ]
 
 
+[project.urls]
+homepage = "https://github.com/djangoaddicts/django-pygwalker"
+repository = "https://github.com/djangoaddicts/django-pygwalker"
+
+
 [tool.bandit]
 exclude_dirs = ["venv", "tests"]
 
 
 [tool.black]
 line-length = 120
```

### Comparing `django-pygwalker-0.0.2/src/django_pygwalker.egg-info/PKG-INFO` & `django-pygwalker-0.0.3/src/django_pygwalker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Metadata-Version: 2.1
 Name: django-pygwalker
-Version: 0.0.2
+Version: 0.0.3
+Summary: PyGWalker views for Django projects
 Author-email: David Slusser <dbslusser@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -673,14 +674,16 @@
           The GNU General Public License does not permit incorporating your program
         into proprietary programs.  If your program is a subroutine library, you
         may consider it more useful to permit linking proprietary applications with
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
+Project-URL: homepage, https://github.com/djangoaddicts/django-pygwalker
+Project-URL: repository, https://github.com/djangoaddicts/django-pygwalker
 Keywords: django,visualization,data-analysis,data-exploration,tableau,tableau-alternative
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
@@ -703,17 +706,16 @@
 # django-pygwalker
 [![Downloads](https://static.pepy.tech/badge/django-pygwalker)](https://pepy.tech/project/django-pygwalker)
 [![OpenSSF Best Practices](https://bestpractices.coreinfrastructure.org/projects/7682/badge)](https://bestpractices.coreinfrastructure.org/projects/7682)
 
 ![PyPI - Python](https://img.shields.io/pypi/pyversions/django-pygwalker)
 ![PyPI - Django](https://img.shields.io/pypi/djversions/django-pygwalker)
 
-Turn your Django querysets into user interfaces for visual analysis with PyGWalker.
+This utility creates user interfaces for visual analysis using PyGWalker in your django application. A PyGWalker page can be created from a Django queryset, a static csv file, or an uploaded csv file.
 
-This utility creates user interfaces based on your Django querysets for visual analysis using PyGwalker. 
 For more information on PyGWalker see the github repo available here: https://github.com/Kanaries/pygwalker 
 
 
 <br/>
 
 ## Code Quality
 | Workflow | Description             | Status                                                                       |
@@ -763,15 +765,22 @@
     ```
 - add the following to your INSTALLED_APPS in settings.py:
 
     ```python 
     djangoaddicts.pygwalker
     ```
 
-    ***NOTE:*** *adding djangoaddicts.pygwalker to INSTALLED_APPS is only required if you intend to use the built-in templates.* 
+    ***NOTE:*** *adding djangoaddicts.pygwalker to INSTALLED_APPS is only required if you intend to use the built-in templates or the 'generic' PyGWalker view.* 
+
+- to include the generic PyGWalker view (creates the PyGWalker page from an upload of a csv file) add the following to your project-level urls.py:
+
+    ```python
+    path("pygwalker/", include("djangoaddicts.pygwalker.urls"), ),
+    ```
+
 
 <br/>
 
 ## Features
 
 ### PygWalkerView
 The PygWalkerView renders a page containing PyGWalker html. This view takes a queryset parameter and includes all data in the queryset for visualizations. By default fields defined in the model will be included. To exclude fields or include additional fields (such as related fields), use the field_list parameter to specify exact fields desired for visualizations.
```

### Comparing `django-pygwalker-0.0.2/src/djangoaddicts/pygwalker/views.py` & `django-pygwalker-0.0.3/src/djangoaddicts/pygwalker/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,30 @@
+import mimetypes
+
 import pandas as pd
 import pygwalker as pyg
+from django.conf import settings
+from django.contrib import messages
 from django.db.models import QuerySet
 from django.shortcuts import render
 from django.views.generic import View
 
+from djangoaddicts.pygwalker.forms import UploadFileForm
+
 
 class PygWalkerView(View):
     """View to create a PyGWalker visualization interface from a Django queryset.
     See https://github.com/Kanaries/pygwalker for more information on PyGWalker.
 
     class parameters:
-        field_list    - list of model fields to include (defaults to fields defined in the model)
+        field_list    - list of model fields to include; defaults to fields defined in the model
         queryset      - queryset providing data available to visualization
-        theme         - PyGWalker theme to use for pyg html (defaults to "media")
-        title         - title used on html render
         template_name - template used when rendering page; defaults to: pygwalker/bs5/pyg.html
+        theme         - PyGWalker theme to use for pyg html; defaults to: "media"
+        title         - title used on html render
 
     example:
 
         from djangoaddicts.pygwalker.views import PygWalkerView
         class MyPygView(PygWalkerView):
             queryset = Order.objects.all()
             title = "Order Data Analysis"
@@ -40,17 +46,17 @@
 
 class StaticCsvPygWalkerView(View):
     """View to create a PyGWalker visualization interface from a statically definied csv file.
     See https://github.com/Kanaries/pygwalker for more information on PyGWalker.
 
     class parameters:
         csv_file      - csv file containing data to visualize
-        theme         - PyGWalker theme to use for pyg html (defaults to "media")
-        title         - title used on html render
         template_name - template used when rendering page; defaults to: pygwalker/bs5/pyg.html
+        theme         - PyGWalker theme to use for pyg html; defaults to: "media"
+        title         - title used on html render
 
     example:
 
         from djangoaddicts.pygwalker.views import StaticCsvPygWalkerView
         class MyPygView(StaticCsvPygWalkerView):
             csv_file = "my_csv_file.csv
             title = "Order Data Analysis"
@@ -62,7 +68,54 @@
     theme: str = "media"
     title: str = "Data Analysis"
 
     def get(self, request):
         pd_data = pd.read_csv(self.csv_file)
         context = {"pyg": pyg.walk(pd_data, return_html=True, dark=self.theme), "title": self.title}
         return render(request, self.template_name, context)
+
+
+class DynamicCsvPygWalkerView(View):
+    """View to create a PyGWalker visualization interface from a provided csv file.
+    See https://github.com/Kanaries/pygwalker for more information on PyGWalker.
+
+    class parameters:
+        template_name - template used when rendering page; defaults to: pygwalker/bs5/pygwalker_dynamic.html
+        theme         - PyGWalker theme to use for pyg html; defaults to "media"
+        title         - title used on html render
+    """
+
+    template_name: str = "pygwalker/bs5/pygwalker_dynamic.html"
+    theme: str = getattr(settings, "PYGWALKER_THEME", "media")
+    title: str = "Upload a csv file"
+
+    def get(self, request):
+        context = {"form": UploadFileForm(), "title": "Upload a csv file"}
+        return render(request, self.template_name, context)
+
+    def post(self, request):
+        context = {}
+        form = UploadFileForm(request.POST, request.FILES)
+        if form.is_valid():
+            csv_file = form.cleaned_data["csv_file"]
+            if mimetypes.guess_type(csv_file.name)[0] not in ["text/csv"]:
+                messages.add_message(
+                    request, messages.ERROR, "file provided is not a csv file", extra_tags="alert-danger"
+                )
+                return render(request, self.template_name, context)
+            pd_data = pd.read_csv(csv_file)
+            context["pyg"] = pyg.walk(pd_data, return_html=True, dark=self.theme)
+            context[
+                "title"
+            ] = f"""Showing data from <span class="text-secondary">{csv_file.name.split("/")[-1]}</span>"""
+            return render(request, self.template_name, context)
+        else:
+            for error in form.errors:
+                for i in form.errors[error].data:
+                    for msg in i.messages:
+                        messages.add_message(
+                            self.request,
+                            messages.ERROR,
+                            msg,
+                            extra_tags="alert-danger",
+                        )
+        return self.get(request)
```

