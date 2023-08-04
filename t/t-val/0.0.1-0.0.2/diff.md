# Comparing `tmp/t_val-0.0.1.tar.gz` & `tmp/t_val-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\t_val-0.0.1.tar", last modified: Fri Aug  4 11:24:47 2023, max compression
+gzip compressed data, was "dist\t_val-0.0.2.tar", last modified: Fri Aug  4 11:42:08 2023, max compression
```

## Comparing `t_val-0.0.1.tar` & `t_val-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 11:24:47.000000 t_val-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-08-04 11:24:47.000000 t_val-0.0.1/libname/
--rw-rw-rw-   0        0        0      405 2023-08-04 11:17:21.000000 t_val-0.0.1/libname/t_val.py
--rw-rw-rw-   0        0        0       26 2023-08-04 09:59:35.000000 t_val-0.0.1/libname/__init__.py
--rw-rw-rw-   0        0        0      269 2023-08-04 11:24:47.000000 t_val-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-04 11:24:47.000000 t_val-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      398 2023-08-04 10:38:19.000000 t_val-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 11:24:47.000000 t_val-0.0.1/t_val.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-04 11:24:47.000000 t_val-0.0.1/t_val.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      269 2023-08-04 11:24:47.000000 t_val-0.0.1/t_val.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-08-04 11:24:47.000000 t_val-0.0.1/t_val.egg-info/requires.txt
--rw-rw-rw-   0        0        0      189 2023-08-04 11:24:47.000000 t_val-0.0.1/t_val.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-08-04 11:24:47.000000 t_val-0.0.1/t_val.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 11:42:08.000000 t_val-0.0.2/
+drwxrwxrwx   0        0        0        0 2023-08-04 11:42:08.000000 t_val-0.0.2/libname/
+-rw-rw-rw-   0        0        0      405 2023-08-04 11:17:21.000000 t_val-0.0.2/libname/t_val.py
+-rw-rw-rw-   0        0        0       26 2023-08-04 09:59:35.000000 t_val-0.0.2/libname/__init__.py
+-rw-rw-rw-   0        0        0      269 2023-08-04 11:42:08.000000 t_val-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-04 11:42:08.000000 t_val-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      386 2023-08-04 11:36:56.000000 t_val-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:42:08.000000 t_val-0.0.2/t_val.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-04 11:42:08.000000 t_val-0.0.2/t_val.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      269 2023-08-04 11:42:08.000000 t_val-0.0.2/t_val.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-08-04 11:42:08.000000 t_val-0.0.2/t_val.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-08-04 11:42:08.000000 t_val-0.0.2/t_val.egg-info/top_level.txt
```

