# Comparing `tmp/methodism-0.1.5.tar.gz` & `tmp/methodism-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "methodism-0.1.5.tar", last modified: Mon Jun  5 09:22:43 2023, max compression
+gzip compressed data, was "methodism-0.1.6.tar", last modified: Fri Aug  4 12:36:07 2023, max compression
```

## Comparing `methodism-0.1.5.tar` & `methodism-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 09:22:43.576184 methodism-0.1.5/
--rw-rw-rw-   0        0        0     4537 2023-06-05 09:22:43.576184 methodism-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4055 2023-06-05 09:21:58.000000 methodism-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 09:22:43.556042 methodism-0.1.5/methodism/
--rw-rw-rw-   0        0        0      449 2023-05-30 07:21:18.000000 methodism-0.1.5/methodism/__init__.py
--rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.1.5/methodism/costumizing.py
--rw-rw-rw-   0        0        0      856 2023-05-30 07:16:02.000000 methodism-0.1.5/methodism/decors.py
--rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.1.5/methodism/error_messages.py
--rw-rw-rw-   0        0        0     2192 2023-05-29 07:11:47.000000 methodism-0.1.5/methodism/helper.py
--rw-rw-rw-   0        0        0     6982 2023-06-05 09:21:58.000000 methodism-0.1.5/methodism/main.py
-drwxrwxrwx   0        0        0        0 2023-06-05 09:22:43.576184 methodism-0.1.5/methodism.egg-info/
--rw-rw-rw-   0        0        0     4537 2023-06-05 09:22:43.000000 methodism-0.1.5/methodism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-06-05 09:22:43.000000 methodism-0.1.5/methodism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 09:22:43.000000 methodism-0.1.5/methodism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-05 09:22:43.000000 methodism-0.1.5/methodism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      603 2023-06-05 09:21:58.000000 methodism-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0      546 2023-06-05 09:22:43.585229 methodism-0.1.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 12:36:07.908416 methodism-0.1.6/
+-rw-rw-rw-   0        0        0     4537 2023-08-04 12:36:07.908416 methodism-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4055 2023-06-05 09:21:58.000000 methodism-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 12:36:07.891892 methodism-0.1.6/methodism/
+-rw-rw-rw-   0        0        0      449 2023-05-30 07:21:18.000000 methodism-0.1.6/methodism/__init__.py
+-rw-rw-rw-   0        0        0     3583 2023-04-28 10:28:06.000000 methodism-0.1.6/methodism/costumizing.py
+-rw-rw-rw-   0        0        0      856 2023-05-30 07:16:02.000000 methodism-0.1.6/methodism/decors.py
+-rw-rw-rw-   0        0        0     6421 2023-04-27 06:52:43.000000 methodism-0.1.6/methodism/error_messages.py
+-rw-rw-rw-   0        0        0     2192 2023-05-29 07:11:47.000000 methodism-0.1.6/methodism/helper.py
+-rw-rw-rw-   0        0        0     7019 2023-08-04 12:34:12.000000 methodism-0.1.6/methodism/main.py
+drwxrwxrwx   0        0        0        0 2023-08-04 12:36:07.907422 methodism-0.1.6/methodism.egg-info/
+-rw-rw-rw-   0        0        0     4537 2023-08-04 12:36:07.000000 methodism-0.1.6/methodism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-08-04 12:36:07.000000 methodism-0.1.6/methodism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 12:36:07.000000 methodism-0.1.6/methodism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-04 12:36:07.000000 methodism-0.1.6/methodism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      603 2023-08-04 12:35:30.000000 methodism-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      546 2023-08-04 12:36:07.910421 methodism-0.1.6/setup.cfg
```

### Comparing `methodism-0.1.5/PKG-INFO` & `methodism-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.1.5
+Version: 0.1.6
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `methodism-0.1.5/README.md` & `methodism-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `methodism-0.1.5/methodism/costumizing.py` & `methodism-0.1.6/methodism/costumizing.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.5/methodism/decors.py` & `methodism-0.1.6/methodism/decors.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.5/methodism/error_messages.py` & `methodism-0.1.6/methodism/error_messages.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.5/methodism/helper.py` & `methodism-0.1.6/methodism/helper.py`

 * *Files identical despite different names*

### Comparing `methodism-0.1.5/methodism/main.py` & `methodism-0.1.6/methodism/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     not_auth_methods = []  # def hello_world() => hello.world
 
     @method_and_params_checker
     def post(self, requests, *args, **kwargs):
         method = requests.data.get("method")
         params = requests.data.get("params")
         headers = requests.headers
-        if method not in self.not_auth_methods:
+        if method not in self.not_auth_methods and "*" not in self.not_auth_methods:
             authorization = headers.get(self.auth_headers, '')
             pattern = re_compile(self.token_key + r" (.+)")
 
             if not pattern.match(authorization):
                 return Response(custom_response(status=False, method=method, message=MESSAGE['NotAuthenticated']))
             input_token = pattern.findall(authorization)[0]
```

### Comparing `methodism-0.1.5/methodism.egg-info/PKG-INFO` & `methodism-0.1.6/methodism.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: methodism
-Version: 0.1.5
+Version: 0.1.6
 Summary: Help to build APIs Faster
 Home-page: https://github.com/xudoyberdi123/Methodism
 Author: xudikk
 Author-email: xudikk <xudikk.1@gmail.com>
 Project-URL: Homepage, https://github.com/xudikk/Methodism
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `methodism-0.1.5/pyproject.toml` & `methodism-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "djangorestframework>=3.14.0",
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "methodism"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="xudikk", email="xudikk.1@gmail.com" },
 ]
 description = "Help to build APIs Faster"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `methodism-0.1.5/setup.cfg` & `methodism-0.1.6/setup.cfg`

 * *Files identical despite different names*

