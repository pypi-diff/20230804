# Comparing `tmp/mkdocs-autolinks-plugin-0.7.0.tar.gz` & `tmp/mkdocs-autolinks-plugin-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-autolinks-plugin-0.7.0.tar", last modified: Mon Feb 27 16:43:09 2023, max compression
+gzip compressed data, was "mkdocs-autolinks-plugin-0.7.1.tar", last modified: Fri Aug  4 14:42:06 2023, max compression
```

## Comparing `mkdocs-autolinks-plugin-0.7.0.tar` & `mkdocs-autolinks-plugin-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 zhannum    (501) staff       (20)        0 2023-02-27 16:43:09.676621 mkdocs-autolinks-plugin-0.7.0/
--rw-r--r--   0 zhannum    (501) staff       (20)     1056 2023-02-27 16:24:42.000000 mkdocs-autolinks-plugin-0.7.0/LICENSE
--rw-r--r--   0 zhannum    (501) staff       (20)      970 2023-02-27 16:43:09.676693 mkdocs-autolinks-plugin-0.7.0/PKG-INFO
--rw-r--r--   0 zhannum    (501) staff       (20)     1970 2023-02-27 16:37:39.000000 mkdocs-autolinks-plugin-0.7.0/README.md
-drwxr-xr-x   0 zhannum    (501) staff       (20)        0 2023-02-27 16:43:09.675540 mkdocs-autolinks-plugin-0.7.0/mkdocs_autolinks_plugin/
--rw-r--r--   0 zhannum    (501) staff       (20)        0 2023-02-27 16:24:42.000000 mkdocs-autolinks-plugin-0.7.0/mkdocs_autolinks_plugin/__init__.py
--rw-r--r--   0 zhannum    (501) staff       (20)     3451 2023-02-27 16:37:39.000000 mkdocs-autolinks-plugin-0.7.0/mkdocs_autolinks_plugin/plugin.py
-drwxr-xr-x   0 zhannum    (501) staff       (20)        0 2023-02-27 16:43:09.676487 mkdocs-autolinks-plugin-0.7.0/mkdocs_autolinks_plugin.egg-info/
--rw-r--r--   0 zhannum    (501) staff       (20)      970 2023-02-27 16:43:09.000000 mkdocs-autolinks-plugin-0.7.0/mkdocs_autolinks_plugin.egg-info/PKG-INFO
--rw-r--r--   0 zhannum    (501) staff       (20)      390 2023-02-27 16:43:09.000000 mkdocs-autolinks-plugin-0.7.0/mkdocs_autolinks_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 zhannum    (501) staff       (20)        1 2023-02-27 16:43:09.000000 mkdocs-autolinks-plugin-0.7.0/mkdocs_autolinks_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 zhannum    (501) staff       (20)       76 2023-02-27 16:43:09.000000 mkdocs-autolinks-plugin-0.7.0/mkdocs_autolinks_plugin.egg-info/entry_points.txt
--rw-r--r--   0 zhannum    (501) staff       (20)       14 2023-02-27 16:43:09.000000 mkdocs-autolinks-plugin-0.7.0/mkdocs_autolinks_plugin.egg-info/requires.txt
--rw-r--r--   0 zhannum    (501) staff       (20)       24 2023-02-27 16:43:09.000000 mkdocs-autolinks-plugin-0.7.0/mkdocs_autolinks_plugin.egg-info/top_level.txt
--rw-r--r--   0 zhannum    (501) staff       (20)       79 2023-02-27 16:43:09.677494 mkdocs-autolinks-plugin-0.7.0/setup.cfg
--rw-r--r--   0 zhannum    (501) staff       (20)     1297 2023-02-27 16:38:14.000000 mkdocs-autolinks-plugin-0.7.0/setup.py
+drwxr-xr-x   0 zhannum    (501) staff       (20)        0 2023-08-04 14:42:06.151785 mkdocs-autolinks-plugin-0.7.1/
+-rw-r--r--   0 zhannum    (501) staff       (20)     1056 2023-02-27 16:24:42.000000 mkdocs-autolinks-plugin-0.7.1/LICENSE
+-rw-r--r--   0 zhannum    (501) staff       (20)      970 2023-08-04 14:42:06.151855 mkdocs-autolinks-plugin-0.7.1/PKG-INFO
+-rw-r--r--   0 zhannum    (501) staff       (20)     1970 2023-02-27 16:37:39.000000 mkdocs-autolinks-plugin-0.7.1/README.md
+drwxr-xr-x   0 zhannum    (501) staff       (20)        0 2023-08-04 14:42:06.150916 mkdocs-autolinks-plugin-0.7.1/mkdocs_autolinks_plugin/
+-rw-r--r--   0 zhannum    (501) staff       (20)        0 2023-02-27 16:24:42.000000 mkdocs-autolinks-plugin-0.7.1/mkdocs_autolinks_plugin/__init__.py
+-rw-r--r--   0 zhannum    (501) staff       (20)     3381 2023-08-04 14:39:29.000000 mkdocs-autolinks-plugin-0.7.1/mkdocs_autolinks_plugin/plugin.py
+drwxr-xr-x   0 zhannum    (501) staff       (20)        0 2023-08-04 14:42:06.151672 mkdocs-autolinks-plugin-0.7.1/mkdocs_autolinks_plugin.egg-info/
+-rw-r--r--   0 zhannum    (501) staff       (20)      970 2023-08-04 14:42:06.000000 mkdocs-autolinks-plugin-0.7.1/mkdocs_autolinks_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 zhannum    (501) staff       (20)      390 2023-08-04 14:42:06.000000 mkdocs-autolinks-plugin-0.7.1/mkdocs_autolinks_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 zhannum    (501) staff       (20)        1 2023-08-04 14:42:06.000000 mkdocs-autolinks-plugin-0.7.1/mkdocs_autolinks_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 zhannum    (501) staff       (20)       76 2023-08-04 14:42:06.000000 mkdocs-autolinks-plugin-0.7.1/mkdocs_autolinks_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 zhannum    (501) staff       (20)       14 2023-08-04 14:42:06.000000 mkdocs-autolinks-plugin-0.7.1/mkdocs_autolinks_plugin.egg-info/requires.txt
+-rw-r--r--   0 zhannum    (501) staff       (20)       24 2023-08-04 14:42:06.000000 mkdocs-autolinks-plugin-0.7.1/mkdocs_autolinks_plugin.egg-info/top_level.txt
+-rw-r--r--   0 zhannum    (501) staff       (20)       79 2023-08-04 14:42:06.152073 mkdocs-autolinks-plugin-0.7.1/setup.cfg
+-rw-r--r--   0 zhannum    (501) staff       (20)     1297 2023-08-04 14:40:33.000000 mkdocs-autolinks-plugin-0.7.1/setup.py
```

### Comparing `mkdocs-autolinks-plugin-0.7.0/LICENSE` & `mkdocs-autolinks-plugin-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-autolinks-plugin-0.7.0/PKG-INFO` & `mkdocs-autolinks-plugin-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mkdocs-autolinks-plugin
-Version: 0.7.0
+Version: 0.7.1
 Summary: An MkDocs plugin
 Home-page: https://github.com/midnightprioriem/mkdocs-autolinks-plugin
-Download-URL: https://github.com/midnightprioriem/mkdocs-autolinks-plugin/archive/v_070.tar.gz
+Download-URL: https://github.com/midnightprioriem/mkdocs-autolinks-plugin/archive/v_071.tar.gz
 Author: Zach Hannum
 Author-email: zacharyhannum@gmail.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `mkdocs-autolinks-plugin-0.7.0/README.md` & `mkdocs-autolinks-plugin-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-autolinks-plugin-0.7.0/mkdocs_autolinks_plugin/plugin.py` & `mkdocs-autolinks-plugin-0.7.1/mkdocs_autolinks_plugin/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 import pathlib
 import re
 from urllib.parse import quote
 import logging
 from collections import defaultdict
 
 from mkdocs.plugins import BasePlugin
-from mkdocs.utils import warning_filter
 
 LOG = logging.getLogger("mkdocs.plugins." + __name__)
-LOG.addFilter(warning_filter)
 
 # For Regex, match groups are:
 #       0: Whole markdown link e.g. [Alt-text](url)
 #       1: Alt text
 #       2: Full URL e.g. url + hash anchor
 #       3: Filename e.g. filename.md
 #       4: File extension e.g. .md, .png, etc.
```

### Comparing `mkdocs-autolinks-plugin-0.7.0/mkdocs_autolinks_plugin.egg-info/PKG-INFO` & `mkdocs-autolinks-plugin-0.7.1/mkdocs_autolinks_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mkdocs-autolinks-plugin
-Version: 0.7.0
+Version: 0.7.1
 Summary: An MkDocs plugin
 Home-page: https://github.com/midnightprioriem/mkdocs-autolinks-plugin
-Download-URL: https://github.com/midnightprioriem/mkdocs-autolinks-plugin/archive/v_070.tar.gz
+Download-URL: https://github.com/midnightprioriem/mkdocs-autolinks-plugin/archive/v_071.tar.gz
 Author: Zach Hannum
 Author-email: zacharyhannum@gmail.com
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

### Comparing `mkdocs-autolinks-plugin-0.7.0/setup.py` & `mkdocs-autolinks-plugin-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-autolinks-plugin',
-    version='0.7.0',
+    version='0.7.1',
     description='An MkDocs plugin',
     long_description='An MkDocs plugin that automagically generates relative links between markdown pages',
     keywords='mkdocs',
     url='https://github.com/midnightprioriem/mkdocs-autolinks-plugin',
-    download_url='https://github.com/midnightprioriem/mkdocs-autolinks-plugin/archive/v_070.tar.gz',
+    download_url='https://github.com/midnightprioriem/mkdocs-autolinks-plugin/archive/v_071.tar.gz',
     author='Zach Hannum',
     author_email='zacharyhannum@gmail.com',
     license='MIT',
     python_requires='>=3.4',
     install_requires=[
         'mkdocs>=1.2.3',
     ],
```

