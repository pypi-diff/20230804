# Comparing `tmp/heisenbergpy-0.0.1.tar.gz` & `tmp/heisenbergpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heisenbergpy-0.0.1.tar", last modified: Mon Jun  5 16:04:52 2023, max compression
+gzip compressed data, was "heisenbergpy-0.0.2.tar", last modified: Fri Aug  4 17:04:13 2023, max compression
```

## Comparing `heisenbergpy-0.0.1.tar` & `heisenbergpy-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 16:04:52.403264 heisenbergpy-0.0.1/
--rw-rw-rw-   0        0        0      116 2023-06-05 16:04:52.402265 heisenbergpy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-05 15:54:12.000000 heisenbergpy-0.0.1/README.md
--rw-rw-rw-   0        0        0      143 2023-06-05 16:04:23.000000 heisenbergpy-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-05 16:04:52.403264 heisenbergpy-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-05 16:04:52.344197 heisenbergpy-0.0.1/src/
--rw-rw-rw-   0        0        0     2071 2023-06-03 19:11:34.000000 heisenbergpy-0.0.1/src/heisenberg.py
-drwxrwxrwx   0        0        0        0 2023-06-05 16:04:52.400265 heisenbergpy-0.0.1/src/heisenbergpy.egg-info/
--rw-rw-rw-   0        0        0      116 2023-06-05 16:04:52.000000 heisenbergpy-0.0.1/src/heisenbergpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-06-05 16:04:52.000000 heisenbergpy-0.0.1/src/heisenbergpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 16:04:52.000000 heisenbergpy-0.0.1/src/heisenbergpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-05 16:04:52.000000 heisenbergpy-0.0.1/src/heisenbergpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 17:04:13.765421 heisenbergpy-0.0.2/
+-rw-rw-rw-   0        0        0      116 2023-08-04 17:04:13.755387 heisenbergpy-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       50 2023-06-05 16:06:15.000000 heisenbergpy-0.0.2/README.md
+-rw-rw-rw-   0        0        0      143 2023-08-04 17:01:56.000000 heisenbergpy-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-04 17:04:13.765421 heisenbergpy-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 17:04:13.743388 heisenbergpy-0.0.2/src/
+-rw-rw-rw-   0        0        0     2063 2023-08-04 16:49:47.000000 heisenbergpy-0.0.2/src/heisenberg.py
+drwxrwxrwx   0        0        0        0 2023-08-04 17:04:13.754388 heisenbergpy-0.0.2/src/heisenbergpy.egg-info/
+-rw-rw-rw-   0        0        0      116 2023-08-04 17:04:13.000000 heisenbergpy-0.0.2/src/heisenbergpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-08-04 17:04:13.000000 heisenbergpy-0.0.2/src/heisenbergpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 17:04:13.000000 heisenbergpy-0.0.2/src/heisenbergpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-08-04 17:04:13.000000 heisenbergpy-0.0.2/src/heisenbergpy.egg-info/top_level.txt
```

### Comparing `heisenbergpy-0.0.1/src/heisenberg.py` & `heisenbergpy-0.0.2/src/heisenberg.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,23 +22,23 @@
             logging.error("Invalid API key")
             return None
         elif response.status_code != 200:
             logging.error(f"Error {response.status_code}: {response.text}")
             return None
         return response.json()
     
-    def new_collection(self, name, dim, space):
+    def new_bucket(self, name, dim, space):
         data = {
             'name': name,
             'dim': dim,
             'space': space
         }
         self._request('POST', 'newcollection', data)
     
-    def delete_collection(self, name):
+    def delete_bucket(self, name):
         data = {
             'name': name
         }
         self._request('POST', 'deletecollection', data)
     
     def get(self, collection, key):
         data = {
```

