# Comparing `tmp/icesat2-toolkit-1.1.0.tar.gz` & `tmp/icesat2-toolkit-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icesat2-toolkit-1.1.0.tar", last modified: Wed Dec 14 23:51:09 2022, max compression
+gzip compressed data, was "icesat2-toolkit-1.3.0.tar", last modified: Thu Aug  3 23:26:56 2023, max compression
```

## Comparing `icesat2-toolkit-1.1.0.tar` & `icesat2-toolkit-1.3.0.tar`

### file list

```diff
@@ -1,79 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 23:51:09.466238 icesat2-toolkit-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       27 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    13704 2022-12-14 23:51:09.466238 icesat2-toolkit-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    12846 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 23:51:09.454237 icesat2-toolkit-1.1.0/icesat2_toolkit/
--rw-r--r--   0 runner    (1001) docker     (122)     1501 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28657 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/convert.py
--rw-r--r--   0 runner    (1001) docker     (122)     1987 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/convert_calendar_decimal.py
--rw-r--r--   0 runner    (1001) docker     (122)     2356 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/convert_delta_time.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     2261 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/convert_julian.py
--rw-r--r--   0 runner    (1001) docker     (122)      459 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/count_leap_seconds.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 23:51:09.458238 icesat2-toolkit-1.1.0/icesat2_toolkit/data/
--rw-r--r--   0 runner    (1001) docker     (122)   651269 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/data/ICESat-2_granules_global.png
--rw-r--r--   0 runner    (1001) docker     (122)   974986 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/data/ICESat-2_granules_polar.png
--rwxr-xr-x   0 runner    (1001) docker     (122)    10661 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/data/leap-seconds.list
--rw-r--r--   0 runner    (1001) docker     (122)    55390 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 23:51:09.458238 icesat2-toolkit-1.1.0/icesat2_toolkit/io/
--rw-r--r--   0 runner    (1001) docker     (122)    26069 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/io/ATL03.py
--rw-r--r--   0 runner    (1001) docker     (122)    15919 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/io/ATL06.py
--rw-r--r--   0 runner    (1001) docker     (122)    12761 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/io/ATL07.py
--rw-r--r--   0 runner    (1001) docker     (122)    12714 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/io/ATL10.py
--rw-r--r--   0 runner    (1001) docker     (122)    13275 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/io/ATL11.py
--rw-r--r--   0 runner    (1001) docker     (122)    11962 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/io/ATL12.py
--rw-r--r--   0 runner    (1001) docker     (122)      126 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5915 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/read_ICESat2_ATL03.py
--rw-r--r--   0 runner    (1001) docker     (122)     4115 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/read_ICESat2_ATL06.py
--rw-r--r--   0 runner    (1001) docker     (122)     3389 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/read_ICESat2_ATL07.py
--rw-r--r--   0 runner    (1001) docker     (122)     3082 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/read_ICESat2_ATL10.py
--rw-r--r--   0 runner    (1001) docker     (122)     4372 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/read_ICESat2_ATL11.py
--rw-r--r--   0 runner    (1001) docker     (122)     3343 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/read_ICESat2_ATL12.py
--rw-r--r--   0 runner    (1001) docker     (122)    32685 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/spatial.py
--rw-r--r--   0 runner    (1001) docker     (122)    22477 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     8744 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)    56247 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/utilities.py
--rw-r--r--   0 runner    (1001) docker     (122)      341 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/icesat2_toolkit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 23:51:09.458238 icesat2-toolkit-1.1.0/icesat2_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    13704 2022-12-14 23:51:09.000000 icesat2-toolkit-1.1.0/icesat2_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2331 2022-12-14 23:51:09.000000 icesat2-toolkit-1.1.0/icesat2_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-14 23:51:09.000000 icesat2-toolkit-1.1.0/icesat2_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       77 2022-12-14 23:51:09.000000 icesat2-toolkit-1.1.0/icesat2_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2022-12-14 23:51:09.000000 icesat2-toolkit-1.1.0/icesat2_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 23:51:09.462238 icesat2-toolkit-1.1.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (122)    47808 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_DEM_ICESat2_ATL03.py
--rw-r--r--   0 runner    (1001) docker     (122)    52751 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_DEM_ICESat2_ATL06.py
--rw-r--r--   0 runner    (1001) docker     (122)    49073 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_DEM_ICESat2_ATL11.py
--rw-r--r--   0 runner    (1001) docker     (122)   168516 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_ICESat2_ATL03.py
--rw-r--r--   0 runner    (1001) docker     (122)   188970 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_ICESat2_ATL03_histogram.py
--rw-r--r--   0 runner    (1001) docker     (122)    29351 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL03_RGI.py
--rw-r--r--   0 runner    (1001) docker     (122)    33543 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL06_RGI.py
--rw-r--r--   0 runner    (1001) docker     (122)    32245 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL06_drainages.py
--rw-r--r--   0 runner    (1001) docker     (122)    33713 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL06_grounded.py
--rw-r--r--   0 runner    (1001) docker     (122)    33150 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL06_ice_shelves.py
--rw-r--r--   0 runner    (1001) docker     (122)    30934 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL11_RGI.py
--rw-r--r--   0 runner    (1001) docker     (122)    29720 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL11_drainages.py
--rw-r--r--   0 runner    (1001) docker     (122)    31030 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL11_grounded.py
--rw-r--r--   0 runner    (1001) docker     (122)    30459 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL11_ice_shelves.py
--rw-r--r--   0 runner    (1001) docker     (122)    12878 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/convert_ICESat2_format.py
--rw-r--r--   0 runner    (1001) docker     (122)    11704 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/copy_scf_ICESat2_files.py
--rw-r--r--   0 runner    (1001) docker     (122)    14772 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/nsidc_icesat2_associated.py
--rw-r--r--   0 runner    (1001) docker     (122)    23492 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/nsidc_icesat2_convert.py
--rw-r--r--   0 runner    (1001) docker     (122)    21445 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/nsidc_icesat2_dragann.py
--rw-r--r--   0 runner    (1001) docker     (122)    25132 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/nsidc_icesat2_sync.py
--rw-r--r--   0 runner    (1001) docker     (122)    22508 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/nsidc_icesat2_sync_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)    31177 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/reduce_ICESat2_ATL06_raster.py
--rw-r--r--   0 runner    (1001) docker     (122)    34095 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/reduce_ICESat2_ATL07_raster.py
--rw-r--r--   0 runner    (1001) docker     (122)    30213 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/reduce_ICESat2_ATL10_raster.py
--rw-r--r--   0 runner    (1001) docker     (122)    29981 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/reduce_ICESat2_ATL11_raster.py
--rw-r--r--   0 runner    (1001) docker     (122)    16059 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/scp_ICESat2_files.py
--rw-r--r--   0 runner    (1001) docker     (122)    13661 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/scp_scf_ICESat2_files.py
--rw-r--r--   0 runner    (1001) docker     (122)     8632 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/scripts/symbolic_ICESat2_files.py
--rw-r--r--   0 runner    (1001) docker     (122)      288 2022-12-14 23:51:09.466238 icesat2-toolkit-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-14 23:51:09.462238 icesat2-toolkit-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     8110 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/test/test_download_and_read.py
--rw-r--r--   0 runner    (1001) docker     (122)     1059 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/test/test_leap_seconds.py
--rw-r--r--   0 runner    (1001) docker     (122)     3999 2022-12-14 23:51:00.000000 icesat2-toolkit-1.1.0/test/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 23:26:56.053846 icesat2-toolkit-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    13641 2023-08-03 23:26:56.053846 icesat2-toolkit-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    12783 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 23:26:56.045847 icesat2-toolkit-1.3.0/icesat2_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (122)      873 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28492 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2356 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/convert_delta_time.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 23:26:56.045847 icesat2-toolkit-1.3.0/icesat2_toolkit/data/
+-rwxr-xr-x   0 runner    (1001) docker     (122)    10666 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/data/leap-seconds.list
+-rw-r--r--   0 runner    (1001) docker     (122)    55407 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 23:26:56.045847 icesat2-toolkit-1.3.0/icesat2_toolkit/io/
+-rw-r--r--   0 runner    (1001) docker     (122)    26014 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/io/ATL03.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16280 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/io/ATL06.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13122 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/io/ATL07.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13075 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/io/ATL10.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13636 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/io/ATL11.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12323 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/io/ATL12.py
+-rw-r--r--   0 runner    (1001) docker     (122)      126 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41157 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/spatial.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25897 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8992 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/tools.py
+-rw-r--r--   0 runner    (1001) docker     (122)    66790 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/icesat2_toolkit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 23:26:56.045847 icesat2-toolkit-1.3.0/icesat2_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    13641 2023-08-03 23:26:55.000000 icesat2-toolkit-1.3.0/icesat2_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1888 2023-08-03 23:26:56.000000 icesat2-toolkit-1.3.0/icesat2_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-03 23:26:55.000000 icesat2-toolkit-1.3.0/icesat2_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-08-03 23:26:55.000000 icesat2-toolkit-1.3.0/icesat2_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-08-03 23:26:55.000000 icesat2-toolkit-1.3.0/icesat2_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 23:26:56.053846 icesat2-toolkit-1.3.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (122)    47515 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_DEM_ICESat2_ATL03.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52458 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_DEM_ICESat2_ATL06.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48780 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_DEM_ICESat2_ATL11.py
+-rw-r--r--   0 runner    (1001) docker     (122)   168288 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_ICESat2_ATL03.py
+-rw-r--r--   0 runner    (1001) docker     (122)   188748 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_ICESat2_ATL03_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29058 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL03_RGI.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33250 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL06_RGI.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31952 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL06_drainages.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33420 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL06_grounded.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32857 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL06_ice_shelves.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30641 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL11_RGI.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29427 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL11_drainages.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30737 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL11_grounded.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30166 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL11_ice_shelves.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12880 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/convert_ICESat2_format.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11704 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/copy_scf_ICESat2_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14774 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/nsidc_icesat2_associated.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23494 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/nsidc_icesat2_convert.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21390 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/nsidc_icesat2_dragann.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25134 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/nsidc_icesat2_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22750 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/nsidc_icesat2_sync_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31017 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/reduce_ICESat2_ATL06_raster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33960 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/reduce_ICESat2_ATL07_raster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30078 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/reduce_ICESat2_ATL10_raster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29846 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/reduce_ICESat2_ATL11_raster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16059 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/scp_ICESat2_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13661 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/scp_scf_ICESat2_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8632 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/scripts/symbolic_ICESat2_files.py
+-rw-r--r--   0 runner    (1001) docker     (122)      288 2023-08-03 23:26:56.053846 icesat2-toolkit-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-03 23:26:56.053846 icesat2-toolkit-1.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7402 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/test/test_download_and_read.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1043 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/test/test_leap_seconds.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3983 2023-08-03 23:26:41.000000 icesat2-toolkit-1.3.0/test/test_time.py
```

### Comparing `icesat2-toolkit-1.1.0/LICENSE` & `icesat2-toolkit-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `icesat2-toolkit-1.1.0/PKG-INFO` & `icesat2-toolkit-1.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icesat2-toolkit
-Version: 1.1.0
+Version: 1.3.0
 Summary: Python tools for obtaining and working with elevation data from the NASA ICESat-2 mission
 Home-page: https://github.com/tsutterley/read-ICESat-2
 Author: Tyler Sutterley
 Author-email: tsutterl@uw.edu
 License: MIT
 Keywords: ICESat-2 laser altimetry,ATLAS,surface elevation and change
 Classifier: Development Status :: 3 - Alpha
@@ -23,16 +23,14 @@
 read-ICESat-2
 =============
 
 |Language|
 |License|
 |PyPI Version|
 |Documentation Status|
-|Binder|
-|Pangeo|
 |zenodo|
 |Shot Count|
 
 .. |Language| image:: https://img.shields.io/pypi/pyversions/icesat2-toolkit?color=green
    :target: https://www.python.org/
 
 .. |License| image:: https://img.shields.io/badge/license-MIT-green.svg
@@ -40,20 +38,14 @@
 
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/icesat2-toolkit.svg
    :target: https://pypi.python.org/pypi/icesat2-toolkit/
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/read-icesat-2/badge/?version=latest
    :target: https://read-icesat-2.readthedocs.io/en/latest/?badge=latest
 
-.. |Binder| image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/tsutterley/read-ICESat-2/main
-
-.. |Pangeo| image:: https://img.shields.io/static/v1.svg?logo=Jupyter&label=PangeoBinderAWS&message=us-west-2&color=orange
-   :target: https://aws-uswest2-binder.pangeo.io/v2/gh/tsutterley/read-ICESat-2/main?urlpath=lab
-
 .. |zenodo| image:: https://zenodo.org/badge/193143942.svg
    :target: https://zenodo.org/badge/latestdoi/193143942
 
 .. |Shot count| image:: https://img.shields.io/badge/dynamic/json?label=ICESat-2%20shot%20count&query=message&url=https%3A%2F%2Fraw.githubusercontent.com%2Ftsutterley%2Ftsutterley%2Fmaster%2FIS2-shot-count.json
    :target: https://icesat-2.gsfc.nasa.gov/
 
 Python tools for obtaining and working with elevation data from the NASA ICESat-2 mission
@@ -165,38 +157,41 @@
 
 ICESat-2 Granules
 #################
 
 Each orbit of ICESat-2 data is broken up into 14 granules.
 The granule boundaries limit the size of each ATL03 file and simplify the formation of higher level data products.
 
-.. image:: ./icesat2_toolkit/data/ICESat-2_granules_global.png
+.. image:: ./doc/source/_assets/ICESat-2_granules_global.png
   :alt: ICESat-2 global granules
 
-.. image:: ./icesat2_toolkit/data/ICESat-2_granules_polar.png
+.. image:: ./doc/source/_assets/ICESat-2_granules_polar.png
   :alt: ICESat-2 polar granules
 
 Dependencies
 ############
 
- - `numpy: Scientific Computing Tools For Python <https://numpy.org>`_
- - `scipy: Scientific Tools for Python <https://docs.scipy.org/doc/>`_
- - `mpi4py: Python bindings of the Message Passing Interface (MPI) <https://mpi4py.readthedocs.io/en/stable/>`_
- - `h5py: Python interface for Hierarchal Data Format 5 (HDF5) <http://h5py.org>`_
- - `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
- - `zarr: Chunked, compressed, N-dimensional arrays in Python <https://github.com/zarr-developers/zarr-python>`_
- - `pandas: Python Data Analysis Library <https://pandas.pydata.org/>`_
- - `scikit-learn: Machine Learning in Python <https://scikit-learn.org/stable/index.html>`_
- - `shapely: PostGIS-ish operations outside a database context for Python <http://toblerity.org/shapely/index.html>`_
- - `fiona: Python wrapper for vector data access functions from the OGR library <https://fiona.readthedocs.io/en/latest/manual.html>`_
- - `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
- - `paramiko: Native Python SSHv2 protocol library <http://www.paramiko.org/>`_
- - `scp: scp module for paramiko <https://github.com/jbardin/scp.py>`_
- - `future: Compatibility layer between Python 2 and Python 3 <http://python-future.org/>`_
- - `yapc: Python version of the NASA Goddard Space Flight Center YAPC Program <https://github.com/tsutterley/yapc>`_
+- `numpy: Scientific Computing Tools For Python <https://numpy.org>`_
+- `scipy: Scientific Tools for Python <https://docs.scipy.org/doc//>`_
+- `mpi4py: Python bindings of the Message Passing Interface (MPI) <https://mpi4py.readthedocs.io/en/stable/>`_
+- `h5py: Python interface for Hierarchal Data Format 5 (HDF5) <http://h5py.org>`_
+- `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
+- `zarr: Chunked, compressed, N-dimensional arrays in Python <https://github.com/zarr-developers/zarr-python>`_
+- `pandas: Python Data Analysis Library <https://pandas.pydata.org/>`_
+- `scikit-learn: Machine Learning in Python <https://scikit-learn.org/stable/index.html>`_
+- `dateutil: powerful extensions to datetime <https://dateutil.readthedocs.io/en/stable/>`_
+- `shapely: PostGIS-ish operations outside a database context for Python <http://toblerity.org/shapely/index.html>`_
+- `fiona: Python wrapper for vector data access functions from the OGR library <https://fiona.readthedocs.io/en/latest/manual.html>`_
+- `future: Compatibility layer between Python 2 and Python 3 <http://python-future.org/>`_
+- `boto3: Amazon Web Services (AWS) SDK for Python <https://boto3.amazonaws.com/v1/documentation/api/latest/index.html>`_
+- `s3fs: Pythonic file interface to S3 built on top of botocore <https://s3fs.readthedocs.io/en/latest/>`_
+- `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
+- `paramiko: Native Python SSHv2 protocol library <http://www.paramiko.org>`_
+- `scp: scp module for paramiko <https://github.com/jbardin/scp.py>`_
+- `yapc: Python version of the NASA Goddard Space Flight Center YAPC Program <https://github.com/tsutterley/yapc>`_
 
 Download
 ########
 
 | The program homepage is:
 | https://github.com/tsutterley/read-icesat-2
 | A zip archive of the latest version is available directly at:
```

### Comparing `icesat2-toolkit-1.1.0/README.rst` & `icesat2-toolkit-1.3.0/icesat2_toolkit.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,36 @@
+Metadata-Version: 2.1
+Name: icesat2-toolkit
+Version: 1.3.0
+Summary: Python tools for obtaining and working with elevation data from the NASA ICESat-2 mission
+Home-page: https://github.com/tsutterley/read-ICESat-2
+Author: Tyler Sutterley
+Author-email: tsutterl@uw.edu
+License: MIT
+Keywords: ICESat-2 laser altimetry,ATLAS,surface elevation and change
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
 =============
 read-ICESat-2
 =============
 
 |Language|
 |License|
 |PyPI Version|
 |Documentation Status|
-|Binder|
-|Pangeo|
 |zenodo|
 |Shot Count|
 
 .. |Language| image:: https://img.shields.io/pypi/pyversions/icesat2-toolkit?color=green
    :target: https://www.python.org/
 
 .. |License| image:: https://img.shields.io/badge/license-MIT-green.svg
@@ -19,20 +38,14 @@
 
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/icesat2-toolkit.svg
    :target: https://pypi.python.org/pypi/icesat2-toolkit/
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/read-icesat-2/badge/?version=latest
    :target: https://read-icesat-2.readthedocs.io/en/latest/?badge=latest
 
-.. |Binder| image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/tsutterley/read-ICESat-2/main
-
-.. |Pangeo| image:: https://img.shields.io/static/v1.svg?logo=Jupyter&label=PangeoBinderAWS&message=us-west-2&color=orange
-   :target: https://aws-uswest2-binder.pangeo.io/v2/gh/tsutterley/read-ICESat-2/main?urlpath=lab
-
 .. |zenodo| image:: https://zenodo.org/badge/193143942.svg
    :target: https://zenodo.org/badge/latestdoi/193143942
 
 .. |Shot count| image:: https://img.shields.io/badge/dynamic/json?label=ICESat-2%20shot%20count&query=message&url=https%3A%2F%2Fraw.githubusercontent.com%2Ftsutterley%2Ftsutterley%2Fmaster%2FIS2-shot-count.json
    :target: https://icesat-2.gsfc.nasa.gov/
 
 Python tools for obtaining and working with elevation data from the NASA ICESat-2 mission
@@ -144,38 +157,41 @@
 
 ICESat-2 Granules
 #################
 
 Each orbit of ICESat-2 data is broken up into 14 granules.
 The granule boundaries limit the size of each ATL03 file and simplify the formation of higher level data products.
 
-.. image:: ./icesat2_toolkit/data/ICESat-2_granules_global.png
+.. image:: ./doc/source/_assets/ICESat-2_granules_global.png
   :alt: ICESat-2 global granules
 
-.. image:: ./icesat2_toolkit/data/ICESat-2_granules_polar.png
+.. image:: ./doc/source/_assets/ICESat-2_granules_polar.png
   :alt: ICESat-2 polar granules
 
 Dependencies
 ############
 
- - `numpy: Scientific Computing Tools For Python <https://numpy.org>`_
- - `scipy: Scientific Tools for Python <https://docs.scipy.org/doc/>`_
- - `mpi4py: Python bindings of the Message Passing Interface (MPI) <https://mpi4py.readthedocs.io/en/stable/>`_
- - `h5py: Python interface for Hierarchal Data Format 5 (HDF5) <http://h5py.org>`_
- - `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
- - `zarr: Chunked, compressed, N-dimensional arrays in Python <https://github.com/zarr-developers/zarr-python>`_
- - `pandas: Python Data Analysis Library <https://pandas.pydata.org/>`_
- - `scikit-learn: Machine Learning in Python <https://scikit-learn.org/stable/index.html>`_
- - `shapely: PostGIS-ish operations outside a database context for Python <http://toblerity.org/shapely/index.html>`_
- - `fiona: Python wrapper for vector data access functions from the OGR library <https://fiona.readthedocs.io/en/latest/manual.html>`_
- - `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
- - `paramiko: Native Python SSHv2 protocol library <http://www.paramiko.org/>`_
- - `scp: scp module for paramiko <https://github.com/jbardin/scp.py>`_
- - `future: Compatibility layer between Python 2 and Python 3 <http://python-future.org/>`_
- - `yapc: Python version of the NASA Goddard Space Flight Center YAPC Program <https://github.com/tsutterley/yapc>`_
+- `numpy: Scientific Computing Tools For Python <https://numpy.org>`_
+- `scipy: Scientific Tools for Python <https://docs.scipy.org/doc//>`_
+- `mpi4py: Python bindings of the Message Passing Interface (MPI) <https://mpi4py.readthedocs.io/en/stable/>`_
+- `h5py: Python interface for Hierarchal Data Format 5 (HDF5) <http://h5py.org>`_
+- `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
+- `zarr: Chunked, compressed, N-dimensional arrays in Python <https://github.com/zarr-developers/zarr-python>`_
+- `pandas: Python Data Analysis Library <https://pandas.pydata.org/>`_
+- `scikit-learn: Machine Learning in Python <https://scikit-learn.org/stable/index.html>`_
+- `dateutil: powerful extensions to datetime <https://dateutil.readthedocs.io/en/stable/>`_
+- `shapely: PostGIS-ish operations outside a database context for Python <http://toblerity.org/shapely/index.html>`_
+- `fiona: Python wrapper for vector data access functions from the OGR library <https://fiona.readthedocs.io/en/latest/manual.html>`_
+- `future: Compatibility layer between Python 2 and Python 3 <http://python-future.org/>`_
+- `boto3: Amazon Web Services (AWS) SDK for Python <https://boto3.amazonaws.com/v1/documentation/api/latest/index.html>`_
+- `s3fs: Pythonic file interface to S3 built on top of botocore <https://s3fs.readthedocs.io/en/latest/>`_
+- `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
+- `paramiko: Native Python SSHv2 protocol library <http://www.paramiko.org>`_
+- `scp: scp module for paramiko <https://github.com/jbardin/scp.py>`_
+- `yapc: Python version of the NASA Goddard Space Flight Center YAPC Program <https://github.com/tsutterley/yapc>`_
 
 Download
 ########
 
 | The program homepage is:
 | https://github.com/tsutterley/read-icesat-2
 | A zip archive of the latest version is available directly at:
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/__init__.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,22 +18,9 @@
 import icesat2_toolkit.spatial
 import icesat2_toolkit.time
 import icesat2_toolkit.utilities
 import icesat2_toolkit.version
 from icesat2_toolkit.convert_delta_time import convert_delta_time
 from icesat2_toolkit import io
 
-# deprecated modules
-from icesat2_toolkit.read_ICESat2_ATL03 import read_HDF5_ATL03, \
-    find_HDF5_ATL03_beams, read_HDF5_ATL09, read_HDF5_ATL03_main, read_HDF5_ATL03_beam
-from icesat2_toolkit.read_ICESat2_ATL06 import read_HDF5_ATL06, \
-    find_HDF5_ATL06_beams, read_HDF5_ATL06_beam
-from icesat2_toolkit.read_ICESat2_ATL07 import read_HDF5_ATL07, \
-    find_HDF5_ATL07_beams
-from icesat2_toolkit.read_ICESat2_ATL10 import read_HDF5_ATL10, \
-    find_HDF5_ATL10_beams
-from icesat2_toolkit.read_ICESat2_ATL11 import read_HDF5_ATL11
-from icesat2_toolkit.read_ICESat2_ATL12 import read_HDF5_ATL12, \
-    find_HDF5_ATL12_beams
-
 # get version number
 __version__ = icesat2_toolkit.version.version
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/convert.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,29 +40,26 @@
 import numpy as np
 from icesat2_toolkit.convert_delta_time import convert_delta_time
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     import pandas
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("pandas not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("pandas not available", ImportWarning)
 try:
     import zarr
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("zarr not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("zarr not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 class convert():
     np.seterr(invalid='ignore')
     def __init__(self, filename=None, reformat=None):
         """Utilities for converting ICESat-2 HDF5 files into different formats
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/convert_delta_time.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/convert_delta_time.py`

 * *Files identical despite different names*

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/data/leap-seconds.list` & `icesat2-toolkit-1.3.0/icesat2_toolkit/data/leap-seconds.list`

 * *Files 2% similar despite different names*

```diff
@@ -200,18 +200,18 @@
 #	(whichever is later).
 #	If an announcement by the IERS specifies that no leap second is
 #	scheduled, then only the expiration date of the file will
 #	be advanced to show that the information in the file is still
 #	current -- the update time stamp, the data and the name of the file
 #	will not change.
 #
-#	Updated through IERS Bulletin C64
-#	File expires on:  28 June 2023
+#	Updated through IERS Bulletin C65
+#	File expires on:  28 December 2023
 #
-#@	3896899200
+#@	3912710400
 #
 2272060800	10	# 1 Jan 1972
 2287785600	11	# 1 Jul 1972
 2303683200	12	# 1 Jan 1973
 2335219200	13	# 1 Jan 1974
 2366755200	14	# 1 Jan 1975
 2398291200	15	# 1 Jan 1976
@@ -248,8 +248,8 @@
 #	in data lines. It includes the NTP values
 #	of both the last modification time and the
 #	expiration time of the file, but not the
 #	white space on those lines.
 #	the hash line is also ignored in the
 #	computation.
 #
-#h 	2c413af9 124e1031 f165174 ff527c6b 756ae00b
+#h 	e76a99dc 65f15cc7 e613e040 f5078b5e b23834fe
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/fit.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/fit.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 import scipy.stats
 import scipy.signal
 import scipy.optimize
 
 # attempt imports
 try:
     import sklearn.neighbors
-except (ImportError, ModuleNotFoundError) as e:
-    warnings.filterwarnings("always")
-    warnings.warn("scikit-learn not available")
+except (ImportError, ModuleNotFoundError) as exc:
+    warnings.filterwarnings("module")
+    warnings.warn("scikit-learn not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: compress complete list of valid indices into a set of ranges
 def compress_list(i,n):
     """
     Compress complete list of valid indices into a set of ranges
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/io/ATL03.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/io/ATL03.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,16 @@
 import numpy as np
 import scipy.interpolate
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: read ICESat-2 ATL03 HDF5 data files
 def read_granule(FILENAME, ATTRIBUTES=False, **kwargs):
     """
     Reads ICESat-2 ATL03 Global Geolocated Photons data files
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/io/ATL06.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/io/ATL06.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 u"""
-ATL06.py (12/2022)
+ATL06.py (05/2023)
 Read ICESat-2 ATL06 (Land Ice Along-Track Height Product) data files
 
 OPTIONS:
     ATTRIBUTES: read HDF5 attributes for groups and variables
     HISTOGRAM: read ATL06 residual_histogram variables
     QUALITY: read ATL06 segment_quality variables
 
@@ -12,14 +12,15 @@
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
     h5py: Python interface for Hierarchal Data Format 5 (HDF5)
         https://www.h5py.org/
 
 UPDATE HISTORY:
+    Updated 05/2023: extract more ancillary data from ATL06 files
     Updated 12/2022: place some imports behind try/except statements
         refactor ICESat-2 data product read programs under io
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 10/2021: using python logging for handling verbose output
     Updated 02/2021: add check if input streaming from bytes
     Updated 10/2020: add small function to find valid beam groups
     Updated 07/2020: added function docstrings
@@ -37,17 +38,16 @@
 import warnings
 import numpy as np
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: read ICESat-2 ATL06 HDF5 data files
 def read_granule(FILENAME, ATTRIBUTES=False, HISTOGRAM=False,
     QUALITY=False, **kwargs):
     """
@@ -195,15 +195,20 @@
     # number of GPS seconds between the GPS epoch (1980-01-06T00:00:00Z UTC)
     # and ATLAS Standard Data Product (SDP) epoch (2018-01-01:T00:00:00Z UTC)
     # Add this value to delta time parameters to compute full gps_seconds
     # could alternatively use the Julian day of the ATLAS SDP epoch: 2458119.5
     # and add leap seconds since 2018-01-01:T00:00:00Z UTC (ATLAS SDP epoch)
     IS2_atl06_mds['ancillary_data'] = {}
     IS2_atl06_attrs['ancillary_data'] = {}
-    for key in ['atlas_sdp_gps_epoch']:
+    ancillary_keys = ['atlas_sdp_gps_epoch','data_end_utc','data_start_utc',
+        'end_cycle','end_geoseg','end_gpssow','end_gpsweek','end_orbit',
+        'end_region','end_rgt','granule_end_utc','granule_start_utc','release',
+        'start_cycle','start_geoseg','start_gpssow','start_gpsweek',
+        'start_orbit','start_region','start_rgt','version']
+    for key in ancillary_keys:
         # get each HDF5 variable
         IS2_atl06_mds['ancillary_data'][key] = fileID['ancillary_data'][key][:]
         # Getting attributes of group and included variables
         if ATTRIBUTES:
             # Variable Attributes
             IS2_atl06_attrs['ancillary_data'][key] = {}
             for att_name,att_val in fileID['ancillary_data'][key].attrs.items():
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/io/ATL07.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/io/ATL07.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python
 u"""
-ATL07.py (12/2022)
+ATL07.py (05/2023)
 Read ICESat-2 ATL07 (Sea Ice Height) data files
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
     h5py: Python interface for Hierarchal Data Format 5 (HDF5)
         https://www.h5py.org/
 
 UPDATE HISTORY:
+    Updated 05/2023: extract more ancillary data from ATL07 files
     Updated 12/2022: place some imports behind try/except statements
         refactor ICESat-2 data product read programs under io
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 10/2021: using python logging for handling verbose output
     Updated 02/2021: add check if input streaming from bytes
     Updated 10/2020: add small function to find valid beam groups
     Updated 07/2020: added function docstrings
@@ -30,17 +31,16 @@
 import warnings
 import numpy as np
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: read ICESat-2 ATL07 HDF5 data files
 def read_granule(FILENAME, ATTRIBUTES=False, **kwargs):
     """
     Reads ICESat-2 ATL07 (Sea Ice Height) data files
@@ -142,15 +142,20 @@
     # number of GPS seconds between the GPS epoch (1980-01-06T00:00:00Z UTC)
     # and ATLAS Standard Data Product (SDP) epoch (2018-01-01:T00:00:00Z UTC)
     # Add this value to delta time parameters to compute full gps_seconds
     # could alternatively use the Julian day of the ATLAS SDP epoch: 2458119.5
     # and add leap seconds since 2018-01-01:T00:00:00Z UTC (ATLAS SDP epoch)
     IS2_atl07_mds['ancillary_data'] = {}
     IS2_atl07_attrs['ancillary_data'] = {}
-    for key in ['atlas_sdp_gps_epoch']:
+    ancillary_keys = ['atlas_sdp_gps_epoch','data_end_utc','data_start_utc',
+        'end_cycle','end_geoseg','end_gpssow','end_gpsweek','end_orbit',
+        'end_region','end_rgt','granule_end_utc','granule_start_utc','release',
+        'start_cycle','start_geoseg','start_gpssow','start_gpsweek',
+        'start_orbit','start_region','start_rgt','version']
+    for key in ancillary_keys:
         # get each HDF5 variable
         IS2_atl07_mds['ancillary_data'][key] = fileID['ancillary_data'][key][:]
         # Getting attributes of group and included variables
         if ATTRIBUTES:
             # Variable Attributes
             IS2_atl07_attrs['ancillary_data'][key] = {}
             for att_name,att_val in fileID['ancillary_data'][key].attrs.items():
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/io/ATL10.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/io/ATL10.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python
 u"""
-ATL10.py (12/2022)
+ATL10.py (05/2023)
 Read ICESat-2 ATL10 (Sea Ice Freeboard) data files
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
     h5py: Python interface for Hierarchal Data Format 5 (HDF5)
         https://www.h5py.org/
 
 UPDATE HISTORY:
+    Updated 05/2023: extract more ancillary data from ATL10 files
     Updated 12/2022: place some imports behind try/except statements
         refactor ICESat-2 data product read programs under io
     Updated 04/2022: updated docstrings to numpy documentation format
     Written 12/2021
 """
 from __future__ import print_function
 
@@ -25,17 +26,16 @@
 import warnings
 import numpy as np
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: read ICESat-2 ATL10 HDF5 data files
 def read_granule(FILENAME, ATTRIBUTES=False, **kwargs):
     """
     Reads ICESat-2 ATL10 (Sea Ice Freeboard) data files
@@ -140,15 +140,20 @@
     # number of GPS seconds between the GPS epoch (1980-01-06T00:00:00Z UTC)
     # and ATLAS Standard Data Product (SDP) epoch (2018-01-01:T00:00:00Z UTC)
     # Add this value to delta time parameters to compute full gps_seconds
     # could alternatively use the Julian day of the ATLAS SDP epoch: 2458119.5
     # and add leap seconds since 2018-01-01:T00:00:00Z UTC (ATLAS SDP epoch)
     IS2_atl10_mds['ancillary_data'] = {}
     IS2_atl10_attrs['ancillary_data'] = {}
-    for key in ['atlas_sdp_gps_epoch']:
+    ancillary_keys = ['atlas_sdp_gps_epoch','data_end_utc','data_start_utc',
+        'end_cycle','end_geoseg','end_gpssow','end_gpsweek','end_orbit',
+        'end_region','end_rgt','granule_end_utc','granule_start_utc','release',
+        'start_cycle','start_geoseg','start_gpssow','start_gpsweek',
+        'start_orbit','start_region','start_rgt','version']
+    for key in ancillary_keys:
         # get each HDF5 variable
         IS2_atl10_mds['ancillary_data'][key] = fileID['ancillary_data'][key][:]
         # Getting attributes of group and included variables
         if ATTRIBUTES:
             # Variable Attributes
             IS2_atl10_attrs['ancillary_data'][key] = {}
             for att_name,att_val in fileID['ancillary_data'][key].attrs.items():
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/io/ATL11.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/io/ATL11.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 u"""
-ATL11.py (12/2022)
+ATL11.py (05/2023)
 Read ICESat-2 ATL11 (Annual Land Ice Height) data files
 
 OPTIONS:
     GROUPS: HDF5 groups to read for each beam pair
     ATTRIBUTES: read HDF5 attributes for groups and variables
     REFERENCE: read ATL11 reference surface variables
     CROSSOVERS: read ATL11 crossover height variables
@@ -14,14 +14,15 @@
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
     h5py: Python interface for Hierarchal Data Format 5 (HDF5)
         https://www.h5py.org/
 
 UPDATE HISTORY:
+    Updated 05/2023: extract more ancillary data from ATL11 files
     Updated 12/2022: place some imports behind try/except statements
         refactor ICESat-2 data product read programs under io
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 10/2021: using python logging for handling verbose output
     Updated 03/2021: added function for reading only pair level variables
         simplified group reads to iterate within a try/except statement
         added keyword argument to explicitly define groups to read
@@ -38,17 +39,16 @@
 import warnings
 import numpy as np
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: read ICESat-2 ATL11 HDF5 data files
 def read_granule(FILENAME, GROUPS=['cycle_stats'], ATTRIBUTES=False,
     REFERENCE=False, CROSSOVERS=False, SUBSETTING=False, **kwargs):
     """
@@ -175,15 +175,20 @@
     # number of GPS seconds between the GPS epoch (1980-01-06T00:00:00Z UTC)
     # and ATLAS Standard Data Product (SDP) epoch (2018-01-01:T00:00:00Z UTC)
     # Add this value to delta time parameters to compute full gps_seconds
     # could alternatively use the Julian day of the ATLAS SDP epoch: 2458119.5
     # and add leap seconds since 2018-01-01:T00:00:00Z UTC (ATLAS SDP epoch)
     IS2_atl11_mds['ancillary_data'] = {}
     IS2_atl11_attrs['ancillary_data'] = {}
-    for key in ['atlas_sdp_gps_epoch']:
+    ancillary_keys = ['atlas_sdp_gps_epoch','data_end_utc','data_start_utc',
+        'end_cycle','end_geoseg','end_gpssow','end_gpsweek','end_orbit',
+        'end_region','end_rgt','granule_end_utc','granule_start_utc','release',
+        'start_cycle','start_geoseg','start_gpssow','start_gpsweek',
+        'start_orbit','start_region','start_rgt','version']
+    for key in ancillary_keys:
         # get each HDF5 variable
         IS2_atl11_mds['ancillary_data'][key] = fileID['ancillary_data'][key][:]
         # Getting attributes of group and included variables
         if ATTRIBUTES:
             # Variable Attributes
             IS2_atl11_attrs['ancillary_data'][key] = {}
             for att_name,att_val in fileID['ancillary_data'][key].attrs.items():
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/io/ATL12.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/io/ATL12.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 #!/usr/bin/env python
 u"""
-ATL12.py (12/2022)
+ATL12.py (05/2023)
 Read ICESat-2 ATL12 (Ocean Surface Height) data files
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
     h5py: Python interface for Hierarchal Data Format 5 (HDF5)
         https://www.h5py.org/
 
 UPDATE HISTORY:
+    Updated 05/2023: extract more ancillary data from ATL12 files
     Updated 12/2022: place some imports behind try/except statements
         refactor ICESat-2 data product read programs under io
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 10/2021: using python logging for handling verbose output
     Updated 02/2021: add check if input streaming from bytes
     Updated 10/2020: add small function to find valid beam groups
     Updated 07/2020: added function docstrings
@@ -29,17 +30,16 @@
 import warnings
 import numpy as np
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: read ICESat-2 ATL12 HDF5 data files
 def read_granule(FILENAME, ATTRIBUTES=False, **kwargs):
     """
     Reads ICESat-2 ATL12 (Ocean Surface Height) data files
@@ -137,15 +137,20 @@
     # number of GPS seconds between the GPS epoch (1980-01-06T00:00:00Z UTC)
     # and ATLAS Standard Data Product (SDP) epoch (2018-01-01:T00:00:00Z UTC)
     # Add this value to delta time parameters to compute full gps_seconds
     # could alternatively use the Julian day of the ATLAS SDP epoch: 2458119.5
     # and add leap seconds since 2018-01-01:T00:00:00Z UTC (ATLAS SDP epoch)
     IS2_atl12_mds['ancillary_data'] = {}
     IS2_atl12_attrs['ancillary_data'] = {}
-    for key in ['atlas_sdp_gps_epoch']:
+    ancillary_keys = ['atlas_sdp_gps_epoch','data_end_utc','data_start_utc',
+        'end_cycle','end_geoseg','end_gpssow','end_gpsweek','end_orbit',
+        'end_region','end_rgt','granule_end_utc','granule_start_utc','release',
+        'start_cycle','start_geoseg','start_gpssow','start_gpsweek',
+        'start_orbit','start_region','start_rgt','version']
+    for key in ancillary_keys:
         # get each HDF5 variable
         IS2_atl12_mds['ancillary_data'][key] = fileID['ancillary_data'][key][:]
         # Getting attributes of group and included variables
         if ATTRIBUTES:
             # Variable Attributes
             IS2_atl12_attrs['ancillary_data'][key] = {}
             for att_name,att_val in fileID['ancillary_data'][key].attrs.items():
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/spatial.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/spatial.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 u"""
 spatial.py
-Written by Tyler Sutterley (12/2022)
+Written by Tyler Sutterley (05/2023)
 
 Utilities for reading and operating on spatial data
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
         https://numpy.org/doc/stable/user/numpy-for-matlab-users.html
@@ -13,76 +13,80 @@
         https://unidata.github.io/netcdf4-python/netCDF4/index.html
     h5py: Pythonic interface to the HDF5 binary data format
         https://www.h5py.org/
     gdal: Pythonic interface to the Geospatial Data Abstraction Library (GDAL)
         https://pypi.python.org/pypi/GDAL
 
 UPDATE HISTORY:
+    Updated 05/2023: using pathlib to define and expand paths
+    Updated 04/2023: copy inputs in cartesian to not modify original arrays
+        added iterative methods for converting from cartesian to geodetic
+    Updated 03/2023: add basic variable typing to function inputs
     Updated 12/2022: place some imports behind try/except statements
     Updated 10/2022: verify data variable in netCDF4/HDF5 read functions
     Updated 07/2022: filter warnings after import attempts
     Updated 06/2022: place netCDF4 import behind try/except statements
         added field_mapping options to netCDF4 and HDF5 reads
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 01/2022: use iteration breaks in convert ellipsoid function
     Written 11/2021
 """
-import os
+from __future__ import annotations
+
 import re
 import io
 import copy
 import gzip
 import uuid
 import logging
+import pathlib
 import warnings
 import numpy as np
-
 # attempt imports
 try:
+    import osgeo.gdal, osgeo.osr, osgeo.gdalconst
+except (ImportError, ModuleNotFoundError) as exc:
+    warnings.filterwarnings("module")
+    warnings.warn("GDAL not available", ImportWarning)
+try:
     import h5py
-except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+except (ImportError, ModuleNotFoundError) as exc:
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     import netCDF4
-except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("netCDF4 not available")
-    warnings.warn("Some functions will throw an exception if called")
-try:
-    import osgeo.gdal, osgeo.osr, osgeo.gdalconst
-except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("GDAL not available")
-    warnings.warn("Some functions will throw an exception if called")
+except (ImportError, ModuleNotFoundError) as exc:
+    warnings.filterwarnings("module")
+    warnings.warn("netCDF4 not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
-def case_insensitive_filename(filename):
+def case_insensitive_filename(filename: str | pathlib.Path):
     """
     Searches a directory for a filename without case dependence
 
     Parameters
     ----------
     filename: str
         input filename
     """
     # check if file presently exists with input case
-    if not os.access(os.path.expanduser(filename),os.F_OK):
+    filename = pathlib.Path(filename).expanduser().absolute()
+    if not filename.exists():
         # search for filename without case dependence
-        basename = os.path.basename(filename)
-        directory = os.path.dirname(os.path.expanduser(filename))
-        f = [f for f in os.listdir(directory) if re.match(basename,f,re.I)]
+        f = [f.name for f in filename.parent.iterdir() if
+            re.match(filename.name, f.name, re.I)]
+        # raise error if no file found
         if not f:
-            raise FileNotFoundError(f'{filename} not found in file system')
-        filename = os.path.join(directory,f.pop())
-    return os.path.expanduser(filename)
+            raise FileNotFoundError(str(filename))
+        filename = filename.with_name(f.pop())
+    # return the matched filename
+    return filename
 
-def from_file(filename, format, **kwargs):
+def from_file(filename: str, format: str, **kwargs):
     """
     Wrapper function for reading data from an input format
 
     Parameters
     ----------
     filename: str
         full path of input file
@@ -98,15 +102,15 @@
         dinput = from_HDF5(filename, **kwargs)
     elif (format == 'geotiff'):
         dinput = from_geotiff(filename, **kwargs)
     else:
         raise ValueError(f'Invalid format {format}')
     return dinput
 
-def from_netCDF4(filename, **kwargs):
+def from_netCDF4(filename: str, **kwargs):
     """
     Read data from a netCDF4 file
 
     Parameters
     ----------
     filename: str
         full path of input netCDF4 file
@@ -120,74 +124,74 @@
         name for y-dimension variable
     varname: str, default 'data'
         name for data variable
     field_mapping: dict, default {}
         mapping between output variables and input netCDF4
     """
     # set default keyword arguments
-    kwargs.setdefault('compression',None)
-    kwargs.setdefault('timename','time')
-    kwargs.setdefault('xname','lon')
-    kwargs.setdefault('yname','lat')
-    kwargs.setdefault('varname','data')
-    kwargs.setdefault('field_mapping',{})
+    kwargs.setdefault('compression', None)
+    kwargs.setdefault('timename', 'time')
+    kwargs.setdefault('xname', 'lon')
+    kwargs.setdefault('yname', 'lat')
+    kwargs.setdefault('varname', 'data')
+    kwargs.setdefault('field_mapping', {})
     # read data from netCDF4 file
     # Open the NetCDF4 file for reading
     if (kwargs['compression'] == 'gzip'):
         # read as in-memory (diskless) netCDF4 dataset
-        with gzip.open(case_insensitive_filename(filename),'r') as f:
-            fileID = netCDF4.Dataset(uuid.uuid4().hex,memory=f.read())
+        with gzip.open(case_insensitive_filename(filename), 'r') as f:
+            fileID = netCDF4.Dataset(uuid.uuid4().hex, memory=f.read())
     elif (kwargs['compression'] == 'bytes'):
         # read as in-memory (diskless) netCDF4 dataset
-        fileID = netCDF4.Dataset(uuid.uuid4().hex,memory=filename.read())
+        fileID = netCDF4.Dataset(uuid.uuid4().hex, memory=filename.read())
     else:
         # read netCDF4 dataset
         fileID = netCDF4.Dataset(case_insensitive_filename(filename), 'r')
     # Output NetCDF file information
     logging.info(fileID.filepath())
     logging.info(list(fileID.variables.keys()))
     # create python dictionary for output variables and attributes
     dinput = {}
     dinput['attributes'] = {}
     # get attributes for the file
-    for attr in ['title','description','projection']:
+    for attr in ['title', 'description', 'projection']:
         # try getting the attribute
         try:
-            ncattr, = [s for s in fileID.ncattrs() if re.match(attr,s,re.I)]
+            ncattr, = [s for s in fileID.ncattrs() if re.match(attr, s, re.I)]
             dinput['attributes'][attr] = fileID.getncattr(ncattr)
-        except (ValueError,AttributeError):
+        except (ValueError, AttributeError):
             pass
     # list of attributes to attempt to retrieve from included variables
-    attributes_list = ['description','units','long_name','calendar',
-        'standard_name','grid_mapping','_FillValue']
+    attributes_list = ['description', 'units', 'long_name', 'calendar',
+        'standard_name', 'grid_mapping', '_FillValue']
     # mapping between netCDF4 variable names and output names
     if not kwargs['field_mapping']:
         kwargs['field_mapping']['x'] = copy.copy(kwargs['xname'])
         kwargs['field_mapping']['y'] = copy.copy(kwargs['yname'])
         if kwargs['varname'] is not None:
             kwargs['field_mapping']['data'] = copy.copy(kwargs['varname'])
         if kwargs['timename'] is not None:
             kwargs['field_mapping']['time'] = copy.copy(kwargs['timename'])
     # for each variable
-    for key,nc in kwargs['field_mapping'].items():
+    for key, nc in kwargs['field_mapping'].items():
         # Getting the data from each NetCDF variable
         dinput[key] = fileID.variables[nc][:]
         # get attributes for the included variables
         dinput['attributes'][key] = {}
         for attr in attributes_list:
             # try getting the attribute
             try:
                 ncattr, = [s for s in fileID.variables[nc].ncattrs()
-                    if re.match(attr,s,re.I)]
+                    if re.match(attr, s, re.I)]
                 dinput['attributes'][key][attr] = \
                     fileID.variables[nc].getncattr(ncattr)
-            except (ValueError,AttributeError):
+            except (ValueError, AttributeError):
                 pass
     # get projection information if there is a grid_mapping attribute
-    if 'grid_mapping' in dinput['attributes']['data'].keys():
+    if 'data' in dinput.keys() and 'grid_mapping' in dinput['attributes']['data'].keys():
         # try getting the attribute
         grid_mapping = dinput['attributes']['data']['grid_mapping']
         # get coordinate reference system attributes
         dinput['attributes']['crs'] = {}
         for att_name in fileID[grid_mapping].ncattrs():
             dinput['attributes']['crs'][att_name] = \
                 fileID.variables[grid_mapping].getncattr(att_name)
@@ -202,15 +206,15 @@
         dinput['data'].fill_value = dinput['attributes']['data']['_FillValue']
         dinput['data'].mask = (dinput['data'].data == dinput['data'].fill_value)
     # Closing the NetCDF file
     fileID.close()
     # return the spatial variables
     return dinput
 
-def from_HDF5(filename, **kwargs):
+def from_HDF5(filename: str | pathlib.Path, **kwargs):
     """
     Read data from a HDF5 file
 
     Parameters
     ----------
     filename: str
         full path of input HDF5 file
@@ -224,28 +228,28 @@
         name for y-dimension variable
     varname: str, default 'data'
         name for data variable
     field_mapping: dict, default {}
         mapping between output variables and input HDF5
     """
     # set default keyword arguments
-    kwargs.setdefault('compression',None)
-    kwargs.setdefault('timename','time')
-    kwargs.setdefault('xname','lon')
-    kwargs.setdefault('yname','lat')
-    kwargs.setdefault('varname','data')
-    kwargs.setdefault('field_mapping',{})
+    kwargs.setdefault('compression', None)
+    kwargs.setdefault('timename', 'time')
+    kwargs.setdefault('xname', 'lon')
+    kwargs.setdefault('yname', 'lat')
+    kwargs.setdefault('varname', 'data')
+    kwargs.setdefault('field_mapping', {})
     # read data from HDF5 file
     # Open the HDF5 file for reading
     if (kwargs['compression'] == 'gzip'):
         # read gzip compressed file and extract into in-memory file object
-        with gzip.open(case_insensitive_filename(filename),'r') as f:
+        with gzip.open(case_insensitive_filename(filename), 'r') as f:
             fid = io.BytesIO(f.read())
         # set filename of BytesIO object
-        fid.filename = os.path.basename(filename)
+        fid.filename = filename.name
         # rewind to start of file
         fid.seek(0)
         # read as in-memory (diskless) HDF5 dataset from BytesIO object
         fileID = h5py.File(fid, 'r')
     elif (kwargs['compression'] == 'bytes'):
         # read as in-memory (diskless) HDF5 dataset
         fileID = h5py.File(filename, 'r')
@@ -255,50 +259,50 @@
     # Output HDF5 file information
     logging.info(fileID.filename)
     logging.info(list(fileID.keys()))
     # create python dictionary for output variables and attributes
     dinput = {}
     dinput['attributes'] = {}
     # get attributes for the file
-    for attr in ['title','description','projection']:
+    for attr in ['title', 'description', 'projection']:
         # try getting the attribute
         try:
             dinput['attributes'][attr] = fileID.attrs[attr]
-        except (KeyError,AttributeError):
+        except (KeyError, AttributeError):
             pass
     # list of attributes to attempt to retrieve from included variables
-    attributes_list = ['description','units','long_name','calendar',
-        'standard_name','grid_mapping','_FillValue']
+    attributes_list = ['description', 'units', 'long_name', 'calendar',
+        'standard_name', 'grid_mapping', '_FillValue']
     # mapping between HDF5 variable names and output names
     if not kwargs['field_mapping']:
         kwargs['field_mapping']['x'] = copy.copy(kwargs['xname'])
         kwargs['field_mapping']['y'] = copy.copy(kwargs['yname'])
         if kwargs['varname'] is not None:
             kwargs['field_mapping']['data'] = copy.copy(kwargs['varname'])
         if kwargs['timename'] is not None:
             kwargs['field_mapping']['time'] = copy.copy(kwargs['timename'])
     # for each variable
-    for key,h5 in kwargs['field_mapping'].items():
+    for key, h5 in kwargs['field_mapping'].items():
         # Getting the data from each HDF5 variable
         dinput[key] = np.copy(fileID[h5][:])
         # get attributes for the included variables
         dinput['attributes'][key] = {}
         for attr in attributes_list:
             # try getting the attribute
             try:
                 dinput['attributes'][key][attr] = fileID[h5].attrs[attr]
-            except (KeyError,AttributeError):
+            except (KeyError, AttributeError):
                 pass
     # get projection information if there is a grid_mapping attribute
-    if 'grid_mapping' in dinput['attributes']['data'].keys():
+    if 'data' in dinput.keys() and 'grid_mapping' in dinput['attributes']['data'].keys():
         # try getting the attribute
         grid_mapping = dinput['attributes']['data']['grid_mapping']
         # get coordinate reference system attributes
         dinput['attributes']['crs'] = {}
-        for att_name,att_val in fileID[grid_mapping].attrs.items():
+        for att_name, att_val in fileID[grid_mapping].attrs.items():
             dinput['attributes']['crs'][att_name] = att_val
         # get the spatial projection reference information from wkt
         # and overwrite the file-level projection attribute (if existing)
         srs = osgeo.osr.SpatialReference()
         srs.ImportFromWkt(dinput['attributes']['crs']['crs_wkt'])
         dinput['attributes']['projection'] = srs.ExportToProj4()
     # convert to masked array if fill values
@@ -307,73 +311,73 @@
         dinput['data'].fill_value = dinput['attributes']['data']['_FillValue']
         dinput['data'].mask = (dinput['data'].data == dinput['data'].fill_value)
     # Closing the HDF5 file
     fileID.close()
     # return the spatial variables
     return dinput
 
-def from_geotiff(filename, **kwargs):
+def from_geotiff(filename: str, **kwargs):
     """
     Read data from a geotiff file
 
     Parameters
     ----------
     filename: str
         full path of input geotiff file
     compression: str or NoneType, default None
         file compression type
     bounds: list or NoneType, default bounds
-        extent of the file to read: [xmin, xmax, ymin, ymax]
+        extent of the file to read: ``[xmin, xmax, ymin, ymax]``
     """
     # set default keyword arguments
-    kwargs.setdefault('compression',None)
-    kwargs.setdefault('bounds',None)
+    kwargs.setdefault('compression', None)
+    kwargs.setdefault('bounds', None)
     # Open the geotiff file for reading
     if (kwargs['compression'] == 'gzip'):
         # read as GDAL gzip virtual geotiff dataset
-        mmap_name = f"/vsigzip/{case_insensitive_filename(filename)}"
+        mmap_name = f"/vsigzip/{str(case_insensitive_filename(filename))}"
         ds = osgeo.gdal.Open(mmap_name)
     elif (kwargs['compression'] == 'bytes'):
         # read as GDAL memory-mapped (diskless) geotiff dataset
         mmap_name = f"/vsimem/{uuid.uuid4().hex}"
         osgeo.gdal.FileFromMemBuffer(mmap_name, filename.read())
         ds = osgeo.gdal.Open(mmap_name)
     else:
         # read geotiff dataset
-        ds = osgeo.gdal.Open(case_insensitive_filename(filename),
+        ds = osgeo.gdal.Open(str(case_insensitive_filename(filename)),
             osgeo.gdalconst.GA_ReadOnly)
     # print geotiff file if verbose
-    logging.info(filename)
+    logging.info(str(filename))
     # create python dictionary for output variables and attributes
     dinput = {}
-    dinput['attributes'] = {c:dict() for c in ['x','y','data']}
+    dinput['attributes'] = {c:dict() for c in ['x', 'y', 'data']}
     # get the spatial projection reference information
     srs = ds.GetSpatialRef()
     dinput['attributes']['projection'] = srs.ExportToProj4()
     dinput['attributes']['wkt'] = srs.ExportToWkt()
     # get dimensions
     xsize = ds.RasterXSize
     ysize = ds.RasterYSize
     bsize = ds.RasterCount
     # get geotiff info
     info_geotiff = ds.GetGeoTransform()
-    dinput['attributes']['spacing'] = (info_geotiff[1],info_geotiff[5])
+    dinput['attributes']['spacing'] = (info_geotiff[1], info_geotiff[5])
     # calculate image extents
     xmin = info_geotiff[0]
     ymax = info_geotiff[3]
     xmax = xmin + (xsize-1)*info_geotiff[1]
     ymin = ymax + (ysize-1)*info_geotiff[5]
     # x and y pixel center coordinates (converted from upper left)
     x = xmin + info_geotiff[1]/2.0 + np.arange(xsize)*info_geotiff[1]
     y = ymax + info_geotiff[5]/2.0 + np.arange(ysize)*info_geotiff[5]
     # if reducing to specified bounds
     if kwargs['bounds'] is not None:
         # reduced x and y limits
-        xlimits = (kwargs['bounds'][0],kwargs['bounds'][1])
-        ylimits = (kwargs['bounds'][2],kwargs['bounds'][3])
+        xlimits = (kwargs['bounds'][0], kwargs['bounds'][1])
+        ylimits = (kwargs['bounds'][2], kwargs['bounds'][3])
         # Specify offset and rows and columns to read
         xoffset = int((xlimits[0] - xmin)/info_geotiff[1])
         yoffset = int((ymax - ylimits[1])/np.abs(info_geotiff[5]))
         xcount = int((xlimits[1] - xlimits[0])/info_geotiff[1]) + 1
         ycount = int((ylimits[1] - ylimits[0])/np.abs(info_geotiff[5])) + 1
         # reduced x and y pixel center coordinates
         dinput['x'] = x[slice(xoffset, xoffset + xcount, None)]
@@ -394,36 +398,45 @@
         dinput['data'] = ds.ReadAsArray()
     # image extent
     dinput['attributes']['extent'] = (xmin, xmax, ymin, ymax)
     # set default time to zero for each band
     dinput.setdefault('time', np.zeros((bsize)))
     # check if image has fill values
     dinput['data'] = np.ma.asarray(dinput['data'])
-    dinput['data'].mask = np.zeros_like(dinput['data'],dtype=bool)
+    dinput['data'].mask = np.zeros_like(dinput['data'], dtype=bool)
     if ds.GetRasterBand(1).GetNoDataValue():
         # mask invalid values
         dinput['data'].fill_value = ds.GetRasterBand(1).GetNoDataValue()
         # create mask array for bad values
         dinput['data'].mask[:] = (dinput['data'].data == dinput['data'].fill_value)
         # set attribute for fill value
         dinput['attributes']['data']['_FillValue'] = dinput['data'].fill_value
     # close the dataset
     ds = None
     # return the spatial variables
     return dinput
 
-def convert_ellipsoid(phi1, h1, a1, f1, a2, f2, eps=1e-12, itmax=10):
+def convert_ellipsoid(
+        phi1: np.ndarray,
+        h1: np.ndarray,
+        a1: float,
+        f1: float,
+        a2: float,
+        f2: float,
+        eps: float = 1e-12,
+        itmax: int = 10
+    ):
     """
     Convert latitudes and heights to a different ellipsoid using Newton-Raphson
 
     Parameters
     ----------
-    phi1: float
+    phi1: np.ndarray
         latitude of input ellipsoid in degrees
-    h1: float
+    h1: np.ndarray
         height above input ellipsoid in meters
     a1: float
         semi-major axis of input ellipsoid
     f1: float
         flattening of input ellipsoid
     a2: float
         semi-major axis of output ellipsoid
@@ -433,22 +446,22 @@
         tolerance to prevent division by small numbers and
         to determine convergence
     itmax: int, default 10
         maximum number of iterations to use in Newton-Raphson
 
     Returns
     -------
-    phi2: float
+    phi2: np.ndarray
         latitude of output ellipsoid in degrees
-    h2: float
+    h2: np.ndarray
         height above output ellipsoid in meters
 
     References
     ----------
-    .. [1] J Meeus, Astronomical Algorithms, pp. 77-82 (1991)
+    .. [1] J. Meeus, *Astronomical Algorithms*, 2nd edition, 477 pp., (1998).
     """
     if (len(phi1) != len(h1)):
         raise ValueError('phi and h have incompatable dimensions')
     # semiminor axis of input and output ellipsoid
     b1 = (1.0 - f1)*a1
     b2 = (1.0 - f2)*a2
     # initialize output arrays
@@ -531,15 +544,15 @@
             k1 = b2 * hpr1sin
             k2 = a2 * hpr1cos
             # perform newton-raphson iteration to solve for u2
             # sin(u2) will not be close to zero since abs(phi1) > 45
             for i in range(0, itmax+1):
                 sinu2 = np.sin(u2)
                 fu2 = k0 * np.cos(u2) + k1 / np.tan(u2) - k2
-                fu2p =  -1 * (k0 * sinu2 + k1 / (sinu2 * sinu2))
+                fu2p = -1 * (k0 * sinu2 + k1 / (sinu2 * sinu2))
                 if (np.abs(fu2p) < eps):
                     break
                 else:
                     delta = fu2 / fu2p
                     u2 -= delta
                     if (np.abs(delta) < eps):
                         break
@@ -550,40 +563,46 @@
                 phi2[N] = np.sign(phi2[N])*90.0
             # calculate height
             h2[N] = (hpr1sin - b2 * np.sin(u2)) / np.sin(phi2r)
 
     # return the latitude and height
     return (phi2, h2)
 
-def compute_delta_h(a1, f1, a2, f2, lat):
+def compute_delta_h(
+        a1: float,
+        f1: float,
+        a2: float,
+        f2: float,
+        lat: np.ndarray
+    ):
     """
     Compute difference in elevation for two ellipsoids at a given
         latitude using a simplified empirical equation
 
     Parameters
     ----------
     a1: float
         semi-major axis of input ellipsoid
     f1: float
         flattening of input ellipsoid
     a2: float
         semi-major axis of output ellipsoid
     f2: float
         flattening of output ellipsoid
-    lat: float
+    lat: np.ndarray
         latitudes (degrees north)
 
     Returns
     -------
-    delta_h: float
+    delta_h: np.ndarray
         difference in elevation for two ellipsoids
 
     References
     ----------
-    .. [1] J Meeus, Astronomical Algorithms, pp. 77-82 (1991)
+    .. [1] J Meeus, *Astronomical Algorithms*, pp. 77--82, (1991).
     """
     # force phi into range -90 <= phi <= 90
     gt90, = np.nonzero((lat < -90.0) | (lat > 90.0))
     lat[gt90] = np.sign(lat[gt90])*90.0
     # semiminor axis of input and output ellipsoid
     b1 = (1.0 - f1)*a1
     b2 = (1.0 - f2)*a2
@@ -592,49 +611,57 @@
     delta_b = b2 - b1
     # compute differences between ellipsoids
     # delta_h = -(delta_a * cos(phi)^2 + delta_b * sin(phi)^2)
     phi = lat * np.pi/180.0
     delta_h = -(delta_a*np.cos(phi)**2 + delta_b*np.sin(phi)**2)
     return delta_h
 
-def wrap_longitudes(lon):
+def wrap_longitudes(lon: float | np.ndarray):
     """
     Wraps longitudes to range from -180 to +180
 
     Parameters
     ----------
-    lon: float
+    lon: float or np.ndarray
         longitude (degrees east)
     """
     phi = np.arctan2(np.sin(lon*np.pi/180.0), np.cos(lon*np.pi/180.0))
     # convert phi from radians to degrees
     return phi*180.0/np.pi
 
-def to_cartesian(lon, lat, h=0.0, a_axis=6378137.0, flat=1.0/298.257223563):
+def to_cartesian(
+        lon: np.ndarray,
+        lat: np.ndarray,
+        h: float | np.ndarray = 0.0,
+        a_axis: float = 6378137.0,
+        flat: float = 1.0/298.257223563
+    ):
     """
     Converts geodetic coordinates to Cartesian coordinates
 
     Parameters
     ----------
-    lon: float
+    lon: np.ndarray
         longitude (degrees east)
-    lat: float
+    lat: np.ndarray
         latitude (degrees north)
-    h: float, default 0.0
+    h: float or np.ndarray, default 0.0
         height above ellipsoid (or sphere)
     a_axis: float, default 6378137.0
         semimajor axis of the ellipsoid
+
         for spherical coordinates set to radius of the Earth
     flat: float, default 1.0/298.257223563
         ellipsoidal flattening
+
         for spherical coordinates set to 0
     """
-    # verify axes
-    lon = np.atleast_1d(lon)
-    lat = np.atleast_1d(lat)
+    # verify axes and copy to not modify inputs
+    lon = np.atleast_1d(np.copy(lon))
+    lat = np.atleast_1d(np.copy(lat))
     # fix coordinates to be 0:360
     lon[lon < 0] += 360.0
     # Linear eccentricity and first numerical eccentricity
     lin_ecc = np.sqrt((2.0*flat - flat**2)*a_axis**2)
     ecc1 = lin_ecc/a_axis
     # convert from geodetic latitude to geocentric latitude
     dtr = np.pi/180.0
@@ -643,135 +670,350 @@
     # prime vertical radius of curvature
     N = a_axis/np.sqrt(1.0 - ecc1**2.0*np.sin(latitude_geodetic_rad)**2.0)
     # calculate X, Y and Z from geodetic latitude and longitude
     X = (N + h) * np.cos(latitude_geodetic_rad) * np.cos(lon*dtr)
     Y = (N + h) * np.cos(latitude_geodetic_rad) * np.sin(lon*dtr)
     Z = (N * (1.0 - ecc1**2.0) + h) * np.sin(latitude_geodetic_rad)
     # return the cartesian coordinates
-    return (X,Y,Z)
+    return (X, Y, Z)
 
-def to_sphere(x, y, z):
+def to_sphere(x: np.ndarray, y: np.ndarray, z: np.ndarray):
     """
     Convert from cartesian coordinates to spherical coordinates
 
     Parameters
     ----------
-    x, float
+    x, np.ndarray
         cartesian x-coordinates
-    y, float
+    y, np.ndarray
         cartesian y-coordinates
-    z, float
+    z, np.ndarray
         cartesian z-coordinates
     """
+    # verify axes and copy to not modify inputs
+    x = np.atleast_1d(np.copy(x))
+    y = np.atleast_1d(np.copy(y))
+    z = np.atleast_1d(np.copy(z))
     # calculate radius
     rad = np.sqrt(x**2.0 + y**2.0 + z**2.0)
     # calculate angular coordinates
     # phi: azimuthal angle
-    phi = np.arctan2(y,x)
+    phi = np.arctan2(y, x)
     # th: polar angle
     th = np.arccos(z/rad)
     # convert to degrees and fix to 0:360
     lon = 180.0*phi/np.pi
     if np.any(lon < 0):
         lt0 = np.nonzero(lon < 0)
         lon[lt0] += 360.0
     # convert to degrees and fix to -90:90
     lat = 90.0 - (180.0*th/np.pi)
     np.clip(lat, -90, 90, out=lat)
     # return latitude, longitude and radius
-    return (lon,lat,rad)
+    return (lon, lat, rad)
+
+def to_geodetic(
+        x: np.ndarray,
+        y: np.ndarray,
+        z: np.ndarray,
+        a_axis: float = 6378137.0,
+        flat: float = 1.0/298.257223563,
+        method: str = 'bowring',
+        eps: float = np.finfo(np.float64).eps,
+        iterations: int = 10
+    ):
+    """
+    Convert from cartesian coordinates to geodetic coordinates
+    using either iterative or closed-form methods
+
+    Parameters
+    ----------
+    x, float
+        cartesian x-coordinates
+    y, float
+        cartesian y-coordinates
+    z, float
+        cartesian z-coordinates
+    a_axis: float, default 6378137.0
+        semimajor axis of the ellipsoid
+    flat: float, default 1.0/298.257223563
+        ellipsoidal flattening
+    method: str, default 'bowring'
+        method to use for conversion
+
+            - ``'moritz'``: iterative solution
+            - ``'bowring'``: iterative solution
+            - ``'zhu'``: closed-form solution
+    eps: float, default np.finfo(np.float64).eps
+        tolerance for iterative methods
+    iterations: int, default 10
+        maximum number of iterations
+    """
+    # verify axes and copy to not modify inputs
+    x = np.atleast_1d(np.copy(x))
+    y = np.atleast_1d(np.copy(y))
+    z = np.atleast_1d(np.copy(z))
+    # calculate the geodetic coordinates using the specified method
+    if (method.lower() == 'moritz'):
+        return _moritz_iterative(x, y, z, a_axis=a_axis, flat=flat,
+            eps=eps, iterations=iterations)
+    elif (method.lower() == 'bowring'):
+        return _bowring_iterative(x, y, z, a_axis=a_axis, flat=flat,
+            eps=eps, iterations=iterations)
+    elif (method.lower() == 'zhu'):
+        return _zhu_closed_form(x, y, z, a_axis=a_axis, flat=flat)
+    else:
+        raise ValueError(f'Unknown conversion method: {method}')
 
-def to_geodetic(x, y, z, a_axis=6378137.0, flat=1.0/298.257223563):
+def _moritz_iterative(
+        x: np.ndarray,
+        y: np.ndarray,
+        z: np.ndarray,
+        a_axis: float = 6378137.0,
+        flat: float = 1.0/298.257223563,
+        eps: float = np.finfo(np.float64).eps,
+        iterations: int = 10
+    ):
     """
     Convert from cartesian coordinates to geodetic coordinates
-    using a closed form solution
+    using the iterative solution of [1]_
 
     Parameters
     ----------
     x, float
         cartesian x-coordinates
     y, float
         cartesian y-coordinates
     z, float
         cartesian z-coordinates
     a_axis: float, default 6378137.0
         semimajor axis of the ellipsoid
     flat: float, default 1.0/298.257223563
         ellipsoidal flattening
+    eps: float, default np.finfo(np.float64).eps
+        tolerance for iterative method
+    iterations: int, default 10
+        maximum number of iterations
 
     References
     ----------
-    .. [1] J Zhu "Exact conversion of Earth-centered, Earth-fixed
-        coordinates to geodetic coordinates"
-        Journal of Guidance, Control, and Dynamics,
-        16(2), 389--391, 1993
-        https://arc.aiaa.org/doi/abs/10.2514/3.21016
+    .. [1] B. Hofmann-Wellenhof and H. Moritz,
+        *Physical Geodesy*, 2nd Edition, 403 pp., (2006).
+        `doi: 10.1007/978-3-211-33545-1
+        <https://doi.org/10.1007/978-3-211-33545-1>`_
     """
-    # semiminor axis of the WGS84 ellipsoid [m]
-    b_axis = (1.0 - flat)*a_axis
     # Linear eccentricity and first numerical eccentricity
     lin_ecc = np.sqrt((2.0*flat - flat**2)*a_axis**2)
     ecc1 = lin_ecc/a_axis
+    # degrees to radians
+    dtr = np.pi/180.0
+    # calculate longitude
+    lon = np.arctan2(y, x)/dtr
+    # set initial estimate of height to 0
+    h = np.zeros_like(lon)
+    h0 = np.inf*np.ones_like(lon)
+    # calculate radius of parallel
+    p = np.sqrt(x**2 + y**2)
+    # initial estimated value for phi using h=0
+    phi = np.arctan(z/(p*(1.0 - ecc1**2)))
+    # iterate to tolerance or to maximum number of iterations
+    i = 0
+    while np.any(np.abs(h - h0) > eps) and (i <= iterations):
+        # copy previous iteration of height
+        h0 = np.copy(h)
+        # calculate radius of curvature
+        N = a_axis/np.sqrt(1.0 - ecc1**2 * np.sin(phi)**2)
+        # estimate new value of height
+        h = p/np.cos(phi) - N
+        # estimate new value for latitude using heights
+        phi = np.arctan(z/(p*(1.0 - ecc1**2*N/(N + h))))
+        # add to iterator
+        i += 1
+    # return latitude, longitude and height
+    return (lon, phi/dtr, h)
+
+def _bowring_iterative(
+        x: np.ndarray,
+        y: np.ndarray,
+        z: np.ndarray,
+        a_axis: float = 6378137.0,
+        flat: float = 1.0/298.257223563,
+        eps: float = np.finfo(np.float64).eps,
+        iterations: int = 10
+    ):
+    """
+    Convert from cartesian coordinates to geodetic coordinates
+    using the iterative solution of [1]_ [2]_
+
+    Parameters
+    ----------
+    x, float
+        cartesian x-coordinates
+    y, float
+        cartesian y-coordinates
+    z, float
+        cartesian z-coordinates
+    a_axis: float, default 6378137.0
+        semimajor axis of the ellipsoid
+    flat: float, default 1.0/298.257223563
+        ellipsoidal flattening
+    eps: float, default np.finfo(np.float64).eps
+        tolerance for iterative method
+    iterations: int, default 10
+        maximum number of iterations
+
+    References
+    ----------
+    .. [1] B. R. Bowring, "Transformation from spatial
+        to geodetic coordinates," *Survey Review*, 23(181),
+        323--327, (1976). `doi: 10.1179/sre.1976.23.181.323
+        <https://doi.org/10.1179/sre.1976.23.181.323>`_
+    .. [2] B. R. Bowring, "The Accuracy Of Geodetic
+        Latitude and Height Equations," *Survey Review*, 28(218),
+        202--206, (1985). `doi: 10.1179/sre.1985.28.218.202
+        <https://doi.org/10.1179/sre.1985.28.218.202>`_
+    """
+    # semiminor axis of the WGS84 ellipsoid [m]
+    b_axis = (1.0 - flat)*a_axis
+    # Linear eccentricity
+    lin_ecc = np.sqrt((2.0*flat - flat**2)*a_axis**2)
+    # square of first and second numerical eccentricity
+    e12 = lin_ecc**2/a_axis**2
+    e22 = lin_ecc**2/b_axis**2
+    # degrees to radians
+    dtr = np.pi/180.0
+    # calculate longitude
+    lon = np.arctan2(y, x)/dtr
+    # calculate radius of parallel
+    p = np.sqrt(x**2 + y**2)
+    # initial estimated value for reduced parametric latitude
+    u = np.arctan(a_axis*z/(b_axis*p))
+    # initial estimated value for latitude
+    phi = np.arctan((z + e22*b_axis*np.sin(u)**3) /
+        (p - e12*a_axis*np.cos(u)**3))
+    phi0 = np.inf*np.ones_like(lon)
+    # iterate to tolerance or to maximum number of iterations
+    i = 0
+    while np.any(np.abs(phi - phi0) > eps) and (i <= iterations):
+        # copy previous iteration of phi
+        phi0 = np.copy(phi)
+        # calculate reduced parametric latitude
+        u = np.arctan(b_axis*np.tan(phi)/a_axis)
+        # estimate new value of latitude
+        phi = np.arctan((z + e22*b_axis*np.sin(u)**3) /
+            (p - e12*a_axis*np.cos(u)**3))
+        # add to iterator
+        i += 1
+    # calculate final radius of curvature
+    N = a_axis/np.sqrt(1.0 - e12 * np.sin(phi)**2)
+    # estimate final height (Bowring, 1985)
+    h = p*np.cos(phi) + z*np.sin(phi) - a_axis**2/N
+    # return latitude, longitude and height
+    return (lon, phi/dtr, h)
+
+def _zhu_closed_form(
+        x: np.ndarray,
+        y: np.ndarray,
+        z: np.ndarray,
+        a_axis: float = 6378137.0,
+        flat: float = 1.0/298.257223563,
+    ):
+    """
+    Convert from cartesian coordinates to geodetic coordinates
+    using the closed-form solution of [1]_
+
+    Parameters
+    ----------
+    x, float
+        cartesian x-coordinates
+    y, float
+        cartesian y-coordinates
+    z, float
+        cartesian z-coordinates
+    a_axis: float, default 6378137.0
+        semimajor axis of the ellipsoid
+    flat: float, default 1.0/298.257223563
+        ellipsoidal flattening
+
+    References
+    ----------
+    .. [1] J. Zhu, "Exact conversion of Earth-centered,
+        Earth-fixed coordinates to geodetic coordinates,"
+        *Journal of Guidance, Control, and Dynamics*,
+        16(2), 389--391, (1993). `doi: 10.2514/3.21016
+        <https://arc.aiaa.org/doi/abs/10.2514/3.21016>`_
+    """
+    # semiminor axis of the WGS84 ellipsoid [m]
+    b_axis = (1.0 - flat)*a_axis
+    # Linear eccentricity
+    lin_ecc = np.sqrt((2.0*flat - flat**2)*a_axis**2)
     # square of first numerical eccentricity
-    e12 = ecc1**2
+    e12 = lin_ecc**2/a_axis**2
     # degrees to radians
     dtr = np.pi/180.0
-    # calculate distance
-    w = np.sqrt(x**2 + y**2)
     # calculate longitude
-    lon = np.arctan2(y,x)/dtr
+    lon = np.arctan2(y, x)/dtr
+    # calculate radius of parallel
+    w = np.sqrt(x**2 + y**2)
+    # allocate for output latitude and height
     lat = np.zeros_like(lon)
     h = np.zeros_like(lon)
-    if (w == 0):
+    if np.any(w == 0):
         # special case where w == 0 (exact polar solution)
-        h = np.sign(z)*z - b_axis
-        lat = 90.0*np.sign(z)
+        ind, = np.nonzero(w == 0)
+        h[ind] = np.sign(z[ind])*z[ind] - b_axis
+        lat[ind] = 90.0*np.sign(z[ind])
     else:
         # all other cases
+        ind, = np.nonzero(w != 0)
         l = e12/2.0
-        m = (w/a_axis)**2.0
-        n = ((1.0-e12)*z/b_axis)**2.0
+        m = (w[ind]/a_axis)**2.0
+        n = ((1.0 - e12)*z[ind]/b_axis)**2.0
         i = -(2.0*l**2 + m + n)/2.0
         k = (l**2.0 - m - n)*l**2.0
         q = (1.0/216.0)*(m + n - 4.0*l**2)**3.0 + m*n*l**2.0
         D = np.sqrt((2.0*q - m*n*l**2)*m*n*l**2)
-        B = i/3.0 - (q+D)**(1.0/3.0) - (q-D)**(1.0/3.0)
-        t = np.sqrt(np.sqrt(B**2-k) - (B+i)/2.0)-np.sign(m-n)*np.sqrt((B-i)/2.0)
-        wi = w/(t+l)
-        zi = (1.0-e12)*z/(t-l)
+        B = i/3.0 - (q + D)**(1.0/3.0) - (q - D)**(1.0/3.0)
+        t = np.sqrt(np.sqrt(B**2-k) - (B + i)/2.0) - \
+            np.sign(m - n)*np.sqrt((B - i)/2.0)
+        wi = w/(t + l)
+        zi = (1.0 - e12)*z[ind]/(t - l)
         # calculate latitude and height
-        lat = np.arctan2(zi,((1.0-e12)*wi))/dtr
-        h = np.sign(t-1.0+l)*np.sqrt((w-wi)**2.0 + (z-zi)**2.0)
+        lat[ind] = np.arctan2(zi, ((1.0 - e12)*wi))/dtr
+        h[ind] = np.sign(t-1.0+l)*np.sqrt((w-wi)**2.0 + (z[ind]-zi)**2.0)
     # return latitude, longitude and height
-    return (lon,lat,h)
+    return (lon, lat, h)
 
-def scale_areas(lat, flat=1.0/298.257223563, ref=70.0):
+def scale_areas(
+        lat: np.ndarray,
+        flat: float=1.0/298.257223563,
+        ref: float=70.0
+    ):
     """
     Calculates area scaling factors for a polar stereographic projection
-    including special case of at the exact pole
+    including special case of at the exact pole [1]_ [2]_
 
     Parameters
     ----------
-    lat: float,
+    lat: np.ndarray
         latitude (degrees north)
     flat: float, default 1.0/298.257223563
         ellipsoidal flattening
     ref: float, default 70.0
         reference latitude (true scale latitude)
 
     Returns
     -------
-    scale: float
+    scale: np.ndarray
         area scaling factors at input latitudes
 
     References
     ----------
-    .. [1] Snyder, J P (1982) Map Projections used by the U.S. Geological Survey
-        Forward formulas for the ellipsoid.  Geological Survey Bulletin
-        1532, U.S. Government Printing Office.
+    .. [1] J. P. Snyder, *Map Projections used by the U.S. Geological Survey*,
+        Geological Survey Bulletin 1532, U.S. Government Printing Office, (1982).
     .. [2] JPL Technical Memorandum 3349-85-101
     """
     # convert latitude from degrees to positive radians
     theta = np.abs(lat)*np.pi/180.0
     # convert reference latitude from degrees to positive radians
     theta_ref = np.abs(ref)*np.pi/180.0
     # square of the eccentricity of the ellipsoid
@@ -787,33 +1029,48 @@
     mref = np.cos(theta_ref)/np.sqrt(1.0 - ecc2*np.sin(theta_ref)**2)
     tref = np.tan(np.pi/4.0 - theta_ref/2.0)/((1.0 - ecc*np.sin(theta_ref)) / \
         (1.0 + ecc*np.sin(theta_ref)))**(ecc/2.0)
     # distance scaling
     k = (mref/m)*(t/tref)
     kp = 0.5*mref*np.sqrt(((1.0+ecc)**(1.0+ecc))*((1.0-ecc)**(1.0-ecc)))/tref
     # area scaling
-    scale = np.where(np.isclose(theta,np.pi/2.0),1.0/(kp**2),1.0/(k**2))
+    scale = np.where(np.isclose(theta, np.pi/2.0), 1.0/(kp**2), 1.0/(k**2))
     return scale
 
 # PURPOSE: check a specified 2D point is inside a specified 2D polygon
-def inside_polygon(x, y, xpts, ypts, threshold=0.01):
+def inside_polygon(
+        x: np.ndarray,
+        y: np.ndarray,
+        xpts: np.ndarray,
+        ypts: np.ndarray,
+        threshold: float = 0.01
+    ):
     """
     Indicates whether a specified 2D point is inside a specified 2D polygon
 
-    Inputs:
-        x: x coordinates of the 2D point(s) to check.
-        y: y coordinates of the 2D point(s) to check.
-        xpts: The x coordinates of the 2D polygon.
-        ypts: The y coordinates of the 2D polygon.
+    Parameters
+    ----------
+    x: np.ndarray
+        x-coordinates of the 2D point(s) to check
+    y: np.ndarray
+        y-coordinates of the 2D point(s) to check
+    xpts: np.ndarray
+        x-coordinates of the 2D polygon.
+    ypts: np.ndarray
+        y-coordinates of the 2D polygon
+    threshold: float, default 0.01
+        minimum angle for checking if inside polygon
 
-    Options:
-        threshold: minimum angle for checking if inside polygon
+    Returns
+    -------
+    flag: np.ndarray
+        flag denoting if points are within polygon
 
-    Returns:
-        flag: True for points within polygon, False for points outside polygon
+        - ``True``: within polygon
+        - ``False``: outside polygon
     """
     # create numpy arrays for 2D points
     x = np.atleast_1d(x)
     y = np.atleast_1d(y)
     nn = len(x)
     # create numpy arrays for polygon points
     xpts = np.array(xpts)
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/time.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/time.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 #!/usr/bin/env python
 u"""
 time.py
-Written by Tyler Sutterley (10/2022)
+Written by Tyler Sutterley (05/2023)
 Utilities for calculating time operations
 
 PYTHON DEPENDENCIES:
     numpy: Scientific Computing Tools For Python
         https://numpy.org
     dateutil: powerful extensions to datetime
         https://dateutil.readthedocs.io/en/stable/
     lxml: processing XML and HTML in Python
         https://pypi.python.org/pypi/lxml
 
 PROGRAM DEPENDENCIES:
     utilities.py: download and management utilities for syncing files
 
 UPDATE HISTORY:
+    Updated 05/2023: allow epoch arguments to be numpy datetime64 or strings
+        function to convert a string with time zone information to datetime
+    Updated 04/2023: using pathlib to define and expand paths
+    Updated 03/2023: add basic variable typing to function inputs
+    Updated 12/2022: output variables for some standard epochs
+    Updated 11/2022: use f-strings for formatting verbose or ascii output
     Updated 10/2022: added more time parsing for longer periods
+        added encoding for reading leap seconds ascii files
     Updated 08/2022: output variables to unit conversion to seconds
         and the number of days per month for both leap and standard years
     Updated 05/2022: changed keyword arguments to camel case
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 04/2021: updated NIST ftp server url for leap-seconds.list
     Updated 03/2021: replaced numpy bool/int to prevent deprecation warnings
     Updated 02/2021: parse date strings "time-units since yyyy-mm-dd hh:mm:ss"
         replaced numpy int/float to prevent deprecation warnings
     Updated 01/2021: added ftp connection checks
         merged with convert_julian and convert_calendar_decimal
         added calendar_days routine to get number of days per month
     Updated 08/2020: added NASA Earthdata routines for downloading from NSIDC
     Written 07/2020
 """
+from __future__ import annotations
+
 import re
 import copy
 import logging
+import pathlib
 import warnings
 import datetime
 import traceback
 import numpy as np
 import dateutil.parser
 import icesat2_toolkit.utilities
 
@@ -59,74 +69,108 @@
 _to_sec['month'] = 30.0 * 86400.0
 _to_sec['months'] = 30.0 * 86400.0
 _to_sec['common_year'] = 365.0 * 86400.0
 _to_sec['common_years'] = 365.0 * 86400.0
 _to_sec['year'] = 365.25 * 86400.0
 _to_sec['years'] = 365.25 * 86400.0
 
+# standard epochs
+_mjd_epoch = (1858, 11, 17, 0, 0, 0)
+_ntp_epoch = (1900, 1, 1, 0, 0, 0)
+_unix_epoch = (1970, 1, 1, 0, 0, 0)
+_gps_epoch = (1980, 1, 6, 0, 0, 0)
+_tide_epoch = (1992, 1, 1, 0, 0, 0)
+_j2000_epoch = (2000, 1, 1, 12, 0, 0)
+_atlas_sdp_epoch = (2018, 1, 1, 0, 0, 0)
+
+# PURPOSE: parse a date string and convert to a datetime object in UTC
+def parse(date_string: str):
+    """
+    Parse a date string and convert to a naive ``datetime`` object in UTC
+
+    Parameters
+    ----------
+    date_string: str
+        formatted time string
+
+    Returns
+    -------
+    date: obj
+        output ``datetime`` object
+    """
+    # parse the date string
+    date = dateutil.parser.parse(date_string)
+    # convert to UTC if containing time-zone information
+    # then drop the timezone information to prevent unsupported errors
+    if date.tzinfo:
+        date = date.astimezone(dateutil.tz.UTC).replace(tzinfo=None)
+    # return the datetime object
+    return date
+
 # PURPOSE: parse a date string into epoch and units scale
-def parse_date_string(date_string):
+def parse_date_string(date_string: str):
     """
-    parse a date string of the form
+    Parse a date string of the form
 
     - time-units since ``yyyy-mm-dd hh:mm:ss``
     - ``yyyy-mm-dd hh:mm:ss`` for exact calendar dates
 
     Parameters
     ----------
     date_string: str
         time-units since yyyy-mm-dd hh:mm:ss
 
     Returns
     -------
     epoch: list
-        epoch of delta time
+        epoch of ``delta_time``
     conversion_factor: float
         multiplication factor to convert to seconds
     """
     # try parsing the original date string as a date
     try:
-        epoch = dateutil.parser.parse(date_string)
+        epoch = parse(date_string)
     except ValueError:
         pass
     else:
         # return the epoch (as list)
-        return (datetime_to_list(epoch),0.0)
+        return (datetime_to_list(epoch), 0.0)
     # split the date string into units and epoch
     units,epoch = split_date_string(date_string)
     if units not in _to_sec.keys():
         raise ValueError(f'Invalid units: {units}')
     # return the epoch (as list) and the time unit conversion factors
     return (datetime_to_list(epoch), _to_sec[units])
 
 # PURPOSE: split a date string into units and epoch
-def split_date_string(date_string):
+def split_date_string(date_string: str):
     """
-    split a date string into units and epoch
+    Split a date string into units and epoch
 
     Parameters
     ----------
     date_string: str
         time-units since yyyy-mm-dd hh:mm:ss
     """
     try:
         units,_,epoch = date_string.split(None, 2)
     except ValueError:
         raise ValueError(f'Invalid format: {date_string}')
     else:
-        return (units.lower(), dateutil.parser.parse(epoch))
+        return (units.lower(), parse(epoch))
 
 # PURPOSE: convert a datetime object into a list
 def datetime_to_list(date):
     """
-    convert a datetime object into a list
+    Convert a ``datetime`` object into a list
 
     Parameters
     ----------
-    date: datetime object
+    date: obj
+        Input ``datetime`` object to convert
 
     Returns
     -------
     date: list
         [year,month,day,hour,minute,second]
     """
     return [date.year, date.month, date.day,
@@ -134,21 +178,21 @@
 
 # days per month in a leap and a standard year
 # only difference is February (29 vs. 28)
 _dpm_leap = [31, 29, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
 _dpm_stnd = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]
 
 # PURPOSE: gets the number of days per month for a given year
-def calendar_days(year):
+def calendar_days(year: int | float | np.ndarray) -> np.ndarray:
     """
     Calculates the number of days per month for a given year
 
     Parameters
     ----------
-    year: int or float
+    year: int, float or np.ndarray
         calendar year
 
     Returns
     -------
     dpm: list
         number of days for each month
     """
@@ -165,133 +209,174 @@
     m4000 = (year % 4000)
     # find indices for standard years and leap years using criteria
     if ((m4 == 0) & (m100 != 0) | (m400 == 0) & (m4000 != 0)):
         return np.array(_dpm_leap, dtype=np.float64)
     elif ((m4 != 0) | (m100 == 0) & (m400 != 0) | (m4000 == 0)):
         return np.array(_dpm_stnd, dtype=np.float64)
 
-# PURPOSE: convert a numpy datetime array to delta times from the UNIX epoch
-def convert_datetime(date, epoch=(1970, 1, 1, 0, 0, 0)):
+# PURPOSE: convert a numpy datetime array to delta times since an epoch
+def convert_datetime(
+        date: float | np.ndarray,
+        epoch: str | tuple | list | np.datetime64 = _unix_epoch
+    ):
     """
-    Convert a numpy datetime array to seconds since ``epoch``
+    Convert a ``numpy`` ``datetime`` array to seconds since ``epoch``
 
     Parameters
     ----------
-    date: obj
+    date: np.ndarray
         numpy datetime array
-    epoch: tuple, default (1970,1,1,0,0,0)
-        epoch for output delta_time
+    epoch: str, tuple, list, np.ndarray, default (1970,1,1,0,0,0)
+        epoch for output ``delta_time``
 
     Returns
     -------
     delta_time: float
         seconds since epoch
     """
-    epoch = datetime.datetime(*epoch)
-    return (date - np.datetime64(epoch)) / np.timedelta64(1, 's')
+    # convert epoch to datetime variables
+    if isinstance(epoch, (tuple, list)):
+        epoch = np.datetime64(datetime.datetime(*epoch))
+    elif isinstance(epoch, str):
+        epoch = np.datetime64(parse(epoch))
+    # convert to delta time
+    return (date - epoch) / np.timedelta64(1, 's')
 
 # PURPOSE: convert times from seconds since epoch1 to time since epoch2
-def convert_delta_time(delta_time, epoch1=None, epoch2=None, scale=1.0):
+def convert_delta_time(
+        delta_time: np.ndarray,
+        epoch1: str | tuple | list | np.datetime64 | None = None,
+        epoch2: str | tuple | list | np.datetime64 | None = None,
+        scale: float = 1.0
+    ):
     """
     Convert delta time from seconds since ``epoch1`` to time since ``epoch2``
 
     Parameters
     ----------
-    delta_time: float
+    delta_time: np.ndarray
         seconds since epoch1
     epoch1: tuple or NoneType, default None
-        epoch for input delta_time
+        epoch for input ``delta_time``
     epoch2: tuple or NoneType, default None
-        epoch for output delta_time
+        epoch for output ``delta_time``
     scale: float, default 1.0
         scaling factor for converting time to output units
     """
-    epoch1 = datetime.datetime(*epoch1)
-    epoch2 = datetime.datetime(*epoch2)
-    delta_time_epochs = (epoch2 - epoch1).total_seconds()
+    # convert epochs to datetime variables
+    if isinstance(epoch1, (tuple, list)):
+        epoch1 = np.datetime64(datetime.datetime(*epoch1))
+    elif isinstance(epoch1, str):
+        epoch1 = np.datetime64(parse(epoch1))
+    if isinstance(epoch2, (tuple, list)):
+        epoch2 = np.datetime64(datetime.datetime(*epoch2))
+    elif isinstance(epoch2, str):
+        epoch2 = np.datetime64(parse(epoch2))
+    # calculate the total difference in time in seconds
+    delta_time_epochs = (epoch2 - epoch1) / np.timedelta64(1, 's')
     # subtract difference in time and rescale to output units
     return scale*(delta_time - delta_time_epochs)
 
 # PURPOSE: calculate the delta time from calendar date
 # http://scienceworld.wolfram.com/astronomy/JulianDate.html
-def convert_calendar_dates(year, month, day, hour=0.0, minute=0.0, second=0.0,
-    epoch=(1992, 1, 1, 0, 0, 0), scale=1.0):
+def convert_calendar_dates(
+        year: np.ndarray,
+        month: np.ndarray,
+        day: np.ndarray,
+        hour: np.ndarray | float = 0.0,
+        minute: np.ndarray | float = 0.0,
+        second: np.ndarray | float = 0.0,
+        epoch: tuple | list | np.datetime64 = _tide_epoch,
+        scale: float = 1.0
+    ) -> np.ndarray:
     """
     Calculate the time in time units since ``epoch`` from calendar dates
 
     Parameters
     ----------
-    year: float
+    year: np.ndarray
         calendar year
-    month: float
+    month: np.ndarray
         month of the year
-    day: float
+    day: np.ndarray
         day of the month
-    hour: float, default 0.0
+    hour: np.ndarray or float, default 0.0
         hour of the day
-    minute: float, default 0.0
+    minute: np.ndarray or float, default 0.0
         minute of the hour
-    second: float, default 0.0
+    second: np.ndarray or float, default 0.0
         second of the minute
-    epoch: tuple, default (1992,1,1,0,0,0)
-        epoch for output delta_time
+    epoch: tuple or list, default icesat2_toolkit.time._tide_epoch
+        epoch for output ``delta_time``
     scale: float, default 1.0
         scaling factor for converting time to output units
 
     Returns
     -------
-    delta_time: float
-        days since epoch
+    delta_time: np.ndarray
+        time since epoch
     """
     # calculate date in Modified Julian Days (MJD) from calendar date
     # MJD: days since November 17, 1858 (1858-11-17T00:00:00)
     MJD = 367.0*year - np.floor(7.0*(year + np.floor((month+9.0)/12.0))/4.0) - \
         np.floor(3.0*(np.floor((year + (month - 9.0)/7.0)/100.0) + 1.0)/4.0) + \
         np.floor(275.0*month/9.0) + day + hour/24.0 + minute/1440.0 + \
         second/86400.0 + 1721028.5 - 2400000.5
-    epoch1 = datetime.datetime(1858, 11, 17, 0, 0, 0)
-    epoch2 = datetime.datetime(*epoch)
-    delta_time_epochs = (epoch2 - epoch1).total_seconds()
-    # return the date in days since epoch
-    return scale*np.array(MJD - delta_time_epochs/86400.0, dtype=np.float64)
+    # convert epochs to datetime variables
+    epoch1 = np.datetime64(datetime.datetime(*_mjd_epoch))
+    if isinstance(epoch, (tuple, list)):
+        epoch = np.datetime64(datetime.datetime(*epoch))
+    elif isinstance(epoch, str):
+        epoch = np.datetime64(parse(epoch))
+    # calculate the total difference in time in days
+    delta_time_epochs = (epoch - epoch1) / np.timedelta64(1, 'D')
+    # return the date in units (default days) since epoch
+    return scale*np.array(MJD - delta_time_epochs, dtype=np.float64)
 
 # PURPOSE: Converts from calendar dates into decimal years
-def convert_calendar_decimal(year, month, day=None, hour=None, minute=None,
-    second=None, DofY=None):
+def convert_calendar_decimal(
+        year: np.ndarray,
+        month: np.ndarray,
+        day: np.ndarray,
+        hour: np.ndarray | float | None = None,
+        minute: np.ndarray | float | None = None,
+        second: np.ndarray | float | None = None,
+        DofY: np.ndarray | float | None = None,
+    ) -> np.ndarray:
     """
     Converts from calendar date into decimal years taking into
     account leap years
 
     Parameters
     ----------
-    year: float
+    year: np.ndarray
         calendar year
-    month: float
+    month: np.ndarray
         calendar month
-    day: float or NoneType, default None
+    day: np.ndarray, float or NoneType, default None
         day of the month
-    hour: float or NoneType, default None
+    hour: np.ndarray, float or NoneType, default None
         hour of the day
-    minute: float or NoneType, default None
+    minute: np.ndarray, float or NoneType, default None
         minute of the hour
-    second: float or NoneType, default None
+    second: np.ndarray, float or NoneType, default None
         second of the minute
-    DofY: float or NoneType, default None
-        day of the year (January 1 = 1)
+    DofY: np.ndarray, float or NoneType, default None
+        day of the year
 
     Returns
     -------
-    t_date: float
+    t_date: np.ndarray
         date in decimal-year format
 
     References
     ----------
-    .. [1] Dershowitz, N. and E.M. Reingold. 2008.
-        Calendrical Calculations.
-        Cambridge: Cambridge University Press.
+    .. [1] N. Dershowitz, and E. M. Reingold.
+        *Calendrical Calculations*,
+        Cambridge: Cambridge University Press, (2008).
     """
 
     # number of dates
     n_dates = len(np.atleast_1d(year))
 
     # create arrays for calendar date variables
     cal_date = {}
@@ -400,54 +485,54 @@
         (cal_date['DofY'][stnd] + cal_date['hour'][stnd]/24. + \
         cal_date['minute'][stnd]/1440. + \
         cal_date['second'][stnd]/86400.)/np.sum(dpm_stnd)
 
     return t_date
 
 # PURPOSE: Converts from Julian day to calendar date and time
-def convert_julian(JD, **kwargs):
+def convert_julian(JD: np.ndarray, **kwargs):
     """
     Converts from Julian day to calendar date and time
 
     Parameters
     ----------
-    JD: float
+    JD: np.ndarray
         Julian Day (days since 01-01-4713 BCE at 12:00:00)
     astype: str or NoneType, default None
         convert output to variable type
     format: str, default 'dict'
         format of output variables
 
             - ``'dict'``: dictionary with variable keys
             - ``'tuple'``: tuple in most-to-least-significant order
             - ``'zip'``: aggregated variable sets
 
     Returns
     -------
-    year: float
+    year: np.ndarray
         calendar year
-    month: float
+    month: np.ndarray
         calendar month
-    day: float
+    day: np.ndarray
         day of the month
-    hour: float
+    hour: np.ndarray
         hour of the day
-    minute: float
+    minute: np.ndarray
         minute of the hour
-    second: float
+    second: np.ndarray
         second of the minute
 
     References
     ----------
-    .. [1] "Numerical Recipes in C", by William H. Press,
+    .. [1] W. H. Press, *Numerical Recipes in C*,
         Brian P. Flannery, Saul A. Teukolsky, and William T. Vetterling.
-        Cambridge University Press, 1988 (second printing).
-    .. [2] Hatcher, D. A., "Simple Formulae for Julian Day Numbers and
-        Calendar Dates", Quarterly Journal of the Royal Astronomical
-        Society, 25(1), 1984.
+        Cambridge University Press, (1988).
+    .. [2] D. A. Hatcher, "Simple Formulae for Julian Day Numbers and
+        Calendar Dates", *Quarterly Journal of the Royal Astronomical
+        Society*, 25(1), 1984.
     """
     # set default keyword arguments
     kwargs.setdefault('astype', None)
     kwargs.setdefault('format', 'dict')
     # raise warnings for deprecated keyword arguments
     deprecated_keywords = dict(ASTYPE='astype', FORMAT='format')
     for old,new in deprecated_keywords.items():
@@ -512,21 +597,24 @@
             hour=hour, minute=minute, second=second)
     elif (kwargs['format'] == 'tuple'):
         return (year, month, day, hour, minute, second)
     elif (kwargs['format'] == 'zip'):
         return zip(year, month, day, hour, minute, second)
 
 # PURPOSE: Count number of leap seconds that have passed for each GPS time
-def count_leap_seconds(GPS_Time, truncate=True):
+def count_leap_seconds(
+        GPS_Time: np.ndarray | float,
+        truncate: bool = True
+    ):
     """
     Counts the number of leap seconds between a given GPS time and UTC
 
     Parameters
     ----------
-    GPS_Time: float
+    GPS_Time: np.ndarray or float
         seconds since January 6, 1980 at 00:00:00
     truncate: bool, default True
         Reduce list of leap seconds to positive GPS times
 
     Returns
     -------
     n_leaps: float
@@ -541,66 +629,70 @@
         if (count > 0):
             indices = np.nonzero(GPS_Time >= leap)
             n_leaps[indices] += 1.0
     # return the number of leap seconds for converting to UTC
     return n_leaps
 
 # PURPOSE: Define GPS leap seconds
-def get_leap_seconds(truncate=True):
+def get_leap_seconds(truncate: bool = True):
     """
     Gets a list of GPS times for when leap seconds occurred
 
     Parameters
     ----------
     truncate: bool, default True
         Reduce list of leap seconds to positive GPS times
 
     Returns
     -------
     GPS time: float
         GPS seconds when leap seconds occurred
     """
-    FILE = icesat2_toolkit.utilities.get_data_path(['data','leap-seconds.list'])
+    leap_secs = icesat2_toolkit.utilities.get_data_path(['data','leap-seconds.list'])
     # find line with file expiration as delta time
-    with open(FILE,'r') as fid:
+    with leap_secs.open(mode='r', encoding='utf8') as fid:
         secs, = [re.findall(r'\d+',i).pop() for i in fid.read().splitlines()
             if re.match(r'^(?=#@)',i)]
     # check that leap seconds file is still valid
-    expiry = datetime.datetime(1900,1,1) + datetime.timedelta(seconds=int(secs))
-    today = datetime.datetime.now()
+    expiry = datetime.datetime(*_ntp_epoch) + datetime.timedelta(seconds=int(secs))
+    today = datetime.datetime.utcnow()
     update_leap_seconds() if (expiry < today) else None
     # get leap seconds
-    leap_UTC,TAI_UTC = np.loadtxt(icesat2_toolkit.utilities.get_data_path(FILE)).T
+    leap_UTC,TAI_UTC = np.loadtxt(leap_secs).T
     # TAI time is ahead of GPS by 19 seconds
     TAI_GPS = 19.0
     # convert leap second epochs from NTP to GPS
     # convert from time of 2nd leap second to time of 1st leap second
-    leap_GPS = convert_delta_time(leap_UTC+TAI_UTC-TAI_GPS-1,
-        epoch1=(1900,1,1,0,0,0), epoch2=(1980,1,6,0,0,0))
+    leap_GPS = convert_delta_time(leap_UTC + TAI_UTC - TAI_GPS - 1,
+        epoch1=_ntp_epoch, epoch2=_gps_epoch)
     # return the GPS times of leap second occurance
     if truncate:
         return leap_GPS[leap_GPS >= 0].astype(np.float64)
     else:
         return leap_GPS.astype(np.float64)
 
 # PURPOSE: connects to servers and downloads leap second files
-def update_leap_seconds(timeout=20, verbose=False, mode=0o775):
+def update_leap_seconds(
+        timeout: int | None = 20,
+        verbose: bool = False,
+        mode: oct = 0o775
+    ):
     """
     Connects to servers to download leap-seconds.list files from NIST servers
 
     - https://www.nist.gov/pml/time-and-frequency-division/leap-seconds-faqs
 
     Servers and Mirrors
 
     - ftp://ftp.nist.gov/pub/time/leap-seconds.list
     - https://www.ietf.org/timezones/data/leap-seconds.list
 
     Parameters
     ----------
-    timeout: int, default 20
+    timeout: int or None, default 20
         timeout in seconds for blocking operations
     verbose: bool, default False
         print file information about output file
     mode: oct, default 0o775
         permissions mode of output file
     """
     # local version of file
@@ -610,26 +702,27 @@
 
     # try downloading from NIST ftp servers
     HOST = ['ftp.nist.gov','pub','time',FILE]
     try:
         icesat2_toolkit.utilities.check_ftp_connection(HOST[0])
         icesat2_toolkit.utilities.from_ftp(HOST, timeout=timeout, local=LOCAL,
             hash=HASH, verbose=verbose, mode=mode)
-    except Exception as e:
+    except Exception as exc:
         logging.debug(traceback.format_exc())
         pass
     else:
         return
 
     # try downloading from Internet Engineering Task Force (IETF) mirror
     REMOTE = ['https://www.ietf.org','timezones','data',FILE]
     try:
         icesat2_toolkit.utilities.from_http(REMOTE, timeout=timeout, local=LOCAL,
             hash=HASH, verbose=verbose, mode=mode)
-    except Exception as e:
+    except Exception as exc:
         logging.debug(traceback.format_exc())
         pass
     else:
         return
 
     # return exception that no server could be connected
     raise Exception('All Server Connection Error')
+
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/tools.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,25 @@
     Updated 12/2021: added custom colormap function for some common scales
     Written 09/2021
 """
 import os
 import re
 import copy
 import colorsys
+import warnings
 import numpy as np
-import matplotlib.cm as cm
-import matplotlib.colors as colors
+# attempt imports
+try:
+    import matplotlib.cm as cm
+    import matplotlib.colors as colors
+except (ImportError, ModuleNotFoundError) as exc:
+    warnings.filterwarnings("module")
+    warnings.warn("matplotlib not available", ImportWarning)
+# ignore warnings
+warnings.filterwarnings("ignore")
 
 def from_cpt(filename, use_extremes=True, **kwargs):
     """
     Reads GMT color palette table files and registers the
     colormap to be recognizable by ``plt.cm.get_cmap()``
 
     Can import HSV (hue-saturation-value) or RGB values
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit/utilities.py` & `icesat2-toolkit-1.3.0/icesat2_toolkit/utilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 #!/usr/bin/env python
 u"""
 utilities.py
-Written by Tyler Sutterley (12/2022)
+Written by Tyler Sutterley (07/2023)
 Download and management utilities for syncing time and auxiliary files
 
 PYTHON DEPENDENCIES:
     lxml: processing XML and HTML in Python
         https://pypi.python.org/pypi/lxml
 
 UPDATE HISTORY:
+    Updated 07/2023: add function for S3 filesystem
+        add s3 and opendap endpoint options to cmr query functions
+    Updated 06/2023: add functions to retrieve and revoke Earthdata tokens
+    Updated 05/2023: using pathlib to define and expand paths
+    Updated 03/2023: add basic variable typing to function inputs
+    Updated 01/2023: updated SSL context to fix some deprecation warnings
     Updated 12/2022: add variables for NASA DAAC and s3 providers
         add functions for managing and maintaining git repositories
     Updated 08/2022: added s3 presigned url functions
     Updated 07/2022: renamed cmr functions, added s3 client function
     Updated 06/2022: add NASA CMR spatial bounding box queries
     Updated 04/2022: updated docstrings to numpy documentation format
     Updated 03/2022: added NASA CMR query parameters for ATL14/15
@@ -33,140 +39,164 @@
         normalize source and destination paths in copy
     Updated 09/2020: copy from http and https to bytesIO object in chunks
         use netrc credentials if not entered from NSIDC functions
         generalize build opener function for different Earthdata instances
     Updated 08/2020: add Earthdata opener, login and download functions
     Written 08/2020
 """
-from __future__ import print_function, division
+from __future__ import print_function, division, annotations
 
 import sys
 import os
 import re
 import io
 import ssl
 import json
-import boto3
 import netrc
 import ftplib
 import shutil
 import base64
 import socket
 import getpass
 import inspect
 import hashlib
 import logging
+import pathlib
 import builtins
 import datetime
 import dateutil
 import warnings
 import posixpath
 import lxml.etree
 import subprocess
-import calendar,time
+import calendar, time
 if sys.version_info[0] == 2:
     from cookielib import CookieJar
     from urllib import urlencode
     import urllib2
 else:
     from http.cookiejar import CookieJar
     from urllib.parse import urlencode
     import urllib.request as urllib2
 
+# attempt imports
+try:
+    import boto3
+except (ImportError, ModuleNotFoundError) as exc:
+    warnings.filterwarnings("module")
+    warnings.warn("boto3 not available", ImportWarning)
+try:
+    import s3fs
+except (ImportError, ModuleNotFoundError) as exc:
+    warnings.filterwarnings("module")
+    warnings.warn("s3fs not available", ImportWarning)
+# ignore warnings
+warnings.filterwarnings("ignore")
+
 # PURPOSE: get absolute path within a package from a relative path
-def get_data_path(relpath):
+def get_data_path(relpath: list | str | pathlib.Path):
     """
     Get the absolute path within a package from a relative path
 
     Parameters
     ----------
-    relpath: str,
+    relpath: list, str or pathlib.Path
         relative path
     """
     # current file path
     filename = inspect.getframeinfo(inspect.currentframe()).filename
-    filepath = os.path.dirname(os.path.abspath(filename))
-    if isinstance(relpath,list):
+    filepath = pathlib.Path(filename).absolute().parent
+    if isinstance(relpath, list):
         # use *splat operator to extract from list
-        return os.path.join(filepath,*relpath)
-    elif isinstance(relpath,str):
-        return os.path.join(filepath,relpath)
+        return filepath.joinpath(*relpath)
+    elif isinstance(relpath, (str, pathlib.Path)):
+        return filepath.joinpath(relpath)
 
 # PURPOSE: get the hash value of a file
-def get_hash(local, algorithm='MD5'):
+def get_hash(
+        local: str | io.IOBase | pathlib.Path,
+        algorithm: str = 'MD5'
+    ):
     """
-    Get the hash value from a local file or BytesIO object
+    Get the hash value from a local file or ``BytesIO`` object
 
     Parameters
     ----------
-    local: obj or str
+    local: obj, str or pathlib.Path
         BytesIO object or path to file
     algorithm: str, default 'MD5'
         hashing algorithm for checksum validation
 
             - ``'MD5'``: Message Digest
             - ``'sha1'``: Secure Hash Algorithm
     """
     # check if open file object or if local file exists
     if isinstance(local, io.IOBase):
         if (algorithm == 'MD5'):
             return hashlib.md5(local.getvalue()).hexdigest()
         elif (algorithm == 'sha1'):
             return hashlib.sha1(local.getvalue()).hexdigest()
-    elif os.access(os.path.expanduser(local),os.F_OK):
+    elif isinstance(local, (str, pathlib.Path)):
         # generate checksum hash for local file
+        local = pathlib.Path(local).expanduser()
+        # if file currently doesn't exist, return empty string
+        if not local.exists():
+            return ''
         # open the local_file in binary read mode
-        with open(os.path.expanduser(local), 'rb') as local_buffer:
+        with local.open(mode='rb') as local_buffer:
             # generate checksum hash for a given type
             if (algorithm == 'MD5'):
                 return hashlib.md5(local_buffer.read()).hexdigest()
             elif (algorithm == 'sha1'):
                 return hashlib.sha1(local_buffer.read()).hexdigest()
     else:
         return ''
 
 # PURPOSE: get the git hash value
-def get_git_revision_hash(refname='HEAD', short=False):
+def get_git_revision_hash(
+        refname: str = 'HEAD',
+        short: bool = False
+    ):
     """
-    Get the git hash value for a particular reference
+    Get the ``git`` hash value for a particular reference
 
     Parameters
     ----------
     refname: str, default HEAD
         Symbolic reference name
     short: bool, default False
         Return the shorted hash value
     """
     # get path to .git directory from current file path
     filename = inspect.getframeinfo(inspect.currentframe()).filename
-    basepath = os.path.dirname(os.path.dirname(os.path.abspath(filename)))
-    gitpath = os.path.join(basepath,'.git')
+    basepath = pathlib.Path(filename).absolute().parent.parent
+    gitpath = basepath.joinpath('.git')
     # build command
     cmd = ['git', f'--git-dir={gitpath}', 'rev-parse']
     cmd.append('--short') if short else None
     cmd.append(refname)
     # get output
     with warnings.catch_warnings():
         return str(subprocess.check_output(cmd), encoding='utf8').strip()
 
 # PURPOSE: get the current git status
 def get_git_status():
-    """Get the status of a git repository as a boolean value
+    """Get the status of a ``git`` repository as a boolean value
     """
     # get path to .git directory from current file path
     filename = inspect.getframeinfo(inspect.currentframe()).filename
-    basepath = os.path.dirname(os.path.dirname(os.path.abspath(filename)))
-    gitpath = os.path.join(basepath,'.git')
+    basepath = pathlib.Path(filename).absolute().parent.parent
+    gitpath = basepath.joinpath('.git')
     # build command
     cmd = ['git', f'--git-dir={gitpath}', 'status', '--porcelain']
     with warnings.catch_warnings():
         return bool(subprocess.check_output(cmd))
 
 # PURPOSE: recursively split a url path
-def url_split(s):
+def url_split(s: str):
     """
     Recursively split a url path into a list
 
     Parameters
     ----------
     s: str
         url string
@@ -174,14 +204,130 @@
     head, tail = posixpath.split(s)
     if head in ('http:','https:','ftp:','s3:'):
         return s,
     elif head in ('', posixpath.sep):
         return tail,
     return url_split(head) + (tail,)
 
+# PURPOSE: convert file lines to arguments
+def convert_arg_line_to_args(arg_line):
+    """
+    Convert file lines to arguments
+
+    Parameters
+    ----------
+    arg_line: str
+        line string containing a single argument and/or comments
+    """
+    # remove commented lines and after argument comments
+    for arg in re.sub(r'\#(.*?)$',r'',arg_line).split():
+        if not arg.strip():
+            continue
+        yield arg
+
+# PURPOSE: returns the Unix timestamp value for a formatted date string
+def get_unix_time(
+        time_string: str,
+        format: str = '%Y-%m-%d %H:%M:%S'
+    ):
+    """
+    Get the Unix timestamp value for a formatted date string
+
+    Parameters
+    ----------
+    time_string: str
+        formatted time string to parse
+    format: str, default '%Y-%m-%d %H:%M:%S'
+        format for input time string
+    """
+    try:
+        parsed_time = time.strptime(time_string.rstrip(), format)
+    except (TypeError, ValueError):
+        pass
+    else:
+        return calendar.timegm(parsed_time)
+    # try parsing with dateutil
+    try:
+        parsed_time = dateutil.parser.parse(time_string.rstrip())
+    except (TypeError, ValueError):
+        return None
+    else:
+        return parsed_time.timestamp()
+
+# PURPOSE: output a time string in isoformat
+def isoformat(time_string: str):
+    """
+    Reformat a date string to ISO formatting
+
+    Parameters
+    ----------
+    time_string: str
+        formatted time string to parse
+    """
+    # try parsing with dateutil
+    try:
+        parsed_time = dateutil.parser.parse(time_string.rstrip())
+    except (TypeError, ValueError):
+        return None
+    else:
+        return parsed_time.isoformat()
+
+# PURPOSE: rounds a number to an even number less than or equal to original
+def even(value: float):
+    """
+    Rounds a number to an even number less than or equal to original
+
+    Parameters
+    ----------
+    value: float
+        number to be rounded
+    """
+    return 2*int(value//2)
+
+# PURPOSE: rounds a number upward to its nearest integer
+def ceil(value: float):
+    """
+    Rounds a number upward to its nearest integer
+
+    Parameters
+    ----------
+    value: float
+        number to be rounded upward
+    """
+    return -int(-value//1)
+
+# PURPOSE: make a copy of a file with all system information
+def copy(
+        source: str,
+        destination: str,
+        move: bool = False,
+        **kwargs
+    ):
+    """
+    Copy or move a file with all system information
+
+    Parameters
+    ----------
+    source: str
+        source file
+    destination: str
+        copied destination file
+    move: bool, default False
+        remove the source file
+    """
+    source = pathlib.Path(source).expanduser().absolute()
+    destination = pathlib.Path(destination).expanduser().absolute()
+    # log source and destination
+    logging.info(f'{str(source)} -->\n\t{str(destination)}')
+    shutil.copyfile(source, destination)
+    shutil.copystat(source, destination)
+    # remove the original file if moving
+    if move:
+        source.unlink()
+
 # NASA on-prem DAAC providers
 _daac_providers = {
     'gesdisc': 'GES_DISC',
     'ghrcdaac': 'GHRC_DAAC',
     'lpdaac': 'LPDAAC_ECS',
     'nsidc': 'NSIDC_ECS',
     'ornldaac': 'ORNL_DAAC',
@@ -215,16 +361,19 @@
     'lpdaac': 'lp-prod-protected',
     'nsidc': 'nsidc-cumulus-prod-protected',
     'ornldaac': 'ornl-cumulus-prod-protected',
     'podaac': 'podaac-ops-cumulus-protected'
 }
 
 # PURPOSE: get AWS s3 client for NSIDC Cumulus
-def s3_client(HOST=_s3_endpoints['nsidc'], timeout=None,
-    region_name='us-west-2'):
+def s3_client(
+        HOST: str = _s3_endpoints['nsidc'],
+        timeout: int | None = None,
+        region_name: str = 'us-west-2'
+    ):
     """
     Get AWS s3 client for NSIDC data in the cloud
     https://data.nsidc.earthdatacloud.nasa.gov/s3credentials
 
     Parameters
     ----------
     HOST: str
@@ -247,16 +396,55 @@
         aws_access_key_id=cumulus['accessKeyId'],
         aws_secret_access_key=cumulus['secretAccessKey'],
         aws_session_token=cumulus['sessionToken'],
         region_name=region_name)
     # return the AWS client for region
     return client
 
+# PURPOSE: get AWS s3 file system for NSIDC Cumulus
+def s3_filesystem(
+        HOST: str = _s3_endpoints['nsidc'],
+        timeout: int | None = None,
+        region_name: str = 'us-west-2'
+    ):
+    """
+    Get AWS s3 file system object for NSIDC data in the cloud
+    https://data.nsidc.earthdatacloud.nasa.gov/s3credentials
+
+    Parameters
+    ----------
+    HOST: str
+        NSIDC AWS S3 credential host
+    timeout: int or NoneType, default None
+        timeout in seconds for blocking operations
+    region_name: str, default 'us-west-2'
+        AWS region name
+
+    Returns
+    -------
+    session: obj
+        AWS s3 file system session for NSIDC Cumulus
+    """
+    request = urllib2.Request(HOST)
+    response = urllib2.urlopen(request, timeout=timeout)
+    cumulus = json.loads(response.read())
+    # get AWS file system session object
+    session = s3fs.S3FileSystem(anon=False,
+        key=cumulus['accessKeyId'],
+        secret=cumulus['secretAccessKey'],
+        token=cumulus['sessionToken'],
+        client_kwargs=dict(
+            region_name=region_name
+        )
+    )
+    # return the AWS session for region
+    return session
+
 # PURPOSE: get a s3 bucket name from a presigned url
-def s3_bucket(presigned_url):
+def s3_bucket(presigned_url: str):
     """
     Get a s3 bucket name from a presigned url
 
     Parameters
     ----------
     presigned_url: str
         s3 presigned url
@@ -267,15 +455,15 @@
         s3 bucket name
     """
     host = url_split(presigned_url)
     bucket = re.sub(r's3:\/\/', r'', host[0], re.IGNORECASE)
     return bucket
 
 # PURPOSE: get a s3 bucket key from a presigned url
-def s3_key(presigned_url):
+def s3_key(presigned_url: str):
     """
     Get a s3 bucket key from a presigned url
 
     Parameters
     ----------
     presigned_url: str
         s3 presigned url or https url
@@ -295,15 +483,18 @@
     else:
         # join presigned url to form bucket key
         key = posixpath.join(*host[1:])
     # return the s3 bucket key for object
     return key
 
 # PURPOSE: get a s3 presigned url from a bucket and key
-def s3_presigned_url(bucket, key):
+def s3_presigned_url(
+        bucket: str,
+        key: str
+    ):
     """
     Get a s3 presigned url from a bucket and object key
 
     Parameters
     ----------
     bucket: str
         s3 bucket name
@@ -314,151 +505,54 @@
     -------
     presigned_url: str
         s3 presigned url
     """
     return posixpath.join('s3://', bucket, key)
 
 # PURPOSE: generate a s3 presigned https url from a bucket and key
-def generate_presigned_url(bucket, key, expiration=3600):
+def generate_presigned_url(
+        bucket: str,
+        key: str,
+        expiration: int = 3600
+    ):
     """
     Generate a presigned https URL to share an S3 object
 
     Parameters
     ----------
     bucket: str
         s3 bucket name
     key: str
         s3 bucket key for object
+    expiration: int
+        Time in seconds for the presigned URL to remain valid
 
     Returns
     -------
     presigned_url: str
         s3 presigned https url
     """
     # generate a presigned URL for S3 object
     s3 = boto3.client('s3')
     try:
         response = s3.generate_presigned_url('get_object',
             Params={'Bucket': bucket, 'Key': key},
             ExpiresIn=expiration)
-    except Exception as e:
-        logging.error(e)
+    except Exception as exc:
+        logging.error(exc)
         return None
     # The response contains the presigned URL
     return response
 
-# PURPOSE: convert file lines to arguments
-def convert_arg_line_to_args(arg_line):
-    """
-    Convert file lines to arguments
-
-    Parameters
-    ----------
-    arg_line: str
-        line string containing a single argument and/or comments
-    """
-    # remove commented lines and after argument comments
-    for arg in re.sub(r'\#(.*?)$',r'',arg_line).split():
-        if not arg.strip():
-            continue
-        yield arg
-
-# PURPOSE: returns the Unix timestamp value for a formatted date string
-def get_unix_time(time_string, format='%Y-%m-%d %H:%M:%S'):
-    """
-    Get the Unix timestamp value for a formatted date string
-
-    Parameters
-    ----------
-    time_string: str
-        formatted time string to parse
-    format: str, default '%Y-%m-%d %H:%M:%S'
-        format for input time string
-    """
-    try:
-        parsed_time = time.strptime(time_string.rstrip(), format)
-    except (TypeError, ValueError):
-        pass
-    else:
-        return calendar.timegm(parsed_time)
-    # try parsing with dateutil
-    try:
-        parsed_time = dateutil.parser.parse(time_string.rstrip())
-    except (TypeError, ValueError):
-        return None
-    else:
-        return parsed_time.timestamp()
-
-# PURPOSE: output a time string in isoformat
-def isoformat(time_string):
-    """
-    Reformat a date string to ISO formatting
-
-    Parameters
-    ----------
-    time_string: str
-        formatted time string to parse
-    """
-    # try parsing with dateutil
-    try:
-        parsed_time = dateutil.parser.parse(time_string.rstrip())
-    except (TypeError, ValueError):
-        return None
-    else:
-        return parsed_time.isoformat()
-
-# PURPOSE: rounds a number to an even number less than or equal to original
-def even(value):
-    """
-    Rounds a number to an even number less than or equal to original
-
-    Parameters
-    ----------
-    value: float
-        number to be rounded
-    """
-    return 2*int(value//2)
-
-# PURPOSE: rounds a number upward to its nearest integer
-def ceil(value):
-    """
-    Rounds a number upward to its nearest integer
-
-    Parameters
-    ----------
-    value: float
-        number to be rounded upward
-    """
-    return -int(-value//1)
-
-# PURPOSE: make a copy of a file with all system information
-def copy(source, destination, move=False, **kwargs):
-    """
-    Copy or move a file with all system information
-
-    Parameters
-    ----------
-    source: str
-        source file
-    destination: str
-        copied destination file
-    move: bool, default False
-        remove the source file
-    """
-    source = os.path.abspath(os.path.expanduser(source))
-    destination = os.path.abspath(os.path.expanduser(destination))
-    # log source and destination
-    logging.info(f'{source} -->\n\t{destination}')
-    shutil.copyfile(source, destination)
-    shutil.copystat(source, destination)
-    if move:
-        os.remove(source)
-
 # PURPOSE: check ftp connection
-def check_ftp_connection(HOST, username=None, password=None):
+def check_ftp_connection(
+        HOST: str,
+        username: str | None = None,
+        password: str | None = None
+    ):
     """
     Check internet connection with ftp host
 
     Parameters
     ----------
     HOST: str
         remote ftp host
@@ -476,16 +570,23 @@
         raise RuntimeError('Check internet connection')
     except ftplib.error_perm:
         raise RuntimeError('Check login credentials')
     else:
         return True
 
 # PURPOSE: list a directory on a ftp host
-def ftp_list(HOST, username=None, password=None, timeout=None,
-    basename=False, pattern=None, sort=False):
+def ftp_list(
+        HOST: str | list,
+        username: str | None = None,
+        password: str | None = None,
+        timeout: int | None = None,
+        basename: bool = False,
+        pattern: str | None = None,
+        sort: bool = False
+    ):
     """
     List a directory on a ftp host
 
     Parameters
     ----------
     HOST: str or list
         remote ftp host path split as list
@@ -548,34 +649,43 @@
             i = [i for i,j in sorted(enumerate(output), key=lambda i: i[1])]
             # sort list of listed items and last modified times
             output = [output[indice] for indice in i]
             mtimes = [mtimes[indice] for indice in i]
         # close the ftp connection
         ftp.close()
         # return the list of items and last modified times
-        return (output,mtimes)
+        return (output, mtimes)
 
 # PURPOSE: download a file from a ftp host
-def from_ftp(HOST, username=None, password=None, timeout=None,
-    local=None, hash='', chunk=8192, verbose=False, fid=sys.stdout,
-    mode=0o775):
+def from_ftp(
+        HOST: str | list,
+        username: str | None = None,
+        password: str | None = None,
+        timeout: int | None = None,
+        local: str | pathlib.Path | None = None,
+        hash: str = '',
+        chunk: int = 8192,
+        verbose: bool = False,
+        fid=sys.stdout,
+        mode: oct = 0o775
+    ):
     """
     Download a file from a ftp host
 
     Parameters
     ----------
     HOST: str or list
         remote ftp host path
     username: str or NoneType
         ftp username
     password: str or NoneType
         ftp password
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
-    local: str or NoneType, default None
+    local: str, pathlib.Path or NoneType, default None
         path to local file
     hash: str, default ''
         MD5 hash of local file
     chunk: int, default 8192
         chunk size for transfer encoding
     verbose: bool, default False
         print file transfer information
@@ -594,15 +704,15 @@
     logging.basicConfig(stream=fid, level=loglevel)
     # verify inputs for remote ftp host
     if isinstance(HOST, str):
         HOST = url_split(HOST)
     # try downloading from ftp
     try:
         # try to connect to ftp host
-        ftp = ftplib.FTP(HOST[0],timeout=timeout)
+        ftp = ftplib.FTP(HOST[0], timeout=timeout)
     except (socket.gaierror,IOError):
         raise RuntimeError(f'Unable to connect to {HOST[0]}')
     else:
         ftp.login(username,password)
         # remote path
         ftp_remote_path = posixpath.join(*HOST[1:])
         # copy remote file contents to bytesIO object
@@ -616,70 +726,80 @@
         remote_hash = hashlib.md5(remote_buffer.getvalue()).hexdigest()
         # get last modified date of remote file and convert into unix time
         mdtm = ftp.sendcmd(f'MDTM {ftp_remote_path}')
         remote_mtime = get_unix_time(mdtm[4:], format="%Y%m%d%H%M%S")
         # compare checksums
         if local and (hash != remote_hash):
             # convert to absolute path
-            local = os.path.abspath(local)
+            local = pathlib.Path(local).expanduser().absolute()
             # create directory if non-existent
-            if not os.access(os.path.dirname(local), os.F_OK):
-                os.makedirs(os.path.dirname(local), mode)
+            local.parent.mkdir(mode=mode, parents=True, exist_ok=True)
             # print file information
-            args = (posixpath.join(*HOST),local)
+            args = (posixpath.join(*HOST), str(local))
             logging.info('{0} -->\n\t{1}'.format(*args))
             # store bytes to file using chunked transfer encoding
             remote_buffer.seek(0)
-            with open(os.path.expanduser(local), 'wb') as f:
+            with local.open(mode='wb') as f:
                 shutil.copyfileobj(remote_buffer, f, chunk)
             # change the permissions mode
-            os.chmod(local,mode)
+            local.chmod(mode)
             # keep remote modification time of file and local access time
-            os.utime(local, (os.stat(local).st_atime, remote_mtime))
+            os.utime(local, (local.stat().st_atime, remote_mtime))
         # close the ftp connection
         ftp.close()
         # return the bytesIO object
         remote_buffer.seek(0)
         return remote_buffer
 
+# default ssl context
+_default_ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
+
 # PURPOSE: check internet connection
-def check_connection(HOST):
+def check_connection(HOST: str, context=_default_ssl_context):
     """
     Check internet connection with http host
 
     Parameters
     ----------
     HOST: str
         remote http host
+    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+        SSL context for ``urllib`` opener object
     """
     # attempt to connect to http host
     try:
-        urllib2.urlopen(HOST,timeout=20,context=ssl.SSLContext())
-    except urllib2.URLError:
-        raise RuntimeError('Check internet connection')
+        urllib2.urlopen(HOST, timeout=20, context=context)
+    except urllib2.URLError as exc:
+        raise RuntimeError('Check internet connection') from exc
     else:
         return True
 
 # PURPOSE: list a directory on an Apache http Server
-def http_list(HOST, timeout=None, context=ssl.SSLContext(),
-    parser=lxml.etree.HTMLParser(), format='%Y-%m-%d %H:%M',
-    pattern='', sort=False):
+def http_list(
+        HOST: str | list,
+        timeout: int | None = None,
+        context = _default_ssl_context,
+        parser = lxml.etree.HTMLParser(),
+        format: str = '%Y-%m-%d %H:%M',
+        pattern: str = '',
+        sort: bool = False
+    ):
     """
     List a directory on an Apache http Server
 
     Parameters
     ----------
     HOST: str or list
         remote http host path
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
-    context: obj, default ssl.SSLContext()
-        SSL context for url opener object
+    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+        SSL context for ``urllib`` opener object
     parser: obj, default lxml.etree.HTMLParser()
-        HTML parser for lxml
+        HTML parser for ``lxml``
     format: str, default '%Y-%m-%d %H:%M'
         format for input time string
     pattern: str, default ''
         regular expression pattern for reducing list
     sort: bool, default False
         sort output list
 
@@ -694,59 +814,65 @@
     """
     # verify inputs for remote http host
     if isinstance(HOST, str):
         HOST = url_split(HOST)
     # try listing from http
     try:
         # Create and submit request.
-        request=urllib2.Request(posixpath.join(*HOST))
-        response=urllib2.urlopen(request,timeout=timeout,context=context)
-    except (urllib2.HTTPError, urllib2.URLError) as e:
+        request = urllib2.Request(posixpath.join(*HOST))
+        response = urllib2.urlopen(request, timeout=timeout, context=context)
+    except (urllib2.HTTPError, urllib2.URLError) as exc:
         colerror = 'List error from {0}'.format(posixpath.join(*HOST))
-        return (False,False,colerror)
+        return (False, False, colerror)
     else:
         # read and parse request for files (column names and modified times)
-        tree = lxml.etree.parse(response,parser)
+        tree = lxml.etree.parse(response, parser)
         colnames = tree.xpath('//tr/td[not(@*)]//a/@href')
         # get the Unix timestamp value for a modification time
         collastmod = [get_unix_time(i,format=format)
             for i in tree.xpath('//tr/td[@align="right"][1]/text()')]
         # reduce using regular expression pattern
         if pattern:
-            i = [i for i,f in enumerate(colnames) if re.search(pattern,f)]
+            i = [i for i,f in enumerate(colnames) if re.search(pattern, f)]
             # reduce list of column names and last modified times
             colnames = [colnames[indice] for indice in i]
             collastmod = [collastmod[indice] for indice in i]
         # sort the list
         if sort:
             i = [i for i,j in sorted(enumerate(colnames), key=lambda i: i[1])]
             # sort list of column names and last modified times
             colnames = [colnames[indice] for indice in i]
             collastmod = [collastmod[indice] for indice in i]
         # return the list of column names and last modified times
-        return (colnames,collastmod,None)
+        return (colnames, collastmod, None)
 
 # PURPOSE: download a file from a http host
-def from_http(HOST, timeout=None, context=ssl.SSLContext(),
-    local=None, hash='', chunk=16384, verbose=False, fid=sys.stdout,
-    mode=0o775):
+def from_http(
+        HOST: str | list,
+        timeout: int | None = None,
+        context = _default_ssl_context,
+        local: str | pathlib.Path | None = None,
+        hash: str = '',
+        chunk: int = 16384,
+        verbose: bool = False,
+        fid = sys.stdout,
+        mode: oct = 0o775
+    ):
     """
     Download a file from a http host
 
     Parameters
     ----------
     HOST: str or list
         remote http host path split as list
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
-    context: obj, default ssl.SSLContext()
-        SSL context for url opener object
-    timeout: int or NoneType, default None
-        timeout in seconds for blocking operations
-    local: str or NoneType, default None
+    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+        SSL context for ``urllib`` opener object
+    local: str, pathlib.Path or NoneType, default None
         path to local file
     hash: str, default ''
         MD5 hash of local file
     chunk: int, default 16384
         chunk size for transfer encoding
     verbose: bool, default False
         print file transfer information
@@ -766,59 +892,64 @@
     # verify inputs for remote http host
     if isinstance(HOST, str):
         HOST = url_split(HOST)
     # try downloading from http
     try:
         # Create and submit request.
         request = urllib2.Request(posixpath.join(*HOST))
-        response = urllib2.urlopen(request,timeout=timeout,context=context)
-    except (urllib2.HTTPError, urllib2.URLError):
+        response = urllib2.urlopen(request, timeout=timeout, context=context)
+    except (urllib2.HTTPError, urllib2.URLError) as exc:
         raise Exception('Download error from {0}'.format(posixpath.join(*HOST)))
     else:
         # copy remote file contents to bytesIO object
         remote_buffer = io.BytesIO()
         shutil.copyfileobj(response, remote_buffer, chunk)
         remote_buffer.seek(0)
         # save file basename with bytesIO object
         remote_buffer.filename = HOST[-1]
         # generate checksum hash for remote file
         remote_hash = hashlib.md5(remote_buffer.getvalue()).hexdigest()
         # compare checksums
         if local and (hash != remote_hash):
             # convert to absolute path
-            local = os.path.abspath(local)
+            local = pathlib.Path(local).expanduser().absolute()
             # create directory if non-existent
-            if not os.access(os.path.dirname(local), os.F_OK):
-                os.makedirs(os.path.dirname(local), mode)
+            local.parent.mkdir(mode=mode, parents=True, exist_ok=True)
             # print file information
-            args = (posixpath.join(*HOST),local)
+            args = (posixpath.join(*HOST), str(local))
             logging.info('{0} -->\n\t{1}'.format(*args))
             # store bytes to file using chunked transfer encoding
             remote_buffer.seek(0)
-            with open(os.path.expanduser(local), 'wb') as f:
+            with local.open(mode='wb') as f:
                 shutil.copyfileobj(remote_buffer, f, chunk)
             # change the permissions mode
-            os.chmod(local,mode)
+            local.chmod(mode)
         # return the bytesIO object
         remote_buffer.seek(0)
         return remote_buffer
 
 # PURPOSE: attempt to build an opener with netrc
-def attempt_login(urs, context=ssl.SSLContext(),
-    password_manager=True, get_ca_certs=False, redirect=False,
-    authorization_header=False, **kwargs):
+def attempt_login(
+        urs: str,
+        context=_default_ssl_context,
+        password_manager: bool = True,
+        get_ca_certs: bool = False,
+        redirect: bool = False,
+        authorization_header: bool = False,
+        **kwargs
+    ):
     """
     attempt to build a urllib opener for NASA Earthdata
 
     Parameters
     ----------
     urs: str
         Earthdata login URS 3 host
-    context: obj, default ssl.SSLContext()
-        SSL context for url opener object
+    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+        SSL context for ``urllib`` opener object
     password_manager: bool, default True
         Create password manager context using default realm
     get_ca_certs: bool, default False
         Get list of loaded “certification authority” certificates
     redirect: bool, default False
         Create redirect handler object
     authorization_header: bool, default False
@@ -837,21 +968,21 @@
     opener: obj
         OpenerDirector instance
     """
     # set default keyword arguments
     kwargs.setdefault('username', os.environ.get('EARTHDATA_USERNAME'))
     kwargs.setdefault('password', os.environ.get('EARTHDATA_PASSWORD'))
     kwargs.setdefault('retries', 5)
-    kwargs.setdefault('netrc', os.path.expanduser('~/.netrc'))
+    kwargs.setdefault('netrc', pathlib.Path.home().joinpath('.netrc'))
     try:
         # only necessary on jupyterhub
-        os.chmod(kwargs['netrc'], 0o600)
+        kwargs['netrc'].chmod(mode=0o600)
         # try retrieving credentials from netrc
         username, _, password = netrc.netrc(kwargs['netrc']).authenticators(urs)
-    except Exception as e:
+    except Exception as exc:
         # try retrieving credentials from environmental variables
         username, password = (kwargs['username'], kwargs['password'])
         pass
     # if username or password are not available
     if not username:
         username = builtins.input(f'Username for {urs}: ')
     if not password:
@@ -866,44 +997,51 @@
             get_ca_certs=get_ca_certs,
             redirect=redirect,
             authorization_header=authorization_header,
             urs=urs)
         # try logging in by check credentials
         try:
             check_credentials()
-        except Exception as e:
+        except Exception as exc:
             pass
         else:
             return opener
         # reattempt login
         username = builtins.input(f'Username for {urs}: ')
         password = getpass.getpass(prompt=prompt)
     # reached end of available retries
     raise RuntimeError('End of Retries: Check NASA Earthdata credentials')
 
 # PURPOSE: "login" to NASA Earthdata with supplied credentials
-def build_opener(username, password, context=ssl.SSLContext(),
-    password_manager=True, get_ca_certs=False, redirect=False,
-    authorization_header=False, urs='https://urs.earthdata.nasa.gov'):
+def build_opener(
+        username: str,
+        password: str,
+        context=_default_ssl_context,
+        password_manager: bool = True,
+        get_ca_certs: bool = False,
+        redirect: bool = False,
+        authorization_header: bool = False,
+        urs: str = 'https://urs.earthdata.nasa.gov'
+    ):
     """
-    build urllib opener for NASA Earthdata with supplied credentials
+    Build ``urllib`` opener for NASA Earthdata with supplied credentials
 
     Parameters
     ----------
     username: str or NoneType, default None
         NASA Earthdata username
     password: str or NoneType, default None
         NASA Earthdata password
-    context: obj, default ssl.SSLContext()
-        SSL context for url opener object
+    context: obj, default ssl.SSLContext(ssl.PROTOCOL_TLS)
+        SSL context for ``urllib`` opener object
     password_manager: bool, default True
         Create password manager context using default realm
-    get_ca_certs: bool, default False
+    get_ca_certs: bool, default True
         Get list of loaded “certification authority” certificates
-    redirect: bool, default False
+    redirect: bool, default True
         Create redirect handler object
     authorization_header: bool, default False
         Add base64 encoded authorization header to opener
     urs: str, default 'https://urs.earthdata.nasa.gov'
         Earthdata login URS 3 host
 
     Returns
@@ -913,15 +1051,15 @@
     """
     # https://docs.python.org/3/howto/urllib2.html#id5
     handler = []
     # create a password manager
     if password_manager:
         password_mgr = urllib2.HTTPPasswordMgrWithDefaultRealm()
         # Add the username and password for NASA Earthdata Login system
-        password_mgr.add_password(None,urs,username,password)
+        password_mgr.add_password(None, urs, username, password)
         handler.append(urllib2.HTTPBasicAuthHandler(password_mgr))
     # Create cookie jar for storing cookies. This is used to store and return
     # the session cookie given to use by the data server (otherwise will just
     # keep sending us back to Earthdata Login to authenticate).
     cookie_jar = CookieJar()
     handler.append(urllib2.HTTPCookieProcessor(cookie_jar))
     # SSL context handler
@@ -933,42 +1071,203 @@
         handler.append(urllib2.HTTPRedirectHandler())
     # create "opener" (OpenerDirector instance)
     opener = urllib2.build_opener(*handler)
     # Encode username/password for request authorization headers
     # add Authorization header to opener
     if authorization_header:
         b64 = base64.b64encode(f'{username}:{password}'.encode())
-        opener.addheaders = [("Authorization","Basic {0}".format(b64.decode()))]
+        opener.addheaders = [("Authorization", f"Basic {b64.decode()}")]
     # Now all calls to urllib2.urlopen use our opener.
     urllib2.install_opener(opener)
     # All calls to urllib2.urlopen will now use handler
     # Make sure not to include the protocol in with the URL, or
     # HTTPPasswordMgrWithDefaultRealm will be confused.
     return opener
 
+# PURPOSE: generate a NASA Earthdata user token
+def get_token(
+        HOST: str = 'https://urs.earthdata.nasa.gov/api/users/token',
+        username: str | None = None,
+        password: str | None = None,
+        build: bool = True,
+        urs: str = 'urs.earthdata.nasa.gov',
+    ):
+    """
+    Generate a NASA Earthdata User Token
+
+    Parameters
+    ----------
+    HOST: str or list
+        NASA Earthdata token API host
+    username: str or NoneType, default None
+        NASA Earthdata username
+    password: str or NoneType, default None
+        NASA Earthdata password
+    build: bool, default True
+        Build opener and check WebDAV credentials
+    timeout: int or NoneType, default None
+        timeout in seconds for blocking operations
+    urs: str, default 'urs.earthdata.nasa.gov'
+        NASA Earthdata URS 3 host
+
+    Returns
+    -------
+    token: dict
+        JSON response with NASA Earthdata User Token
+    """
+    # attempt to build urllib2 opener and check credentials
+    if build:
+        attempt_login(urs,
+            username=username,
+            password=password,
+            password_manager=False,
+            authorization_header=True)
+    # create post response with Earthdata token API
+    try:
+        request = urllib2.Request(HOST, method='POST')
+        response = urllib2.urlopen(request)
+    except urllib2.HTTPError as exc:
+        logging.debug(exc.code)
+        raise RuntimeError(exc.reason) from exc
+    except urllib2.URLError as exc:
+        logging.debug(exc.reason)
+        raise RuntimeError('Check internet connection') from exc
+    # read and return JSON response
+    return json.loads(response.read())
+
+# PURPOSE: generate a NASA Earthdata user token
+def list_tokens(
+        HOST: str = 'https://urs.earthdata.nasa.gov/api/users/tokens',
+        username: str | None = None,
+        password: str | None = None,
+        build: bool = True,
+        urs: str = 'urs.earthdata.nasa.gov',
+    ):
+    """
+    List the current associated NASA Earthdata User Tokens
+
+    Parameters
+    ----------
+    HOST: str
+        NASA Earthdata list token API host
+    username: str or NoneType, default None
+        NASA Earthdata username
+    password: str or NoneType, default None
+        NASA Earthdata password
+    build: bool, default True
+        Build opener and check WebDAV credentials
+    timeout: int or NoneType, default None
+        timeout in seconds for blocking operations
+    urs: str, default 'urs.earthdata.nasa.gov'
+        NASA Earthdata URS 3 host
+
+    Returns
+    -------
+    tokens: list
+        JSON response with NASA Earthdata User Tokens
+    """
+    # attempt to build urllib2 opener and check credentials
+    if build:
+        attempt_login(urs,
+            username=username,
+            password=password,
+            password_manager=False,
+            authorization_header=True)
+    # create get response with Earthdata list tokens API
+    try:
+        request = urllib2.Request(HOST)
+        response = urllib2.urlopen(request)
+    except urllib2.HTTPError as exc:
+        logging.debug(exc.code)
+        raise RuntimeError(exc.reason) from exc
+    except urllib2.URLError as exc:
+        logging.debug(exc.reason)
+        raise RuntimeError('Check internet connection') from exc
+    # read and return JSON response
+    return json.loads(response.read())
+
+# PURPOSE: revoke a NASA Earthdata user token
+def revoke_token(
+        token: str,
+        HOST: str = f'https://urs.earthdata.nasa.gov/api/users/revoke_token',
+        username: str | None = None,
+        password: str | None = None,
+        build: bool = True,
+        urs: str = 'urs.earthdata.nasa.gov',
+    ):
+    """
+    Generate a NASA Earthdata User Token
+
+    Parameters
+    ----------
+    token: str
+        NASA Earthdata token to be revoked
+    HOST: str
+        NASA Earthdata revoke token API host
+    username: str or NoneType, default None
+        NASA Earthdata username
+    password: str or NoneType, default None
+        NASA Earthdata password
+    build: bool, default True
+        Build opener and check WebDAV credentials
+    timeout: int or NoneType, default None
+        timeout in seconds for blocking operations
+    urs: str, default 'urs.earthdata.nasa.gov'
+        NASA Earthdata URS 3 host
+    """
+    # attempt to build urllib2 opener and check credentials
+    if build:
+        attempt_login(urs,
+            username=username,
+            password=password,
+            password_manager=False,
+            authorization_header=True)
+    # full path for NASA Earthdata revoke token API
+    url = f'{HOST}?token={token}'
+    # create post response with Earthdata revoke tokens API
+    try:
+        request = urllib2.Request(url, method='POST')
+        response = urllib2.urlopen(request)
+    except urllib2.HTTPError as exc:
+        logging.debug(exc.code)
+        raise RuntimeError(exc.reason) from exc
+    except urllib2.URLError as exc:
+        logging.debug(exc.reason)
+        raise RuntimeError('Check internet connection') from exc
+    # verbose response
+    logging.debug(f'Token Revoked: {token}')
+
 # PURPOSE: check that entered NASA Earthdata credentials are valid
 def check_credentials():
     """
     Check that entered NASA Earthdata credentials are valid
     """
     try:
         remote_path = posixpath.join('https://n5eil01u.ecs.nsidc.org','ATLAS')
         request = urllib2.Request(url=remote_path)
         response = urllib2.urlopen(request, timeout=20)
-    except urllib2.HTTPError:
-        raise RuntimeError('Check your NASA Earthdata credentials')
-    except urllib2.URLError:
-        raise RuntimeError('Check internet connection')
+    except urllib2.HTTPError as exc:
+        raise RuntimeError('Check your NASA Earthdata credentials') from exc
+    except urllib2.URLError as exc:
+        raise RuntimeError('Check internet connection') from exc
     else:
         return True
 
 # PURPOSE: list a directory on NSIDC https server
-def nsidc_list(HOST, username=None, password=None, build=True,
-    timeout=None, urs='urs.earthdata.nasa.gov',
-    parser=lxml.etree.HTMLParser(), pattern='', sort=False):
+def nsidc_list(
+        HOST: str | list,
+        username: str | None = None,
+        password: str | None = None,
+        build: bool = True,
+        timeout: int | None = None,
+        urs: str = 'urs.earthdata.nasa.gov',
+        parser=lxml.etree.HTMLParser(),
+        pattern: str = '',
+        sort: bool = False
+    ):
     """
     List a directory on NSIDC
 
     Parameters
     ----------
     HOST: str or list
         remote https host
@@ -979,15 +1278,15 @@
     build: bool, default True
         Build opener and check WebDAV credentials
     timeout: int or NoneType, default None
         timeout in seconds for blocking operations
     urs: str, default 'urs.earthdata.nasa.gov'
         NASA Earthdata URS 3 host
     parser: obj, default lxml.etree.HTMLParser()
-        HTML parser for lxml
+        HTML parser for ``lxml``
     pattern: str, default ''
         regular expression pattern for reducing list
     sort: bool, default False
         sort output list
 
     Returns
     -------
@@ -1004,43 +1303,55 @@
     # verify inputs for remote https host
     if isinstance(HOST, str):
         HOST = url_split(HOST)
     # try listing from https
     try:
         # Create and submit request.
         request = urllib2.Request(posixpath.join(*HOST))
-        tree = lxml.etree.parse(urllib2.urlopen(request,timeout=timeout),parser)
-    except (urllib2.HTTPError, urllib2.URLError) as e:
+        response = urllib2.urlopen(request, timeout=timeout)
+        tree = lxml.etree.parse(response, parser)
+    except (urllib2.HTTPError, urllib2.URLError) as exc:
         colerror = 'List error from {0}'.format(posixpath.join(*HOST))
-        return (False,False,colerror)
+        return (False, False, colerror)
     else:
         # read and parse request for files (column names and modified times)
         colnames = tree.xpath('//td[@class="indexcolname"]//a/@href')
         # get the Unix timestamp value for a modification time
         collastmod = [get_unix_time(i,format='%Y-%m-%d %H:%M')
             for i in tree.xpath('//td[@class="indexcollastmod"]/text()')]
         # reduce using regular expression pattern
         if pattern:
-            i = [i for i,f in enumerate(colnames) if re.search(pattern,f)]
+            i = [i for i,f in enumerate(colnames) if re.search(pattern, f)]
             # reduce list of column names and last modified times
             colnames = [colnames[indice] for indice in i]
             collastmod = [collastmod[indice] for indice in i]
         # sort the list
         if sort:
             i = [i for i,j in sorted(enumerate(colnames), key=lambda i: i[1])]
             # sort list of column names and last modified times
             colnames = [colnames[indice] for indice in i]
             collastmod = [collastmod[indice] for indice in i]
         # return the list of column names and last modified times
-        return (colnames,collastmod,None)
+        return (colnames, collastmod, None)
 
 # PURPOSE: download a file from a NSIDC https server
-def from_nsidc(HOST, username=None, password=None, build=True,
-    timeout=None, urs='urs.earthdata.nasa.gov', local=None,
-    hash='', chunk=16384, verbose=False, fid=sys.stdout, mode=0o775):
+def from_nsidc(
+        HOST: str | list,
+        username: str | None = None,
+        password: str | None = None,
+        build: bool = True,
+        timeout: int | None = None,
+        urs: str = 'urs.earthdata.nasa.gov',
+        local: str | pathlib.Path | None = None,
+        hash: str = '',
+        chunk: int = 16384,
+        verbose: bool = False,
+        fid=sys.stdout,
+        mode: oct = 0o775
+    ):
     """
     Download a file from a NSIDC https server
 
     Parameters
     ----------
     HOST: str or list
         remote https host
@@ -1083,55 +1394,54 @@
     # verify inputs for remote https host
     if isinstance(HOST, str):
         HOST = url_split(HOST)
     # try downloading from https
     try:
         # Create and submit request.
         request = urllib2.Request(posixpath.join(*HOST))
-        response = urllib2.urlopen(request,timeout=timeout)
-    except (urllib2.HTTPError, urllib2.URLError) as e:
+        response = urllib2.urlopen(request, timeout=timeout)
+    except (urllib2.HTTPError, urllib2.URLError) as exc:
         response_error = 'Download error from {0}'.format(posixpath.join(*HOST))
-        return (False,response_error)
+        return (False, response_error)
     else:
         # copy remote file contents to bytesIO object
         remote_buffer = io.BytesIO()
         shutil.copyfileobj(response, remote_buffer, chunk)
         remote_buffer.seek(0)
         # save file basename with bytesIO object
         remote_buffer.filename = HOST[-1]
         # generate checksum hash for remote file
         remote_hash = hashlib.md5(remote_buffer.getvalue()).hexdigest()
         # compare checksums
         if local and (hash != remote_hash):
             # convert to absolute path
-            local = os.path.abspath(local)
+            local = pathlib.Path(local).expanduser().absolute()
             # create directory if non-existent
-            if not os.access(os.path.dirname(local), os.F_OK):
-                os.makedirs(os.path.dirname(local), mode)
+            local.parent.mkdir(mode=mode, parents=True, exist_ok=True)
             # print file information
-            args = (posixpath.join(*HOST),local)
+            args = (posixpath.join(*HOST), str(local))
             logging.info('{0} -->\n\t{1}'.format(*args))
             # store bytes to file using chunked transfer encoding
             remote_buffer.seek(0)
-            with open(os.path.expanduser(local), 'wb') as f:
+            with local.open(mode='wb') as f:
                 shutil.copyfileobj(remote_buffer, f, chunk)
             # change the permissions mode
-            os.chmod(local,mode)
+            local.chmod(mode=mode)
         # return the bytesIO object
         remote_buffer.seek(0)
         return (remote_buffer,None)
 
 # PURPOSE: build formatted query string for ICESat-2 release
-def cmr_query_release(release):
+def cmr_query_release(release: str | int | None):
     """
     Build formatted query string for ICESat-2 release
 
     Parameters
     ----------
-    release: str
+    release: str, int or None
         ICESat-2 data release to query
 
     Returns
     -------
     query_params: str
         formatted string for CMR queries
     """
@@ -1147,21 +1457,21 @@
     while len(release) <= desired_pad_length:
         padded_release = release.zfill(desired_pad_length)
         query_params += f'&version={padded_release}'
         desired_pad_length -= 1
     return query_params
 
 # PURPOSE: check if the submitted cycles are valid
-def cmr_cycles(cycle):
+def cmr_cycles(cycle: str | int | list | None):
     """
     Check if the submitted cycles are valid
 
     Parameters
     ----------
-    cycle: str, list or NoneType, default None
+    cycle: str, int, list or NoneType
         ICESat-2 91-day orbital cycle
 
     Returns
     -------
     cycle_list: list
         formatted available 91-day orbital cycles
     """
@@ -1191,26 +1501,25 @@
             for c in cycle:
                 assert int(c) > 0, "Cycle number must be positive"
                 cycle_list.append(str(c).zfill(cycle_length))
         else:
             raise TypeError("Please enter the cycle number as a list or string")
         # check if user-entered cycle is outside of currently available range
         if not set(all_cycles) & set(cycle_list):
-            warnings.filterwarnings("always")
-            warnings.warn("Listed cycle is not presently available")
+            logging.warning("Listed cycle is not presently available")
         return cycle_list
 
 # PURPOSE: check if the submitted RGTs are valid
-def cmr_tracks(track):
+def cmr_tracks(track: str | int | list | None):
     """
     Check if the submitted RGTs are valid
 
     Parameters
     ----------
-    track: str, list or NoneType, default None
+    track: str, int, list or NoneType
         ICESat-2 reference ground track (RGT)
 
     Returns
     -------
     track_list: list
         formatted available reference ground tracks (RGTs)
     """
@@ -1231,26 +1540,25 @@
                 track_list.append(str(t).zfill(track_length))
         else:
             raise TypeError(
                 "Reference Ground Track as a list or string"
             )
         # check if user-entered RGT is outside of the valid range
         if not set(all_tracks) & set(track_list):
-            warnings.filterwarnings("always")
-            warnings.warn("Listed Reference Ground Track is not available")
+            logging.warning("Listed Reference Ground Track is not available")
         return track_list
 
 # PURPOSE: check if the submitted granule regions are valid
-def cmr_granules(granule):
+def cmr_granules(granule: str | int | list | None):
     """
     Check if the submitted granule regions are valid
 
     Parameters
     ----------
-    granule: str, list or NoneType, default None
+    granule: str, int, list or NoneType
         ICESat-2 granule region
 
     Returns
     -------
     granule_list: list
         formatted available granule regions
     """
@@ -1269,26 +1577,25 @@
             for g in granule:
                 assert int(g) > 0, "Granule region must be positive"
                 granule_list.append(str(g).zfill(granule_length))
         else:
             raise TypeError("Please enter the granule region as a list or string")
         # check if user-entered granule is outside of currently available range
         if not set(all_granules) & set(granule_list):
-            warnings.filterwarnings("always")
-            warnings.warn("Listed granule region is not presently available")
+            logging.warning("Listed granule region is not presently available")
         return granule_list
 
 # PURPOSE: check if the submitted ATL14/ATL15 regions are valid
-def cmr_regions(region):
+def cmr_regions(region: str | list | None):
     """
     Check if the submitted ATL14/ATL15 regions are valid
 
     Parameters
     ----------
-    region: str, list or NoneType, default None
+    region: str, list or NoneType
         ICESat-2 ATL14/ATL15 region
 
     Returns
     -------
     region_list: list
         formatted available ATL14/ATL15 regions
     """
@@ -1305,26 +1612,25 @@
             for r in region:
                 assert r in all_regions
                 region_list.append(str(r))
         else:
             raise TypeError("Please enter the region as a list or string")
         # check if user-entered region is currently not available
         if not set(all_regions) & set(region_list):
-            warnings.filterwarnings("always")
-            warnings.warn("Listed region is not presently available")
+            logging.warning("Listed region is not presently available")
         return region_list
 
 # PURPOSE: check if the submitted ATL14/ATL15 regions are valid
-def cmr_resolutions(resolution):
+def cmr_resolutions(resolution: str | list | None):
     """
     Check if the submitted ATL14/ATL15 resolutions are valid
 
     Parameters
     ----------
-    resolution: str, list or NoneType, default None
+    resolution: str, list or NoneType
         ICESat-2 ATL14/ATL15 spatial resolution
 
     Returns
     -------
     resolution_list: list
         formatted available ATL14/ATL15 resolutions
     """
@@ -1341,19 +1647,18 @@
             for r in resolution:
                 assert r in all_resolutions
                 resolution_list.append(str(r))
         else:
             raise TypeError("Please enter the resolution as a list or string")
         # check if user-entered resolution is currently not available
         if not set(all_resolutions) & set(resolution_list):
-            warnings.filterwarnings("always")
-            warnings.warn("Listed resolution is not presently available")
+            logging.warning("Listed resolution is not presently available")
         return resolution_list
 
-def cmr_readable_granules(product, **kwargs):
+def cmr_readable_granules(product: str, **kwargs):
     """
     Create list of readable granule names for CMR queries
 
     Parameters
     ----------
     product: str
         ICESat-2 data product
@@ -1408,22 +1713,32 @@
                         pattern = f"{product}_{14 * '?'}_{t}{c}{g}_*"
                     # append the granule pattern
                     readable_granule_list.append(pattern)
     # return readable granules list
     return readable_granule_list
 
 # PURPOSE: filter the CMR json response for desired data files
-def cmr_filter_json(search_results, request_type="application/x-hdfeos"):
+def cmr_filter_json(
+        search_results: dict,
+        endpoint: str = "data",
+        request_type: str = "application/x-hdfeos"
+    ):
     """
     Filter the CMR json response for desired data files
 
     Parameters
     ----------
     search_results: dict
         json response from CMR query
+    endpoint: str, default 'data'
+        url endpoint type
+
+            - ``'data'``: NASA Earthdata https archive
+            - ``'opendap'``: NASA Earthdata OPeNDAP archive
+            - ``'s3'``: NASA Earthdata Cumulus AWS S3 bucket
     request_type: str, default 'application/x-hdfeos'
         data type for reducing CMR query
 
     Returns
     -------
     producer_granule_ids: list
         ICESat-2 granules
@@ -1431,31 +1746,55 @@
         ICESat-2 granule urls from NSIDC
     """
     # output list of granule ids and urls
     producer_granule_ids = []
     granule_urls = []
     # check that there are urls for request
     if ('feed' not in search_results) or ('entry' not in search_results['feed']):
-        return (producer_granule_ids,granule_urls)
+        return (producer_granule_ids, granule_urls)
+    # descriptor links for each endpoint
+    rel = {}
+    rel['data'] = "http://esipfed.org/ns/fedsearch/1.1/data#"
+    rel['opendap'] = "http://esipfed.org/ns/fedsearch/1.1/service#"
+    rel['s3'] = "http://esipfed.org/ns/fedsearch/1.1/s3#"
     # iterate over references and get cmr location
     for entry in search_results['feed']['entry']:
         producer_granule_ids.append(entry['producer_granule_id'])
         for link in entry['links']:
-            if (link['type'] == request_type):
+            # skip links without descriptors
+            if ('rel' not in link.keys()):
+                continue
+            if ('type' not in link.keys()):
+                continue
+            # append if selected endpoint and request type
+            if (link['rel'] == rel[endpoint]) and (link['type'] == request_type):
                 granule_urls.append(link['href'])
                 break
     # return the list of urls and granule ids
-    return (producer_granule_ids,granule_urls)
+    return (producer_granule_ids, granule_urls)
 
 # PURPOSE: cmr queries for orbital parameters
-def cmr(product=None, release=None, cycles=None, tracks=None,
-    granules=None, regions=None, resolutions=None, bbox=None,
-    start_date=None, end_date=None, provider='NSIDC_ECS',
-    request_type="application/x-hdfeos", opener=None,
-    verbose=False, fid=sys.stdout):
+def cmr(
+        product: str = None,
+        release: str = None,
+        cycles: str | int | list | None = None,
+        tracks: str | int | list | None = None,
+        granules: str | int | list | None = None,
+        regions: str | list | None = None,
+        resolutions: str | list | None = None,
+        bbox: list | None = None,
+        start_date: str | None = None,
+        end_date: str | None = None,
+        provider: str = 'NSIDC_ECS',
+        endpoint: str = 'data',
+        request_type: str = "application/x-hdfeos",
+        opener = None,
+        verbose: bool = False,
+        fid = sys.stdout
+    ):
     """
     Query the NASA Common Metadata Repository (CMR) for ICESat-2 data
 
     Parameters
     ----------
     product: str or NoneType, default None
         ICESat-2 data product to query
@@ -1476,14 +1815,20 @@
         (``lon_min``, ``lat_min``, ``lon_max``, ``lat_max``)
     start_date: str or NoneType, default None
         starting date for CMR product query
     end_date: str or NoneType, default None
         ending date for CMR product query
     provider: str, default 'NSIDC_ECS'
         CMR data provider
+    endpoint: str, default 'data'
+        url endpoint type
+
+            - ``'data'``: NASA Earthdata https archive
+            - ``'opendap'``: NASA Earthdata OPeNDAP archive
+            - ``'s3'``: NASA Earthdata Cumulus AWS S3 bucket
     request_type: str, default 'application/x-hdfeos'
         data type for reducing CMR query
     opener: obj or NoneType, default None
         OpenerDirector instance
     verbose: bool, default False
         print file transfer information
     fid: obj, default sys.stdout
@@ -1503,15 +1848,15 @@
     if opener is None:
         # build urllib2 opener with SSL context
         # https://docs.python.org/3/howto/urllib2.html#id5
         handler = []
         # Create cookie jar for storing cookies
         cookie_jar = CookieJar()
         handler.append(urllib2.HTTPCookieProcessor(cookie_jar))
-        handler.append(urllib2.HTTPSHandler(context=ssl.SSLContext()))
+        handler.append(urllib2.HTTPSHandler(context=_default_ssl_context))
         # create "opener" (OpenerDirector instance)
         opener = urllib2.build_opener(*handler)
     # build CMR query
     cmr_query_type = 'granules'
     cmr_format = 'json'
     cmr_page_size = 2000
     CMR_HOST = ['https://cmr.earthdata.nasa.gov','search',
@@ -1558,15 +1903,16 @@
         response = opener.open(req)
         # get scroll id for next iteration
         if not cmr_scroll_id:
             headers = {k.lower():v for k,v in dict(response.info()).items()}
             cmr_scroll_id = headers['cmr-scroll-id']
         # read the CMR search as JSON
         search_page = json.loads(response.read().decode('utf-8'))
-        ids,urls = cmr_filter_json(search_page, request_type=request_type)
+        ids,urls = cmr_filter_json(search_page,
+            endpoint=endpoint, request_type=request_type)
         if not urls:
             break
         # extend lists
         producer_granule_ids.extend(ids)
         granule_urls.extend(urls)
     # return the list of granule ids and urls
     return (producer_granule_ids, granule_urls)
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit.egg-info/PKG-INFO` & `icesat2-toolkit-1.3.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,15 @@
-Metadata-Version: 2.1
-Name: icesat2-toolkit
-Version: 1.1.0
-Summary: Python tools for obtaining and working with elevation data from the NASA ICESat-2 mission
-Home-page: https://github.com/tsutterley/read-ICESat-2
-Author: Tyler Sutterley
-Author-email: tsutterl@uw.edu
-License: MIT
-Keywords: ICESat-2 laser altimetry,ATLAS,surface elevation and change
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-
 =============
 read-ICESat-2
 =============
 
 |Language|
 |License|
 |PyPI Version|
 |Documentation Status|
-|Binder|
-|Pangeo|
 |zenodo|
 |Shot Count|
 
 .. |Language| image:: https://img.shields.io/pypi/pyversions/icesat2-toolkit?color=green
    :target: https://www.python.org/
 
 .. |License| image:: https://img.shields.io/badge/license-MIT-green.svg
@@ -40,20 +17,14 @@
 
 .. |PyPI Version| image:: https://img.shields.io/pypi/v/icesat2-toolkit.svg
    :target: https://pypi.python.org/pypi/icesat2-toolkit/
 
 .. |Documentation Status| image:: https://readthedocs.org/projects/read-icesat-2/badge/?version=latest
    :target: https://read-icesat-2.readthedocs.io/en/latest/?badge=latest
 
-.. |Binder| image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/tsutterley/read-ICESat-2/main
-
-.. |Pangeo| image:: https://img.shields.io/static/v1.svg?logo=Jupyter&label=PangeoBinderAWS&message=us-west-2&color=orange
-   :target: https://aws-uswest2-binder.pangeo.io/v2/gh/tsutterley/read-ICESat-2/main?urlpath=lab
-
 .. |zenodo| image:: https://zenodo.org/badge/193143942.svg
    :target: https://zenodo.org/badge/latestdoi/193143942
 
 .. |Shot count| image:: https://img.shields.io/badge/dynamic/json?label=ICESat-2%20shot%20count&query=message&url=https%3A%2F%2Fraw.githubusercontent.com%2Ftsutterley%2Ftsutterley%2Fmaster%2FIS2-shot-count.json
    :target: https://icesat-2.gsfc.nasa.gov/
 
 Python tools for obtaining and working with elevation data from the NASA ICESat-2 mission
@@ -165,38 +136,41 @@
 
 ICESat-2 Granules
 #################
 
 Each orbit of ICESat-2 data is broken up into 14 granules.
 The granule boundaries limit the size of each ATL03 file and simplify the formation of higher level data products.
 
-.. image:: ./icesat2_toolkit/data/ICESat-2_granules_global.png
+.. image:: ./doc/source/_assets/ICESat-2_granules_global.png
   :alt: ICESat-2 global granules
 
-.. image:: ./icesat2_toolkit/data/ICESat-2_granules_polar.png
+.. image:: ./doc/source/_assets/ICESat-2_granules_polar.png
   :alt: ICESat-2 polar granules
 
 Dependencies
 ############
 
- - `numpy: Scientific Computing Tools For Python <https://numpy.org>`_
- - `scipy: Scientific Tools for Python <https://docs.scipy.org/doc/>`_
- - `mpi4py: Python bindings of the Message Passing Interface (MPI) <https://mpi4py.readthedocs.io/en/stable/>`_
- - `h5py: Python interface for Hierarchal Data Format 5 (HDF5) <http://h5py.org>`_
- - `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
- - `zarr: Chunked, compressed, N-dimensional arrays in Python <https://github.com/zarr-developers/zarr-python>`_
- - `pandas: Python Data Analysis Library <https://pandas.pydata.org/>`_
- - `scikit-learn: Machine Learning in Python <https://scikit-learn.org/stable/index.html>`_
- - `shapely: PostGIS-ish operations outside a database context for Python <http://toblerity.org/shapely/index.html>`_
- - `fiona: Python wrapper for vector data access functions from the OGR library <https://fiona.readthedocs.io/en/latest/manual.html>`_
- - `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
- - `paramiko: Native Python SSHv2 protocol library <http://www.paramiko.org/>`_
- - `scp: scp module for paramiko <https://github.com/jbardin/scp.py>`_
- - `future: Compatibility layer between Python 2 and Python 3 <http://python-future.org/>`_
- - `yapc: Python version of the NASA Goddard Space Flight Center YAPC Program <https://github.com/tsutterley/yapc>`_
+- `numpy: Scientific Computing Tools For Python <https://numpy.org>`_
+- `scipy: Scientific Tools for Python <https://docs.scipy.org/doc//>`_
+- `mpi4py: Python bindings of the Message Passing Interface (MPI) <https://mpi4py.readthedocs.io/en/stable/>`_
+- `h5py: Python interface for Hierarchal Data Format 5 (HDF5) <http://h5py.org>`_
+- `netCDF4: Python interface to the netCDF C library <https://unidata.github.io/netcdf4-python/>`_
+- `zarr: Chunked, compressed, N-dimensional arrays in Python <https://github.com/zarr-developers/zarr-python>`_
+- `pandas: Python Data Analysis Library <https://pandas.pydata.org/>`_
+- `scikit-learn: Machine Learning in Python <https://scikit-learn.org/stable/index.html>`_
+- `dateutil: powerful extensions to datetime <https://dateutil.readthedocs.io/en/stable/>`_
+- `shapely: PostGIS-ish operations outside a database context for Python <http://toblerity.org/shapely/index.html>`_
+- `fiona: Python wrapper for vector data access functions from the OGR library <https://fiona.readthedocs.io/en/latest/manual.html>`_
+- `future: Compatibility layer between Python 2 and Python 3 <http://python-future.org/>`_
+- `boto3: Amazon Web Services (AWS) SDK for Python <https://boto3.amazonaws.com/v1/documentation/api/latest/index.html>`_
+- `s3fs: Pythonic file interface to S3 built on top of botocore <https://s3fs.readthedocs.io/en/latest/>`_
+- `lxml: processing XML and HTML in Python <https://pypi.python.org/pypi/lxml>`_
+- `paramiko: Native Python SSHv2 protocol library <http://www.paramiko.org>`_
+- `scp: scp module for paramiko <https://github.com/jbardin/scp.py>`_
+- `yapc: Python version of the NASA Goddard Space Flight Center YAPC Program <https://github.com/tsutterley/yapc>`_
 
 Download
 ########
 
 | The program homepage is:
 | https://github.com/tsutterley/read-icesat-2
 | A zip archive of the latest version is available directly at:
```

### Comparing `icesat2-toolkit-1.1.0/icesat2_toolkit.egg-info/SOURCES.txt` & `icesat2-toolkit-1.3.0/icesat2_toolkit.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,26 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 icesat2_toolkit/__init__.py
 icesat2_toolkit/convert.py
-icesat2_toolkit/convert_calendar_decimal.py
 icesat2_toolkit/convert_delta_time.py
-icesat2_toolkit/convert_julian.py
-icesat2_toolkit/count_leap_seconds.py
 icesat2_toolkit/fit.py
-icesat2_toolkit/read_ICESat2_ATL03.py
-icesat2_toolkit/read_ICESat2_ATL06.py
-icesat2_toolkit/read_ICESat2_ATL07.py
-icesat2_toolkit/read_ICESat2_ATL10.py
-icesat2_toolkit/read_ICESat2_ATL11.py
-icesat2_toolkit/read_ICESat2_ATL12.py
 icesat2_toolkit/spatial.py
 icesat2_toolkit/time.py
 icesat2_toolkit/tools.py
 icesat2_toolkit/utilities.py
 icesat2_toolkit/version.py
 icesat2_toolkit.egg-info/PKG-INFO
 icesat2_toolkit.egg-info/SOURCES.txt
 icesat2_toolkit.egg-info/dependency_links.txt
 icesat2_toolkit.egg-info/requires.txt
 icesat2_toolkit.egg-info/top_level.txt
-icesat2_toolkit/data/ICESat-2_granules_global.png
-icesat2_toolkit/data/ICESat-2_granules_polar.png
 icesat2_toolkit/data/leap-seconds.list
 icesat2_toolkit/io/ATL03.py
 icesat2_toolkit/io/ATL06.py
 icesat2_toolkit/io/ATL07.py
 icesat2_toolkit/io/ATL10.py
 icesat2_toolkit/io/ATL11.py
 icesat2_toolkit/io/ATL12.py
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_DEM_ICESat2_ATL03.py` & `icesat2-toolkit-1.3.0/scripts/MPI_DEM_ICESat2_ATL03.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,41 +111,37 @@
 import scipy.interpolate
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import fiona
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
+    warnings.filterwarnings("module")
     warnings.warn("fiona not available")
     warnings.warn("Some functions will throw an exception if called")
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import osgeo.gdal
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("GDAL not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("GDAL not available", ImportWarning)
 try:
     from shapely.geometry import MultiPoint, Polygon
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapely not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapely not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # digital elevation models
 elevation_dir = {}
 elevation_tile_index = {}
 # ArcticDEM
@@ -523,15 +519,15 @@
             distributed_map = np.zeros((n_pe),dtype=int)
             # create empty intersection map array for receiving
             associated_map[key] = np.zeros((n_pe),dtype=int)
             # finds if points are encapsulated (within tile)
             int_test = poly_obj.intersects(xy_point)
             if int_test:
                 # extract intersected points
-                int_map = list(map(poly_obj.intersects,xy_point))
+                int_map = list(map(poly_obj.intersects, xy_point.geoms))
                 int_indices, = np.nonzero(int_map)
                 # set distributed_map indices to True for intersected points
                 distributed_map[ind[int_indices]] = True
             # communicate output MPI matrices between ranks
             # operation is a logical "or" across the elements.
             comm.Allreduce(sendbuf=[distributed_map, MPI.BOOL], \
                 recvbuf=[associated_map[key], MPI.BOOL], op=MPI.LOR)
@@ -802,15 +798,15 @@
     # parallel h5py I/O does not support compression filters at this time
     if (comm.rank == 0) and bool(valid_tiles):
         # output HDF5 files with output masks
         fargs = (PRD,DEM_MODEL,YY,MM,DD,HH,MN,SS,TRK,CYC,GRN,RL,VRS,AUX)
         file_format = '{0}_{1}_{2}{3}{4}{5}{6}{7}_{8}{9}{10}_{11}_{12}{13}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
         # print file information
-        logging.into(f'\t{output_file}')
+        logging.info(f'\t{output_file}')
         # write to output HDF5 file
         HDF5_ATL03_dem_write(IS2_atl03_dem, IS2_atl03_dem_attrs,
             CLOBBER=True, INPUT=os.path.basename(args.file),
             FILL_VALUE=IS2_atl03_fill, DIMENSIONS=IS2_atl03_dims,
             FILENAME=output_file)
         # change the permissions mode
         os.chmod(output_file, args.mode)
@@ -952,14 +948,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_DEM_ICESat2_ATL06.py` & `icesat2-toolkit-1.3.0/scripts/MPI_DEM_ICESat2_ATL06.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,41 +111,37 @@
 import scipy.interpolate
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import fiona
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
+    warnings.filterwarnings("module")
     warnings.warn("fiona not available")
     warnings.warn("Some functions will throw an exception if called")
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import osgeo.gdal
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("GDAL not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("GDAL not available", ImportWarning)
 try:
     from shapely.geometry import MultiPoint, Polygon
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapely not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapely not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # digital elevation models
 elevation_dir = {}
 elevation_tile_index = {}
 # ArcticDEM
@@ -523,15 +519,15 @@
             distributed_map = np.zeros((n_seg),dtype=int)
             # create empty intersection map array for receiving
             associated_map[key] = np.zeros((n_seg),dtype=int)
             # finds if points are encapsulated (within tile)
             int_test = poly_obj.intersects(xy_point)
             if int_test:
                 # extract intersected points
-                int_map = list(map(poly_obj.intersects,xy_point))
+                int_map = list(map(poly_obj.intersects, xy_point.geoms))
                 int_indices, = np.nonzero(int_map)
                 # set distributed_map indices to True for intersected points
                 distributed_map[ind[int_indices]] = True
             # communicate output MPI matrices between ranks
             # operation is a logical "or" across the elements.
             comm.Allreduce(sendbuf=[distributed_map, MPI.BOOL], \
                 recvbuf=[associated_map[key], MPI.BOOL], op=MPI.LOR)
@@ -834,15 +830,15 @@
     # parallel h5py I/O does not support compression filters at this time
     if (comm.rank == 0) and bool(valid_tiles):
         # output HDF5 files with output masks
         fargs = (PRD,DEM_MODEL,YY,MM,DD,HH,MN,SS,TRK,CYC,GRN,RL,VRS,AUX)
         file_format = '{0}_{1}_{2}{3}{4}{5}{6}{7}_{8}{9}{10}_{11}_{12}{13}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
         # print file information
-        logging.into(f'\t{output_file}')
+        logging.info(f'\t{output_file}')
         # write to output HDF5 file
         HDF5_ATL06_dem_write(IS2_atl06_dem, IS2_atl06_dem_attrs,
             CLOBBER=True, INPUT=os.path.basename(args.file),
             FILL_VALUE=IS2_atl06_fill, DIMENSIONS=IS2_atl06_dims,
             FILENAME=output_file)
         # change the permissions mode
         os.chmod(output_file, args.mode)
@@ -1007,14 +1003,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_DEM_ICESat2_ATL11.py` & `icesat2-toolkit-1.3.0/scripts/MPI_DEM_ICESat2_ATL11.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,41 +90,37 @@
 import scipy.interpolate
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import fiona
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
+    warnings.filterwarnings("module")
     warnings.warn("fiona not available")
     warnings.warn("Some functions will throw an exception if called")
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import osgeo.gdal
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("GDAL not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("GDAL not available", ImportWarning)
 try:
     from shapely.geometry import MultiPoint, Polygon
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapely not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapely not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # digital elevation models
 elevation_dir = {}
 elevation_tile_index = {}
 # ArcticDEM
@@ -500,15 +496,15 @@
             distributed_map = np.zeros((n_points),dtype=int)
             # create empty intersection map array for receiving
             associated_map[key] = np.zeros((n_points),dtype=int)
             # finds if points are encapsulated (within tile)
             int_test = poly_obj.intersects(xy_point)
             if int_test:
                 # extract intersected points
-                int_map = list(map(poly_obj.intersects,xy_point))
+                int_map = list(map(poly_obj.intersects, xy_point.geoms))
                 int_indices, = np.nonzero(int_map)
                 # set distributed_map indices to True for intersected points
                 distributed_map[ind[int_indices]] = True
             # communicate output MPI matrices between ranks
             # operation is a logical "or" across the elements.
             comm.Allreduce(sendbuf=[distributed_map, MPI.BOOL], \
                 recvbuf=[associated_map[key], MPI.BOOL], op=MPI.LOR)
@@ -814,15 +810,15 @@
     # parallel h5py I/O does not support compression filters at this time
     if (comm.rank == 0) and bool(valid_tiles):
         # output HDF5 files with output masks
         fargs = (PRD,DEM_MODEL,TRK,GRAN,SCYC,ECYC,RL,VERS,AUX)
         file_format = '{0}_{1}_{2}{3}_{4}{5}_{6}_{7}{8}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
         # print file information
-        logging.into(f'\t{output_file}')
+        logging.info(f'\t{output_file}')
         # write to output HDF5 file
         HDF5_ATL11_dem_write(IS2_atl11_dem, IS2_atl11_dem_attrs,
             CLOBBER=True, INPUT=os.path.basename(args.file),
             FILL_VALUE=IS2_atl11_fill, DIMENSIONS=IS2_atl11_dims,
             FILENAME=output_file)
         # change the permissions mode
         os.chmod(output_file, args.mode)
@@ -978,14 +974,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_ICESat2_ATL03.py` & `icesat2-toolkit-1.3.0/scripts/MPI_ICESat2_ATL03.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,35 +85,32 @@
 import scipy.interpolate
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import sklearn.neighbors
     import sklearn.cluster
-except (ImportError, ModuleNotFoundError) as e:
-    warnings.filterwarnings("always")
-    warnings.warn("scikit-learn not available")
+except (ImportError, ModuleNotFoundError) as exc:
+    warnings.filterwarnings("module")
+    warnings.warn("scikit-learn not available", ImportWarning)
 try:
     import yapc.classify_photons
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("pyYAPC not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("pyYAPC not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: keep track of MPI threads
 def info(rank, size):
     logging.info(f'Rank {rank+1:d} of {size:d}')
     logging.info(f'module name: {__name__}')
@@ -2460,14 +2457,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_ICESat2_ATL03_histogram.py` & `icesat2-toolkit-1.3.0/scripts/MPI_ICESat2_ATL03_histogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,35 +124,32 @@
 import scipy.interpolate
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import sklearn.neighbors
     import sklearn.cluster
-except (ImportError, ModuleNotFoundError) as e:
-    warnings.filterwarnings("always")
-    warnings.warn("scikit-learn not available")
+except (ImportError, ModuleNotFoundError) as exc:
+    warnings.filterwarnings("module")
+    warnings.warn("scikit-learn not available", ImportWarning)
 try:
     import yapc.classify_photons
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("pyYAPC not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("pyYAPC not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: keep track of MPI threads
 def info(rank, size):
     logging.info(f'Rank {rank+1:d} of {size:d}')
     logging.info(f'module name: {__name__}')
@@ -548,15 +545,15 @@
         tlm_buffer = 100.0
         # flag denoting photon events as possible TEP
         if (int(RL) < 4):
             isTEP = np.any((fileID[gtx]['heights']['signal_conf_ph'][:]==-2),axis=1)
         else:
             isTEP = (fileID[gtx]['heights']['quality_ph'][:] == 3)
         # photon event weights
-        Distributed_Weights = np.zeros((n_pe),dtype=np.float)
+        Distributed_Weights = np.zeros((n_pe), dtype=np.float64)
         # run for each major frame (distributed over comm.size # of processes)
         for iteration in range(comm.rank, major_frame_count, comm.size):
             # background atlas index for iteration
             idx = unique_index[iteration]
             # photon indices for major frame (buffered by 1 frame on each side)
             # do not use possible TEP photons in photon classification
             i1, = np.nonzero((photon_mframes >= unique_major_frames[iteration]-1) &
@@ -576,15 +573,15 @@
                     h_win_width += tlm_height[b][idx]
             # calculate photon event weights
             Distributed_Weights[i1[i2]] = yapc.classify_photons(x_atc[i1],
                 h_ph[i1], h_win_width, i2, K=0, min_knn=5, min_ph=3,
                 min_xspread=1.0, min_hspread=0.01, win_x=15.0, win_h=6.0,
                 method='linear')
         # photon event weights
-        pe_weights = np.zeros((n_pe),dtype=np.float)
+        pe_weights = np.zeros((n_pe), dtype=np.float64)
         comm.Allreduce(sendbuf=[Distributed_Weights, MPI.DOUBLE], \
             recvbuf=[pe_weights, MPI.DOUBLE], op=MPI.SUM)
         Distributed_Weights = None
         # wait for all distributed processes to finish for beam
         comm.Barrier()
 
         # photon event weights scaled to a single byte
@@ -2729,14 +2726,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL03_RGI.py` & `icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL03_RGI.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,35 +92,31 @@
 import numpy as np
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import shapefile
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapefile not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapefile not available", ImportWarning)
 try:
     from shapely.geometry import MultiPoint, Polygon
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapely not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapely not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: keep track of MPI threads
 def info(rank, size):
     logging.info(f'Rank {rank+1:d} of {size:d}')
     logging.info(f'module name: {__name__}')
@@ -327,15 +323,15 @@
         associated_map = np.zeros((n_pe),dtype=bool)
         associated_RGIId = np.zeros((n_pe),dtype='|S14')
         for key,poly_obj in poly_dict.items():
             # finds if points are encapsulated (within RGI polygon)
             int_test = poly_obj.intersects(xy_point)
             if int_test:
                 # extract intersected points
-                int_map = list(map(poly_obj.intersects,xy_point))
+                int_map = list(map(poly_obj.intersects, xy_point.geoms))
                 int_indices, = np.nonzero(int_map)
                 # set distributed_map indices to True for intersected points
                 distributed_map[ind[int_indices]] = True
                 distributed_RGIId[ind[int_indices]] = key
         # communicate output MPI matrices between ranks
         # operation is a logical "or" across the elements.
         comm.Allreduce(sendbuf=[distributed_map, MPI.BOOL], \
@@ -454,15 +450,15 @@
     # parallel h5py I/O does not support compression filters at this time
     if (comm.rank == 0) and valid_check:
         # output HDF5 file with RGI masks
         fargs=(PRD,RGI_VERSION,RGI_NAME,YY,MM,DD,HH,MN,SS,TRK,CYC,GRN,RL,VRS,AUX)
         file_format='{0}_RGI{1}_{2}_{3}{4}{5}{6}{7}{8}_{9}{10}{11}_{12}_{13}{14}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
         # print file information
-        logging.into(f'\t{output_file}')
+        logging.info(f'\t{output_file}')
         # write to output HDF5 file
         HDF5_ATL03_mask_write(IS2_atl03_mask, IS2_atl03_mask_attrs,
             CLOBBER=True, INPUT=os.path.basename(args.file),
             FILL_VALUE=IS2_atl03_fill, DIMENSIONS=IS2_atl03_dims,
             FILENAME=output_file)
         # change the permissions mode
         os.chmod(output_file, args.mode)
@@ -603,14 +599,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL06_RGI.py` & `icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL06_RGI.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,35 +91,31 @@
 import numpy as np
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import shapefile
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapefile not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapefile not available", ImportWarning)
 try:
     from shapely.geometry import MultiPoint, Polygon
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapely not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapely not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: keep track of MPI threads
 def info(rank, size):
     logging.info(f'Rank {rank+1:d} of {size:d}')
     logging.info(f'module name: {__name__}')
@@ -328,15 +324,15 @@
         associated_map = np.zeros((n_seg),dtype=bool)
         associated_RGIId = np.zeros((n_seg),dtype='|S14')
         for key,poly_obj in poly_dict.items():
             # finds if points are encapsulated (within RGI polygon)
             int_test = poly_obj.intersects(xy_point)
             if int_test:
                 # extract intersected points
-                int_map = list(map(poly_obj.intersects,xy_point))
+                int_map = list(map(poly_obj.intersects, xy_point.geoms))
                 int_indices, = np.nonzero(int_map)
                 # set distributed_map indices to True for intersected points
                 distributed_map[ind[int_indices]] = True
                 distributed_RGIId[ind[int_indices]] = key
         # communicate output MPI matrices between ranks
         # operation is a logical "or" across the elements.
         comm.Allreduce(sendbuf=[distributed_map, MPI.BOOL], \
@@ -477,15 +473,15 @@
     # parallel h5py I/O does not support compression filters at this time
     if (comm.rank == 0) and valid_check:
         # output HDF5 file with RGI masks
         fargs=(PRD,RGI_VERSION,RGI_NAME,YY,MM,DD,HH,MN,SS,TRK,CYC,GRN,RL,VRS,AUX)
         file_format='{0}_RGI{1}_{2}_{3}{4}{5}{6}{7}{8}_{9}{10}{11}_{12}_{13}{14}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
         # print file information
-        logging.into(f'\t{output_file}')
+        logging.info(f'\t{output_file}')
         # write to output HDF5 file
         HDF5_ATL06_mask_write(IS2_atl06_mask, IS2_atl06_mask_attrs,
             CLOBBER=True, INPUT=os.path.basename(args.file),
             FILL_VALUE=IS2_atl06_fill, DIMENSIONS=IS2_atl06_dims,
             FILENAME=output_file)
         # change the permissions mode
         os.chmod(output_file, args.mode)
@@ -532,15 +528,15 @@
         fileID[gtx].create_group('land_ice_segments')
         h5[gtx] = dict(land_ice_segments={})
         for att_name in ['Description','data_rate']:
             att_val = IS2_atl06_attrs[gtx]['land_ice_segments'][att_name]
             fileID[gtx]['land_ice_segments'].attrs[att_name] = att_val
 
         # segment_id, geolocation, time and height variables
-        for k in ['segment_id','latitude','longitude','delta_time']:
+        for k in ['delta_time','segment_id','latitude','longitude']:
             # values and attributes
             v = IS2_atl06_mask[gtx]['land_ice_segments'][k]
             attrs = IS2_atl06_attrs[gtx]['land_ice_segments'][k]
             fillvalue = FILL_VALUE[gtx]['land_ice_segments'][k]
             # Defining the HDF5 dataset variables
             val = '{0}/{1}/{2}'.format(gtx,'land_ice_segments',k)
             if fillvalue:
@@ -649,14 +645,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL06_drainages.py` & `icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL06_drainages.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,35 +71,31 @@
 import numpy as np
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import shapefile
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapefile not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapefile not available", ImportWarning)
 try:
     from shapely.geometry import MultiPoint, Polygon
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapely not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapely not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # IMBIE-2 Drainage basins
 IMBIE_basin_file = {}
 IMBIE_basin_file['N'] = ['GRE_Basins_IMBIE2_v1.3','GRE_Basins_IMBIE2_v1.3.shp']
 IMBIE_basin_file['S'] = ['ANT_Basins_IMBIE2_v1.6','ANT_Basins_IMBIE2_v1.6.shp']
@@ -323,15 +319,15 @@
             distributed_map = np.zeros((n_seg),dtype=bool)
             # create empty intersection map array for receiving
             associated_map[key] = np.zeros((n_seg),dtype=bool)
             # finds if points are encapsulated (within basin)
             int_test = poly_obj.intersects(xy_point)
             if int_test:
                 # extract intersected points
-                int_map = list(map(poly_obj.intersects,xy_point))
+                int_map = list(map(poly_obj.intersects, xy_point.geoms))
                 int_indices, = np.nonzero(int_map)
                 # set distributed_map indices to True for intersected points
                 distributed_map[ind[int_indices]] = True
             # communicate output MPI matrices between ranks
             # operation is a logical "or" across the elements.
             comm.Allreduce(sendbuf=[distributed_map, MPI.BOOL], \
                 recvbuf=[associated_map[key], MPI.BOOL], op=MPI.LOR)
@@ -454,15 +450,15 @@
     # parallel h5py I/O does not support compression filters at this time
     if (comm.rank == 0) and valid_check:
         # output HDF5 file with drainage basin masks
         fargs = (PRD,BASIN_TITLE,YY,MM,DD,HH,MN,SS,TRK,CYC,GRN,RL,VRS,AUX)
         file_format = '{0}_{1}_{2}{3}{4}{5}{6}{7}_{8}{9}{10}_{11}_{12}{13}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
         # print file information
-        logging.into(f'\t{output_file}')
+        logging.info(f'\t{output_file}')
         # write to output HDF5 file
         HDF5_ATL06_mask_write(IS2_atl06_mask, IS2_atl06_mask_attrs,
             CLOBBER=True, INPUT=os.path.basename(args.file),
             FILL_VALUE=IS2_atl06_fill, DIMENSIONS=IS2_atl06_dims,
             FILENAME=output_file)
         # change the permissions mode
         os.chmod(output_file, args.mode)
@@ -509,15 +505,15 @@
         fileID[gtx].create_group('land_ice_segments')
         h5[gtx] = dict(land_ice_segments={})
         for att_name in ['Description','data_rate']:
             att_val = IS2_atl06_attrs[gtx]['land_ice_segments'][att_name]
             fileID[gtx]['land_ice_segments'].attrs[att_name] = att_val
 
         # segment_id, geolocation, time and height variables
-        for k in ['segment_id','latitude','longitude','delta_time']:
+        for k in ['delta_time','segment_id','latitude','longitude']:
             # values and attributes
             v = IS2_atl06_mask[gtx]['land_ice_segments'][k]
             attrs = IS2_atl06_attrs[gtx]['land_ice_segments'][k]
             fillvalue = FILL_VALUE[gtx]['land_ice_segments'][k]
             # Defining the HDF5 dataset variables
             val = '{0}/{1}/{2}'.format(gtx,'land_ice_segments',k)
             if fillvalue:
@@ -626,14 +622,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL06_grounded.py` & `icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL06_grounded.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,35 +75,31 @@
 import numpy as np
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import shapefile
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapefile not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapefile not available", ImportWarning)
 try:
     from shapely.geometry import MultiPoint, Polygon
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapely not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapely not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # regional grounded ice files
 grounded_file = {}
 grounded_file['N'] = ['BedMachineGreenlandGroundedv4.shp']
 grounded_file['S'] = ['IceBoundaries_Antarctica_v02.shp']
@@ -322,15 +318,15 @@
             distributed_map = np.zeros((n_seg),dtype=bool)
             # create empty intersection map array for receiving
             associated_map[key] = np.zeros((n_seg),dtype=bool)
             # finds if points are encapsulated (within grounded region)
             int_test = poly_obj.intersects(xy_point)
             if int_test:
                 # extract intersected points
-                int_map = list(map(poly_obj.intersects,xy_point))
+                int_map = list(map(poly_obj.intersects, xy_point.geoms))
                 int_indices, = np.nonzero(int_map)
                 # set distributed_map indices to True for intersected points
                 distributed_map[ind[int_indices]] = True
             # communicate output MPI matrices between ranks
             # operation is a logical "or" across the elements.
             comm.Allreduce(sendbuf=[distributed_map, MPI.BOOL], \
                 recvbuf=[associated_map[key], MPI.BOOL], op=MPI.LOR)
@@ -470,15 +466,15 @@
     # parallel h5py I/O does not support compression filters at this time
     if (comm.rank == 0) and valid_check:
         # output HDF5 files with grounded ice masks
         fargs = (PRD,'GROUNDED_MASK',YY,MM,DD,HH,MN,SS,TRK,CYC,GRN,RL,VRS,AUX)
         file_format = '{0}_{1}_{2}{3}{4}{5}{6}{7}_{8}{9}{10}_{11}_{12}{13}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
         # print file information
-        logging.into(f'\t{output_file}')
+        logging.info(f'\t{output_file}')
         # write to output HDF5 file
         HDF5_ATL06_mask_write(IS2_atl06_mask, IS2_atl06_mask_attrs, CLOBBER=True,
             INPUT=os.path.basename(args.file), FILL_VALUE=IS2_atl06_fill,
             FILENAME=output_file)
         # change the permissions mode
         os.chmod(output_file, args.mode)
     # close the input file
@@ -524,15 +520,15 @@
         fileID[gtx].create_group('land_ice_segments')
         h5[gtx] = dict(land_ice_segments={})
         for att_name in ['Description','data_rate']:
             att_val = IS2_atl06_attrs[gtx]['land_ice_segments'][att_name]
             fileID[gtx]['land_ice_segments'].attrs[att_name] = att_val
 
         # segment_id, geolocation, time and height variables
-        for k in ['segment_id','latitude','longitude','delta_time']:
+        for k in ['delta_time','segment_id','latitude','longitude']:
             # values and attributes
             v = IS2_atl06_mask[gtx]['land_ice_segments'][k]
             attrs = IS2_atl06_attrs[gtx]['land_ice_segments'][k]
             fillvalue = FILL_VALUE[gtx]['land_ice_segments'][k]
             # Defining the HDF5 dataset variables
             val = '{0}/{1}/{2}'.format(gtx,'land_ice_segments',k)
             if fillvalue:
@@ -641,14 +637,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL06_ice_shelves.py` & `icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL06_ice_shelves.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,35 +73,31 @@
 import numpy as np
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import shapefile
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapefile not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapefile not available", ImportWarning)
 try:
     from shapely.geometry import MultiPoint, Polygon
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapely not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapely not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # regional ice shelf files
 ice_shelf_file = {}
 ice_shelf_file['N'] = ['BedMachineGreenlandFloatingv4.shp']
 ice_shelf_file['S'] = ['IceBoundaries_Antarctica_v02.shp']
@@ -311,15 +307,15 @@
             distributed_map = np.zeros((n_seg),dtype=bool)
             # create empty intersection map array for receiving
             associated_map[key] = np.zeros((n_seg),dtype=bool)
             # finds if points are encapsulated (within ice shelf)
             int_test = poly_obj.intersects(xy_point)
             if int_test:
                 # extract intersected points
-                int_map = list(map(poly_obj.intersects,xy_point))
+                int_map = list(map(poly_obj.intersects, xy_point.geoms))
                 int_indices, = np.nonzero(int_map)
                 # set distributed_map indices to True for intersected points
                 distributed_map[ind[int_indices]] = True
             # communicate output MPI matrices between ranks
             # operation is a logical "or" across the elements.
             comm.Allreduce(sendbuf=[distributed_map, MPI.BOOL], \
                 recvbuf=[associated_map[key], MPI.BOOL], op=MPI.LOR)
@@ -459,15 +455,15 @@
     # parallel h5py I/O does not support compression filters at this time
     if (comm.rank == 0) and valid_check:
         # output HDF5 files with ice shelf masks
         fargs = (PRD,'ICE_SHELF_MASK',YY,MM,DD,HH,MN,SS,TRK,CYC,GRN,RL,VRS,AUX)
         file_format = '{0}_{1}_{2}{3}{4}{5}{6}{7}_{8}{9}{10}_{11}_{12}{13}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
         # print file information
-        logging.into(f'\t{output_file}')
+        logging.info(f'\t{output_file}')
         # write to output HDF5 file
         HDF5_ATL06_mask_write(IS2_atl06_mask, IS2_atl06_mask_attrs, CLOBBER=True,
             INPUT=os.path.basename(args.file), FILL_VALUE=IS2_atl06_fill,
             FILENAME=output_file)
         # change the permissions mode
         os.chmod(output_file, args.mode)
     # close the input file
@@ -513,15 +509,15 @@
         fileID[gtx].create_group('land_ice_segments')
         h5[gtx] = dict(land_ice_segments={})
         for att_name in ['Description','data_rate']:
             att_val = IS2_atl06_attrs[gtx]['land_ice_segments'][att_name]
             fileID[gtx]['land_ice_segments'].attrs[att_name] = att_val
 
         # segment_id, geolocation, time and height variables
-        for k in ['segment_id','latitude','longitude','delta_time']:
+        for k in ['delta_time','segment_id','latitude','longitude']:
             # values and attributes
             v = IS2_atl06_mask[gtx]['land_ice_segments'][k]
             attrs = IS2_atl06_attrs[gtx]['land_ice_segments'][k]
             fillvalue = FILL_VALUE[gtx]['land_ice_segments'][k]
             # Defining the HDF5 dataset variables
             val = '{0}/{1}/{2}'.format(gtx,'land_ice_segments',k)
             if fillvalue:
@@ -630,14 +626,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL11_RGI.py` & `icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL11_RGI.py`

 * *Files 3% similar despite different names*

```diff
@@ -84,35 +84,31 @@
 import collections
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import shapefile
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapefile not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapefile not available", ImportWarning)
 try:
     from shapely.geometry import MultiPoint, Polygon
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapely not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapely not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: keep track of MPI threads
 def info(rank, size):
     logging.info(f'Rank {rank+1:d} of {size:d}')
     logging.info(f'module name: {__name__}')
@@ -315,15 +311,15 @@
         associated_map = np.zeros((n_points),dtype=bool)
         associated_RGIId = np.zeros((n_points),dtype='|S14')
         for key,poly_obj in poly_dict.items():
             # finds if points are encapsulated (within RGI polygon)
             int_test = poly_obj.intersects(xy_point)
             if int_test:
                 # extract intersected points
-                int_map = list(map(poly_obj.intersects,xy_point))
+                int_map = list(map(poly_obj.intersects, xy_point.geoms))
                 int_indices, = np.nonzero(int_map)
                 # set distributed_map indices to True for intersected points
                 distributed_map[ind[int_indices]] = True
                 distributed_RGIId[ind[int_indices]] = key
         # communicate output MPI matrices between ranks
         # operation is a logical "or" across the elements.
         comm.Allreduce(sendbuf=[distributed_map, MPI.BOOL], \
@@ -474,15 +470,15 @@
     # parallel h5py I/O does not support compression filters at this time
     if (comm.rank == 0) and valid_check:
         # output HDF5 file with RGI masks
         fargs = (PRD,RGI_VERSION,RGI_NAME,TRK,GRAN,SCYC,ECYC,RL,VERS,AUX)
         file_format = '{0}_RGI{1}_{2}_{3}{4}_{5}{6}_{7}_{8}{9}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
         # print file information
-        logging.into(f'\t{output_file}')
+        logging.info(f'\t{output_file}')
         # write to output HDF5 file
         HDF5_ATL11_mask_write(IS2_atl11_mask, IS2_atl11_mask_attrs,
             CLOBBER=True, INPUT=os.path.basename(args.file),
             FILL_VALUE=IS2_atl11_fill, DIMENSIONS=IS2_atl11_dims,
             FILENAME=output_file)
         # change the permissions mode
         os.chmod(output_file, args.mode)
@@ -637,14 +633,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL11_drainages.py` & `icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL11_drainages.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,35 +63,31 @@
 import collections
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import shapefile
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapefile not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapefile not available", ImportWarning)
 try:
     from shapely.geometry import MultiPoint, Polygon
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapely not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapely not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # IMBIE-2 Drainage basins
 IMBIE_basin_file = {}
 IMBIE_basin_file['N'] = ['GRE_Basins_IMBIE2_v1.3','GRE_Basins_IMBIE2_v1.3.shp']
 IMBIE_basin_file['S'] = ['ANT_Basins_IMBIE2_v1.6','ANT_Basins_IMBIE2_v1.6.shp']
@@ -310,15 +306,15 @@
             distributed_map = np.zeros((n_points),dtype=bool)
             # create empty intersection map array for receiving
             associated_map[key] = np.zeros((n_points),dtype=bool)
             # finds if points are encapsulated (within basin)
             int_test = poly_obj.intersects(xy_point)
             if int_test:
                 # extract intersected points
-                int_map = list(map(poly_obj.intersects,xy_point))
+                int_map = list(map(poly_obj.intersects, xy_point.geoms))
                 int_indices, = np.nonzero(int_map)
                 # set distributed_map indices to True for intersected points
                 distributed_map[ind[int_indices]] = True
             # communicate output MPI matrices between ranks
             # operation is a logical "or" across the elements.
             comm.Allreduce(sendbuf=[distributed_map, MPI.BOOL], \
                 recvbuf=[associated_map[key], MPI.BOOL], op=MPI.LOR)
@@ -447,15 +443,15 @@
     # parallel h5py I/O does not support compression filters at this time
     if (comm.rank == 0) and valid_check:
         # output HDF5 file with drainage basin masks
         fargs = (PRD,BASIN_TITLE,TRK,GRAN,SCYC,ECYC,RL,VERS,AUX)
         file_format = '{0}_{1}_{2}{3}_{4}{5}_{6}_{7}{8}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
         # print file information
-        logging.into(f'\t{output_file}')
+        logging.info(f'\t{output_file}')
         # write to output HDF5 file
         HDF5_ATL11_mask_write(IS2_atl11_mask, IS2_atl11_mask_attrs,
             CLOBBER=True, INPUT=os.path.basename(args.file),
             FILL_VALUE=IS2_atl11_fill, DIMENSIONS=IS2_atl11_dims,
             FILENAME=output_file)
         # change the permissions mode
         os.chmod(output_file, args.mode)
@@ -610,14 +606,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL11_grounded.py` & `icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL11_grounded.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,35 +67,31 @@
 import collections
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import shapefile
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapefile not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapefile not available", ImportWarning)
 try:
     from shapely.geometry import MultiPoint, Polygon
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapely not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapely not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # regional grounded ice files
 grounded_file = {}
 grounded_file['N'] = ['BedMachineGreenlandGroundedv4.shp']
 grounded_file['S'] = ['IceBoundaries_Antarctica_v02.shp']
@@ -309,15 +305,15 @@
             distributed_map = np.zeros((n_points),dtype=bool)
             # create empty intersection map array for receiving
             associated_map[key] = np.zeros((n_points),dtype=bool)
             # finds if points are encapsulated (within grounded ice)
             int_test = poly_obj.intersects(xy_point)
             if int_test:
                 # extract intersected points
-                int_map = list(map(poly_obj.intersects,xy_point))
+                int_map = list(map(poly_obj.intersects, xy_point.geoms))
                 int_indices, = np.nonzero(int_map)
                 # set distributed_map indices to True for intersected points
                 distributed_map[ind[int_indices]] = True
             # communicate output MPI matrices between ranks
             # operation is a logical "or" across the elements.
             comm.Allreduce(sendbuf=[distributed_map, MPI.BOOL], \
                 recvbuf=[associated_map[key], MPI.BOOL], op=MPI.LOR)
@@ -462,15 +458,15 @@
     # parallel h5py I/O does not support compression filters at this time
     if (comm.rank == 0) and valid_check:
         # output HDF5 files with grounded ice masks
         fargs = (PRD,'GROUNDED_MASK',TRK,GRAN,SCYC,ECYC,RL,VERS,AUX)
         file_format = '{0}_{1}_{2}{3}_{4}{5}_{6}_{7}{8}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
         # print file information
-        logging.into(f'\t{output_file}')
+        logging.info(f'\t{output_file}')
         # write to output HDF5 file
         HDF5_ATL11_mask_write(IS2_atl11_mask, IS2_atl11_mask_attrs,
             CLOBBER=True, INPUT=os.path.basename(args.file),
             FILL_VALUE=IS2_atl11_fill, DIMENSIONS=IS2_atl11_dims,
             FILENAME=output_file)
         # change the permissions mode
         os.chmod(output_file, args.mode)
@@ -625,14 +621,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/MPI_reduce_ICESat2_ATL11_ice_shelves.py` & `icesat2-toolkit-1.3.0/scripts/MPI_reduce_ICESat2_ATL11_ice_shelves.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,35 +65,31 @@
 import collections
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 try:
     from mpi4py import MPI
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("mpi4py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("mpi4py not available", ImportWarning)
 try:
     import shapefile
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapefile not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapefile not available", ImportWarning)
 try:
     from shapely.geometry import MultiPoint, Polygon
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("shapely not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("shapely not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # regional ice shelf files
 ice_shelf_file = {}
 ice_shelf_file['N'] = ['BedMachineGreenlandFloatingv4.shp']
 ice_shelf_file['S'] = ['IceBoundaries_Antarctica_v02.shp']
@@ -298,15 +294,15 @@
             distributed_map = np.zeros((n_points),dtype=bool)
             # create empty intersection map array for receiving
             associated_map[key] = np.zeros((n_points),dtype=bool)
             # finds if points are encapsulated (within ice shelf)
             int_test = poly_obj.intersects(xy_point)
             if int_test:
                 # extract intersected points
-                int_map = list(map(poly_obj.intersects,xy_point))
+                int_map = list(map(poly_obj.intersects, xy_point.geoms))
                 int_indices, = np.nonzero(int_map)
                 # set distributed_map indices to True for intersected points
                 distributed_map[ind[int_indices]] = True
             # communicate output MPI matrices between ranks
             # operation is a logical "or" across the elements.
             comm.Allreduce(sendbuf=[distributed_map, MPI.BOOL], \
                 recvbuf=[associated_map[key], MPI.BOOL], op=MPI.LOR)
@@ -451,15 +447,15 @@
     # parallel h5py I/O does not support compression filters at this time
     if (comm.rank == 0) and valid_check:
         # output HDF5 files with ice shelf masks
         fargs = (PRD,'ICE_SHELF_MASK',TRK,GRAN,SCYC,ECYC,RL,VERS,AUX)
         file_format = '{0}_{1}_{2}{3}_{4}{5}_{6}_{7}{8}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
         # print file information
-        logging.into(f'\t{output_file}')
+        logging.info(f'\t{output_file}')
         # write to output HDF5 file
         HDF5_ATL11_mask_write(IS2_atl11_mask, IS2_atl11_mask_attrs,
             CLOBBER=True, INPUT=os.path.basename(args.file),
             FILL_VALUE=IS2_atl11_fill, DIMENSIONS=IS2_atl11_dims,
             FILENAME=output_file)
         # change the permissions mode
         os.chmod(output_file, args.mode)
@@ -614,14 +610,13 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # run main program
 if __name__ == '__main__':
     main()
```

### Comparing `icesat2-toolkit-1.1.0/scripts/convert_ICESat2_format.py` & `icesat2-toolkit-1.3.0/scripts/convert_ICESat2_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 
 # PURPOSE: wrapper for running conversion program in multiprocessing mode
 def multiprocess_convert(hdf5_file, FORMAT=None, CHUNKS=None, CLOBBER=False,
     MODE=0o775):
     try:
         output = convert_HDF5(hdf5_file,FORMAT=FORMAT,CHUNKS=CHUNKS,
             CLOBBER=CLOBBER,MODE=MODE)
-    except Exception as e:
+    except Exception as exc:
         # if there has been an error exception
         # print the type, value, and stack trace of the
         # current exception being handled
         logging.critical(f'process id {os.getpid():d} failed')
         logging.error(traceback.format_exc())
     else:
         return output
@@ -249,15 +249,15 @@
         help='Years to run')
     # subdirectories of data to run
     parser.add_argument('--subdirectory','-S',
         type=str, nargs='+',
         help='subdirectories of data to run')
     # ICESat-2 data release
     parser.add_argument('--release','-r',
-        type=str, default='004',
+        type=str, default='006',
         help='ICESat-2 Data Release')
     # ICESat-2 data version
     parser.add_argument('--version','-v',
         type=int, nargs='+', default=range(1,10),
         help='ICESat-2 Data Version')
     # ICESat-2 granule region
     parser.add_argument('--granule','-g',
```

### Comparing `icesat2-toolkit-1.1.0/scripts/copy_scf_ICESat2_files.py` & `icesat2-toolkit-1.3.0/scripts/copy_scf_ICESat2_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     # ICESat-2 data product
     parser.add_argument('--product','-p',
         metavar='PRODUCTS', type=str,
         choices=PRODUCTS.keys(), default='ATL06',
         help='ICESat-2 data product to copy')
     # ICESat-2 data release
     parser.add_argument('--release','-r',
-        type=str, default='004',
+        type=str, default='006',
         help='ICESat-2 data release to copy')
     # ICESat-2 data version
     parser.add_argument('--version','-v',
         type=int, nargs='+', default=range(1,10),
         help='ICESat-2 data versions to copy')
     # ICESat-2 granule region
     parser.add_argument('--granule','-g',
```

### Comparing `icesat2-toolkit-1.1.0/scripts/nsidc_icesat2_associated.py` & `icesat2-toolkit-1.3.0/scripts/nsidc_icesat2_associated.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
         for out in output:
             logging.info(out.get())
 
 # PURPOSE: wrapper for running the sync program in multiprocessing mode
 def multiprocess_sync(*args, **kwds):
     try:
         output = http_pull_file(*args, **kwds)
-    except Exception as e:
+    except Exception as exc:
         # if there has been an error exception
         # print the type, value, and stack trace of the
         # current exception being handled
         logging.critical(f'process id {os.getpid():d} failed')
         logging.error(traceback.format_exc())
     else:
         return output
```

### Comparing `icesat2-toolkit-1.1.0/scripts/nsidc_icesat2_convert.py` & `icesat2-toolkit-1.3.0/scripts/nsidc_icesat2_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,15 +309,15 @@
     if LOG:
         os.chmod(os.path.join(DIRECTORY,LOGFILE), MODE)
 
 # PURPOSE: wrapper for running the sync program in multiprocessing mode
 def multiprocess_sync(*args, **kwds):
     try:
         output = http_pull_file(*args, **kwds)
-    except Exception as e:
+    except Exception as exc:
         # if there has been an error exception
         # print the type, value, and stack trace of the
         # current exception being handled
         logging.critical(f'process id {os.getpid():d} failed')
         logging.error(traceback.format_exc())
     else:
         return output
@@ -433,15 +433,15 @@
         help='Years to run')
     # subdirectories of data to run
     parser.add_argument('--subdirectory','-S',
         type=str, nargs='+',
         help='subdirectories of data to run')
     # ICESat-2 data release
     parser.add_argument('--release','-r',
-        type=str, default='004',
+        type=str, default='006',
         help='ICESat-2 Data Release')
     # ICESat-2 data version
     parser.add_argument('--version','-v',
         type=int, nargs='+', default=range(1,10),
         help='ICESat-2 Data Version')
     # ICESat-2 granule region
     parser.add_argument('--granule','-g',
```

### Comparing `icesat2-toolkit-1.1.0/scripts/nsidc_icesat2_dragann.py` & `icesat2-toolkit-1.3.0/scripts/nsidc_icesat2_dragann.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,17 +85,16 @@
 import multiprocessing as mp
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: sync ATL03 geolocated photon height products and appends the
 # ATL08 DRAGANN classifications from NSIDC
 def nsidc_icesat2_dragann(DIRECTORY, RELEASE, VERSIONS, GRANULES, TRACKS,
     YEARS=None, SUBDIRECTORY=None, CYCLES=None, FLATTEN=False,
@@ -406,15 +405,15 @@
         help='Years to run')
     # subdirectories of data to run
     parser.add_argument('--subdirectory','-S',
         type=str, nargs='+',
         help='subdirectories of data to run')
     # ICESat-2 data release
     parser.add_argument('--release','-r',
-        type=str, default='004',
+        type=str, default='006',
         help='ICESat-2 Data Release')
     # ICESat-2 data version
     parser.add_argument('--version','-v',
         type=int, nargs='+', default=range(1,10),
         help='ICESat-2 Data Version')
     # ICESat-2 granule region
     parser.add_argument('--granule','-g',
```

### Comparing `icesat2-toolkit-1.1.0/scripts/nsidc_icesat2_sync.py` & `icesat2-toolkit-1.3.0/scripts/nsidc_icesat2_sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
     if LOG:
         os.chmod(os.path.join(DIRECTORY,LOGFILE), MODE)
 
 # PURPOSE: wrapper for running the sync program in multiprocessing mode
 def multiprocess_sync(*args, **kwds):
     try:
         output = http_pull_file(*args, **kwds)
-    except Exception as e:
+    except Exception as exc:
         # if there has been an error exception
         # print the type, value, and stack trace of the
         # current exception being handled
         logging.critical(f'process id {os.getpid():d} failed')
         logging.error(traceback.format_exc())
     else:
         return output
@@ -463,15 +463,15 @@
         help='Years to sync')
     # subdirectories of data to sync
     parser.add_argument('--subdirectory','-S',
         type=str, nargs='+',
         help='subdirectories of data to sync')
     # ICESat-2 data release
     parser.add_argument('--release','-r',
-        type=str, default='004',
+        type=str, default='006',
         help='ICESat-2 Data Release')
     # ICESat-2 data version
     parser.add_argument('--version','-v',
         type=int, nargs='+', default=range(1,10),
         help='ICESat-2 Data Version')
     # ICESat-2 granule region
     region = parser.add_mutually_exclusive_group(required=False)
```

### Comparing `icesat2-toolkit-1.1.0/scripts/nsidc_icesat2_sync_s3.py` & `icesat2-toolkit-1.3.0/scripts/nsidc_icesat2_sync_s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,23 +103,32 @@
     Written 01/2019
 """
 from __future__ import print_function
 
 import sys
 import os
 import re
-import boto3
 import logging
 import argparse
+import warnings
 import posixpath
 import traceback
 import lxml.etree
 import multiprocessing as mp
 import icesat2_toolkit as is2tk
 
+# attempt imports
+try:
+    import boto3
+except (ImportError, ModuleNotFoundError) as exc:
+    warnings.filterwarnings("module")
+    warnings.warn("boto3 not available", ImportWarning)
+# ignore warnings
+warnings.filterwarnings("ignore")
+
 # PURPOSE: sync the ICESat-2 elevation data from NSIDC
 def nsidc_icesat2_sync_s3(aws_access_key_id, aws_secret_access_key,
     aws_region_name, s3_bucket_name, s3_bucket_path,
     PRODUCTS, RELEASE, VERSIONS, GRANULES, TRACKS,
     YEARS=None, SUBDIRECTORY=None, CYCLES=None, REGION=None,
     AUXILIARY=False, INDEX=None, FLATTEN=False, TIMEOUT=None,
     RETRY=1, PROCESSES=0, CLOBBER=False):
@@ -307,15 +316,15 @@
             temp = output.get()
             logging.info(temp) if temp else None
 
 # PURPOSE: wrapper for running the sync program in multiprocessing mode
 def multiprocess_sync(*args, **kwds):
     try:
         output = http_pull_file(*args, **kwds)
-    except Exception as e:
+    except Exception as exc:
         # if there has been an error exception
         # print the type, value, and stack trace of the
         # current exception being handled
         logging.critical(f'process id {os.getpid():d} failed')
         logging.error(traceback.format_exc())
     else:
         return output
@@ -427,15 +436,15 @@
         help='Years to sync')
     # subdirectories of data to sync
     parser.add_argument('--subdirectory','-S',
         type=str, nargs='+',
         help='subdirectories of data to sync')
     # ICESat-2 data release
     parser.add_argument('--release','-r',
-        type=str, default='004',
+        type=str, default='006',
         help='ICESat-2 Data Release')
     # ICESat-2 data version
     parser.add_argument('--version','-v',
         type=int, nargs='+', default=range(1,10),
         help='ICESat-2 Data Version')
     # ICESat-2 granule region
     region = parser.add_mutually_exclusive_group(required=False)
```

### Comparing `icesat2-toolkit-1.1.0/scripts/reduce_ICESat2_ATL06_raster.py` & `icesat2-toolkit-1.3.0/scripts/reduce_ICESat2_ATL06_raster.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,17 +65,16 @@
 import scipy.interpolate
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: try to get the projection information for the input file
 def get_projection(attributes, PROJECTION):
     # coordinate reference system string from file
     try:
@@ -385,15 +384,15 @@
     if OUTPUT:
         output_file = os.path.expanduser(OUTPUT)
     else:
         fargs = (PRD,'MASK',YY,MM,DD,HH,MN,SS,TRK,CYCL,GRAN,RL,VERS,AUX)
         file_format = '{0}_{1}_{2}{3}{4}{5}{6}{7}_{8}{9}{10}_{11}_{12}{13}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
     # print file information
-    logging.into(f'\t{output_file}')
+    logging.info(f'\t{output_file}')
     # write to output HDF5 file
     HDF5_ATL06_mask_write(IS2_atl06_mask, IS2_atl06_mask_attrs,
         CLOBBER=True, INPUT=os.path.basename(FILE),
         FILL_VALUE=IS2_atl06_fill, DIMENSIONS=IS2_atl06_dims,
         FILENAME=output_file)
     # change the permissions mode
     os.chmod(output_file, MODE)
@@ -438,23 +437,22 @@
         fileID[gtx].create_group('land_ice_segments')
         h5[gtx] = dict(land_ice_segments={})
         for att_name in ['Description','data_rate']:
             att_val = IS2_atl06_attrs[gtx]['land_ice_segments'][att_name]
             fileID[gtx]['land_ice_segments'].attrs[att_name] = att_val
 
         # segment_id, geolocation, time and height variables
-        for k in ['segment_id','latitude','longitude','delta_time']:
+        for k in ['delta_time','segment_id','latitude','longitude']:
             # values and attributes
             v = IS2_atl06_mask[gtx]['land_ice_segments'][k]
             attrs = IS2_atl06_attrs[gtx]['land_ice_segments'][k]
             fillvalue = FILL_VALUE[gtx]['land_ice_segments'][k]
             # Defining the HDF5 dataset variables
             val = '{0}/{1}/{2}'.format(gtx,'land_ice_segments',k)
             if fillvalue:
-                print(k)
                 h5[gtx]['land_ice_segments'][k] = fileID.create_dataset(val,
                     np.shape(v), data=v, dtype=v.dtype, fillvalue=fillvalue,
                     compression='gzip')
             else:
                 h5[gtx]['land_ice_segments'][k] = fileID.create_dataset(val,
                     np.shape(v), data=v, dtype=v.dtype, compression='gzip')
             # create or attach dimensions for HDF5 variable
@@ -556,15 +554,14 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Create masks for reducing ICESat-2 data
```

### Comparing `icesat2-toolkit-1.1.0/scripts/reduce_ICESat2_ATL07_raster.py` & `icesat2-toolkit-1.3.0/scripts/reduce_ICESat2_ATL07_raster.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,17 +65,16 @@
 import scipy.interpolate
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: try to get the projection information for the input file
 def get_projection(attributes, PROJECTION):
     # coordinate reference system string from file
     try:
@@ -416,15 +415,15 @@
     if OUTPUT:
         output_file = os.path.expanduser(OUTPUT)
     else:
         fargs = (PRD,HMN,'MASK',YY,MM,DD,HH,MN,SS,TRK,CYCL,SN,RL,VERS,AUX)
         file_format = '{0}-{1}_{2}_{3}{4}{5}{6}{7}{8}_{9}{10}{11}_{12}_{13}{14}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
     # print file information
-    logging.into(f'\t{output_file}')
+    logging.info(f'\t{output_file}')
     # write to output HDF5 file
     HDF5_ATL07_mask_write(IS2_atl07_mask, IS2_atl07_mask_attrs,
         CLOBBER=True, INPUT=os.path.basename(FILE),
         FILL_VALUE=IS2_atl07_fill, DIMENSIONS=IS2_atl07_dims,
         FILENAME=output_file)
     # change the permissions mode
     os.chmod(output_file, MODE)
@@ -595,15 +594,14 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
```

### Comparing `icesat2-toolkit-1.1.0/scripts/reduce_ICESat2_ATL10_raster.py` & `icesat2-toolkit-1.3.0/scripts/reduce_ICESat2_ATL10_raster.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,17 +65,16 @@
 import scipy.interpolate
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: try to get the projection information for the input file
 def get_projection(attributes, PROJECTION):
     # coordinate reference system string from file
     try:
@@ -375,15 +374,15 @@
     if OUTPUT:
         output_file = os.path.expanduser(OUTPUT)
     else:
         fargs = (PRD,HMN,'MASK',YY,MM,DD,HH,MN,SS,TRK,CYCL,SN,RL,VERS,AUX)
         file_format = '{0}-{1}_{2}_{3}{4}{5}{6}{7}{8}_{9}{10}{11}_{12}_{13}{14}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
     # print file information
-    logging.into(f'\t{output_file}')
+    logging.info(f'\t{output_file}')
     # write to output HDF5 file
     HDF5_ATL10_mask_write(IS2_atl10_mask, IS2_atl10_mask_attrs,
         CLOBBER=True, INPUT=os.path.basename(FILE),
         FILL_VALUE=IS2_atl10_fill, DIMENSIONS=IS2_atl10_dims,
         FILENAME=output_file)
     # change the permissions mode
     os.chmod(output_file, MODE)
@@ -555,15 +554,14 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Create masks for reducing ICESat-2 data
```

### Comparing `icesat2-toolkit-1.1.0/scripts/reduce_ICESat2_ATL11_raster.py` & `icesat2-toolkit-1.3.0/scripts/reduce_ICESat2_ATL11_raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,16 @@
 import scipy.interpolate
 import icesat2_toolkit as is2tk
 
 # attempt imports
 try:
     import h5py
 except ModuleNotFoundError:
-    warnings.filterwarnings("always")
-    warnings.warn("h5py not available")
-    warnings.warn("Some functions will throw an exception if called")
+    warnings.filterwarnings("module")
+    warnings.warn("h5py not available", ImportWarning)
 # ignore warnings
 warnings.filterwarnings("ignore")
 
 # PURPOSE: try to get the projection information for the input file
 def get_projection(attributes, PROJECTION):
     # coordinate reference system string from file
     try:
@@ -397,15 +396,15 @@
     if OUTPUT:
         output_file = os.path.expanduser(OUTPUT)
     else:
         fargs = (PRD,'MASK',TRK,GRAN,SCYC,ECYC,RL,VERS,AUX)
         file_format = '{0}_{1}_{2}{3}_{4}{5}_{6}_{7}{8}.h5'
         output_file = os.path.join(DIRECTORY,file_format.format(*fargs))
     # print file information
-    logging.into(f'\t{output_file}')
+    logging.info(f'\t{output_file}')
     # write to output HDF5 file
     HDF5_ATL11_mask_write(IS2_atl11_mask, IS2_atl11_mask_attrs,
         CLOBBER=True, INPUT=os.path.basename(FILE),
         FILL_VALUE=IS2_atl11_fill, DIMENSIONS=IS2_atl11_dims,
         FILENAME=output_file)
     # change the permissions mode
     os.chmod(output_file, MODE)
@@ -558,15 +557,14 @@
     tce = datetime.datetime(int(YY[1]), int(MM[1]), int(DD[1]),
         int(HH[1]), int(MN[1]), int(SS[1]), int(1e6*(SS[1] % 1)))
     fileID.attrs['time_coverage_end'] = tce.isoformat()
     fileID.attrs['time_coverage_duration'] = f'{tmx-tmn:0.0f}'
     # add software information
     fileID.attrs['software_reference'] = is2tk.version.project_name
     fileID.attrs['software_version'] = is2tk.version.full_version
-    fileID.attrs['software_revision'] = is2tk.utilities.get_git_revision_hash()
     # Closing the HDF5 file
     fileID.close()
 
 # PURPOSE: create argument parser
 def arguments():
     parser = argparse.ArgumentParser(
         description="""Create masks for reducing ICESat-2 ATL11 annual land
```

### Comparing `icesat2-toolkit-1.1.0/scripts/scp_ICESat2_files.py` & `icesat2-toolkit-1.3.0/scripts/scp_ICESat2_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
     # ICESat-2 data product
     parser.add_argument('--product','-p',
         metavar='PRODUCTS', type=str,
         choices=PRODUCTS.keys(), default='ATL06',
         help='ICESat-2 data product to copy')
     # ICESat-2 data release
     parser.add_argument('--release','-r',
-        type=str, default='004',
+        type=str, default='006',
         help='ICESat-2 data release to copy')
     # ICESat-2 data version
     parser.add_argument('--version','-v',
         type=int, nargs='+', default=range(1,10),
         help='ICESat-2 data versions to copy')
     # ICESat-2 granule region
     parser.add_argument('--granule','-g',
```

### Comparing `icesat2-toolkit-1.1.0/scripts/scp_scf_ICESat2_files.py` & `icesat2-toolkit-1.3.0/scripts/scp_scf_ICESat2_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
     # ICESat-2 data product
     parser.add_argument('--product','-p',
         metavar='PRODUCTS', type=str,
         choices=PRODUCTS.keys(), default='ATL06',
         help='ICESat-2 data product to copy')
     # ICESat-2 data release
     parser.add_argument('--release','-r',
-        type=str, default='004',
+        type=str, default='006',
         help='ICESat-2 data release to copy')
     # ICESat-2 data version
     parser.add_argument('--version','-v',
         type=int, nargs='+', default=range(1,10),
         help='ICESat-2 data versions to copy')
     # ICESat-2 granule region
     parser.add_argument('--granule','-g',
```

### Comparing `icesat2-toolkit-1.1.0/scripts/symbolic_ICESat2_files.py` & `icesat2-toolkit-1.3.0/scripts/symbolic_ICESat2_files.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     # ICESat-2 data product
     parser.add_argument('--product','-p',
         metavar='PRODUCTS', type=str,
         choices=PRODUCTS.keys(), default='ATL06',
         help='ICESat-2 data product to create symbolic links')
     # ICESat-2 data release
     parser.add_argument('--release','-r',
-        type=str, default='004',
+        type=str, default='006',
         help='ICESat-2 data release to create symbolic links')
     # ICESat-2 data version
     parser.add_argument('--version','-v',
         type=int, nargs='+', default=range(1,10),
         help='ICESat-2 data versions to create symbolic links')
     # ICESat-2 granule region
     parser.add_argument('--granule','-g',
```

### Comparing `icesat2-toolkit-1.1.0/setup.py` & `icesat2-toolkit-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `icesat2-toolkit-1.1.0/test/test_download_and_read.py` & `icesat2-toolkit-1.3.0/test/test_download_and_read.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,168 +1,169 @@
 #!/usr/bin/env python
 u"""
-test_download_and_read.py (08/2022)
+test_download_and_read.py (03/2023)
 
 UPDATE HISTORY:
+    Updated 03/2023: replace deprecated functions with new io functions
     Updated 08/2022: added backup AWS access to files
     Updated 02/2022: add CMR query tests for cycles, tracks and granules
     Updated 01/2022: update data releases for all products
     Updated 03/2021: modify ATL11 to read from explicitly named groups
     Updated 11/2020: use output error string returned by from_nsidc
     Written 08/2020
 """
-import warnings
 import pytest
 import posixpath
-import icesat2_toolkit.utilities
-from icesat2_toolkit.read_ICESat2_ATL03 import read_HDF5_ATL03
-from icesat2_toolkit.read_ICESat2_ATL06 import read_HDF5_ATL06
-from icesat2_toolkit.read_ICESat2_ATL07 import read_HDF5_ATL07
-from icesat2_toolkit.read_ICESat2_ATL11 import read_HDF5_ATL11
-from icesat2_toolkit.read_ICESat2_ATL12 import read_HDF5_ATL12
+import icesat2_toolkit as is2tk
 
 # PURPOSE: Download an ATL03 file from NSIDC and check that read program runs
 def test_ATL03_download_and_read(username,password):
     HOST = ['https://n5eil01u.ecs.nsidc.org','ATLAS','ATL03.005','2018.10.14',
         'ATL03_20181014000347_02350101_005_01.h5']
-    buffer, error = icesat2_toolkit.utilities.from_nsidc(HOST,
+    buffer, error = is2tk.utilities.from_nsidc(HOST,
         username=username, password=password,
         local=HOST[-1], verbose=True)
     # attempt download from AWS
     if not buffer:
-        url = posixpath.dirname(icesat2_toolkit.utilities._s3_endpoints['nsidc'])
-        bucket = icesat2_toolkit.utilities._s3_buckets['nsidc']
-        key = icesat2_toolkit.utilities.s3_key(posixpath.join(*HOST))
-        buffer, error = icesat2_toolkit.utilities.from_nsidc([url,bucket,key],
+        url = posixpath.dirname(is2tk.utilities._s3_endpoints['nsidc'])
+        bucket = is2tk.utilities._s3_buckets['nsidc']
+        key = is2tk.utilities.s3_key(posixpath.join(*HOST))
+        buffer, error = is2tk.utilities.from_nsidc([url,bucket,key],
             username=username, password=password, local=HOST[-1],
             verbose=True)
     # raise exception if download error
     if not buffer:
         raise Exception(error)
     # read ATL03 data from downloaded HDF5 file
-    IS2_atl03_mds,IS2_atl03_attrs,IS2_atl03_beams = read_HDF5_ATL03(HOST[-1],
-        ATTRIBUTES=False, VERBOSE=True)
-    assert all(gtx in IS2_atl03_mds.keys() for gtx in IS2_atl03_beams)
+    mds,attrs,beams = is2tk.io.ATL03.read_granule(HOST[-1],
+        ATTRIBUTES=False,
+        VERBOSE=True
+    )
+    assert all(gtx in mds.keys() for gtx in beams)
 
 # PURPOSE: Download an ATL06 file from NSIDC and check that read program runs
 def test_ATL06_download_and_read(username,password):
     HOST = ['https://n5eil01u.ecs.nsidc.org','ATLAS','ATL06.005','2018.10.14',
         'ATL06_20181014001049_02350102_005_01.h5']
-    buffer, error = icesat2_toolkit.utilities.from_nsidc(HOST,
+    buffer, error = is2tk.utilities.from_nsidc(HOST,
         username=username, password=password,
         local=HOST[-1], verbose=True)
     # attempt download from AWS
     if not buffer:
-        url = posixpath.dirname(icesat2_toolkit.utilities._s3_endpoints['nsidc'])
-        bucket = icesat2_toolkit.utilities._s3_buckets['nsidc']
-        key = icesat2_toolkit.utilities.s3_key(posixpath.join(*HOST))
-        buffer, error = icesat2_toolkit.utilities.from_nsidc([url,bucket,key],
+        url = posixpath.dirname(is2tk.utilities._s3_endpoints['nsidc'])
+        bucket = is2tk.utilities._s3_buckets['nsidc']
+        key = is2tk.utilities.s3_key(posixpath.join(*HOST))
+        buffer, error = is2tk.utilities.from_nsidc([url,bucket,key],
             username=username, password=password, local=HOST[-1],
             verbose=True)
     # raise exception if download error
     if not buffer:
         raise Exception(error)
     # read ATL06 data from downloaded HDF5 file
-    IS2_atl06_mds,IS2_atl06_attrs,IS2_atl06_beams = read_HDF5_ATL06(HOST[-1],
-        ATTRIBUTES=False, HISTOGRAM=False, QUALITY=False, VERBOSE=True)
-    assert all(gtx in IS2_atl06_mds.keys() for gtx in IS2_atl06_beams)
+    mds,attrs,beams = is2tk.io.ATL06.read_granule(HOST[-1],
+        ATTRIBUTES=False,
+        HISTOGRAM=False,
+        QUALITY=False,
+        VERBOSE=True
+    )
+    assert all(gtx in mds.keys() for gtx in beams)
 
 # PURPOSE: Download an ATL07 file from NSIDC and check that read program runs
 def test_ATL07_download_and_read(username,password):
     HOST = ['https://n5eil01u.ecs.nsidc.org','ATLAS','ATL07.005','2018.10.14',
         'ATL07-01_20181014000347_02350101_005_03.h5']
-    buffer, error = icesat2_toolkit.utilities.from_nsidc(HOST,
+    buffer, error = is2tk.utilities.from_nsidc(HOST,
         username=username, password=password,
         local=HOST[-1], verbose=True)
     # attempt download from AWS
     if not buffer:
-        url = posixpath.dirname(icesat2_toolkit.utilities._s3_endpoints['nsidc'])
-        bucket = icesat2_toolkit.utilities._s3_buckets['nsidc']
-        key = icesat2_toolkit.utilities.s3_key(posixpath.join(*HOST))
-        buffer, error = icesat2_toolkit.utilities.from_nsidc([url,bucket,key],
+        url = posixpath.dirname(is2tk.utilities._s3_endpoints['nsidc'])
+        bucket = is2tk.utilities._s3_buckets['nsidc']
+        key = is2tk.utilities.s3_key(posixpath.join(*HOST))
+        buffer, error = is2tk.utilities.from_nsidc([url,bucket,key],
             username=username, password=password, local=HOST[-1],
             verbose=True)
     # raise exception if download error
     if not buffer:
         raise Exception(error)
     # read ATL07 data from downloaded HDF5 file
-    IS2_ATL07_mds,IS2_ATL07_attrs,IS2_ATL07_beams = read_HDF5_ATL07(HOST[-1],
+    mds,attrs,beams = is2tk.io.ATL07.read_granule(HOST[-1],
         ATTRIBUTES=False, VERBOSE=True)
-    assert all(gtx in IS2_ATL07_mds.keys() for gtx in IS2_ATL07_beams)
+    assert all(gtx in mds.keys() for gtx in beams)
 
 # PURPOSE: Download an ATL11 file from NSIDC and check that read program runs
 def test_ATL11_download_and_read(username,password):
     # attempt download from on-prem NSIDC
     HOST = ['https://n5eil01u.ecs.nsidc.org','ATLAS','ATL11.005','2019.03.29',
         'ATL11_000103_0315_005_03.h5']
-    buffer, error = icesat2_toolkit.utilities.from_nsidc(HOST,
+    buffer, error = is2tk.utilities.from_nsidc(HOST,
         username=username, password=password,
         local=HOST[-1], verbose=True)
     # attempt download from AWS
     if not buffer:
-        url = posixpath.dirname(icesat2_toolkit.utilities._s3_endpoints['nsidc'])
-        bucket = icesat2_toolkit.utilities._s3_buckets['nsidc']
-        key = icesat2_toolkit.utilities.s3_key(posixpath.join(*HOST))
-        buffer, error = icesat2_toolkit.utilities.from_nsidc([url,bucket,key],
+        url = posixpath.dirname(is2tk.utilities._s3_endpoints['nsidc'])
+        bucket = is2tk.utilities._s3_buckets['nsidc']
+        key = is2tk.utilities.s3_key(posixpath.join(*HOST))
+        buffer, error = is2tk.utilities.from_nsidc([url,bucket,key],
             username=username, password=password, local=HOST[-1],
             verbose=True)
     # raise exception if download error
     if not buffer:
         raise Exception(error)
     # read ATL12 data from downloaded HDF5 file
     GROUPS = ['cycle_stats','ref_surf','crossing_track_data']
-    IS2_ATL11_mds,IS2_ATL11_attrs,IS2_ATL11_pairs = read_HDF5_ATL11(HOST[-1],
+    mds,attrs,pairs = is2tk.io.ATL11.read_granule(HOST[-1],
         ATTRIBUTES=False, GROUPS=GROUPS, VERBOSE=True)
-    assert all(ptx in IS2_ATL11_mds.keys() for ptx in IS2_ATL11_pairs)
-    ptx = IS2_ATL11_pairs[0]
-    assert all(group in IS2_ATL11_mds[ptx].keys() for group in GROUPS)
+    assert all(ptx in mds.keys() for ptx in pairs)
+    ptx = pairs[0]
+    assert all(group in mds[ptx].keys() for group in GROUPS)
 
 # PURPOSE: Download an ATL12 file from NSIDC and check that read program runs
 def test_ATL12_download_and_read(username,password):
     HOST = ['https://n5eil01u.ecs.nsidc.org','ATLAS','ATL12.005','2018.10.14',
         'ATL12_20181014031222_02370101_005_02.h5']
-    buffer, error = icesat2_toolkit.utilities.from_nsidc(HOST,
+    buffer, error = is2tk.utilities.from_nsidc(HOST,
         username=username, password=password,
         local=HOST[-1], verbose=True)
     # attempt download from AWS
     if not buffer:
-        url = posixpath.dirname(icesat2_toolkit.utilities._s3_endpoints['nsidc'])
-        bucket = icesat2_toolkit.utilities._s3_buckets['nsidc']
-        key = icesat2_toolkit.utilities.s3_key(posixpath.join(*HOST))
-        buffer, error = icesat2_toolkit.utilities.from_nsidc([url,bucket,key],
+        url = posixpath.dirname(is2tk.utilities._s3_endpoints['nsidc'])
+        bucket = is2tk.utilities._s3_buckets['nsidc']
+        key = is2tk.utilities.s3_key(posixpath.join(*HOST))
+        buffer, error = is2tk.utilities.from_nsidc([url,bucket,key],
             username=username, password=password, local=HOST[-1],
             verbose=True)
     # raise exception if download error
     if not buffer:
         raise Exception(error)
     # read ATL12 data from downloaded HDF5 file
-    IS2_ATL12_mds,IS2_ATL12_attrs,IS2_ATL12_beams = read_HDF5_ATL12(HOST[-1],
+    mds,attrs,beams = is2tk.io.ATL12.read_granule(HOST[-1],
         ATTRIBUTES=False, VERBOSE=True)
-    assert all(gtx in IS2_ATL12_mds.keys() for gtx in IS2_ATL12_beams)
+    assert all(gtx in mds.keys() for gtx in beams)
 
 # PURPOSE: test CMR queries for specific cycles
 def test_cmr_query_cycles():
-    ids,urls = icesat2_toolkit.utilities.cmr(product='ATL06',
+    ids,urls = is2tk.utilities.cmr(product='ATL06',
         release='005',cycles=[2,3],tracks=752,granules=10,
         verbose=False)
     valid = ['ATL06_20190215171140_07520210_005_01.h5',
         'ATL06_20190517125119_07520310_005_01.h5']
     assert all(id in valid for id in ids)
 
 # PURPOSE: test CMR queries for specific tracks
 def test_cmr_query_tracks():
-    ids,urls = icesat2_toolkit.utilities.cmr(product='ATL06',
+    ids,urls = is2tk.utilities.cmr(product='ATL06',
         release='005',cycles=2,tracks=[752,753],granules=10,
         verbose=False)
     valid = ['ATL06_20190215171140_07520210_005_01.h5',
         'ATL06_20190215184558_07530210_005_01.h5']
     assert all(id in valid for id in ids)
 
 # PURPOSE: test CMR queries for specific granules
 def test_cmr_query_granules():
-    ids,urls = icesat2_toolkit.utilities.cmr(product='ATL06',
+    ids,urls = is2tk.utilities.cmr(product='ATL06',
         release='005',cycles=2,tracks=752,granules=[10,11,12],
         verbose=False)
     valid = ['ATL06_20190215171140_07520210_005_01.h5',
         'ATL06_20190215171921_07520211_005_01.h5',
         'ATL06_20190215172504_07520212_005_01.h5']
     assert all(id in valid for id in ids)
```

### Comparing `icesat2-toolkit-1.1.0/test/test_leap_seconds.py` & `icesat2-toolkit-1.3.0/test/test_leap_seconds.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 u"""
 test_leap_seconds.py (08/2020)
 """
 import os
 import pytest
-import warnings
 import icesat2_toolkit.time
 import icesat2_toolkit.utilities
 
 # PURPOSE: Define GPS leap seconds
 def get_leaps():
     """
     Gets a list of GPS times for when leap seconds occurred
```

### Comparing `icesat2-toolkit-1.1.0/test/test_time.py` & `icesat2-toolkit-1.3.0/test/test_time.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python
 u"""
 test_time.py (08/2020)
 Verify time conversion functions
 """
 import pytest
-import warnings
 import numpy as np
 import icesat2_toolkit.time
 
 # parameterize calendar dates
 @pytest.mark.parametrize("YEAR", np.random.randint(1992,2020,size=2))
 @pytest.mark.parametrize("MONTH", np.random.randint(1,13,size=2))
 # PURPOSE: verify forward and backwards time conversions
```

