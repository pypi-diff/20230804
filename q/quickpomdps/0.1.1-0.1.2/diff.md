# Comparing `tmp/quickpomdps-0.1.1.tar.gz` & `tmp/quickpomdps-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickpomdps-0.1.1.tar", max compression
+gzip compressed data, was "quickpomdps-0.1.2.tar", max compression
```

## Comparing `quickpomdps-0.1.1.tar` & `quickpomdps-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2021-08-09 20:48:12.025347 quickpomdps-0.1.1/LICENSE
--rw-r--r--   0        0        0     2358 2021-10-12 19:54:46.437747 quickpomdps-0.1.1/README.md
--rw-r--r--   0        0        0      622 2023-05-30 02:48:04.542078 quickpomdps-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      514 2021-10-12 19:49:46.840831 quickpomdps-0.1.1/quickpomdps/__init__.py
--rw-r--r--   0        0        0     2893 2021-10-11 23:14:35.254846 quickpomdps-0.1.1/quickpomdps/setup.jl
--rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 quickpomdps-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2021-08-09 20:48:12.025347 quickpomdps-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3174 2023-08-03 17:53:32.866438 quickpomdps-0.1.2/README.md
+-rw-r--r--   0        0        0      622 2023-08-03 21:46:54.414996 quickpomdps-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      885 2023-08-03 21:58:14.485777 quickpomdps-0.1.2/quickpomdps/__init__.py
+-rw-r--r--   0        0        0     2893 2021-10-11 23:14:35.254846 quickpomdps-0.1.2/quickpomdps/setup.jl
+-rw-r--r--   0        0        0     3919 1970-01-01 00:00:00.000000 quickpomdps-0.1.2/PKG-INFO
```

### Comparing `quickpomdps-0.1.1/LICENSE` & `quickpomdps-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quickpomdps-0.1.1/pyproject.toml` & `quickpomdps-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quickpomdps"
-version = "0.1.1"
+version = "0.1.2"
 description = "Describing and Solving POMDPs in Python"
 authors = ["rejuvyesh <mail@rejuvyesh.com>", "Zachary Sunberg <sunbergzach@gmail.com>", "Lasse Peters <lasse.peters@mailbox.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/JuliaPOMDP/quickpomdps/"
 
 [tool.poetry.dependencies]
```

### Comparing `quickpomdps-0.1.1/quickpomdps/setup.jl` & `quickpomdps-0.1.2/quickpomdps/setup.jl`

 * *Files identical despite different names*

