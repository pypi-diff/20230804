# Comparing `tmp/eikobot-0.5.1.tar.gz` & `tmp/eikobot-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eikobot-0.5.1.tar", last modified: Wed Jun  7 15:29:15 2023, max compression
+gzip compressed data, was "eikobot-0.6.0.tar", last modified: Thu Aug  3 22:43:31 2023, max compression
```

## Comparing `eikobot-0.5.1.tar` & `eikobot-0.6.0.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.464075 eikobot-0.5.1/
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1059 2023-06-05 11:53:10.000000 eikobot-0.5.1/LICENSE
--rw-r--r--   0 yaron     (1000) yaron     (1000)     3252 2023-06-07 15:29:15.464075 eikobot-0.5.1/PKG-INFO
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2644 2023-06-07 14:01:19.000000 eikobot-0.5.1/README.md
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.460075 eikobot-0.5.1/eikobot/
--rw-r--r--   0 yaron     (1000) yaron     (1000)      159 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     6055 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/__main__.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.460075 eikobot-0.5.1/eikobot/core/
--rw-r--r--   0 yaron     (1000) yaron     (1000)       39 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/__init__.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.460075 eikobot-0.5.1/eikobot/core/compiler/
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1263 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    85130 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/_parser.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1666 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/_token.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2420 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/decorator.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.464075 eikobot-0.5.1/eikobot/core/compiler/definitions/
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2786 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/_resource.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1593 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/base_model.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    35673 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/base_types.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    12465 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/context.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    12376 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/function.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2777 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/definitions/typedef.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     8553 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/importlib.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     9149 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/lexer.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      306 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/compiler/misc.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     8779 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/compiler/ops.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2828 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/deployer.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2893 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/errors.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     8016 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/exporter.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     4755 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/handlers.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      395 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/helpers.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.464075 eikobot-0.5.1/eikobot/core/lib/
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/__init__.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.464075 eikobot-0.5.1/eikobot/core/lib/std/
--rw-r--r--   0 yaron     (1000) yaron     (1000)      819 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/lib/std/__init__.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)    14244 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/lib/std/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/std/env.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1486 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/std/env.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      316 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/std/file.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)     6997 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/lib/std/file.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/std/regex.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)      325 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/std/regex.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)       50 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/lib/std/test.eiko
--rw-r--r--   0 yaron     (1000) yaron     (1000)      520 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/core/lib/std/test.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2248 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/logger.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.464075 eikobot-0.5.1/eikobot/core/package_manager/
--rw-r--r--   0 yaron     (1000) yaron     (1000)    10663 2023-06-07 15:28:36.000000 eikobot-0.5.1/eikobot/core/package_manager/__init__.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      803 2023-06-05 11:53:10.000000 eikobot-0.5.1/eikobot/core/plugin.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-06-07 14:01:19.000000 eikobot-0.5.1/eikobot/py.typed
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.460075 eikobot-0.5.1/eikobot.egg-info/
--rw-r--r--   0 yaron     (1000) yaron     (1000)     3252 2023-06-07 15:29:15.000000 eikobot-0.5.1/eikobot.egg-info/PKG-INFO
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1663 2023-06-07 15:29:15.000000 eikobot-0.5.1/eikobot.egg-info/SOURCES.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)        1 2023-06-07 15:29:15.000000 eikobot-0.5.1/eikobot.egg-info/dependency_links.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)       49 2023-06-07 15:29:15.000000 eikobot-0.5.1/eikobot.egg-info/entry_points.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)      108 2023-06-07 15:29:15.000000 eikobot-0.5.1/eikobot.egg-info/requires.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)        8 2023-06-07 15:29:15.000000 eikobot-0.5.1/eikobot.egg-info/top_level.txt
--rw-r--r--   0 yaron     (1000) yaron     (1000)     4076 2023-06-07 15:29:15.464075 eikobot-0.5.1/setup.cfg
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1401 2023-06-07 15:24:36.000000 eikobot-0.5.1/setup.py
-drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-06-07 15:29:15.464075 eikobot-0.5.1/tests/
--rw-r--r--   0 yaron     (1000) yaron     (1000)     8976 2023-06-07 14:01:19.000000 eikobot-0.5.1/tests/test_compilation.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2792 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_datatypes.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      750 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_decorator.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     5979 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_deployer.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     1350 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_exporter.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     2353 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_import.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)    16877 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_lexer.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      921 2023-06-07 14:01:19.000000 eikobot-0.5.1/tests/test_package.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)     9776 2023-06-07 14:01:19.000000 eikobot-0.5.1/tests/test_parser.py
--rw-r--r--   0 yaron     (1000) yaron     (1000)      409 2023-06-05 11:53:10.000000 eikobot-0.5.1/tests/test_promises.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:43:31.020184 eikobot-0.6.0/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1059 2023-08-03 22:09:03.000000 eikobot-0.6.0/LICENSE
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2262 2023-08-03 22:43:31.020184 eikobot-0.6.0/PKG-INFO
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1654 2023-08-03 22:37:24.000000 eikobot-0.6.0/README.md
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:43:31.016184 eikobot-0.6.0/eikobot/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      159 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     6065 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/__main__.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:43:31.016184 eikobot-0.6.0/eikobot/core/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1039 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/__init__.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:43:31.020184 eikobot-0.6.0/eikobot/core/compiler/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1263 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/compiler/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    92611 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/compiler/_parser.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1747 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/compiler/_token.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2420 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/compiler/decorator.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:43:31.020184 eikobot-0.6.0/eikobot/core/compiler/definitions/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/compiler/definitions/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2848 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/compiler/definitions/_resource.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1593 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/compiler/definitions/base_model.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    39137 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/compiler/definitions/base_types.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    12818 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/compiler/definitions/context.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    14114 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/compiler/definitions/function.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2782 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/compiler/definitions/typedef.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     8545 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/compiler/importlib.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     9570 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/compiler/lexer.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      306 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/compiler/misc.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     8825 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/compiler/ops.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2828 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/deployer.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2893 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/errors.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     8039 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/exporter.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     5413 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/handlers.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      519 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/helpers.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:43:31.020184 eikobot-0.6.0/eikobot/core/lib/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/lib/__init__.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:43:31.020184 eikobot-0.6.0/eikobot/core/lib/std/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      868 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/lib/std/__init__.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    21891 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/lib/std/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/lib/std/env.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1486 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/lib/std/env.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      316 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/lib/std/file.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     8265 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/lib/std/file.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/lib/std/regex.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      325 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/lib/std/regex.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)       50 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/lib/std/test.eiko
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      520 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/lib/std/test.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2248 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/core/logger.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:43:31.020184 eikobot-0.6.0/eikobot/core/package_manager/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    10659 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/package_manager/__init__.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1384 2023-08-03 22:37:24.000000 eikobot-0.6.0/eikobot/core/plugin.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:09:03.000000 eikobot-0.6.0/eikobot/py.typed
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:43:31.016184 eikobot-0.6.0/eikobot.egg-info/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2262 2023-08-03 22:43:31.000000 eikobot-0.6.0/eikobot.egg-info/PKG-INFO
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1663 2023-08-03 22:43:31.000000 eikobot-0.6.0/eikobot.egg-info/SOURCES.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        1 2023-08-03 22:43:31.000000 eikobot-0.6.0/eikobot.egg-info/dependency_links.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)       49 2023-08-03 22:43:31.000000 eikobot-0.6.0/eikobot.egg-info/entry_points.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      108 2023-08-03 22:43:31.000000 eikobot-0.6.0/eikobot.egg-info/requires.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)        8 2023-08-03 22:43:31.000000 eikobot-0.6.0/eikobot.egg-info/top_level.txt
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     4082 2023-08-03 22:43:31.020184 eikobot-0.6.0/setup.cfg
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1401 2023-08-03 22:37:24.000000 eikobot-0.6.0/setup.py
+drwxr-xr-x   0 yaron     (1000) yaron     (1000)        0 2023-08-03 22:43:31.020184 eikobot-0.6.0/tests/
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    10617 2023-08-03 22:37:24.000000 eikobot-0.6.0/tests/test_compilation.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2792 2023-08-03 22:09:03.000000 eikobot-0.6.0/tests/test_datatypes.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      750 2023-08-03 22:09:03.000000 eikobot-0.6.0/tests/test_decorator.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     5979 2023-08-03 22:09:03.000000 eikobot-0.6.0/tests/test_deployer.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     1350 2023-08-03 22:09:03.000000 eikobot-0.6.0/tests/test_exporter.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     2353 2023-08-03 22:09:03.000000 eikobot-0.6.0/tests/test_import.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)    17333 2023-08-03 22:37:24.000000 eikobot-0.6.0/tests/test_lexer.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      921 2023-08-03 22:09:03.000000 eikobot-0.6.0/tests/test_package.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)     9776 2023-08-03 22:09:03.000000 eikobot-0.6.0/tests/test_parser.py
+-rw-r--r--   0 yaron     (1000) yaron     (1000)      409 2023-08-03 22:09:03.000000 eikobot-0.6.0/tests/test_promises.py
```

### Comparing `eikobot-0.5.1/LICENSE` & `eikobot-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/PKG-INFO` & `eikobot-0.6.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eikobot
-Version: 0.5.1
+Version: 0.6.0
 Summary: The eikobot desired state engine.
 Author: kazaamjt
 Author-email: kazaamjt@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -66,36 +66,7 @@
 
 Or by activating the venv first:
 
 ```bash
 . eikobot-venv/bin/activate
 eikobot
 ```
-
-## Linters, type checkers, testing, etc
-
-Currently this project uses:
-
-- `mypy` for advanced type checking
-- `isort` to auto format the imports
-- `black` to auto format code
-- `flake8` to do basic linting (and pointing out where isort and black would make changes)
-- `pylint` for advanced linting and code smell detection
-- `bandit` to scan for security issues
-
-Note that the `flake8-isort` and `flake8-black` plugins are used,
-and Flake8 will emit `isort` and `black` issues but not auto format them,
-these tools will still need to be ran afterwards to fix any errors.  
-The `Flake8-pylint` and `Flake8-mypy` plugins are not used as they are in broken state.  
-
-For vscode, adding the following settings to your config is recommended:
-
-```json
-{
-    "python.linting.flake8Enabled": true,
-    "python.linting.mypyEnabled": true,
-    "python.linting.pylintEnabled": true,
-    "python.testing.pytestEnabled": true,
-    "python.testing.pytestArgs": [],
-    "editor.insertSpaces": true,
-}
-```
```

### Comparing `eikobot-0.5.1/README.md` & `eikobot-0.6.0/eikobot.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: eikobot
+Version: 0.6.0
+Summary: The eikobot desired state engine.
+Author: kazaamjt
+Author-email: kazaamjt@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: System :: Systems Administration
+Classifier: Topic :: Utilities
+Classifier: Intended Audience :: System Administrators
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Requires-Python: >=3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Eikobot Desired State Engine
 
 *The little Desired State Engine that made it so.*  
 
 Eikobot is a desired state orchestrator.  
 The basic idea is that you describe your infrastructure and eikobot
 will make it happen.  
@@ -47,36 +66,7 @@
 
 Or by activating the venv first:
 
 ```bash
 . eikobot-venv/bin/activate
 eikobot
 ```
-
-## Linters, type checkers, testing, etc
-
-Currently this project uses:
-
-- `mypy` for advanced type checking
-- `isort` to auto format the imports
-- `black` to auto format code
-- `flake8` to do basic linting (and pointing out where isort and black would make changes)
-- `pylint` for advanced linting and code smell detection
-- `bandit` to scan for security issues
-
-Note that the `flake8-isort` and `flake8-black` plugins are used,
-and Flake8 will emit `isort` and `black` issues but not auto format them,
-these tools will still need to be ran afterwards to fix any errors.  
-The `Flake8-pylint` and `Flake8-mypy` plugins are not used as they are in broken state.  
-
-For vscode, adding the following settings to your config is recommended:
-
-```json
-{
-    "python.linting.flake8Enabled": true,
-    "python.linting.mypyEnabled": true,
-    "python.linting.pylintEnabled": true,
-    "python.testing.pytestEnabled": true,
-    "python.testing.pytestArgs": [],
-    "editor.insertSpaces": true,
-}
-```
```

### Comparing `eikobot-0.5.1/eikobot/__main__.py` & `eikobot-0.6.0/eikobot/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         print(compiler.context)
 
     pc_time_taken = time.process_time() - pc_start
     time_taken = time.time() - start
     pc_time_taken_formatted = str(datetime.timedelta(seconds=pc_time_taken))
     time_taken_formatted = str(datetime.timedelta(seconds=time_taken))
     logger.info(
-        f"Compiled in {time_taken_formatted} "
+        f"Compiled in {time_taken_formatted} 🤖 "
         f"(Process time: {pc_time_taken_formatted})"
     )
 
     return compiler
 
 
 @cli.command()
@@ -158,15 +158,15 @@
             logger.error(
                 "Failed to deploy model. "
                 f"({deployer.progress.done} out of {deployer.progress.total} tasks done)"
             )
         else:
             time_taken = time.time() - start
             time_taken_formatted = str(datetime.timedelta(seconds=time_taken))
-            logger.info(f"Deployed in {time_taken_formatted}")
+            logger.info(f"Deployed in {time_taken_formatted} 🤖")
 
 
 @cli.group()
 def package() -> None:
     pass
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `eikobot-0.5.1/eikobot/core/compiler/__init__.py` & `eikobot-0.6.0/eikobot/core/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/eikobot/core/compiler/_parser.py` & `eikobot-0.6.0/eikobot/core/compiler/_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -457,44 +457,95 @@
                 index=self.token.index,
             )
         self.identifier = self.token.content
 
     def assign(
         self,
         value: StorableTypes,
-        assign_context: Union[CompilerContext, EikoResource],
+        assign_context: CompilerContext | EikoResource,
         compile_context: CompilerContext,
         token: Token,
     ) -> StorableTypes:
         """Assigns the variable a value."""
+        type_expr: EikoType | None = None
+        prev_def: EikoBaseType | EikoUnset | None = None
+        if isinstance(assign_context, EikoResource):
+            prev_def = assign_context.properties.get(self.identifier)
+
+        elif isinstance(assign_context, CompilerContext):
+            _prev_def = assign_context.shallow_get(self.identifier)
+            if isinstance(_prev_def, (EikoBaseType, EikoUnset)):
+                prev_def = _prev_def
+
         if self.type_expr is not None:
             type_expr = self.type_expr.compile(compile_context)
             if type_expr.inverse_type_check(value.type):
                 type_constr = compile_context.get(type_expr.name)
                 if isinstance(type_constr, EikoTypeDef):
                     if isinstance(value, EikoBaseType):
                         value = type_constr.execute(value, token)
                     else:
                         raise EikoInternalError(
                             "Something went wrong trying to coerce a type to it's typedef.",
                             token=token,
                         )
-            if not type_expr.type_check(value.type):
+
+            if prev_def is not None and not prev_def.type.type_check(type_expr):
                 raise EikoCompilationError(
-                    "Variable assigned incompatible type:"
-                    f" given value of type '{value.type}' but expected type '{type_expr}'",
-                    token=token,
+                    "Reassinging types is not allowed.",
+                    token=self.token,
                 )
 
-            if isinstance(value, EikoList) and isinstance(type_expr, EikoListType):
+        elif prev_def is not None:
+            type_expr = prev_def.type
+
+        if type_expr is not None:
+            if (
+                isinstance(value, EikoList)
+                and value.type.element_type.name == ""
+                and isinstance(type_expr, EikoListType)
+            ):
                 value.update_typing(type_expr)
 
-            if isinstance(value, EikoDict) and isinstance(type_expr, EikoDictType):
+            elif (
+                isinstance(value, EikoDict)
+                and value.type.key_type.name == ""
+                and value.type.value_type.name == ""
+                and isinstance(type_expr, EikoDictType)
+            ):
                 value.update_typing(type_expr)
 
+            elif not value.type.type_check(type_expr):
+                if value.type.inverse_type_check(type_expr):
+                    if type_expr.typedef is None:
+                        raise EikoCompilationError(
+                            "A coercion failed. Type is not a TypeDef.",
+                            token=token,
+                        )
+                    if isinstance(value, EikoBaseType):
+                        value = type_expr.typedef.execute(value, token)
+                    else:
+                        raise EikoInternalError(
+                            "A coercion failed due to a bug. Please report this on Github.",
+                            token=token,
+                        )
+                else:
+                    raise EikoCompilationError(
+                        "Variable assigned incompatible type:"
+                        f" given value of type '{value.type}' but expected type '{type_expr}'",
+                        token=token,
+                    )
+
+            else:
+                if isinstance(value, EikoList) and isinstance(type_expr, EikoListType):
+                    value.update_typing(type_expr)
+
+                if isinstance(value, EikoDict) and isinstance(type_expr, EikoDictType):
+                    value.update_typing(type_expr)
+
         elif isinstance(value, EikoList) and len(value.elements) == 0:
             raise EikoCompilationError(
                 "A list must be given a type expressing or initial values.",
                 token=self.token,
             )
 
         elif isinstance(value, EikoDict) and len(value.elements) == 0:
@@ -676,16 +727,16 @@
     def compile(self, context: CompilerContext) -> Optional[EikoBaseType]:
         eiko_callable = self.identifier_expr.compile(context)
 
         if isinstance(eiko_callable, EikoResourceDefinition):
             eiko_callable = eiko_callable.default_constructor
 
         args: list[PassedArg] = []
+        keyword_args: dict[str, PassedArg] = {}
         if isinstance(eiko_callable, ConstructorDefinition):
-            keyword_args: dict[str, PassedArg] = {}
             kw_args = False
             for arg_expr in self.args.elements:
                 if isinstance(arg_expr, AssignmentExprAST):
                     kw_args = True
                     if not isinstance(arg_expr.lhs, VariableExprAST):
                         raise EikoCompilationError(
                             "Expected an identifier on the left hand side of keyword argument.",
@@ -740,24 +791,41 @@
 
             raise EikoInternalError(
                 "Not sure what happened here. This is probably a bug",
                 token=self.token,
             )
 
         if isinstance(eiko_callable, EikoBuiltinFunction):
+            parsing_kw = False
             for arg_expr in self.args.elements:
-                arg_value = arg_expr.compile(context)
-                if not isinstance(arg_value, EikoBaseType):
-                    raise EikoCompilationError(
-                        "The provided argument did not provide a valid value.",
-                        token=arg_expr.token,
-                    )
-                args.append(PassedArg(arg_expr.token, arg_value))
+                if isinstance(arg_expr, AssignmentExprAST):
+                    parsing_kw = True
+                    arg_value = arg_expr.rhs.compile(context)
+                    if not isinstance(arg_value, EikoBaseType):
+                        raise EikoCompilationError(
+                            "The provided argument is not a valid value.",
+                            token=arg_expr.token,
+                        )
+                    kw_arg = PassedArg(arg_expr.lhs.token, arg_value)
+                    keyword_args[kw_arg.token.content] = kw_arg
+                else:
+                    if parsing_kw:
+                        raise EikoCompilationError(
+                            "A positional argument cannot follow a keyword argument.",
+                            token=arg_expr.token,
+                        )
+                    arg_value = arg_expr.compile(context)
+                    if not isinstance(arg_value, EikoBaseType):
+                        raise EikoCompilationError(
+                            "The provided argument is not a valid value.",
+                            token=arg_expr.token,
+                        )
+                    args.append(PassedArg(arg_expr.token, arg_value))
 
-            return eiko_callable.execute(self.token, args)
+            return eiko_callable.execute(self.token, args, keyword_args)
 
         if isinstance(eiko_callable, EikoEnumDefinition):
             if len(self.args.elements) != 1:
                 raise EikoCompilationError(
                     f"Enum '{eiko_callable.name}' takes exactly 1 argument.",
                     token=self.token,
                 )
@@ -955,31 +1023,53 @@
         default_value = self.expr.rhs.compile(context)
         if not isinstance(default_value, EikoBaseType):
             raise EikoCompilationError(
                 f"{res_name}.{self.name} did not get a valid default value.",
                 token=self.expr.rhs.token,
             )
 
+        lhs_type_expr: TypeExprAST | None = None
+        if isinstance(default_value, EikoList):
+            if default_value.type.name == "list[]":
+                if isinstance(_type, EikoListType):
+                    lhs_type_expr = self.expr.lhs.type_expr
+                    default_value.type = _type
+                else:
+                    raise EikoInternalError(
+                        "Something went wrong initializing a list as default argument."
+                    )
+
+        elif isinstance(default_value, EikoDict):
+            if default_value.type.name == "dict[]":
+                if isinstance(_type, EikoDictType):
+                    lhs_type_expr = self.expr.lhs.type_expr
+                    default_value.type = _type
+                else:
+                    raise EikoInternalError(
+                        "Something went wrong initializing a list as default argument."
+                    )
+
         if not _type.type_check(default_value.type):
             if _type.inverse_type_check(default_value.type):
                 if _type.typedef is None:
                     raise EikoInternalError(
                         "Something went wrong trying to coerce a type to it's typedef.",
                         token=self.expr.token,
                     )
                 default_value = _type.typedef.execute(
                     default_value,
                     self.expr.rhs.token,
                 )
             else:
                 raise EikoCompilationError(
                     f"The default value of {res_name}.{self.name} does not fit type described in its type expression.",
+                    token=self.expr.rhs.token,
                 )
 
-        return ResourceProperty(self.name, _type, default_value)
+        return ResourceProperty(self.name, _type, default_value, lhs_type_expr)
 
 
 @dataclass
 class DecoratorExprAST(ExprAST):
     """A decorator, used to decorate resource definitions."""
 
     identifier: VariableExprAST
@@ -1028,15 +1118,15 @@
 class ResourceDefinitionAST(ExprAST):
     """
     A resource definition represents the resources properties and constructors.
     """
 
     name: str
     decorators: list[DecoratorExprAST]
-    super_expr: Optional[VariableExprAST]
+    super_expr: DotExprAST | VariableExprAST | None
 
     def __post_init__(self) -> None:
         self.constructor: Optional["ConstructorExprAST"] = None
         self.type = EikoType(self.name, EikoObjectType)
         self.properties: dict[str, ResourcePropertyAST] = {}
         self.promises: list[PromiseExprAST] = []
 
@@ -1046,22 +1136,22 @@
     def add_promise(self, promise: PromiseExprAST) -> None:
         self.promises.append(promise)
 
     # pylint: disable = too-many-locals
     def compile(self, context: CompilerContext) -> EikoResourceDefinition:
         super_res: Optional[EikoResourceDefinition] = None
         if self.super_expr is not None:
-            compiled_super_expr = self.super_expr.compile(context)
-            if not isinstance(compiled_super_expr, EikoResourceDefinition):
+            _super_res = self.super_expr.compile(context)
+            if not isinstance(_super_res, EikoResourceDefinition):
                 raise EikoCompilationError(
                     "Expected a resource definition to inherit from.",
                     token=self.super_expr.token,
                 )
 
-            super_res = compiled_super_expr
+            super_res = _super_res
             self.type.super = super_res.instance_type
             new_prop_dict: dict[str, ResourcePropertyAST] = {}
             for super_property_ast in super_res.expr.properties.values():
                 new_prop = self.properties.get(super_property_ast.name)
                 if new_prop is not None:
                     new_type = new_prop.compile_type(context)
                     prev_type = super_property_ast.compile_type(context)
@@ -1071,14 +1161,24 @@
                             f"in super type '{super_res.name}'.",
                             token=new_prop.token,
                         )
                 new_prop_dict[super_property_ast.name] = super_property_ast
             new_prop_dict.update(self.properties)
             self.properties = new_prop_dict
 
+            for super_promise in super_res.expr.promises:
+                for promise in self.promises:
+                    if super_promise.var.identifier == promise.var.identifier:
+                        raise EikoCompilationError(
+                            f"Promise '{super_promise.var.identifier}' already defined "
+                            f"in super type '{super_res.name}'.",
+                            token=promise.token,
+                        )
+                self.promises.append(super_promise)
+
         arg_properties: dict[str, ResourceProperty] = {}
         for property_ast in self.properties.values():
             prop = property_ast.compile(context, self.name)
             _prop = arg_properties.get(prop.name)
             if _prop is not None:
                 raise EikoCompilationError(
                     f"Property '{prop.name}' was already defined in class '{self.name}'.",
@@ -1100,15 +1200,15 @@
                     AssignmentExprAST(
                         self.token,
                         DotExprAST(
                             Token(TokenType.DOT, ".", token.index),
                             VariableExprAST(
                                 Token(TokenType.IDENTIFIER, "self", token.index)
                             ),
-                            VariableExprAST(token),
+                            VariableExprAST(token, prop.type_expr),
                         ),
                         VariableExprAST(token),
                     ),
                 )
         else:
             default_constructor = self.constructor.compile(context)
 
@@ -1561,15 +1661,15 @@
 
 @dataclass
 class EnumValueExprAst(ExprAST):
     """Represents a value tied to an enum class."""
 
     def __post_init__(self) -> None:
         super().__post_init__()
-        self.value = self.token.content.lower()
+        self.value = self.token.content
 
     def compile(self, context: CompilerContext) -> Optional[StorableTypes]:
         raise NotImplementedError(self.token)
 
 
 @dataclass
 class EnumExprAst(ExprAST):
@@ -1584,14 +1684,39 @@
             values[value.value] = EikoEnumValue(value_type, value.value)
 
         definition = EikoEnumDefinition(self.token.content, value_type, values)
         context.set(definition.name, definition)
         return definition
 
 
+@dataclass
+class ForExprAst(ExprAST):
+    """Represents a for loop that loops over an iterable."""
+
+    loop_var_expr: VariableExprAST
+    iterable_expr: ExprAST
+    body: list[ExprAST]
+
+    def compile(self, context: CompilerContext) -> None:
+        compiled_iterable = self.iterable_expr.compile(context)
+        if not isinstance(compiled_iterable, EikoBaseType):
+            raise EikoCompilationError(
+                "Expression is not iterable, but FOR requires an iterable.",
+                token=self.iterable_expr.token,
+            )
+
+        for obj in compiled_iterable.iterate(self.iterable_expr.token):
+            sub_context = context.get_subcontext(f"{context.name}-for")
+            self.loop_var_expr.assign(
+                obj, sub_context, context, self.loop_var_expr.token
+            )
+            for line in self.body:
+                line.compile(sub_context)
+
+
 class Parser:
     """
     Parses tokens 1 by 1, and turns them in to Expressions.
     """
 
     def __init__(self, file: Path) -> None:
         self.lexer = Lexer(file)
@@ -1617,14 +1742,15 @@
             "//": 70,
             "%": 70,
             "u-": 80,
             "**": 90,
             ".": 100,
             "(": 100,
             "[": 100,
+            ":": 100,
         }
 
     def parse(self) -> Iterator[ExprAST]:
         """Parses tokens and constructs the next set of ASTs."""
         expr = self._parse_top_level()
         while not isinstance(expr, EOFExprAST):
             yield expr
@@ -1760,14 +1886,17 @@
 
         if self._current.type == TokenType.AT_SIGN:
             return self._parse_decorator([])
 
         if self._current.type == TokenType.ENUM:
             return self._parse_enum()
 
+        if self._current.type == TokenType.FOR:
+            return self._parse_for()
+
         raise EikoSyntaxError(
             f"Unexpected token {self._current.type.name}.", index=self._current.index
         )
 
     def _parse_unary_op(self) -> Union[UnaryNegExprAST, UnaryNotExprAST]:
         token = self._current
         self._advance()
@@ -1812,14 +1941,21 @@
             bin_op_token = self._current
             if self._current.type not in [
                 TokenType.LEFT_PAREN,
                 TokenType.LEFT_SQ_BRACKET,
             ]:
                 self._advance()
             rhs = self._parse_primary()
+            if (
+                isinstance(rhs, VariableExprAST)
+                and self._current.type == TokenType.COLON
+                and self._next.type == TokenType.IDENTIFIER
+            ):
+                self._advance()
+                rhs = VariableExprAST(rhs.token, self._parse_type())
 
             # if current op binds less tightly with rhs than the operator after rhs,
             # let the pending operator take rhs as it's lhs
             next_op_precedence = self._bin_op_precedence.get(self._current.content, 0)
             if expr_precedence < next_op_precedence:
                 rhs = self._parse_bin_op_rhs(current_predecedence + 0.0001, rhs)
 
@@ -1973,32 +2109,41 @@
             )
 
         identifier_token = self._next
         self._advance()
         self._advance()
 
         # Inheritance
-        super_expr: Optional[VariableExprAST] = None
+        super_expr: VariableExprAST | DotExprAST | None = None
         if self._current.type == TokenType.LEFT_PAREN:
             self._advance()
             super_expr = self._parse_identifier()
+            while True:
+                if self._current.type != TokenType.DOT:
+                    break
+
+                self._advance()
+                super_expr = DotExprAST(
+                    self._previous, super_expr, self._parse_identifier()
+                )
+
             if self._current.type != TokenType.RIGHT_PAREN:
                 raise EikoParserError(
                     f"Unexpected token {self._current.content}. Expected ')'.",
                     token=self._current,
                 )
             self._advance()
 
         rd_ast = ResourceDefinitionAST(
             identifier_token, identifier_token.content, decorators, super_expr
         )
 
         if self._current.type != TokenType.COLON:
             raise EikoParserError(
-                f"Unexpected token {self._current.content}.",
+                f"Unexpected token {self._current.content}. Expected a ':'.",
                 token=self._current,
             )
         self._advance()
 
         while self._next.type == TokenType.INDENT:
             self._advance()
 
@@ -2009,14 +2154,20 @@
                     token=self._previous,
                 )
             raise EikoParserError(
                 f"Unexpected token {self._current.content}, "
                 "expected indented code block.",
                 token=self._current,
             )
+
+        if self._next.type == TokenType.TRIPLE_DOT:
+            self._advance()
+            self._advance()
+            return rd_ast
+
         indent = self._current.content
         constructor: Optional[ConstructorExprAST] = None
         while True:
             while self._next.type == TokenType.INDENT:
                 self._advance()
             if self._current.content != indent:
                 break
@@ -2029,19 +2180,19 @@
                 rd_ast.add_property(self._parse_resource_property())
             elif self._current.type == TokenType.PROMISE:
                 rd_ast.add_promise(self._parse_promise())
             elif self._current.type == TokenType.INDENT:
                 pass
             else:
                 raise EikoSyntaxError(
-                    f"Unexpected token in resource definition '{rd_ast.name}'",
-                    index=rd_ast.token.index,
+                    f"Unexpected token '{self._current.content}' in resource definition '{rd_ast.name}'",
+                    index=self._current.index,
                 )
 
-        if not rd_ast.properties:
+        if not rd_ast.properties and rd_ast.super_expr is None:
             raise EikoSyntaxError(
                 "A resource must have atleast 1 property. (Besides promises.)",
                 index=rd_ast.token.index,
             )
         rd_ast.constructor = constructor
 
         return rd_ast
@@ -2085,14 +2236,20 @@
                 self._advance()
                 break
             if self._current.type != TokenType.COMMA:
                 raise EikoSyntaxError(
                     "Expected a ',' or a ')'.", index=self._current.index
                 )
             self._advance(skip_indentation=True)
+            if (
+                self._current.type == TokenType.RIGHT_PAREN
+                and self._next.type == TokenType.COLON
+            ):
+                self._advance()
+                break
             args.append(self._parse_consructor_arg())
             if self._current.type == TokenType.INDENT:
                 self._advance(skip_indentation=True)
 
         if self._current.type != TokenType.COLON:
             raise EikoSyntaxError("Expected a ':'.", index=self._current.index)
         self._advance()
@@ -2272,15 +2429,16 @@
         body: list[ExprAST] = []
         while True:
             body.append(self._parse_expression())
             while self._next.type == TokenType.INDENT:
                 self._advance()
             if self._current.type != TokenType.INDENT:
                 raise EikoInternalError(
-                    "Unexpected issue, please report this on github."
+                    "Unexpected issue, please report this on github.",
+                    token=self._current,
                 )
             if self._current.content != self._current_indent:
                 break
             self._advance()
 
         self._current_indent = prev_indent
         return body
@@ -2424,7 +2582,36 @@
                     "Unexpected issue, please report this on github."
                 )
             if self._current.content != indent:
                 break
             self._advance()
 
         return EnumExprAst(identifier_token, values)
+
+    def _parse_for(self) -> ForExprAst:
+        token = self._current
+        self._advance()
+
+        if self._current.type != TokenType.IDENTIFIER:
+            raise EikoParserError(
+                f"Unexpected token {self._next.content}, " "expected an identifier.",
+                token=self._next,
+            )
+
+        loop_var_expr = self._parse_identifier()
+        if self._current.type != TokenType.IN:
+            raise EikoParserError(
+                f"Unexpected token {self._next.content}, " "expected an 'in' token.",
+                token=self._next,
+            )
+        self._advance()
+        iterable_expr = self._parse_expression()
+
+        if self._current.type != TokenType.COLON:
+            raise EikoParserError(
+                f"Unexpected token {self._next.content}, " "expected a ':'.",
+                token=self._next,
+            )
+        self._advance()
+
+        body = self._parse_body()
+        return ForExprAst(token, loop_var_expr, iterable_expr, body)
```

### Comparing `eikobot-0.5.1/eikobot/core/compiler/_token.py` & `eikobot-0.6.0/eikobot/core/compiler/_token.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,26 +22,30 @@
     ELIF = auto()
     ELSE = auto()
     AND = auto()
     OR = auto()
     DEF = auto()
     PROMISE = auto()
     ENUM = auto()
+    FOR = auto()
+    IN = auto()
 
     IDENTIFIER = auto()
 
     LEFT_PAREN = auto()
     RIGHT_PAREN = auto()
     LEFT_SQ_BRACKET = auto()
     RIGHT_SQ_BRACKET = auto()
     LEFT_BRACE = auto()
     RIGHT_BRACE = auto()
     COLON = auto()
     COMMA = auto()
     DOT = auto()
+    DOUBLE_DOT = auto()
+    TRIPLE_DOT = auto()
     AT_SIGN = auto()
 
     DOUBLE_COLON = auto()
     ASSIGNMENT_OP = auto()
     ARITHMETIC_OP = auto()
     COMPARISON_OP = auto()
```

### Comparing `eikobot-0.5.1/eikobot/core/compiler/decorator.py` & `eikobot-0.6.0/eikobot/core/compiler/decorator.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/eikobot/core/compiler/definitions/_resource.py` & `eikobot-0.6.0/eikobot/core/compiler/definitions/_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Resource and ResourceProperty class definitions.
 Resource is the base building block of the eiko language model.
 """
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Optional, Union
 
-from ...handlers import Handler
 from .base_types import EikoBaseType, EikoPromise, EikoResource, EikoType
 
 if TYPE_CHECKING:
-    from .._parser import ResourceDefinitionAST
+    from ...handlers import Handler
+    from .._parser import ResourceDefinitionAST, TypeExprAST
     from .._token import Token
     from .base_model import EikoBaseModel
     from .function import ConstructorDefinition
 
 
 @dataclass
 class ResourceProperty:
@@ -21,14 +21,15 @@
     Internal representation of a resource property for constructors.
     It does not verify wether the default value given is the correct type.
     """
 
     name: str
     type: EikoType
     default_value: Optional[EikoBaseType] = None
+    type_expr: "TypeExprAST | None" = None
 
 
 @dataclass
 class EikoPromiseDefinition:
     """
     Internal representation of a promise constructor.
     """
@@ -64,15 +65,15 @@
         self.name = expr.name
         self.instance_type: EikoType = expr.type
         self.default_constructor = default_constructor
         self.default_constructor.parent = self
         self.properties: PropertiesDict = properties
         self.index_def = [list(properties.keys())[0]]
         self.promises: list[EikoPromiseDefinition] = promises
-        self.handler: Optional[type[Handler]] = None
+        self.handler: Optional[type["Handler"]] = None
         self.linked_basemodel: Optional[type["EikoBaseModel"]] = None
 
     def printable(self, indent: str = "") -> str:
         return_str = f"{indent}Resource Definition '{self.name}'"
         if self.type.super is not None:
             return_str += f"('{self.type.super.name}')"
         return_str += ": " + "{\n"
```

### Comparing `eikobot-0.5.1/eikobot/core/compiler/definitions/base_model.py` & `eikobot-0.6.0/eikobot/core/compiler/definitions/base_model.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/eikobot/core/compiler/definitions/base_types.py` & `eikobot-0.6.0/eikobot/core/compiler/definitions/base_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,47 +57,58 @@
     def convert(cls, _: "BuiltinTypes") -> "EikoBaseType":
         raise ValueError
 
     def type_check(self, expected_type: "EikoType") -> bool:
         """
         Recursivly type checks.
 
-        NOTE: in most cases it should be value.type(expected_type)
+        NOTE: in most cases it should be value.type.type_check(expected_type)
         and not the other way around.
         """
+        if self == eiko_any_type:
+            return True
+
         if self.name == expected_type.name:
             return True
 
-        if expected_type.super is not None:
-            return self.type_check(expected_type.super)
+        if self.super is not None:
+            return self.super.type_check(expected_type)
+
+        if isinstance(expected_type, EikoUnion):
+            for expected_sub_type in expected_type.types:
+                if self.type_check(expected_sub_type):
+                    return True
+
+        if isinstance(expected_type, EikoOptional):
+            return self.type_check(expected_type.optional_type)
 
         return False
 
     def inverse_type_check(self, expected_type: "EikoType") -> bool:
         """Checks if a given type is the same or a super type of this type."""
         if self.name == expected_type.name:
             return True
 
-        if self.super is not None:
-            return self.super.inverse_type_check(expected_type)
+        if expected_type.super is not None:
+            return self.inverse_type_check(expected_type.super)
 
         return False
 
     def get_top_level_type(self) -> "EikoType":
         """Returns the toplevel super type."""
         if self.super is None:
             return self
 
         return self.super
 
     def __repr__(self) -> str:
         return self.name
 
     def __str__(self) -> str:
-        return self.name
+        return self.__repr__()
 
 
 @dataclass
 class EikoUnset:
     """
     Special type, allowing for forward declarations.
     """
@@ -112,20 +123,24 @@
     def printable(_: str) -> str:
         return "Unset"
 
     def to_py(self) -> None:
         return None
 
 
+eiko_any_type = EikoType("Any")
 EikoType.type = EikoType("Type")
 EikoObjectType = EikoType("Object")
 
 
 def type_list_to_type(types: list[EikoType]) -> EikoType:
     """Turns a list of Eiko types in to a single usable type."""
+    if len(types) == 0:
+        return EikoType("")
+
     if len(types) == 1:
         _type = types[0]
     else:
         union_name = "Union["
         for sub_type in types:
             union_name += sub_type.name + ","
         _type = EikoUnion(union_name[:-1] + "]", types)
@@ -144,16 +159,16 @@
         self.types = types
         super().__init__(name)
 
     def type_check(self, expected_type: EikoType) -> bool:
         """Recursivly type checks."""
 
         if isinstance(expected_type, EikoUnion):
-            for _type in expected_type.types:
-                if not self.type_check(_type):
+            for _type in self.types:
+                if not expected_type.type_check(_type):
                     return False
             return True
 
         for _type in self.types:
             if _type.type_check(expected_type):
                 return True
 
@@ -189,23 +204,26 @@
 
     def printable(self, indent: str = "") -> str:
         raise NotImplementedError
 
     def truthiness(self) -> bool:
         raise NotImplementedError
 
-    def type_check(self, expected_type: EikoType) -> bool:
-        return expected_type.type_check(self.type)
-
     def index(self) -> str:
         raise NotImplementedError
 
     def to_py(self) -> Union[PyTypes, "EikoPromise"]:
         raise NotImplementedError
 
+    def iterate(self, token: Token) -> Iterator["EikoBaseType"]:
+        raise EikoCompilationError(
+            f"Object of type '{self.type}' is not iterable.",
+            token=token,
+        )
+
 
 EikoNoneType = EikoType("None")
 
 
 class EikoOptional(EikoType):
     """Eiko optional means a value can be None."""
 
@@ -488,15 +506,15 @@
         Set this promise's value.
         This method will make sure the type is correct
 
         Raises ValueError if value is not the right type
         or if the promis was already assigned a different value.
         """
         _value = to_eiko(value)
-        if not _value.type_check(self.type):
+        if not _value.type.type_check(self.type):
             raise ValueError
 
         if self.value is not None and _value.get_value() != self.value.get_value():
             ctx.error(
                 f"Promise '{self.name}' already has a value and new value is different."
             )
             raise ValueError
@@ -510,15 +528,15 @@
         """
         if self.value is not None:
             raise EikoCompilationError(
                 "Tried to assign an already assigned promise.",
                 token=token,
             )
 
-        if not value.type_check(self.type):
+        if not value.type.type_check(self.type):
             raise EikoCompilationError(
                 f"Tried to assign promise a value of type '{self.type.name}' "
                 f"but got a value of type '{value.type.name}'.",
                 token=token,
             )
 
         self.value = value
@@ -534,17 +552,14 @@
             raise EikoCompilationError(
                 "An unfulfilled Promise cannot be checked for truthiness, "
                 "as its value does not yet exist."
             )
 
         return self.value.truthiness()
 
-    def type_check(self, expected_type: EikoType) -> bool:
-        return expected_type.type_check(self.type)
-
     def index(self) -> str:
         return f"promise-{self.parent.index()}.{self.name}"
 
     def to_py(self) -> "EikoPromise[T]":
         return self
 
     def resolve(self, expect: Type[T]) -> T:
@@ -711,15 +726,15 @@
                 f"Property '{name}' of class '{self.type}' "
                 f"cannot be assigned a value of type '{value.type}'.",
                 token=token,
             )
 
         prop = self.properties.get(name)
         if isinstance(prop, EikoUnset):
-            if not value.type_check(prop.type):
+            if not value.type.type_check(prop.type):
                 if prop.type.inverse_type_check(value.type):
                     if prop.type.typedef is not None:
                         value = prop.type.typedef.execute(value, token)
                     else:
                         raise EikoInternalError(
                             "Ran in to a typedef that does not have a constructor. "
                             "This is most likely a bug. PLease report this on Github.",
@@ -822,24 +837,30 @@
     EikoEnumValue,
 )
 _builtin_function_type = EikoType("builtin_function", EikoObjectType)
 
 
 @dataclass
 class PassedArg:
-    """A passed arg is a compiled expression passed as an arg."""
+    """
+    A passed arg is a compiled expression passed as an arg.
+    This is an Arg meant to be passed to an EikoBuiltinFunction.
+    """
 
     token: Token
     value: EikoBaseType
 
 
 @dataclass
 class BuiltinFunctionArg:
+    """An arg passed to a builtin function."""
+
     name: str
     type: EikoType
+    default_value: EikoBaseType | None = None
 
 
 class EikoBuiltinFunction(EikoBaseType):
     """
     Built in functions are typically convenience functions.
     They cannot be user generated.
     """
@@ -848,38 +869,74 @@
         self,
         identifier: str,
         args: list[BuiltinFunctionArg],
         body: Callable[..., Optional[EikoBaseType]],
     ) -> None:
         super().__init__(_builtin_function_type)
         self.identifier = identifier
-        self.args = args
         self.body = body
 
+        self.args: list[BuiltinFunctionArg] = []
+        self.kw_args: dict[str, BuiltinFunctionArg] = {}
+        for arg in args:
+            if arg.default_value is None:
+                self.args.append(arg)
+            else:
+                self.kw_args[arg.name] = arg
+
     def execute(
-        self, callee_token: Token, args: list[PassedArg]
+        self,
+        callee_token: Token,
+        args: list[PassedArg],
+        keyword_args: dict[str, PassedArg] | None = None,
     ) -> Optional[EikoBaseType]:
         """Execute the builtin function."""
-        if len(args) != len(self.args):
+        if len(args) > len(self.args) + len(self.kw_args):
             raise EikoCompilationError(
                 "Too many arguments given to function call.",
                 token=callee_token,
             )
 
+        if len(args) < len(self.args):
+            raise EikoCompilationError(
+                "Missing positional arguments for function call.",
+                token=callee_token,
+            )
+
         validated_args: list[EikoBaseType] = []
         for passed_arg, expected_arg in zip(args, self.args):
             if not expected_arg.type.type_check(passed_arg.value.type):
                 raise EikoCompilationError(
                     f"Argument '{expected_arg.name}' must be of type '{expected_arg.type}', "
-                    f"but got '{passed_arg.value.type}'",
+                    f"but got '{passed_arg.value.type}' instead.",
                     token=passed_arg.token,
                 )
             validated_args.append(passed_arg.value)
 
-        return self.body(*validated_args)
+        validated_kw_args: dict[str, EikoBaseType] = {}
+        if keyword_args is not None:
+            for arg_name, passed_arg in keyword_args.items():
+                expected_kw_arg = self.kw_args.get(arg_name)
+
+                if expected_kw_arg is None:
+                    raise EikoCompilationError(
+                        f"Callable no such argument: '{arg_name}'.",
+                        token=passed_arg.token,
+                    )
+
+                if not expected_kw_arg.type.type_check(passed_arg.value.type):
+                    raise EikoCompilationError(
+                        f"Argument '{expected_kw_arg.name}' must be of type '{expected_kw_arg.type}', "
+                        f"but got '{passed_arg.value.type}' instead.",
+                        token=passed_arg.token,
+                    )
+
+                validated_kw_args[arg_name] = passed_arg.value
+
+        return self.body(*validated_args, **validated_kw_args)
 
     def truthiness(self) -> bool:
         raise NotImplementedError
 
 
 class EikoListType(EikoType):
     """Represents an Eiko list type, which is a container of types."""
@@ -888,15 +945,15 @@
         super().__init__(f"list[{element_type.name}]")
         self.element_type = element_type
 
     def type_check(self, expected_type: "EikoType") -> bool:
         if isinstance(expected_type, EikoListType):
             return self.element_type.type_check(expected_type.element_type)
 
-        return False
+        return super().type_check(expected_type)
 
 
 class EikoList(EikoBaseType):
     """Represents a list of objects in the Eiko language."""
 
     type: EikoListType
 
@@ -977,14 +1034,18 @@
 
     def index(self) -> str:
         raise NotImplementedError
 
     def to_py(self) -> list[Union[PyTypes, "EikoPromise"]]:
         return [element.to_py() for element in self.elements]
 
+    def iterate(self, _: Token) -> Iterator["EikoBaseType"]:
+        for element in self.elements:
+            yield element
+
 
 class EikoDictType(EikoType):
     """Represents an Eiko Union type, which combines 2 or more types."""
 
     def __init__(self, key_type: EikoType, value_type: EikoType) -> None:
         super().__init__(f"dict[{key_type.name}, {value_type.name}]")
         self.key_type = key_type
@@ -993,15 +1054,15 @@
     def type_check(self, expected_type: "EikoType") -> bool:
         if isinstance(expected_type, EikoDictType):
             if self.key_type.type_check(
                 expected_type.key_type
             ) and self.value_type.type_check(expected_type.value_type):
                 return True
 
-        return False
+        return super().type_check(expected_type)
 
 
 EikoIndexTypes = Union[
     bool,
     float,
     int,
     None,
@@ -1025,14 +1086,39 @@
         super().__init__(EikoDictType(key_type, value_type))
         self.elements: dict[Union[EikoBaseType, bool, float, int, str], EikoBaseType]
         if elements is None:
             self.elements = {}
         else:
             self.elements = elements
 
+        self.get_func = EikoBuiltinFunction(
+            "get",
+            [
+                BuiltinFunctionArg("key", key_type),
+                BuiltinFunctionArg("default_value", eiko_any_type, eiko_none_object),
+            ],
+            body=self._get,
+        )
+
+        self.values_func = EikoBuiltinFunction(
+            "values",
+            [],
+            body=self._values,
+        )
+
+    def _get(
+        self,
+        key: Union[EikoBaseType, bool, float, int, str],
+        default_value: EikoBaseType = eiko_none_object,
+    ) -> EikoBaseType:
+        return self.elements.get(key, default_value)
+
+    def _values(self) -> EikoList:
+        return EikoList(self.type.value_type, list(self.elements.values()))
+
     def update_typing(self, new_type: EikoDictType) -> None:
         self.type = new_type
 
     def insert(
         self,
         key: EikoBaseType,
         value: EikoBaseType,
@@ -1162,25 +1248,38 @@
             return key
 
         raise EikoCompilationError(
             f"Object of type '{key.type.name}' can not be for keys in dictionairies.",
             token=key_token,
         )
 
+    def iterate(self, _: Token) -> Iterator["EikoBaseType"]:
+        for element in self.elements:
+            yield to_eiko(element)
+
+    def get(self, name: str, token: Optional[Token] = None) -> "EikoBaseType":
+        if name == "values":
+            return self.values_func
+
+        if name == "get":
+            return self.get_func
+
+        return super().get(name, token)
+
 
 # Move to another file
-def to_eiko_type(cls: Optional[Type]) -> Type[EikoBaseType]:
+def to_eiko_type(cls: Optional[Type]) -> Type[EikoBaseType] | Type[EikoType]:
     """
     Takes a python type and returns it's eikobot compatible type.
     If said type exists.
     """
     if cls is None:
         return EikoNone
 
-    if issubclass(cls, EikoBaseType):
+    if issubclass(cls, EikoBaseType) or issubclass(cls, EikoType):
         return cls
 
     if cls == bool:
         return EikoBool
 
     if cls == float:
         return EikoFloat
@@ -1245,14 +1344,14 @@
         return EikoDict(
             type_list_to_type(key_types), type_list_to_type(value_types), d_elements
         )
 
     if isinstance(value, EikoBaseType):
         return value
 
-    if isinstance(value, BaseModel):
+    if isinstance(value, BaseModel) and hasattr(value, "raw_resource"):
         return value.raw_resource  # type: ignore
 
     if value is None:
         return eiko_none_object
 
     raise ValueError
```

### Comparing `eikobot-0.5.1/eikobot/core/compiler/definitions/context.py` & `eikobot-0.6.0/eikobot/core/compiler/definitions/context.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING, Optional, Type, Union
 
 from ... import logger
 from ...errors import EikoCompilationError, EikoInternalError
 from ...handlers import Handler
+from ...plugin import eiko_type, human_readable, machine_readable
 from .._token import Token
 from ..decorator import index_decorator
-from ..importlib import import_python_code
+from ..importlib import _load_plugin, import_python_code
 from ._resource import EikoResourceDefinition
 from .base_model import EikoBaseModel
 from .base_types import (
     BuiltinTypes,
     EikoBaseType,
     EikoBool,
     EikoDictType,
@@ -46,14 +47,17 @@
     "Path": EikoPath,
     "None": eiko_none_object,
     "Union": EikoUnion,
     "Optional": EikoOptional,
     "list": EikoListType,
     "dict": EikoDictType,
     "index": index_decorator,
+    "type": _load_plugin("", "type", eiko_type),
+    "human_readable": _load_plugin("", "human_readable", human_readable),
+    "machine_readable": _load_plugin("", "machine_readable", machine_readable),
 }
 
 
 @dataclass
 class LazyLoadModule:
     """A lazyLoadModule is meant to only be compiled when it is directly called."""
 
@@ -139,16 +143,16 @@
                 return_str += value.__repr__(extra_indent)
             elif isinstance(value, LazyLoadModule):
                 pass
             elif isinstance(value, EikoResourceDefinition):
                 return_str += value.printable(extra_indent)
             elif isinstance(value, EikoBaseType):
                 extra_extra_indent = extra_indent + "    "
-                return_str += f"{extra_indent}var '{key}':\n"
-                return_str += extra_extra_indent + value.printable(extra_extra_indent)
+                return_str += f"{extra_indent}var '{key}': "
+                return_str += value.printable(extra_extra_indent)
                 return_str += "\n"
             else:
                 return_str += f"{extra_indent}{key}: {value}\n"
 
         return_str += indent + "}\n"
         return return_str
 
@@ -196,15 +200,18 @@
         name: str,
         value: Union[_StorableTypes, "CompilerContext", EikoUnset],
         token: Optional[Token] = None,
     ) -> None:
         """Set a value. Throws an error if it's already set."""
         prev_value = self.shallow_get(name)
         if isinstance(prev_value, EikoUnset):
-            if prev_value.type.inverse_type_check(value.type):
+            if (
+                prev_value.type.inverse_type_check(value.type)
+                and prev_value.type.name != value.type.name
+            ):
                 constr = self.get(prev_value.type.name)
                 if isinstance(constr, EikoTypeDef):
                     if isinstance(value, EikoBaseType):
                         value = constr.execute(value, token)
                     else:
                         raise EikoInternalError(
                             "Something went wrong trying to coerce a type to it's typedef.",
```

### Comparing `eikobot-0.5.1/eikobot/core/compiler/definitions/function.py` & `eikobot-0.6.0/eikobot/core/compiler/definitions/function.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 """
 While real functions don't exist in the eiko language,
 constructors and plugins do, and they need some kind of representation.
 """
+import inspect
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Optional, Type, Union
+from pathlib import Path
+from types import UnionType
+from typing import (
+    TYPE_CHECKING,
+    Dict,
+    List,
+    Optional,
+    Type,
+    Union,
+    get_args,
+    get_origin,
+)
 
 from ...errors import EikoCompilationError, EikoInternalError, EikoPluginError
 from ...plugin import EikoPluginException, EikoPluginTyping
 from .._token import Token
 from .base_types import (
     INDEXABLE_TYPES,
     EikoBaseType,
@@ -67,15 +79,15 @@
     ) -> EikoResource:
         """
         Executes a function call based on a premade constructor spec.
         """
         if self.parent.promises and self.parent.handler is None:
             raise EikoCompilationError(
                 f"Resource Definition '{self.parent.name}' has promises, "
-                "but no handler",
+                "but no handler.",
                 token=self.parent.expr.token,
             )
 
         if len(positional_args) + len(keyword_args) > len(self.args) - 1:
             raise EikoCompilationError(
                 "Too many arguments given to function call. "
                 f"Expected {len(self.args) - 1}, "
@@ -169,17 +181,17 @@
     def _handle_args(  # pylint: disable=too-many-branches
         self,
         handled_args: dict[str, EikoBaseType],
         positional_args: list[PassedArg],
         keyword_args: dict[str, PassedArg],
     ) -> None:
         for passed_arg, arg in zip(positional_args, list(self.args.values())[1:]):
-            if not passed_arg.value.type_check(arg.type):
+            if not passed_arg.value.type.type_check(arg.type):
                 # Try to coerce the type
-                if arg.type.inverse_type_check(passed_arg.value.type):
+                if passed_arg.value.type.inverse_type_check(arg.type):
                     if arg.type.typedef is None:
                         raise EikoInternalError(
                             "Failed to coerce type.",
                             token=passed_arg.token,
                         )
                     passed_arg.value = arg.type.typedef.execute(
                         passed_arg.value, passed_arg.token
@@ -203,15 +215,15 @@
             kw_arg = self.args.get(arg_name)
             if kw_arg is None:
                 raise EikoCompilationError(
                     f"'{self.parent.name}.{self.name}()' has no argument '{arg_name}'.",
                     token=passed_arg.token,
                 )
 
-            if not passed_arg.value.type_check(kw_arg.type):
+            if not passed_arg.value.type.type_check(kw_arg.type):
                 if kw_arg.type.inverse_type_check(passed_arg.value.type):
                     if kw_arg.type.typedef is not None:
                         passed_arg.value = kw_arg.type.typedef.execute(
                             passed_arg.value,
                             passed_arg.token,
                         )
                     else:
@@ -299,37 +311,84 @@
                 python_exception=e,
             ) from e
 
         return to_eiko(val)
 
     def _handle_arg(
         self, arg: "ExprAST", context: "CompilerContext", required_arg: PluginArg
-    ) -> Union[EikoBaseType, bool, float, int, str]:
+    ) -> "StorableTypes | PyTypes":
         compiled_arg = arg.compile(context)
         if compiled_arg is None:
             raise EikoCompilationError(
                 f"Plugin '{self.module}.{self.identifier}' arg '{required_arg.name}' expects a value "
                 f"but expression did not result in a suitable value.",
                 token=arg.token,
             )
-        if issubclass(required_arg.py_type, EikoBaseType):
-            converted_arg: Union["StorableTypes", PyTypes] = compiled_arg
-        else:
+
+        converted_arg: "StorableTypes | PyTypes"
+        if required_arg.py_type in [None, bool, float, int, str, dict, list, Path]:
             if isinstance(compiled_arg, EikoBaseType):
-                converted_arg = compiled_arg.to_py()
+                try:
+                    converted_arg = compiled_arg.to_py()
+                except NotImplementedError:
+                    converted_arg = compiled_arg
             else:
+                converted_arg = compiled_arg
+
+            if not isinstance(converted_arg, required_arg.py_type):
                 raise EikoCompilationError(
-                    "Failed to convert to python type when passing to plugin.",
+                    f"Plugin '{self.module}.{self.identifier}' arg '{required_arg.name}' expects an argument "
+                    f"of type '{required_arg.py_type.__name__}', but instead got '{compiled_arg.type}'.",
                     token=arg.token,
                 )
 
-        if not isinstance(converted_arg, required_arg.py_type):
-            raise EikoCompilationError(
-                f"Plugin '{self.module}.{self.identifier}' arg '{required_arg.name}' expects an argument "
-                f"of type '{required_arg.py_type.__name__}', but instead got '{compiled_arg.type}'.",
-                token=arg.token,
+            return converted_arg
+
+        converted_arg = compiled_arg
+
+        if self._type_check(converted_arg, required_arg.py_type):
+            return converted_arg
+
+        raise EikoCompilationError(
+            f"Plugin '{self.module}.{self.identifier}' arg '{required_arg.name}' expects an argument "
+            f"of type '{required_arg.py_type}', but instead got '{compiled_arg.type}'.",
+            token=arg.token,
+        )
+
+    def _type_check(self, arg: "StorableTypes | PyTypes", expected: Type) -> bool:
+        try:
+            return isinstance(arg, expected)
+        except TypeError:
+            pass
+
+        origin = get_origin(expected)
+        if origin in (Union, UnionType):
+            for arg_type in get_args(expected):
+                if self._type_check(arg, arg_type):
+                    return True
+            return False
+
+        if origin is (list, List):
+            # if not isinstance(arg, list):
+            #     return False
+            #  args = get_args(expected)
+            raise EikoInternalError(
+                "Something went horribly wrong during a python runtime type check."
             )
 
-        return converted_arg  # type: ignore
+        if origin in (dict, Dict):
+            raise EikoInternalError(
+                "Something went horribly wrong during a python runtime type check."
+            )
+
+        if origin in (type, Type):
+            for arg_type in get_args(expected):
+                if inspect.isclass(arg) and issubclass(arg, arg_type):
+                    return True
+            return False
+
+        raise EikoInternalError(
+            "Something went horribly wrong during a python runtime type check."
+        )
 
     def truthiness(self) -> bool:
         raise NotImplementedError
```

### Comparing `eikobot-0.5.1/eikobot/core/compiler/definitions/typedef.py` & `eikobot-0.6.0/eikobot/core/compiler/definitions/typedef.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     def truthiness(self) -> bool:
         raise NotImplementedError
 
     def execute(self, arg: EikoBaseType, arg_token: Optional[Token]) -> BuiltinTypes:
         """
         Cast a value to a type and make sure it fits the given condition expression.
         """
-        if arg.type_check(self.type):
+        if arg.type.type_check(self.type):
             raise EikoCompilationError(
                 f"Type '{self.name}' requires '{self.type.name}' but was passed '{arg.type.name}'.",
                 token=arg_token,
             )
 
         if isinstance(self.super, EikoType):
             base_constructor = self.context.get(self.super.name)
```

### Comparing `eikobot-0.5.1/eikobot/core/compiler/importlib.py` & `eikobot-0.6.0/eikobot/core/compiler/importlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 The importlib allows for importing
 of both Eiko and Python code.
 """
 import importlib.util
 from dataclasses import dataclass
 from inspect import getfullargspec, getmembers, isclass, isfunction
 from pathlib import Path
-from types import FunctionType, ModuleType
-from typing import TYPE_CHECKING, Optional
+from types import ModuleType
+from typing import TYPE_CHECKING, Callable, Optional
 
 from .. import logger
 from ..errors import EikoCompilationError
 from ..handlers import CRUDHandler, Handler
 from ._token import Token
 from .definitions.base_model import EikoBaseModel
 from .definitions.function import PluginArg, PluginDefinition
@@ -205,15 +205,15 @@
         py_module = importlib.util.module_from_spec(spec)
         spec.loader.exec_module(py_module)  # type: ignore
         return py_module
 
     raise EikoCompilationError(f"Failed to import python module {module_name} ")
 
 
-def _load_plugin(module: str, name: str, function: FunctionType) -> PluginDefinition:
+def _load_plugin(module: str, name: str, function: Callable) -> PluginDefinition:
     fullargspec = getfullargspec(function)
     annotations = fullargspec.annotations
     return_type = annotations.get("return", "")
     if return_type == "":
         raise EikoCompilationError(
             f"Plugin {module}.{name} return type annotation is missing."
         )
```

### Comparing `eikobot-0.5.1/eikobot/core/compiler/lexer.py` & `eikobot-0.6.0/eikobot/core/compiler/lexer.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,25 +22,26 @@
     "else": TokenType.ELSE,
     "from": TokenType.FROM,
     "and": TokenType.AND,
     "or": TokenType.OR,
     "def": TokenType.DEF,
     "promise": TokenType.PROMISE,
     "enum": TokenType.ENUM,
+    "for": TokenType.FOR,
+    "in": TokenType.IN,
 }
 
 SPECIAL_CHARS = {
     "(": TokenType.LEFT_PAREN,
     ")": TokenType.RIGHT_PAREN,
     "[": TokenType.LEFT_SQ_BRACKET,
     "]": TokenType.RIGHT_SQ_BRACKET,
     "{": TokenType.LEFT_BRACE,
     "}": TokenType.RIGHT_BRACE,
     ",": TokenType.COMMA,
-    ".": TokenType.DOT,
     "@": TokenType.AT_SIGN,
 }
 
 
 class Lexer:
     """The lexer parses a given input and creates a set of tokens from said input."""
 
@@ -192,17 +193,21 @@
             self._next()
             if self._current == "\n":
                 raise EikoSyntaxError(
                     "EOL while scanning string literal", index=self._current_index()
                 )
 
         self._next()
-        escaped_string = bytes(_string, encoding="utf-8").decode(
-            encoding="unicode_escape"
-        )
+        try:
+            escaped_string = bytes(_string, encoding="utf-8").decode(
+                encoding="unicode_escape"
+            )
+        except UnicodeDecodeError as e:
+            raise EikoSyntaxError(str(e), index=index) from e
+
         return Token(TokenType.STRING, escaped_string, index)
 
     def _scan_raw_string(self, index: Index) -> Token:
         _string = ""
         delimiter = self._current
         self._next()
         while self._current != delimiter:
@@ -210,32 +215,39 @@
             self._next()
             if self._current == "\n":
                 raise EikoSyntaxError(
                     "EOL while scanning string literal", index=self._current_index()
                 )
 
         self._next()
-        raw_string = bytes(_string, encoding="utf-8").decode(
-            encoding="raw_unicode_escape"
-        )
-        return Token(TokenType.STRING, raw_string, index)
+        return Token(TokenType.STRING, _string, index)
 
     def _scan_f_string(self, index: Index) -> Token:
         string_token = self._scan_string()
         string_token.index = index
         string_token.type = TokenType.F_STRING
         return string_token
 
     def _scan_other(self) -> Token:  # pylint: disable=too-many-return-statements
         index = self._current_index()
         if self._current in SPECIAL_CHARS:
             special_char = self._current
             self._next()
             return Token(SPECIAL_CHARS[special_char], special_char, index)
 
+        if self._current == ".":
+            self._next()
+            if self._current == ".":
+                self._next()
+                if self._current == ".":
+                    self._next()
+                    return Token(TokenType.TRIPLE_DOT, "...", index)
+                return Token(TokenType.DOUBLE_DOT, "..", index)
+            return Token(TokenType.DOT, ".", index)
+
         if self._current == "=":
             self._next()
             if self._current == "=":
                 self._next()
                 return Token(TokenType.COMPARISON_OP, "==", index)
             return Token(TokenType.ASSIGNMENT_OP, "=", index)
```

### Comparing `eikobot-0.5.1/eikobot/core/compiler/ops.py` & `eikobot-0.6.0/eikobot/core/compiler/ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,14 +273,17 @@
         "It shouldn't be possible for this bug to happen, yet here we are."
     )
 
 
 def _eq_compare(
     a: EikoBaseType, b: EikoBaseType, op: ComparisonOP, b_token: Token
 ) -> EikoBool:
+    if a is b:
+        return EikoBool(True)
+
     if isinstance(a, (EikoInt, EikoFloat)) and isinstance(b, (EikoInt, EikoFloat)):
         return EikoBool(a.value == b.value)
 
     if not a.type == b.type:
         return EikoBool(False)
 
     if isinstance(a, EikoStr) and isinstance(b, EikoStr):
```

### Comparing `eikobot-0.5.1/eikobot/core/deployer.py` & `eikobot-0.6.0/eikobot/core/deployer.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/eikobot/core/errors.py` & `eikobot-0.6.0/eikobot/core/errors.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/eikobot/core/exporter.py` & `eikobot-0.6.0/eikobot/core/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,17 +195,18 @@
             return pre_task
 
         handler = None
         if resource.class_ref.handler is not None:
             handler = resource.class_ref.handler()
             self.total_tasks += 1
 
+        _id = resource.index()
         task = Task(
-            resource.index(),
-            HandlerContext(resource),
+            _id,
+            HandlerContext(resource, _id),
             handler,
         )
 
         for value in resource.properties.values():
             if isinstance(value, EikoResource):
                 task.process_sub_task(self._parse_task(value))
             elif isinstance(value, (EikoList, EikoDict)):
```

### Comparing `eikobot-0.5.1/eikobot/core/handlers.py` & `eikobot-0.6.0/eikobot/core/handlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,52 @@
 """
 Handlers are a way to describe to Eikobot how something should be deployed.
 """
 from dataclasses import dataclass
+from pathlib import Path
 from typing import Any, Union
 
 from . import logger
 from .compiler.definitions.base_model import BaseModel
 from .compiler.definitions.base_types import EikoResource
 from .errors import EikoUnresolvedPromiseError
 
+CACHE_DIR = Path(".eikobot_cache")
+CACHE_DIR.mkdir(exist_ok=True)
+
 
 @dataclass
 class HandlerContext:
     """A HandlerContext keeps track of things required for a deployment."""
 
     raw_resource: EikoResource
+    task_id: str
 
     def __post_init__(self) -> None:
         self.resource: Union[dict, BaseModel]
         self.changes: dict[str, Any] = {}
         self.deployed = False
         self.updated = False
         self.failed = False
         self.promises = self.raw_resource.promises
         self.name = self.raw_resource.index()
+        self.extras: dict[str, Any] = {}
+        self.task_cache = CACHE_DIR / self.normalized_task_id()
+
+        self.task_cache.mkdir(exist_ok=True)
+
+    def normalized_task_id(self) -> str:
+        """
+        Removes backslashes, forward slashes and : from the task_id
+        so it can be used for paths on both unix and windows.
+        """
+        _normalized = self.task_id.replace("\\", "-")
+        _normalized = _normalized.replace("/", "-")
+        _normalized = _normalized.replace(" ", "")
+        return _normalized.replace(":", ".")
 
     def add_change(self, key: str, value: Any) -> None:
         self.changes[key] = value
 
     def debug(self, msg: str) -> None:
         logger.debug(msg, pre=f"[{self.name}] ")
```

### Comparing `eikobot-0.5.1/eikobot/core/lib/std/__init__.eiko` & `eikobot-0.6.0/eikobot/core/lib/std/__init__.eiko`

 * *Files 25% similar despite different names*

```diff
@@ -18,20 +18,26 @@
 
 @index(["host.host", "cmd"])
 resource Cmd:
     host: Host
     cmd: str
 
 
+enum Shell:
+    powershell
+    bash
+    sh
+
+
 @index(["host.host", "_hash"])
 resource Script:
     host: Host
     script: str
-    exec_shell: Optional[str]
+    exec_shell: Optional[Shell]
 
     _hash: str
 
-    def __init__(self, host: Host, script: str, exec_shell: Optional[str] = None):
+    def __init__(self, host: Host, script: str, exec_shell: Optional[Shell] = None):
         self.host = host
         self.script = script
         self.exec_shell = exec_shell
         self._hash = hash(self.script)
```

### Comparing `eikobot-0.5.1/eikobot/core/lib/std/__init__.py` & `eikobot-0.6.0/eikobot/core/lib/std/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 The Eiko standard library contains various quality of life
 plugins and resources.
 """
 import asyncio
 import getpass
 import os
+import re
 from dataclasses import dataclass
 from ipaddress import IPv4Address, IPv6Address, ip_address
 from typing import Optional, Type, Union
 
 import asyncssh
 from asyncssh.connection import SSHClientConnection as SSHConnection
 from asyncssh.listener import SSHListener
@@ -115,14 +116,16 @@
     os_version: EikoPromise[str]
 
     class Config:
         arbitrary_types_allowed = True
         extra = Extra.allow
 
     def __post_init__(self) -> None:
+        self.is_windows_host: bool = False
+
         self._connection: SSHConnection
         self._con_ref_count: int = 0
         self._connected: asyncio.Event = asyncio.Event()
         self._disconnect_tasks: list[asyncio.Task] = []
         self._forwarded_ports: dict[int, ForwardedPortListener] = {}
         self._forwarded_ports_stop_tasks: list[asyncio.Task] = []
 
@@ -144,15 +147,29 @@
         if self.username is not None:
             extra_args["username"] = self.username
 
         if self.ssh_requires_pass:
             if self.password is not None:
                 extra_args["password"] = self.password
 
-        return await asyncssh.connect(self.host, **extra_args)
+        try:
+            return await asyncssh.connect(self.host, **extra_args)
+        except asyncssh.HostKeyNotVerifiable as e:
+            key_scan = await asyncio.subprocess.create_subprocess_shell(  # pylint: disable=no-member
+                f"ssh {self.host} echo",
+                stdout=asyncio.subprocess.PIPE,
+                stderr=asyncio.subprocess.PIPE,
+            )
+
+            _, stderr = await key_scan.communicate()
+            if key_scan.returncode != 0:
+                raise EikoDeployError(
+                    f"Host verification failed \n{stderr.decode()}"
+                ) from e
+            return await asyncssh.connect(self.host, **extra_args)
 
     def disconnect(self, ctx: HandlerContext) -> None:
         """Disconnects if nothing else is using the same connection."""
         self._disconnect_tasks.append(
             asyncio.create_task(
                 self._disconnect_delay(ctx),
                 name=f"disconnect-{self.host}-{self._con_ref_count}",
@@ -166,29 +183,114 @@
             self._connection.close()
             ctx.debug(f"SSH: Disconnected from '{self.host}'.")
 
     async def wait_until_disconnected(self) -> None:
         await asyncio.gather(*self._forwarded_ports_stop_tasks)
         await asyncio.gather(*self._disconnect_tasks)
 
+    async def scp_to(
+        self,
+        file_name: str,
+        ctx: HandlerContext,
+        destination: str | None = None,
+    ) -> None:
+        """
+        Copies a file from the local host to the remote host
+        """
+        extra_args: dict[str, str] = {}
+        if self.username is not None:
+            extra_args["username"] = self.username
+
+        if self.ssh_requires_pass:
+            if self.password is not None:
+                extra_args["password"] = self.password
+
+        if destination is None:
+            destination = file_name
+
+        ctx.debug(f"Copying file '{file_name}' to host.")
+        await asyncssh.scp(
+            file_name,
+            f"{self.host}:{destination}",
+            **extra_args,  # type: ignore
+        )
+
+    async def scp_from(
+        self,
+        file_name: str,
+        ctx: HandlerContext,
+        destination: str | None = None,
+    ) -> None:
+        """
+        Copies a file to the local host from the remote host
+        """
+        extra_args: dict[str, str] = {}
+        if self.username is not None:
+            extra_args["username"] = self.username
+
+        if self.ssh_requires_pass:
+            if self.password is not None:
+                extra_args["password"] = self.password
+
+        if destination is None:
+            destination = file_name
+
+        ctx.debug(f"Copying file '{file_name}' from host.")
+        await asyncssh.scp(
+            f"{self.host}:{file_name}",
+            destination,
+            **extra_args,  # type: ignore
+        )
+
     async def script(
         self, script: str, exec_shell: str, ctx: HandlerContext
     ) -> CmdResult:
         """Runs a script on the remote host."""
+        if self.is_windows_host:
+            script_file_name = f"script-{ctx.normalized_task_id()}.ps1"
+            with open(ctx.task_cache / script_file_name, "w", encoding="utf-8") as f:
+                f.write(script)
+
+            extra_args: dict[str, str] = {}
+            if self.username is not None:
+                extra_args["username"] = self.username
+
+            if self.ssh_requires_pass:
+                if self.password is not None:
+                    extra_args["password"] = self.password
+
+            await asyncssh.scp(
+                ctx.task_cache / script_file_name,
+                f"{self.host}:{script_file_name}",
+                **extra_args,  # type: ignore
+            )
+            result = await self._execute_windows(
+                f".\\{script_file_name}",
+                ctx,
+                script,
+            )
+            await self._connection.run(
+                f"del {script_file_name}",
+                term_type="xterm-color",
+            )
+            return result
+
         if "sudo " in script:
             ssh_exec = self._execute_sudo
         else:
             ssh_exec = self._execute
 
         _script = f"{exec_shell} << EOF\n{script}\nEOF"
         return await ssh_exec(_script, ctx, script)
 
     async def execute(self, cmd: str, ctx: HandlerContext) -> CmdResult:
         """Executes one or more commands in an ssh session."""
-        if "sudo " in cmd:
+        if self.is_windows_host:
+            ssh_exec = self._execute_windows
+        elif "sudo " in cmd:
             ssh_exec = self._execute_sudo
         else:
             ssh_exec = self._execute
 
         return await ssh_exec(cmd, ctx)
 
     async def _execute(
@@ -200,38 +302,51 @@
         """
         Execute a command on the remote host.
         Command will not be recorded.
         """
         if original_command is None:
             original_command = cmd
         ctx.debug("Execute: " + original_command)
+
         cmd_str = 'HISTIGNORE="*" ' + cmd
 
         try:
             await self.connect(ctx)
         except OSError:
             return CmdResult(
                 original_command, 1, "SSH: Failed to connect to host.", ctx
             )
 
         process = await self._connection.run(
             cmd_str,
             term_type="xterm-color",
-            stderr=asyncssh.STDOUT,
         )
         self.disconnect(ctx)
 
         if process.stdout is None:
             _stdout = ""
         elif isinstance(process.stdout, bytes):
             _stdout = process.stdout.decode()
         else:
             _stdout = process.stdout
         stdout = self._clean_log(_stdout)
-        ctx.debug("stdout:\n" + stdout)
+
+        # try again as Windows
+        if "'HISTIGNORE' is not recognized" in stdout:
+            ctx.debug(
+                "Potential Windows machine detected, retrying with updated settings."
+            )
+            self.is_windows_host = True
+            await self.execute("Set-ExecutionPolicy RemoteSigned", ctx)
+            return await self._execute_windows(cmd, ctx)
+
+        if stdout:
+            ctx.debug("stdout:\n" + stdout)
+        else:
+            ctx.debug("stdout:")
 
         returncode = 1
         if process.returncode is not None:
             returncode = process.returncode
 
         return CmdResult(original_command, returncode, stdout, ctx)
 
@@ -248,24 +363,135 @@
                 f"echo -n {self.password} | sudo -S ls > /dev/null && " + cmd,
                 ctx,
                 cmd,
             )
 
         return await self.execute(cmd, ctx)
 
+    async def _execute_windows(
+        self,
+        cmd: str,
+        ctx: HandlerContext,
+        original_command: Optional[str] = None,
+    ) -> CmdResult:
+        if original_command is None:
+            original_command = cmd
+        ctx.debug("Execute: " + original_command)
+
+        cmd = cmd.replace('"', '\\"')
+        if not cmd.startswith("powershell"):
+            cmd_str = f'powershell -NoLogo -NoProfile "{cmd}"'
+        else:
+            cmd_str = cmd
+
+        rcode_file = f"returncode-{ctx.normalized_task_id()}"
+        output_file = f"output-{ctx.normalized_task_id()}"
+        cmd_str = f"chcp 65001 & {cmd_str} > {output_file} & "
+        cmd_str += f"echo %ERRORLEVEL% > {rcode_file}"
+
+        try:
+            await self.connect(ctx)
+        except OSError:
+            return CmdResult(
+                original_command, 1, "SSH: Failed to connect to host.", ctx
+            )
+
+        await self._connection.run(
+            cmd_str,
+            term_type="xterm-color",
+        )
+
+        extra_args: dict[str, str] = {}
+        if self.username is not None:
+            extra_args["username"] = self.username
+
+        if self.ssh_requires_pass:
+            if self.password is not None:
+                extra_args["password"] = self.password
+
+        await asyncssh.scp(
+            f"{self.host}:{rcode_file}",
+            ctx.task_cache / rcode_file,
+            **extra_args,  # type: ignore
+        )
+        with open(ctx.task_cache / rcode_file, encoding="utf-8") as f:
+            returncode = int(f.read())
+        os.remove(ctx.task_cache / rcode_file)
+
+        await self._connection.run(
+            f"del {rcode_file}",
+            term_type="xterm-color",
+        )
+
+        await asyncssh.scp(
+            f"{self.host}:{output_file}",
+            ctx.task_cache / output_file,
+            **extra_args,  # type: ignore
+        )
+        with open(ctx.task_cache / output_file, encoding="utf-8") as f:
+            stdout = self._clean_log(f.read())
+        os.remove(ctx.task_cache / output_file)
+
+        await self._connection.run(
+            f"del {output_file}",
+            term_type="xterm-color",
+        )
+
+        if stdout:
+            ctx.debug("stdout:\n" + stdout)
+        else:
+            ctx.debug("stdout:")
+
+        self.disconnect(ctx)
+
+        return CmdResult(original_command, returncode, stdout, ctx)
+
     def _clean_log(self, log: str) -> str:
         log = log.replace("\r\n", "\n")
+
+        # strip all ansi characters
+        ansi_escape = re.compile(
+            r"""
+                \x1B  # ESC
+                (?:   # 7-bit C1 Fe (except CSI)
+                    [@-Z\\-_]
+                |     # or [ for CSI, followed by a control sequence
+                    \[
+                    [0-?]*  # Parameter bytes
+                    [ -/]*  # Intermediate bytes
+                    [@-~]   # Final byte
+                )
+            """,
+            re.VERBOSE,
+        )
+        log = ansi_escape.sub("", log)
+
         sudo_log_str = "[sudo] password for "
         if self.username is not None:
             sudo_log_str += self.username
         else:
             sudo_log_str += os.getlogin()
-
         sudo_log_str += ": "
-        return log.replace(sudo_log_str, "")
+        log = log.replace(sudo_log_str, "")
+
+        # weird windows stuff
+        log = log.replace("0;Administrator: C:\\Windows\\system32\\conhost.exe", "")
+        log = log.replace("0;C:\\Windows\\system32\\conhost.exe", "")
+        log = log.replace("Active code page: 65001", "")
+
+        # strip beeps, lol
+        log = log.replace("\x07", "")
+
+        log = log.removesuffix("\n")
+
+        # Remove any extranious whitespace
+        while "\n\n\n" in log:
+            log = log.replace("\n\n\n", "\n\n")
+
+        return log
 
     async def forward_port(
         self, ctx: HandlerContext, local_port: int, remote_port: int | None = None
     ) -> None:
         """
         Forwards a port using ssh.
         """
@@ -353,37 +579,49 @@
             return
 
         os_platform_promis = ctx.resource.raw_resource.promises["os_platform"]
         os_name_promise = ctx.resource.raw_resource.promises["os_name"]
         os_version_promis = ctx.resource.raw_resource.promises["os_version"]
 
         os_string = result.output.replace("\n", "")
-        os_platform_promis.set(os_string, ctx)
         if os_string == "":
             os_platform_promis.set("windows", ctx)
             os_name_promise.set("windows", ctx)
             os_version_result = await ctx.resource.execute(
-                r'(Get-ItemProperty "HKLM:\SOFTWARE\Microsoft\Windows NT\CurrentVersion").ReleaseId',
+                "(Get-ComputerInfo).WindowsProductName",
                 ctx,
             )
             os_version_promis.set(os_version_result.output.replace("\n", ""), ctx)
+            await ctx.resource.execute("Set-ExecutionPolicy RemoteSigned", ctx)
+            ctx.debug(f"OS Detection: {os_version_promis.resolve(str)}")
         elif os_string == "linux-gnu":
+            os_platform_promis.set("linux-gnu", ctx)
             os_release = await ctx.resource.execute("cat /etc/os-release", ctx)
             os_info: dict[str, str] = {}
             for line in os_release.output.splitlines():
                 key, value = line.split("=")
                 os_info[key] = value
 
             os_name_promise.set(os_info["ID"], ctx)
             os_version_promis.set(os_info["VERSION_ID"], ctx)
+            ctx.debug(
+                "OS Detection: "
+                f"{os_platform_promis.resolve(str)}-{os_name_promise.resolve(str)}-{os_version_promis.resolve(str)}"
+            )
 
         else:
+            os_platform_promis.set("unknown", ctx)
             os_name_promise.set("unknown", ctx)
             os_version_promis.set("unknown", ctx)
 
+            ctx.debug(
+                "OS Detection: "
+                f"{os_platform_promis.resolve(str)}-{os_name_promise.resolve(str)}-{os_version_promis.resolve(str)}"
+            )
+
         ctx.deployed = True
 
     async def cleanup(self, ctx: HandlerContext) -> None:
         ctx.debug("Cleaning up ssh connection.")
         if isinstance(ctx.resource, HostModel):
             await ctx.resource.wait_until_disconnected()
 
@@ -452,15 +690,15 @@
         if ctx.resource.exec_shell is None:
             platform = ctx.resource.host.os_platform.resolve(str)
             if platform == "linux-gnu":
                 exec_shell = "bash"
             elif platform == "windows":
                 exec_shell = "powershell"
             else:
-                exec_shell = "bash"
+                exec_shell = "sh"
         else:
             exec_shell = ctx.resource.exec_shell
 
         result = await ctx.resource.host.script(ctx.resource.script, exec_shell, ctx)
         if result.failed():
             return
```

### Comparing `eikobot-0.5.1/eikobot/core/lib/std/env.py` & `eikobot-0.6.0/eikobot/core/lib/std/env.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/eikobot/core/lib/std/file.py` & `eikobot-0.6.0/eikobot/core/lib/std/file.py`

 * *Files 21% similar despite different names*

```diff
@@ -103,137 +103,172 @@
     __eiko_resource__ = "File"
 
     async def create(self, ctx: HandlerContext) -> None:
         if not isinstance(ctx.resource, FileModel):
             ctx.failed = True
             return
 
-        if ctx.resource.requires_sudo:
+        if ctx.resource.host.is_windows_host:
+            await self._create_win(ctx, ctx.resource)
+
+        else:
+            await self._create(ctx, ctx.resource)
+
+    async def _create(self, ctx: HandlerContext, resource: FileModel) -> None:
+        if resource.requires_sudo:
             sudo = "sudo "
         else:
             sudo = ""
 
-        result = await ctx.resource.host.execute(
-            f"{sudo}mkdir -p {ctx.resource.path.parent}", ctx
+        result = await resource.host.execute(
+            f"{sudo}mkdir -p {resource.path.parent}", ctx
         )
         if result.returncode != 0:
             ctx.failed = True
             return
 
-        result = await ctx.resource.host.execute(
-            f'echo -n "{ctx.resource.content}" | {sudo}tee {ctx.resource.path}',
+        result = await resource.host.execute(
+            f'echo -n "{resource.content}" | {sudo}tee {resource.path}',
             ctx,
         )
         if result.returncode != 0:
             ctx.failed = True
             return
 
-        result = await ctx.resource.host.execute(
-            f"{sudo}chmod {ctx.resource.mode} " f"{ctx.resource.path}",
+        result = await resource.host.execute(
+            f"{sudo}chmod {resource.mode} " f"{resource.path}",
             ctx,
         )
         if result.returncode != 0:
             ctx.failed = True
             return
 
-        if ctx.resource.owner is not None:
-            result = await ctx.resource.host.execute(
-                f"{sudo}chown {ctx.resource.owner} {ctx.resource.path}",
+        if resource.owner is not None:
+            result = await resource.host.execute(
+                f"{sudo}chown {resource.owner} {resource.path}",
                 ctx,
             )
             if result.returncode != 0:
                 ctx.failed = True
                 return
 
-        if ctx.resource.group is not None:
-            result = await ctx.resource.host.execute(
-                f"{sudo}chgrp {ctx.resource.group} {ctx.resource.path}",
+        if resource.group is not None:
+            result = await resource.host.execute(
+                f"{sudo}chgrp {resource.group} {resource.path}",
                 ctx,
             )
             if result.returncode != 0:
                 ctx.failed = True
                 return
 
         ctx.deployed = True
 
+    async def _create_win(self, ctx: HandlerContext, resource: FileModel) -> None:
+        result = await resource.host.execute(f"mkdir {resource.path.parent}", ctx)
+        if result.returncode != 0:
+            ctx.failed = True
+            return
+
+        with open(ctx.task_cache / resource.path.name, "w", encoding="utf-8") as f:
+            f.write(resource.content)
+
+        await resource.host.scp_to(
+            str(ctx.task_cache / resource.path.name),
+            ctx,
+            str(resource.path),
+        )
+
+        ctx.deployed = True
+
     async def read(self, ctx: HandlerContext) -> None:
         if not isinstance(ctx.resource, FileModel):
             ctx.failed = True
             return
 
-        if ctx.resource.requires_sudo:
+        if ctx.resource.host.is_windows_host:
+            await self._read_win(ctx, ctx.resource)
+
+        else:
+            await self._read(ctx, ctx.resource)
+
+    async def _read(self, ctx: HandlerContext, resource: FileModel) -> None:
+        if resource.requires_sudo:
             sudo = "sudo "
         else:
             sudo = ""
 
-        cat_result = await ctx.resource.host.execute(
-            f"{sudo}cat {ctx.resource.path}", ctx
-        )
+        cat_result = await resource.host.execute(f"{sudo}cat {resource.path}", ctx)
         if cat_result.returncode == 0:
             ctx.deployed = True
-            if cat_result.output != ctx.resource.content:
+            if cat_result.output != resource.content:
                 ctx.add_change("content", cat_result.output)
 
-            ls_result = await ctx.resource.host.execute(
-                f"{sudo}ls -l {ctx.resource.path}", ctx
-            )
+            ls_result = await resource.host.execute(f"{sudo}ls -l {resource.path}", ctx)
             if ls_result.returncode == 0:
                 if isinstance(ls_result.output, str):
                     ls_parsed = ls_result.output.split(" ")
-                    if parse_rwx_mode(ls_parsed[0]) != ctx.resource.mode:
+                    if parse_rwx_mode(ls_parsed[0]) != resource.mode:
                         ctx.add_change("mode", parse_rwx_mode(ls_parsed[0]))
-                    if (
-                        ctx.resource.owner is not None
-                        and ls_parsed[2] != ctx.resource.owner
-                    ):
+                    if resource.owner is not None and ls_parsed[2] != resource.owner:
                         ctx.add_change("owner", ls_parsed[2])
-                    if (
-                        ctx.resource.group is not None
-                        and ls_parsed[3] != ctx.resource.group
-                    ):
+                    if resource.group is not None and ls_parsed[3] != resource.group:
                         ctx.add_change("group", ls_parsed[3])
                 else:
                     ctx.failed = True
 
+    async def _read_win(self, ctx: HandlerContext, resource: FileModel) -> None:
+        cat_result = await resource.host.execute(f"cat {resource.path}", ctx)
+        if cat_result.returncode == 0:
+            ctx.deployed = True
+            if cat_result.output != resource.content:
+                ctx.add_change("content", cat_result.output)
+
     async def update(self, ctx: HandlerContext) -> None:
         if not isinstance(ctx.resource, FileModel):
             ctx.failed = True
             return
 
-        if ctx.resource.requires_sudo:
+        if ctx.resource.host.is_windows_host:
+            await self._create_win(ctx, ctx.resource)
+
+        else:
+            await self._update(ctx, ctx.resource)
+
+    async def _update(self, ctx: HandlerContext, resource: FileModel) -> None:
+        if resource.requires_sudo:
             sudo = "sudo "
         else:
             sudo = ""
 
         if ctx.changes.get("content") is not None:
-            result = await ctx.resource.host.execute(
-                f'echo -n "{ctx.resource.content}" | {sudo}tee {ctx.resource.path}',
+            result = await resource.host.execute(
+                f'echo -n "{resource.content}" | {sudo}tee {resource.path}',
                 ctx,
             )
             if result.failed():
                 return
 
         if ctx.changes.get("mode") is not None:
-            result = await ctx.resource.host.execute(
-                f"{sudo}chmod {ctx.resource.mode} " f"{ctx.resource.path}",
+            result = await resource.host.execute(
+                f"{sudo}chmod {resource.mode} " f"{resource.path}",
                 ctx,
             )
             if result.failed():
                 return
 
         if ctx.changes.get("owner") is not None:
-            result = await ctx.resource.host.execute(
-                f"{sudo}chown {ctx.resource.owner} {ctx.resource.path}",
+            result = await resource.host.execute(
+                f"{sudo}chown {resource.owner} {resource.path}",
                 ctx,
             )
             if result.failed():
                 return
 
         if ctx.changes.get("group") is not None:
-            result = await ctx.resource.host.execute(
-                f"{sudo}chgrp {ctx.resource.group} {ctx.resource.path}",
+            result = await resource.host.execute(
+                f"{sudo}chgrp {resource.group} {resource.path}",
                 ctx,
             )
             if result.failed():
                 return
 
         ctx.deployed = True
```

### Comparing `eikobot-0.5.1/eikobot/core/lib/std/test.py` & `eikobot-0.6.0/eikobot/core/lib/std/test.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/eikobot/core/logger.py` & `eikobot-0.6.0/eikobot/core/logger.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/eikobot/core/package_manager/__init__.py` & `eikobot-0.6.0/eikobot/core/package_manager/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 import copy
 import os
 import shutil
 import subprocess
 import sys
 import tarfile
 import tomllib
-from dataclasses import dataclass
 from pathlib import Path
 from typing import Optional
 from urllib.parse import urlparse
 
 import aiohttp
 from packaging import version
 from pydantic import BaseModel, ValidationError
 
 from ... import VERSION
-from .. import logger
+from .. import human_readable, logger
 from ..compiler.importlib import INTERNAL_LIB_PATH
+from ..errors import EikoError
 
 CACHE_PATH = Path(__file__).parent / "cache"
 CACHE_PATH.mkdir(exist_ok=True)
 LIB_PATH = Path(__file__).parent / "lib"
 LIB_PATH.mkdir(exist_ok=True)
 
 PKG_INDEX: dict[str, "PackageData"] = {}
 
 
-class EikoPackageError(Exception):
+class EikoPackageError(EikoError):
     """An error that occured during the eiko compilation process."""
 
     def __init__(self, reason: str, *args: object) -> None:
         super().__init__(reason, *args)
 
 
 class PackageData(BaseModel):
@@ -203,23 +203,14 @@
 
     else:
         raise EikoPackageError(
             "Currently only direct links to an eiko package are supported."
         )
 
 
-def _human_readable(number: int) -> str:
-    number = number // 8
-    for unit in ["", "K", "M", "G", "T"]:
-        if number < 10240:
-            return f"{number}{unit}B"
-        number = number // 1024
-    return f"{number}PB"
-
-
 async def _download_to_cache(url: str) -> None:
     pkg_path = CACHE_PATH / Path(urlparse(url).path).name
     async with aiohttp.ClientSession(timeout=aiohttp.ClientTimeout(10)) as session:
         logger.info(f"Fetching {url}")
         try:
             response = await session.get(url)
             total_dl_size = int(response.headers.get("CONTENT-LENGTH", 0))
@@ -230,20 +221,20 @@
                     f.write(data)
                     downloaded += sys.getsizeof(data)
                     percent = int((downloaded / total_dl_size) * 20)
                     pg_bar = "=" * percent
                     if percent == 20:
                         print(
                             f"    [{pg_bar}]",
-                            f"{_human_readable(total_dl_size)}/{_human_readable(total_dl_size)}",
+                            f"{human_readable(total_dl_size)}/{human_readable(total_dl_size)}",
                         )
                     else:
                         print(
                             f"    [{pg_bar}>{(20 - percent - 1) * ' '}]",
-                            f"{_human_readable(downloaded)}/{_human_readable(total_dl_size)}",
+                            f"{human_readable(downloaded)}/{human_readable(total_dl_size)}",
                             end="\r",
                         )
 
         except aiohttp.ClientError as e:
             raise EikoPackageError(f"Failed to download {url}: {e}") from e
 
     _install_pkg_from_cache(pkg_path.name)
@@ -268,14 +259,17 @@
 
     pkg_lib_path = LIB_PATH / pkg_name
     pkg_data = _read_pkg_toml(pkg_lib_path / "eiko.toml")
     prev_pkg = PKG_INDEX.get(pkg_data.name)
     if prev_pkg is not None:
         _uninstall_pkg(prev_pkg)
 
+    with tarfile.open(CACHE_PATH / archive_name, "r:gz") as archive:
+        archive.extractall(LIB_PATH)
+
     if pkg_data.version is None:
         logger.debug(f"Installing '{pkg_data.name}'.")
     else:
         logger.debug(f"Installing '{pkg_data.name}=={pkg_data.version}'.")
 
     requirements_file = pkg_lib_path / "requirements.txt"
     if requirements_file.exists():
@@ -286,16 +280,18 @@
         )
 
     logger.debug("Installing requirements.")
     for req in pkg_data.requires:
         install_pkg(req)
 
     try:
-        os.symlink(
-            pkg_lib_path / pkg_data.source_dir, INTERNAL_LIB_PATH / pkg_data.source_dir
+        shutil.copytree(
+            pkg_lib_path / pkg_data.source_dir,
+            INTERNAL_LIB_PATH / pkg_data.source_dir,
+            dirs_exist_ok=False,
         )
     except FileExistsError:
         # This is a bug in the package index
         # I have no idea what causes it, but this is hack around the issue.
         os.remove(INTERNAL_LIB_PATH / pkg_data.source_dir)
         os.symlink(
             pkg_lib_path / pkg_data.source_dir, INTERNAL_LIB_PATH / pkg_data.source_dir
@@ -323,10 +319,14 @@
         return
 
     _uninstall_pkg(pkg_data)
 
 
 def _uninstall_pkg(pkg_data: PackageData) -> None:
     logger.debug(f"Uninstalling '{pkg_data.pkg_name_version()}'")
-    os.remove(INTERNAL_LIB_PATH / pkg_data.source_dir)
+    try:
+        shutil.rmtree(INTERNAL_LIB_PATH / pkg_data.source_dir)
+    except FileNotFoundError:
+        pass
+
     shutil.rmtree(LIB_PATH / pkg_data.pkg_name_version())
     logger.info(f"Uninstalled '{pkg_data.pkg_name_version()}'")
```

### Comparing `eikobot-0.5.1/eikobot.egg-info/SOURCES.txt` & `eikobot-0.6.0/eikobot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/setup.cfg` & `eikobot-0.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 warn_redundant_casts = True
 warn_return_any = True
 warn_unused_ignores = True
 disallow_untyped_decorators = True
 
 [flake8]
 max-line-length = 120
-ignore = W191, W503, F401
+ignore = W191, W503, F401, E203
 exclude = 
 	__pycache__,
 	build,
 	dist,
 	.pytest_cache,
 	.mypy_cache,
```

### Comparing `eikobot-0.5.1/setup.py` & `eikobot-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 import setuptools
 
 this_directory = Path(__file__).parent
 with open(this_directory / "README.md", encoding="utf-8") as f:
     long_description = f.read()
 
-VERSION = "0.5.1"
+VERSION = "0.6.0"
 REQUIRES = [
-    "aiohttp==3.8.4",
+    "aiohttp==3.8.5",
     "asyncssh==2.13.1",
     "click==8.1.3",
     "colorama==0.4.6",
     "jinja2==3.1.2",
     "packaging==23.1",
     "pydantic==1.10.4",
 ]
```

### Comparing `eikobot-0.5.1/tests/test_compilation.py` & `eikobot-0.6.0/tests/test_compilation.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 
 import pytest
 
 from eikobot.core.compiler import Compiler
 from eikobot.core.compiler._parser import Parser
 from eikobot.core.compiler.definitions._resource import EikoResourceDefinition
 from eikobot.core.compiler.definitions.base_types import (
+    EikoBool,
     EikoEnumValue,
     EikoInt,
+    EikoList,
     EikoNone,
     EikoResource,
     EikoStr,
 )
 from eikobot.core.compiler.definitions.context import CompilerContext
 from eikobot.core.compiler.definitions.typedef import EikoTypeDef
 from eikobot.core.errors import EikoCompilationError
@@ -264,14 +266,22 @@
     assert var_h.type.name == "Test"
     assert var_h.type.super is not None
     assert var_h.type.super.name == "Object"
     assert var_h.to_py() == {
         "prop_1": var_d.to_py(),
     }
 
+    var_i = compiler.context.get("i")
+    assert isinstance(var_i, EikoResource)
+    assert var_i.type.name == "TripleDotInherit"
+    assert var_i.to_py() == {
+        "prop_1": "a",
+        "prop_2": 1,
+    }
+
 
 def test_enum(eiko_enum_file: Path) -> None:
     compiler = Compiler()
     compiler.compile(eiko_enum_file)
 
     var_test_1 = compiler.context.get("test_1")
     assert isinstance(var_test_1, EikoResource)
@@ -286,7 +296,52 @@
     var_test_2_enum_opt_1 = var_test_2.properties.get("prop_1")
     assert isinstance(var_test_2_enum_opt_1, EikoEnumValue)
     assert var_test_2_enum_opt_1.value == "option_1"
 
     var_enum_to_str = compiler.context.get("enum_to_str")
     assert isinstance(var_enum_to_str, EikoStr)
     assert var_enum_to_str.value == "option_3"
+
+
+@pytest.mark.parametrize(
+    "input_str,outcome",
+    [
+        ('a = 1\nb = type(a) == "int"', True),
+        ('a = 1\nb = type(a) == "str"', False),
+        ('a = "1"\nb = type(a) == "str"', True),
+        ('a = True\nb = type(a) == "bool"', True),
+        ('a = [True]\nb = type(a) == "list[bool]"', True),
+    ],
+)
+def test_type_plugin(tmp_eiko_file: Path, input_str: str, outcome: bool) -> None:
+    compiler = Compiler()
+
+    with open(tmp_eiko_file, "w", encoding="utf-8") as f:
+        f.write(input_str)
+
+    compiler.compile(tmp_eiko_file)
+    b = compiler.context.get("b")
+    assert isinstance(b, EikoBool)
+    assert b.value == outcome
+
+
+def test_for(eiko_for_file: Path) -> None:
+    compiler = Compiler()
+    compiler.compile(eiko_for_file)
+
+    results_list = compiler.context.get("test_list")
+    assert isinstance(results_list, EikoList)
+
+    assert isinstance(results_list.elements[0], EikoStr)
+    assert results_list.elements[0].value == "hello"
+
+    assert isinstance(results_list.elements[1], EikoStr)
+    assert results_list.elements[1].value == "haha"
+
+    assert isinstance(results_list.elements[2], EikoInt)
+    assert results_list.elements[2].value == 12
+
+    assert isinstance(results_list.elements[3], EikoStr)
+    assert results_list.elements[3].value == "key_1"
+
+    assert isinstance(results_list.elements[4], EikoInt)
+    assert results_list.elements[4].value == 1
```

### Comparing `eikobot-0.5.1/tests/test_datatypes.py` & `eikobot-0.6.0/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/tests/test_decorator.py` & `eikobot-0.6.0/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/tests/test_deployer.py` & `eikobot-0.6.0/tests/test_deployer.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/tests/test_exporter.py` & `eikobot-0.6.0/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/tests/test_import.py` & `eikobot-0.6.0/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/tests/test_lexer.py` & `eikobot-0.6.0/tests/test_lexer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # pylint: disable=missing-module-docstring
 # pylint: disable=missing-function-docstring
 # pylint: disable=protected-access
 # pylint: disable=too-many-statements
 from pathlib import Path
 
+import pytest
+
 from eikobot.core.compiler._token import Token, TokenType
-from eikobot.core.compiler.lexer import Lexer
+from eikobot.core.compiler.lexer import EikoSyntaxError, Lexer
 from eikobot.core.compiler.misc import Index
 
 
 def test_char_generator(eiko_file_1: Path) -> None:
     """
     Tests Lexer._next_char and Lexer._current_index
     """
@@ -451,7 +453,23 @@
 def test_comment_end_of_file_lexing(tmp_eiko_file: Path) -> None:
     with open(tmp_eiko_file, "w", encoding="utf-8") as f:
         f.write("# Test comment")
 
     lexer = Lexer(tmp_eiko_file)
     assert lexer.next_token() == Token(TokenType.INDENT, "", Index(0, 0, tmp_eiko_file))
     assert lexer.next_token() == Token(TokenType.EOF, "EOF", Index(1, 0, tmp_eiko_file))
+
+
+def test_unicode_escape_error(tmp_eiko_file: Path) -> None:
+    file_path = "\\U"
+    model = f'path = Path("{file_path}")'
+    with open(tmp_eiko_file, "w", encoding="utf-8") as f:
+        f.write(model)
+
+    lexer = Lexer(tmp_eiko_file)
+    lexer.next_token()
+    lexer.next_token()
+    lexer.next_token()
+    lexer.next_token()
+    lexer.next_token()
+    with pytest.raises(EikoSyntaxError):
+        lexer.next_token()
```

### Comparing `eikobot-0.5.1/tests/test_package.py` & `eikobot-0.6.0/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `eikobot-0.5.1/tests/test_parser.py` & `eikobot-0.6.0/tests/test_parser.py`

 * *Files identical despite different names*

