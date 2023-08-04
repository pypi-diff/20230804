# Comparing `tmp/hyper-bump-it-0.4.1.tar.gz` & `tmp/hyper-bump-it-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyper-bump-it-0.4.1.tar", last modified: Sun May  7 21:42:06 2023, max compression
+gzip compressed data, was "hyper-bump-it-0.5.0.tar", last modified: Fri Aug  4 14:03:32 2023, max compression
```

## Comparing `hyper-bump-it-0.4.1.tar` & `hyper-bump-it-0.5.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.747787 hyper-bump-it-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-07 21:42:06.747787 hyper-bump-it-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.739787 hyper-bump-it-0.4.1/hyper_bump_it/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.743787 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.743787 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/by.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5948 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.743787 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/file_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/top_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/to.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.747787 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/keystone_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/execution_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.747787 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/matching_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/text_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/planned_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/vcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/hyper_bump_it/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:42:06.739787 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5412 2023-05-07 21:42:06.000000 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-07 21:42:06.000000 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:42:06.000000 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-07 21:42:06.000000 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-07 21:42:06.000000 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-07 21:42:06.000000 hyper-bump-it-0.4.1/hyper_bump_it.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 21:42:06.747787 hyper-bump-it-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-07 21:41:51.000000 hyper-bump-it-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:03:32.360273 hyper-bump-it-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-08-04 14:03:32.356273 hyper-bump-it-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:03:32.352273 hyper-bump-it-0.5.0/hyper_bump_it/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:03:32.352273 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:03:32.356273 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/by.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5984 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:03:32.356273 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/interactive/file_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/interactive/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/interactive/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/interactive/top_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/to.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:03:32.356273 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/config/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/config/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/config/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10186 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/config/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/config/keystone_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15814 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/execution_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3154 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:03:32.356273 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/format_pattern/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/format_pattern/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/format_pattern/keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/format_pattern/matching_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4457 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/format_pattern/text_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/planned_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/vcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/hyper_bump_it/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:03:32.352273 hyper-bump-it-0.5.0/hyper_bump_it.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-08-04 14:03:32.000000 hyper-bump-it-0.5.0/hyper_bump_it.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-08-04 14:03:32.000000 hyper-bump-it-0.5.0/hyper_bump_it.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:03:32.000000 hyper-bump-it-0.5.0/hyper_bump_it.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-04 14:03:32.000000 hyper-bump-it-0.5.0/hyper_bump_it.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-04 14:03:32.000000 hyper-bump-it-0.5.0/hyper_bump_it.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-04 14:03:32.000000 hyper-bump-it-0.5.0/hyper_bump_it.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 14:03:32.360273 hyper-bump-it-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-04 14:03:22.000000 hyper-bump-it-0.5.0/setup.py
```

### Comparing `hyper-bump-it-0.4.1/LICENSE` & `hyper-bump-it-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.1/PKG-INFO` & `hyper-bump-it-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyper-bump-it
-Version: 0.4.1
+Version: 0.5.0
 Summary: A version bumping tool
 Author-email: Patrick Lannigan <p.lannigan@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/plannigan/hyper-bump-it
 Project-URL: changelog, https://github.com/plannigan/hyper-bump-it/blob/main/CHANGELOG.md
 Project-URL: issues, https://github.com/plannigan/hyper-bump-it/issues
 Keywords: version,bump,command line
@@ -20,14 +20,15 @@
 
 [![CI pipeline status](https://github.com/plannigan/hyper-bump-it/actions/workflows/main.yml/badge.svg?branch=main)][ci]
 [![PyPI](https://img.shields.io/pypi/v/hyper-bump-it)][pypi]
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyper-bump-it)][pypi]
 [![codecov](https://codecov.io/gh/plannigan/hyper-bump-it/branch/main/graph/badge.svg?token=V4DADJU0BI)][codecov]
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)][mypy-home]
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)][black-home]
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/plannigan/hyper-bump-it/badge)][scorecard]
 
 # Hyper Bump It
 
 A command line tool for updating the version in project files needed for the next release.
 
 `hyper-bump-it`'s features include:
 
@@ -147,7 +148,8 @@
 ```
 
 [ci]: https://github.com/plannigan/hyper-bump-it/actions
 [pypi]: https://pypi.org/project/hyper-bump-it/
 [codecov]: https://codecov.io/gh/plannigan/hyper-bump-it
 [mypy-home]: http://mypy-lang.org/
 [black-home]: https://github.com/psf/black
+[scorecard]: https://securityscorecards.dev/viewer/?uri=github.com/plannigan/hyper-bump-it
```

### Comparing `hyper-bump-it-0.4.1/README.md` & `hyper-bump-it-0.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [![CI pipeline status](https://github.com/plannigan/hyper-bump-it/actions/workflows/main.yml/badge.svg?branch=main)][ci]
 [![PyPI](https://img.shields.io/pypi/v/hyper-bump-it)][pypi]
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyper-bump-it)][pypi]
 [![codecov](https://codecov.io/gh/plannigan/hyper-bump-it/branch/main/graph/badge.svg?token=V4DADJU0BI)][codecov]
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)][mypy-home]
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)][black-home]
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/plannigan/hyper-bump-it/badge)][scorecard]
 
 # Hyper Bump It
 
 A command line tool for updating the version in project files needed for the next release.
 
 `hyper-bump-it`'s features include:
 
@@ -127,7 +128,8 @@
 ```
 
 [ci]: https://github.com/plannigan/hyper-bump-it/actions
 [pypi]: https://pypi.org/project/hyper-bump-it/
 [codecov]: https://codecov.io/gh/plannigan/hyper-bump-it
 [mypy-home]: http://mypy-lang.org/
 [black-home]: https://github.com/psf/black
+[scorecard]: https://securityscorecards.dev/viewer/?uri=github.com/plannigan/hyper-bump-it
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/by.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/by.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,15 +35,20 @@
     remote: Annotated[Optional[str], common.remote()] = None,
     commit_format_pattern: Annotated[
         Optional[str], common.commit_format_pattern()
     ] = None,
     branch_format_pattern: Annotated[
         Optional[str], common.branch_format_pattern()
     ] = None,
-    tag_format_pattern: Annotated[Optional[str], common.tag_format_pattern()] = None,
+    tag_name_format_pattern: Annotated[
+        Optional[str], common.tag_name_format_pattern()
+    ] = None,
+    tag_message_format_pattern: Annotated[
+        Optional[str], common.tag_message_format_pattern()
+    ] = None,
     allowed_init_branch: Annotated[
         Optional[list[str]], common.allowed_init_branch()
     ] = None,
     allow_any_init_branch: Annotated[
         Optional[bool], common.allow_any_init_branch()
     ] = None,
 ) -> None:
@@ -62,15 +67,16 @@
                 current_version=current_version,
                 commit=commit,
                 branch=branch,
                 tag=tag,
                 remote=remote,
                 commit_format_pattern=commit_format_pattern,
                 branch_format_pattern=branch_format_pattern,
-                tag_format_pattern=tag_format_pattern,
+                tag_name_format_pattern=tag_name_format_pattern,
+                tag_message_format_pattern=tag_message_format_pattern,
                 allowed_initial_branches=common.allowed_init_branches(
                     allowed_init_branch, allow_any_init_branch
                 ),
             )
         )
 
         core.do_bump(app_config)
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/common.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,18 @@
 branch = _create_option_factory("Control branch Git action")
 tag = _create_option_factory("Control tag Git action")
 remote = _create_option_factory("Name of remote to use when pushing changes")
 commit_format_pattern = _create_option_factory(
     "Format pattern to use for commit message"
 )
 branch_format_pattern = _create_option_factory("Format pattern to use for branch name")
-tag_format_pattern = _create_option_factory("Format pattern to use for tag name")
+tag_name_format_pattern = _create_option_factory("Format pattern to use for tag name")
+tag_message_format_pattern = _create_option_factory(
+    "Format pattern to use for tag message"
+)
 # Typer returns an empty tuple even when the default is None and the argument is annotated as Optional[list[str]]
 # https://github.com/tiangolo/typer/issues/170
 allowed_init_branch = _create_option_factory(
     "Name of allowed initial branch (can be used multiple times)"
 )
 allow_any_init_branch = _create_option_factory(
     "Disable any initial branch restrictions. (takes precedence over --allowed-init-branch)",
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/init.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/init.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     DEFAULT_ALLOWED_INITIAL_BRANCHES,
     DEFAULT_BRANCH_ACTION,
     DEFAULT_BRANCH_FORMAT_PATTERN,
     DEFAULT_COMMIT_ACTION,
     DEFAULT_COMMIT_FORMAT_PATTERN,
     DEFAULT_REMOTE,
     DEFAULT_TAG_ACTION,
-    DEFAULT_TAG_FORMAT_PATTERN,
+    DEFAULT_TAG_NAME_FORMAT_PATTERN,
     HYPER_CONFIG_FILE_NAME,
     PYPROJECT_FILE_NAME,
     PYPROJECT_SUB_TABLE_KEYS,
     ROOT_TABLE_KEY,
     ConfigFile,
     FileDefinition,
     GitAction,
@@ -81,17 +81,17 @@
     ] = DEFAULT_REMOTE,
     commit_format_pattern: Annotated[
         str, common.commit_format_pattern(GIT_PANEL_NAME, show_default=True)
     ] = DEFAULT_COMMIT_FORMAT_PATTERN,
     branch_format_pattern: Annotated[
         str, common.branch_format_pattern(GIT_PANEL_NAME, show_default=True)
     ] = DEFAULT_BRANCH_FORMAT_PATTERN,
-    tag_format_pattern: Annotated[
-        str, common.tag_format_pattern(GIT_PANEL_NAME, show_default=True)
-    ] = DEFAULT_TAG_FORMAT_PATTERN,
+    tag_name_format_pattern: Annotated[
+        str, common.tag_name_format_pattern(GIT_PANEL_NAME, show_default=True)
+    ] = DEFAULT_TAG_NAME_FORMAT_PATTERN,
     allowed_init_branch: Annotated[
         list[str], common.allowed_init_branch(GIT_PANEL_NAME, show_default=True)
     ] = list(DEFAULT_ALLOWED_INITIAL_BRANCHES),
     allow_any_init_branch: Annotated[
         bool, common.allow_any_init_branch(GIT_PANEL_NAME)
     ] = False,
 ) -> None:
@@ -107,15 +107,15 @@
     config = ConfigFile(
         current_version=current_version,
         files=[FileDefinition(file_glob=common.EXAMPLE_FILE_GLOB)],
         git=GitConfigFile(
             remote=remote,
             commit_format_pattern=commit_format_pattern,
             branch_format_pattern=branch_format_pattern,
-            tag_format_pattern=tag_format_pattern,
+            tag_name_format_pattern=tag_name_format_pattern,
             allowed_initial_branches=frozenset(allowed_init_branch),
             actions=actions,
         ),
     )
     with common.handle_bump_errors():
         if non_interactive:
             ui.display(
@@ -152,15 +152,15 @@
 
 
 def _write_config(config: Mapping, config_file: Path) -> None:  # type: ignore[type-arg]
     config_file.write_text(tomlkit.dumps(config))
 
 
 def _config_to_dict(config: ConfigFile) -> dict:  # type: ignore[type-arg]
-    config_dict = config.dict(exclude_defaults=True)
+    config_dict = config.model_dump(exclude_defaults=True)
     if config.current_version is not None:
         config_dict["current_version"] = str(config.current_version)
     _git_branch_set_to_list(config_dict, "allowed_initial_branches")
     _git_branch_set_to_list(config_dict, "extend_allowed_initial_branches")
     return {ROOT_TABLE_KEY: config_dict}
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/file_validation.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/interactive/file_validation.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/files.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/interactive/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     Done = "done"
 
 
 class FilesConfigEditor:
     def __init__(
         self, initial_config: list[FileDefinition], validator: DefinitionValidator
     ) -> None:
-        self._config = [file.copy() for file in initial_config]
+        self._config = [file.model_copy() for file in initial_config]
         self._validator = validator
         self._config_funcs = {
             FilesMenu.Add: self._add_definition,
             FilesMenu.Remove: self._remove_definition,
             FilesMenu.Edit: self._edit_definition,
             FilesMenu.List: self._list_definitions,
         }
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/git.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/interactive/git.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,41 +11,44 @@
 from ...config import (
     DEFAULT_BRANCH_ACTION,
     DEFAULT_BRANCH_FORMAT_PATTERN,
     DEFAULT_COMMIT_ACTION,
     DEFAULT_COMMIT_FORMAT_PATTERN,
     DEFAULT_REMOTE,
     DEFAULT_TAG_ACTION,
-    DEFAULT_TAG_FORMAT_PATTERN,
+    DEFAULT_TAG_MESSAGE_FORMAT_PATTERN,
+    DEFAULT_TAG_NAME_FORMAT_PATTERN,
     GitAction,
     GitActionsConfigFile,
     GitConfigFile,
 )
 from ...config.core import DEFAULT_ALLOWED_INITIAL_BRANCHES
 from ...error import first_error_message
 
 
 class GitMenu(Enum):
     Remote = "remote"
     CommitFormatPattern = "commit"
     BranchFormatPattern = "branch"
-    TagFormatPattern = "tag"
+    TagNameFormatPattern = "tag-name"
+    TagMessageFormatPattern = "tag-message"
     AllowedBranches = "allowed-branches"
     Actions = "actions"
     Done = "done"
 
 
 class GitConfigEditor:
     def __init__(self, initial_config: GitConfigFile) -> None:
-        self._config: GitConfigFile = initial_config.copy(deep=True)
+        self._config: GitConfigFile = initial_config.model_copy(deep=True)
         self._config_funcs = {
             GitMenu.Remote: self._configure_remote,
             GitMenu.CommitFormatPattern: self._configure_commit_format_pattern,
             GitMenu.BranchFormatPattern: self._configure_branch_format_pattern,
-            GitMenu.TagFormatPattern: self._configure_tag_format_pattern,
+            GitMenu.TagNameFormatPattern: self._configure_tag_name_format_pattern,
+            GitMenu.TagMessageFormatPattern: self._configure_tag_message_format_pattern,
             GitMenu.AllowedBranches: self._configure_allowed_branches,
             GitMenu.Actions: self._configure_actions,
         }
 
     def configure(self) -> GitConfigFile:
         """
         Use interactive prompts to allow the user to edit the configuration.
@@ -75,27 +78,35 @@
         self._configure_format_pattern(
             "branch name",
             "branch_format_pattern",
             self._config.branch_format_pattern,
             DEFAULT_BRANCH_FORMAT_PATTERN,
         )
 
-    def _configure_tag_format_pattern(self) -> None:
+    def _configure_tag_name_format_pattern(self) -> None:
         self._configure_format_pattern(
             "tag name",
-            "tag_format_pattern",
-            self._config.tag_format_pattern,
-            DEFAULT_TAG_FORMAT_PATTERN,
+            "tag_name_format_pattern",
+            self._config.tag_name_format_pattern,
+            DEFAULT_TAG_NAME_FORMAT_PATTERN,
+        )
+
+    def _configure_tag_message_format_pattern(self) -> None:
+        self._configure_format_pattern(
+            "tag name",
+            "tag_format_message_pattern",
+            self._config.tag_message_format_pattern,
+            DEFAULT_TAG_MESSAGE_FORMAT_PATTERN,
         )
 
     def _configure_allowed_branches(self) -> None:
         allowed_branches, extend_overload_branches = AllowedBranchEditor(
             self._config.allowed_initial_branches
         ).configure()
-        self._config = self._config.copy(
+        self._config = self._config.model_copy(
             update={
                 "allowed_initial_branches": allowed_branches,
                 "extend_allowed_initial_branches": extend_overload_branches,
             }
         )
 
     def _configure_format_pattern(
@@ -106,15 +117,15 @@
         )
         ui.blank_line()
 
     def _store_update(
         self, config_name: str, value: Union[Optional[str], frozenset[str]]
     ) -> None:
         if value is not None:
-            self._config = self._config.copy(update={config_name: value})
+            self._config = self._config.model_copy(update={config_name: value})
 
     def _configure_actions(self) -> None:
         ui.display("There are three Git actions: create, branch, tag")
         ui.display(
             Text("They can each be set to: ")
             .append(GitAction.Skip.value, style="vcs.action")
             .append(", ")
@@ -145,26 +156,27 @@
                 ui.display(
                     Text("")
                     .append("Error", style="invalid")
                     .append(": ")
                     .append(first_error_message(ex))
                 )
 
-        self._config = self._config.copy(update={"actions": actions})
+        self._config = self._config.model_copy(update={"actions": actions})
         ui.blank_line()
 
 
 def _prompt_git_menu() -> GitMenu:
     return ui.choice_enum(
         "What part of configuration would you like to edit?",
         option_descriptions={
             GitMenu.Remote: "Name of remote to use when pushing changes",
             GitMenu.CommitFormatPattern: "Format pattern to use for commit message",
             GitMenu.BranchFormatPattern: "Format pattern to use for branch name",
-            GitMenu.TagFormatPattern: "Format pattern to use for tag name",
+            GitMenu.TagNameFormatPattern: "Format pattern to use for tag name",
+            GitMenu.TagMessageFormatPattern: "Format pattern to use for tag message",
             GitMenu.AllowedBranches: "Names of allowed initial branches",
             GitMenu.Actions: "Configure what Git actions should be performed",
             GitMenu.Done: "Stop editing the Git integration settings",
         },
         default=GitMenu.Done,
     )
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/interactive/top_level.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/interactive/top_level.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         project_root: Path,
     ) -> None:
         if initial_config.current_version is None:
             raise ValueError(
                 "The current version of the initial config must not be None."
             )
         self._current_version: Version = initial_config.current_version
-        self._config: ConfigFile = initial_config.copy(deep=True)
+        self._config: ConfigFile = initial_config.model_copy(deep=True)
         self._pyproject = pyproject
         self._project_root = project_root
         self._was_configured: Set[TopMenu] = set()
         self._config_funcs = {
             TopMenu.General: self._configure_general,
             TopMenu.Files: self._configure_files,
             TopMenu.Git: self._configure_git,
@@ -60,32 +60,32 @@
         return self._config, self._pyproject
 
     def _configure_general(self) -> None:
         show_confirm_prompt = _prompt_show_confirm(self._config.show_confirm_prompt)
         ui.blank_line()
         self._pyproject = _prompt_pyproject(self._pyproject)
         ui.blank_line()
-        self._config = self._config.copy(
+        self._config = self._config.model_copy(
             update={"show_confirm_prompt": show_confirm_prompt}
         )
 
     def _configure_files(self) -> None:
         editor = FilesConfigEditor(
             self._config.files,
             DefinitionValidator(self._current_version, self._project_root),
         )
         file_config, has_keystone = editor.configure()
         current_version = None if has_keystone else self._current_version
-        self._config = self._config.copy(
+        self._config = self._config.model_copy(
             update={"files": file_config, "current_version": current_version}
         )
 
     def _configure_git(self) -> None:
         editor = GitConfigEditor(self._config.git)
-        self._config = self._config.copy(update={"git": editor.configure()})
+        self._config = self._config.model_copy(update={"git": editor.configure()})
 
 
 def _prompt_top_level_menu() -> TopMenu:
     return ui.choice_enum(
         "What part of configuration would you like to edit?",
         option_descriptions={
             TopMenu.General: "Top level settings that don't fit in a specific category",
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/cli/to.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/cli/to.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,20 @@
     remote: Annotated[Optional[str], common.remote()] = None,
     commit_format_pattern: Annotated[
         Optional[str], common.commit_format_pattern()
     ] = None,
     branch_format_pattern: Annotated[
         Optional[str], common.branch_format_pattern()
     ] = None,
-    tag_format_pattern: Annotated[Optional[str], common.tag_format_pattern()] = None,
+    tag_name_format_pattern: Annotated[
+        Optional[str], common.tag_name_format_pattern()
+    ] = None,
+    tag_message_format_pattern: Annotated[
+        Optional[str], common.tag_message_format_pattern()
+    ] = None,
     allowed_init_branch: Annotated[
         Optional[list[str]], common.allowed_init_branch()
     ] = None,
     allow_any_init_branch: Annotated[
         Optional[bool], common.allow_any_init_branch()
     ] = None,
 ) -> None:
@@ -67,15 +72,16 @@
                 current_version=current_version,
                 commit=commit,
                 branch=branch,
                 tag=tag,
                 remote=remote,
                 commit_format_pattern=commit_format_pattern,
                 branch_format_pattern=branch_format_pattern,
-                tag_format_pattern=tag_format_pattern,
+                tag_name_format_pattern=tag_name_format_pattern,
+                tag_message_format_pattern=tag_message_format_pattern,
                 allowed_initial_branches=common.allowed_init_branches(
                     allowed_init_branch, allow_any_init_branch
                 ),
             )
         )
 
         core.do_bump(app_config)
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/compat.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/compat.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/__init__.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/config/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,16 @@
     DEFAULT_BRANCH_ACTION,
     DEFAULT_BRANCH_FORMAT_PATTERN,
     DEFAULT_COMMIT_ACTION,
     DEFAULT_COMMIT_FORMAT_PATTERN,
     DEFAULT_REMOTE,
     DEFAULT_SEARCH_PATTERN,
     DEFAULT_TAG_ACTION,
-    DEFAULT_TAG_FORMAT_PATTERN,
+    DEFAULT_TAG_MESSAGE_FORMAT_PATTERN,
+    DEFAULT_TAG_NAME_FORMAT_PATTERN,
     HYPER_CONFIG_FILE_NAME,
     PYPROJECT_FILE_NAME,
     GitAction,
 )
 from .file import (
     PYPROJECT_SUB_TABLE_KEYS,
     ROOT_TABLE_KEY,
@@ -36,15 +37,16 @@
     "BumpPart",
     "BumpToArgs",
     "Config",
     "ConfigFile",
     "ConfigVersionUpdater",
     "DEFAULT_ALLOWED_INITIAL_BRANCHES",
     "DEFAULT_TAG_ACTION",
-    "DEFAULT_TAG_FORMAT_PATTERN",
+    "DEFAULT_TAG_MESSAGE_FORMAT_PATTERN",
+    "DEFAULT_TAG_NAME_FORMAT_PATTERN",
     "DEFAULT_REMOTE",
     "DEFAULT_SEARCH_PATTERN",
     "DEFAULT_COMMIT_ACTION",
     "DEFAULT_COMMIT_FORMAT_PATTERN",
     "DEFAULT_BRANCH_FORMAT_PATTERN",
     "DEFAULT_BRANCH_ACTION",
     "File",
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/application.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/config/application.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 
 
 @dataclass
 class Git:
     remote: str
     commit_format_pattern: str
     branch_format_pattern: str
-    tag_format_pattern: str
+    tag_name_format_pattern: str
+    tag_message_format_pattern: str
     allowed_initial_branches: frozenset[str]
     actions: GitActions
 
 
 @dataclass
 class File:
     file_glob: str
@@ -165,15 +166,18 @@
 
 
 def _convert_git(args: Union[BumpToArgs, BumpByArgs], git: file.Git) -> Git:
     return Git(
         remote=args.remote or git.remote,
         commit_format_pattern=args.commit_format_pattern or git.commit_format_pattern,
         branch_format_pattern=args.branch_format_pattern or git.branch_format_pattern,
-        tag_format_pattern=args.tag_format_pattern or git.tag_format_pattern,
+        tag_name_format_pattern=args.tag_name_format_pattern
+        or git.tag_name_format_pattern,
+        tag_message_format_pattern=args.tag_message_format_pattern
+        or git.tag_message_format_pattern,
         allowed_initial_branches=_merge_allowed_branches(
             args.allowed_initial_branches,
             git.allowed_initial_branches,
             git.extend_allowed_initial_branches,
         ),
         actions=GitActions(
             commit=args.commit or git.actions.commit,
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/cli.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/config/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,15 +24,16 @@
     current_version: Optional[Version]
     commit: Optional[GitAction]
     branch: Optional[GitAction]
     tag: Optional[GitAction]
     remote: Optional[str]
     commit_format_pattern: Optional[str]
     branch_format_pattern: Optional[str]
-    tag_format_pattern: Optional[str]
+    tag_name_format_pattern: Optional[str]
+    tag_message_format_pattern: Optional[str]
     allowed_initial_branches: Optional[frozenset[str]]
 
 
 @dataclass
 class BumpByArgs:
     part_to_bump: BumpPart
     config_file: Optional[Path]  # absolute resolved path
@@ -43,9 +44,10 @@
     current_version: Optional[Version]
     commit: Optional[GitAction]
     branch: Optional[GitAction]
     tag: Optional[GitAction]
     remote: Optional[str]
     commit_format_pattern: Optional[str]
     branch_format_pattern: Optional[str]
-    tag_format_pattern: Optional[str]
+    tag_name_format_pattern: Optional[str]
+    tag_message_format_pattern: Optional[str]
     allowed_initial_branches: Optional[frozenset[str]]
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/core.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/config/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 DEFAULT_TAG_ACTION = GitAction.Skip
 
 DEFAULT_REMOTE = "origin"
 DEFAULT_COMMIT_FORMAT_PATTERN: str = (
     f"Bump version: {{{keys.CURRENT_VERSION}}} → {{{keys.NEW_VERSION}}}"
 )
 DEFAULT_BRANCH_FORMAT_PATTERN = f"bump_version_to_{{{keys.NEW_VERSION}}}"
-DEFAULT_TAG_FORMAT_PATTERN = f"v{{{keys.NEW_VERSION}}}"
+DEFAULT_TAG_NAME_FORMAT_PATTERN = f"v{{{keys.NEW_VERSION}}}"
+DEFAULT_TAG_MESSAGE_FORMAT_PATTERN: str = DEFAULT_COMMIT_FORMAT_PATTERN
 DEFAULT_SEARCH_PATTERN = f"{{{keys.VERSION}}}"
 DEFAULT_ALLOWED_INITIAL_BRANCHES = frozenset({"main", "master"})
 
 HYPER_CONFIG_FILE_NAME = "hyper-bump-it.toml"
 PYPROJECT_FILE_NAME = "pyproject.toml"
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/file.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/config/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import dataclasses
 from collections.abc import Sequence
 from pathlib import Path
-from typing import Optional, Union, cast
+from typing import Annotated, Optional, Union, cast
 
 import tomlkit
 from pydantic import (
     BaseModel,
+    ConfigDict,
     Field,
-    StrictBool,
-    StrictStr,
     ValidationError,
-    root_validator,
-    validator,
+    WrapValidator,
+    model_validator,
 )
+from pydantic_core.core_schema import ValidatorFunctionWrapHandler
 from tomlkit import TOMLDocument
 from tomlkit.exceptions import TOMLKitError
 
 from ..compat import TypeAlias
 from ..error import (
     ConfigurationFileNotFoundError,
     ConfigurationFileReadError,
@@ -30,106 +29,114 @@
     DEFAULT_BRANCH_ACTION,
     DEFAULT_BRANCH_FORMAT_PATTERN,
     DEFAULT_COMMIT_ACTION,
     DEFAULT_COMMIT_FORMAT_PATTERN,
     DEFAULT_REMOTE,
     DEFAULT_SEARCH_PATTERN,
     DEFAULT_TAG_ACTION,
-    DEFAULT_TAG_FORMAT_PATTERN,
+    DEFAULT_TAG_MESSAGE_FORMAT_PATTERN,
+    DEFAULT_TAG_NAME_FORMAT_PATTERN,
     HYPER_CONFIG_FILE_NAME,
     PYPROJECT_FILE_NAME,
     GitAction,
     validate_git_action_combination,
 )
 
 ROOT_TABLE_KEY = "hyper-bump-it"
 PYPROJECT_SUB_TABLE_KEYS = ("tool", ROOT_TABLE_KEY)
 
 
 class HyperBaseMode(BaseModel):
-    class Config:
-        extra = "forbid"
-        min_anystr_length = 1
-        allow_mutation = False
+    model_config = ConfigDict(
+        extra="forbid", str_min_length=1, frozen=True, strict=True
+    )
+
+
+def _check_action(
+    value: Optional[object], handler: ValidatorFunctionWrapHandler
+) -> GitAction:
+    if isinstance(value, str):
+        for action in GitAction:
+            if value == action.value:
+                return action
+        raise ValueError(f"value must be one of: {', '.join(GitAction)}")
+    return cast(GitAction, handler(value))
+
+
+PossiblyStrGitAction = Annotated[GitAction, WrapValidator(_check_action)]
 
 
 class GitActions(HyperBaseMode):
-    commit: GitAction = DEFAULT_COMMIT_ACTION
-    branch: GitAction = DEFAULT_BRANCH_ACTION
-    tag: GitAction = DEFAULT_TAG_ACTION
+    commit: PossiblyStrGitAction = DEFAULT_COMMIT_ACTION
+    branch: PossiblyStrGitAction = DEFAULT_BRANCH_ACTION
+    tag: PossiblyStrGitAction = DEFAULT_TAG_ACTION
 
-    @root_validator(skip_on_failure=True)
+    @model_validator(mode="after")
     def _check_git_actions(
-        cls,
-        values: dict[str, GitAction],
-    ) -> dict[str, GitAction]:
-        validate_git_action_combination(**values)
-        return values
+        self,
+    ) -> "GitActions":
+        validate_git_action_combination(
+            commit=self.commit, branch=self.branch, tag=self.tag
+        )
+        return self
 
 
 class Git(HyperBaseMode):
-    remote: StrictStr = DEFAULT_REMOTE
-    commit_format_pattern: StrictStr = DEFAULT_COMMIT_FORMAT_PATTERN
-    branch_format_pattern: StrictStr = DEFAULT_BRANCH_FORMAT_PATTERN
-    tag_format_pattern: StrictStr = DEFAULT_TAG_FORMAT_PATTERN
+    remote: str = DEFAULT_REMOTE
+    commit_format_pattern: str = DEFAULT_COMMIT_FORMAT_PATTERN
+    branch_format_pattern: str = DEFAULT_BRANCH_FORMAT_PATTERN
+    tag_name_format_pattern: str = DEFAULT_TAG_NAME_FORMAT_PATTERN
+    tag_message_format_pattern: str = DEFAULT_TAG_MESSAGE_FORMAT_PATTERN
     allowed_initial_branches: frozenset[str] = DEFAULT_ALLOWED_INITIAL_BRANCHES
     extend_allowed_initial_branches: frozenset[str] = frozenset()
     actions: GitActions = GitActions()
 
 
 class File(HyperBaseMode):
-    file_glob: StrictStr  # relative to project root directory
-    keystone: StrictBool = False
-    search_format_pattern: StrictStr = DEFAULT_SEARCH_PATTERN
-    replace_format_pattern: Optional[StrictStr] = None
+    file_glob: str  # relative to project root directory
+    keystone: bool = False
+    search_format_pattern: str = DEFAULT_SEARCH_PATTERN
+    replace_format_pattern: Optional[str] = None
+
+
+HyperConfigFileValues: TypeAlias = dict[str, Union[list[File], Optional[str], Git]]
 
 
-HyperConfigFileValues: TypeAlias = dict[
-    str, Union[list[File], Optional[StrictStr], Git]
-]
+def _check_version(
+    value: Optional[object], handler: ValidatorFunctionWrapHandler
+) -> Optional[Version]:
+    if isinstance(value, str):
+        return Version.parse(value)
+    return cast(Version, handler(value))
+
+
+OptionalVersion = Annotated[Optional[Version], WrapValidator(_check_version)]
 
 
 class ConfigFile(HyperBaseMode):
-    files: list[File] = Field(..., min_items=1)
-    current_version: Optional[Version] = None
-    show_confirm_prompt: StrictBool = True
+    files: list[File] = Field(..., min_length=1)
+    current_version: OptionalVersion = None
+    show_confirm_prompt: bool = True
     git: Git = Git()
 
-    @validator("current_version", pre=True)
-    def _check_version(cls, value: Optional[object]) -> Optional[Version]:
-        if value is None:
-            return None
-        if isinstance(value, Version):
-            return dataclasses.replace(value)
-        if isinstance(value, str):
-            return Version.parse(value)
-        raise TypeError(
-            "Value must be a version or a string that can be parsed into a version"
-        )
-
-    @root_validator(skip_on_failure=True)
-    def _check_keystone_files(
-        cls,
-        values: HyperConfigFileValues,
-    ) -> HyperConfigFileValues:
-        files = cast(list[File], values["files"])
-        keystone_file_count = sum(1 for file in files if file.keystone)
+    @model_validator(mode="after")
+    def _check_keystone_files(self) -> "ConfigFile":
+        keystone_file_count = sum(1 for file in self.files if file.keystone)
         if keystone_file_count > 1:
             raise ValueError("Only one file is allowed to be a keystone file")
-        current_version = values.get("current_version")
-        if current_version is None:
+        if self.current_version is None:
             if keystone_file_count == 0:
                 raise ValueError(
                     "current_version must be set if there is not a keystone file"
                 )
         elif keystone_file_count != 0:
             raise ValueError(
                 "Configuration can't specify the current_version while also having a keystone file"
             )
-        return values
+        return self
 
     @property
     def keystone_config(self) -> Optional[tuple[str, str]]:
         for file in self.files:
             if file.keystone:
                 return file.file_glob, file.search_format_pattern
         return None
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/config/keystone_parser.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/config/keystone_parser.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/core.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/core.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/error.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pydantic import ValidationError
 from rich.text import Text
 
 from . import ui
 
 if TYPE_CHECKING:
-    from pydantic.error_wrappers import ErrorDict
+    from pydantic_core import ErrorDetails
 
 
 class BumpItError(Exception):
     """Base for library errors"""
 
     def __rich__(self) -> Text:
         return Text(str(self))
@@ -361,16 +361,20 @@
     def __rich__(self) -> Text:
         return Text("No configuration file found in directory ").append(
             str(self.project_root), style="file.path"
         )
 
 
 class ConfigurationFileError(ConfigurationError):
-    def __init__(self, file: Path, message_suffix: str) -> None:
+    def __init__(
+        self, file: Path, message_suffix: Union[str, Callable[[], str]]
+    ) -> None:
         self.file = file
+        if not isinstance(message_suffix, str):
+            message_suffix = message_suffix()
         super().__init__(f"The configuration file ({self.file}) {message_suffix}")
 
     @property
     def _message_prefix(self) -> Text:
         return (
             Text("The configuration file (")
             .append(str(self.file), style="file.path")
@@ -401,54 +405,61 @@
             .append("'")
         )
 
 
 class InvalidConfigurationError(ConfigurationFileError):
     def __init__(self, file: Path, cause: ValidationError) -> None:
         self.cause = cause
-        super().__init__(file, f"is not valid: {self.cause}")
+        super().__init__(file, lambda: self._append_message_suffix(Text()).plain)
 
-    # Slightly customized variant of pydantic's __str__() to make it more end user-friendly
-    # and enhanced with rich styles.
     def __rich__(self) -> Text:
+        return self._append_message_suffix(self._message_prefix)
+
+    # Slightly customized variant of pydantic's ValidationError.__str__() to make it more end-user
+    # friendly and enhanced with rich styles.
+    def _append_message_suffix(self, initial_text: Text) -> Text:
         errors = self.cause.errors()
         num_errors = len(errors)
 
-        message = self._message_prefix.append("is not valid:\n")
+        message = initial_text.append("is not valid:\n")
         message.append(f"{num_errors} validation error")
         if num_errors != 1:
             message.append("s")
         message.append(" for ")
-        message.append(self.cause.model.__name__, style="emphasis")
+        message.append(self.cause.title, style="emphasis")
         message.append("\n")
-        message.append(InvalidConfigurationError.display_errors(errors))
+        message.append(InvalidConfigurationError._display_errors(errors))
         return message
 
     @staticmethod
-    def display_errors(errors: list["ErrorDict"]) -> Text:
+    def _display_errors(errors: list["ErrorDetails"]) -> Text:
         return Text("\n").join(
             InvalidConfigurationError._display_error_loc(e)
             .append("  ")
             .append(e["msg"], style="error.msg")
             for e in errors
         )
 
     @staticmethod
-    def _display_error_loc(error: "ErrorDict") -> Text:
-        if len(error["loc"]) == 1 and error["loc"][0] == "__root__":
+    def _display_error_loc(error: "ErrorDetails") -> Text:
+        if len(error["loc"]) == 0:
             return Text("")
         return (
-            Text(" -> ")
+            Text(".")
             .join(Text(str(e), style="error.loc") for e in error["loc"])
             .append("\n")
         )
 
 
 def first_error_message(ex: ValidationError) -> str:
-    return ex.errors()[0]["msg"]
+    first_error = ex.errors(include_context=True)[0]
+    if (ctx := first_error.get("ctx")) is not None:
+        if (ctx_error := ctx.get("error")) is not None:
+            return str(ctx_error)
+    return first_error["msg"]
 
 
 TValue = TypeVar("TValue")
 
 
 def _list_str_values(values: Collection[str]) -> str:
     return ", ".join(value for value in values)
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/execution_plan.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/execution_plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -181,24 +181,32 @@
     def display_intent(self) -> None:
         ui.display(
             Text("Commit changes: ").append(self._commit_message, style="vcs.commit")
         )
 
 
 class CreateTagAction:
-    def __init__(self, repo: Repo, tag_name: str) -> None:
+    def __init__(self, repo: Repo, tag_name: str, tag_message: str) -> None:
         self._repo = repo
         self._tag_name = tag_name
+        self._tag_message = tag_message
 
     def __call__(self) -> None:
-        ui.display(Text("Tagging commit: ").append(self._tag_name, style="vcs.tag"))
-        vcs.create_tag(self._repo, self._tag_name)
+        ui.display(self._action_description(Text("Tagging commit: ")))
+        vcs.create_tag(self._repo, self._tag_name, self._tag_message)
 
     def display_intent(self) -> None:
-        ui.display(Text("Tag commit: ").append(self._tag_name, style="vcs.tag"))
+        ui.display(self._action_description(Text("Tag commit: ")))
+
+    def _action_description(self, prefix: Text) -> Text:
+        return (
+            prefix.append(self._tag_name, style="vcs.tag")
+            .append(" - ")
+            .append(self._tag_message, style="vcs.tag")
+        )
 
 
 class PushChangesAction:
     def __init__(self, repo: Repo, operation_info: vcs.GitOperationsInfo) -> None:
         self._repo = repo
         self._operation_info = operation_info
 
@@ -238,14 +246,18 @@
         switch_back = SwitchBranchAction(repo, repo.active_branch.name)
 
     if git_operations_info.actions.commit.should_create:
         final_actions.append(
             CommitChangesAction(repo, git_operations_info.commit_message)
         )
     if git_operations_info.actions.tag.should_create:
-        final_actions.append(CreateTagAction(repo, git_operations_info.tag_name))
+        final_actions.append(
+            CreateTagAction(
+                repo, git_operations_info.tag_name, git_operations_info.tag_message
+            )
+        )
     if git_operations_info.actions.any_push:
         final_actions.append(PushChangesAction(repo, git_operations_info))
 
     if switch_back is not None:
         final_actions.append(switch_back)
     return initial_actions, final_actions
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/files.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/files.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/keys.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/format_pattern/keys.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/matching_pattern.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/format_pattern/matching_pattern.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/format_pattern/text_formatter.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/format_pattern/text_formatter.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/planned_changes.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/planned_changes.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/ui.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/ui.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/vcs.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/vcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 
 @dataclass
 class GitOperationsInfo:
     remote: str
     commit_message: str
     branch_name: str
     tag_name: str
+    tag_message: str
     allowed_initial_branches: frozenset[str]
     actions: GitActions
 
     @classmethod
     def from_config(cls, config: Git, formatter: TextFormatter) -> "GitOperationsInfo":
         """
         Convert the configuration into the necessary operation information.
@@ -38,15 +39,16 @@
         :return: Git operation information.
         :raises FormatError: Format pattern was invalid or attempted to use an invalid key.
         """
         return cls(
             remote=config.remote,
             commit_message=formatter.format(config.commit_format_pattern),
             branch_name=formatter.format(config.branch_format_pattern),
-            tag_name=formatter.format(config.tag_format_pattern),
+            tag_name=formatter.format(config.tag_name_format_pattern),
+            tag_message=formatter.format(config.tag_message_format_pattern),
             allowed_initial_branches=config.allowed_initial_branches,
             actions=config.actions,
         )
 
 
 def get_vetted_repo(project_root: Path, operation_info: GitOperationsInfo) -> Repo:
     """
@@ -116,22 +118,21 @@
 def commit_changes(repo: Repo, commit_message: str) -> None:
     index = repo.index
     for diff in index.diff(None):
         if diff.deleted_file:
             index.remove(diff.a_path)
         else:
             index.add(diff.a_path)
-    for file in repo.untracked_files:
-        index.add(file)
 
-    index.commit(commit_message)
+    index.write_tree()
+    repo.git.commit(message=commit_message)
 
 
-def create_tag(repo: Repo, tag_name: str) -> None:
-    repo.create_tag(tag_name)
+def create_tag(repo: Repo, tag_name: str, tag_message: str) -> None:
+    repo.create_tag(tag_name, message=tag_message)
 
 
 def push_changes(repo: Repo, operation_info: GitOperationsInfo) -> None:
     to_push = [
         operation_info.branch_name
         if operation_info.actions.branch == GitAction.CreateAndPush
         else repo.active_branch.name
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it/_hyper_bump_it/version.py` & `hyper-bump-it-0.5.0/hyper_bump_it/_hyper_bump_it/version.py`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it.egg-info/PKG-INFO` & `hyper-bump-it-0.5.0/hyper_bump_it.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyper-bump-it
-Version: 0.4.1
+Version: 0.5.0
 Summary: A version bumping tool
 Author-email: Patrick Lannigan <p.lannigan@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/plannigan/hyper-bump-it
 Project-URL: changelog, https://github.com/plannigan/hyper-bump-it/blob/main/CHANGELOG.md
 Project-URL: issues, https://github.com/plannigan/hyper-bump-it/issues
 Keywords: version,bump,command line
@@ -20,14 +20,15 @@
 
 [![CI pipeline status](https://github.com/plannigan/hyper-bump-it/actions/workflows/main.yml/badge.svg?branch=main)][ci]
 [![PyPI](https://img.shields.io/pypi/v/hyper-bump-it)][pypi]
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/hyper-bump-it)][pypi]
 [![codecov](https://codecov.io/gh/plannigan/hyper-bump-it/branch/main/graph/badge.svg?token=V4DADJU0BI)][codecov]
 [![Checked with mypy](https://img.shields.io/badge/mypy-checked-blue)][mypy-home]
 [![Code style: black](https://img.shields.io/badge/code%20style-black-black.svg)][black-home]
+[![OpenSSF Scorecard](https://api.securityscorecards.dev/projects/github.com/plannigan/hyper-bump-it/badge)][scorecard]
 
 # Hyper Bump It
 
 A command line tool for updating the version in project files needed for the next release.
 
 `hyper-bump-it`'s features include:
 
@@ -147,7 +148,8 @@
 ```
 
 [ci]: https://github.com/plannigan/hyper-bump-it/actions
 [pypi]: https://pypi.org/project/hyper-bump-it/
 [codecov]: https://codecov.io/gh/plannigan/hyper-bump-it
 [mypy-home]: http://mypy-lang.org/
 [black-home]: https://github.com/psf/black
+[scorecard]: https://securityscorecards.dev/viewer/?uri=github.com/plannigan/hyper-bump-it
```

### Comparing `hyper-bump-it-0.4.1/hyper_bump_it.egg-info/SOURCES.txt` & `hyper-bump-it-0.5.0/hyper_bump_it.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyper-bump-it-0.4.1/pyproject.toml` & `hyper-bump-it-0.5.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [project]
 name = "hyper-bump-it"
-version = "0.4.1"
+version = "0.5.0"
 description = "A version bumping tool"
 readme = "README.md"
 requires-python = ">=3.9,<4.0"
 license = {text = "MIT"}
 dependencies = [
     "GitPython>=3.1.29,<4",
     "tomlkit>=0.11.6,<1.0",
     "typer>=0.9.0,<1.0",
-    "pydantic>=1.10.2,<2",
+    "pydantic>=2.1.0,<3",
     "rich>=12.6.0,<14",
     "typing-extensions>=4.4.0,<5; python_version < '3.11'",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -53,21 +53,29 @@
 files = "hyper_bump_it"
 show_error_codes = true
 warn_unused_configs = true
 pretty = true
 strict = true
 disallow_any_explicit = true
 warn_unreachable = true
+plugins = [
+  "pydantic.mypy"
+]
 
 [[tool.mypy.overrides]]
 module = [
     "git.*",
 ]
 implicit_reexport = true
 
+[tool.pydantic-mypy]
+init_forbid_extra = true
+init_typed = true
+warn_required_dynamic_aliases = true
+
 # testing
 [tool.pytest.ini_options]
 addopts = "--verbose --cov=hyper_bump_it --cov-report xml:/tmp/coverage.xml --cov-report term-missing:skip-covered"
 testpaths = ["tests"]
 
 [tool.coverage.run]
 branch = true
```

