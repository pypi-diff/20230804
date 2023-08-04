# Comparing `tmp/foo_bar_lib_probe-0.1.tar.gz` & `tmp/foo_bar_lib_probe-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foo_bar_lib_probe-0.1.tar", last modified: Fri Aug  4 11:07:21 2023, max compression
+gzip compressed data, was "foo_bar_lib_probe-0.2.tar", last modified: Fri Aug  4 11:26:35 2023, max compression
```

## Comparing `foo_bar_lib_probe-0.1.tar` & `foo_bar_lib_probe-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 11:07:21.685441 foo_bar_lib_probe-0.1/
--rw-rw-rw-   0        0        0     1106 2023-08-04 10:27:13.000000 foo_bar_lib_probe-0.1/LICENSE
--rw-rw-rw-   0        0        0      255 2023-08-04 11:07:21.685441 foo_bar_lib_probe-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      257 2023-08-04 11:04:47.000000 foo_bar_lib_probe-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 11:07:21.685441 foo_bar_lib_probe-0.1/foo_bar_lib_probe/
--rw-rw-rw-   0        0        0        0 2023-08-04 10:20:46.000000 foo_bar_lib_probe-0.1/foo_bar_lib_probe/__init__.py
--rw-rw-rw-   0        0        0       80 2023-08-04 10:40:26.000000 foo_bar_lib_probe-0.1/foo_bar_lib_probe/foo.py
-drwxrwxrwx   0        0        0        0 2023-08-04 11:07:21.685441 foo_bar_lib_probe-0.1/foo_bar_lib_probe.egg-info/
--rw-rw-rw-   0        0        0      255 2023-08-04 11:07:21.000000 foo_bar_lib_probe-0.1/foo_bar_lib_probe.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-08-04 11:07:21.000000 foo_bar_lib_probe-0.1/foo_bar_lib_probe.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 11:07:21.000000 foo_bar_lib_probe-0.1/foo_bar_lib_probe.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-08-04 11:07:21.000000 foo_bar_lib_probe-0.1/foo_bar_lib_probe.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 11:07:21.685441 foo_bar_lib_probe-0.1/setup.cfg
--rw-rw-rw-   0        0        0      315 2023-08-04 10:54:27.000000 foo_bar_lib_probe-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:26:35.924203 foo_bar_lib_probe-0.2/
+-rw-rw-rw-   0        0        0     1106 2023-08-04 10:27:13.000000 foo_bar_lib_probe-0.2/LICENSE
+-rw-rw-rw-   0        0        0      251 2023-08-04 11:26:35.924203 foo_bar_lib_probe-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-08-04 11:08:01.000000 foo_bar_lib_probe-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 11:26:35.924203 foo_bar_lib_probe-0.2/foo_bar_lib_probe/
+-rw-rw-rw-   0        0        0        0 2023-08-04 10:20:46.000000 foo_bar_lib_probe-0.2/foo_bar_lib_probe/__init__.py
+-rw-rw-rw-   0        0        0       80 2023-08-04 10:40:26.000000 foo_bar_lib_probe-0.2/foo_bar_lib_probe/foo.py
+drwxrwxrwx   0        0        0        0 2023-08-04 11:26:35.924203 foo_bar_lib_probe-0.2/foo_bar_lib_probe.egg-info/
+-rw-rw-rw-   0        0        0      251 2023-08-04 11:26:35.000000 foo_bar_lib_probe-0.2/foo_bar_lib_probe.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-08-04 11:26:35.000000 foo_bar_lib_probe-0.2/foo_bar_lib_probe.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 11:26:35.000000 foo_bar_lib_probe-0.2/foo_bar_lib_probe.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-08-04 11:26:35.000000 foo_bar_lib_probe-0.2/foo_bar_lib_probe.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 11:26:35.924203 foo_bar_lib_probe-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      334 2023-08-04 11:25:52.000000 foo_bar_lib_probe-0.2/setup.py
```

### Comparing `foo_bar_lib_probe-0.1/LICENSE` & `foo_bar_lib_probe-0.2/LICENSE`

 * *Files identical despite different names*

