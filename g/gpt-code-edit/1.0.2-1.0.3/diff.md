# Comparing `tmp/gpt-code-edit-1.0.2.tar.gz` & `tmp/gpt-code-edit-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-code-edit-1.0.2.tar", last modified: Fri Aug  4 14:16:59 2023, max compression
+gzip compressed data, was "gpt-code-edit-1.0.3.tar", last modified: Fri Aug  4 14:24:06 2023, max compression
```

## Comparing `gpt-code-edit-1.0.2.tar` & `gpt-code-edit-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 14:16:59.174688 gpt-code-edit-1.0.2/
--rw-rw-rw-   0        0        0     5492 2023-08-04 14:16:59.172671 gpt-code-edit-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4676 2023-08-04 14:13:07.000000 gpt-code-edit-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 14:16:59.102671 gpt-code-edit-1.0.2/chatgpt_cli/
--rw-rw-rw-   0        0        0        0 2023-08-04 09:45:39.000000 gpt-code-edit-1.0.2/chatgpt_cli/__init__.py
--rw-rw-rw-   0        0        0     7541 2023-08-04 09:31:34.000000 gpt-code-edit-1.0.2/chatgpt_cli/arguement_validator.py
--rw-rw-rw-   0        0        0    11011 2023-07-19 16:18:28.000000 gpt-code-edit-1.0.2/chatgpt_cli/code_parser.py
--rw-rw-rw-   0        0        0     6467 2023-08-04 13:43:04.000000 gpt-code-edit-1.0.2/chatgpt_cli/gpt_request.py
--rw-rw-rw-   0        0        0     1061 2023-08-04 13:58:33.000000 gpt-code-edit-1.0.2/chatgpt_cli/main.py
-drwxrwxrwx   0        0        0        0 2023-08-04 14:16:59.166668 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/
--rw-rw-rw-   0        0        0     5492 2023-08-04 14:16:58.000000 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-08-04 14:16:59.000000 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 14:16:58.000000 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-08-04 14:16:58.000000 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       66 2023-08-04 14:16:58.000000 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-04 14:16:58.000000 gpt-code-edit-1.0.2/gpt_code_edit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 14:16:59.175670 gpt-code-edit-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1313 2023-08-04 14:16:52.000000 gpt-code-edit-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:24:06.192075 gpt-code-edit-1.0.3/
+-rw-rw-rw-   0        0        0     5492 2023-08-04 14:24:06.191073 gpt-code-edit-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4676 2023-08-04 14:13:07.000000 gpt-code-edit-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 14:24:06.118073 gpt-code-edit-1.0.3/chatgpt_cli/
+-rw-rw-rw-   0        0        0        0 2023-08-04 09:45:39.000000 gpt-code-edit-1.0.3/chatgpt_cli/__init__.py
+-rw-rw-rw-   0        0        0     7541 2023-08-04 09:31:34.000000 gpt-code-edit-1.0.3/chatgpt_cli/arguement_validator.py
+-rw-rw-rw-   0        0        0    11011 2023-07-19 16:18:28.000000 gpt-code-edit-1.0.3/chatgpt_cli/code_parser.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:24:06.135071 gpt-code-edit-1.0.3/chatgpt_cli/commands/
+-rw-rw-rw-   0        0        0        0 2023-08-04 14:23:06.000000 gpt-code-edit-1.0.3/chatgpt_cli/commands/__init__.py
+-rw-rw-rw-   0        0        0     6609 2023-08-04 14:02:44.000000 gpt-code-edit-1.0.3/chatgpt_cli/commands/code_edit.py
+-rw-rw-rw-   0        0        0     3393 2023-08-04 14:03:26.000000 gpt-code-edit-1.0.3/chatgpt_cli/commands/review_to_file.py
+-rw-rw-rw-   0        0        0     1090 2023-08-04 13:42:38.000000 gpt-code-edit-1.0.3/chatgpt_cli/commands/set_api_key.py
+-rw-rw-rw-   0        0        0     6467 2023-08-04 13:43:04.000000 gpt-code-edit-1.0.3/chatgpt_cli/gpt_request.py
+-rw-rw-rw-   0        0        0     1061 2023-08-04 13:58:33.000000 gpt-code-edit-1.0.3/chatgpt_cli/main.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:24:06.186072 gpt-code-edit-1.0.3/gpt_code_edit.egg-info/
+-rw-rw-rw-   0        0        0     5492 2023-08-04 14:24:05.000000 gpt-code-edit-1.0.3/gpt_code_edit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-08-04 14:24:06.000000 gpt-code-edit-1.0.3/gpt_code_edit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 14:24:05.000000 gpt-code-edit-1.0.3/gpt_code_edit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-04 14:24:06.000000 gpt-code-edit-1.0.3/gpt_code_edit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-08-04 14:24:06.000000 gpt-code-edit-1.0.3/gpt_code_edit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-04 14:24:06.000000 gpt-code-edit-1.0.3/gpt_code_edit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 14:24:06.193071 gpt-code-edit-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1313 2023-08-04 14:23:55.000000 gpt-code-edit-1.0.3/setup.py
```

### Comparing `gpt-code-edit-1.0.2/PKG-INFO` & `gpt-code-edit-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-code-edit
-Version: 1.0.2
+Version: 1.0.3
 Summary: A command line interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits including refactoring, adding comments, adding docstrings, or adding error handling.
 Home-page: https://github.com/ben-23-96/chatgpt_code_improve_cli
 Author: Ben Speakman
 Author-email: benspeakman23@yahoo.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gpt-code-edit-1.0.2/README.md` & `gpt-code-edit-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gpt-code-edit-1.0.2/chatgpt_cli/arguement_validator.py` & `gpt-code-edit-1.0.3/chatgpt_cli/arguement_validator.py`

 * *Files identical despite different names*

### Comparing `gpt-code-edit-1.0.2/chatgpt_cli/code_parser.py` & `gpt-code-edit-1.0.3/chatgpt_cli/code_parser.py`

 * *Files identical despite different names*

### Comparing `gpt-code-edit-1.0.2/chatgpt_cli/gpt_request.py` & `gpt-code-edit-1.0.3/chatgpt_cli/gpt_request.py`

 * *Files identical despite different names*

### Comparing `gpt-code-edit-1.0.2/chatgpt_cli/main.py` & `gpt-code-edit-1.0.3/chatgpt_cli/main.py`

 * *Files identical despite different names*

### Comparing `gpt-code-edit-1.0.2/gpt_code_edit.egg-info/PKG-INFO` & `gpt-code-edit-1.0.3/gpt_code_edit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-code-edit
-Version: 1.0.2
+Version: 1.0.3
 Summary: A command line interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits including refactoring, adding comments, adding docstrings, or adding error handling.
 Home-page: https://github.com/ben-23-96/chatgpt_code_improve_cli
 Author: Ben Speakman
 Author-email: benspeakman23@yahoo.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gpt-code-edit-1.0.2/setup.py` & `gpt-code-edit-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="gpt-code-edit",
-    version="1.0.2",
+    version="1.0.3",
     packages=find_packages(),
 
     # Metadata
     author="Ben Speakman",
     author_email="benspeakman23@yahoo.com",
     description="A command line interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits including refactoring, adding comments, adding docstrings, or adding error handling.",
     long_description=open('README.md').read(),
```

