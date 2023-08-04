# Comparing `tmp/tappack-0.2.0.tar.gz` & `tmp/tappack-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tappack-0.2.0.tar", last modified: Mon Apr 10 13:55:34 2023, max compression
+gzip compressed data, was "tappack-0.3.0.tar", last modified: Fri Aug  4 14:27:18 2023, max compression
```

## Comparing `tappack-0.2.0.tar` & `tappack-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:55:34.339856 tappack-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-10 13:55:34.339856 tappack-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-10 13:55:31.000000 tappack-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 13:55:34.339856 tappack-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-10 13:55:31.000000 tappack-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:55:34.335856 tappack-0.2.0/tappack/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 13:55:26.000000 tappack-0.2.0/tappack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-04-10 13:55:26.000000 tappack-0.2.0/tappack/autoexec.be.template
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-10 13:55:31.000000 tappack-0.2.0/tappack/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-10 13:55:26.000000 tappack-0.2.0/tappack/packaging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-10 13:55:31.000000 tappack-0.2.0/tappack/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-04-10 13:55:31.000000 tappack-0.2.0/tappack/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-04-10 13:55:31.000000 tappack-0.2.0/tappack/source.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-10 13:55:31.000000 tappack-0.2.0/tappack/tunnel.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-10 13:55:31.000000 tappack-0.2.0/tappack/version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 13:55:34.339856 tappack-0.2.0/tappack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-04-10 13:55:34.000000 tappack-0.2.0/tappack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-10 13:55:34.000000 tappack-0.2.0/tappack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 13:55:34.000000 tappack-0.2.0/tappack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-10 13:55:34.000000 tappack-0.2.0/tappack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-10 13:55:34.000000 tappack-0.2.0/tappack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-10 13:55:34.000000 tappack-0.2.0/tappack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:27:18.503270 tappack-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-08-04 14:27:18.503270 tappack-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-08-04 14:27:11.000000 tappack-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 14:27:18.503270 tappack-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-08-04 14:27:11.000000 tappack-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:27:18.499270 tappack-0.3.0/tappack/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 14:27:11.000000 tappack-0.3.0/tappack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-08-04 14:27:16.000000 tappack-0.3.0/tappack/autoexec.be.template
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-04 14:27:11.000000 tappack-0.3.0/tappack/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-04 14:27:11.000000 tappack-0.3.0/tappack/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-04 14:27:11.000000 tappack-0.3.0/tappack/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-08-04 14:27:16.000000 tappack-0.3.0/tappack/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-08-04 14:27:16.000000 tappack-0.3.0/tappack/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-08-04 14:27:11.000000 tappack-0.3.0/tappack/tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 14:27:16.000000 tappack-0.3.0/tappack/version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 14:27:18.503270 tappack-0.3.0/tappack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-08-04 14:27:18.000000 tappack-0.3.0/tappack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-04 14:27:18.000000 tappack-0.3.0/tappack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 14:27:18.000000 tappack-0.3.0/tappack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-04 14:27:18.000000 tappack-0.3.0/tappack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 14:27:18.000000 tappack-0.3.0/tappack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-04 14:27:18.000000 tappack-0.3.0/tappack.egg-info/top_level.txt
```

### Comparing `tappack-0.2.0/PKG-INFO` & `tappack-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tappack
-Version: 0.2.0
+Version: 0.3.0
 Summary: A packager for Tasmota Berry Application (TAPP) apps
 Home-page: https://link.frontmatter.ai/tappack
 Author: Frontmatter
 License: Copyright © 2023 Frontmatter. All rights reserved.
 Keywords: development berry script tasmota tapp
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `tappack-0.2.0/README.md` & `tappack-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tappack-0.2.0/setup.py` & `tappack-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `tappack-0.2.0/tappack/packaging.py` & `tappack-0.3.0/tappack/packaging.py`

 * *Files identical despite different names*

### Comparing `tappack-0.2.0/tappack/patch.py` & `tappack-0.3.0/tappack/patch.py`

 * *Files identical despite different names*

### Comparing `tappack-0.2.0/tappack/server.py` & `tappack-0.3.0/tappack/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 import threading
 from pathlib import Path
 from time import sleep
 
 import click
 
 from tappack.constants import CODE_MASK_DEFAULT
@@ -11,14 +12,15 @@
     from flask import Flask, send_file
     from tappack.tunnel import Tunnel
 except ImportError as exception:  # pragma: no cover
     msg = f'Running tappack server requires additional dependencies. ' \
           f'To install them, run: pip install tappack[server] --upgrade'
     raise ImportError(msg) from exception
 
+CHANNEL_ID_NONE = 'none'
 
 class TappServer:
 
     def __init__(self, paths, port=8080, channel_id=None):
 
         self.port = port
         self.paths = paths
@@ -68,26 +70,30 @@
 
 def start(paths, port, channel_id):
     with TappServer(paths, port, channel_id=channel_id) as tapp_server:
         with Tunnel(port) as tunnel:
             for name, packager in tapp_server.packagers.items():
                 url_tapp = f'{tunnel.tunnel.public_url}/{name}.tapp'
                 code_mask = packager.code_mask or CODE_MASK_DEFAULT
+                code_mask = re.sub(r'\s+', ' ', code_mask).strip()
                 code_snippet = code_mask.format(url=url_tapp, name=name)
                 msg = f'Serving project "{name}": `{code_snippet}`'
                 print(msg)
             tapp_server.wait()
 
 
 @click.command()
 @click.option('--project', '-p', multiple=True, metavar='PATH', required=True)
 @click.option('--port', '-pt', default=8080, show_default=True)
 @click.option('--channel-id', '-id', type=str, default='development',
               help='Identifier for the release channel. '
                    'Only relevant if your manifests contain release channel information. Example: development'
               )
 def main(project, port, channel_id):
+    if channel_id == CHANNEL_ID_NONE:
+        channel_id = None
+
     start(project, port, channel_id)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `tappack-0.2.0/tappack/source.py` & `tappack-0.3.0/tappack/source.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,20 +8,23 @@
 import yaml
 
 from tappack.constants import ENCODING, NAME_MANIFEST
 from tappack.patch import Version
 
 
 def from_manifest(classes, data, channel_id, extra_args=None):
-    class_map = {cls.__name__: cls for cls in classes}
+    class_map = {cls.__name__: cls for cls in classes or {}}
 
     channels = data.get('.channels', {})
     if channel_id in channels:
         data = channels[channel_id]
 
+    if not classes:
+        return data
+
     class_name = data.pop('.type', None)
     source_class = class_map.get(class_name)
     if source_class is None:
         if channels:
             return None
         else:
             raise ValueError(f"Invalid object type: {class_name}")
@@ -62,14 +65,15 @@
                 logging.warning(msg)
 
             self.manifest = {}
 
         self.dependencies = list(self.get_dependencies())
         self.patches = self.get_patches()
         self.code_mask = self.manifest.get('code_mask')
+        self.autoexec = from_manifest(None, self.manifest.get('autoexec', {}), self.channel_id)
 
     def iter_files(self, prefix=None):
         """
 
         Generator that recursively iterates any files in the specified path, then any files in any sub-dependencies,
         passing down the current path prefix, plus the name of the dependency. This yields tuples containing the
         relative path of each file paired with the file data as bytes.
@@ -114,15 +118,22 @@
 
         paths = self.get_submodule_paths(file_data)
         paths = [str(path) for path in paths]
 
         path = Path(__file__).absolute().resolve().parent / 'autoexec.be.template'
         text = path.read_text(encoding=ENCODING)
 
-        replacements = {'paths': repr(paths), 'module_name': self.name}
+        auto_import = str(bool(self.autoexec.get('import'))).lower()
+
+        replacements = {
+            'paths': repr(paths),
+            'module_name': self.name,
+            'import': auto_import,
+            'channel_id': repr(self.channel_id) if self.channel_id else 'nil'
+        }
 
         for key, replacement in replacements.items():
             text = text.replace(f'{{{key}}}', replacement)
 
         print(f'Added submodule paths to autoexec.be: {paths}')
 
         return text
```

### Comparing `tappack-0.2.0/tappack/tunnel.py` & `tappack-0.3.0/tappack/tunnel.py`

 * *Files identical despite different names*

### Comparing `tappack-0.2.0/tappack.egg-info/PKG-INFO` & `tappack-0.3.0/tappack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tappack
-Version: 0.2.0
+Version: 0.3.0
 Summary: A packager for Tasmota Berry Application (TAPP) apps
 Home-page: https://link.frontmatter.ai/tappack
 Author: Frontmatter
 License: Copyright © 2023 Frontmatter. All rights reserved.
 Keywords: development berry script tasmota tapp
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

