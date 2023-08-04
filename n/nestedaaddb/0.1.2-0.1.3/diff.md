# Comparing `tmp/nestedaaddb-0.1.2.tar.gz` & `tmp/nestedaaddb-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestedaaddb-0.1.2.tar", last modified: Wed Jul 26 01:28:36 2023, max compression
+gzip compressed data, was "nestedaaddb-0.1.3.tar", last modified: Fri Aug  4 01:46:02 2023, max compression
```

## Comparing `nestedaaddb-0.1.2.tar` & `nestedaaddb-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 abhishekpratap.singh   (502) staff       (20)        0 2023-07-26 01:28:36.248365 nestedaaddb-0.1.2/
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     5196 2023-07-26 01:28:36.248209 nestedaaddb-0.1.2/PKG-INFO
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     4770 2023-07-26 00:42:05.000000 nestedaaddb-0.1.2/README.md
-drwxr-xr-x   0 abhishekpratap.singh   (502) staff       (20)        0 2023-07-26 01:28:36.246490 nestedaaddb-0.1.2/nestedaaddb/
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       79 2023-02-19 03:38:52.000000 nestedaaddb-0.1.2/nestedaaddb/__init__.py
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     6928 2023-03-07 06:13:17.000000 nestedaaddb-0.1.2/nestedaaddb/databricks_client.py
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     4486 2022-11-16 07:00:43.000000 nestedaaddb-0.1.2/nestedaaddb/graph_client.py
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     4432 2023-03-07 05:27:06.000000 nestedaaddb-0.1.2/nestedaaddb/nested_groups.py
-drwxr-xr-x   0 abhishekpratap.singh   (502) staff       (20)        0 2023-07-26 01:28:36.247957 nestedaaddb-0.1.2/nestedaaddb.egg-info/
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     5196 2023-07-26 01:28:36.000000 nestedaaddb-0.1.2/nestedaaddb.egg-info/PKG-INFO
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)      321 2023-07-26 01:28:36.000000 nestedaaddb-0.1.2/nestedaaddb.egg-info/SOURCES.txt
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)        1 2023-07-26 01:28:36.000000 nestedaaddb-0.1.2/nestedaaddb.egg-info/dependency_links.txt
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       39 2023-07-26 01:28:36.000000 nestedaaddb-0.1.2/nestedaaddb.egg-info/requires.txt
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       12 2023-07-26 01:28:36.000000 nestedaaddb-0.1.2/nestedaaddb.egg-info/top_level.txt
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)      643 2023-07-26 01:19:53.000000 nestedaaddb-0.1.2/pyproject.toml
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       38 2023-07-26 01:28:36.248415 nestedaaddb-0.1.2/setup.cfg
--rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       38 2022-05-20 15:06:37.000000 nestedaaddb-0.1.2/setup.py
+drwxr-xr-x   0 abhishekpratap.singh   (502) staff       (20)        0 2023-08-04 01:46:02.230067 nestedaaddb-0.1.3/
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     6949 2023-08-04 01:46:02.229908 nestedaaddb-0.1.3/PKG-INFO
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     6523 2023-08-04 01:35:04.000000 nestedaaddb-0.1.3/README.md
+drwxr-xr-x   0 abhishekpratap.singh   (502) staff       (20)        0 2023-08-04 01:46:02.228104 nestedaaddb-0.1.3/nestedaaddb/
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       79 2023-02-19 03:38:52.000000 nestedaaddb-0.1.3/nestedaaddb/__init__.py
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     6928 2023-03-07 06:13:17.000000 nestedaaddb-0.1.3/nestedaaddb/databricks_client.py
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     4486 2022-11-16 07:00:43.000000 nestedaaddb-0.1.3/nestedaaddb/graph_client.py
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     4432 2023-03-07 05:27:06.000000 nestedaaddb-0.1.3/nestedaaddb/nested_groups.py
+drwxr-xr-x   0 abhishekpratap.singh   (502) staff       (20)        0 2023-08-04 01:46:02.229486 nestedaaddb-0.1.3/nestedaaddb.egg-info/
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)     6949 2023-08-04 01:46:02.000000 nestedaaddb-0.1.3/nestedaaddb.egg-info/PKG-INFO
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)      321 2023-08-04 01:46:02.000000 nestedaaddb-0.1.3/nestedaaddb.egg-info/SOURCES.txt
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)        1 2023-08-04 01:46:02.000000 nestedaaddb-0.1.3/nestedaaddb.egg-info/dependency_links.txt
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       39 2023-08-04 01:46:02.000000 nestedaaddb-0.1.3/nestedaaddb.egg-info/requires.txt
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       12 2023-08-04 01:46:02.000000 nestedaaddb-0.1.3/nestedaaddb.egg-info/top_level.txt
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)      643 2023-08-04 01:44:31.000000 nestedaaddb-0.1.3/pyproject.toml
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       38 2023-08-04 01:46:02.230120 nestedaaddb-0.1.3/setup.cfg
+-rw-r--r--   0 abhishekpratap.singh   (502) staff       (20)       38 2022-05-20 15:06:37.000000 nestedaaddb-0.1.3/setup.py
```

### Comparing `nestedaaddb-0.1.2/nestedaaddb/databricks_client.py` & `nestedaaddb-0.1.3/nestedaaddb/databricks_client.py`

 * *Files identical despite different names*

### Comparing `nestedaaddb-0.1.2/nestedaaddb/graph_client.py` & `nestedaaddb-0.1.3/nestedaaddb/graph_client.py`

 * *Files identical despite different names*

### Comparing `nestedaaddb-0.1.2/nestedaaddb/nested_groups.py` & `nestedaaddb-0.1.3/nestedaaddb/nested_groups.py`

 * *Files identical despite different names*

### Comparing `nestedaaddb-0.1.2/pyproject.toml` & `nestedaaddb-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nestedaaddb"
-version = "0.1.2"
+version = "0.1.3"
 description = "A package that allows to sync Nested AAD Group to DataBricks"
 readme = "README.md"
 authors = [{ name = "Abhishek Pratap Singh", email = "sumoaps@outlook.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

