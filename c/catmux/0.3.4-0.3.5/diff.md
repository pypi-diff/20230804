# Comparing `tmp/catmux-0.3.4.tar.gz` & `tmp/catmux-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catmux-0.3.4.tar", last modified: Sat Jul 22 23:01:28 2023, max compression
+gzip compressed data, was "catmux-0.3.5.tar", last modified: Fri Aug  4 19:48:46 2023, max compression
```

## Comparing `catmux-0.3.4.tar` & `catmux-0.3.5.tar`

### file list

```diff
@@ -1,33 +1,40 @@
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-07-22 23:01:28.309641 catmux-0.3.4/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1068 2023-04-04 19:35:47.000000 catmux-0.3.4/LICENSE
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     6358 2023-07-22 23:01:28.309641 catmux-0.3.4/PKG-INFO
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     5927 2023-07-22 21:14:37.000000 catmux-0.3.4/README.md
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-07-22 23:01:28.305641 catmux-0.3.4/catmux/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2023-04-04 19:35:47.000000 catmux-0.3.4/catmux/__init__.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1984 2023-07-22 20:22:49.000000 catmux-0.3.4/catmux/example_session.yaml
--rw-rw-r--   0 mauch     (1000) mauch     (1000)      210 2023-07-21 15:13:50.000000 catmux-0.3.4/catmux/exceptions.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1758 2023-07-22 22:59:09.000000 catmux-0.3.4/catmux/prefix.py
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-07-22 23:01:28.309641 catmux-0.3.4/catmux/resources/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        0 2023-07-22 21:14:37.000000 catmux-0.3.4/catmux/resources/__init__.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1984 2023-07-22 21:14:37.000000 catmux-0.3.4/catmux/resources/example_session.yaml
--rw-rw-r--   0 mauch     (1000) mauch     (1000)      810 2023-07-22 21:14:37.000000 catmux-0.3.4/catmux/resources/readme_tmux.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1593 2023-07-22 21:14:37.000000 catmux-0.3.4/catmux/resources/tmux_default.conf
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     8951 2023-07-22 22:59:09.000000 catmux-0.3.4/catmux/session.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     2172 2023-04-04 19:35:47.000000 catmux-0.3.4/catmux/split.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     2426 2023-07-22 22:53:23.000000 catmux-0.3.4/catmux/tmux_wrapper.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     4066 2023-07-21 15:13:50.000000 catmux-0.3.4/catmux/window.py
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-07-22 23:01:28.305641 catmux-0.3.4/catmux.egg-info/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     6358 2023-07-22 23:01:28.000000 catmux-0.3.4/catmux.egg-info/PKG-INFO
--rw-rw-r--   0 mauch     (1000) mauch     (1000)      723 2023-07-22 23:01:28.000000 catmux-0.3.4/catmux.egg-info/SOURCES.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        1 2023-07-22 23:01:28.000000 catmux-0.3.4/catmux.egg-info/dependency_links.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        7 2023-07-22 23:01:28.000000 catmux-0.3.4/catmux.egg-info/requires.txt
--rw-rw-r--   0 mauch     (1000) mauch     (1000)        7 2023-07-22 23:01:28.000000 catmux-0.3.4/catmux.egg-info/top_level.txt
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-07-22 23:01:28.309641 catmux-0.3.4/script/
--rwxrwxr-x   0 mauch     (1000) mauch     (1000)     4846 2023-07-22 21:14:37.000000 catmux-0.3.4/script/catmux_create_session
--rw-rw-r--   0 mauch     (1000) mauch     (1000)       38 2023-07-22 23:01:28.309641 catmux-0.3.4/setup.cfg
--rw-rw-r--   0 mauch     (1000) mauch     (1000)      825 2023-07-22 23:01:13.000000 catmux-0.3.4/setup.py
-drwxrwxr-x   0 mauch     (1000) mauch     (1000)        0 2023-07-22 23:01:28.309641 catmux-0.3.4/test/
--rw-rw-r--   0 mauch     (1000) mauch     (1000)      644 2023-07-22 21:03:52.000000 catmux-0.3.4/test/test_debug.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     1328 2023-07-22 22:59:09.000000 catmux-0.3.4/test/test_helpers.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     5112 2023-07-22 22:59:09.000000 catmux-0.3.4/test/test_parsing.py
--rw-rw-r--   0 mauch     (1000) mauch     (1000)     2820 2023-07-22 22:59:09.000000 catmux-0.3.4/test/test_run.py
+drwxr-xr-x   0 fexner    (1000) fexner    (1000)        0 2023-08-04 19:48:46.389978 catmux-0.3.5/
+-rw-r--r--   0 fexner    (1000) fexner    (1000)       56 2023-08-04 19:20:06.000000 catmux-0.3.5/.coveragerc
+drwxr-xr-x   0 fexner    (1000) fexner    (1000)        0 2023-08-04 19:48:46.383311 catmux-0.3.5/.github/
+drwxr-xr-x   0 fexner    (1000) fexner    (1000)        0 2023-08-04 19:48:46.386644 catmux-0.3.5/.github/workflows/
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     1114 2023-08-04 19:43:48.000000 catmux-0.3.5/.github/workflows/coverage.yaml
+-rw-r--r--   0 fexner    (1000) fexner    (1000)      815 2023-08-04 19:20:06.000000 catmux-0.3.5/.github/workflows/package.yaml
+-rw-r--r--   0 fexner    (1000) fexner    (1000)      387 2023-08-04 19:20:06.000000 catmux-0.3.5/.github/workflows/pre-commit.yaml
+-rw-r--r--   0 fexner    (1000) fexner    (1000)       29 2023-08-04 19:20:06.000000 catmux-0.3.5/.gitignore
+-rw-r--r--   0 fexner    (1000) fexner    (1000)      490 2022-04-15 19:44:17.000000 catmux-0.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 fexner    (1000) fexner    (1000)    11680 2022-04-15 19:44:17.000000 catmux-0.3.5/.pylintrc
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     1068 2022-04-15 08:48:31.000000 catmux-0.3.5/LICENSE
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     6358 2023-08-04 19:48:46.389978 catmux-0.3.5/PKG-INFO
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     5927 2023-08-04 19:20:06.000000 catmux-0.3.5/README.md
+drwxr-xr-x   0 fexner    (1000) fexner    (1000)        0 2023-08-04 19:48:46.386644 catmux-0.3.5/catmux/
+-rw-r--r--   0 fexner    (1000) fexner    (1000)        0 2022-04-16 08:21:45.000000 catmux-0.3.5/catmux/__init__.py
+-rw-r--r--   0 fexner    (1000) fexner    (1000)      210 2023-08-04 19:20:06.000000 catmux-0.3.5/catmux/exceptions.py
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     1758 2023-08-04 19:20:06.000000 catmux-0.3.5/catmux/prefix.py
+drwxr-xr-x   0 fexner    (1000) fexner    (1000)        0 2023-08-04 19:48:46.389978 catmux-0.3.5/catmux/resources/
+-rw-r--r--   0 fexner    (1000) fexner    (1000)        0 2023-08-04 19:20:06.000000 catmux-0.3.5/catmux/resources/__init__.py
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     1984 2023-08-04 19:20:06.000000 catmux-0.3.5/catmux/resources/example_session.yaml
+-rw-r--r--   0 fexner    (1000) fexner    (1000)      810 2023-08-04 19:20:06.000000 catmux-0.3.5/catmux/resources/readme_tmux.txt
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     1593 2023-08-04 19:20:06.000000 catmux-0.3.5/catmux/resources/tmux_default.conf
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     8951 2023-08-04 19:20:06.000000 catmux-0.3.5/catmux/session.py
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     2172 2023-05-23 19:42:19.000000 catmux-0.3.5/catmux/split.py
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     2426 2023-05-23 19:42:19.000000 catmux-0.3.5/catmux/tmux_wrapper.py
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     4066 2023-08-04 19:20:06.000000 catmux-0.3.5/catmux/window.py
+drwxr-xr-x   0 fexner    (1000) fexner    (1000)        0 2023-08-04 19:48:46.386644 catmux-0.3.5/catmux.egg-info/
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     6358 2023-08-04 19:48:46.000000 catmux-0.3.5/catmux.egg-info/PKG-INFO
+-rw-r--r--   0 fexner    (1000) fexner    (1000)      683 2023-08-04 19:48:46.000000 catmux-0.3.5/catmux.egg-info/SOURCES.txt
+-rw-r--r--   0 fexner    (1000) fexner    (1000)        1 2023-08-04 19:48:46.000000 catmux-0.3.5/catmux.egg-info/dependency_links.txt
+-rw-r--r--   0 fexner    (1000) fexner    (1000)        7 2023-08-04 19:48:46.000000 catmux-0.3.5/catmux.egg-info/requires.txt
+-rw-r--r--   0 fexner    (1000) fexner    (1000)        7 2023-08-04 19:48:46.000000 catmux-0.3.5/catmux.egg-info/top_level.txt
+drwxr-xr-x   0 fexner    (1000) fexner    (1000)        0 2023-08-04 19:48:46.389978 catmux-0.3.5/script/
+-rwxr-xr-x   0 fexner    (1000) fexner    (1000)     4851 2023-08-04 19:43:48.000000 catmux-0.3.5/script/catmux_create_session
+-rw-r--r--   0 fexner    (1000) fexner    (1000)       38 2023-08-04 19:48:46.389978 catmux-0.3.5/setup.cfg
+-rw-r--r--   0 fexner    (1000) fexner    (1000)      825 2023-08-04 19:44:13.000000 catmux-0.3.5/setup.py
+drwxr-xr-x   0 fexner    (1000) fexner    (1000)        0 2023-08-04 19:48:46.389978 catmux-0.3.5/test/
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     1328 2023-08-04 19:20:06.000000 catmux-0.3.5/test/test_helpers.py
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     5112 2023-08-04 19:20:06.000000 catmux-0.3.5/test/test_parsing.py
+-rw-r--r--   0 fexner    (1000) fexner    (1000)     2820 2023-08-04 19:20:06.000000 catmux-0.3.5/test/test_run.py
```

### Comparing `catmux-0.3.4/LICENSE` & `catmux-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `catmux-0.3.4/PKG-INFO` & `catmux-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catmux
-Version: 0.3.4
+Version: 0.3.5
 Summary: A tmux orchestration package.
 Home-page: https://github.com/fmauch/catmux
 Author: Felix Exner
 Author-email: felix_mauch@web.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `catmux-0.3.4/README.md` & `catmux-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `catmux-0.3.4/catmux/example_session.yaml` & `catmux-0.3.5/catmux/resources/example_session.yaml`

 * *Files identical despite different names*

### Comparing `catmux-0.3.4/catmux/prefix.py` & `catmux-0.3.5/catmux/prefix.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.4/catmux/resources/readme_tmux.txt` & `catmux-0.3.5/catmux/resources/readme_tmux.txt`

 * *Files identical despite different names*

### Comparing `catmux-0.3.4/catmux/resources/tmux_default.conf` & `catmux-0.3.5/catmux/resources/tmux_default.conf`

 * *Files identical despite different names*

### Comparing `catmux-0.3.4/catmux/session.py` & `catmux-0.3.5/catmux/session.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.4/catmux/split.py` & `catmux-0.3.5/catmux/split.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.4/catmux/tmux_wrapper.py` & `catmux-0.3.5/catmux/tmux_wrapper.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.4/catmux/window.py` & `catmux-0.3.5/catmux/window.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.4/catmux.egg-info/PKG-INFO` & `catmux-0.3.5/catmux.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catmux
-Version: 0.3.4
+Version: 0.3.5
 Summary: A tmux orchestration package.
 Home-page: https://github.com/fmauch/catmux
 Author: Felix Exner
 Author-email: felix_mauch@web.de
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `catmux-0.3.4/catmux.egg-info/SOURCES.txt` & `catmux-0.3.5/catmux.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,17 @@
+.coveragerc
+.gitignore
+.pre-commit-config.yaml
+.pylintrc
 LICENSE
 README.md
 setup.py
-./catmux/__init__.py
-./catmux/example_session.yaml
-./catmux/exceptions.py
-./catmux/prefix.py
-./catmux/session.py
-./catmux/split.py
-./catmux/tmux_wrapper.py
-./catmux/window.py
+.github/workflows/coverage.yaml
+.github/workflows/package.yaml
+.github/workflows/pre-commit.yaml
 catmux/__init__.py
 catmux/exceptions.py
 catmux/prefix.py
 catmux/session.py
 catmux/split.py
 catmux/tmux_wrapper.py
 catmux/window.py
@@ -22,11 +21,10 @@
 catmux.egg-info/requires.txt
 catmux.egg-info/top_level.txt
 catmux/resources/__init__.py
 catmux/resources/example_session.yaml
 catmux/resources/readme_tmux.txt
 catmux/resources/tmux_default.conf
 script/catmux_create_session
-test/test_debug.py
 test/test_helpers.py
 test/test_parsing.py
 test/test_run.py
```

### Comparing `catmux-0.3.4/script/catmux_create_session` & `catmux-0.3.5/script/catmux_create_session`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         tmux_config = os.path.expanduser("~/.tmux.conf")
     elif os.path.exists("/etc/tmux.conf"):
         tmux_config = "/etc/tmux.conf"
     else:
         with resources.path(
             ".".join(["catmux", "resources"]), "tmux_default.conf"
         ) as catmux_session:
-            tmux_config = catmux_session
+            tmux_config = str(catmux_session)
 
     print("Using tmux config file: {}".format(tmux_config))
     command += ["-f", tmux_config]
 
     command += ["new-session", "-s", args.session_name]
     command.append("-d")
     print(" ".join(command))
```

### Comparing `catmux-0.3.4/setup.py` & `catmux-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="catmux",
-    version="0.3.4",
+    version="0.3.5",
     license="MIT",
     author="Felix Exner",
     author_email="felix_mauch@web.de",
     description="A tmux orchestration package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fmauch/catmux",
```

### Comparing `catmux-0.3.4/test/test_helpers.py` & `catmux-0.3.5/test/test_helpers.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.4/test/test_parsing.py` & `catmux-0.3.5/test/test_parsing.py`

 * *Files identical despite different names*

### Comparing `catmux-0.3.4/test/test_run.py` & `catmux-0.3.5/test/test_run.py`

 * *Files identical despite different names*

