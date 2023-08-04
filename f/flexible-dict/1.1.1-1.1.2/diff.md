# Comparing `tmp/flexible_dict-1.1.1.tar.gz` & `tmp/flexible_dict-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexible_dict-1.1.1.tar", last modified: Tue Jul 25 03:24:28 2023, max compression
+gzip compressed data, was "flexible_dict-1.1.2.tar", last modified: Fri Aug  4 11:32:38 2023, max compression
```

## Comparing `flexible_dict-1.1.1.tar` & `flexible_dict-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-25 03:24:28.475708 flexible_dict-1.1.1/
--rw-r--r--   0 bytedance   (501) staff       (20)     1248 2023-07-25 03:24:28.475598 flexible_dict-1.1.1/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      959 2023-07-24 11:06:26.000000 flexible_dict-1.1.1/README.md
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-25 03:24:28.473820 flexible_dict-1.1.1/flexible_dict/
--rw-r--r--   0 bytedance   (501) staff       (20)      182 2023-07-24 08:27:54.000000 flexible_dict-1.1.1/flexible_dict/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      508 2023-07-24 09:58:30.000000 flexible_dict-1.1.1/flexible_dict/__main__.py
--rw-r--r--   0 bytedance   (501) staff       (20)       88 2023-07-25 03:17:53.000000 flexible_dict-1.1.1/flexible_dict/about.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5203 2023-07-24 08:26:14.000000 flexible_dict-1.1.1/flexible_dict/json_object.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-25 03:24:28.475002 flexible_dict-1.1.1/flexible_dict/script/
--rw-r--r--   0 bytedance   (501) staff       (20)       24 2023-07-24 09:41:19.000000 flexible_dict-1.1.1/flexible_dict/script/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5360 2023-07-25 03:14:12.000000 flexible_dict-1.1.1/flexible_dict/script/class_builder.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-25 03:24:28.474628 flexible_dict-1.1.1/flexible_dict.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)     1248 2023-07-25 03:24:28.000000 flexible_dict-1.1.1/flexible_dict.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      393 2023-07-25 03:24:28.000000 flexible_dict-1.1.1/flexible_dict.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-25 03:24:28.000000 flexible_dict-1.1.1/flexible_dict.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       14 2023-07-25 03:24:28.000000 flexible_dict-1.1.1/flexible_dict.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-07-25 03:24:28.475750 flexible_dict-1.1.1/setup.cfg
--rw-r--r--   0 bytedance   (501) staff       (20)      970 2023-07-24 10:52:09.000000 flexible_dict-1.1.1/setup.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-25 03:24:28.475279 flexible_dict-1.1.1/tests/
--rw-r--r--   0 bytedance   (501) staff       (20)      625 2023-07-25 03:17:01.000000 flexible_dict-1.1.1/tests/test_build_class.py
--rw-r--r--   0 bytedance   (501) staff       (20)      410 2023-07-24 08:27:54.000000 flexible_dict-1.1.1/tests/test_json_object.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-04 11:32:38.655166 flexible_dict-1.1.2/
+-rw-r--r--   0 bytedance   (501) staff       (20)     2080 2023-08-04 11:32:38.655022 flexible_dict-1.1.2/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)     1791 2023-08-04 11:30:22.000000 flexible_dict-1.1.2/README.md
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-04 11:32:38.653164 flexible_dict-1.1.2/flexible_dict/
+-rw-r--r--   0 bytedance   (501) staff       (20)      208 2023-07-28 02:13:43.000000 flexible_dict-1.1.2/flexible_dict/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      508 2023-07-24 09:58:30.000000 flexible_dict-1.1.2/flexible_dict/__main__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)       88 2023-08-04 11:21:04.000000 flexible_dict-1.1.2/flexible_dict/about.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9197 2023-07-28 02:13:43.000000 flexible_dict-1.1.2/flexible_dict/json_object.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-04 11:32:38.654137 flexible_dict-1.1.2/flexible_dict/script/
+-rw-r--r--   0 bytedance   (501) staff       (20)       24 2023-07-26 03:47:11.000000 flexible_dict-1.1.2/flexible_dict/script/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5360 2023-07-25 03:14:12.000000 flexible_dict-1.1.2/flexible_dict/script/class_builder.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-04 11:32:38.653750 flexible_dict-1.1.2/flexible_dict.egg-info/
+-rw-r--r--   0 bytedance   (501) staff       (20)     2080 2023-08-04 11:32:38.000000 flexible_dict-1.1.2/flexible_dict.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)      393 2023-08-04 11:32:38.000000 flexible_dict-1.1.2/flexible_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-08-04 11:32:38.000000 flexible_dict-1.1.2/flexible_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       14 2023-08-04 11:32:38.000000 flexible_dict-1.1.2/flexible_dict.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       38 2023-08-04 11:32:38.655219 flexible_dict-1.1.2/setup.cfg
+-rw-r--r--   0 bytedance   (501) staff       (20)      970 2023-07-24 10:52:09.000000 flexible_dict-1.1.2/setup.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-08-04 11:32:38.654793 flexible_dict-1.1.2/tests/
+-rw-r--r--   0 bytedance   (501) staff       (20)      625 2023-07-25 03:17:01.000000 flexible_dict-1.1.2/tests/test_build_class.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1112 2023-07-28 02:13:43.000000 flexible_dict-1.1.2/tests/test_json_object.py
```

### Comparing `flexible_dict-1.1.1/PKG-INFO` & `flexible_dict-1.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,25 @@
-Metadata-Version: 2.1
-Name: flexible_dict
-Version: 1.1.1
-Summary: A flexible way to access dict data instead of built-in dict.
-Home-page: https://github.com/darkpeath/flexible_dict
-Author: darkpeath
-Author-email: darkpeath@gmail.com
-Platform: any
-Description-Content-Type: text/markdown
-
-
 # Flexible Dict
 
 A flexible way to access dict data instead of built-in dict.
 
 ## Installation
 
 ```shell
 pip install flexible-dict
 ```
 
 ## Usage
 
 ### Define a dict class and access value
 
+#### Way 1
+
+Use a decorator `json_object` to make class to be a flexible dict.
+
 ```python
 from flexible_dict import json_object, MISSING
 
 @json_object
 class A:
     i: int = 3
     j: str = "init value"
@@ -40,14 +33,60 @@
 print(a.j)
 
 a.j = "update value"  # set value
 
 print(a['j'])  # access value via native dict way
 ```
 
+**There is a bug in init a nested json_object dict  with a non-empty dict, be careful when init a dict or use Way 2 instead.**
+
+#### Way 2 (suggested)
+
+Inherit the `JsonObject` class to define a flexible dict.
+
+```python
+from flexible_dict import JsonObject, MISSING
+
+class A(JsonObject):
+    i: int = 3
+    j: str = None
+    s: float
+    g: int = MISSING
+    
+class B(JsonObject):
+    a: A
+    k: int = 5
+
+a = A()
+assert a.i == 3
+assert a.j is None
+assert a.s is None
+try:
+    a.g
+except KeyError:
+    pass
+else:
+    assert False
+a.j = 10
+assert a.j == 10
+assert a['j'] == 10
+
+b = B({"a": {"i": 7, "j": 21}})
+assert b.k == 5
+assert b.a.i == 7
+assert b.a.j == 21
+assert b.a.s is None
+try:
+    b.a.g
+except KeyError:
+    pass
+else:
+    assert False
+```
+
 ### Build a json_object class from json data
 
 Suppose there is a file named `a.py` with content
 
 ```json
 {
   "a": 1,
@@ -71,8 +110,7 @@
 
 @json_object
 class A:
     a: int
     b: str
     c: dict
 ```
-
```

### Comparing `flexible_dict-1.1.1/flexible_dict/script/class_builder.py` & `flexible_dict-1.1.2/flexible_dict/script/class_builder.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.1.1/flexible_dict.egg-info/PKG-INFO` & `flexible_dict-1.1.2/flexible_dict.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flexible-dict
-Version: 1.1.1
+Version: 1.1.2
 Summary: A flexible way to access dict data instead of built-in dict.
 Home-page: https://github.com/darkpeath/flexible_dict
 Author: darkpeath
 Author-email: darkpeath@gmail.com
 Platform: any
 Description-Content-Type: text/markdown
 
@@ -19,14 +19,18 @@
 pip install flexible-dict
 ```
 
 ## Usage
 
 ### Define a dict class and access value
 
+#### Way 1
+
+Use a decorator `json_object` to make class to be a flexible dict.
+
 ```python
 from flexible_dict import json_object, MISSING
 
 @json_object
 class A:
     i: int = 3
     j: str = "init value"
@@ -40,14 +44,60 @@
 print(a.j)
 
 a.j = "update value"  # set value
 
 print(a['j'])  # access value via native dict way
 ```
 
+**There is a bug in init a nested json_object dict  with a non-empty dict, be careful when init a dict or use Way 2 instead.**
+
+#### Way 2 (suggested)
+
+Inherit the `JsonObject` class to define a flexible dict.
+
+```python
+from flexible_dict import JsonObject, MISSING
+
+class A(JsonObject):
+    i: int = 3
+    j: str = None
+    s: float
+    g: int = MISSING
+    
+class B(JsonObject):
+    a: A
+    k: int = 5
+
+a = A()
+assert a.i == 3
+assert a.j is None
+assert a.s is None
+try:
+    a.g
+except KeyError:
+    pass
+else:
+    assert False
+a.j = 10
+assert a.j == 10
+assert a['j'] == 10
+
+b = B({"a": {"i": 7, "j": 21}})
+assert b.k == 5
+assert b.a.i == 7
+assert b.a.j == 21
+assert b.a.s is None
+try:
+    b.a.g
+except KeyError:
+    pass
+else:
+    assert False
+```
+
 ### Build a json_object class from json data
 
 Suppose there is a file named `a.py` with content
 
 ```json
 {
   "a": 1,
@@ -71,8 +121,7 @@
 
 @json_object
 class A:
     a: int
     b: str
     c: dict
 ```
-
```

### Comparing `flexible_dict-1.1.1/setup.py` & `flexible_dict-1.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.1.1/tests/test_build_class.py` & `flexible_dict-1.1.2/tests/test_build_class.py`

 * *Files identical despite different names*

