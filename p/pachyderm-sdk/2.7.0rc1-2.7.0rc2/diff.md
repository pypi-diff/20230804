# Comparing `tmp/pachyderm_sdk-2.7.0rc1.tar.gz` & `tmp/pachyderm_sdk-2.7.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pachyderm_sdk-2.7.0rc1.tar", max compression
+gzip compressed data, was "pachyderm_sdk-2.7.0rc2.tar", max compression
```

## Comparing `pachyderm_sdk-2.7.0rc1.tar` & `pachyderm_sdk-2.7.0rc2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     2830 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/README.md
--rw-r--r--   0        0        0      357 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/__init__.py
--rw-r--r--   0        0        0      645 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/__main__.py
--rw-r--r--   0        0        0        8 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/.gitignore
--rw-r--r--   0        0        0        0 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/__init__.py
--rw-r--r--   0        0        0     2731 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/admin/__init__.py
--rw-r--r--   0        0        0     1036 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/admin/extension.py
--rw-r--r--   0        0        0    45738 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/auth/__init__.py
--rw-r--r--   0        0        0    12532 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/debug/__init__.py
--rw-r--r--   0        0        0     1572 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/debug/extension.py
--rw-r--r--   0        0        0    12463 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/enterprise/__init__.py
--rw-r--r--   0        0        0    19931 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/identity/__init__.py
--rw-r--r--   0        0        0    15874 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/license/__init__.py
--rw-r--r--   0        0        0    83954 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/__init__.py
--rw-r--r--   0        0        0     5398 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/_additions.py
--rw-r--r--   0        0        0    25802 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/extension.py
--rw-r--r--   0        0        0     4018 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/file.py
--rw-r--r--   0        0        0    86768 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pps/__init__.py
--rw-r--r--   0        0        0      677 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pps/_additions.py
--rw-r--r--   0        0        0     4222 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pps/extension.py
--rw-r--r--   0        0        0     1113 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/taskapi/__init__.py
--rw-r--r--   0        0        0    10917 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/transaction/__init__.py
--rw-r--r--   0        0        0     3614 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/transaction/extension.py
--rw-r--r--   0        0        0     2041 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/version/__init__.py
--rw-r--r--   0        0        0     4638 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/worker/__init__.py
--rw-r--r--   0        0        0     1872 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/worker/extension.py
--rw-r--r--   0        0        0    12044 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/client.py
--rw-r--r--   0        0        0     4077 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/config.py
--rw-r--r--   0        0        0      994 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/constants.py
--rw-r--r--   0        0        0     1570 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/datum_batching.py
--rw-r--r--   0        0        0     1613 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/errors.py
--rw-r--r--   0        0        0     1858 2023-07-27 16:44:06.630522 pachyderm_sdk-2.7.0rc1/pachyderm_sdk/interceptor.py
--rw-r--r--   0        0        0     1503 2023-07-27 16:44:39.426643 pachyderm_sdk-2.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     4217 1970-01-01 00:00:00.000000 pachyderm_sdk-2.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     2830 2023-08-04 18:42:47.546602 pachyderm_sdk-2.7.0rc2/README.md
+-rw-r--r--   0        0        0      357 2023-08-04 18:42:47.546602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/__init__.py
+-rw-r--r--   0        0        0      645 2023-08-04 18:42:47.546602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/__main__.py
+-rw-r--r--   0        0        0        8 2023-08-04 18:42:47.546602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/.gitignore
+-rw-r--r--   0        0        0        0 2023-08-04 18:42:47.546602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/__init__.py
+-rw-r--r--   0        0        0     2731 2023-08-04 18:42:47.546602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/admin/__init__.py
+-rw-r--r--   0        0        0     1036 2023-08-04 18:42:47.546602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/admin/extension.py
+-rw-r--r--   0        0        0    45738 2023-08-04 18:42:47.546602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/auth/__init__.py
+-rw-r--r--   0        0        0    12532 2023-08-04 18:42:47.546602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/debug/__init__.py
+-rw-r--r--   0        0        0     1572 2023-08-04 18:42:47.546602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/debug/extension.py
+-rw-r--r--   0        0        0    12463 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/enterprise/__init__.py
+-rw-r--r--   0        0        0    19931 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/identity/__init__.py
+-rw-r--r--   0        0        0    15874 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/license/__init__.py
+-rw-r--r--   0        0        0    83954 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pfs/__init__.py
+-rw-r--r--   0        0        0     5447 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pfs/_additions.py
+-rw-r--r--   0        0        0    25802 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pfs/extension.py
+-rw-r--r--   0        0        0     4018 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pfs/file.py
+-rw-r--r--   0        0        0    86768 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pps/__init__.py
+-rw-r--r--   0        0        0      677 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pps/_additions.py
+-rw-r--r--   0        0        0     4222 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pps/extension.py
+-rw-r--r--   0        0        0     1113 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/taskapi/__init__.py
+-rw-r--r--   0        0        0    10917 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/transaction/__init__.py
+-rw-r--r--   0        0        0     3614 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/transaction/extension.py
+-rw-r--r--   0        0        0     2041 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/version/__init__.py
+-rw-r--r--   0        0        0     4638 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/worker/__init__.py
+-rw-r--r--   0        0        0     1872 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/worker/extension.py
+-rw-r--r--   0        0        0    12044 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/client.py
+-rw-r--r--   0        0        0     4077 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/config.py
+-rw-r--r--   0        0        0      994 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/constants.py
+-rw-r--r--   0        0        0     1570 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/datum_batching.py
+-rw-r--r--   0        0        0     1613 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/errors.py
+-rw-r--r--   0        0        0     1858 2023-08-04 18:42:47.550602 pachyderm_sdk-2.7.0rc2/pachyderm_sdk/interceptor.py
+-rw-r--r--   0        0        0     1503 2023-08-04 18:43:22.631065 pachyderm_sdk-2.7.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     4217 1970-01-01 00:00:00.000000 pachyderm_sdk-2.7.0rc2/PKG-INFO
```

### Comparing `pachyderm_sdk-2.7.0rc1/README.md` & `pachyderm_sdk-2.7.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/__main__.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/admin/__init__.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/admin/extension.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/admin/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/auth/__init__.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/debug/__init__.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/debug/extension.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/debug/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/enterprise/__init__.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/enterprise/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/identity/__init__.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/license/__init__.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/license/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/__init__.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pfs/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/_additions.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pfs/_additions.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,16 @@
         project = self.project.name
     return f"{project}/{self.name}"
 
 
 def _Repo___post_init__(self: "Repo") -> None:
     if not self.project or not self.project.name:
         self.project = Project(name="default")
+    if not self.type:
+        self.type = "user"
     super(self.__class__, self).__post_init__()
 
 
 Repo.from_uri = _Repo_from_uri
 Repo.as_uri = Repo.__str__ = _Repo_as_uri
 Repo.__post_init__ = _Repo___post_init__
```

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/extension.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pfs/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pfs/file.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pfs/file.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pps/__init__.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pps/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pps/_additions.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pps/_additions.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/pps/extension.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/pps/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/taskapi/__init__.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/taskapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/transaction/__init__.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/transaction/extension.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/transaction/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/version/__init__.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/worker/__init__.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/api/worker/extension.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/api/worker/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/client.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/client.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/config.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/config.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/constants.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/datum_batching.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/datum_batching.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/errors.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pachyderm_sdk/interceptor.py` & `pachyderm_sdk-2.7.0rc2/pachyderm_sdk/interceptor.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.7.0rc1/pyproject.toml` & `pachyderm_sdk-2.7.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pachyderm_sdk"
-version = "2.7.0-rc.1"
+version = "2.7.0-rc.2"
 description = "Python Pachyderm Client"
 authors = ["Pachyderm Integrations <integrations@pachyderm.io>"]
 license = "Apache 2.0"
 documentation = "https://docs.pachyderm.com/latest/sdk/python/"
 readme = 'README.md'
 repository = "https://github.com/pachyderm/pachyderm/tree/master/python-sdk"
 keywords = ["pachyderm"]
```

### Comparing `pachyderm_sdk-2.7.0rc1/PKG-INFO` & `pachyderm_sdk-2.7.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pachyderm-sdk
-Version: 2.7.0rc1
+Version: 2.7.0rc2
 Summary: Python Pachyderm Client
 Home-page: https://github.com/pachyderm/pachyderm/tree/master/python-sdk
 License: Apache 2.0
 Keywords: pachyderm
 Author: Pachyderm Integrations
 Author-email: integrations@pachyderm.io
 Requires-Python: >=3.8,<4.0
```

