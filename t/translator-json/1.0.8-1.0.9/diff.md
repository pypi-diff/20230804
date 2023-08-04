# Comparing `tmp/translator_json-1.0.8.tar.gz` & `tmp/translator_json-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translator_json-1.0.8.tar", last modified: Sun Jun 25 05:08:19 2023, max compression
+gzip compressed data, was "translator_json-1.0.9.tar", last modified: Fri Aug  4 15:38:54 2023, max compression
```

## Comparing `translator_json-1.0.8.tar` & `translator_json-1.0.9.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:08:19.524297 translator_json-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)       52 2023-06-25 05:08:07.000000 translator_json-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2271 2023-06-25 05:08:19.525297 translator_json-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1732 2023-06-25 05:08:07.000000 translator_json-1.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-06-25 05:08:07.000000 translator_json-1.0.8/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      198 2023-06-25 05:08:19.525297 translator_json-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-06-25 05:08:07.000000 translator_json-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:08:19.525297 translator_json-1.0.8/translator/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-06-25 05:08:07.000000 translator_json-1.0.8/translator/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-25 05:08:19.525297 translator_json-1.0.8/translator/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     4868 2023-06-25 05:08:07.000000 translator_json-1.0.8/translator/translate_generator.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-25 05:08:19.524297 translator_json-1.0.8/translator_json.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2271 2023-06-25 05:08:19.000000 translator_json-1.0.8/translator_json.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      387 2023-06-25 05:08:19.000000 translator_json-1.0.8/translator_json.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-25 05:08:19.000000 translator_json-1.0.8/translator_json.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2023-06-25 05:08:19.000000 translator_json-1.0.8/translator_json.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      106 2023-06-25 05:08:19.000000 translator_json-1.0.8/translator_json.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-25 05:08:19.000000 translator_json-1.0.8/translator_json.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)    83021 2023-06-25 05:08:07.000000 translator_json-1.0.8/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:38:54.265612 translator_json-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)       86 2023-08-04 15:38:36.000000 translator_json-1.0.9/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-08-04 15:38:36.000000 translator_json-1.0.9/.gitlab-ci.yml
+-rw-r--r--   0 root         (0) root         (0)     2209 2023-08-04 15:38:54.265612 translator_json-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1732 2023-08-04 15:38:36.000000 translator_json-1.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      975 2023-08-04 15:38:36.000000 translator_json-1.0.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-08-04 15:38:36.000000 translator_json-1.0.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 15:38:54.265612 translator_json-1.0.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:38:54.262612 translator_json-1.0.9/translator/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-04 15:38:36.000000 translator_json-1.0.9/translator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4475 2023-08-04 15:38:36.000000 translator_json-1.0.9/translator/glossary.py
+-rw-rw-rw-   0 root         (0) root         (0)     8381 2023-08-04 15:38:36.000000 translator_json-1.0.9/translator/translate_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)      514 2023-08-04 15:38:36.000000 translator_json-1.0.9/translator/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 15:38:54.264612 translator_json-1.0.9/translator_json.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2209 2023-08-04 15:38:54.000000 translator_json-1.0.9/translator_json.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      403 2023-08-04 15:38:54.000000 translator_json-1.0.9/translator_json.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 15:38:54.000000 translator_json-1.0.9/translator_json.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      149 2023-08-04 15:38:54.000000 translator_json-1.0.9/translator_json.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      115 2023-08-04 15:38:54.000000 translator_json-1.0.9/translator_json.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-08-04 15:38:54.000000 translator_json-1.0.9/translator_json.egg-info/top_level.txt
```

### Comparing `translator_json-1.0.8/PKG-INFO` & `translator_json-1.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: translator_json
-Version: 1.0.8
+Version: 1.0.9
 Summary: A translator for Json info
-Home-page: https://gitlab.com/FlorentSimonnot1/translator
-Author: Florent Simonnot
-Author-email: contact@gwanly.fr
-License: UNKNOWN
-Project-URL: Source, https://gitlab.com/FlorentSimonnot1/translator
-Platform: UNKNOWN
+Author-email: Florent Simonnot <contact@gwanly.com>
+License: Apache Software License
+Project-URL: Repository, https://gitlab.com/FlorentSimonnot1/translator
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # The Translator
 
 ## Why this plugin
 
@@ -87,8 +84,7 @@
 ### List available languages
 
     json_translator -a
 
 ## Examples
 
     json_translator -c googlekey.json -i fr.json -o ./myPath/ -l en,de,ko,it,es
-
```

### Comparing `translator_json-1.0.8/README.md` & `translator_json-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `translator_json-1.0.8/translator_json.egg-info/PKG-INFO` & `translator_json-1.0.9/translator_json.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 Metadata-Version: 2.1
 Name: translator-json
-Version: 1.0.8
+Version: 1.0.9
 Summary: A translator for Json info
-Home-page: https://gitlab.com/FlorentSimonnot1/translator
-Author: Florent Simonnot
-Author-email: contact@gwanly.fr
-License: UNKNOWN
-Project-URL: Source, https://gitlab.com/FlorentSimonnot1/translator
-Platform: UNKNOWN
+Author-email: Florent Simonnot <contact@gwanly.com>
+License: Apache Software License
+Project-URL: Repository, https://gitlab.com/FlorentSimonnot1/translator
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # The Translator
 
 ## Why this plugin
 
@@ -87,8 +84,7 @@
 ### List available languages
 
     json_translator -a
 
 ## Examples
 
     json_translator -c googlekey.json -i fr.json -o ./myPath/ -l en,de,ko,it,es
-
```

