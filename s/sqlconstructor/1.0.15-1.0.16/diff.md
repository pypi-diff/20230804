# Comparing `tmp/sqlconstructor-1.0.15.tar.gz` & `tmp/sqlconstructor-1.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlconstructor-1.0.15.tar", last modified: Fri Aug  4 01:38:24 2023, max compression
+gzip compressed data, was "sqlconstructor-1.0.16.tar", last modified: Fri Aug  4 03:02:45 2023, max compression
```

## Comparing `sqlconstructor-1.0.15.tar` & `sqlconstructor-1.0.16.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-08-04 01:38:24.731502 sqlconstructor-1.0.15/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1071 2023-07-30 07:56:34.000000 sqlconstructor-1.0.15/LICENSE
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8809 2023-08-04 01:38:24.731502 sqlconstructor-1.0.15/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8008 2023-08-04 01:34:33.000000 sqlconstructor-1.0.15/README.md
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      867 2023-08-04 01:17:38.000000 sqlconstructor-1.0.15/pyproject.toml
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       38 2023-08-04 01:38:24.731502 sqlconstructor-1.0.15/setup.cfg
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-08-04 01:38:24.729502 sqlconstructor-1.0.15/src/
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-08-04 01:38:24.731502 sqlconstructor-1.0.15/src/sqlconstructor/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      252 2023-08-04 01:04:49.000000 sqlconstructor-1.0.15/src/sqlconstructor/__init__.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     2404 2023-08-04 01:04:49.000000 sqlconstructor-1.0.15/src/sqlconstructor/constants.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      744 2023-08-04 01:04:50.000000 sqlconstructor-1.0.15/src/sqlconstructor/helpers.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5124 2023-08-04 01:18:32.000000 sqlconstructor-1.0.15/src/sqlconstructor/sql_container.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1651 2023-08-04 01:20:13.000000 sqlconstructor-1.0.15/src/sqlconstructor/sql_cte.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5559 2023-08-04 01:16:46.000000 sqlconstructor-1.0.15/src/sqlconstructor/sql_query.py
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3893 2023-08-04 01:04:51.000000 sqlconstructor-1.0.15/src/sqlconstructor/sql_section.py
-drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-08-04 01:38:24.731502 sqlconstructor-1.0.15/src/sqlconstructor.egg-info/
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8809 2023-08-04 01:38:24.000000 sqlconstructor-1.0.15/src/sqlconstructor.egg-info/PKG-INFO
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)      425 2023-08-04 01:38:24.000000 sqlconstructor-1.0.15/src/sqlconstructor.egg-info/SOURCES.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)        1 2023-08-04 01:38:24.000000 sqlconstructor-1.0.15/src/sqlconstructor.egg-info/dependency_links.txt
--rw-r--r--   0 akvilary  (1000) akvilary  (1000)       15 2023-08-04 01:38:24.000000 sqlconstructor-1.0.15/src/sqlconstructor.egg-info/top_level.txt
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-08-04 03:02:45.479045 sqlconstructor-1.0.16/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1071 2023-07-30 07:56:34.000000 sqlconstructor-1.0.16/LICENSE
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8924 2023-08-04 03:02:45.479045 sqlconstructor-1.0.16/PKG-INFO
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8123 2023-08-04 03:00:35.000000 sqlconstructor-1.0.16/README.md
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      867 2023-08-04 03:02:12.000000 sqlconstructor-1.0.16/pyproject.toml
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)       38 2023-08-04 03:02:45.479045 sqlconstructor-1.0.16/setup.cfg
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-08-04 03:02:45.477045 sqlconstructor-1.0.16/src/
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-08-04 03:02:45.478045 sqlconstructor-1.0.16/src/sqlconstructor/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      252 2023-08-04 01:04:49.000000 sqlconstructor-1.0.16/src/sqlconstructor/__init__.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     2404 2023-08-04 01:04:49.000000 sqlconstructor-1.0.16/src/sqlconstructor/constants.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      744 2023-08-04 01:04:50.000000 sqlconstructor-1.0.16/src/sqlconstructor/helpers.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5130 2023-08-04 02:53:00.000000 sqlconstructor-1.0.16/src/sqlconstructor/sql_container.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     1651 2023-08-04 01:40:25.000000 sqlconstructor-1.0.16/src/sqlconstructor/sql_cte.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     5559 2023-08-04 01:16:46.000000 sqlconstructor-1.0.16/src/sqlconstructor/sql_query.py
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     3893 2023-08-04 01:04:51.000000 sqlconstructor-1.0.16/src/sqlconstructor/sql_section.py
+drwxr-xr-x   0 akvilary  (1000) akvilary  (1000)        0 2023-08-04 03:02:45.479045 sqlconstructor-1.0.16/src/sqlconstructor.egg-info/
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)     8924 2023-08-04 03:02:45.000000 sqlconstructor-1.0.16/src/sqlconstructor.egg-info/PKG-INFO
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)      425 2023-08-04 03:02:45.000000 sqlconstructor-1.0.16/src/sqlconstructor.egg-info/SOURCES.txt
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)        1 2023-08-04 03:02:45.000000 sqlconstructor-1.0.16/src/sqlconstructor.egg-info/dependency_links.txt
+-rw-r--r--   0 akvilary  (1000) akvilary  (1000)       15 2023-08-04 03:02:45.000000 sqlconstructor-1.0.16/src/sqlconstructor.egg-info/top_level.txt
```

### Comparing `sqlconstructor-1.0.15/LICENSE` & `sqlconstructor-1.0.16/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.15/PKG-INFO` & `sqlconstructor-1.0.16/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: sqlconstructor
-Version: 1.0.15
-Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!
-Author-email: Andrey Smirnov <abc-sm@yandex.ru>
-Project-URL: Homepage, https://github.com/akvilary/sqlconstructor
-Project-URL: Bug Tracker, https://github.com/akvilary/sqlconstructor/issues
-Project-URL: Telegram, https://t.me/sqlconstructor
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # sqlconstructor
 **sqlconstructor** is simple, yet very flexible, sql building tool.
 
 ## How to install
 You could install from PyPi:
 ```console
 $ python3 -m pip install sqlconstructor
@@ -86,16 +71,23 @@
 #### or later in SqlContainer
 ```python
 import sqlconstructor as sc
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    # set variables to existing container
+    # set variable to existing container
     container.vars['product_name'] = 'Smart'
+    # or
+    container(product_name='Smart')
+    # if you would like to remove all vars
+    container.vars.clear()
+	# if you would like to rewrite all vars
+	vars = {'product_name': 'Smart'}
+	container.vars = vars
 
 
 def get_product_query() -> sc.SqlContainer:
     q = sc.SqlQuery()
     q['select'](
         'id',
         'name',
@@ -114,18 +106,16 @@
 ```python
 import sqlconstructor as sc
 from functools import cache
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    # set single variable (and do not rewrite other variables)
+    # set variable to existing container
     container.vars['product_name'] = 'Smart'
-    # or you could rewrite all vars by
-    container(product_name='Smart')
 
 
 @cache
 def get_product_query() -> sc.SqlContainer:
     ...
 ```
```

### Comparing `sqlconstructor-1.0.15/README.md` & `sqlconstructor-1.0.16/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: sqlconstructor
+Version: 1.0.16
+Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!
+Author-email: Andrey Smirnov <abc-sm@yandex.ru>
+Project-URL: Homepage, https://github.com/akvilary/sqlconstructor
+Project-URL: Bug Tracker, https://github.com/akvilary/sqlconstructor/issues
+Project-URL: Telegram, https://t.me/sqlconstructor
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # sqlconstructor
 **sqlconstructor** is simple, yet very flexible, sql building tool.
 
 ## How to install
 You could install from PyPi:
 ```console
 $ python3 -m pip install sqlconstructor
@@ -71,16 +86,23 @@
 #### or later in SqlContainer
 ```python
 import sqlconstructor as sc
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    # set variables to existing container
+    # set variable to existing container
     container.vars['product_name'] = 'Smart'
+    # or
+    container(product_name='Smart')
+    # if you would like to remove all vars
+    container.vars.clear()
+	# if you would like to rewrite all vars
+	vars = {'product_name': 'Smart'}
+	container.vars = vars
 
 
 def get_product_query() -> sc.SqlContainer:
     q = sc.SqlQuery()
     q['select'](
         'id',
         'name',
@@ -99,18 +121,16 @@
 ```python
 import sqlconstructor as sc
 from functools import cache
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    # set single variable (and do not rewrite other variables)
+    # set variable to existing container
     container.vars['product_name'] = 'Smart'
-    # or you could rewrite all vars by
-    container(product_name='Smart')
 
 
 @cache
 def get_product_query() -> sc.SqlContainer:
     ...
 ```
```

### Comparing `sqlconstructor-1.0.15/pyproject.toml` & `sqlconstructor-1.0.16/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sqlconstructor"
-version = "1.0.15"
+version = "1.0.16"
 authors = [
   { name="Andrey Smirnov", email="abc-sm@yandex.ru" },
 ]
 description = "Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `sqlconstructor-1.0.15/src/sqlconstructor/constants.py` & `sqlconstructor-1.0.16/src/sqlconstructor/constants.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.15/src/sqlconstructor/helpers.py` & `sqlconstructor-1.0.16/src/sqlconstructor/helpers.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.15/src/sqlconstructor/sql_container.py` & `sqlconstructor-1.0.16/src/sqlconstructor/sql_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
     def __bool__(self):
         """True if self.text is True"""
         return bool(self.text)
 
     def __call__(self, **kwargs) -> Self:
         """Let you pass keyword arguments for later use in replacement job"""
-        self.vars = kwargs
+        self.vars.update(kwargs)
         return self
 
     def __repr__(self) -> str:
         """Convert SqlContainer instance to str"""
         return get_string_representation(self.text, self.wrapper_text)
 
     def __str__(self) -> str:
```

### Comparing `sqlconstructor-1.0.15/src/sqlconstructor/sql_cte.py` & `sqlconstructor-1.0.16/src/sqlconstructor/sql_cte.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.15/src/sqlconstructor/sql_query.py` & `sqlconstructor-1.0.16/src/sqlconstructor/sql_query.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.15/src/sqlconstructor/sql_section.py` & `sqlconstructor-1.0.16/src/sqlconstructor/sql_section.py`

 * *Files identical despite different names*

### Comparing `sqlconstructor-1.0.15/src/sqlconstructor.egg-info/PKG-INFO` & `sqlconstructor-1.0.16/src/sqlconstructor.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlconstructor
-Version: 1.0.15
+Version: 1.0.16
 Summary: Let you build SQL requests in pythonic way. SQL blocks could be nested and flexible as you want it to be, constructed dynamically and look pretty! You could also build request once and cache it (but still use variables to replace dynamically). Solid solution!
 Author-email: Andrey Smirnov <abc-sm@yandex.ru>
 Project-URL: Homepage, https://github.com/akvilary/sqlconstructor
 Project-URL: Bug Tracker, https://github.com/akvilary/sqlconstructor/issues
 Project-URL: Telegram, https://t.me/sqlconstructor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -86,16 +86,23 @@
 #### or later in SqlContainer
 ```python
 import sqlconstructor as sc
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    # set variables to existing container
+    # set variable to existing container
     container.vars['product_name'] = 'Smart'
+    # or
+    container(product_name='Smart')
+    # if you would like to remove all vars
+    container.vars.clear()
+	# if you would like to rewrite all vars
+	vars = {'product_name': 'Smart'}
+	container.vars = vars
 
 
 def get_product_query() -> sc.SqlContainer:
     q = sc.SqlQuery()
     q['select'](
         'id',
         'name',
@@ -114,18 +121,16 @@
 ```python
 import sqlconstructor as sc
 from functools import cache
 
 
 def main():
     container: sc.SqlContainer = get_product_query()
-    # set single variable (and do not rewrite other variables)
+    # set variable to existing container
     container.vars['product_name'] = 'Smart'
-    # or you could rewrite all vars by
-    container(product_name='Smart')
 
 
 @cache
 def get_product_query() -> sc.SqlContainer:
     ...
 ```
```

