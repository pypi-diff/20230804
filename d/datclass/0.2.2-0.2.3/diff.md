# Comparing `tmp/datclass-0.2.2.tar.gz` & `tmp/datclass-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datclass-0.2.2.tar", last modified: Tue Apr 18 05:49:03 2023, max compression
+gzip compressed data, was "datclass-0.2.3.tar", last modified: Fri Aug  4 11:38:20 2023, max compression
```

## Comparing `datclass-0.2.2.tar` & `datclass-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:49:03.440471 datclass-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-18 05:48:56.000000 datclass-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 05:48:56.000000 datclass-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-18 05:49:03.440471 datclass-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-04-18 05:48:56.000000 datclass-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-18 05:48:56.000000 datclass-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 05:48:56.000000 datclass-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 05:49:03.440471 datclass-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:49:03.436471 datclass-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:49:03.436471 datclass-0.2.2/src/datclass/
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-04-18 05:49:02.000000 datclass-0.2.2/src/datclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 05:48:56.000000 datclass-0.2.2/src/datclass/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-04-18 05:48:56.000000 datclass-0.2.2/src/datclass/gens.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-18 05:48:56.000000 datclass-0.2.2/src/datclass/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:49:03.440471 datclass-0.2.2/src/datclass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-18 05:49:03.000000 datclass-0.2.2/src/datclass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-18 05:49:03.000000 datclass-0.2.2/src/datclass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 05:49:03.000000 datclass-0.2.2/src/datclass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 05:49:03.000000 datclass-0.2.2/src/datclass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-18 05:49:03.000000 datclass-0.2.2/src/datclass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 05:49:03.000000 datclass-0.2.2/src/datclass.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:38:20.801518 datclass-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-04 11:38:10.000000 datclass-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-04 11:38:10.000000 datclass-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-08-04 11:38:20.797517 datclass-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-08-04 11:38:10.000000 datclass-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-04 11:38:10.000000 datclass-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 11:38:10.000000 datclass-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 11:38:20.801518 datclass-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:38:20.797517 datclass-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:38:20.797517 datclass-0.2.3/src/datclass/
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-08-04 11:38:19.000000 datclass-0.2.3/src/datclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:38:10.000000 datclass-0.2.3/src/datclass/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8163 2023-08-04 11:38:10.000000 datclass-0.2.3/src/datclass/gens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-08-04 11:38:10.000000 datclass-0.2.3/src/datclass/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 11:38:20.797517 datclass-0.2.3/src/datclass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-08-04 11:38:20.000000 datclass-0.2.3/src/datclass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-04 11:38:20.000000 datclass-0.2.3/src/datclass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 11:38:20.000000 datclass-0.2.3/src/datclass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-04 11:38:20.000000 datclass-0.2.3/src/datclass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-04 11:38:20.000000 datclass-0.2.3/src/datclass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-04 11:38:20.000000 datclass-0.2.3/src/datclass.egg-info/top_level.txt
```

### Comparing `datclass-0.2.2/LICENSE` & `datclass-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datclass-0.2.2/PKG-INFO` & `datclass-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datclass
-Version: 0.2.2
+Version: 0.2.3
 Summary: python package dataclass utils
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/datclass
 Project-URL: Homepage, https://github.com/foyoux/datclass
 Project-URL: Bug Tracker, https://github.com/foyoux/datclass/issues
 Keywords: dataclass
 Classifier: Programming Language :: Python
```

### Comparing `datclass-0.2.2/README.md` & `datclass-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `datclass-0.2.2/pyproject.toml` & `datclass-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datclass-0.2.2/src/datclass/__init__.py` & `datclass-0.2.3/src/datclass/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __title__ = 'datclass'
 __author__ = 'foyoux'
-__version__ = '0.2.2'
+__version__ = '0.2.3'
 
 __all__ = [
     'main',
     'DatGen',
     'DatClass',
     'get_datclass',
 ]
@@ -67,15 +67,15 @@
                 origin = get_origin(attr_type)
                 if origin is None and is_dataclass(attr_type):
                     attr = getattr(self, attr_name)
                     setattr(self, attr_name, attr_type(**attr) if attr else None)
                     continue
                 for item_type in get_args(attr_type):
                     if is_dataclass(item_type):
-                        setattr(self, attr_name, [item_type(**i) for i in getattr(self, attr_name)])
+                        setattr(self, attr_name, [item_type(**i) for i in getattr(self, attr_name) or []])
 
     return __datclass__
 
 
 DatClass = get_datclass()
```

### Comparing `datclass-0.2.2/src/datclass/gens.py` & `datclass-0.2.3/src/datclass/gens.py`

 * *Files identical despite different names*

### Comparing `datclass-0.2.2/src/datclass/utils.py` & `datclass-0.2.3/src/datclass/utils.py`

 * *Files identical despite different names*

### Comparing `datclass-0.2.2/src/datclass.egg-info/PKG-INFO` & `datclass-0.2.3/src/datclass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datclass
-Version: 0.2.2
+Version: 0.2.3
 Summary: python package dataclass utils
 Author: foyoux
 Project-URL: Source, https://github.com/foyoux/datclass
 Project-URL: Homepage, https://github.com/foyoux/datclass
 Project-URL: Bug Tracker, https://github.com/foyoux/datclass/issues
 Keywords: dataclass
 Classifier: Programming Language :: Python
```

