# Comparing `tmp/types-aiobotocore-application-insights-2.5.2.post1.tar.gz` & `tmp/types-aiobotocore-application-insights-2.5.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-application-insights-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:52 2023, max compression
+gzip compressed data, was "types-aiobotocore-application-insights-2.5.2.post2.tar", last modified: Fri Aug  4 12:00:25 2023, max compression
```

## Comparing `types-aiobotocore-application-insights-2.5.2.post1.tar` & `types-aiobotocore-application-insights-2.5.2.post2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.769654 types-aiobotocore-application-insights-2.5.2.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-08-02 14:51:52.769654 types-aiobotocore-application-insights-2.5.2.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13580 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:52.769654 types-aiobotocore-application-insights-2.5.2.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.769654 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22655 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    22619 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-08-02 14:33:15.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-08-02 14:33:15.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19809 2023-08-02 14:33:15.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:14.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.769654 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15149 2023-08-02 14:51:52.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:51:52.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:52.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 14:51:52.000000 types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.471113 types-aiobotocore-application-insights-2.5.2.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 11:40:22.000000 types-aiobotocore-application-insights-2.5.2.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-08-04 12:00:25.471113 types-aiobotocore-application-insights-2.5.2.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-08-04 11:40:22.000000 types-aiobotocore-application-insights-2.5.2.post2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 12:00:25.471113 types-aiobotocore-application-insights-2.5.2.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-04 11:40:22.000000 types-aiobotocore-application-insights-2.5.2.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.459112 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-08-04 11:40:22.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-04 11:40:22.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-04 11:40:22.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22655 2023-08-04 11:40:22.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22619 2023-08-04 11:40:22.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-08-04 11:40:22.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9530 2023-08-04 11:40:22.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 11:40:22.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19824 2023-08-04 11:40:23.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19809 2023-08-04 11:40:23.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-04 11:40:22.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 12:00:25.471113 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2023-08-04 12:00:25.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-04 12:00:25.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:25.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 12:00:25.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 12:00:25.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-04 12:00:25.000000 types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-application-insights-2.5.2.post1/LICENSE` & `types-aiobotocore-application-insights-2.5.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2.post1/setup.py` & `types-aiobotocore-application-insights-2.5.2.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-application-insights",
-    version="2.5.2.post1",
+    version="2.5.2.post2",
     packages=["types_aiobotocore_application_insights"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ApplicationInsights 2.5.2 service generated with"
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

### Comparing `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/__init__.py` & `types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/__init__.pyi` & `types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/__main__.py` & `types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ApplicationInsights 2.5.2\nVersion:        "
-        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
+        " 2.5.2.post2\nBuilder version: 7.17.2\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_application_insights//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/application-insights.html#ApplicationInsights\nOther"
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

### Comparing `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/client.py` & `types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/client.pyi` & `types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/literals.py` & `types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/literals.pyi` & `types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/type_defs.py` & `types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/type_defs.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights/type_defs.pyi` & `types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights/type_defs.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-application-insights-2.5.2.post1/types_aiobotocore_application_insights.egg-info/SOURCES.txt` & `types-aiobotocore-application-insights-2.5.2.post2/types_aiobotocore_application_insights.egg-info/SOURCES.txt`

 * *Files identical despite different names*

