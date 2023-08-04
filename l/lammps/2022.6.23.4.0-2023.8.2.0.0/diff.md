# Comparing `tmp/lammps-2022.6.23.4.0.tar.gz` & `tmp/lammps-2023.8.2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lammps-2022.6.23.4.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "lammps-2023.8.2.0.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `lammps-2022.6.23.4.0.tar` & `lammps-2023.8.2.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      382 2022-11-09 12:37:21.000000 lammps-2022.6.23.4.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     2823 2022-11-09 12:37:21.000000 lammps-2022.6.23.4.0/.github/workflows/wheel.yml
--rw-r--r--   0        0        0     1066 2022-11-09 12:37:21.000000 lammps-2022.6.23.4.0/CMakeLists.txt
--rw-r--r--   0        0        0    18059 2022-11-09 12:37:21.000000 lammps-2022.6.23.4.0/LICENSE
--rw-r--r--   0        0        0     1703 2022-11-09 12:37:21.000000 lammps-2022.6.23.4.0/README.md
--rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 lammps-2022.6.23.4.0/lammps/__init__.py
--rw-r--r--   0        0        0      925 2022-11-09 12:37:21.000000 lammps-2022.6.23.4.0/lammps/executable.py
--rw-r--r--   0        0        0     2090 2022-11-09 12:37:21.000000 lammps-2022.6.23.4.0/pyproject.toml
--rw-r--r--   0        0        0       27 2022-11-09 12:37:21.000000 lammps-2022.6.23.4.0/tests/test_import.py
--rw-r--r--   0        0        0    22969 2022-11-09 12:37:21.000000 lammps-2022.6.23.4.0/PKG-INFO
+-rw-r--r--   0        0        0      382 2022-11-09 12:37:21.000000 lammps-2023.8.2.0.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2844 2022-11-09 12:37:21.000000 lammps-2023.8.2.0.0/.github/workflows/wheel.yml
+-rw-r--r--   0        0        0     1067 2022-11-09 12:37:21.000000 lammps-2023.8.2.0.0/CMakeLists.txt
+-rw-r--r--   0        0        0    18059 2022-11-09 12:37:21.000000 lammps-2023.8.2.0.0/LICENSE
+-rw-r--r--   0        0        0     1703 2022-11-09 12:37:21.000000 lammps-2023.8.2.0.0/README.md
+-rw-r--r--   0        0        0      524 2022-11-09 12:37:21.000000 lammps-2023.8.2.0.0/lammps/__init__.py
+-rw-r--r--   0        0        0      925 2022-11-09 12:37:21.000000 lammps-2023.8.2.0.0/lammps/executable.py
+-rw-r--r--   0        0        0     2064 2022-11-09 12:37:21.000000 lammps-2023.8.2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       27 2022-11-09 12:37:21.000000 lammps-2023.8.2.0.0/tests/test_import.py
+-rw-r--r--   0        0        0    22968 2022-11-09 12:37:21.000000 lammps-2023.8.2.0.0/PKG-INFO
```

### Comparing `lammps-2022.6.23.4.0/.github/workflows/wheel.yml` & `lammps-2023.8.2.0.0/.github/workflows/wheel.yml`

 * *Files 9% similar despite different names*

```diff
@@ -88,17 +88,17 @@
         with:
           path: dist/*.tar.gz
 
   upload_pypi:
     needs: [build_wheels, build_sdist]
     runs-on: ubuntu-latest
     if: github.event_name == 'push' && startsWith(github.event.ref, 'refs/tags/v')
+    permissions:
+        # IMPORTANT: this permission is mandatory for trusted publishing
+        id-token: write
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@master
-        with:
-          user: __token__
-          password: ${{ secrets.PYPI_PASSWORD }}
+      - uses: pypa/gh-action-pypi-publish@v1
```

### Comparing `lammps-2022.6.23.4.0/CMakeLists.txt` & `lammps-2023.8.2.0.0/CMakeLists.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 endif()
 set(CMAKE_INSTALL_BINDIR .)
 set(CMAKE_INSTALL_LIBDIR .)
 
 # download LAMMPS to ${LAMMPS_SOURCE_ROOT}
 include(FetchContent)
 FetchContent_Declare(lammps
-  GIT_REPOSITORY    https://github.com/njzjz/lammps
+  GIT_REPOSITORY    https://github.com/lammps/lammps
   GIT_TAG           ${LAMMPS_VERSION}
 )
 FetchContent_GetProperties(lammps)
 if(NOT lammps_POPULATED)
   FetchContent_Populate(lammps)
   include(${lammps_SOURCE_DIR}/cmake/presets/most.cmake)
   if (WIN32)
```

### Comparing `lammps-2022.6.23.4.0/LICENSE` & `lammps-2023.8.2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lammps-2022.6.23.4.0/README.md` & `lammps-2023.8.2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `lammps-2022.6.23.4.0/lammps/__init__.py` & `lammps-2023.8.2.0.0/lammps/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 """
 
 from .constants import *                # lgtm [py/polluting-import]
 from .core import *                     # lgtm [py/polluting-import]
 from .data import *                     # lgtm [py/polluting-import]
 from .pylammps import *                 # lgtm [py/polluting-import]
 
-__version__ = 20220623
+__version__ = 20230802
```

### Comparing `lammps-2022.6.23.4.0/lammps/executable.py` & `lammps-2023.8.2.0.0/lammps/executable.py`

 * *Files identical despite different names*

### Comparing `lammps-2022.6.23.4.0/pyproject.toml` & `lammps-2023.8.2.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["scikit-build-core>=0.1.4"]
 build-backend = "scikit_build_core.build"
 
 [project]
 name = "lammps"
-version = "2022.6.23.4.0"
+version = "2023.8.2.0.0"
 description = "unoffical LAMMPS Molecular Dynamics Python package"
 authors = [
   {name = "The LAMMPS Developers", email = "developers@lammps.org"},
   {name = "Jinzhe Zeng", email = "jinzhe.zeng@rutgers.edu"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
@@ -33,15 +33,15 @@
 [project.scripts]
 lmp = "lammps.executable:lmp"
 
 [tool.scikit-build]
 wheel.install-dir = "lammps"
 wheel.py-api = "py2.py3"
 cmake.args = [
-    "-D LAMMPS_VERSION=93fc33a5504ff56186c266926490d32d3ed2b700",
+    "-D LAMMPS_VERSION=stable_2Aug2023",
     "-D LAMMPS_EXCEPTIONS=ON",
     "-D BUILD_SHARED_LIBS=ON",
 ]
 
 [tool.cibuildwheel]
 build = ["cp311-*"]
 skip = ["*-win32", "*-manylinux_i686", "*-musllinux*"]
```

### Comparing `lammps-2022.6.23.4.0/PKG-INFO` & `lammps-2023.8.2.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lammps
-Version: 2022.6.23.4.0
+Version: 2023.8.2.0.0
 Summary: unoffical LAMMPS Molecular Dynamics Python package
 Keywords: lammps
 Author-Email: The LAMMPS Developers <developers@lammps.org>, Jinzhe Zeng <jinzhe.zeng@rutgers.edu>
 License: GNU GENERAL PUBLIC LICENSE
         
         Version 2, June 1991
```

