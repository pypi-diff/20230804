# Comparing `tmp/weasel-0.1.1.tar.gz` & `tmp/weasel-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weasel-0.1.1.tar", last modified: Fri Jul  7 07:38:14 2023, max compression
+gzip compressed data, was "weasel-0.2.0.tar", last modified: Fri Aug  4 11:12:06 2023, max compression
```

## Comparing `weasel-0.1.1.tar` & `weasel-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.092214 weasel-0.1.1/
--rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-07-07 07:38:04.000000 weasel-0.1.1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)     4055 2023-07-07 07:38:14.092214 weasel-0.1.1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     3024 2023-07-07 07:38:04.000000 weasel-0.1.1/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      403 2023-07-07 07:38:04.000000 weasel-0.1.1/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)     1374 2023-07-07 07:38:14.092214 weasel-0.1.1/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)      136 2023-07-07 07:38:04.000000 weasel-0.1.1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.084215 weasel-0.1.1/weasel/
--rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/about.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.088214 weasel-0.1.1/weasel/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)      272 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8231 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/assets.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4757 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/clone.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5160 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/document.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8460 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/dvc.py
--rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/main.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2934 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/pull.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2764 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/push.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7967 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/remote_storage.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14748 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/cli/run.py
--rw-r--r--   0 vsts      (1001) docker     (122)      134 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/compat.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1006 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/errors.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4627 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/schemas.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.088214 weasel-0.1.1/weasel/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.088214 weasel-0.1.1/weasel/tests/cli/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/cli/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6698 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/cli/test_cli.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5928 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/cli/test_cli_app.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1908 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/cli/test_document.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2058 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/cli/test_remote.py
--rw-r--r--   0 vsts      (1001) docker     (122)      831 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/test_schemas.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5222 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/test_validation.py
--rw-r--r--   0 vsts      (1001) docker     (122)      600 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/tests/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.092214 weasel-0.1.1/weasel/util/
--rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2960 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/commands.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5778 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/config.py
--rw-r--r--   0 vsts      (1001) docker     (122)      595 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/environment.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2796 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/filesystem.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2232 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/frozen.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6419 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/git.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1380 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/hashing.py
--rw-r--r--   0 vsts      (1001) docker     (122)      247 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/logging.py
--rw-r--r--   0 vsts      (1001) docker     (122)      587 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/modules.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1294 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/remote.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3221 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/validation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2098 2023-07-07 07:38:04.000000 weasel-0.1.1/weasel/util/versions.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-07-07 07:38:14.088214 weasel-0.1.1/weasel.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     4055 2023-07-07 07:38:14.000000 weasel-0.1.1/weasel.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1117 2023-07-07 07:38:14.000000 weasel-0.1.1/weasel.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-07-07 07:38:14.000000 weasel-0.1.1/weasel.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       42 2023-07-07 07:38:14.000000 weasel-0.1.1/weasel.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      202 2023-07-07 07:38:14.000000 weasel-0.1.1/weasel.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-07-07 07:38:14.000000 weasel-0.1.1/weasel.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-04 11:12:06.640233 weasel-0.2.0/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1083 2023-08-04 11:11:51.000000 weasel-0.2.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)     4078 2023-08-04 11:12:06.640233 weasel-0.2.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     3024 2023-08-04 11:11:51.000000 weasel-0.2.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      403 2023-08-04 11:11:51.000000 weasel-0.2.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)     1437 2023-08-04 11:12:06.640233 weasel-0.2.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)      136 2023-08-04 11:11:51.000000 weasel-0.2.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-04 11:12:06.632233 weasel-0.2.0/weasel/
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       59 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       82 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/about.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-04 11:12:06.636233 weasel-0.2.0/weasel/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)      272 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8231 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/cli/assets.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4757 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/cli/clone.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5739 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/cli/document.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8460 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/cli/dvc.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      441 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/cli/main.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2934 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/cli/pull.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2764 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/cli/push.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7953 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/cli/remote_storage.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    14748 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/cli/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      134 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1006 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/errors.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4016 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/schemas.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-04 11:12:06.636233 weasel-0.2.0/weasel/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-04 11:12:06.636233 weasel-0.2.0/weasel/tests/cli/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/tests/cli/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6698 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/tests/cli/test_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5928 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/tests/cli/test_cli_app.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3628 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/tests/cli/test_document.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2058 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/tests/cli/test_remote.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      831 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/tests/test_schemas.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5222 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/tests/test_validation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      600 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/tests/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-04 11:12:06.640233 weasel-0.2.0/weasel/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      841 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2960 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/util/commands.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5778 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/util/config.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1058 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/util/environment.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2801 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/util/filesystem.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2232 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/util/frozen.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6419 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/util/git.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1380 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/util/hashing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      247 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/util/logging.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      587 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/util/modules.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1301 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/util/remote.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3221 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/util/validation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2098 2023-08-04 11:11:51.000000 weasel-0.2.0/weasel/util/versions.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-04 11:12:06.632233 weasel-0.2.0/weasel.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     4078 2023-08-04 11:12:06.000000 weasel-0.2.0/weasel.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1117 2023-08-04 11:12:06.000000 weasel-0.2.0/weasel.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-04 11:12:06.000000 weasel-0.2.0/weasel.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       42 2023-08-04 11:12:06.000000 weasel-0.2.0/weasel.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)      240 2023-08-04 11:12:06.000000 weasel-0.2.0/weasel.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        7 2023-08-04 11:12:06.000000 weasel-0.2.0/weasel.egg-info/top_level.txt
```

### Comparing `weasel-0.1.1/LICENSE` & `weasel-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/PKG-INFO` & `weasel-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weasel
-Version: 0.1.1
+Version: 0.2.0
 Summary: Weasel: A small and easy workflow system
 Home-page: https://github.com/explosion/weasel/
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/weasel/releases
 Project-URL: Source, https://github.com/explosion/weasel/
@@ -17,14 +17,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # Weasel: A small and easy workflow system
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: weasel Version: 0.1.1 Summary: Weasel: A small and
+Metadata-Version: 2.1 Name: weasel Version: 0.2.0 Summary: Weasel: A small and
 easy workflow system Home-page: https://github.com/explosion/weasel/ Author:
 Explosion Author-email: contact@explosion.ai License: MIT Project-URL: Release
 notes, https://github.com/explosion/weasel/releases Project-URL: Source, https:
 //github.com/explosion/weasel/ Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Scientific/Engineering Description-Content-
-Type: text/markdown License-File: LICENSE [https://explosion.ai/assets/img/
-logo.svg] # Weasel: A small and easy workflow system Weasel lets you manage and
-share **end-to-end workflows** for different **use cases and domains**, and
-orchestrate training, packaging and serving your custom pipelines. You can
-start off by cloning a pre-defined project template, adjust it to fit your
-needs, load in your data, train a pipeline, export it as a Python package,
-upload your outputs to a remote storage and share your results with your team.
-Weasel can be used via the [`weasel`](https://github.com/explosion/weasel/blob/
-main/docs/cli.md) command and we provide templates in our [`projects`](https://
-github.com/explosion/projects) repo. ![Illustration of project workflow and
-commands](https://raw.githubusercontent.com/explosion/weasel/main/docs/assets/
-images/projects.svg) ## ð¡ Example: Get started with a project template The
-easiest way to get started is to clone a project template and run it âÂ for
-example, this [end-to-end template](https://github.com/explosion/projects/tree/
-v3/pipelines/tagger_parser_ud) that lets you train a spaCy **part-of-speech
+Python :: 3.11 Classifier: Topic :: Scientific/Engineering Requires-Python:
+>=3.6 Description-Content-Type: text/markdown License-File: LICENSE [https://
+explosion.ai/assets/img/logo.svg] # Weasel: A small and easy workflow system
+Weasel lets you manage and share **end-to-end workflows** for different **use
+cases and domains**, and orchestrate training, packaging and serving your
+custom pipelines. You can start off by cloning a pre-defined project template,
+adjust it to fit your needs, load in your data, train a pipeline, export it as
+a Python package, upload your outputs to a remote storage and share your
+results with your team. Weasel can be used via the [`weasel`](https://
+github.com/explosion/weasel/blob/main/docs/cli.md) command and we provide
+templates in our [`projects`](https://github.com/explosion/projects) repo. !
+[Illustration of project workflow and commands](https://
+raw.githubusercontent.com/explosion/weasel/main/docs/assets/images/
+projects.svg) ## ð¡ Example: Get started with a project template The easiest
+way to get started is to clone a project template and run it âÂ for example,
+this [end-to-end template](https://github.com/explosion/projects/tree/v3/
+pipelines/tagger_parser_ud) that lets you train a spaCy **part-of-speech
 tagger** and **dependency parser** on a Universal Dependencies treebank.
 ```shell python -m weasel clone pipelines/tagger_parser_ud ``` > **Note** > >
 Our [`projects`](https://github.com/explosion/projects) repo includes various >
 project templates for different NLP tasks, models, workflows and integrations >
 that you can clone and run. The easiest way to get started is to pick a >
 template, clone it and start modifying it! ## ð Documentation Get started
 with the documentation: - [Learn how to create a Weasel workflow](https://
```

### Comparing `weasel-0.1.1/README.md` & `weasel-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/setup.cfg` & `weasel-0.2.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = weasel
-version = 0.1.1
+version = 0.2.0
 description = Weasel: A small and easy workflow system
 url = https://github.com/explosion/weasel/
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -23,24 +23,26 @@
 	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering
 project_urls = 
 	Release notes = https://github.com/explosion/weasel/releases
 	Source = https://github.com/explosion/weasel/
 
 [options]
+python_requires = >=3.6
 install_requires = 
-	confection>=0.0.4,<0.1.0
+	confection>=0.0.4,<0.2.0
 	packaging>=20.0
 	wasabi>=0.9.1,<1.2.0
 	srsly>=2.4.3,<3.0.0
 	catalogue>=2.0.6,<2.1.0
 	typer>=0.3.0,<0.8.0
-	pathy>=0.10.0
+	cloudpathlib>=0.7.0,<0.16.0
+	smart-open>=5.2.1,<7.0.0
 	requests>=2.13.0,<3.0.0
-	pydantic>=1.7.4,!=1.8,!=1.8.1,<1.11.0
+	pydantic>=1.7.4,!=1.8,!=1.8.1,<3.0.0
 
 [options.entry_points]
 console_scripts = 
 	weasel = weasel.cli:app
 
 [mypy]
 ignore_missing_imports = True
```

### Comparing `weasel-0.1.1/weasel/cli/assets.py` & `weasel-0.2.0/weasel/cli/assets.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/cli/clone.py` & `weasel-0.2.0/weasel/cli/clone.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/cli/document.py` & `weasel-0.2.0/weasel/cli/document.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 and will run the specified commands in order. Commands are only re-run if their
 inputs have changed."""
 INTRO_ASSETS = f"""The following assets are defined by the project. They can
 be fetched by running [`weasel assets`]({DOCS_URL}/tree/main/docs/cli.md#open_file_folder-assets)
 in the project directory."""
 # These markers are added to the Markdown and can be used to update the file in
 # place if it already exists. Only the auto-generated part will be replaced.
-MARKER_START = "<!-- WEASEL: AUTO-GENERATED DOCS START (do not remove) -->"
-MARKER_END = "<!-- WEASEL: AUTO-GENERATED DOCS END (do not remove) -->"
+MARKER_TAGS = ("WEASEL", "SPACY PROJECT")
+MARKER_START = "<!-- {tag}: AUTO-GENERATED DOCS START (do not remove) -->"
+MARKER_END = "<!-- {tag}: AUTO-GENERATED DOCS END (do not remove) -->"
 # If this marker is used in an existing README, it's ignored and not replaced
-MARKER_IGNORE = "<!-- WEASEL: IGNORE -->"
+MARKER_IGNORE = "<!-- {tag}: IGNORE -->"
 
 
 @app.command("document")
 def project_document_cli(
     # fmt: off
     project_dir: Path = Arg(Path.cwd(), help="Path to cloned project. Defaults to current working directory.", exists=True, file_okay=False),
     output_file: Path = Opt("-", "--output", "-o", help="Path to output Markdown file for output. Defaults to - for standard output"),
@@ -48,15 +49,15 @@
 
 def project_document(
     project_dir: Path, output_file: Path, *, no_emoji: bool = False
 ) -> None:
     is_stdout = str(output_file) == "-"
     config = load_project_config(project_dir)
     md = MarkdownRenderer(no_emoji=no_emoji)
-    md.add(MARKER_START)
+    md.add(MARKER_START.format(tag="WEASEL"))
     title = config.get("title")
     description = config.get("description")
     md.add(md.title(1, f"Weasel Project{f': {title}' if title else ''}", "🪐"))
     if description:
         md.add(description)
     md.add(md.title(2, PROJECT_FILE, "📋"))
     md.add(INTRO_PROJECT)
@@ -87,29 +88,43 @@
                 if (p / dest_path).exists():
                     dest = md.link(dest, dest_path)
         data.append((dest, source, a.get("description", "")))
     if data:
         md.add(md.title(3, "Assets", "🗂"))
         md.add(INTRO_ASSETS)
         md.add(md.table(data, ["File", "Source", "Description"]))
-    md.add(MARKER_END)
+    md.add(MARKER_END.format(tag="WEASEL"))
     # Output result
     if is_stdout:
         print(md.text)
     else:
         content = md.text
         if output_file.exists():
             with output_file.open("r", encoding="utf8") as f:
                 existing = f.read()
-            if MARKER_IGNORE in existing:
-                msg.warn("Found ignore marker in existing file: skipping", output_file)
-                return
-            if MARKER_START in existing and MARKER_END in existing:
-                msg.info("Found existing file: only replacing auto-generated docs")
-                before = existing.split(MARKER_START)[0]
-                after = existing.split(MARKER_END)[1]
-                content = f"{before}{content}{after}"
-            else:
+
+            for marker_tag in MARKER_TAGS:
+                if MARKER_IGNORE.format(tag=marker_tag) in existing:
+                    msg.warn(
+                        "Found ignore marker in existing file: skipping", output_file
+                    )
+                    return
+
+            marker_tag_found = False
+            for marker_tag in MARKER_TAGS:
+                markers = {
+                    "start": MARKER_START.format(marker_tag),
+                    "end": MARKER_END.format(marker_tag),
+                }
+                if markers["start"] in existing and markers["end"] in existing:
+                    marker_tag_found = True
+                    msg.info("Found existing file: only replacing auto-generated docs")
+                    before = existing.split(markers["start"])[0]
+                    after = existing.split(markers["end"])[1]
+                    content = f"{before}{content}{after}"
+                    break
+            if not marker_tag_found:
                 msg.warn("Replacing existing file")
+
         with output_file.open("w", encoding="utf8") as f:
             f.write(content)
         msg.good("Saved project documentation", output_file)
```

### Comparing `weasel-0.1.1/weasel/cli/dvc.py` & `weasel-0.2.0/weasel/cli/dvc.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/cli/pull.py` & `weasel-0.2.0/weasel/cli/pull.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/cli/push.py` & `weasel-0.2.0/weasel/cli/push.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/cli/remote_storage.py` & `weasel-0.2.0/weasel/cli/remote_storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 from wasabi import msg
 
 from ..errors import Errors
 from ..util import check_spacy_env_vars, download_file, ensure_pathy, get_checksum
 from ..util import get_hash, make_tempdir, upload_file
 
 if TYPE_CHECKING:
-    from pathy import FluidPath
+    from cloudpathlib import CloudPath
 
 
 class RemoteStorage:
     """Push and pull outputs to and from a remote file storage.
 
     Remotes can be anything that `smart-open` can support: AWS, GCS, file system,
     ssh, etc.
     """
 
     def __init__(self, project_root: Path, url: str, *, compression="gz"):
         self.root = project_root
         self.url = ensure_pathy(url)
         self.compression = compression
 
-    def push(self, path: Path, command_hash: str, content_hash: str) -> "FluidPath":
+    def push(self, path: Path, command_hash: str, content_hash: str) -> "CloudPath":
         """Compress a file or directory within a project and upload it to a remote
         storage. If an object exists at the full URL, nothing is done.
 
         Within the remote storage, files are addressed by their project path
         (url encoded) and two user-supplied hashes, representing their creation
         context and their file contents. If the URL already exists, the data is
         not uploaded. Paths are archived and compressed prior to upload.
@@ -54,15 +54,15 @@
 
     def pull(
         self,
         path: Path,
         *,
         command_hash: Optional[str] = None,
         content_hash: Optional[str] = None,
-    ) -> Optional["FluidPath"]:
+    ) -> Optional["CloudPath"]:
         """Retrieve a file from the remote cache. If the file already exists,
         nothing is done.
 
         If the command_hash and/or content_hash are specified, only matching
         results are returned. If no results are available, an error is raised.
         """
         dest = self.root / path
@@ -104,15 +104,15 @@
 
     def find(
         self,
         path: Path,
         *,
         command_hash: Optional[str] = None,
         content_hash: Optional[str] = None,
-    ) -> Optional["FluidPath"]:
+    ) -> Optional["CloudPath"]:
         """Find the best matching version of a file within the storage,
         or `None` if no match can be found. If both the creation and content hash
         are specified, only exact matches will be returned. Otherwise, the most
         recent matching file is preferred.
         """
         name = self.encode_name(str(path))
         urls = []
@@ -126,23 +126,23 @@
             if (self.url / name).exists():
                 for sub_dir in (self.url / name).iterdir():
                     urls.extend(sub_dir.iterdir())
                 if content_hash is not None:
                     urls = [url for url in urls if url.parts[-1] == content_hash]
         if len(urls) >= 2:
             try:
-                urls.sort(key=lambda x: x.stat().last_modified)  # type: ignore
+                urls.sort(key=lambda x: x.stat().st_mtime)
             except Exception:
                 msg.warn(
                     "Unable to sort remote files by last modified. The file(s) "
                     "pulled from the cache may not be the most recent."
                 )
         return urls[-1] if urls else None
 
-    def make_url(self, path: Path, command_hash: str, content_hash: str) -> "FluidPath":
+    def make_url(self, path: Path, command_hash: str, content_hash: str) -> "CloudPath":
         """Construct a URL from a subpath, a creation hash and a content hash."""
         return self.url / self.encode_name(str(path)) / command_hash / content_hash
 
     def encode_name(self, name: str) -> str:
         """Encode a subpath into a URL-safe name."""
         return urllib.parse.quote_plus(name)
```

### Comparing `weasel-0.1.1/weasel/cli/run.py` & `weasel-0.2.0/weasel/cli/run.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/errors.py` & `weasel-0.2.0/weasel/errors.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/schemas.py` & `weasel-0.2.0/weasel/schemas.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from collections import defaultdict
 from typing import Any, Dict, List, Optional, Type, Union
 
-from pydantic import BaseModel, BaseSettings, Field, StrictStr, ValidationError
-from pydantic import root_validator
+try:
+    from pydantic.v1 import BaseModel, Field, StrictStr, ValidationError, root_validator
+except ImportError:
+    from pydantic import BaseModel, Field, StrictStr, ValidationError, root_validator  # type: ignore
+
 from wasabi import msg
 
 
 def validate(schema: Type[BaseModel], obj: Dict[str, Any]) -> List[str]:
     """Validate data against a given pydantic schema.
 
     obj (Dict[str, Any]): JSON-serializable data to validate.
@@ -86,25 +89,7 @@
     def check_legacy_keys(cls, obj: Dict[str, Any]) -> Dict[str, Any]:
         if "spacy_version" in obj:
             msg.warn(
                 "Your project configuration file includes a `spacy_version` key, "
                 "which is now deprecated. Weasel will not validate your version of spaCy.",
             )
         return obj
-
-
-class SpacyEnvVars(BaseSettings):
-    SPACY_CONFIG_OVERRIDES: Optional[str] = None
-    SPACY_PROJECT_USE_GIT_VERSION: Optional[bool] = None
-
-    def check(self):
-        if self.SPACY_CONFIG_OVERRIDES is not None:
-            msg.warn(
-                "You've set a `SPACY_CONFIG_OVERRIDES` environment variable, "
-                "which is now deprecated. Weasel will not use it. "
-                "You can use `WEASEL_CONFIG_OVERRIDES` instead."
-            )
-        if self.SPACY_PROJECT_USE_GIT_VERSION is not None:
-            msg.warn(
-                "You've set a `SPACY_PROJECT_USE_GIT_VERSION` environment variable, "
-                "which is now deprecated. Weasel will not use it."
-            )
```

### Comparing `weasel-0.1.1/weasel/tests/cli/test_cli.py` & `weasel-0.2.0/weasel/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/tests/cli/test_cli_app.py` & `weasel-0.2.0/weasel/tests/cli/test_cli_app.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/tests/cli/test_remote.py` & `weasel-0.2.0/weasel/tests/cli/test_remote.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/tests/test_schemas.py` & `weasel-0.2.0/weasel/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/tests/test_validation.py` & `weasel-0.2.0/weasel/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/tests/util.py` & `weasel-0.2.0/weasel/tests/util.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/util/__init__.py` & `weasel-0.2.0/weasel/util/__init__.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/util/commands.py` & `weasel-0.2.0/weasel/util/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             stdout=subprocess.PIPE if capture else None,
             stderr=subprocess.STDOUT if capture else None,
         )
     except FileNotFoundError:
         # Indicates the *command* wasn't found, it's an error before the command
         # is run.
         raise FileNotFoundError(
-            Errors.E970.format(str_command=cmd_str, tool=cmd_list[0])
+            Errors.E501.format(str_command=cmd_str, tool=cmd_list[0])
         ) from None
     if ret.returncode != 0 and capture:
         message = f"Error running command:\n\n{cmd_str}\n\n"
         message += f"Subprocess exited with status {ret.returncode}"
         if ret.stdout is not None:
             message += "\n\nProcess log (stdout and stderr):\n\n"
             message += ret.stdout
```

### Comparing `weasel-0.1.1/weasel/util/config.py` & `weasel-0.2.0/weasel/util/config.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/util/filesystem.py` & `weasel-0.2.0/weasel/util/filesystem.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,17 +70,17 @@
     else:
         return path
 
 
 def ensure_pathy(path):
     """Temporary helper to prevent importing Pathy globally (which can cause
     slow and annoying Google Cloud warning)."""
-    from pathy import Pathy  # noqa: F811
+    from cloudpathlib import AnyPath  # noqa: F811
 
-    return Pathy.fluid(path)
+    return AnyPath(path)
 
 
 def is_subpath_of(parent, child):
     """
     Check whether `child` is a path contained within `parent`.
     """
     # Based on https://stackoverflow.com/a/37095733 .
```

### Comparing `weasel-0.1.1/weasel/util/frozen.py` & `weasel-0.2.0/weasel/util/frozen.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/util/git.py` & `weasel-0.2.0/weasel/util/git.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/util/hashing.py` & `weasel-0.2.0/weasel/util/hashing.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/util/modules.py` & `weasel-0.2.0/weasel/util/modules.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/util/remote.py` & `weasel-0.2.0/weasel/util/remote.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import shutil
 from pathlib import Path
 from typing import TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
-    from pathy import FluidPath
+    from cloudpathlib import CloudPath
 
 
-def upload_file(src: Path, dest: Union[str, "FluidPath"]) -> None:
+def upload_file(src: Path, dest: Union[str, "CloudPath"]) -> None:
     """Upload a file.
 
     src (Path): The source path.
     url (str): The destination URL to upload to.
     """
     import smart_open
 
@@ -22,15 +22,15 @@
     dest = str(dest)
     with smart_open.open(dest, mode="wb") as output_file:
         with src.open(mode="rb") as input_file:
             output_file.write(input_file.read())
 
 
 def download_file(
-    src: Union[str, "FluidPath"], dest: Path, *, force: bool = False
+    src: Union[str, "CloudPath"], dest: Path, *, force: bool = False
 ) -> None:
     """Download a file using smart_open.
 
     url (str): The URL of the file.
     dest (Path): The destination path.
     force (bool): Whether to force download even if file exists.
         If False, the download will be skipped.
```

### Comparing `weasel-0.1.1/weasel/util/validation.py` & `weasel-0.2.0/weasel/util/validation.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel/util/versions.py` & `weasel-0.2.0/weasel/util/versions.py`

 * *Files identical despite different names*

### Comparing `weasel-0.1.1/weasel.egg-info/PKG-INFO` & `weasel-0.2.0/weasel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: weasel
-Version: 0.1.1
+Version: 0.2.0
 Summary: Weasel: A small and easy workflow system
 Home-page: https://github.com/explosion/weasel/
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Project-URL: Release notes, https://github.com/explosion/weasel/releases
 Project-URL: Source, https://github.com/explosion/weasel/
@@ -17,14 +17,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a href="https://explosion.ai"><img src="https://explosion.ai/assets/img/logo.svg" width="125" height="125" align="right" /></a>
 
 # Weasel: A small and easy workflow system
```

#### html2text {}

```diff
@@ -1,35 +1,36 @@
-Metadata-Version: 2.1 Name: weasel Version: 0.1.1 Summary: Weasel: A small and
+Metadata-Version: 2.1 Name: weasel Version: 0.2.0 Summary: Weasel: A small and
 easy workflow system Home-page: https://github.com/explosion/weasel/ Author:
 Explosion Author-email: contact@explosion.ai License: MIT Project-URL: Release
 notes, https://github.com/explosion/weasel/releases Project-URL: Source, https:
 //github.com/explosion/weasel/ Classifier: Environment :: Console Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: Science/
 Research Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: MacOS ::
 MacOS X Classifier: Operating System :: Microsoft :: Windows Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Scientific/Engineering Description-Content-
-Type: text/markdown License-File: LICENSE [https://explosion.ai/assets/img/
-logo.svg] # Weasel: A small and easy workflow system Weasel lets you manage and
-share **end-to-end workflows** for different **use cases and domains**, and
-orchestrate training, packaging and serving your custom pipelines. You can
-start off by cloning a pre-defined project template, adjust it to fit your
-needs, load in your data, train a pipeline, export it as a Python package,
-upload your outputs to a remote storage and share your results with your team.
-Weasel can be used via the [`weasel`](https://github.com/explosion/weasel/blob/
-main/docs/cli.md) command and we provide templates in our [`projects`](https://
-github.com/explosion/projects) repo. ![Illustration of project workflow and
-commands](https://raw.githubusercontent.com/explosion/weasel/main/docs/assets/
-images/projects.svg) ## ð¡ Example: Get started with a project template The
-easiest way to get started is to clone a project template and run it âÂ for
-example, this [end-to-end template](https://github.com/explosion/projects/tree/
-v3/pipelines/tagger_parser_ud) that lets you train a spaCy **part-of-speech
+Python :: 3.11 Classifier: Topic :: Scientific/Engineering Requires-Python:
+>=3.6 Description-Content-Type: text/markdown License-File: LICENSE [https://
+explosion.ai/assets/img/logo.svg] # Weasel: A small and easy workflow system
+Weasel lets you manage and share **end-to-end workflows** for different **use
+cases and domains**, and orchestrate training, packaging and serving your
+custom pipelines. You can start off by cloning a pre-defined project template,
+adjust it to fit your needs, load in your data, train a pipeline, export it as
+a Python package, upload your outputs to a remote storage and share your
+results with your team. Weasel can be used via the [`weasel`](https://
+github.com/explosion/weasel/blob/main/docs/cli.md) command and we provide
+templates in our [`projects`](https://github.com/explosion/projects) repo. !
+[Illustration of project workflow and commands](https://
+raw.githubusercontent.com/explosion/weasel/main/docs/assets/images/
+projects.svg) ## ð¡ Example: Get started with a project template The easiest
+way to get started is to clone a project template and run it âÂ for example,
+this [end-to-end template](https://github.com/explosion/projects/tree/v3/
+pipelines/tagger_parser_ud) that lets you train a spaCy **part-of-speech
 tagger** and **dependency parser** on a Universal Dependencies treebank.
 ```shell python -m weasel clone pipelines/tagger_parser_ud ``` > **Note** > >
 Our [`projects`](https://github.com/explosion/projects) repo includes various >
 project templates for different NLP tasks, models, workflows and integrations >
 that you can clone and run. The easiest way to get started is to pick a >
 template, clone it and start modifying it! ## ð Documentation Get started
 with the documentation: - [Learn how to create a Weasel workflow](https://
```

### Comparing `weasel-0.1.1/weasel.egg-info/SOURCES.txt` & `weasel-0.2.0/weasel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

