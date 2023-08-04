# Comparing `tmp/mkdocs_pymdownx_material_extras-2.5.tar.gz` & `tmp/mkdocs_pymdownx_material_extras-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_pymdownx_material_extras-2.5.tar", last modified: Thu Jul 27 01:48:22 2023, max compression
+gzip compressed data, was "mkdocs_pymdownx_material_extras-2.5.1.tar", last modified: Fri Aug  4 03:45:05 2023, max compression
```

## Comparing `mkdocs_pymdownx_material_extras-2.5.tar` & `mkdocs_pymdownx_material_extras-2.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:48:22.797864 mkdocs_pymdownx_material_extras-2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-27 01:48:22.797864 mkdocs_pymdownx_material_extras-2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:48:22.797864 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/__meta__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:48:22.797864 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:48:22.793864 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:48:22.797864 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/
--rw-r--r--   0 runner    (1001) docker     (123)    68921 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/extra-ba994a2e31.css
--rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/extra-loader-11e3a2e3.js
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/material-extra-3rdparty-a81e7739.js
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/material-extra-theme-8d50d708.js
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:48:22.797864 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/partials/
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/partials/footer.html
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/partials/header.html
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/partials/libs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:48:22.797864 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-07-27 01:48:22.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-27 01:48:22.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 01:48:22.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-27 01:48:22.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 01:48:22.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-27 01:48:22.000000 mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:48:22.797864 mkdocs_pymdownx_material_extras-2.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/requirements/project.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-27 01:48:22.797864 mkdocs_pymdownx_material_extras-2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-27 01:48:19.000000 mkdocs_pymdownx_material_extras-2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:45:05.505073 mkdocs_pymdownx_material_extras-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-08-04 03:45:05.505073 mkdocs_pymdownx_material_extras-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:45:05.501073 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/__meta__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:45:05.505073 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:45:05.501073 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:45:05.505073 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/
+-rw-r--r--   0 runner    (1001) docker     (123)    68921 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/extra-ba994a2e31.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6244 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/extra-loader-11e3a2e3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/material-extra-3rdparty-a81e7739.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/material-extra-theme-8d50d708.js
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:45:05.505073 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/partials/
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/partials/footer.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/partials/header.html
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/partials/libs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:45:05.501073 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-08-04 03:45:05.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-08-04 03:45:05.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 03:45:05.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-04 03:45:05.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 03:45:05.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 03:45:05.000000 mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 03:45:05.505073 mkdocs_pymdownx_material_extras-2.5.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/requirements/project.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-04 03:45:05.505073 mkdocs_pymdownx_material_extras-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-08-04 03:45:01.000000 mkdocs_pymdownx_material_extras-2.5.1/setup.py
```

### Comparing `mkdocs_pymdownx_material_extras-2.5/LICENSE.md` & `mkdocs_pymdownx_material_extras-2.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocs_pymdownx_material_extras-2.5/PKG-INFO` & `mkdocs_pymdownx_material_extras-2.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs_pymdownx_material_extras
-Version: 2.5
+Version: 2.5.1
 Summary: Plugin to extend MkDocs Material theme.
 Home-page: https://github.com/facelessuser/mkdocs_pymdownx_material_extras
 Author: Isaac Muse
 Author-email: Isaac.Muse@gmail.com
 License: MIT License
 Keywords: mkdocs plugin material
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs_pymdownx_material_extras-2.5/README.md` & `mkdocs_pymdownx_material_extras-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/__init__.py` & `mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,17 @@
             name = f.replace('\\', '/').replace(base_path, '')
             if name not in extras:
                 config['extra_css'].append(name)
 
         if MKDOCS_150:
             from mkdocs.config.config_options import ExtraScriptValue
 
-            extras = set(script.path for script in config['extra_javascript'])
+            extras = set(
+                script.path if not isinstance(script, str) else script for script in config['extra_javascript']
+            )
             for f in glob.glob(base_path + '**/extra*.js', recursive=True):
                 name = f.replace('\\', '/').replace(base_path, '')
                 if name not in extras:
                     config['extra_javascript'].append(ExtraScriptValue(name))
         else:
             extras = set(config['extra_javascript'])
             for f in glob.glob(base_path + '**/extra*.js', recursive=True):
```

### Comparing `mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/__meta__.py` & `mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/__meta__.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,9 +181,9 @@
 
     # Handle post
     post = int(m.group('post')) if m.group('post') else 0
 
     return Version(major, minor, micro, release, pre, post, dev)
 
 
-__version_info__ = Version(2, 5, 0, "final")
+__version_info__ = Version(2, 5, 1, "final")
 __version__ = __version_info__._get_canonical()
```

### Comparing `mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/extra-ba994a2e31.css` & `mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/extra-ba994a2e31.css`

 * *Files identical despite different names*

### Comparing `mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/extra-loader-11e3a2e3.js` & `mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/extra-loader-11e3a2e3.js`

 * *Files identical despite different names*

### Comparing `mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/material-extra-3rdparty-a81e7739.js` & `mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/material-extra-3rdparty-a81e7739.js`

 * *Files identical despite different names*

### Comparing `mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/material-extra-theme-8d50d708.js` & `mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/assets/pymdownx-extras/material-extra-theme-8d50d708.js`

 * *Files identical despite different names*

### Comparing `mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/main.html` & `mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/main.html`

 * *Files identical despite different names*

### Comparing `mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/partials/footer.html` & `mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/partials/footer.html`

 * *Files identical despite different names*

### Comparing `mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras/theme/partials/header.html` & `mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras/theme/partials/header.html`

 * *Files identical despite different names*

### Comparing `mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras.egg-info/PKG-INFO` & `mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-pymdownx-material-extras
-Version: 2.5
+Version: 2.5.1
 Summary: Plugin to extend MkDocs Material theme.
 Home-page: https://github.com/facelessuser/mkdocs_pymdownx_material_extras
 Author: Isaac Muse
 Author-email: Isaac.Muse@gmail.com
 License: MIT License
 Keywords: mkdocs plugin material
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mkdocs_pymdownx_material_extras-2.5/mkdocs_pymdownx_material_extras.egg-info/SOURCES.txt` & `mkdocs_pymdownx_material_extras-2.5.1/mkdocs_pymdownx_material_extras.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs_pymdownx_material_extras-2.5/setup.py` & `mkdocs_pymdownx_material_extras-2.5.1/setup.py`

 * *Files identical despite different names*

