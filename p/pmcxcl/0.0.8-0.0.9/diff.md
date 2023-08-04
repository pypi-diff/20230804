# Comparing `tmp/pmcxcl-0.0.8-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/pmcxcl-0.0.9-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 871555 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat  1817600 b- defN 23-Jul-30 19:08 _pmcxcl.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1626 b- defN 23-Jul-30 19:05 pmcxcl/__init__.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-Jul-30 19:05 pmcxcl/bench.py
--rw-rw-rw-  2.0 fat     9258 b- defN 23-Jul-30 19:08 pmcxcl-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-30 19:08 pmcxcl-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-30 19:08 pmcxcl-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      535 b- defN 23-Jul-30 19:08 pmcxcl-0.0.8.dist-info/RECORD
-7 files, 1830878 bytes uncompressed, 870621 bytes compressed:  52.4%
+Zip file size: 871224 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat  1817600 b- defN 23-Jul-31 03:23 _pmcxcl.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1626 b- defN 23-Jul-31 03:20 pmcxcl/__init__.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 23-Jul-31 03:20 pmcxcl/bench.py
+-rw-rw-rw-  2.0 fat     8500 b- defN 23-Jul-31 03:23 pmcxcl-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-Jul-31 03:23 pmcxcl-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 23-Jul-31 03:23 pmcxcl-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      535 b- defN 23-Jul-31 03:23 pmcxcl-0.0.9.dist-info/RECORD
+7 files, 1830120 bytes uncompressed, 870290 bytes compressed:  52.4%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: pmcxcl/__init__.py
 Comment: 
 
 Filename: pmcxcl/bench.py
 Comment: 
 
-Filename: pmcxcl-0.0.8.dist-info/METADATA
+Filename: pmcxcl-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: pmcxcl-0.0.8.dist-info/WHEEL
+Filename: pmcxcl-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: pmcxcl-0.0.8.dist-info/top_level.txt
+Filename: pmcxcl-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: pmcxcl-0.0.8.dist-info/RECORD
+Filename: pmcxcl-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pmcxcl-0.0.8.dist-info/METADATA` & `pmcxcl-0.0.9.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pmcxcl
-Version: 0.0.8
-Summary: Python bindings for Monte Carlo eXtreme photon transport simulator
+Version: 0.0.9
+Summary: Python bindings for Monte Carlo eXtreme (OpenCL) photon transport simulator
 Home-page: https://github.com/fangq/mcxcl
 Author: Matin Raayai Ardakani, Qianqian Fang
 Author-email: raayaiardakani.m@northeastern.edu, q.fang@neu.edu
 Maintainer: Qianqian Fang
 License: GPLv3+
 Download-URL: http://mcx.space
-Keywords: Monte Carlo simulation,Biophotonics,Ray-tracing,Rendering,GPU,Modeling,Biomedical Optics,Tissue Optics,Simulator,Optics
+Keywords: Monte Carlo simulation,Biophotonics,Ray-tracing,Rendering,GPU,Modeling,Biomedical Optics,Tissue Optics,Simulator,Optics,OpenCL
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Environment :: GPU
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
@@ -28,22 +28,22 @@
 ![](http://mcx.space/img/mcx18_banner.png)
 
 # PMCX-CL - Python bindings for Monte Carlo eXtreme (OpenCL) photon transport simulator
 
 - Copyright: (C) Matin Raayai Ardakani (2022-2023) <raayaiardakani.m at northeastern.edu> 
 and Qianqian Fang (2019-2023) <q.fang at neu.edu>
 - License: GNU Public License V3 or later
-- Version: 0.0.8
+- Version: 0.0.9
 - URL: https://pypi.org/project/pmcxcl/
 - Github: https://github.com/fangq/mcxcl
 
+![Mex and Binaries](https://github.com/fangq/mcxcl/actions/workflows/build_all.yml/badge.svg)
 ![Linux Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_linux_manywheel.yml/badge.svg)\
 ![MacOS Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_macos_wheel.yml/badge.svg)\
 ![Windows Python Module](https://github.com/fangq/mcxcl/actions/workflows/build_windows_wheel.yml/badge.svg)\
-![Mex and Binaries](https://github.com/fangq/mcxcl/actions/workflows/build_all.yml/badge.svg)
 
 This module provides a Python binding for Monte Carlo eXtreme for OpenCL (MCXCL).
 For other binaries, including the standalone executable and the MATLAB bindings,
 see [our website](https://mcx.space).
 
 Monte Carlo eXtreme (MCX) is a fast photon transport simulation software for 3D 
 heterogeneous turbid media. By taking advantage of the massively parallel 
@@ -99,24 +99,14 @@
   manager, preferably after selecting the correct Xcode version:
   ```zsh
     brew install libomp
     brew link --force libomp
   ```
 * **CMake**: CMake version 3.15 and later is required. Refer to the [CMake website](https://cmake.org/download/) for more information on how to download.
   CMake is also widely available on package managers across all operating systems.
-* **Zlib Compression Development Headers**: On Linux, this is generally available via the built-in package manager. For 
-  example, on Debian-based distributions like Ubuntu it is available via ```apt``` under the name ```zlib1g-dev```. On
-  macOS, brew provides it under the name ```zlib```. No packaged versions of Zlib are available for windows, therefore it must be
-  downloaded manually and added to the CMake environment variables in your working Powershell session:
-  ```powershell
-    curl.exe --retry 3 -kL https://cytranet.dl.sourceforge.net/project/gnuwin32/zlib/1.2.3/zlib-1.2.3-lib.zip --output zlib.zip
-    Expand-Archive .\zlib.zip -DestinationPath zlib\
-    $env:CMAKE_INCLUDE_PATH=$PWD\zlib\include
-    $env:CMAKE_LIBRARY_PATH=$PWD\zlib\lib
-  ```
 
 ### Build Steps
 1. Ensure that ```cmake```, ```python``` and the C/C++ compiler are all located over your ```PATH```.
 This can be queried via ```echo $env:PATH``` on Windows or ```echo $PATH``` on Linux. If not, locate them and add their folder to the ```PATH```.
 
 2. Clone the repository and switch to the ```pmcxcl/``` folder:
     ```bash
```

