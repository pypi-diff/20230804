# Comparing `tmp/types-aiobotocore-elasticbeanstalk-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-elasticbeanstalk-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elasticbeanstalk-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-elasticbeanstalk-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:50 2023, max compression
```

## Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1.tar` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.817593 types-aiobotocore-elasticbeanstalk-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:12.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21861 2023-08-02 14:52:14.817593 types-aiobotocore-elasticbeanstalk-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20307 2023-08-02 14:38:12.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.817593 types-aiobotocore-elasticbeanstalk-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:38:12.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.805593 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45011 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    44947 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    52786 2023-08-02 14:38:16.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    52747 2023-08-02 14:38:15.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:12.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-02 14:38:13.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.817593 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21861 2023-08-02 14:52:14.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-02 14:52:14.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:14.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.516070 types-aiobotocore-elasticbeanstalk-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-08-04 12:00:50.508070 types-aiobotocore-elasticbeanstalk-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13757 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:50.516070 types-aiobotocore-elasticbeanstalk-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-04 11:45:40.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.508070 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45011 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44947 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11778 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8168 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    52786 2023-08-04 11:45:44.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52747 2023-08-04 11:45:43.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-08-04 11:45:41.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:50.508070 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15311 2023-08-04 12:00:50.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-08-04 12:00:50.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:50.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:50.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:50.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-04 12:00:50.000000 types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/LICENSE` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/setup.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elasticbeanstalk",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_elasticbeanstalk"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElasticBeanstalk 2.5.2 service generated with"
-        " mypy-boto3-builder 7.17.1"
+        " mypy-boto3-builder 7.17.2"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/__init__.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/__init__.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/__main__.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ElasticBeanstalk 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elasticbeanstalk//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elasticbeanstalk.html#ElasticBeanstalk\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2.post1")
+    print("2.5.2.post2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/client.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/client.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/literals.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/literals.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/paginator.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/paginator.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/type_defs.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/type_defs.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/waiter.py` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk/waiter.pyi` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elasticbeanstalk-2.5.2.post1/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt` & `types-aiobotocore-elasticbeanstalk-2.5.2.post2/types_aiobotocore_elasticbeanstalk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

