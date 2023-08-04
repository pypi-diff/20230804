# Comparing `tmp/jsoneng-1.0.7.tar.gz` & `tmp/jsoneng-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsoneng-1.0.7.tar", last modified: Mon Jun 26 00:41:05 2023, max compression
+gzip compressed data, was "jsoneng-1.0.8.tar", last modified: Fri Aug  4 20:42:32 2023, max compression
```

## Comparing `jsoneng-1.0.7.tar` & `jsoneng-1.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 00:41:05.956152 jsoneng-1.0.7/
--rw-rw-rw-   0        0        0     1091 2023-05-13 03:44:08.000000 jsoneng-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     2021 2023-06-26 00:41:05.956152 jsoneng-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2023-05-13 03:44:08.000000 jsoneng-1.0.7/README.md
--rw-rw-rw-   0        0        0      108 2023-05-13 03:44:08.000000 jsoneng-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0      682 2023-06-26 00:41:05.958907 jsoneng-1.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-26 00:41:05.926730 jsoneng-1.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-06-26 00:41:05.937527 jsoneng-1.0.7/src/jsoneng/
--rw-rw-rw-   0        0        0     4252 2023-06-26 00:40:16.000000 jsoneng-1.0.7/src/jsoneng/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 00:41:05.955641 jsoneng-1.0.7/src/jsoneng.egg-info/
--rw-rw-rw-   0        0        0     2021 2023-06-26 00:41:05.000000 jsoneng-1.0.7/src/jsoneng.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-06-26 00:41:05.000000 jsoneng-1.0.7/src/jsoneng.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 00:41:05.000000 jsoneng-1.0.7/src/jsoneng.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-26 00:41:05.000000 jsoneng-1.0.7/src/jsoneng.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 20:42:32.527798 jsoneng-1.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-05-13 03:44:08.000000 jsoneng-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     2021 2023-08-04 20:42:32.528793 jsoneng-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2023-05-13 03:44:08.000000 jsoneng-1.0.8/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-13 03:44:08.000000 jsoneng-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0      682 2023-08-04 20:42:32.530134 jsoneng-1.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 20:42:32.494731 jsoneng-1.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-08-04 20:42:32.512140 jsoneng-1.0.8/src/jsoneng/
+-rw-rw-rw-   0        0        0     4328 2023-08-04 20:40:58.000000 jsoneng-1.0.8/src/jsoneng/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-04 20:42:32.527798 jsoneng-1.0.8/src/jsoneng.egg-info/
+-rw-rw-rw-   0        0        0     2021 2023-08-04 20:42:32.000000 jsoneng-1.0.8/src/jsoneng.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-08-04 20:42:32.000000 jsoneng-1.0.8/src/jsoneng.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 20:42:32.000000 jsoneng-1.0.8/src/jsoneng.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-04 20:42:32.000000 jsoneng-1.0.8/src/jsoneng.egg-info/top_level.txt
```

### Comparing `jsoneng-1.0.7/LICENSE` & `jsoneng-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jsoneng-1.0.7/PKG-INFO` & `jsoneng-1.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsoneng
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package for a python JSON database CRUD engine
 Home-page: https://github.com/youhengzhou/jsoneng
 Author: YouHeng Zhou
 Author-email: youhengzhou@cmail.carleton.ca
 Project-URL: Bug Tracker, https://github.com/youhengzhou/jsoneng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jsoneng-1.0.7/README.md` & `jsoneng-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `jsoneng-1.0.7/setup.cfg` & `jsoneng-1.0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206a 736f 6e65 6e67 0d0a 7665 7273   = jsoneng..vers
-00000020: 696f 6e20 3d20 312e 302e 370d 0a61 7574  ion = 1.0.7..aut
+00000020: 696f 6e20 3d20 312e 302e 380d 0a61 7574  ion = 1.0.8..aut
 00000030: 686f 7220 3d20 596f 7548 656e 6720 5a68  hor = YouHeng Zh
 00000040: 6f75 0d0a 6175 7468 6f72 5f65 6d61 696c  ou..author_email
 00000050: 203d 2079 6f75 6865 6e67 7a68 6f75 4063   = youhengzhou@c
 00000060: 6d61 696c 2e63 6172 6c65 746f 6e2e 6361  mail.carleton.ca
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 4120 7061 636b 6167 6520 666f 7220 6120  A package for a 
 00000090: 7079 7468 6f6e 204a 534f 4e20 6461 7461  python JSON data
```

### Comparing `jsoneng-1.0.7/src/jsoneng/__init__.py` & `jsoneng-1.0.8/src/jsoneng/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 import os
 import json
 
+
 class JsonDB:
-    def __init__(self, path=None, indent=4):
-        self.path = path or os.path.join(os.getcwd(), 'jdb')
+    def __init__(self, dictionary=None, path=None, indent=4):
+        self.path = path or os.path.join(os.getcwd(), "jdb")
         self.indent = indent
+        if dictionary is not None:
+            self.create(dictionary)
 
     def _get_file_path(self, *args):
         dir_path = os.path.join(self.path, *args)
-        file_path = os.path.join(dir_path, 'jdb.json')
+        file_path = os.path.join(dir_path, "jdb.json")
         return dir_path, file_path
-    
+
     def _write_json(self, data, file_path):
-        with open(file_path, 'w') as f:
+        with open(file_path, "w") as f:
             json.dump(data, f, indent=self.indent)
-    
+
     def set_indent(self, indent):
         self.indent = indent
 
     def create(self, dictionary, *args):
         dir_path, file_path = self._get_file_path(*args)
         os.makedirs(dir_path, exist_ok=True)
         self._write_json(dictionary, file_path)
 
     def retrieve(self, *args):
         _, file_path = self._get_file_path(*args)
         if os.path.exists(file_path):
-            with open(file_path, 'r') as f:
+            with open(file_path, "r") as f:
                 return json.load(f)
         return False
 
     def retrieve_k(self, key, *args):
         data = self.retrieve(*args)
         return data.get(key, False) if data else False
 
@@ -43,15 +46,15 @@
 
     def update_kv(self, key, value, *args):
         return self.update({key: value}, *args)
 
     def patch(self, dictionary, *args):
         _, file_path = self._get_file_path(*args)
         if os.path.exists(file_path):
-            with open(file_path, 'r+') as f:
+            with open(file_path, "r+") as f:
                 data = json.load(f)
                 data.update(dictionary)
                 f.seek(0)
                 self._write_json(data, file_path)
             return True
         return False
 
@@ -60,31 +63,31 @@
 
     def delete(self, *args):
         dir_path, file_path = self._get_file_path(*args)
         if os.path.exists(file_path):
             os.remove(file_path)
             os.rmdir(dir_path)
             return True
-        print('The selected file does not exist')
+        print("The selected file does not exist")
         return False
 
     def delete_k(self, key, *args):
         _, file_path = self._get_file_path(*args)
         if os.path.exists(file_path):
-            with open(file_path, 'r+') as f:
+            with open(file_path, "r+") as f:
                 data = json.load(f)
                 if key in data:
                     del data[key]
                     f.seek(0)
                     f.truncate()
                     self._write_json(data, file_path)
                     return True
-                print('The selected key does not exist')
+                print("The selected key does not exist")
                 return False
-        print('The selected file does not exist')
+        print("The selected file does not exist")
         return False
 
     def print(self, *args):
         data = self.retrieve(*args)
         if data:
             print(json.dumps(data, indent=4))
         else:
@@ -100,33 +103,33 @@
         self.update_kv(key, value, *args)
 
     def d(self, key, *args):
         self.delete_k(key, *args)
 
     def p(self, key, value, *args):
         self.patch_kv(key, value, *args)
-    
+
     def ptr(self, key, *args):
         value = self.retrieve_k(key, *args)
         if value:
             print({key: value})
         else:
             print("Key not found")
 
     def i(self, value, *args):
         data = self.retrieve(*args)
         highest = max(map(int, data.keys()), default=-1)
         self.patch_kv(str(highest + 1), value, *args)
-    
+
     # def k(self, desc, value, *args):
     #     data = self.retrieve(*args)
     #     highest = max(map(int, data.keys()), default=-1)
     #     self.patch_kv(str(highest + 1) + ' ' + desc, value, *args)
 
-    def v(self, desc, value='', *args):
+    def v(self, desc, value="", *args):
         if value:
-            value = ' ' + value
+            value = " " + value
         self.i(desc + value, *args)
 
     def f(self, key, value, *args):
         if not self.retrieve_k(key, *args):
             self.patch_kv(key, value, *args)
```

### Comparing `jsoneng-1.0.7/src/jsoneng.egg-info/PKG-INFO` & `jsoneng-1.0.8/src/jsoneng.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsoneng
-Version: 1.0.7
+Version: 1.0.8
 Summary: A package for a python JSON database CRUD engine
 Home-page: https://github.com/youhengzhou/jsoneng
 Author: YouHeng Zhou
 Author-email: youhengzhou@cmail.carleton.ca
 Project-URL: Bug Tracker, https://github.com/youhengzhou/jsoneng/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

