# Comparing `tmp/panther-1.7.9.tar.gz` & `tmp/panther-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panther-1.7.9.tar", last modified: Tue Jul  4 19:40:00 2023, max compression
+gzip compressed data, was "panther-2.0.0.tar", last modified: Fri Aug  4 12:43:24 2023, max compression
```

## Comparing `panther-1.7.9.tar` & `panther-2.0.0.tar`

### file list

```diff
@@ -1,59 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.239499 panther-1.7.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-04 19:39:46.000000 panther-1.7.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-04 19:40:00.239499 panther-1.7.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-04 19:39:46.000000 panther-1.7.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.235499 panther-1.7.9/panther/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-04 19:39:46.000000 panther-1.7.9/panther/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-04 19:39:46.000000 panther-1.7.9/panther/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-07-04 19:39:46.000000 panther-1.7.9/panther/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-07-04 19:39:46.000000 panther-1.7.9/panther/authentications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-07-04 19:39:46.000000 panther-1.7.9/panther/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.235499 panther-1.7.9/panther/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/create_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/monitor_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/run_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-07-04 19:39:46.000000 panther-1.7.9/panther/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-04 19:39:46.000000 panther-1.7.9/panther/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.239499 panther-1.7.9/panther/db/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.239499 panther-1.7.9/panther/db/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/queries/mongodb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/queries/pantherdb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/queries/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-04 19:39:46.000000 panther-1.7.9/panther/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-07-04 19:39:46.000000 panther-1.7.9/panther/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-04 19:39:46.000000 panther-1.7.9/panther/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-07-04 19:39:46.000000 panther-1.7.9/panther/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.239499 panther-1.7.9/panther/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-04 19:39:46.000000 panther-1.7.9/panther/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-04 19:39:46.000000 panther-1.7.9/panther/middlewares/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-04 19:39:46.000000 panther-1.7.9/panther/middlewares/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-04 19:39:46.000000 panther-1.7.9/panther/middlewares/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-04 19:39:46.000000 panther-1.7.9/panther/middlewares/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.239499 panther-1.7.9/panther/panel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-04 19:39:46.000000 panther-1.7.9/panther/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-04 19:39:46.000000 panther-1.7.9/panther/panel/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-04 19:39:46.000000 panther-1.7.9/panther/panel/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-04 19:39:46.000000 panther-1.7.9/panther/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-07-04 19:39:46.000000 panther-1.7.9/panther/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-04 19:39:46.000000 panther-1.7.9/panther/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-07-04 19:39:46.000000 panther-1.7.9/panther/routings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-07-04 19:39:46.000000 panther-1.7.9/panther/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-04 19:39:46.000000 panther-1.7.9/panther/throttling.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-04 19:39:46.000000 panther-1.7.9/panther/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:40:00.235499 panther-1.7.9/panther.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-04 19:40:00.000000 panther-1.7.9/panther.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-04 19:40:00.000000 panther-1.7.9/panther.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:40:00.000000 panther-1.7.9/panther.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-04 19:40:00.000000 panther-1.7.9/panther.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-04 19:40:00.000000 panther-1.7.9/panther.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-04 19:40:00.000000 panther-1.7.9/panther.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-04 19:39:46.000000 panther-1.7.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 19:40:00.239499 panther-1.7.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-07-04 19:39:46.000000 panther-1.7.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.552842 panther-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-08-04 12:43:09.000000 panther-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-08-04 12:43:24.552842 panther-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6912 2023-08-04 12:43:09.000000 panther-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.548842 panther-2.0.0/panther/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-04 12:43:09.000000 panther-2.0.0/panther/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-08-04 12:43:09.000000 panther-2.0.0/panther/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-08-04 12:43:09.000000 panther-2.0.0/panther/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-08-04 12:43:09.000000 panther-2.0.0/panther/authentications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-08-04 12:43:09.000000 panther-2.0.0/panther/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.548842 panther-2.0.0/panther/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/create_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/monitor_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8633 2023-08-04 12:43:09.000000 panther-2.0.0/panther/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-08-04 12:43:09.000000 panther-2.0.0/panther/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.548842 panther-2.0.0/panther/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.552842 panther-2.0.0/panther/db/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/queries/mongodb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/queries/pantherdb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/queries/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-08-04 12:43:09.000000 panther-2.0.0/panther/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-08-04 12:43:09.000000 panther-2.0.0/panther/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-08-04 12:43:09.000000 panther-2.0.0/panther/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11215 2023-08-04 12:43:09.000000 panther-2.0.0/panther/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.552842 panther-2.0.0/panther/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-04 12:43:09.000000 panther-2.0.0/panther/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-08-04 12:43:09.000000 panther-2.0.0/panther/middlewares/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-04 12:43:09.000000 panther-2.0.0/panther/middlewares/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-08-04 12:43:09.000000 panther-2.0.0/panther/middlewares/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-08-04 12:43:09.000000 panther-2.0.0/panther/middlewares/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.552842 panther-2.0.0/panther/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:09.000000 panther-2.0.0/panther/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-08-04 12:43:09.000000 panther-2.0.0/panther/panel/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-08-04 12:43:09.000000 panther-2.0.0/panther/panel/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-04 12:43:09.000000 panther-2.0.0/panther/panel/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-08-04 12:43:09.000000 panther-2.0.0/panther/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-04 12:43:09.000000 panther-2.0.0/panther/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-08-04 12:43:09.000000 panther-2.0.0/panther/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-08-04 12:43:09.000000 panther-2.0.0/panther/routings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-08-04 12:43:09.000000 panther-2.0.0/panther/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-04 12:43:09.000000 panther-2.0.0/panther/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-04 12:43:09.000000 panther-2.0.0/panther/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.548842 panther-2.0.0/panther.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-08-04 12:43:24.000000 panther-2.0.0/panther.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-04 12:43:24.000000 panther-2.0.0/panther.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:43:24.000000 panther-2.0.0/panther.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 12:43:24.000000 panther-2.0.0/panther.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-04 12:43:24.000000 panther-2.0.0/panther.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 12:43:24.000000 panther-2.0.0/panther.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-08-04 12:43:09.000000 panther-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:43:24.552842 panther-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-04 12:43:09.000000 panther-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:43:24.552842 panther-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-04 12:43:09.000000 panther-2.0.0/tests/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-08-04 12:43:09.000000 panther-2.0.0/tests/test_pantherdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26448 2023-08-04 12:43:09.000000 panther-2.0.0/tests/test_routing.py
```

### Comparing `panther-1.7.9/LICENSE` & `panther-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `panther-1.7.9/panther/_utils.py` & `panther-2.0.0/panther/_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -65,27 +65,26 @@
     path, name = dotted_path.rsplit('.', 1)
     module = importlib.import_module(path)
     return getattr(module, name)
 
 
 def read_multipart_form_data(content_type: str, body: str) -> dict:
     """
-    content_type = 'application/json'
     content_type = 'multipart/form-data; boundary=--------------------------984465134948354357674418'
     """
     boundary = content_type[30:]
 
-    per_pattern = r'(.*\r\nContent-Disposition: form-data; name=")(.*)'  # (Junk)(FieldName)
+    pre_pattern = r'(.*\r\nContent-Disposition: form-data; name=")(.*)"'  # (Junk)(FieldName)"
     value_pattern = r'(\r\n\r\n)(.*)'  # (Junk)(Value)
 
     # (Junk)(FieldName) (Junk)(Value)(Junk)
-    field_pattern = per_pattern + value_pattern + r'(\r\n.*)'
+    field_pattern = pre_pattern + value_pattern + r'(\r\n.*)'
 
     # (Junk)(FieldName) (Junk)(FileName)(Junk)(ContentType) (Junk)(Value)
-    file_pattern = per_pattern + r'("; filename=")(.*)("\r\nContent-Type: )(.*)' + value_pattern
+    file_pattern = pre_pattern + r'("; filename=")(.*)("\r\nContent-Type: )(.*)' + value_pattern
 
     fields = dict()
     for field in body.split(boundary):
         if match := re.match(pattern=field_pattern, string=field):
             _, field_name, _, value, _ = match.groups()
             fields[field_name] = value
 
@@ -98,17 +97,7 @@
             #     'filename': file_name,
             #     'Content-Type': content_type,
             #     'value': value
             # }
             # fields[field_name] = data
             logger.error("We Don't Handle Files In Multipart Request Yet.")
     return fields
-
-
-def collect_path_variables(request_path: str, found_path: str) -> dict:
-    found_path = found_path.removesuffix('/').removeprefix('/')
-    request_path = request_path.removesuffix('/').removeprefix('/')
-    path_variables = dict()
-    for f_path, r_path in zip(found_path.split('/'), request_path.split('/')):
-        if f_path.startswith('<'):
-            path_variables[f_path[1:-1]] = r_path
-    return path_variables
```

### Comparing `panther-1.7.9/panther/app.py` & `panther-2.0.0/panther/app.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 import functools
-from datetime import timedelta, datetime
-
 from pydantic import ValidationError
+from datetime import timedelta, datetime
 from orjson.orjson import JSONDecodeError
 
 from panther import status
 from panther.logger import logger
 from panther.configs import config
 from panther.request import Request
-from panther.throttling import Throttling, throttling_storage
+from panther.utils import round_datetime
 from panther.response import Response, IterableDataTypes
+from panther.throttling import Throttling, throttling_storage
 from panther.caching import get_cached_response_data, set_cache_response, cache_key
-from panther.exceptions import APIException, InvalidPathVariableException, AuthorizationException, JsonDecodeException, \
-    ThrottlingException
-from panther.utils import round_datetime
+from panther.exceptions import (
+    InvalidPathVariableException,
+    AuthorizationException,
+    ThrottlingException,
+    JsonDecodeException,
+    MethodNotAllowed,
+    APIException,
+)
 
 
 class API:
     def __init__(
             self,
             input_model=None,
             output_model=None,
@@ -47,15 +52,16 @@
             # 2. Throttling
             self.handle_throttling()
 
             # 3. Permissions
             self.handle_permissions()
 
             # 4. Validate Input
-            self.validate_input()
+            if self.request.method in ['POST', 'PUT', 'PATCH']:
+                self.validate_input()
 
             # 5. Validate Path Variables
             self.validate_path_variables(func, kwargs)
 
             # 6. Get Cached Response
             if self.cache and self.request.method == 'GET':
                 if cached := get_cached_response_data(request=self.request):
@@ -156,7 +162,56 @@
                         variables[user_var] = value.lower() not in ['false', '0']
                     elif _type is int:
                         try:
                             variables[user_var] = int(value)
                         except ValueError:
                             raise InvalidPathVariableException(value=value, arg_type=_type)
                     break
+
+
+class GenericAPI:
+    input_model = None
+    output_model = None
+    auth: bool = False
+    permissions: list | None = None
+    throttling: Throttling = None
+    cache: bool = False
+    cache_exp_time: timedelta | int | None = None
+    
+    async def get(self, *args, **kwargs):
+        raise MethodNotAllowed
+
+    async def post(self, *args, **kwargs):
+        raise MethodNotAllowed
+
+    async def put(self, *args, **kwargs):
+        raise MethodNotAllowed
+
+    async def patch(self, *args, **kwargs):
+        raise MethodNotAllowed
+
+    async def delete(self, *args, **kwargs):
+        raise MethodNotAllowed
+
+    @classmethod
+    async def call_method(cls, *args, **kwargs):
+        match kwargs['request'].method:
+            case 'GET':
+                func = cls().get
+            case 'POST':
+                func = cls().post
+            case 'PUT':
+                func = cls().put
+            case 'PATCH':
+                func = cls().patch
+            case 'DELETE':
+                func = cls().delete
+
+        return await API(
+            input_model=cls.input_model,
+            output_model=cls.output_model,
+            auth=cls.auth,
+            permissions=cls.permissions,
+            throttling=cls.throttling,
+            cache=cls.cache,
+            cache_exp_time=cls.cache_exp_time,
+        )(func)(*args, **kwargs)
```

### Comparing `panther-1.7.9/panther/authentications.py` & `panther-2.0.0/panther/authentications.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,33 @@
+from abc import abstractmethod
 from datetime import datetime
+from jose import JWTError, jwt
 from panther.logger import logger
 from panther.configs import config
 from panther.db.models import BaseUser
 from panther.request import Request
-from panther.cli.utils import import_error
 from panther.exceptions import AuthenticationException
-try:
-    from jose import JWTError, jwt
-except ImportError:
-    import_error('python-jose')
-    exit()
 
 
-class JWTAuthentication:
+class BaseAuthentication:
+    @classmethod
+    @abstractmethod
+    def authentication(cls, request: Request):
+        """
+        Return User Instance
+        """
+        raise cls.exception(f'{cls.__name__}.authentication() is not implemented.')
+
+    @staticmethod
+    def exception(message: str, /):
+        logger.error(f'Authentication Error: "{message}"')
+        return AuthenticationException
+
+
+class JWTAuthentication(BaseAuthentication):
     model = BaseUser
     keyword = 'Bearer'
     algorithm = 'HS256'
     HTTP_HEADER_ENCODING = 'iso-8859-1'  # Header encoding (see RFC5987)
 
     @staticmethod
     def get_authorization_header(request: Request):
```

### Comparing `panther-1.7.9/panther/caching.py` & `panther-2.0.0/panther/caching.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,44 +5,46 @@
 
 
 from panther.logger import logger
 from panther.configs import config
 from panther.request import Request
 from panther.db.connection import redis
 from panther.response import Response, ResponseDataTypes
+from panther.utils import generate_hash_value_from_string
 
 
 caches = dict()
-Cached = namedtuple('Cached', ['data', 'status_code'])
+CachedResponse = namedtuple('Cached', ['data', 'status_code'])
 
 
 def cache_key(request: Request, /):
     client = request.user and request.user.id or request.client.ip
-    return f'{client}-{request.path}-{request.data}'
+    query_params_hash = generate_hash_value_from_string(request.scope['query_string'].decode('utf-8'))
+    return f'{client}-{request.path}{query_params_hash}-{request.data}'
 
 
-def get_cached_response_data(*, request: Request) -> Cached | None:
+def get_cached_response_data(*, request: Request) -> CachedResponse | None:
     """
     If redis.is_connected:
         Get Cached Data From Redis
     else:
         Get Cached Data From Memory
     """
     key = cache_key(request)
     if redis.is_connected:  # NOQA: Unresolved References
         data = (redis.get(key) or b'{}').decode()
         if cached := json.loads(data):
-            return Cached(*cached)
+            return CachedResponse(*cached)
         else:
             return None
 
     else:
         global caches
         if cached := caches.get(key):
-            return Cached(*cached)
+            return CachedResponse(*cached)
         else:
             return None
 
 
 def set_cache_response(*, request: Request, response: Response, cache_exp_time: timedelta | int) -> None:
     """
     If redis.is_connected:
```

### Comparing `panther-1.7.9/panther/cli/create_command.py` & `panther-2.0.0/panther/cli/create_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.9/panther/cli/main.py` & `panther-2.0.0/panther/cli/main.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import os
 import sys
 
 from rich import print as rprint
 
+from panther import version as panther_version
 from panther.cli.run_command import run
 from panther.cli.create_command import create
 from panther.cli.monitor_command import monitor
 from panther.cli.utils import clean_args, help_message, cli_error
 
 
 def shell() -> None:
     os.system('bpython')
 
 
+def version() -> None:
+    print(panther_version())
+
+
 def start() -> None:
     command = sys.argv and sys.argv[1] or None
     args = clean_args(sys.argv[2:])
 
     match command:
         case '-h' | '--help':
             rprint(help_message)
@@ -24,9 +29,11 @@
             create(sys.argv[2:])
         case 'run':
             run(args)
         case 'shell':
             shell()
         case 'monitor':
             monitor()
+        case 'version':
+            version()
         case _:
             cli_error('Invalid Arguments.')
```

### Comparing `panther-1.7.9/panther/cli/monitor_command.py` & `panther-2.0.0/panther/cli/monitor_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.9/panther/cli/run_command.py` & `panther-2.0.0/panther/cli/run_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.9/panther/cli/template.py` & `panther-2.0.0/panther/cli/template.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,28 +28,28 @@
     }
     return Response(data=data, status_code=status.HTTP_202_ACCEPTED)
 """
 
 models_py = """from panther.db import Model
 """
 
-serializers_py = """from pydantic import BaseModel as Serializer
+serializers_py = """from pydantic import BaseModel
 """
 
 throttling_py = """from datetime import timedelta
 from panther.throttling import Throttling
 
 
 InfoThrottling = Throttling(rate=5, duration=timedelta(minutes=1))
 """
 
 app_urls_py = """from app.apis import hello_world_api, info_api
 
 urls = {
-    '': hello_world_api,
+    '/': hello_world_api,
     'info/': info_api,
 }
 """
 
 configs_py = """\"""
 {PROJECT_NAME} Project (Generated by Panther on %s)
 \"""
@@ -60,20 +60,19 @@
 from panther.utils import load_env
 from panther.throttling import Throttling
 
 
 BASE_DIR = Path(__name__).resolve().parent
 env = load_env(BASE_DIR / '.env')
 
-DB_NAME = env['DB_NAME']
 SECRET_KEY = env['SECRET_KEY']
 
 # # # More Info: Https://PantherPy.GitHub.io/middlewares/
 MIDDLEWARES = [
-    ('panther.middlewares.db.Middleware', {'url': f'pantherdb://{BASE_DIR}/{DB_NAME}.pdb'}),
+    ('panther.middlewares.db.Middleware', {'url': f'pantherdb://{BASE_DIR}/database.pdb'}),
 ]
 
 # More Info: https://PantherPy.GitHub.io/configs/#user_model
 USER_MODEL = 'panther.db.models.BaseUser'
 
 # More Info: https://PantherPy.GitHub.io/authentications/
 AUTHENTICATION = 'panther.authentications.JWTAuthentication'
@@ -89,16 +88,14 @@
 
 # More Info: https://PantherPy.GitHub.io/urls/
 URLs = 'core/urls.py'
 """ % datetime.now().date().isoformat()
 
 env = """
 SECRET_KEY = '%s'
-
-DB_NAME = '{PROJECT_NAME}'
 """ % generate_secret_key()
 
 main_py = """from panther import Panther
 
 app = Panther(__name__)
 """
```

### Comparing `panther-1.7.9/panther/cli/utils.py` & `panther-2.0.0/panther/cli/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 │                                                          │
 │       - panther shell                                    │
 │           Run interactive python shell                   │
 │                                                          │
 │       - panther monitor                                  │
 │           Show the monitor :)                            │
 │                                                          │
+│       - panther version                                  │
+│           Print the current version of Panther           │
+│                                                          │
 │       - panther [--help | -h ]                           │
 │           Show this message and exit                     │
 ╰{58 * '─'}╯
 """
 
 run_help_message = """
     --host TEXT                     Bind socket to this host.  [default: 127.0.0.1]
@@ -124,18 +127,14 @@
     logger.error(f'Error: {message}\n\nUse panther -h for more help')
 
 
 def import_error_message(module_name: str) -> str:
     return f'No module named "{module_name}"\n\t    Hint: Try to install with "pip install {module_name}"'
 
 
-def import_error(module_name: str) -> None:
-    logger.critical(import_error_message(module_name))
-
-
 def clean_args(args: list[str]) -> dict:
     """
     Input: ['--reload', '--host', '127.0.0.1', ...]
     Output: {'--reload: None, 'host': '127.0.0.1', ...}
     """
     _args = dict()
     for i, arg in enumerate(args):
```

### Comparing `panther-1.7.9/panther/configs.py` & `panther-2.0.0/panther/configs.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,36 +14,36 @@
     life_time: timedelta | int = timedelta(days=1)
 
 
 class Config(TypedDict):
     base_dir: Path
     monitoring: bool
     log_queries: bool
-    urls: dict
-    middlewares: list
-    reversed_middlewares: list
-    db_engine: str
     default_cache_exp: timedelta | None
+    throttling: Throttling | None
     secret_key: bytes | None
+    middlewares: list
+    reversed_middlewares: list
+    user_model: ModelMetaclass | None
     authentication: ModelMetaclass | None
     jwt_config: JWTConfig | None
-    user_model: ModelMetaclass | None
-    throttling: Throttling | None
     models: list[dict]
+    urls: dict
+    db_engine: str
 
 
 config: Config = {
     'base_dir': Path(),
     'monitoring': False,
     'log_queries': False,
+    'default_cache_exp': None,
+    'throttling': None,
     'secret_key': None,
-    'urls': {},
     'middlewares': [],
     'reversed_middlewares': [],
-    'db_engine': '',
-    'default_cache_exp': None,
-    'jwt_config': None,
-    'authentication': None,
     'user_model': None,
-    'throttling': None,
+    'authentication': None,
+    'jwt_config': None,
     'models': [],
+    'urls': {},
+    'db_engine': '',  # TODO: Should we set default db_engine=pantherdb ?
 }
```

### Comparing `panther-1.7.9/panther/db/connection.py` & `panther-2.0.0/panther/db/connection.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.9/panther/db/queries/pantherdb_queries.py` & `panther-2.0.0/panther/db/queries/pantherdb_queries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-from typing import Self
+from sys import version_info
 
 from panther.db.connection import db
-from panther.db.utils import merge_dicts
-from panther.exceptions import DBException
+from panther.db.utils import merge_dicts, prepare_id_for_query
+
+
+if version_info.minor >= 11:
+    from typing import Self
+else:
+    from typing import TypeVar
+    Self = TypeVar("Self", bound="BasePantherDBQuery")
 
 
 class BasePantherDBQuery:
 
     @classmethod
     def _merge(cls, *args) -> dict:
-        # TODO: Convert "id" to "_id"
+        prepare_id_for_query(*args)
         return merge_dicts(*args)
 
     # # # # # Find # # # # #
     @classmethod
     def find_one(cls, _data: dict = None, /, **kwargs) -> Self | None:
         if document := db.session.collection(cls.__name__).find_one(**cls._merge(_data, kwargs)):
             return cls(**document)
@@ -25,18 +31,14 @@
 
     # # # # # Insert # # # # #
     @classmethod
     def insert_one(cls, _data: dict = None, **kwargs) -> Self:
         document = db.session.collection(cls.__name__).insert_one(**cls._merge(_data, kwargs))
         return cls(**document)
 
-    @classmethod
-    def insert_many(cls, _data: dict = None, /, **kwargs):
-        raise DBException('insert_many() is not supported while using PantherDB.')
-
     # # # # # Delete # # # # #
     def delete(self) -> None:
         db.session.collection(self.__class__.__name__).delete_one(_id=self.id)
 
     @classmethod
     def delete_one(cls, _data: dict = None, /, **kwargs) -> bool:
         return db.session.collection(cls.__name__).delete_one(**cls._merge(_data, kwargs))
@@ -49,17 +51,19 @@
     def update(self, **kwargs) -> None:
         for field, value in kwargs.items():
             setattr(self, field, value)
         db.session.collection(self.__class__.__name__).update_one({'_id': self.id}, **kwargs)
 
     @classmethod
     def update_one(cls, _filter, _data: dict = None, /, **kwargs) -> bool:
+        prepare_id_for_query(_filter)
         return db.session.collection(cls.__name__).update_one(_filter, **cls._merge(_data, kwargs))
 
     @classmethod
     def update_many(cls, _filter, _data: dict = None, /, **kwargs) -> int:
+        prepare_id_for_query(_filter)
         return db.session.collection(cls.__name__).update_many(_filter, **cls._merge(_data, kwargs))
 
     # # # # # Other # # # # #
     @classmethod
     def count(cls, _data: dict = None, /, **kwargs) -> int:
         return db.session.collection(cls.__name__).count(**cls._merge(_data, kwargs))
```

### Comparing `panther-1.7.9/panther/db/queries/queries.py` & `panther-2.0.0/panther/db/queries/queries.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Self, NoReturn
+import sys
+from typing import NoReturn
 
 from pydantic import ValidationError
 
 from panther.configs import config
 from panther.db.utils import log_query
 from panther.db.queries.mongodb_queries import BaseMongoDBQuery
 from panther.db.queries.pantherdb_queries import BasePantherDBQuery
@@ -14,14 +15,21 @@
     BaseQuery = BaseMongoDBQuery
 
 __all__ = (
     'Query',
 )
 
 
+if sys.version_info.minor >= 11:
+    from typing import Self
+else:
+    from typing import TypeVar
+    Self = TypeVar("Self", bound="Query")
+
+
 class Query(BaseQuery):
 
     @classmethod
     def validate_data(cls, data: dict, is_updating: bool = False) -> NoReturn:
         """
         *. Validate the input of user with its class
         *. If is_updating is True & exception happens but the message was empty
@@ -67,47 +75,47 @@
             >>> User.insert_one(name='Ali', age=24, ...)
         """
         cls.validate_data(kwargs)
         return super().insert_one(_data, **kwargs)
 
     @classmethod
     @log_query
-    def insert_many(cls, _data: dict = None, **kwargs):
-        return super().insert_many(_data, **kwargs)
+    def insert_many(cls, _data: dict = None, /, **kwargs):
+        raise DBException('insert_many() is not supported yet.')
 
     # # # # # Delete # # # # #
     @log_query
     def delete(self) -> None:
         """
         example:
             >>> from example.app.models import User
             >>> user = User.find_one(name='Ali')
             >>> user.delete()
         """
         return super().delete()
 
     @classmethod
     @log_query
-    def delete_one(cls, **kwargs) -> bool:
+    def delete_one(cls, _data: dict = None, /, **kwargs) -> bool:
         """
         example:
             >>> from example.app.models import User
             >>> User.delete_one(id=1)
         """
-        return super().delete_one(**kwargs)
+        return super().delete_one(_data, **kwargs)
 
     @classmethod
     @log_query
-    def delete_many(cls, **kwargs) -> int:
+    def delete_many(cls, _data: dict = None, /, **kwargs) -> int:
         """
         example:
             >>> from example.app.models import User
             >>> User.delete_many(last_name='Rn')
         """
-        return super().delete_many(**kwargs)
+        return super().delete_many(_data, **kwargs)
 
     # # # # # Update # # # # #
     @log_query
     def update(self, **kwargs) -> None:
         """
         example:
             >>> from example.app.models import User
@@ -126,21 +134,22 @@
             >>> User.update_one({'id': 1}, name='Ali')
             >>> User.update_one({'id': 2}, {'name': 'Ali', 'age': 25})
         """
         return super().update_one(_filter, _data, **kwargs)
 
     @classmethod
     @log_query
-    def update_many(cls, _filter, **kwargs) -> int:
+    def update_many(cls, _filter, _data: dict = None, /, **kwargs) -> int:
         """
         example:
             >>> from example.app.models import User
             >>> User.update_many({'name': 'Mohsen'}, name='Ali')
+            >>> User.update_many({'name': 'Mohsen'}, {'name': 'Ali'})
         """
-        return super().update_many(_filter, **kwargs)
+        return super().update_many(_filter, _data, **kwargs)
 
     # # # # # Other # # # # #
     @classmethod
     @log_query
     def last(cls, _data: dict = None, /, **kwargs) -> Self | None:
         """
         example:
@@ -167,7 +176,18 @@
             >>> from example.app.models import User
             >>> user = User.find_or_insert(name='Ali')
         """
         if obj := cls.find_one(**kwargs):
             return False, obj
         else:
             return True, cls.insert_one(**kwargs)
+
+    @log_query
+    def save(self, **kwargs) -> None:
+        """
+        example:
+            >>> from example.app.models import User
+            >>> user = User.find_one(name='Ali')
+            >>> user.name = 'Saba'
+            >>> user.save()
+        """
+        raise DBException('save() is not supported yet.')
```

### Comparing `panther-1.7.9/panther/db/utils.py` & `panther-2.0.0/panther/db/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,29 +16,29 @@
         end = perf_counter()
         class_name = args[0].__name__ if hasattr(args[0], '__name__') else args[0].__class__.__name__
         query_logger.info(f'\033[1mQuery -->\033[0m  {class_name}.{func.__name__}() --> {(end - start) * 1_000:.2} ms')
         return response
     return log
 
 
-def clean_object_id(_id: bson.ObjectId | str) -> bson.ObjectId:
+def prepare_id_for_query(*args, is_mongo: bool = False):
+    for d in args:
+        if d is None:
+            continue
+        if 'id' in d:
+            d['_id'] = d.pop('id')
+
+        if is_mongo and '_id' in d:
+            d['_id'] = _convert_to_object_id(d['_id'])
+
+
+def _convert_to_object_id(_id: bson.ObjectId | str) -> bson.ObjectId:
     if isinstance(_id, bson.ObjectId):
         return _id
     try:
         return bson.ObjectId(_id)
     except Exception:
-        raise bson.errors.InvalidId  # NOQA: Py Unresolved References
-
-
-def clean_object_id_in_dicts(*args):
-    # TODO: Refactor this func
-    for d in args:
-        if d is None:
-            continue
-        if '_id' in d:
-            d['_id'] = clean_object_id(d['_id'])
-        if 'id' in d:
-            d['_id'] = clean_object_id(d.pop('id'))
+        raise bson.errors.InvalidId(f"id={_id} is invalid bson.ObjectId")
 
 
 def merge_dicts(*args) -> dict:
     return reduce(operator.ior, filter(None, args), {})
```

### Comparing `panther-1.7.9/panther/exceptions.py` & `panther-2.0.0/panther/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,19 @@
     status_code: int = status.HTTP_500_INTERNAL_SERVER_ERROR
 
     def __init__(self, detail=None, status_code=None):
         self.detail = detail or self.detail
         self.status_code = status_code or self.status_code
 
 
+class MethodNotAllowed(APIException):
+    detail = 'Method Not Allowed'
+    status_code = status.HTTP_405_METHOD_NOT_ALLOWED
+
+
 class AuthenticationException(APIException):
     detail = 'Authentication Error'
     status_code = status.HTTP_401_UNAUTHORIZED
 
 
 class AuthorizationException(APIException):
     detail = 'Permission Denied'
```

### Comparing `panther-1.7.9/panther/logger.py` & `panther-2.0.0/panther/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from pydantic import BaseModel
 
 from panther.configs import config
 from logging.config import dictConfig
 
 
 LOGS_DIR = config['base_dir'] / 'logs'
-if not os.path.exists(LOGS_DIR):
-    os.makedirs(LOGS_DIR)
 
 
 class LogConfig(BaseModel):
     """Logging configuration to be set for the server."""
 
     LOGGER_NAME: str = 'panther-logger'
     DEFAULT_LOG_FORMAT: str = '%(levelprefix)s | %(asctime)s | %(message)s'
@@ -75,11 +73,18 @@
         'query': {
             'handlers': ['default', 'query_file'],
             'level': LOG_LEVEL,
         },
     }
 
 
-dictConfig(LogConfig().model_dump())
+try:
+    dictConfig(LogConfig().model_dump())
+except ValueError:
+    LOGS_DIR = config['base_dir'] / 'logs'
+    if not os.path.exists(LOGS_DIR):
+        os.makedirs(LOGS_DIR)
+
+
 logger = logging.getLogger('panther')
 query_logger = logging.getLogger('query')
 monitoring_logger = logging.getLogger('monitoring')
```

### Comparing `panther-1.7.9/panther/main.py` & `panther-2.0.0/panther/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import os
 import ast
+import sys
 import asyncio
 from pathlib import Path
 from runpy import run_path
 from pydantic._internal._model_construction import ModelMetaclass
 
 from panther import status
+from panther.app import GenericAPI
 from panther.request import Request
 from panther.response import Response
 from panther.exceptions import APIException
 from panther.configs import JWTConfig, config
 from panther.middlewares.base import BaseMiddleware
 from panther.middlewares.monitoring import Middleware as MonitoringMiddleware
-from panther.routings import find_endpoint, check_urls, collect_urls, finalize_urls
-from panther._utils import http_response, import_class, read_body, collect_path_variables
+from panther.routings import find_endpoint, check_and_load_urls, finalize_urls, flatten_urls, collect_path_variables
+from panther._utils import http_response, import_class, read_body
 
 """ We can't import logger on the top cause it needs config['base_dir'] ans its fill in __init__ """
 
 
 class Panther:
 
     def __init__(self, name):
+        from panther.logger import logger
         os.system('clear')
         config['base_dir'] = Path(name).resolve().parent
         self.panther_dir = Path(__file__).parent
+        if sys.version_info.minor < 11:
+            logger.warning('Use Python Version 3.11+ For Better Performance.')
         self.load_configs()
 
     def load_configs(self) -> None:
         from panther.logger import logger
         logger.debug(f'Base directory: {config["base_dir"]}')
 
         # Check & Read The Configs File
@@ -44,42 +49,38 @@
         config['reversed_middlewares'] = config['middlewares'][::-1]
         config['user_model'] = self._get_user_model()
 
         config['authentication'] = self._get_authentication_class()
         config['jwt_config'] = self._get_jwt_config()
 
         # Find Database Models
-        self.collect_models_for_panel()
+        self._collect_models()
 
         # Check & Collect URLs
         #   check_urls should be the last call in load_configs,
         #   because it will read all files and load them.
         config['urls'] = self._load_urls()
 
         # This import shouldn't be on top
         from panther.panel.urls import urls as panel_urls
-        config['urls']['_panel'] = panel_urls
+        config['urls']['_panel'] = finalize_urls(flatten_urls(panel_urls))
 
         logger.debug('Configs loaded.')
         if config['monitoring']:
             logger.info('Run "panther monitor" in another session for Monitoring.')
 
-    def _load_urls(self) -> dict:
-        urls = check_urls(self.settings.get('URLs')) or {}
-        collect_urls('', urls, collected_urls := dict())
-        return finalize_urls(collected_urls)
-
     def _check_configs(self):
         from panther.logger import logger
         """Read the config file and put it as dict in self.settings"""
         try:
             configs_path = config['base_dir'] / 'core/configs.py'
             self.settings = run_path(str(configs_path))
         except FileNotFoundError:
             logger.critical('core/configs.py Not Found.')
+            # TODO: Exit() Here
 
     def _get_secret_key(self) -> bytes | None:
         if secret_key := self.settings.get('SECRET_KEY'):
             return secret_key.encode()
         return secret_key
 
     def _get_middlewares(self) -> list:
@@ -95,27 +96,29 @@
             if not issubclass(Middleware, BaseMiddleware):
                 logger.critical(f'{Middleware} is not a sub class of BaseMiddleware.')
                 continue
 
             middlewares.append(Middleware(**data))  # NOQA: Py Argument List
         return middlewares
 
-    def _get_authentication_class(self) -> ModelMetaclass | None:
-        return self.settings.get('AUTHENTICATION') and import_class(self.settings['AUTHENTICATION'])
-
     def _get_user_model(self) -> ModelMetaclass:
         return import_class(self.settings.get('USER_MODEL', 'panther.db.models.BaseUser'))
 
+    def _get_authentication_class(self) -> ModelMetaclass | None:
+        return self.settings.get('AUTHENTICATION') and import_class(self.settings['AUTHENTICATION'])
+
     def _get_jwt_config(self) -> JWTConfig:
         """Only Collect JWT Config If Authentication Is JWTAuthentication"""
         if getattr(config['authentication'], '__name__', None) == 'JWTAuthentication':
             user_config = self.settings.get('JWTConfig')
             return JWTConfig(**user_config) if user_config else JWTConfig(key=config['secret_key'].decode())
 
-    def collect_models_for_panel(self):
+    @classmethod
+    def _collect_models(cls):
+        """Collecting models for panel APIs"""
         from panther.db.models import Model
 
         for root, _, files in os.walk(config['base_dir']):
             # Traverse through each directory
             for f in files:
                 # Traverse through each file of directory
                 if f == 'models.py':
@@ -141,32 +144,40 @@
                                             config['models'].append({
                                                 'name': n.name,
                                                 'path':  file_path,
                                                 'class': klass,
                                                 'app': class_path.split('.'),
                                             })
 
+    def _load_urls(self) -> dict:
+        urls = check_and_load_urls(self.settings.get('URLs')) or {}
+        collected_urls = flatten_urls(urls)
+        return finalize_urls(collected_urls)
+
     async def __call__(self, scope, receive, send) -> None:
         """
-        We Used Python3.11 For asyncio.TaskGroup()
+        We Used Python3.11+ For asyncio.TaskGroup()
         1.
             async with asyncio.TaskGroup() as tg:
                 tg.create_task(self.run(scope, receive, send))
         2.
             await self.run(scope, receive, send)
         3.
             async with anyio.create_task_group() as task_group:
                 task_group.start_soon(self.run, scope, receive, send)
                 await anyio.to_thread.run_sync(self.run, scope, receive, send)
         4.
             with ProcessPoolExecutor() as e:
                 e.submit(self.run, scope, receive, send)
         """
-        async with asyncio.TaskGroup() as tg:
-            tg.create_task(self.run(scope, receive, send))
+        if sys.version_info.minor >= 11:
+            async with asyncio.TaskGroup() as tg:
+                tg.create_task(self.run(scope, receive, send))
+        else:
+            await self.run(scope, receive, send)
 
     async def run(self, scope, receive, send):
         from panther.logger import logger
         # Read Body & Create Request
         body = await read_body(receive)
         request = Request(scope=scope, body=body)
 
@@ -186,26 +197,44 @@
             )
 
         try:  # They Both Have The Save Exception (APIException)
             # Call 'Before' Middlewares
             for middleware in config['middlewares']:
                 request = await middleware.before(request=request)
 
-            # User Didn't Use @API Decorator
-            if not hasattr(endpoint, '__wrapped__'):
-                logger.critical(f'You may have forgotten to use @API on the {endpoint.__name__}()')
-                return await http_response(
-                    send,
-                    status_code=status.HTTP_510_NOT_EXTENDED,
-                    monitoring=monitoring_middleware,
-                    exception=True,
-                )
+            if type(endpoint).__name__ == 'function':
+                # User Didn't Use @API Decorator
+                if not hasattr(endpoint, '__wrapped__'):
+                    logger.critical(f'You may have forgotten to use @API on the {endpoint.__name__}()')
+                    return await http_response(
+                        send,
+                        status_code=status.HTTP_510_NOT_EXTENDED,
+                        monitoring=monitoring_middleware,
+                        exception=True,
+                    )
+
+                # Prepare Endpoint
+                _endpoint = endpoint
+
+            else:
+                if not issubclass(endpoint, GenericAPI):
+                    logger.critical(f'You may have forgotten to inherit from GenericAPI on the {endpoint.__name__}()')
+                    return await http_response(
+                        send,
+                        status_code=status.HTTP_510_NOT_EXTENDED,
+                        monitoring=monitoring_middleware,
+                        exception=True,
+                    )
+
+                # Prepare Endpoint
+                _endpoint = endpoint.call_method
 
             # Call Endpoint
-            response = await endpoint(request=request, **path_variables)
+            response = await _endpoint(request=request, **path_variables)
+
         except APIException as e:
             response = self.handle_exceptions(e)
         except Exception as e:
             # Every unhandled exception in Panther or code will catch here
             logger.critical(e)
             return await http_response(
                 send,
```

### Comparing `panther-1.7.9/panther/middlewares/monitoring.py` & `panther-2.0.0/panther/middlewares/monitoring.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.9/panther/middlewares/redis.py` & `panther-2.0.0/panther/middlewares/redis.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.9/panther/request.py` & `panther-2.0.0/panther/request.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -93,21 +93,14 @@
         return self.scope['http_version']
 
     @property
     def scheme(self) -> str:
         return self.scope['scheme']
 
     @property
-    def data(self):
-        """Return The Validated Data
-        It has been set on API.validate_input() while request is happening
-        """
-        return self._validated_data
-
-    @property
     def pure_data(self) -> dict:
         """This is the data before validation"""
         from panther.logger import logger
 
         if self._data is None:
 
             body = self._body.decode('utf-8', errors='replace') or {}
@@ -119,14 +112,21 @@
                 self._data = read_multipart_form_data(content_type=self.headers.content_type, body=body)
             else:
                 logger.error(f'{self.headers.content_type} Is Not Supported.')
                 self._data = {}
 
         return self._data
 
+    @property
+    def data(self):
+        """Return The Validated Data
+        It has been set on API.validate_input() while request is happening
+        """
+        return self._validated_data
+
     def set_validated_data(self, validated_data) -> None:
         self._validated_data = validated_data
 
     @property
     def user(self):
         return self._user
```

### Comparing `panther-1.7.9/panther/response.py` & `panther-2.0.0/panther/response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import orjson as json
 from types import NoneType
+
+from panther.logger import logger
 from pydantic import BaseModel as PydanticBaseModel
 
-ResponseDataTypes = int | dict | list | tuple | set | str | bool | NoneType
+ResponseDataTypes = list | tuple | set | dict | int | str | bool | NoneType
 IterableDataTypes = list | tuple | set
 
 
 class Response:
     def __init__(self, data: ResponseDataTypes = None, status_code: int = 200):
         """
         :param data: should be int | dict | list | tuple | set | str | bool or NoneType
@@ -38,15 +40,25 @@
             raise TypeError(error)
 
     @classmethod
     def clean_data_type(cls, data: any):
         """
         Make sure the response data is only ResponseDataTypes or Iterable of ResponseDataTypes
         """
+
         if issubclass(type(data), PydanticBaseModel):
             return data.model_dump()
 
         elif isinstance(data, IterableDataTypes):
             return [cls.clean_data_type(d) for d in data]
 
-        else:
+        elif isinstance(data, dict):
+            for key, value in data.items():
+                data[key] = cls.clean_data_type(value)
+            else:
+                return data
+
+        elif isinstance(data, (int | str | bool | NoneType)):
             return data
+
+        else:
+            raise ValueError(f'Invalid Response Type: {type(data)}')
```

### Comparing `panther-1.7.9/panther/routings.py` & `panther-2.0.0/panther/routings.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 from runpy import run_path
 from typing import Callable
 from collections import Counter
 from typing import MutableMapping
 from collections.abc import Mapping
 from functools import reduce, partial
 
-
 from panther.configs import config
 
 
-def check_urls(urls: str | None) -> dict | None:
+def check_and_load_urls(urls: str | None) -> dict | None:
     from panther.logger import logger
 
     if urls is None:
         return logger.critical("configs.py Does Not Have 'URLs'")
 
     try:
         full_urls_path = config['base_dir'] / urls
@@ -25,115 +24,163 @@
     except KeyError:
         return logger.critical("'URLs' Address Does Not Have 'urls'")
     if not isinstance(urls_dict, dict):
         return logger.critical("'urls' Of URLs Is Not dict.")
     return urls_dict
 
 
-def collect_urls(pre_url: str, urls: dict, final: dict):
+def flatten_urls(urls: dict) -> dict:
+    return {k: v for k, v in _flattening_urls(urls)}
+
+
+def _flattening_urls(data: dict | Callable, url: str = ''):
+    # Add `/` add the end of url
+    if not url.endswith('/'):
+        url = f'{url}/'
+
+    if isinstance(data, dict):
+        for k, v in data.items():
+            yield from _flattening_urls(v, f'{url}{k}')
+    else:
+        # Remove `/` prefix of url
+        url = url.removeprefix('/')
+
+        # Collect it, if it doesn't have problem
+        if _is_url_endpoint_valid(url=url, endpoint=data):
+            yield url, data
+
+
+def _is_url_endpoint_valid(url: str, endpoint: Callable) -> bool:
     from panther.logger import logger
 
+    if endpoint is ...:
+        logger.error(f"URL Can't Point To Ellipsis. ('{url}' -> ...)")
+    elif endpoint is None:
+        logger.error(f"URL Can't Point To None. ('{url}' -> None)")
+    elif url and not re.match(r'^[a-zA-Z<>0-9_/-]+$', url):
+        logger.error(f"URL Is Not Valid. --> '{url}'")
+    else:
+        return True
+    return False
+
+
+def finalize_urls(urls: dict) -> dict:
+    """convert flat dict to nested"""
+    urls_list = list()
     for url, endpoint in urls.items():
-        if endpoint is ...:
-            logger.error(f"URL Can't Point To Ellipsis. ('{pre_url}{url}' -> ...)")
-        elif endpoint is None:
-            logger.error(f"URL Can't Point To None. ('{pre_url}{url}' -> None)")
-        elif url and not re.match(r'[a-zA-Z<>0-9_/-]', url):
-            logger.error(f"URL Is Not Valid. --> '{pre_url}{url}'")
+        path = dict()
+        if url == '':
+            # This condition only happen when
+            #   user defines the root url == '' instead of '/'
+            url = '/'
+
+        for single_path in list(filter(lambda x: x != '', url.split('/')[:-1][::-1])) or ['']:
+            if single_path != '' and not path:
+                path = {single_path: {'': endpoint}}
+            else:
+                path = {single_path: path or endpoint}
+        urls_list.append(path)
+    return _merge(*urls_list) if urls_list else {}
+
+
+def _merge(destination: MutableMapping, *sources) -> MutableMapping:
+    return _simplify_urls(reduce(partial(_deepmerge), sources, destination))
+
+
+def _simplify_urls(urls):
+    simplified_urls = dict()
+
+    for key, value in urls.items():
+        if isinstance(value, dict):
+            simplified_value = _simplify_urls(value)
+            if isinstance(simplified_value, dict) and len(simplified_value) == 1 and '' in simplified_value:
+                simplified_urls[key] = simplified_value['']
+            else:
+                simplified_urls[key] = simplified_value
         else:
-            if not url.endswith('/'):
-                url = f'{url}/'
-            if isinstance(endpoint, dict):
-                if url != '/':
-                    if pre_url:
-                        pre_url = f'{pre_url}/{url}'
-                    else:
-                        pre_url = url
-                collect_urls(pre_url, endpoint, final)
+            simplified_urls[key] = value
+
+    return simplified_urls
+
+
+def _deepmerge(dst, src):
+    """Credit to Travis Clarke --> https://github.com/clarketm/mergedeep"""
+    for key in src:
+        if key in dst:
+            if _is_recursive_merge(dst[key], src[key]):
+                _deepmerge(dst[key], src[key])
             else:
-                final[f'{pre_url}{url}'] = endpoint
+                dst[key] = deepcopy(src[key])
+        else:
+            dst[key] = deepcopy(src[key])
+    return dst
+
 
-    return urls
+def _is_recursive_merge(a, b):
+    both_mapping = isinstance(a, Mapping) and isinstance(b, Mapping)
+    both_counter = isinstance(a, Counter) and isinstance(b, Counter)
+    return both_mapping and not both_counter
 
 
 def find_endpoint(path: str) -> tuple[Callable | None, str]:
+    urls = config['urls']
+
     if (location := path.find('?')) != -1:
         path = path[:location]
     path = path.removesuffix('/').removeprefix('/')  # 'user/list'
     paths = path.split('/')  # ['user', 'list']
     paths_len = len(paths)
-    sub = config['urls']
-    # sub = {
-    #     'user': {
-    #         '<id>': <function users at 0x7f579d060220>,
-    #         '': <function single_user at 0x7f579d060e00>
-    #     }
-    # }
+
     found_path = ''
     for i, split_path in enumerate(paths):
         last_path = bool((i + 1) == paths_len)
-        found = sub.get(split_path)
+        found = urls.get(split_path)
+
+        # `found` is callable
         if last_path and callable(found):
             found_path += f'{split_path}/'
             return found, found_path
+
+        # `found` is dict
         if isinstance(found, dict):
             found_path += f'{split_path}/'
             if last_path and callable(endpoint := found.get('')):
                 return endpoint, found_path
 
-            sub = found
+            urls = found
             continue
 
-        # found = None
-        # sub = {'<id>': <function return_list at 0x7f0757baff60>} (Example)
+        # `found` is None
         _continue = False
-        for key, value in sub.items():
+        for key, value in urls.items():
             if key.startswith('<'):
                 if last_path:
                     if callable(value):
                         found_path += f'{key}/'
                         return value, found_path
+
+                    elif isinstance(value, dict) and '' in value:
+                        found_path += f'{key}/'
+                        return value[''], found_path
+
                     else:
                         return None, ''
 
-                sub = value
+                urls = value
                 found_path += f'{key}/'
                 _continue = True
                 break
 
         if _continue:
             continue
 
     return None, ''
 
 
-def is_recursive_merge(a, b):
-    both_mapping = isinstance(a, Mapping) and isinstance(b, Mapping)
-    both_counter = isinstance(a, Counter) and isinstance(b, Counter)
-    return both_mapping and not both_counter
-
-
-def deepmerge(dst, src):
-    for key in src:
-        if key in dst:
-            if is_recursive_merge(dst[key], src[key]):
-                deepmerge(dst[key], src[key])
-            else:
-                dst[key] = deepcopy(src[key])
-        else:
-            dst[key] = deepcopy(src[key])
-    return dst
-
-
-def merge(destination: MutableMapping, *sources) -> MutableMapping:
-    """Credit to Travis Clarke --> https://github.com/clarketm/mergedeep"""
-    return reduce(partial(deepmerge), sources, destination)
-
-
-def finalize_urls(urls: dict) -> dict:
-    urls_list = list()
-    for url, endpoint in urls.items():
-        path = dict()
-        for single_path in url.split('/')[:-1][::-1]:
-            path = {single_path: path or endpoint}
-        urls_list.append(path)
-    return merge(*urls_list) if urls_list else {}
+def collect_path_variables(request_path: str, found_path: str) -> dict:
+    found_path = found_path.removesuffix('/').removeprefix('/')
+    request_path = request_path.removesuffix('/').removeprefix('/')
+    path_variables = dict()
+    for f_path, r_path in zip(found_path.split('/'), request_path.split('/')):
+        if f_path.startswith('<'):
+            path_variables[f_path[1:-1]] = r_path
+    return path_variables
```

### Comparing `panther-1.7.9/panther/status.py` & `panther-2.0.0/panther/status.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.9/panther/utils.py` & `panther-2.0.0/panther/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import os
-from datetime import datetime, timedelta
+import hashlib
 from pathlib import Path
+from datetime import datetime, timedelta
+
 from panther.logger import logger
 
 
 def load_env(env_file: str | Path, /) -> dict[str, str]:
     variables = dict()
 
     if env_file is None or not os.path.isfile(env_file):
@@ -25,7 +27,13 @@
 def generate_secret_key() -> str:
     from cryptography.fernet import Fernet
     return Fernet.generate_key().decode()
 
 
 def round_datetime(dt: datetime, delta: timedelta):
     return datetime.min + round((dt - datetime.min) / delta) * delta
+
+
+def generate_hash_value_from_string(string_value: str) -> str:
+    # The point of this method is for maintinance, if we want to change
+    # the hash algorithm in the future, it's will be easy.
+    return hashlib.sha256(string_value.encode('utf-8')).hexdigest()
```

### Comparing `panther-1.7.9/panther.egg-info/SOURCES.txt` & `panther-2.0.0/panther.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -42,8 +42,12 @@
 panther/middlewares/__init__.py
 panther/middlewares/base.py
 panther/middlewares/db.py
 panther/middlewares/monitoring.py
 panther/middlewares/redis.py
 panther/panel/__init__.py
 panther/panel/apis.py
-panther/panel/urls.py
+panther/panel/urls.py
+panther/panel/utils.py
+tests/test_mongodb.py
+tests/test_pantherdb.py
+tests/test_routing.py
```

### Comparing `panther-1.7.9/setup.py` & `panther-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,27 +17,29 @@
         'pymongo>=4.3.3',
     ]
 }
 
 setup(
     name='panther',
     version=VERSION,
-    python_requires='>=3.11',
+    python_requires='>=3.10',
     author='Ali RajabNezhad',
     author_email='alirn76@yahoo.com',
     url='https://github.com/alirn76/panther',
     description='Fast &  Friendly, Web Framework For Building Async APIs',
     long_description=DESCRIPTION,
     long_description_content_type='text/markdown',
     include_package_data=True,
     license='MIT',
     classifiers=[
         'Operating System :: OS Independent',
         'License :: OSI Approved :: MIT License',
+        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
     entry_points={
         'console_scripts': ['panther=panther.cli.main:start'],
     },
     package_data={
         'panther': ['cli/*'],
     },
@@ -46,13 +48,12 @@
         'bson~=0.5',
         'httptools~=0.5',
         'pantherdb~=1.2',
         'pydantic~=2.0',
         'redis~=4.5',
         'rich~=13.3',
         'uvicorn~=0.21',
-        'uvloop~=0.17',
         'watchfiles~=0.18',
         'python-jose~=3.3',
     ],
     extras_require=EXTRAS_REQUIRE,
 )
```

