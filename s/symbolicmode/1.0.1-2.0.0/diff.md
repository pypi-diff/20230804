# Comparing `tmp/symbolicmode-1.0.1.tar.gz` & `tmp/symbolicmode-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symbolicmode-1.0.1.tar", last modified: Wed Aug  2 12:03:21 2023, max compression
+gzip compressed data, was "symbolicmode-2.0.0.tar", last modified: Fri Aug  4 13:58:47 2023, max compression
```

## Comparing `symbolicmode-1.0.1.tar` & `symbolicmode-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-08-02 12:03:08.000000 symbolicmode-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-08-02 12:03:08.000000 symbolicmode-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-02 12:03:11.000000 symbolicmode-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/src/symbolicmode/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9621 2023-08-02 12:03:08.000000 symbolicmode-1.0.1/src/symbolicmode/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/src/symbolicmode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-08-02 12:03:21.000000 symbolicmode-1.0.1/src/symbolicmode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-02 12:03:21.000000 symbolicmode-1.0.1/src/symbolicmode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:03:21.000000 symbolicmode-1.0.1/src/symbolicmode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 12:03:21.000000 symbolicmode-1.0.1/src/symbolicmode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:03:21.118315 symbolicmode-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-02 12:03:08.000000 symbolicmode-1.0.1/tests/test_chmod.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-08-02 12:03:08.000000 symbolicmode-1.0.1/tests/test_modes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:58:47.622050 symbolicmode-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-08-04 13:58:34.000000 symbolicmode-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-08-04 13:58:47.622050 symbolicmode-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-08-04 13:58:34.000000 symbolicmode-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-04 13:58:39.000000 symbolicmode-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 13:58:47.622050 symbolicmode-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:58:47.622050 symbolicmode-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:58:47.622050 symbolicmode-2.0.0/src/symbolicmode/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9621 2023-08-04 13:58:34.000000 symbolicmode-2.0.0/src/symbolicmode/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:58:47.622050 symbolicmode-2.0.0/src/symbolicmode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-08-04 13:58:47.000000 symbolicmode-2.0.0/src/symbolicmode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-04 13:58:47.000000 symbolicmode-2.0.0/src/symbolicmode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 13:58:47.000000 symbolicmode-2.0.0/src/symbolicmode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 13:58:47.000000 symbolicmode-2.0.0/src/symbolicmode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 13:58:47.622050 symbolicmode-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-08-04 13:58:34.000000 symbolicmode-2.0.0/tests/test_chmod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-08-04 13:58:34.000000 symbolicmode-2.0.0/tests/test_modes.py
```

### Comparing `symbolicmode-1.0.1/LICENSE` & `symbolicmode-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `symbolicmode-1.0.1/PKG-INFO` & `symbolicmode-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolicmode
-Version: 1.0.1
+Version: 2.0.0
 Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
 Author-email: Sean Reifschneider <jafo00@gmail.com>
 Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
 Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

### Comparing `symbolicmode-1.0.1/README.md` & `symbolicmode-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `symbolicmode-1.0.1/pyproject.toml` & `symbolicmode-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.pytest.ini_options]
 pythonpath = "src"
 
 [project]
 name = "symbolicmode"
-version = "1.0.1"
+version = "2.0.0"
 authors = [
   { name="Sean Reifschneider", email="jafo00@gmail.com" },
 ]
 description = "Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `symbolicmode-1.0.1/src/symbolicmode/__init__.py` & `symbolicmode-2.0.0/src/symbolicmode/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,30 +179,30 @@
         ((setuid_bit + setgid_bit + sticky_bit) << 9)
         | (perms["u"] << 6)
         | (perms["g"] << 3)
         | (perms["o"])
     )
 
 
-def chmod(mode: Union[int, str], path: Union[str, Path], recurse: bool = False) -> None:
+def chmod(path: Union[str, Path], mode: Union[int, str], recurse: bool = False) -> None:
     """
     Change the mode (permissions) of a specified file or directory.
 
     The mode can be specified as an integer, a string representing an octal integer
     or as a string representing symbolic permissions (e.g., 'u=rwx,g=r,o=r').
 
     Parameters
     ----------
+    path : str or Path
+        The path to the file or directory whose mode is to be changed.
     mode : int or str
         The mode (permissions) to be applied to the file or directory. The mode can
         be specified either as an integer, a string of digits (which are parsed as
         an octal integer), or as a string representing symbolic permissions (e.g.,
         'u=rwx,g=r,o=r').
-    path : str or Path
-        The path to the file or directory whose mode is to be changed.
     recurse : bool (default False)
         If true and "path" is a directory, do a depth-first recursion applying `mode`
         to the directory and all objects below it.
 
     Returns
     -------
     None
@@ -215,38 +215,38 @@
         If the user does not have sufficient privileges to change the mode.
     ValueError
         If the specified mode is invalid.
 
     Examples
     --------
     # Change the mode of a file using an octal integer:
-    chmod(0o755, '/path/to/file')
+    chmod('/path/to/file', 0o755)
 
     # Change the mode of a file using a digit string:
-    chmod('755', '/path/to/file')
+    chmod('/path/to/file', '755')
 
     # Change the mode of a directory using symbolic permissions
-    chmod('u=rwx,g=rx,o=r', '/path/to/directory')
+    chmod('/path/to/directory', 'u=rwx,g=rx,o=r')
     """
 
-    def recurse_chmod(mode: Union[int, str], directory: Union[str, Path]) -> None:
+    def recurse_chmod(directory: Union[str, Path], mode: Union[int, str]) -> None:
         "Recursively apply chmod"
         for dir_path, dirnames, filenames in os.walk(directory, topdown=False):
             for filename in filenames:
-                chmod(mode, os.path.join(dir_path, filename), recurse=False)
+                chmod(os.path.join(dir_path, filename), mode, recurse=False)
             for dirname in dirnames:
-                chmod(mode, os.path.join(dir_path, dirname), recurse=False)
+                chmod(os.path.join(dir_path, dirname), mode, recurse=False)
 
     mode_is_sym_str = type(mode) is str and not set(mode).issubset("01234567")
 
     if recurse or mode_is_sym_str:
         path_stat = os.stat(path)
         path_is_directory = stat.S_ISDIR(path_stat.st_mode)
         if path_is_directory and recurse:
-            recurse_chmod(mode, path)
+            recurse_chmod(path, mode)
 
     if type(mode) is str:
         if not mode_is_sym_str:
             mode = int(mode, 8)
         else:
             path_mode = stat.S_IMODE(path_stat.st_mode)  # type: ignore
             mode = symbolic_to_numeric_permissions(
```

### Comparing `symbolicmode-1.0.1/src/symbolicmode.egg-info/PKG-INFO` & `symbolicmode-2.0.0/src/symbolicmode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symbolicmode
-Version: 1.0.1
+Version: 2.0.0
 Summary: Code to handle symbolic permissions like GNU chmod does ('a=rx,u+w')
 Author-email: Sean Reifschneider <jafo00@gmail.com>
 Project-URL: Homepage, https://github.com/linsomniac/symbolicmode
 Project-URL: Bug Tracker, https://github.com/linsomniac/symbolicmode/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

### Comparing `symbolicmode-1.0.1/tests/test_chmod.py` & `symbolicmode-2.0.0/tests/test_chmod.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,44 +14,44 @@
 
     def tearDown(self):
         os.unlink(self.tmp_file.name)
         self.tmp_dir.cleanup()
 
     def test_chmod_octal_integer(self):
         new_mode = 0o755
-        chmod(0o755, self.tmp_file.name)
+        chmod(self.tmp_file.name, 0o755)
         self.assertEqual(stat.S_IMODE(os.stat(self.tmp_file.name).st_mode), 0o755)
 
     def test_chmod_octal_string(self):
-        chmod("755", self.tmp_file.name)
+        chmod(self.tmp_file.name, "755")
         self.assertEqual(stat.S_IMODE(os.stat(self.tmp_file.name).st_mode), 0o755)
 
     def test_chmod_symbolic_permissions(self):
         new_mode = "u=rwx,g=rx,o=r"
-        chmod(new_mode, self.tmp_dir.name)
+        chmod(self.tmp_dir.name, new_mode)
         self.assertEqual(stat.S_IMODE(os.stat(self.tmp_dir.name).st_mode), 0o754)
 
     def test_recursive(self):
         topdir = os.path.join(self.tmp_dir.name, "topdir")
         os.mkdir(topdir)
         topfile = os.path.join(topdir, "topfile")
         with open(topfile, "w") as fp:
             fp.write("TopFile")
         lowerdir = os.path.join(topdir, "lowerdir")
         os.mkdir(lowerdir)
         lowerfile = os.path.join(lowerdir, "lowerfile")
         with open(lowerfile, "w") as fp:
             fp.write("LowerFile")
 
-        chmod("u=rx,go=", topdir, recurse=True)
+        chmod(topdir, "u=rx,go=", recurse=True)
         self.assertEqual(stat.S_IMODE(os.stat(topdir).st_mode), 0o500)
         self.assertEqual(stat.S_IMODE(os.stat(topfile).st_mode), 0o500)
         self.assertEqual(stat.S_IMODE(os.stat(lowerdir).st_mode), 0o500)
         self.assertEqual(stat.S_IMODE(os.stat(lowerfile).st_mode), 0o500)
 
         #  clean up, allow removal
-        chmod("u=rwx,go=", topdir, recurse=True)
+        chmod(topdir, "u=rwx,go=", recurse=True)
 
 
 # Run the unit tests
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `symbolicmode-1.0.1/tests/test_modes.py` & `symbolicmode-2.0.0/tests/test_modes.py`

 * *Files identical despite different names*

