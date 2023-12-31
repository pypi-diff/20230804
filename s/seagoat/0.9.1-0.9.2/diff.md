# Comparing `tmp/seagoat-0.9.1.tar.gz` & `tmp/seagoat-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seagoat-0.9.1.tar", max compression
+gzip compressed data, was "seagoat-0.9.2.tar", max compression
```

## Comparing `seagoat-0.9.1.tar` & `seagoat-0.9.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-08-02 18:16:36.246643 seagoat-0.9.1/LICENSE
--rw-r--r--   0        0        0     1849 2023-08-02 18:16:36.246643 seagoat-0.9.1/README.md
--rw-r--r--   0        0        0     3120 2023-08-02 18:16:37.398646 seagoat-0.9.1/pyproject.toml
--rw-r--r--   0        0        0       22 2023-08-02 18:16:37.398646 seagoat-0.9.1/seagoat/__init__.py
--rw-r--r--   0        0        0     1601 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/cache.py
--rw-r--r--   0        0        0     3209 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/cli.py
--rw-r--r--   0        0        0      196 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/common.py
--rw-r--r--   0        0        0     4424 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/engine.py
--rw-r--r--   0        0        0     3482 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/file.py
--rw-r--r--   0        0        0     2689 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/repository.py
--rw-r--r--   0        0        0     2021 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/result.py
--rw-r--r--   0        0        0     5766 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/server.py
--rw-r--r--   0        0        0     1678 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/sources/chroma.py
--rw-r--r--   0        0        0     1105 2023-08-02 18:16:36.258643 seagoat-0.9.1/seagoat/sources/ripgrep.py
--rw-r--r--   0        0        0     2863 1970-01-01 00:00:00.000000 seagoat-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-04 13:19:17.527065 seagoat-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1877 2023-08-04 13:19:17.527065 seagoat-0.9.2/README.md
+-rw-r--r--   0        0        0     3120 2023-08-04 13:19:18.639093 seagoat-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-08-04 13:19:18.639093 seagoat-0.9.2/seagoat/__init__.py
+-rw-r--r--   0        0        0     1601 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/cache.py
+-rw-r--r--   0        0        0     3209 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/cli.py
+-rw-r--r--   0        0        0      196 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/common.py
+-rw-r--r--   0        0        0     4424 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/engine.py
+-rw-r--r--   0        0        0     3482 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/file.py
+-rw-r--r--   0        0        0     2689 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/repository.py
+-rw-r--r--   0        0        0     2021 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/result.py
+-rw-r--r--   0        0        0     5766 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/server.py
+-rw-r--r--   0        0        0     1678 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/sources/chroma.py
+-rw-r--r--   0        0        0     1105 2023-08-04 13:19:17.543066 seagoat-0.9.2/seagoat/sources/ripgrep.py
+-rw-r--r--   0        0        0     2891 1970-01-01 00:00:00.000000 seagoat-0.9.2/PKG-INFO
```

### Comparing `seagoat-0.9.1/LICENSE` & `seagoat-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.1/README.md` & `seagoat-0.9.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     <font size="8"><b>SeaGOAT</b></font>
   </p>
 </h1>
 
 A code search engine for the AI age. SeaGOAT leverages vector
 embeddings to enable to search your codebase semantically.
 
+![&nbsp;](assets/demo.gif)
+
 ## Getting started
 
 ### Install SeaGOAT
 
 In order to install SeaGOAT, you need to have the following
 dependencies already installed on your computer:
```

### Comparing `seagoat-0.9.1/pyproject.toml` & `seagoat-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seagoat"
-version = "0.9.1"
+version = "0.9.2"
 description = "A semantic-code search engine"
 authors = ["Daniel Kantor <git@daniel-kantor.com>"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.scripts]
 gt = "seagoat.cli:seagoat"
```

### Comparing `seagoat-0.9.1/seagoat/cache.py` & `seagoat-0.9.2/seagoat/cache.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.1/seagoat/cli.py` & `seagoat-0.9.2/seagoat/cli.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.1/seagoat/engine.py` & `seagoat-0.9.2/seagoat/engine.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.1/seagoat/file.py` & `seagoat-0.9.2/seagoat/file.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.1/seagoat/repository.py` & `seagoat-0.9.2/seagoat/repository.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.1/seagoat/result.py` & `seagoat-0.9.2/seagoat/result.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.1/seagoat/server.py` & `seagoat-0.9.2/seagoat/server.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.1/seagoat/sources/chroma.py` & `seagoat-0.9.2/seagoat/sources/chroma.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.1/seagoat/sources/ripgrep.py` & `seagoat-0.9.2/seagoat/sources/ripgrep.py`

 * *Files identical despite different names*

### Comparing `seagoat-0.9.1/PKG-INFO` & `seagoat-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seagoat
-Version: 0.9.1
+Version: 0.9.2
 Summary: A semantic-code search engine
 License: MIT
 Author: Daniel Kantor
 Author-email: git@daniel-kantor.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -34,14 +34,16 @@
     <font size="8"><b>SeaGOAT</b></font>
   </p>
 </h1>
 
 A code search engine for the AI age. SeaGOAT leverages vector
 embeddings to enable to search your codebase semantically.
 
+![&nbsp;](assets/demo.gif)
+
 ## Getting started
 
 ### Install SeaGOAT
 
 In order to install SeaGOAT, you need to have the following
 dependencies already installed on your computer:
```

