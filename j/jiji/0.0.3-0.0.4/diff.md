# Comparing `tmp/jiji-0.0.3.tar.gz` & `tmp/jiji-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiji-0.0.3.tar", last modified: Thu Aug  3 12:39:37 2023, max compression
+gzip compressed data, was "jiji-0.0.4.tar", last modified: Fri Aug  4 15:52:42 2023, max compression
```

## Comparing `jiji-0.0.3.tar` & `jiji-0.0.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.582543 jiji-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-03 12:39:37.582543 jiji-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 12:39:24.000000 jiji-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.578544 jiji-0.0.3/jiji/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.578544 jiji-0.0.3/jiji/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/jiji.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.578544 jiji-0.0.3/jiji/types/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/types/condition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.578544 jiji-0.0.3/jiji/types/product/
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/types/product/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.578544 jiji-0.0.3/jiji/types/search/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/types/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/types/sort.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-03 12:39:24.000000 jiji-0.0.3/jiji/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:39:37.578544 jiji-0.0.3/jiji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-03 12:39:37.000000 jiji-0.0.3/jiji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-03 12:39:37.000000 jiji-0.0.3/jiji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:39:37.000000 jiji-0.0.3/jiji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 12:39:37.000000 jiji-0.0.3/jiji.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:39:37.582543 jiji-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-03 12:39:24.000000 jiji-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:52:42.117552 jiji-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-04 15:52:42.117552 jiji-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 15:52:30.000000 jiji-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:52:42.113551 jiji-0.0.4/jiji/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 15:52:30.000000 jiji-0.0.4/jiji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-04 15:52:30.000000 jiji-0.0.4/jiji/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:52:42.113551 jiji-0.0.4/jiji/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-04 15:52:30.000000 jiji-0.0.4/jiji/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-08-04 15:52:30.000000 jiji-0.0.4/jiji/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7258 2023-08-04 15:52:30.000000 jiji-0.0.4/jiji/jiji.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:52:42.117552 jiji-0.0.4/jiji/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-04 15:52:30.000000 jiji-0.0.4/jiji/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-04 15:52:30.000000 jiji-0.0.4/jiji/types/condition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:52:42.117552 jiji-0.0.4/jiji/types/product/
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-08-04 15:52:30.000000 jiji-0.0.4/jiji/types/product/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:52:42.117552 jiji-0.0.4/jiji/types/search/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-04 15:52:30.000000 jiji-0.0.4/jiji/types/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-04 15:52:30.000000 jiji-0.0.4/jiji/types/sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-04 15:52:30.000000 jiji-0.0.4/jiji/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 15:52:42.113551 jiji-0.0.4/jiji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-04 15:52:42.000000 jiji-0.0.4/jiji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-04 15:52:42.000000 jiji-0.0.4/jiji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 15:52:42.000000 jiji-0.0.4/jiji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 15:52:42.000000 jiji-0.0.4/jiji.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 15:52:42.117552 jiji-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-04 15:52:30.000000 jiji-0.0.4/setup.py
```

### Comparing `jiji-0.0.3/jiji/filters.py` & `jiji-0.0.4/jiji/filters.py`

 * *Files identical despite different names*

### Comparing `jiji-0.0.3/jiji/jiji.py` & `jiji-0.0.4/jiji/jiji.py`

 * *Files identical despite different names*

### Comparing `jiji-0.0.3/jiji/types/product/__init__.py` & `jiji-0.0.4/jiji/types/product/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 @dataclass
 class Attribute:
     name: str
     value: Union[int, str]
     data_type: str
     unit: Optional[str]
     group_type: str
+    display_type: str | None = None
     # value_str: Union[int, str]
 
 
 @dataclass
 class Price:
     value: int
     view: str
```

