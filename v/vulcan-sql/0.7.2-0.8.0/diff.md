# Comparing `tmp/vulcan-sql-0.7.2.tar.gz` & `tmp/vulcan-sql-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vulcan-sql-0.7.2.tar", last modified: Mon Jul 31 09:41:24 2023, max compression
+gzip compressed data, was "vulcan-sql-0.8.0.tar", last modified: Fri Aug  4 11:09:09 2023, max compression
```

## Comparing `vulcan-sql-0.7.2.tar` & `vulcan-sql-0.8.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-31 09:41:24.135423 vulcan-sql-0.7.2/
--rw-r--r--   0 canner     (501) staff       (20)      397 2023-07-04 06:26:29.000000 vulcan-sql-0.7.2/MANIFEST.in
--rw-r--r--   0 canner     (501) staff       (20)      937 2023-07-31 09:41:24.135028 vulcan-sql-0.7.2/PKG-INFO
--rw-r--r--   0 canner     (501) staff       (20)      542 2023-07-04 02:03:53.000000 vulcan-sql-0.7.2/PUBLIC_README.md
--rw-r--r--   0 canner     (501) staff       (20)     4312 2023-07-27 10:31:34.000000 vulcan-sql-0.7.2/README.md
--rw-r--r--   0 canner     (501) staff       (20)       38 2023-07-31 09:41:24.135743 vulcan-sql-0.7.2/setup.cfg
--rw-r--r--   0 canner     (501) staff       (20)     1143 2023-07-31 09:08:47.000000 vulcan-sql-0.7.2/setup.py
-drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-31 09:41:24.131433 vulcan-sql-0.7.2/vulcan_sql.egg-info/
--rw-r--r--   0 canner     (501) staff       (20)      937 2023-07-31 09:41:24.000000 vulcan-sql-0.7.2/vulcan_sql.egg-info/PKG-INFO
--rw-r--r--   0 canner     (501) staff       (20)      259 2023-07-31 09:41:24.000000 vulcan-sql-0.7.2/vulcan_sql.egg-info/SOURCES.txt
--rw-r--r--   0 canner     (501) staff       (20)        1 2023-07-31 09:41:24.000000 vulcan-sql-0.7.2/vulcan_sql.egg-info/dependency_links.txt
--rw-r--r--   0 canner     (501) staff       (20)       52 2023-07-31 09:41:24.000000 vulcan-sql-0.7.2/vulcan_sql.egg-info/entry_points.txt
--rw-r--r--   0 canner     (501) staff       (20)       10 2023-07-31 09:41:24.000000 vulcan-sql-0.7.2/vulcan_sql.egg-info/top_level.txt
-drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-07-31 09:41:24.133755 vulcan-sql-0.7.2/vulcansql/
--rw-r--r--   0 canner     (501) staff       (20)      170 2023-07-04 02:03:53.000000 vulcan-sql-0.7.2/vulcansql/__init__.py
--rw-r--r--   0 canner     (501) staff       (20)     2147 2023-07-25 07:59:55.000000 vulcan-sql-0.7.2/vulcansql/cli.py
+drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-08-04 11:09:09.797399 vulcan-sql-0.8.0/
+-rw-r--r--   0 canner     (501) staff       (20)      397 2023-07-04 06:26:29.000000 vulcan-sql-0.8.0/MANIFEST.in
+-rw-r--r--   0 canner     (501) staff       (20)      937 2023-08-04 11:09:09.796799 vulcan-sql-0.8.0/PKG-INFO
+-rw-r--r--   0 canner     (501) staff       (20)      542 2023-07-04 02:03:53.000000 vulcan-sql-0.8.0/PUBLIC_README.md
+-rw-r--r--   0 canner     (501) staff       (20)     4312 2023-07-27 10:31:34.000000 vulcan-sql-0.8.0/README.md
+-rw-r--r--   0 canner     (501) staff       (20)       38 2023-08-04 11:09:09.797660 vulcan-sql-0.8.0/setup.cfg
+-rw-r--r--   0 canner     (501) staff       (20)     1143 2023-08-04 10:45:50.000000 vulcan-sql-0.8.0/setup.py
+drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-08-04 11:09:09.792056 vulcan-sql-0.8.0/vulcan_sql.egg-info/
+-rw-r--r--   0 canner     (501) staff       (20)      937 2023-08-04 11:09:09.000000 vulcan-sql-0.8.0/vulcan_sql.egg-info/PKG-INFO
+-rw-r--r--   0 canner     (501) staff       (20)      259 2023-08-04 11:09:09.000000 vulcan-sql-0.8.0/vulcan_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 canner     (501) staff       (20)        1 2023-08-04 11:09:09.000000 vulcan-sql-0.8.0/vulcan_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 canner     (501) staff       (20)       52 2023-08-04 11:09:09.000000 vulcan-sql-0.8.0/vulcan_sql.egg-info/entry_points.txt
+-rw-r--r--   0 canner     (501) staff       (20)       10 2023-08-04 11:09:09.000000 vulcan-sql-0.8.0/vulcan_sql.egg-info/top_level.txt
+drwxr-xr-x   0 canner     (501) staff       (20)        0 2023-08-04 11:09:09.794408 vulcan-sql-0.8.0/vulcansql/
+-rw-r--r--   0 canner     (501) staff       (20)      170 2023-07-04 02:03:53.000000 vulcan-sql-0.8.0/vulcansql/__init__.py
+-rw-r--r--   0 canner     (501) staff       (20)     2147 2023-07-25 07:59:55.000000 vulcan-sql-0.8.0/vulcansql/cli.py
```

### Comparing `vulcan-sql-0.7.2/PKG-INFO` & `vulcan-sql-0.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-sql
-Version: 0.7.2
+Version: 0.8.0
 Summary: VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.
 Home-page: https://github.com/Canner/vulcan-sql
 Author: Canner Team
 Author-email: contact@cannerdata.com
 License: Apache 2.0
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
```

### Comparing `vulcan-sql-0.7.2/PUBLIC_README.md` & `vulcan-sql-0.8.0/PUBLIC_README.md`

 * *Files identical despite different names*

### Comparing `vulcan-sql-0.7.2/README.md` & `vulcan-sql-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `vulcan-sql-0.7.2/setup.py` & `vulcan-sql-0.8.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # read the contents of your README file
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, "PUBLIC_README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup_kwargs = {
     'name': 'vulcan-sql',
-    'version': '0.7.2',
+    'version': '0.8.0',
     'description': 'VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.',
     'long_description': long_description,
     'long_description_content_type': "text/markdown",
     'author': 'Canner Team',
     'author_email': 'contact@cannerdata.com',
     'license': "Apache 2.0",
     'url': 'https://github.com/Canner/vulcan-sql',
```

### Comparing `vulcan-sql-0.7.2/vulcan_sql.egg-info/PKG-INFO` & `vulcan-sql-0.8.0/vulcan_sql.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vulcan-sql
-Version: 0.7.2
+Version: 0.8.0
 Summary: VulcanSQL turns your SQL templates into data APIs for efficient data sharing. No backend skills required. Empower your data sharing, faster.
 Home-page: https://github.com/Canner/vulcan-sql
 Author: Canner Team
 Author-email: contact@cannerdata.com
 License: Apache 2.0
 Requires-Python: >=3.0.0
 Description-Content-Type: text/markdown
```

### Comparing `vulcan-sql-0.7.2/vulcansql/cli.py` & `vulcan-sql-0.8.0/vulcansql/cli.py`

 * *Files identical despite different names*

