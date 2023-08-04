# Comparing `tmp/WignerSymbol-0.0.6.tar.gz` & `tmp/WignerSymbol-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "WignerSymbol-0.0.6.tar", last modified: Tue Aug  1 12:56:59 2023, max compression
+gzip compressed data, was "WignerSymbol-0.0.7.tar", last modified: Fri Aug  4 04:22:09 2023, max compression
```

## Comparing `WignerSymbol-0.0.6.tar` & `WignerSymbol-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 12:56:59.677274 WignerSymbol-0.0.6/
--rw-rw-rw-   0        0        0     1080 2023-06-10 12:36:47.000000 WignerSymbol-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      523 2023-08-01 12:56:59.677274 WignerSymbol-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-06-10 13:25:00.000000 WignerSymbol-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 12:56:59.676274 WignerSymbol-0.0.6/WignerSymbol.egg-info/
--rw-rw-rw-   0        0        0      523 2023-08-01 12:56:59.000000 WignerSymbol-0.0.6/WignerSymbol.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-08-01 12:56:59.000000 WignerSymbol-0.0.6/WignerSymbol.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 12:56:59.000000 WignerSymbol-0.0.6/WignerSymbol.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-01 12:56:58.000000 WignerSymbol-0.0.6/WignerSymbol.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       13 2023-08-01 12:56:59.000000 WignerSymbol-0.0.6/WignerSymbol.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3403 2023-06-10 12:52:17.000000 WignerSymbol-0.0.6/lib.cpp
--rw-rw-rw-   0        0        0      108 2023-06-10 13:15:34.000000 WignerSymbol-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 12:56:59.678277 WignerSymbol-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      925 2023-08-01 12:49:53.000000 WignerSymbol-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:22:09.715169 WignerSymbol-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-08-04 04:21:51.000000 WignerSymbol-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-04 04:21:51.000000 WignerSymbol-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-04 04:22:09.715169 WignerSymbol-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-08-04 04:21:51.000000 WignerSymbol-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:22:09.715169 WignerSymbol-0.0.7/WignerSymbol/
+-rw-r--r--   0 runner    (1001) docker     (123)    36389 2023-08-04 04:21:52.000000 WignerSymbol-0.0.7/WignerSymbol/WignerSymbol.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 04:22:09.715169 WignerSymbol-0.0.7/WignerSymbol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-08-04 04:22:09.000000 WignerSymbol-0.0.7/WignerSymbol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-04 04:22:09.000000 WignerSymbol-0.0.7/WignerSymbol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 04:22:09.000000 WignerSymbol-0.0.7/WignerSymbol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 04:22:09.000000 WignerSymbol-0.0.7/WignerSymbol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-04 04:22:09.000000 WignerSymbol-0.0.7/WignerSymbol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-08-04 04:21:51.000000 WignerSymbol-0.0.7/lib.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-04 04:21:51.000000 WignerSymbol-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 04:22:09.715169 WignerSymbol-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-08-04 04:21:51.000000 WignerSymbol-0.0.7/setup.py
```

### Comparing `WignerSymbol-0.0.6/LICENSE` & `WignerSymbol-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `WignerSymbol-0.0.6/lib.cpp` & `WignerSymbol-0.0.7/lib.cpp`

 * *Files identical despite different names*

### Comparing `WignerSymbol-0.0.6/setup.py` & `WignerSymbol-0.0.7/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 from pathlib import Path
 
 this_dir = Path(__file__).parent
 long_description = (this_dir / "README.md").read_text()
 
-__version__ = "0.0.6"
+__version__ = "0.0.7"
 
 ext_modules = [
     Pybind11Extension("WignerSymbol",
                       ["lib.cpp"],
                       define_macros=[("VERSION", __version__)],
-                      include_dirs=[this_dir],
                       ),
 ]
 
 setup(
     name='WignerSymbol',
     version=__version__,
     author="0382",
     author_email="18322825326@163.com",
+    license="MIT",
     url="https://github.com/0382/WignerSymbol-pybind11",
     description="Python port of 0382/WignerSymbol",
     long_description=long_description,
     long_description_content_type="text/markdown",
     ext_modules=ext_modules,
     cmdclass={"build_ext": build_ext},
     zip_safe=False,
```

