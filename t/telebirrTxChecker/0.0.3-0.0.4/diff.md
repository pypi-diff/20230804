# Comparing `tmp/telebirrTxChecker-0.0.3.tar.gz` & `tmp/telebirrTxChecker-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telebirrTxChecker-0.0.3.tar", last modified: Thu Aug  3 12:23:55 2023, max compression
+gzip compressed data, was "telebirrTxChecker-0.0.4.tar", last modified: Fri Aug  4 08:27:23 2023, max compression
```

## Comparing `telebirrTxChecker-0.0.3.tar` & `telebirrTxChecker-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:23:55.609854 telebirrTxChecker-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-03 12:23:55.609854 telebirrTxChecker-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 12:23:55.609854 telebirrTxChecker-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:23:55.605854 telebirrTxChecker-0.0.3/telebirrTxChecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-03 12:23:55.000000 telebirrTxChecker-0.0.3/telebirrTxChecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-03 12:23:55.000000 telebirrTxChecker-0.0.3/telebirrTxChecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 12:23:55.000000 telebirrTxChecker-0.0.3/telebirrTxChecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-03 12:23:55.000000 telebirrTxChecker-0.0.3/telebirrTxChecker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-03 12:23:55.000000 telebirrTxChecker-0.0.3/telebirrTxChecker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:23:55.605854 telebirrTxChecker-0.0.3/ttxc/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:23:55.605854 telebirrTxChecker-0.0.3/ttxc/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 12:23:55.609854 telebirrTxChecker-0.0.3/ttxc/types/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/types/payer.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/types/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/types/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-03 12:23:44.000000 telebirrTxChecker-0.0.3/ttxc/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-08-04 08:27:23.000000 telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-04 08:27:23.000000 telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 08:27:23.000000 telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 08:27:23.000000 telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 08:27:23.000000 telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/ttxc/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/ttxc/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 08:27:23.564737 telebirrTxChecker-0.0.4/ttxc/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/types/payer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/types/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/types/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-08-04 08:27:11.000000 telebirrTxChecker-0.0.4/ttxc/utils.py
```

### Comparing `telebirrTxChecker-0.0.3/PKG-INFO` & `telebirrTxChecker-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebirrTxChecker
-Version: 0.0.3
+Version: 0.0.4
 Summary: asynchronous telebirr transaction checker
 Home-page: https://github.com/wizkiye/TelebirrPaymentProcessor
 Author: Kidus
 Author-email: wizkiye@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `telebirrTxChecker-0.0.3/README.md` & `telebirrTxChecker-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `telebirrTxChecker-0.0.3/telebirrTxChecker.egg-info/PKG-INFO` & `telebirrTxChecker-0.0.4/telebirrTxChecker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: telebirrTxChecker
-Version: 0.0.3
+Version: 0.0.4
 Summary: asynchronous telebirr transaction checker
 Home-page: https://github.com/wizkiye/TelebirrPaymentProcessor
 Author: Kidus
 Author-email: wizkiye@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `telebirrTxChecker-0.0.3/ttxc/main.py` & `telebirrTxChecker-0.0.4/ttxc/main.py`

 * *Files identical despite different names*

### Comparing `telebirrTxChecker-0.0.3/ttxc/types/transaction.py` & `telebirrTxChecker-0.0.4/ttxc/types/transaction.py`

 * *Files identical despite different names*

### Comparing `telebirrTxChecker-0.0.3/ttxc/utils.py` & `telebirrTxChecker-0.0.4/ttxc/utils.py`

 * *Files identical despite different names*

