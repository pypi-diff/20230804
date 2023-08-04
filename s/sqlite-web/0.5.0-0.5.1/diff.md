# Comparing `tmp/sqlite-web-0.5.0.tar.gz` & `tmp/sqlite-web-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sqlite-web-0.5.0.tar", last modified: Mon Jun 26 01:40:16 2023, max compression
+gzip compressed data, was "dist/sqlite-web-0.5.1.tar", last modified: Fri Aug  4 18:42:36 2023, max compression
```

## Comparing `sqlite-web-0.5.0.tar` & `sqlite-web-0.5.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/
--rw-r--r--   0 charles   (1000) charles   (1000)       94 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/MANIFEST.in
--rw-r--r--   0 charles   (1000) charles   (1000)      511 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)     3835 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/README.md
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/docker/
--rw-r--r--   0 charles   (1000) charles   (1000)     2105 2023-04-19 14:27:45.000000 sqlite-web-0.5.0/docker/Dockerfile
--rwxr-xr-x   0 charles   (1000) charles   (1000)      334 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/run-docker
--rw-r--r--   0 charles   (1000) charles   (1000)       38 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/setup.cfg
--rw-r--r--   0 charles   (1000) charles   (1000)     1219 2023-06-26 01:38:48.000000 sqlite-web-0.5.0/setup.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/
--rw-r--r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/__init__.py
--rw-r--r--   0 charles   (1000) charles   (1000)      153 2022-03-11 19:44:53.000000 sqlite-web-0.5.0/sqlite_web/__main__.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/__pycache__/
--rw-r--r--   0 charles   (1000) charles   (1000)      139 2022-06-13 19:07:21.000000 sqlite-web-0.5.0/sqlite_web/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 charles   (1000) charles   (1000)      287 2022-06-13 19:07:21.000000 sqlite-web-0.5.0/sqlite_web/__pycache__/__main__.cpython-37.pyc
--rw-r--r--   0 charles   (1000) charles   (1000)    25756 2022-06-13 19:07:21.000000 sqlite-web-0.5.0/sqlite_web/__pycache__/sqlite_web.cpython-37.pyc
--rwxr-xr-x   0 charles   (1000) charles   (1000)    38799 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/sqlite_web.py
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/static/
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/static/css/
--rw-r--r--   0 charles   (1000) charles   (1000)   153641 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/css/bootstrap.min.css
--rw-r--r--   0 charles   (1000) charles   (1000)      169 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/css/sqlbrowse.css
--rw-r--r--   0 charles   (1000) charles   (1000)     3489 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/css/syntax-highlight.css
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/static/fonts/
--rw-r--r--   0 charles   (1000) charles   (1000)    20335 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 charles   (1000) charles   (1000)    62927 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 charles   (1000) charles   (1000)    41280 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 charles   (1000) charles   (1000)    23320 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/static/img/
--rw-r--r--   0 charles   (1000) charles   (1000)     8076 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/delete.png
--rw-r--r--   0 charles   (1000) charles   (1000)    42695 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/expression.png
--rw-r--r--   0 charles   (1000) charles   (1000)     7681 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/index-create.png
--rw-r--r--   0 charles   (1000) charles   (1000)     2982 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/index-drop.png
--rw-r--r--   0 charles   (1000) charles   (1000)    20342 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/insert.png
--rw-r--r--   0 charles   (1000) charles   (1000)    25300 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/select-advanced.png
--rw-r--r--   0 charles   (1000) charles   (1000)    14405 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/select.png
--rw-r--r--   0 charles   (1000) charles   (1000)     5221 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/table-alter.png
--rw-r--r--   0 charles   (1000) charles   (1000)    12190 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/table-create.png
--rw-r--r--   0 charles   (1000) charles   (1000)     3039 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/table-drop.png
--rw-r--r--   0 charles   (1000) charles   (1000)    23018 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/trigger-create.png
--rw-r--r--   0 charles   (1000) charles   (1000)     3669 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/trigger-drop.png
--rw-r--r--   0 charles   (1000) charles   (1000)    17914 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/update.png
--rw-r--r--   0 charles   (1000) charles   (1000)     7284 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/view-create.png
--rw-r--r--   0 charles   (1000) charles   (1000)     3040 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/img/view-drop.png
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/static/js/
--rw-r--r--   0 charles   (1000) charles   (1000)    67742 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/js/bootstrap.bundle.min.js
--rw-r--r--   0 charles   (1000) charles   (1000)    96381 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/static/js/jquery-1.11.0.min.js
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web/templates/
--rw-r--r--   0 charles   (1000) charles   (1000)     1090 2022-03-29 14:33:41.000000 sqlite-web-0.5.0/sqlite_web/templates/add_column.html
--rw-r--r--   0 charles   (1000) charles   (1000)     1086 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/add_index.html
--rw-r--r--   0 charles   (1000) charles   (1000)     3517 2022-03-29 14:33:41.000000 sqlite-web-0.5.0/sqlite_web/templates/base.html
--rw-r--r--   0 charles   (1000) charles   (1000)     1634 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/templates/base_table.html
--rw-r--r--   0 charles   (1000) charles   (1000)     1375 2021-05-26 21:50:16.000000 sqlite-web-0.5.0/sqlite_web/templates/base_tables.html
--rw-r--r--   0 charles   (1000) charles   (1000)      811 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/drop_column.html
--rw-r--r--   0 charles   (1000) charles   (1000)      777 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/drop_index.html
--rw-r--r--   0 charles   (1000) charles   (1000)      558 2023-04-17 10:00:39.000000 sqlite-web-0.5.0/sqlite_web/templates/drop_table.html
--rw-r--r--   0 charles   (1000) charles   (1000)      796 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/drop_trigger.html
--rw-r--r--   0 charles   (1000) charles   (1000)     1229 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/index.html
--rw-r--r--   0 charles   (1000) charles   (1000)      465 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/login.html
--rw-r--r--   0 charles   (1000) charles   (1000)     1139 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/rename_column.html
--rw-r--r--   0 charles   (1000) charles   (1000)     2873 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/templates/table_content.html
--rw-r--r--   0 charles   (1000) charles   (1000)      721 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/templates/table_delete.html
--rw-r--r--   0 charles   (1000) charles   (1000)     1060 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/templates/table_export.html
--rw-r--r--   0 charles   (1000) charles   (1000)     1345 2018-08-16 18:40:47.000000 sqlite-web-0.5.0/sqlite_web/templates/table_import.html
--rw-r--r--   0 charles   (1000) charles   (1000)     2690 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/templates/table_insert.html
--rw-r--r--   0 charles   (1000) charles   (1000)     5499 2023-04-11 19:10:55.000000 sqlite-web-0.5.0/sqlite_web/templates/table_query.html
--rw-r--r--   0 charles   (1000) charles   (1000)     5362 2023-04-11 19:10:55.000000 sqlite-web-0.5.0/sqlite_web/templates/table_structure.html
--rw-r--r--   0 charles   (1000) charles   (1000)     3175 2023-04-18 18:28:09.000000 sqlite-web-0.5.0/sqlite_web/templates/table_update.html
-drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/
--rw-r--r--   0 charles   (1000) charles   (1000)      511 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/PKG-INFO
--rw-r--r--   0 charles   (1000) charles   (1000)     2251 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/SOURCES.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        1 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/dependency_links.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       59 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/entry_points.txt
--rw-r--r--   0 charles   (1000) charles   (1000)        1 2022-12-09 13:29:02.000000 sqlite-web-0.5.0/sqlite_web.egg-info/not-zip-safe
--rw-r--r--   0 charles   (1000) charles   (1000)       29 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/requires.txt
--rw-r--r--   0 charles   (1000) charles   (1000)       11 2023-06-26 01:40:16.000000 sqlite-web-0.5.0/sqlite_web.egg-info/top_level.txt
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/
+-rw-r--r--   0 charles   (1000) charles   (1000)       94 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/MANIFEST.in
+-rw-r--r--   0 charles   (1000) charles   (1000)      511 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)     3835 2023-04-18 18:28:09.000000 sqlite-web-0.5.1/README.md
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/docker/
+-rw-r--r--   0 charles   (1000) charles   (1000)     2105 2023-04-19 14:27:45.000000 sqlite-web-0.5.1/docker/Dockerfile
+-rwxr-xr-x   0 charles   (1000) charles   (1000)      334 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/run-docker
+-rw-r--r--   0 charles   (1000) charles   (1000)       38 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/setup.cfg
+-rw-r--r--   0 charles   (1000) charles   (1000)     1219 2023-08-04 18:41:22.000000 sqlite-web-0.5.1/setup.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web/
+-rw-r--r--   0 charles   (1000) charles   (1000)        0 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/__init__.py
+-rw-r--r--   0 charles   (1000) charles   (1000)      153 2022-03-11 19:44:53.000000 sqlite-web-0.5.1/sqlite_web/__main__.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web/__pycache__/
+-rw-r--r--   0 charles   (1000) charles   (1000)      139 2022-06-13 19:07:21.000000 sqlite-web-0.5.1/sqlite_web/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 charles   (1000) charles   (1000)      287 2022-06-13 19:07:21.000000 sqlite-web-0.5.1/sqlite_web/__pycache__/__main__.cpython-37.pyc
+-rw-r--r--   0 charles   (1000) charles   (1000)    25756 2022-06-13 19:07:21.000000 sqlite-web-0.5.1/sqlite_web/__pycache__/sqlite_web.cpython-37.pyc
+-rwxr-xr-x   0 charles   (1000) charles   (1000)    38857 2023-08-04 18:40:43.000000 sqlite-web-0.5.1/sqlite_web/sqlite_web.py
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web/static/
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web/static/css/
+-rw-r--r--   0 charles   (1000) charles   (1000)   153641 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/css/bootstrap.min.css
+-rw-r--r--   0 charles   (1000) charles   (1000)      169 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/css/sqlbrowse.css
+-rw-r--r--   0 charles   (1000) charles   (1000)     3489 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/css/syntax-highlight.css
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web/static/fonts/
+-rw-r--r--   0 charles   (1000) charles   (1000)    20335 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 charles   (1000) charles   (1000)    62927 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 charles   (1000) charles   (1000)    41280 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 charles   (1000) charles   (1000)    23320 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web/static/img/
+-rw-r--r--   0 charles   (1000) charles   (1000)     8076 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/delete.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    42695 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/expression.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     7681 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/index-create.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     2982 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/index-drop.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    20342 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/insert.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    25300 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/select-advanced.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    14405 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/select.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     5221 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/table-alter.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    12190 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/table-create.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     3039 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/table-drop.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    23018 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/trigger-create.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     3669 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/trigger-drop.png
+-rw-r--r--   0 charles   (1000) charles   (1000)    17914 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/update.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     7284 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/view-create.png
+-rw-r--r--   0 charles   (1000) charles   (1000)     3040 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/img/view-drop.png
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web/static/js/
+-rw-r--r--   0 charles   (1000) charles   (1000)    67742 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/js/bootstrap.bundle.min.js
+-rw-r--r--   0 charles   (1000) charles   (1000)    96381 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/static/js/jquery-1.11.0.min.js
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web/templates/
+-rw-r--r--   0 charles   (1000) charles   (1000)     1090 2022-03-29 14:33:41.000000 sqlite-web-0.5.1/sqlite_web/templates/add_column.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1086 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/templates/add_index.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     3517 2022-03-29 14:33:41.000000 sqlite-web-0.5.1/sqlite_web/templates/base.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1634 2023-04-18 18:28:09.000000 sqlite-web-0.5.1/sqlite_web/templates/base_table.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1375 2021-05-26 21:50:16.000000 sqlite-web-0.5.1/sqlite_web/templates/base_tables.html
+-rw-r--r--   0 charles   (1000) charles   (1000)      811 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/templates/drop_column.html
+-rw-r--r--   0 charles   (1000) charles   (1000)      777 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/templates/drop_index.html
+-rw-r--r--   0 charles   (1000) charles   (1000)      558 2023-04-17 10:00:39.000000 sqlite-web-0.5.1/sqlite_web/templates/drop_table.html
+-rw-r--r--   0 charles   (1000) charles   (1000)      796 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/templates/drop_trigger.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1229 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/templates/index.html
+-rw-r--r--   0 charles   (1000) charles   (1000)      465 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/templates/login.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1139 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/templates/rename_column.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     2873 2023-04-18 18:28:09.000000 sqlite-web-0.5.1/sqlite_web/templates/table_content.html
+-rw-r--r--   0 charles   (1000) charles   (1000)      721 2023-04-18 18:28:09.000000 sqlite-web-0.5.1/sqlite_web/templates/table_delete.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1060 2023-04-18 18:28:09.000000 sqlite-web-0.5.1/sqlite_web/templates/table_export.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     1345 2018-08-16 18:40:47.000000 sqlite-web-0.5.1/sqlite_web/templates/table_import.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     2690 2023-04-18 18:28:09.000000 sqlite-web-0.5.1/sqlite_web/templates/table_insert.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     5630 2023-07-10 13:48:26.000000 sqlite-web-0.5.1/sqlite_web/templates/table_query.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     5362 2023-04-11 19:10:55.000000 sqlite-web-0.5.1/sqlite_web/templates/table_structure.html
+-rw-r--r--   0 charles   (1000) charles   (1000)     3175 2023-04-18 18:28:09.000000 sqlite-web-0.5.1/sqlite_web/templates/table_update.html
+drwxr-xr-x   0 charles   (1000) charles   (1000)        0 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web.egg-info/
+-rw-r--r--   0 charles   (1000) charles   (1000)      511 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web.egg-info/PKG-INFO
+-rw-r--r--   0 charles   (1000) charles   (1000)     2251 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web.egg-info/SOURCES.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)        1 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web.egg-info/dependency_links.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       59 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web.egg-info/entry_points.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)        1 2022-12-09 13:29:02.000000 sqlite-web-0.5.1/sqlite_web.egg-info/not-zip-safe
+-rw-r--r--   0 charles   (1000) charles   (1000)       29 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web.egg-info/requires.txt
+-rw-r--r--   0 charles   (1000) charles   (1000)       11 2023-08-04 18:42:36.000000 sqlite-web-0.5.1/sqlite_web.egg-info/top_level.txt
```

### Comparing `sqlite-web-0.5.0/README.md` & `sqlite-web-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/docker/Dockerfile` & `sqlite-web-0.5.1/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/setup.py` & `sqlite-web-0.5.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with open(readme) as fh:
         long_description = fh.read()
 else:
     long_description = ''
 
 setup(
     name='sqlite-web',
-    version='0.5.0',
+    version='0.5.1',
     description='Web-based SQLite database browser.',
     long_description='Web-based SQLite database browser.',
     author='Charles Leifer',
     author_email='coleifer@gmail.com',
     url='https://github.com/coleifer/sqlite-web',
     license='MIT',
     install_requires=[
```

### Comparing `sqlite-web-0.5.0/sqlite_web/__pycache__/sqlite_web.cpython-37.pyc` & `sqlite-web-0.5.1/sqlite_web/__pycache__/sqlite_web.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/sqlite_web.py` & `sqlite-web-0.5.1/sqlite_web/sqlite_web.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,14 +489,16 @@
         total_rows=total_rows)
 
 def minimal_validate_field(field, value):
     if value.lower().strip() == 'null':
         value = None
     if value is None and not field.null:
         return 'NULL', 'Column does not allow NULL values.'
+    if value is None:
+        return None, None
     if isinstance(field, IntegerField) and not value.isdigit():
         return value, 'Value is not a number.'
     elif isinstance(field, FloatField):
         try:
             _ = float(value)
         except Exception:
             return value, 'Value is not a numeric/real.'
@@ -605,15 +607,15 @@
         return redirect(url_for('table_content', table=table))
 
     expr = decode_pk(model, pk)
     try:
         obj = model.get(expr)
     except model.DoesNotExist:
         pk_repr = pk_display(table_pk, pk)
-        flash('Could not fetch row with primary-key %s.' % pk_repr, 'danger')
+        flash('Could not fetch row with primary-key %s.' % str(pk_repr), 'danger')
         return redirect(url_for('table_content', table=table))
 
     columns = dataset.get_columns(table)
     col_dict = {}
     row = {}
     for column in columns:
         value = getattr(obj, column.name)
@@ -683,15 +685,15 @@
         return redirect(url_for('table_content', table=table))
 
     expr = decode_pk(model, pk)
     try:
         row = model.select().where(expr).dicts().get()
     except model.DoesNotExist:
         pk_repr = pk_display(table_pk, pk)
-        flash('Could not fetch row with primary-key %s.' % pk_repr, 'danger')
+        flash('Could not fetch row with primary-key %s.' % str(pk_repr), 'danger')
         return redirect(url_for('table_content', table=table))
 
     if request.method == 'POST':
         try:
             with dataset.transaction() as txn:
                 n = model.delete().where(expr).execute()
         except Exception as exc:
```

### Comparing `sqlite-web-0.5.0/sqlite_web/static/css/bootstrap.min.css` & `sqlite-web-0.5.1/sqlite_web/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/css/syntax-highlight.css` & `sqlite-web-0.5.1/sqlite_web/static/css/syntax-highlight.css`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.eot` & `sqlite-web-0.5.1/sqlite_web/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.svg` & `sqlite-web-0.5.1/sqlite_web/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.ttf` & `sqlite-web-0.5.1/sqlite_web/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/fonts/glyphicons-halflings-regular.woff` & `sqlite-web-0.5.1/sqlite_web/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/delete.png` & `sqlite-web-0.5.1/sqlite_web/static/img/delete.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/expression.png` & `sqlite-web-0.5.1/sqlite_web/static/img/expression.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/index-create.png` & `sqlite-web-0.5.1/sqlite_web/static/img/index-create.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/index-drop.png` & `sqlite-web-0.5.1/sqlite_web/static/img/index-drop.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/insert.png` & `sqlite-web-0.5.1/sqlite_web/static/img/insert.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/select-advanced.png` & `sqlite-web-0.5.1/sqlite_web/static/img/select-advanced.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/select.png` & `sqlite-web-0.5.1/sqlite_web/static/img/select.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/table-alter.png` & `sqlite-web-0.5.1/sqlite_web/static/img/table-alter.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/table-create.png` & `sqlite-web-0.5.1/sqlite_web/static/img/table-create.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/table-drop.png` & `sqlite-web-0.5.1/sqlite_web/static/img/table-drop.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/trigger-create.png` & `sqlite-web-0.5.1/sqlite_web/static/img/trigger-create.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/trigger-drop.png` & `sqlite-web-0.5.1/sqlite_web/static/img/trigger-drop.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/update.png` & `sqlite-web-0.5.1/sqlite_web/static/img/update.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/view-create.png` & `sqlite-web-0.5.1/sqlite_web/static/img/view-create.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/img/view-drop.png` & `sqlite-web-0.5.1/sqlite_web/static/img/view-drop.png`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/js/bootstrap.bundle.min.js` & `sqlite-web-0.5.1/sqlite_web/static/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/static/js/jquery-1.11.0.min.js` & `sqlite-web-0.5.1/sqlite_web/static/js/jquery-1.11.0.min.js`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/add_column.html` & `sqlite-web-0.5.1/sqlite_web/templates/add_column.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/add_index.html` & `sqlite-web-0.5.1/sqlite_web/templates/add_index.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/base.html` & `sqlite-web-0.5.1/sqlite_web/templates/base.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/base_table.html` & `sqlite-web-0.5.1/sqlite_web/templates/base_table.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/base_tables.html` & `sqlite-web-0.5.1/sqlite_web/templates/base_tables.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/drop_column.html` & `sqlite-web-0.5.1/sqlite_web/templates/drop_column.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/drop_index.html` & `sqlite-web-0.5.1/sqlite_web/templates/drop_index.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/drop_table.html` & `sqlite-web-0.5.1/sqlite_web/templates/drop_table.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/drop_trigger.html` & `sqlite-web-0.5.1/sqlite_web/templates/drop_trigger.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/index.html` & `sqlite-web-0.5.1/sqlite_web/templates/index.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/rename_column.html` & `sqlite-web-0.5.1/sqlite_web/templates/rename_column.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/table_content.html` & `sqlite-web-0.5.1/sqlite_web/templates/table_content.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/table_delete.html` & `sqlite-web-0.5.1/sqlite_web/templates/table_delete.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/table_export.html` & `sqlite-web-0.5.1/sqlite_web/templates/table_export.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/table_import.html` & `sqlite-web-0.5.1/sqlite_web/templates/table_import.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/table_insert.html` & `sqlite-web-0.5.1/sqlite_web/templates/table_insert.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/table_query.html` & `sqlite-web-0.5.1/sqlite_web/templates/table_query.html`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,17 @@
       recentQueries = accum.slice(0, 20);
       localStorage.setItem('recentQueries', JSON.stringify(recentQueries));
   {% endif %}
       var historyIndex = 0;
       var sqlTextArea = $('textarea#sql');
 
       sqlTextArea.on('keydown', function(e) {
+        if ((e.metaKey || e.ctrlKey) && e.keyCode == 13) { // ctrl+enter or meta+enter.
+            $("form").submit();
+        }
         if (e.shiftKey) {
           if (e.keyCode == 38) { // up.
             historyIndex += 1;
             if (historyIndex >= recentQueries.length) { historyIndex = 0; }
             sqlTextArea.html(recentQueries[historyIndex]);
             e.preventDefault();
           } else if (e.keyCode == 40) { // down.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/table_structure.html` & `sqlite-web-0.5.1/sqlite_web/templates/table_structure.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web/templates/table_update.html` & `sqlite-web-0.5.1/sqlite_web/templates/table_update.html`

 * *Files identical despite different names*

### Comparing `sqlite-web-0.5.0/sqlite_web.egg-info/SOURCES.txt` & `sqlite-web-0.5.1/sqlite_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

