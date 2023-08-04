# Comparing `tmp/terragrunt-generator-0.7.1.tar.gz` & `tmp/terragrunt-generator-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terragrunt-generator-0.7.1.tar", last modified: Thu Aug  3 09:44:24 2023, max compression
+gzip compressed data, was "terragrunt-generator-0.7.2.tar", last modified: Fri Aug  4 14:35:01 2023, max compression
```

## Comparing `terragrunt-generator-0.7.1.tar` & `terragrunt-generator-0.7.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:44:24.820448 terragrunt-generator-0.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-08-03 09:44:24.820448 terragrunt-generator-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:44:24.820448 terragrunt-generator-0.7.1/generator/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-03 09:44:14.000000 terragrunt-generator-0.7.1/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/generator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/generator/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/generator/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/generator/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/generator/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/generator/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/generator/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-03 09:44:14.000000 terragrunt-generator-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 09:44:24.820448 terragrunt-generator-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:44:24.820448 terragrunt-generator-0.7.1/terragrunt_generator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-08-03 09:44:24.000000 terragrunt-generator-0.7.1/terragrunt_generator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-03 09:44:24.000000 terragrunt-generator-0.7.1/terragrunt_generator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:44:24.000000 terragrunt-generator-0.7.1/terragrunt_generator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-03 09:44:24.000000 terragrunt-generator-0.7.1/terragrunt_generator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-03 09:44:24.000000 terragrunt-generator-0.7.1/terragrunt_generator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-03 09:44:24.000000 terragrunt-generator-0.7.1/terragrunt_generator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:44:24.820448 terragrunt-generator-0.7.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14220 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/tests/test_get_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-03 09:44:04.000000 terragrunt-generator-0.7.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:35:01.762331 terragrunt-generator-0.7.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-08-04 14:35:01.762331 terragrunt-generator-0.7.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21046 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:35:01.762331 terragrunt-generator-0.7.2/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-08-04 14:34:48.000000 terragrunt-generator-0.7.2/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/generator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/generator/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/generator/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/generator/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/generator/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/generator/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/generator/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-08-04 14:34:48.000000 terragrunt-generator-0.7.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 14:35:01.762331 terragrunt-generator-0.7.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:35:01.762331 terragrunt-generator-0.7.2/terragrunt_generator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-08-04 14:35:01.000000 terragrunt-generator-0.7.2/terragrunt_generator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-08-04 14:35:01.000000 terragrunt-generator-0.7.2/terragrunt_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:35:01.000000 terragrunt-generator-0.7.2/terragrunt_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-04 14:35:01.000000 terragrunt-generator-0.7.2/terragrunt_generator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-04 14:35:01.000000 terragrunt-generator-0.7.2/terragrunt_generator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-04 14:35:01.000000 terragrunt-generator-0.7.2/terragrunt_generator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:35:01.762331 terragrunt-generator-0.7.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15916 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/tests/test_get_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-04 14:34:35.000000 terragrunt-generator-0.7.2/tests/test_utils.py
```

### Comparing `terragrunt-generator-0.7.1/COPYING` & `terragrunt-generator-0.7.2/COPYING`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.1/PKG-INFO` & `terragrunt-generator-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terragrunt-generator
-Version: 0.7.1
+Version: 0.7.2
 Summary: generate terragrunt manifest from terraform module.
 Author: Chris
 Author-email: goabonga@pm.me
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: COPYING
```

### Comparing `terragrunt-generator-0.7.1/README.md` & `terragrunt-generator-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.1/generator/generate.py` & `terragrunt-generator-0.7.2/generator/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,17 @@
 def generate_locals(
     url: str = None,
     path: str = None,
     version: str = None,
 ) -> str:
     return f"""
 locals {{
-    source = "{url.replace("https://", "").replace("http://", "") if "http" in url else f'{{find_in_parent_folders("{url}")}}' }{f'//{path}' if path != None else ""}{f'?ref={version}' if "http" in url else ""}"
+    source = {
+        f'"{url.replace("https://", "").replace("http://", "")}{f"//{path}" if path != None else ""}?ref={version}"' if "http" in url else f'find_in_parent_folders("{url}")'
+    }
     all = merge(
         yamldecode(file(find_in_parent_folders("config.yaml"))),
     )
 }}
 """
```

### Comparing `terragrunt-generator-0.7.1/generator/main.py` & `terragrunt-generator-0.7.2/generator/main.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.1/generator/yaml.py` & `terragrunt-generator-0.7.2/generator/yaml.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.1/pyproject.toml` & `terragrunt-generator-0.7.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,13 +19,13 @@
   | build
   | dist
 )/
 '''
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.1"
+version = "0.7.2"
 tag_format = "$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:version",
     "generator/__init__.py",
 ]
```

### Comparing `terragrunt-generator-0.7.1/setup.py` & `terragrunt-generator-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.1/terragrunt_generator.egg-info/PKG-INFO` & `terragrunt-generator-0.7.2/terragrunt_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terragrunt-generator
-Version: 0.7.1
+Version: 0.7.2
 Summary: generate terragrunt manifest from terraform module.
 Author: Chris
 Author-email: goabonga@pm.me
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: COPYING
```

### Comparing `terragrunt-generator-0.7.1/terragrunt_generator.egg-info/SOURCES.txt` & `terragrunt-generator-0.7.2/terragrunt_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.1/tests/test_cli.py` & `terragrunt-generator-0.7.2/tests/test_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 #
 
 include {
     path = find_in_parent_folders()
 }
 
 locals {
-    source = "{find_in_parent_folders("./examples/modules/")}"
+    source = find_in_parent_folders("./examples/modules/")
     all = merge(
         yamldecode(file(find_in_parent_folders("config.yaml"))),
     )
 }
 
 terraform {
     source = lookup(local.all.test, "enabled", true) == true ? local.source : null
```

### Comparing `terragrunt-generator-0.7.1/tests/test_generate.py` & `terragrunt-generator-0.7.2/tests/test_generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -431,14 +431,99 @@
   (lookup(local.all.test, "0", null) == null ? {} : { 0 =  lookup(local.all.test, "0") })
 )'''
     assert results == expected
 
     hcl_files: list
     include: bool = True
 
+    url: str = 'test/test_path'
+    path: str = None
+    version: str = '0.1.0'
+    lookup: str = 'test'
+    name: str = 'test'
+
+    hcl_files = {
+        'variable': [
+            {
+                0: {
+                    'name': 'test',
+                    'description': 'A',
+                    'type': 'string',
+                    'default': None,
+                },
+                1: {
+                    'name': 'test1',
+                    'description': 'A',
+                    'type': 'string',
+                    'default': 'hello',
+                },
+                2: {
+                    'name': 'test2',
+                    'description': 'A',
+                    'type': 'string',
+                },
+            }
+        ]
+    }
+
+    results = generate(
+        url,
+        path,
+        version,
+        lookup,
+        hcl_files,
+        include,
+        name,
+    )
+
+    expected = '''# test 0.1.0
+# test/test_path
+#
+# yaml config
+# ```
+# test:
+#   enabled: true
+#   # 2 - A
+#   2: 
+#   # 1 - A
+#   # 1: "hello"
+#   # 0 - A
+#   # 0: 
+# ```
+#
+
+include {
+    path = find_in_parent_folders()
+}
+
+locals {
+    source = find_in_parent_folders("test/test_path")
+    all = merge(
+        yamldecode(file(find_in_parent_folders("config.yaml"))),
+    )
+}
+
+terraform {
+    source = lookup(local.all.test, "enabled", true) == true ? local.source : null
+}
+
+inputs = merge({
+    # 2 - A - required
+    2 = lookup(local.all.test, "2", "")
+    # 1 - A
+    1 = lookup(local.all.test, "1", "hello")
+},
+  # 0 - A
+  (lookup(local.all.test, "0", null) == null ? {} : { 0 =  lookup(local.all.test, "0") })
+)'''
+    assert results == expected
+
+    hcl_files: list
+    include: bool = True
+
     url: str = 'https://gitserver.com/test/test.git'
     path: str = 'modules/test'
     version: str = '0.1.0'
     lookup: str = 'test'
     name: str = 'test'
 
     hcl_files = {
```

### Comparing `terragrunt-generator-0.7.1/tests/test_get_yaml.py` & `terragrunt-generator-0.7.2/tests/test_get_yaml.py`

 * *Files identical despite different names*

### Comparing `terragrunt-generator-0.7.1/tests/test_reader.py` & `terragrunt-generator-0.7.2/tests/test_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,7 +34,18 @@
 @patch('builtins.open', new_callable=mock_open, read_data=data)
 def test_read_directory(mock_file, mock_directory):
     path = 'path/to/open'
     results = read_directory(path)
     mock_directory.assert_called_with(path)
     mock_file.assert_called_with(f'{path}/test.tf')
     assert results == {'variable': [{'test': {'default': '', 'type': 'string'}}]}
+
+
+@patch('os.listdir', return_value=['test.tf', 'test.tf'])
+@patch('builtins.open', new_callable=mock_open, read_data=data)
+@patch('hcl2.load', MagicMock(side_effect=Exception('mocked error')))
+def test_read_directory_except(mock_file, mock_directory):
+    path = 'path/to/open'
+    results = read_directory(path)
+    mock_directory.assert_called_with(path)
+    mock_file.assert_called_with(f'{path}/test.tf')
+    assert results == {}
```

