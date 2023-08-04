# Comparing `tmp/bitmap2-0.2.4.tar.gz` & `tmp/bitmap2-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmap2-0.2.4.tar", last modified: Sat Jul 15 22:05:30 2023, max compression
+gzip compressed data, was "bitmap2-0.2.5.tar", last modified: Fri Aug  4 16:29:37 2023, max compression
```

## Comparing `bitmap2-0.2.4.tar` & `bitmap2-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:05:30.031397 bitmap2-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:05:30.027397 bitmap2-0.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:05:30.027397 bitmap2-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-15 22:05:20.000000 bitmap2-0.2.4/.github/workflows/pypi-upload.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-07-15 22:05:20.000000 bitmap2-0.2.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-07-15 22:05:20.000000 bitmap2-0.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-07-15 22:05:20.000000 bitmap2-0.2.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-15 22:05:20.000000 bitmap2-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-15 22:05:30.031397 bitmap2-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-15 22:05:20.000000 bitmap2-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:05:30.031397 bitmap2-0.2.4/bitmap2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-07-15 22:05:29.000000 bitmap2-0.2.4/bitmap2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-15 22:05:30.000000 bitmap2-0.2.4/bitmap2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 22:05:29.000000 bitmap2-0.2.4/bitmap2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-15 22:05:29.000000 bitmap2-0.2.4/bitmap2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 22:05:30.031397 bitmap2-0.2.4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-07-15 22:05:20.000000 bitmap2-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:05:30.031397 bitmap2-0.2.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-15 22:05:20.000000 bitmap2-0.2.4/src/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6619 2023-07-15 22:05:20.000000 bitmap2-0.2.4/src/bitmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 22:05:30.031397 bitmap2-0.2.4/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3088 2023-07-15 22:05:20.000000 bitmap2-0.2.4/test/test_bitmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:29:36.999273 bitmap2-0.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:29:36.999273 bitmap2-0.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:29:36.999273 bitmap2-0.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-08-04 16:29:30.000000 bitmap2-0.2.5/.github/workflows/pypi-upload.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-08-04 16:29:30.000000 bitmap2-0.2.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-08-04 16:29:30.000000 bitmap2-0.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-08-04 16:29:30.000000 bitmap2-0.2.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-04 16:29:30.000000 bitmap2-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-04 16:29:36.999273 bitmap2-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-08-04 16:29:30.000000 bitmap2-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:29:36.999273 bitmap2-0.2.5/bitmap2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-04 16:29:36.000000 bitmap2-0.2.5/bitmap2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-04 16:29:36.000000 bitmap2-0.2.5/bitmap2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:29:36.000000 bitmap2-0.2.5/bitmap2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 16:29:36.000000 bitmap2-0.2.5/bitmap2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:29:37.003273 bitmap2-0.2.5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1130 2023-08-04 16:29:30.000000 bitmap2-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:29:36.999273 bitmap2-0.2.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 16:29:30.000000 bitmap2-0.2.5/src/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7276 2023-08-04 16:29:30.000000 bitmap2-0.2.5/src/bitmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:29:36.999273 bitmap2-0.2.5/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3088 2023-08-04 16:29:30.000000 bitmap2-0.2.5/test/test_bitmap.py
```

### Comparing `bitmap2-0.2.4/.github/workflows/pypi-upload.yml` & `bitmap2-0.2.5/.github/workflows/pypi-upload.yml`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.4/.github/workflows/test.yml` & `bitmap2-0.2.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.4/.gitignore` & `bitmap2-0.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.4/LICENSE.md` & `bitmap2-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.4/PKG-INFO` & `bitmap2-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmap2
-Version: 0.2.4
+Version: 0.2.5
 Summary: An updated version of the bitmap library from https://github.com/wanji/bitmap
 Home-page: https://github.com/wbarnha/bitmap
 Author: wbarnha
 Author-email: williambbarnhart@gmail.com
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bitmap2-0.2.4/README.md` & `bitmap2-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.4/bitmap2.egg-info/PKG-INFO` & `bitmap2-0.2.5/bitmap2.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmap2
-Version: 0.2.4
+Version: 0.2.5
 Summary: An updated version of the bitmap library from https://github.com/wanji/bitmap
 Home-page: https://github.com/wbarnha/bitmap
 Author: wbarnha
 Author-email: williambbarnhart@gmail.com
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bitmap2-0.2.4/setup.py` & `bitmap2-0.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `bitmap2-0.2.4/src/bitmap.py` & `bitmap2-0.2.5/src/bitmap.py`

 * *Files 6% similar despite different names*

```diff
@@ -136,14 +136,37 @@
         """
         Get all zero bits, returns generator
         """
         for i in iter(range(self.size())):
             if not self.test(i):
                 yield i
 
+    def merge(self, other_bitmap):
+        """
+        Apply OR operation to bitmap with another BitMap class
+        """
+        # See https://stackoverflow.com/a/30679284/9852671 for notes
+        pos = 0
+        for x, y in zip(self[:], other_bitmap[:]):
+            if x or y:
+                self.set(pos)
+            pos += 1
+
+    def xor(self, other_bitmap):
+        """
+        Apply XOR operation to bitmap with another BitMap class
+        """
+        pos = 0
+        for x, y in zip(self[:], other_bitmap[:]):
+            if (not x) ^ (not y):
+                self.set(pos)
+            else:
+                self.reset(pos)
+            pos += 1
+
     def zero(self):
         """
         Get all zero bits, returns list
         """
         return [i for i in iter(range(self.size())) if not self.test(i)]
 
     def tostring(self):
```

### Comparing `bitmap2-0.2.4/test/test_bitmap.py` & `bitmap2-0.2.5/test/test_bitmap.py`

 * *Files identical despite different names*

