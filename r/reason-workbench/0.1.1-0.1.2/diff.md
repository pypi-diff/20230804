# Comparing `tmp/reason_workbench-0.1.1.tar.gz` & `tmp/reason_workbench-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reason_workbench-0.1.1.tar", last modified: Thu Aug  3 21:36:04 2023, max compression
+gzip compressed data, was "reason_workbench-0.1.2.tar", last modified: Fri Aug  4 19:30:59 2023, max compression
```

## Comparing `reason_workbench-0.1.1.tar` & `reason_workbench-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-03 21:36:04.941100 reason_workbench-0.1.1/
--rw-r--r--   0 joshbottum   (501) staff       (20)       60 2023-08-03 21:36:04.940668 reason_workbench-0.1.1/PKG-INFO
--rw-r--r--   0 joshbottum   (501) staff       (20)      189 2023-07-29 15:22:53.000000 reason_workbench-0.1.1/README.md
-drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-03 21:36:04.936049 reason_workbench-0.1.1/reason_workbench/
--rw-r--r--   0 joshbottum   (501) staff       (20)       32 2023-07-29 15:18:43.000000 reason_workbench-0.1.1/reason_workbench/__init__.py
--rw-r--r--   0 joshbottum   (501) staff       (20)    17468 2023-08-03 21:31:08.000000 reason_workbench-0.1.1/reason_workbench/main.py
-drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-03 21:36:04.940068 reason_workbench-0.1.1/reason_workbench.egg-info/
--rw-r--r--   0 joshbottum   (501) staff       (20)       60 2023-08-03 21:36:04.000000 reason_workbench-0.1.1/reason_workbench.egg-info/PKG-INFO
--rw-r--r--   0 joshbottum   (501) staff       (20)      314 2023-08-03 21:36:04.000000 reason_workbench-0.1.1/reason_workbench.egg-info/SOURCES.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)        1 2023-08-03 21:36:04.000000 reason_workbench-0.1.1/reason_workbench.egg-info/dependency_links.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)       64 2023-08-03 21:36:04.000000 reason_workbench-0.1.1/reason_workbench.egg-info/entry_points.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)       42 2023-08-03 21:36:04.000000 reason_workbench-0.1.1/reason_workbench.egg-info/requires.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)       17 2023-08-03 21:36:04.000000 reason_workbench-0.1.1/reason_workbench.egg-info/top_level.txt
--rw-r--r--   0 joshbottum   (501) staff       (20)       38 2023-08-03 21:36:04.941263 reason_workbench-0.1.1/setup.cfg
--rw-r--r--   0 joshbottum   (501) staff       (20)      418 2023-08-03 19:58:23.000000 reason_workbench-0.1.1/setup.py
+drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-04 19:30:59.119069 reason_workbench-0.1.2/
+-rw-r--r--   0 joshbottum   (501) staff       (20)       60 2023-08-04 19:30:59.118201 reason_workbench-0.1.2/PKG-INFO
+-rw-r--r--   0 joshbottum   (501) staff       (20)      189 2023-07-29 15:22:53.000000 reason_workbench-0.1.2/README.md
+drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-04 19:30:59.112362 reason_workbench-0.1.2/reason_workbench/
+-rw-r--r--   0 joshbottum   (501) staff       (20)       32 2023-07-29 15:18:43.000000 reason_workbench-0.1.2/reason_workbench/__init__.py
+-rw-r--r--   0 joshbottum   (501) staff       (20)    17468 2023-08-03 21:31:08.000000 reason_workbench-0.1.2/reason_workbench/main.py
+drwxr-xr-x   0 joshbottum   (501) staff       (20)        0 2023-08-04 19:30:59.117293 reason_workbench-0.1.2/reason_workbench.egg-info/
+-rw-r--r--   0 joshbottum   (501) staff       (20)       60 2023-08-04 19:30:58.000000 reason_workbench-0.1.2/reason_workbench.egg-info/PKG-INFO
+-rw-r--r--   0 joshbottum   (501) staff       (20)      314 2023-08-04 19:30:58.000000 reason_workbench-0.1.2/reason_workbench.egg-info/SOURCES.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)        1 2023-08-04 19:30:58.000000 reason_workbench-0.1.2/reason_workbench.egg-info/dependency_links.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)       64 2023-08-04 19:30:58.000000 reason_workbench-0.1.2/reason_workbench.egg-info/entry_points.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)       42 2023-08-04 19:30:58.000000 reason_workbench-0.1.2/reason_workbench.egg-info/requires.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)       17 2023-08-04 19:30:58.000000 reason_workbench-0.1.2/reason_workbench.egg-info/top_level.txt
+-rw-r--r--   0 joshbottum   (501) staff       (20)       38 2023-08-04 19:30:59.119277 reason_workbench-0.1.2/setup.cfg
+-rw-r--r--   0 joshbottum   (501) staff       (20)      418 2023-08-04 19:29:12.000000 reason_workbench-0.1.2/setup.py
```

### Comparing `reason_workbench-0.1.1/reason_workbench/main.py` & `reason_workbench-0.1.2/reason_workbench/main.py`

 * *Files identical despite different names*

