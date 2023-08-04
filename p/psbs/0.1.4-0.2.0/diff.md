# Comparing `tmp/psbs-0.1.4.tar.gz` & `tmp/psbs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psbs-0.1.4.tar", last modified: Fri Jun 30 00:51:47 2023, max compression
+gzip compressed data, was "psbs-0.2.0.tar", last modified: Fri Aug  4 01:53:28 2023, max compression
```

## Comparing `psbs-0.1.4.tar` & `psbs-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-30 00:51:47.461061 psbs-0.1.4/
--rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.1.4/LICENSE
--rw-r--r--   0 jcmiller   (501) staff       (20)     5547 2023-06-30 00:51:47.461255 psbs-0.1.4/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)     4874 2023-06-14 19:38:32.000000 psbs-0.1.4/README.md
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-30 00:51:47.456546 psbs-0.1.4/psbs/
--rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.1.4/psbs/__init__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.1.4/psbs/__main__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-06-07 15:11:32.000000 psbs-0.1.4/psbs/config.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      871 2023-06-10 00:05:18.000000 psbs-0.1.4/psbs/example.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)     1146 2023-06-18 20:24:47.000000 psbs-0.1.4/psbs/extension.py
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-30 00:51:47.460441 psbs-0.1.4/psbs/extensions/
--rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-18 20:00:51.000000 psbs-0.1.4/psbs/extensions/__init__.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     3025 2023-06-18 20:24:47.000000 psbs-0.1.4/psbs/extensions/images.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     2721 2023-06-11 15:23:02.000000 psbs-0.1.4/psbs/gister.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     4116 2023-06-18 19:37:14.000000 psbs-0.1.4/psbs/project.py
--rwxr-xr-x   0 jcmiller   (501) staff       (20)     2944 2023-06-19 00:52:39.000000 psbs-0.1.4/psbs/psbs.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1794 2023-06-21 17:31:54.000000 psbs-0.1.4/psbs/psparser.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1548 2023-06-18 20:02:25.000000 psbs-0.1.4/psbs/template.py
--rw-r--r--   0 jcmiller   (501) staff       (20)      728 2023-06-09 22:23:16.000000 psbs-0.1.4/psbs/templatebuilder.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-06-11 15:23:53.000000 psbs-0.1.4/psbs/token.py
--rw-r--r--   0 jcmiller   (501) staff       (20)     1945 2023-06-14 18:47:43.000000 psbs-0.1.4/psbs/utils.py
-drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-06-30 00:51:47.459426 psbs-0.1.4/psbs.egg-info/
--rw-r--r--   0 jcmiller   (501) staff       (20)     5547 2023-06-30 00:51:47.000000 psbs-0.1.4/psbs.egg-info/PKG-INFO
--rw-r--r--   0 jcmiller   (501) staff       (20)      474 2023-06-30 00:51:47.000000 psbs-0.1.4/psbs.egg-info/SOURCES.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-06-30 00:51:47.000000 psbs-0.1.4/psbs.egg-info/dependency_links.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-06-30 00:51:47.000000 psbs-0.1.4/psbs.egg-info/entry_points.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)       43 2023-06-30 00:51:47.000000 psbs-0.1.4/psbs.egg-info/requires.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-06-30 00:51:47.000000 psbs-0.1.4/psbs.egg-info/top_level.txt
--rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-06-30 00:51:47.461874 psbs-0.1.4/setup.cfg
--rw-r--r--   0 jcmiller   (501) staff       (20)     1259 2023-06-30 00:50:30.000000 psbs-0.1.4/setup.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-04 01:53:28.425650 psbs-0.2.0/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1069 2023-06-04 01:40:38.000000 psbs-0.2.0/LICENSE
+-rw-r--r--   0 jcmiller   (501) staff       (20)     6642 2023-08-04 01:53:28.425864 psbs-0.2.0/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)     5970 2023-08-04 01:51:13.000000 psbs-0.2.0/README.md
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-04 01:53:28.419279 psbs-0.2.0/psbs/
+-rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-05 12:31:00.000000 psbs-0.2.0/psbs/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)       32 2023-06-11 15:36:36.000000 psbs-0.2.0/psbs/__main__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      383 2023-07-23 20:27:08.000000 psbs-0.2.0/psbs/config.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      870 2023-07-29 00:01:45.000000 psbs-0.2.0/psbs/example.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1614 2023-08-04 01:50:46.000000 psbs-0.2.0/psbs/extension.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-04 01:53:28.425160 psbs-0.2.0/psbs/extensions/
+-rw-r--r--   0 jcmiller   (501) staff       (20)        0 2023-06-18 20:00:51.000000 psbs-0.2.0/psbs/extensions/__init__.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      568 2023-08-04 01:50:46.000000 psbs-0.2.0/psbs/extensions/build.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)      433 2023-08-04 01:50:46.000000 psbs-0.2.0/psbs/extensions/filters.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     3069 2023-08-04 01:50:46.000000 psbs-0.2.0/psbs/extensions/images.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)    20733 2023-08-04 01:50:46.000000 psbs-0.2.0/psbs/extensions/tiled.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     2916 2023-08-04 01:50:46.000000 psbs-0.2.0/psbs/gister.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     3986 2023-08-04 01:50:46.000000 psbs-0.2.0/psbs/project.py
+-rwxr-xr-x   0 jcmiller   (501) staff       (20)     2944 2023-07-31 14:27:17.000000 psbs-0.2.0/psbs/psbs.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     9509 2023-08-04 01:50:46.000000 psbs-0.2.0/psbs/psparser.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     3044 2023-08-04 01:50:46.000000 psbs-0.2.0/psbs/template.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1118 2023-06-11 15:23:53.000000 psbs-0.2.0/psbs/token.py
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1945 2023-06-14 18:47:43.000000 psbs-0.2.0/psbs/utils.py
+drwxr-xr-x   0 jcmiller   (501) staff       (20)        0 2023-08-04 01:53:28.422733 psbs-0.2.0/psbs.egg-info/
+-rw-r--r--   0 jcmiller   (501) staff       (20)     6642 2023-08-04 01:53:28.000000 psbs-0.2.0/psbs.egg-info/PKG-INFO
+-rw-r--r--   0 jcmiller   (501) staff       (20)      527 2023-08-04 01:53:28.000000 psbs-0.2.0/psbs.egg-info/SOURCES.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        1 2023-08-04 01:53:28.000000 psbs-0.2.0/psbs.egg-info/dependency_links.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       40 2023-08-04 01:53:28.000000 psbs-0.2.0/psbs.egg-info/entry_points.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)       49 2023-08-04 01:53:28.000000 psbs-0.2.0/psbs.egg-info/requires.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)        5 2023-08-04 01:53:28.000000 psbs-0.2.0/psbs.egg-info/top_level.txt
+-rw-r--r--   0 jcmiller   (501) staff       (20)      103 2023-08-04 01:53:28.426504 psbs-0.2.0/setup.cfg
+-rw-r--r--   0 jcmiller   (501) staff       (20)     1277 2023-08-04 01:50:46.000000 psbs-0.2.0/setup.py
```

### Comparing `psbs-0.1.4/LICENSE` & `psbs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psbs-0.1.4/PKG-INFO` & `psbs-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,26 @@
-Metadata-Version: 2.1
-Name: psbs
-Version: 0.1.4
-Summary: PuzzleScript Build System
-Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.4.tar.gz
-Author: J.C. Miller
-Author-email: johncoreymiller@gmail.com
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Games/Entertainment :: Puzzle Games
-Classifier: Topic :: Software Development :: Build Tools
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PSBS
 
 The PuzzleScript Build System!
 
 PSBS combines multiple files into one puzzlescript source file and uploads it to the web.
 
 This is an early development release and changes may be made to the project structure and config file formats in the future.
 
 ## Features
 
- - Compile PuzzleScript games from many files using Jinja2 templates
- - Import images and spritesheets directly into your PuzzleScript game
- - Load existing PuzzleScript projects right from their gists
- - Load existing PuzzleScript projects from a source text file
- - Save PuzzleScript projects to gists
- - Launch your project from play.html or the PuzzleScript editor
- - Supports most PuzzleScript forks including [Pattern:Script](https://github.com/ClementSparrow/Pattern-Script)
- - Use your favorite version control for your PuzzleScript Projects
+ - Compile PuzzleScript games from many files using Jinja2 templates!
+ - Import images and spritesheets directly into your PuzzleScript game!
+ - Load existing PuzzleScript projects right from their gists!
+ - Load existing PuzzleScript projects from a source text file!
+ - Save PuzzleScript projects to gists!
+ - Launch your project from play.html or the PuzzleScript editor!
+ - Supports most PuzzleScript forks!
+ - Use your favorite version control for your PuzzleScript projects!
+ - [Tiled](https://www.mapeditor.org/) level editor integration!
 
 ## Installing
 
 If you already have Python 3.8 or greater and pip installed simply run the following command from your terminal
 
 `pip install psbs`
 
@@ -112,34 +94,76 @@
 - Images:
   - alpha: whether to include the RGBA alpha values for transparency supported by some forks
   - max_colors: maximum colors in output object, PuzzleScript can only handle 10 by default but some forks support up to 36 colors
 
 
 ## Templates
 
-PSBS uses Jinja2, a fast, expressive, extensible templating engine, to build your PuzzleScript project.  To learn more about all of the features available to you check out the Jinja2 [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
+PSBS uses Jinja2, a fast, expressive, extensible templating engine, to build your PuzzleScript project.
+
+I'm currently working on [official documentation](https://jcmiller11.github.io/PSBS/) but this is a work in progress.
+
+To learn more about all of the features available to you check out the Jinja2 [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
 To avoid conflicting with valid PuzzleScript code, the Jinja2 Tags have been changed as follows:
 
-(% blocks %) (( variables )) (# comments #)
+(% statements %) (( expressions )) (# comments #)
 
 ## Images
 
 A helper function has been added to the template environment `Image(filename)` that will import an image file directly into your game as a PuzzleScript object!
 
     Target
     ((image("images/target.png")))
 
-Additionally, this helper function contains the following optional parameters (alpha=False, max_colors=10, x=0, y=0, width=None, height=None)
+Additionally, this helper function contains the following optional parameters (alpha=False, max_colors=10, left=0, top=0, width=None, height=None)
 
-- x: (int) horizontal position in image to start importing from
-- y: (int) vertical position in image to start importing from
+- left: (int) horizontal position in image to start importing from
+- top: (int) vertical position in image to start importing from
 - width: (int) width of the object to import, if None set to the width of the image file
 - height: (int) height of the object to import, if None set to the height of the image file
 
 By using the last four parameters listed one can load objects from a single image as a spritesheet.
 
     (% set directions = ["down","left","up","right"] %) (# Can be placed in your main template #)
     (% for dir in directions %)
     Player_((dir))
-    ((image("images/player.png",x=loop.index0*5,width=5,height=5)))
+    ((image("images/player.png",left=loop.index0*5,width=5,height=5)))
     (% endfor %)
+
+## Tiled
+
+`tiled(filename)`
+
+Imports a [Tiled](https://www.mapeditor.org) map as a level!  If you set generate_tileset to true in your config.yaml PSBS will attempt to generate a Tiled tileset from your game in the bin directory of your project.  Tiled maps made with this tileset can be imported.
+
+Tileset generation not compatible with Pattern:Script at this point in time.
+
+```
+message Welcome to the first level!
+((tiled("src/levels/level1.tmx")))
+
+message Here comes level 2!
+((tiled("src/levels/level2.tmx")))
+```
+
+## Releases
+
+As of PSBS 0.2.0 a release name option has been added to config.yaml, this can be access within your template files using the following functions:
+
+get_build: returns the release name
+
+is_debug: returns true if the release name is "debug"
+
+is_release: returns true if the release name is "release"
+
+```
+(% if is_debug %)
+debug
+verbose_logging
+(% endif %)
+```
+
+```
+markerobject
+(% "transparent" if is_release else "red" %)
+```
```

### Comparing `psbs-0.1.4/psbs/example.txt` & `psbs-0.2.0/psbs/example.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 Target
 Player, Wall, Crate
 
 ======
 RULES
 ======
 
-[ > Player | Crate ] -> [ > Player | > Crate ] 
+[ > Player | Crate ] -> [ > Player | > Crate ]
 
 ==============
 WINCONDITIONS
 ==============
 
 all Target on Crate
```

### Comparing `psbs-0.1.4/psbs/extension.py` & `psbs-0.2.0/psbs/extension.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,34 +3,50 @@
 from importlib import import_module
 from jinja2.exceptions import TemplateError
 
 
 class Extension:
     def __init__(self, config):
         self.methods = {}
+        self.filters = {}
+        self.post = []
         self.config = config
-        if self.get_config():
-            for key, value in self.get_config().items():
-                if key not in self.config:
-                    self.config[key] = None
-                if not self.config[key]:
-                    self.config[key] = value
+        for key, value in self.get_config().items():
+            if key not in self.config:
+                self.config[key] = None
+            if self.config[key] is None:
+                self.config[key] = value
 
     def register(self, name, function):
         if name not in self.methods:
             self.methods[name] = function
 
+    def register_filter(self, name, function):
+        if name not in self.filters:
+            self.filters[name] = function
+
+    def register_post(self, function):
+        self.post.append(function)
+
     @staticmethod
     def get_config():
-        return None
+        return {}
 
     @classmethod
     def get_extensions(cls):
         for extension in glob.glob(
             join(dirname(__file__), "extensions", "*.py")
         ):
             if isfile(extension) and not extension.endswith("__init__.py"):
                 import_module(f"psbs.extensions.{basename(extension)[:-3]}")
         return cls.__subclasses__()
 
+    @classmethod
+    def get_extension_configs(cls):
+        config_dict = {}
+        for extension in cls.get_extensions():
+            if extension.get_config():
+                config_dict[extension.__name__] = extension.get_config()
+        return config_dict
+
     class ExtensionError(TemplateError):
         """Thrown when the extension has a problem with the template"""
```

### Comparing `psbs-0.1.4/psbs/extensions/images.py` & `psbs-0.2.0/psbs/extensions/images.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,41 +45,42 @@
         sprite = wrap(sprite, width)
         sprite = "\n".join(sprite)
         return {"sprite": sprite, "colors": colors}
 
     def image_to_object(
         self,
         file,
-        x=0,
-        y=0,
+        left=0,
+        top=0,
         width=None,
         height=None,
     ):
         if self.config["max_colors"] > 36:
-            raise self.ExtensionError(
-                "Image helper function doesn't support more than 36 colors"
-            )
+            print("Warning: max_colors config values over 36 not supported")
+            self.config["max_colors"] = 36
         if file in self.loaded_images:
             image = self.loaded_images[file]
         else:
             try:
                 image = Image.open(file, "r")
             except IOError as err:
-                raise self.ExtensionError(f"Unable to read image file\n  {err}")
+                raise self.ExtensionError(
+                    f"Unable to read image file\n  {err}"
+                )
             self.loaded_images[file] = image
         # Crop image if needed
         if width:
-            right = x + width
+            right = left + width
         else:
             right = image.size[0]
         if height:
-            bottom = y + height
+            bottom = top + height
         else:
             bottom = image.size[1]
-        image = image.crop((x, y, right, bottom))
+        image = image.crop((left, top, right, bottom))
         image = image.convert("RGBA")
         result = self.__pixel_list_to_sprite(
             image.getdata(), width=image.size[0]
         )
         sprite = result["sprite"]
         colors = result["colors"]
         if len(colors) > 10:
```

### Comparing `psbs-0.1.4/psbs/gister.py` & `psbs-0.2.0/psbs/gister.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,16 +60,20 @@
                 )
             if response.status_code == 422:
                 raise self.GistError("422: Validation failed")
             if response.status_code == 404:
                 raise self.GistError("404: File not found")
             if response.status_code == 403:
                 raise self.GistError("403: Forbidden")
-            if "message" in response:
+            if response.status_code >= 400:
                 raise self.GistError(response)
+            # I can't remember why I was using this
+            # keeping it here in case I remember
+            # if "message" in response:
+            #    raise self.GistError(response)
         except ConnectionError as err:
             print("Error: Unable to connect to GitHub")
             raise SystemExit(1) from err
         except self.GistError as err:
             print(f"Error: Unable to access gist\n  Response: {err}")
             raise SystemExit(1) from err
         return response
```

### Comparing `psbs-0.1.4/psbs/project.py` & `psbs-0.2.0/psbs/project.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from os import path
 from shutil import rmtree
 
 from .gister import Gister
 from .config import Config
-from .psparser import split_ps, get_engine
-from .templatebuilder import make_template
-from .utils import read_file, write_file, write_yaml, make_dir, run_in_browser
-from .template import render_template
+from .psparser import PSParser
+from .template import Template
 from .extension import Extension
+from .utils import read_file, write_file, write_yaml, make_dir, run_in_browser
 
 
 class PSBSProject:
     def __init__(self, config_filename="config.yaml"):
         self.config = Config(config_filename)
 
     def build(self):
@@ -29,20 +28,20 @@
             readme_path,
             "Play this game by pasting the script in "
             f"{self.config['engine']}editor.html",
         )
 
         # Build the script.txt
         print("Building script.txt")
-        source = render_template(
+        template = Template(
             path.join("src", self.config["template"]), self.config
         )
 
         print(f"Writing file {script_path}")
-        write_file(script_path, source)
+        write_file(script_path, template.render())
 
     def upload(self):
         gist_id = self.config["gist_id"]
         if not self.config["gist_id"]:
             print("Error: Unable to upload without a gist_id in config file")
             raise SystemExit(1)
 
@@ -62,56 +61,53 @@
         run_in_browser(url)
 
     @staticmethod
     def create(project_name, gist_id=None, file=None, new_gist=False):
         source = ""
         engine = "https://www.puzzlescript.net/"
 
-        if gist_id:
+        if file:
+            source = read_file(file)
+        elif gist_id:
             print("Downloading data from gist")
             gist = Gister(gist_id=gist_id)
             source = gist.read("script.txt")
-            engine = get_engine(gist.read("readme.txt"))
-        elif file:
-            source = read_file(file)
+            engine = PSParser.get_engine(gist.read("readme.txt"))
         else:
             source = read_file(
                 path.join(path.realpath(path.dirname(__file__)), "example.txt")
             )
 
-        src_tree = split_ps(source)
+        src_tree = PSParser(source).source_tree
 
         if new_gist:
             print("Creating new gist")
             gist = Gister()
             gist_id = gist.create(name=project_name)
 
         config_dict = {
             "gist_id": gist_id,
             "engine": engine,
             "template": "main.pss",
         }
-
-        for extension in Extension.get_extensions():
-            if extension.get_config():
-                config_dict[extension.__name__] = extension.get_config()
+        config_dict.update(Extension.get_extension_configs())
 
         print("Building directory structure")
         make_dir(project_name)
         try:
             make_dir(path.join(project_name, "src"))
             make_dir(path.join(project_name, "bin"))
 
             print("Creating config file")
             write_yaml(path.join(project_name, "config.yaml"), config_dict)
 
             print("Creating template file")
             write_file(
                 path.join(project_name, "src", "main.pss"),
-                make_template(src_tree),
+                Template.make_template(src_tree),
             )
 
             print("Creating source files")
             for section_name, src_blocks in src_tree.items():
                 for index, src_content in enumerate(src_blocks):
                     index += 1
                     if len(src_blocks) == 1:
```

### Comparing `psbs-0.1.4/psbs/psbs.py` & `psbs-0.2.0/psbs/psbs.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.4/psbs/token.py` & `psbs-0.2.0/psbs/token.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.4/psbs/utils.py` & `psbs-0.2.0/psbs/utils.py`

 * *Files identical despite different names*

### Comparing `psbs-0.1.4/psbs.egg-info/PKG-INFO` & `psbs-0.2.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: psbs
-Version: 0.1.4
+Version: 0.2.0
 Summary: PuzzleScript Build System
 Home-page: https://github.com/jcmiller11/PSBS
-Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.4.tar.gz
+Download-URL: https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.0.tar.gz
 Author: J.C. Miller
 Author-email: johncoreymiller@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -23,22 +23,23 @@
 
 PSBS combines multiple files into one puzzlescript source file and uploads it to the web.
 
 This is an early development release and changes may be made to the project structure and config file formats in the future.
 
 ## Features
 
- - Compile PuzzleScript games from many files using Jinja2 templates
- - Import images and spritesheets directly into your PuzzleScript game
- - Load existing PuzzleScript projects right from their gists
- - Load existing PuzzleScript projects from a source text file
- - Save PuzzleScript projects to gists
- - Launch your project from play.html or the PuzzleScript editor
- - Supports most PuzzleScript forks including [Pattern:Script](https://github.com/ClementSparrow/Pattern-Script)
- - Use your favorite version control for your PuzzleScript Projects
+ - Compile PuzzleScript games from many files using Jinja2 templates!
+ - Import images and spritesheets directly into your PuzzleScript game!
+ - Load existing PuzzleScript projects right from their gists!
+ - Load existing PuzzleScript projects from a source text file!
+ - Save PuzzleScript projects to gists!
+ - Launch your project from play.html or the PuzzleScript editor!
+ - Supports most PuzzleScript forks!
+ - Use your favorite version control for your PuzzleScript projects!
+ - [Tiled](https://www.mapeditor.org/) level editor integration!
 
 ## Installing
 
 If you already have Python 3.8 or greater and pip installed simply run the following command from your terminal
 
 `pip install psbs`
 
@@ -112,34 +113,76 @@
 - Images:
   - alpha: whether to include the RGBA alpha values for transparency supported by some forks
   - max_colors: maximum colors in output object, PuzzleScript can only handle 10 by default but some forks support up to 36 colors
 
 
 ## Templates
 
-PSBS uses Jinja2, a fast, expressive, extensible templating engine, to build your PuzzleScript project.  To learn more about all of the features available to you check out the Jinja2 [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
+PSBS uses Jinja2, a fast, expressive, extensible templating engine, to build your PuzzleScript project.
+
+I'm currently working on [official documentation](https://jcmiller11.github.io/PSBS/) but this is a work in progress.
+
+To learn more about all of the features available to you check out the Jinja2 [Template Designer Documentation](https://jinja.palletsprojects.com/en/3.1.x/templates/).
 
 To avoid conflicting with valid PuzzleScript code, the Jinja2 Tags have been changed as follows:
 
-(% blocks %) (( variables )) (# comments #)
+(% statements %) (( expressions )) (# comments #)
 
 ## Images
 
 A helper function has been added to the template environment `Image(filename)` that will import an image file directly into your game as a PuzzleScript object!
 
     Target
     ((image("images/target.png")))
 
-Additionally, this helper function contains the following optional parameters (alpha=False, max_colors=10, x=0, y=0, width=None, height=None)
+Additionally, this helper function contains the following optional parameters (alpha=False, max_colors=10, left=0, top=0, width=None, height=None)
 
-- x: (int) horizontal position in image to start importing from
-- y: (int) vertical position in image to start importing from
+- left: (int) horizontal position in image to start importing from
+- top: (int) vertical position in image to start importing from
 - width: (int) width of the object to import, if None set to the width of the image file
 - height: (int) height of the object to import, if None set to the height of the image file
 
 By using the last four parameters listed one can load objects from a single image as a spritesheet.
 
     (% set directions = ["down","left","up","right"] %) (# Can be placed in your main template #)
     (% for dir in directions %)
     Player_((dir))
-    ((image("images/player.png",x=loop.index0*5,width=5,height=5)))
+    ((image("images/player.png",left=loop.index0*5,width=5,height=5)))
     (% endfor %)
+
+## Tiled
+
+`tiled(filename)`
+
+Imports a [Tiled](https://www.mapeditor.org) map as a level!  If you set generate_tileset to true in your config.yaml PSBS will attempt to generate a Tiled tileset from your game in the bin directory of your project.  Tiled maps made with this tileset can be imported.
+
+Tileset generation not compatible with Pattern:Script at this point in time.
+
+```
+message Welcome to the first level!
+((tiled("src/levels/level1.tmx")))
+
+message Here comes level 2!
+((tiled("src/levels/level2.tmx")))
+```
+
+## Releases
+
+As of PSBS 0.2.0 a release name option has been added to config.yaml, this can be access within your template files using the following functions:
+
+get_build: returns the release name
+
+is_debug: returns true if the release name is "debug"
+
+is_release: returns true if the release name is "release"
+
+```
+(% if is_debug %)
+debug
+verbose_logging
+(% endif %)
+```
+
+```
+markerobject
+(% "transparent" if is_release else "red" %)
+```
```

### Comparing `psbs-0.1.4/setup.py` & `psbs-0.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,33 +3,34 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='psbs',
-    version='0.1.4',
+    version='0.2.0',
     python_requires='>=3.8',
     description='PuzzleScript Build System',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='J.C. Miller',
     author_email='johncoreymiller@gmail.com',
     url='https://github.com/jcmiller11/PSBS',
-    download_url = 'https://github.com/jcmiller11/PSBS/archive/refs/tags/0.1.4.tar.gz',
+    download_url = 'https://github.com/jcmiller11/PSBS/archive/refs/tags/0.2.0.tar.gz',
     license='MIT',
     packages=find_packages(),
     package_data={'': ['example.txt']},
     include_package_data=True,
     install_requires=[
         'jinja2',
         'pyyaml',
         'Pillow',
         'platformdirs',
-        'requests'
+        'requests',
+        'numpy'
     ],
 
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
@@ -37,8 +38,8 @@
         'Topic :: Software Development :: Build Tools'
     ],
     entry_points={
         'console_scripts': [
             'psbs=psbs.psbs:main'
         ],
     },
-)
+)
```

