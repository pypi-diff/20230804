# Comparing `tmp/django-pgviews-redux-0.9.2.tar.gz` & `tmp/django-pgviews-redux-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pgviews-redux-0.9.2.tar", last modified: Mon Apr  3 10:44:30 2023, max compression
+gzip compressed data, was "django-pgviews-redux-0.9.3.tar", last modified: Fri Aug  4 13:06:08 2023, max compression
```

## Comparing `django-pgviews-redux-0.9.2.tar` & `django-pgviews-redux-0.9.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-04-03 10:44:30.206005 django-pgviews-redux-0.9.2/
--rw-r--r--   0 miki      (1000) miki      (1000)        0 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.2/MANIFEST.in
--rw-r--r--   0 miki      (1000) miki      (1000)    14297 2023-04-03 10:44:30.206005 django-pgviews-redux-0.9.2/PKG-INFO
--rw-r--r--   0 miki      (1000) miki      (1000)    13390 2023-04-03 10:42:49.000000 django-pgviews-redux-0.9.2/README.md
-drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-04-03 10:44:30.206005 django-pgviews-redux-0.9.2/django_pgviews/
--rw-r--r--   0 miki      (1000) miki      (1000)        0 2023-02-27 15:28:30.000000 django-pgviews-redux-0.9.2/django_pgviews/__init__.py
--rw-r--r--   0 miki      (1000) miki      (1000)     1418 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.2/django_pgviews/apps.py
--rw-r--r--   0 miki      (1000) miki      (1000)      108 2023-04-03 10:16:45.000000 django-pgviews-redux-0.9.2/django_pgviews/compat.py
-drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-04-03 10:44:30.206005 django-pgviews-redux-0.9.2/django_pgviews/db/
--rw-r--r--   0 miki      (1000) miki      (1000)      772 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.2/django_pgviews/db/__init__.py
-drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-04-03 10:44:30.206005 django-pgviews-redux-0.9.2/django_pgviews/db/sql/
--rw-r--r--   0 miki      (1000) miki      (1000)        0 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.2/django_pgviews/db/sql/__init__.py
--rw-r--r--   0 miki      (1000) miki      (1000)      687 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.2/django_pgviews/db/sql/compiler.py
--rw-r--r--   0 miki      (1000) miki      (1000)      720 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.2/django_pgviews/db/sql/query.py
-drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-04-03 10:44:30.206005 django-pgviews-redux-0.9.2/django_pgviews/management/
--rw-r--r--   0 miki      (1000) miki      (1000)        0 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.2/django_pgviews/management/__init__.py
-drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-04-03 10:44:30.206005 django-pgviews-redux-0.9.2/django_pgviews/management/commands/
--rw-r--r--   0 miki      (1000) miki      (1000)        0 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.2/django_pgviews/management/commands/__init__.py
--rw-r--r--   0 miki      (1000) miki      (1000)     1415 2022-11-21 09:16:10.000000 django-pgviews-redux-0.9.2/django_pgviews/management/commands/clear_pgviews.py
--rw-r--r--   0 miki      (1000) miki      (1000)      828 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.2/django_pgviews/management/commands/refresh_pgviews.py
--rw-r--r--   0 miki      (1000) miki      (1000)     2628 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.2/django_pgviews/management/commands/sync_pgviews.py
--rw-r--r--   0 miki      (1000) miki      (1000)     5610 2022-11-21 09:16:10.000000 django-pgviews-redux-0.9.2/django_pgviews/models.py
--rw-r--r--   0 miki      (1000) miki      (1000)       88 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.2/django_pgviews/signals.py
--rw-r--r--   0 miki      (1000) miki      (1000)    17373 2023-04-03 10:16:45.000000 django-pgviews-redux-0.9.2/django_pgviews/view.py
-drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-04-03 10:44:30.206005 django-pgviews-redux-0.9.2/django_pgviews_redux.egg-info/
--rw-r--r--   0 miki      (1000) miki      (1000)    14297 2023-04-03 10:44:30.000000 django-pgviews-redux-0.9.2/django_pgviews_redux.egg-info/PKG-INFO
--rw-r--r--   0 miki      (1000) miki      (1000)      751 2023-04-03 10:44:30.000000 django-pgviews-redux-0.9.2/django_pgviews_redux.egg-info/SOURCES.txt
--rw-r--r--   0 miki      (1000) miki      (1000)        1 2023-04-03 10:44:30.000000 django-pgviews-redux-0.9.2/django_pgviews_redux.egg-info/dependency_links.txt
--rw-r--r--   0 miki      (1000) miki      (1000)       15 2023-04-03 10:44:30.000000 django-pgviews-redux-0.9.2/django_pgviews_redux.egg-info/top_level.txt
--rw-r--r--   0 miki      (1000) miki      (1000)      333 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.2/pyproject.toml
--rw-r--r--   0 miki      (1000) miki      (1000)       79 2023-04-03 10:44:30.206005 django-pgviews-redux-0.9.2/setup.cfg
--rw-r--r--   0 miki      (1000) miki      (1000)     1259 2023-04-03 10:42:49.000000 django-pgviews-redux-0.9.2/setup.py
+drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-08-04 13:06:08.623762 django-pgviews-redux-0.9.3/
+-rw-r--r--   0 miki      (1000) miki      (1000)        0 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.3/MANIFEST.in
+-rw-r--r--   0 miki      (1000) miki      (1000)    14297 2023-08-04 13:06:08.623762 django-pgviews-redux-0.9.3/PKG-INFO
+-rw-r--r--   0 miki      (1000) miki      (1000)    13390 2023-04-03 10:42:49.000000 django-pgviews-redux-0.9.3/README.md
+drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-08-04 13:06:08.623762 django-pgviews-redux-0.9.3/django_pgviews/
+-rw-r--r--   0 miki      (1000) miki      (1000)        0 2023-02-27 15:28:30.000000 django-pgviews-redux-0.9.3/django_pgviews/__init__.py
+-rw-r--r--   0 miki      (1000) miki      (1000)     1418 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.3/django_pgviews/apps.py
+-rw-r--r--   0 miki      (1000) miki      (1000)      108 2023-04-03 10:16:45.000000 django-pgviews-redux-0.9.3/django_pgviews/compat.py
+drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-08-04 13:06:08.623762 django-pgviews-redux-0.9.3/django_pgviews/db/
+-rw-r--r--   0 miki      (1000) miki      (1000)      772 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.3/django_pgviews/db/__init__.py
+drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-08-04 13:06:08.623762 django-pgviews-redux-0.9.3/django_pgviews/db/sql/
+-rw-r--r--   0 miki      (1000) miki      (1000)        0 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.3/django_pgviews/db/sql/__init__.py
+-rw-r--r--   0 miki      (1000) miki      (1000)      687 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.3/django_pgviews/db/sql/compiler.py
+-rw-r--r--   0 miki      (1000) miki      (1000)      720 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.3/django_pgviews/db/sql/query.py
+drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-08-04 13:06:08.623762 django-pgviews-redux-0.9.3/django_pgviews/management/
+-rw-r--r--   0 miki      (1000) miki      (1000)        0 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.3/django_pgviews/management/__init__.py
+drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-08-04 13:06:08.623762 django-pgviews-redux-0.9.3/django_pgviews/management/commands/
+-rw-r--r--   0 miki      (1000) miki      (1000)        0 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.3/django_pgviews/management/commands/__init__.py
+-rw-r--r--   0 miki      (1000) miki      (1000)     1415 2022-11-21 09:16:10.000000 django-pgviews-redux-0.9.3/django_pgviews/management/commands/clear_pgviews.py
+-rw-r--r--   0 miki      (1000) miki      (1000)      828 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.3/django_pgviews/management/commands/refresh_pgviews.py
+-rw-r--r--   0 miki      (1000) miki      (1000)     2628 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.3/django_pgviews/management/commands/sync_pgviews.py
+-rw-r--r--   0 miki      (1000) miki      (1000)     5610 2022-11-21 09:16:10.000000 django-pgviews-redux-0.9.3/django_pgviews/models.py
+-rw-r--r--   0 miki      (1000) miki      (1000)       88 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.3/django_pgviews/signals.py
+-rw-r--r--   0 miki      (1000) miki      (1000)    17450 2023-08-04 13:04:49.000000 django-pgviews-redux-0.9.3/django_pgviews/view.py
+drwxr-xr-x   0 miki      (1000) miki      (1000)        0 2023-08-04 13:06:08.623762 django-pgviews-redux-0.9.3/django_pgviews_redux.egg-info/
+-rw-r--r--   0 miki      (1000) miki      (1000)    14297 2023-08-04 13:06:08.000000 django-pgviews-redux-0.9.3/django_pgviews_redux.egg-info/PKG-INFO
+-rw-r--r--   0 miki      (1000) miki      (1000)      751 2023-08-04 13:06:08.000000 django-pgviews-redux-0.9.3/django_pgviews_redux.egg-info/SOURCES.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)        1 2023-08-04 13:06:08.000000 django-pgviews-redux-0.9.3/django_pgviews_redux.egg-info/dependency_links.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)       15 2023-08-04 13:06:08.000000 django-pgviews-redux-0.9.3/django_pgviews_redux.egg-info/top_level.txt
+-rw-r--r--   0 miki      (1000) miki      (1000)      333 2022-09-21 09:08:20.000000 django-pgviews-redux-0.9.3/pyproject.toml
+-rw-r--r--   0 miki      (1000) miki      (1000)       79 2023-08-04 13:06:08.623762 django-pgviews-redux-0.9.3/setup.cfg
+-rw-r--r--   0 miki      (1000) miki      (1000)     1259 2023-08-04 13:05:47.000000 django-pgviews-redux-0.9.3/setup.py
```

### Comparing `django-pgviews-redux-0.9.2/PKG-INFO` & `django-pgviews-redux-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgviews-redux
-Version: 0.9.2
+Version: 0.9.3
 Summary: Create and manage Postgres SQL Views in Django
 Home-page: https://github.com/xelixdev/django-pgviews-redux
 Author: Mikuláš Poul
 Author-email: git@mikulaspoul.cz
 License: Public Domain
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-pgviews-redux-0.9.2/README.md` & `django-pgviews-redux-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `django-pgviews-redux-0.9.2/django_pgviews/apps.py` & `django-pgviews-redux-0.9.3/django_pgviews/apps.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-redux-0.9.2/django_pgviews/db/__init__.py` & `django-pgviews-redux-0.9.3/django_pgviews/db/__init__.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-redux-0.9.2/django_pgviews/db/sql/compiler.py` & `django-pgviews-redux-0.9.3/django_pgviews/db/sql/compiler.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-redux-0.9.2/django_pgviews/db/sql/query.py` & `django-pgviews-redux-0.9.3/django_pgviews/db/sql/query.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-redux-0.9.2/django_pgviews/management/commands/clear_pgviews.py` & `django-pgviews-redux-0.9.3/django_pgviews/management/commands/clear_pgviews.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-redux-0.9.2/django_pgviews/management/commands/refresh_pgviews.py` & `django-pgviews-redux-0.9.3/django_pgviews/management/commands/refresh_pgviews.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-redux-0.9.2/django_pgviews/management/commands/sync_pgviews.py` & `django-pgviews-redux-0.9.3/django_pgviews/management/commands/sync_pgviews.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-redux-0.9.2/django_pgviews/models.py` & `django-pgviews-redux-0.9.3/django_pgviews/models.py`

 * *Files identical despite different names*

### Comparing `django-pgviews-redux-0.9.2/django_pgviews/view.py` & `django-pgviews-redux-0.9.3/django_pgviews/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 import django
 from django.apps import apps
 from django.core import exceptions
 from django.db import connections, router, transaction
 from django.db import models
 from django.db.backends.postgresql.schema import DatabaseSchemaEditor
+from django.db.backends.utils import truncate_name
 from django.db.models.query import QuerySet
 
 from django_pgviews.compat import ProgrammingError
 from django_pgviews.db import get_fields_by_name
 
 
 FIELD_SPEC_REGEX = r"^([A-Za-z_][A-Za-z0-9_]*)\." r"([A-Za-z_][A-Za-z0-9_]*)\." r"(\*|(?:[A-Za-z_][A-Za-z0-9_]*))$"
@@ -204,15 +205,15 @@
         view_exists = cursor.fetchone()[0] > 0
 
         query = view_query.query.strip()
         if query.endswith(";"):
             query = query[:-1]
 
         if check_sql_changed and view_exists:
-            temp_viewname = view_name + "_temp"
+            temp_viewname = truncate_name(view_name + "_temp", length=63)
             _, temp_vname = _schema_and_name(connection, temp_viewname)
 
             _drop_mat_view(cursor, temp_viewname)
             _create_mat_view(cursor, temp_viewname, query, view_query.params, with_data=False)
 
             cursor.execute(
                 "SELECT definition FROM pg_matviews WHERE schemaname = %s and matviewname IN (%s, %s);",
```

### Comparing `django-pgviews-redux-0.9.2/django_pgviews_redux.egg-info/PKG-INFO` & `django-pgviews-redux-0.9.3/django_pgviews_redux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgviews-redux
-Version: 0.9.2
+Version: 0.9.3
 Summary: Create and manage Postgres SQL Views in Django
 Home-page: https://github.com/xelixdev/django-pgviews-redux
 Author: Mikuláš Poul
 Author-email: git@mikulaspoul.cz
 License: Public Domain
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `django-pgviews-redux-0.9.2/django_pgviews_redux.egg-info/SOURCES.txt` & `django-pgviews-redux-0.9.3/django_pgviews_redux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-pgviews-redux-0.9.2/setup.py` & `django-pgviews-redux-0.9.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     LONG_DESCRIPTION = open("README.md").read()
 else:
     LONG_DESCRIPTION = ""
 
 
 setup(
     name="django-pgviews-redux",
-    version="0.9.2",
+    version="0.9.3",
     description="Create and manage Postgres SQL Views in Django",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     author="Mikuláš Poul",
     author_email="git@mikulaspoul.cz",
     license="Public Domain",
     packages=find_packages(),
```

