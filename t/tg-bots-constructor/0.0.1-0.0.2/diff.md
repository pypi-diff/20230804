# Comparing `tmp/tg_bots_constructor-0.0.1.tar.gz` & `tmp/tg_bots_constructor-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_bots_constructor-0.0.1.tar", last modified: Fri Aug  4 15:05:13 2023, max compression
+gzip compressed data, was "tg_bots_constructor-0.0.2.tar", last modified: Fri Aug  4 15:13:27 2023, max compression
```

## Comparing `tg_bots_constructor-0.0.1.tar` & `tg_bots_constructor-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 15:05:13.940526 tg_bots_constructor-0.0.1/
--rw-rw-rw-   0        0        0      343 2023-08-04 15:05:13.938515 tg_bots_constructor-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-04 15:05:13.940526 tg_bots_constructor-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1247 2023-08-04 15:05:10.000000 tg_bots_constructor-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 15:05:13.934974 tg_bots_constructor-0.0.1/tg_bots_constructor.egg-info/
--rw-rw-rw-   0        0        0      343 2023-08-04 15:05:13.000000 tg_bots_constructor-0.0.1/tg_bots_constructor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-08-04 15:05:13.000000 tg_bots_constructor-0.0.1/tg_bots_constructor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 15:05:13.000000 tg_bots_constructor-0.0.1/tg_bots_constructor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-08-04 15:05:13.000000 tg_bots_constructor-0.0.1/tg_bots_constructor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-08-04 15:05:13.000000 tg_bots_constructor-0.0.1/tg_bots_constructor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 15:13:27.622776 tg_bots_constructor-0.0.2/
+-rw-rw-rw-   0        0        0      343 2023-08-04 15:13:27.620767 tg_bots_constructor-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-04 15:13:27.624779 tg_bots_constructor-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1247 2023-08-04 15:13:23.000000 tg_bots_constructor-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 15:13:27.568954 tg_bots_constructor-0.0.2/tg_bots_constructor/
+-rw-rw-rw-   0        0        0      157 2023-08-04 14:06:16.000000 tg_bots_constructor-0.0.2/tg_bots_constructor/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-08-04 09:04:25.000000 tg_bots_constructor-0.0.2/tg_bots_constructor/data.py
+-rw-rw-rw-   0        0        0      159 2023-08-04 07:54:47.000000 tg_bots_constructor-0.0.2/tg_bots_constructor/enviroment.py
+-rw-rw-rw-   0        0        0     2834 2023-08-04 09:01:25.000000 tg_bots_constructor-0.0.2/tg_bots_constructor/message_template.py
+drwxrwxrwx   0        0        0        0 2023-08-04 15:13:27.618765 tg_bots_constructor-0.0.2/tg_bots_constructor.egg-info/
+-rw-rw-rw-   0        0        0      343 2023-08-04 15:13:27.000000 tg_bots_constructor-0.0.2/tg_bots_constructor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      356 2023-08-04 15:13:27.000000 tg_bots_constructor-0.0.2/tg_bots_constructor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 15:13:27.000000 tg_bots_constructor-0.0.2/tg_bots_constructor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-08-04 15:13:27.000000 tg_bots_constructor-0.0.2/tg_bots_constructor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-08-04 15:13:27.000000 tg_bots_constructor-0.0.2/tg_bots_constructor.egg-info/top_level.txt
```

### Comparing `tg_bots_constructor-0.0.1/setup.py` & `tg_bots_constructor-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-version = '0.0.1'
+version = '0.0.2'
 
 
 setup(
     name='tg_bots_constructor',
     version=version,
 
     author='morpheus228',
```

