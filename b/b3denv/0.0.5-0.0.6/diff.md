# Comparing `tmp/b3denv-0.0.5.tar.gz` & `tmp/b3denv-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b3denv-0.0.5.tar", last modified: Fri Jun 23 16:25:06 2023, max compression
+gzip compressed data, was "b3denv-0.0.6.tar", last modified: Fri Aug  4 15:40:25 2023, max compression
```

## Comparing `b3denv-0.0.5.tar` & `b3denv-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-06-23 16:25:06.728673 b3denv-0.0.5/
--rw-r--r--   0 robstenson   (501) staff       (20)      453 2023-06-23 16:25:06.728531 b3denv-0.0.5/PKG-INFO
--rw-r--r--   0 robstenson   (501) staff       (20)      430 2023-01-18 18:25:39.000000 b3denv-0.0.5/README.md
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-06-23 16:25:06.727460 b3denv-0.0.5/b3denv/
--rw-r--r--   0 robstenson   (501) staff       (20)    10333 2023-06-23 16:24:37.000000 b3denv-0.0.5/b3denv/__init__.py
--rw-r--r--   0 robstenson   (501) staff       (20)       62 2022-11-09 19:31:16.000000 b3denv-0.0.5/b3denv/__main__.py
-drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-06-23 16:25:06.728369 b3denv-0.0.5/b3denv.egg-info/
--rw-r--r--   0 robstenson   (501) staff       (20)      453 2023-06-23 16:25:06.000000 b3denv-0.0.5/b3denv.egg-info/PKG-INFO
--rw-r--r--   0 robstenson   (501) staff       (20)      209 2023-06-23 16:25:06.000000 b3denv-0.0.5/b3denv.egg-info/SOURCES.txt
--rw-r--r--   0 robstenson   (501) staff       (20)        1 2023-06-23 16:25:06.000000 b3denv-0.0.5/b3denv.egg-info/dependency_links.txt
--rw-r--r--   0 robstenson   (501) staff       (20)       39 2023-06-23 16:25:06.000000 b3denv-0.0.5/b3denv.egg-info/entry_points.txt
--rw-r--r--   0 robstenson   (501) staff       (20)        7 2023-06-23 16:25:06.000000 b3denv-0.0.5/b3denv.egg-info/top_level.txt
--rw-r--r--   0 robstenson   (501) staff       (20)       38 2023-06-23 16:25:06.728764 b3denv-0.0.5/setup.cfg
--rw-r--r--   0 robstenson   (501) staff       (20)      744 2023-06-23 16:24:37.000000 b3denv-0.0.5/setup.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-08-04 15:40:25.665393 b3denv-0.0.6/
+-rw-r--r--   0 robstenson   (501) staff       (20)    11341 2023-08-04 15:38:30.000000 b3denv-0.0.6/LICENSE
+-rw-r--r--   0 robstenson   (501) staff       (20)      475 2023-08-04 15:40:25.665257 b3denv-0.0.6/PKG-INFO
+-rw-r--r--   0 robstenson   (501) staff       (20)      430 2023-01-18 18:25:39.000000 b3denv-0.0.6/README.md
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-08-04 15:40:25.664428 b3denv-0.0.6/b3denv/
+-rw-r--r--   0 robstenson   (501) staff       (20)    10333 2023-08-04 15:40:08.000000 b3denv-0.0.6/b3denv/__init__.py
+-rw-r--r--   0 robstenson   (501) staff       (20)       62 2022-11-09 19:31:16.000000 b3denv-0.0.6/b3denv/__main__.py
+drwxr-xr-x   0 robstenson   (501) staff       (20)        0 2023-08-04 15:40:25.665083 b3denv-0.0.6/b3denv.egg-info/
+-rw-r--r--   0 robstenson   (501) staff       (20)      475 2023-08-04 15:40:25.000000 b3denv-0.0.6/b3denv.egg-info/PKG-INFO
+-rw-r--r--   0 robstenson   (501) staff       (20)      217 2023-08-04 15:40:25.000000 b3denv-0.0.6/b3denv.egg-info/SOURCES.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)        1 2023-08-04 15:40:25.000000 b3denv-0.0.6/b3denv.egg-info/dependency_links.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)       39 2023-08-04 15:40:25.000000 b3denv-0.0.6/b3denv.egg-info/entry_points.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)        7 2023-08-04 15:40:25.000000 b3denv-0.0.6/b3denv.egg-info/top_level.txt
+-rw-r--r--   0 robstenson   (501) staff       (20)       38 2023-08-04 15:40:25.665433 b3denv-0.0.6/setup.cfg
+-rw-r--r--   0 robstenson   (501) staff       (20)      744 2023-08-04 15:38:40.000000 b3denv-0.0.6/setup.py
```

### Comparing `b3denv-0.0.5/b3denv/__init__.py` & `b3denv-0.0.6/b3denv/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         else:
             if a.startswith("-"):
                 dashes.append(a)
             else:
                 args.append(a)
     
     if "-v" in dashes or "--version" in dashes:
-        return "0.0.5"
+        return "0.0.6"
 
     if len(args) == 1:
         print("b3denv <action> <extension-name>?")
         return
 
     action = args[1]
     if len(args) > 2:
```

### Comparing `b3denv-0.0.5/setup.py` & `b3denv-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ### Help with setting up bpy/blender/blender addons
 
 More info available at: [coldtype.xyz](https://coldtype.xyz)
 """
 
 setuptools.setup(
     name="b3denv",
-    version="0.0.5",
+    version="0.0.6",
     author="Rob Stenson / Coldtype",
     author_email="rob@goodhertz.com",
     description="Help with blender python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/stenson/b3denv",
     packages=[
```

