# Comparing `tmp/temper_pygments-0.1.0.tar.gz` & `tmp/temper_pygments-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temper_pygments-0.1.0.tar", max compression
+gzip compressed data, was "temper_pygments-0.1.1.tar", max compression
```

## Comparing `temper_pygments-0.1.0.tar` & `temper_pygments-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      655 2023-07-31 23:29:01.208681 temper_pygments-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       27 2023-04-28 18:18:11.562467 temper_pygments-0.1.0/README.md
--rw-r--r--   0        0        0       84 2023-04-28 19:43:49.952098 temper_pygments-0.1.0/temper_pygments/__init__.py
--rw-r--r--   0        0        0     1795 2023-05-02 11:52:30.257645 temper_pygments-0.1.0/temper_pygments/adapt.py
--rw-r--r--   0        0        0      704 2023-04-28 23:09:13.160673 temper_pygments-0.1.0/temper_pygments/lexer.py
--rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 temper_pygments-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      627 2023-08-04 17:20:48.737120 temper_pygments-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-04-28 18:18:11.562467 temper_pygments-0.1.1/README.md
+-rw-r--r--   0        0        0       84 2023-04-28 19:43:49.952098 temper_pygments-0.1.1/temper_pygments/__init__.py
+-rw-r--r--   0        0        0     1795 2023-05-02 11:52:30.257645 temper_pygments-0.1.1/temper_pygments/adapt.py
+-rw-r--r--   0        0        0      704 2023-04-28 23:09:13.160673 temper_pygments-0.1.1/temper_pygments/lexer.py
+-rw-r--r--   0        0        0      579 1970-01-01 00:00:00.000000 temper_pygments-0.1.1/PKG-INFO
```

### Comparing `temper_pygments-0.1.0/pyproject.toml` & `temper_pygments-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-[tool.poetry]
-name = "temper-pygments"
-version = "0.1.0"
-description = ""
-authors = ["Tom <tom@temper.systems>"]
-readme = "README.md"
-packages = [{include = "temper_pygments"}]
-
-[tool.poetry.dependencies]
-python = "^3.8"
-pygments = "^2.12.0"
-temper-core = "0.0.5"
-temper-syntax = "0.1.0"
-
-[tool.poetry.plugins."pygments.lexers"]
-temper = "temper_pygments:TemperLexer"
-tempermd = "temper_pygments:TemperMdLexer"
-
-[tool.poetry.scripts]
-bundle = 'scripts:bundle'
-test = 'scripts:test'
-
-[tool.poetry.group.dev.dependencies]
-stickytape = "^0.2.1"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "temper-pygments"
+version = "0.1.1"
+description = ""
+authors = ["Tom <tom@temper.systems>"]
+readme = "README.md"
+packages = [{include = "temper_pygments"}]
+
+[tool.poetry.dependencies]
+python = "^3.8"
+pygments = "^2.12.0"
+temper-core = "0.0.5"
+temper-syntax = "0.1.1"
+
+[tool.poetry.plugins."pygments.lexers"]
+temper = "temper_pygments:TemperLexer"
+tempermd = "temper_pygments:TemperMdLexer"
+
+[tool.poetry.scripts]
+bundle = 'scripts:bundle'
+test = 'scripts:test'
+
+[tool.poetry.group.dev.dependencies]
+stickytape = "^0.2.1"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `temper_pygments-0.1.0/temper_pygments/adapt.py` & `temper_pygments-0.1.1/temper_pygments/adapt.py`

 * *Files identical despite different names*

### Comparing `temper_pygments-0.1.0/temper_pygments/lexer.py` & `temper_pygments-0.1.1/temper_pygments/lexer.py`

 * *Files identical despite different names*

### Comparing `temper_pygments-0.1.0/PKG-INFO` & `temper_pygments-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: temper-pygments
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Tom
 Author-email: tom@temper.systems
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pygments (>=2.12.0,<3.0.0)
 Requires-Dist: temper-core (==0.0.5)
-Requires-Dist: temper-syntax (==0.1.0)
+Requires-Dist: temper-syntax (==0.1.1)
 Description-Content-Type: text/markdown
 
 Pygments lexer for Temper.
```

