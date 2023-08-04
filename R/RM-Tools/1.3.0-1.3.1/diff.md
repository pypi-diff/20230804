# Comparing `tmp/RM-Tools-1.3.0.tar.gz` & `tmp/RM-Tools-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/RM-Tools-1.3.0.tar", last modified: Wed Dec 21 00:26:50 2022, max compression
+gzip compressed data, was "dist/RM-Tools-1.3.1.tar", last modified: Fri Aug  4 06:31:00 2023, max compression
```

## Comparing `RM-Tools-1.3.0.tar` & `RM-Tools-1.3.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2022-12-21 00:26:50.432704 RM-Tools-1.3.0/
--rw-r--r--   0 cvaneck    (503) staff       (20)     1106 2020-07-23 17:47:25.000000 RM-Tools-1.3.0/LICENSE.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)      162 2021-04-26 15:31:37.000000 RM-Tools-1.3.0/MANIFEST.in
--rw-r--r--   0 cvaneck    (503) staff       (20)     3361 2022-12-21 00:26:50.432317 RM-Tools-1.3.0/PKG-INFO
--rw-r--r--   0 cvaneck    (503) staff       (20)     2085 2022-12-19 02:59:13.000000 RM-Tools-1.3.0/README.md
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2022-12-21 00:26:50.259507 RM-Tools-1.3.0/RM_Tools.egg-info/
--rw-r--r--   0 cvaneck    (503) staff       (20)     3361 2022-12-21 00:26:49.000000 RM-Tools-1.3.0/RM_Tools.egg-info/PKG-INFO
--rw-r--r--   0 cvaneck    (503) staff       (20)     1901 2022-12-21 00:26:50.000000 RM-Tools-1.3.0/RM_Tools.egg-info/SOURCES.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)        1 2022-12-21 00:26:49.000000 RM-Tools-1.3.0/RM_Tools.egg-info/dependency_links.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)      872 2022-12-21 00:26:49.000000 RM-Tools-1.3.0/RM_Tools.egg-info/entry_points.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)       92 2022-12-21 00:26:49.000000 RM-Tools-1.3.0/RM_Tools.egg-info/requires.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)       30 2022-12-21 00:26:49.000000 RM-Tools-1.3.0/RM_Tools.egg-info/top_level.txt
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2022-12-21 00:26:50.305672 RM-Tools-1.3.0/RMtools_1D/
--rw-r--r--   0 cvaneck    (503) staff       (20)     1593 2019-12-19 15:46:49.000000 RM-Tools-1.3.0/RMtools_1D/README.txt
--rw-r--r--   0 cvaneck    (503) staff       (20)        0 2019-08-02 13:47:51.000000 RM-Tools-1.3.0/RMtools_1D/__init__.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)     9211 2021-09-16 23:55:03.000000 RM-Tools-1.3.0/RMtools_1D/calculate_RMSF.py
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2022-12-21 00:26:50.315675 RM-Tools-1.3.0/RMtools_1D/cats/
--rw-r--r--   0 cvaneck    (503) staff       (20)     2528 2019-05-13 17:33:13.000000 RM-Tools-1.3.0/RMtools_1D/cats/catComplex.csv
--rw-r--r--   0 cvaneck    (503) staff       (20)     5692 2019-05-13 17:33:13.000000 RM-Tools-1.3.0/RMtools_1D/cats/cat_simple_doQUfit.bat
--rw-r--r--   0 cvaneck    (503) staff       (20)     2104 2019-05-13 17:33:13.000000 RM-Tools-1.3.0/RMtools_1D/cats/catalogue.csv
--rw-r--r--   0 cvaneck    (503) staff       (20)     2825 2019-05-13 17:33:13.000000 RM-Tools-1.3.0/RMtools_1D/cats/catalogue1.csv
--rw-r--r--   0 cvaneck    (503) staff       (20)    10670 2019-05-13 17:33:13.000000 RM-Tools-1.3.0/RMtools_1D/cats/testCat.dat
--rwxr-xr-x   0 cvaneck    (503) staff       (20)     4955 2022-07-04 18:23:39.000000 RM-Tools-1.3.0/RMtools_1D/clean_model.py
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2022-12-21 00:26:50.357902 RM-Tools-1.3.0/RMtools_1D/data/
--rw-r--r--   0 cvaneck    (503) staff       (20)    50612 2020-09-17 20:30:02.000000 RM-Tools-1.3.0/RMtools_1D/data/Source1.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)   140348 2022-12-12 07:27:14.000000 RM-Tools-1.3.0/RMtools_1D/data/Source1_FDFdirty.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)   115502 2022-12-12 07:27:14.000000 RM-Tools-1.3.0/RMtools_1D/data/Source1_RMSF-dirtyFDF-plots.pdf
--rw-r--r--   0 cvaneck    (503) staff       (20)   280809 2022-12-12 07:27:14.000000 RM-Tools-1.3.0/RMtools_1D/data/Source1_RMSF.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)     1730 2022-12-12 07:27:14.000000 RM-Tools-1.3.0/RMtools_1D/data/Source1_RMsynth.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)     1950 2022-12-12 07:27:14.000000 RM-Tools-1.3.0/RMtools_1D/data/Source1_RMsynth.json
--rw-r--r--   0 cvaneck    (503) staff       (20)   136375 2022-12-12 07:27:13.000000 RM-Tools-1.3.0/RMtools_1D/data/Source1_spectra-plots.pdf
--rw-r--r--   0 cvaneck    (503) staff       (20)    14400 2022-12-12 07:27:14.000000 RM-Tools-1.3.0/RMtools_1D/data/Source1_weight.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50728 2020-09-17 20:30:02.000000 RM-Tools-1.3.0/RMtools_1D/data/Source2.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50710 2020-09-17 20:30:02.000000 RM-Tools-1.3.0/RMtools_1D/data/Source3.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50677 2020-09-17 20:30:02.000000 RM-Tools-1.3.0/RMtools_1D/data/Source4.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50670 2020-09-17 20:30:02.000000 RM-Tools-1.3.0/RMtools_1D/data/Source5.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50727 2020-09-17 20:30:02.000000 RM-Tools-1.3.0/RMtools_1D/data/Source6.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50687 2020-09-17 20:30:02.000000 RM-Tools-1.3.0/RMtools_1D/data/Source7.dat
--rw-r--r--   0 cvaneck    (503) staff       (20)    50589 2020-09-17 20:30:02.000000 RM-Tools-1.3.0/RMtools_1D/data/Source8.dat
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    25632 2022-12-20 05:11:00.000000 RM-Tools-1.3.0/RMtools_1D/do_QUfit_1D_mnest.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    21451 2022-12-19 02:59:13.000000 RM-Tools-1.3.0/RMtools_1D/do_RMclean_1D.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    31059 2022-12-20 05:11:00.000000 RM-Tools-1.3.0/RMtools_1D/do_RMsynth_1D.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     9936 2021-02-16 16:05:49.000000 RM-Tools-1.3.0/RMtools_1D/do_RMsynth_1D_fromFITS.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    16089 2019-09-12 18:37:00.000000 RM-Tools-1.3.0/RMtools_1D/mk_test_ascii_data.py
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2022-12-21 00:26:50.374238 RM-Tools-1.3.0/RMtools_1D/models_ns/
--rw-r--r--   0 cvaneck    (503) staff       (20)       38 2019-05-13 17:33:13.000000 RM-Tools-1.3.0/RMtools_1D/models_ns/__init__.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     2038 2022-12-19 02:59:13.000000 RM-Tools-1.3.0/RMtools_1D/models_ns/m1.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     3854 2022-12-19 02:59:13.000000 RM-Tools-1.3.0/RMtools_1D/models_ns/m11.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     2365 2022-12-19 02:59:13.000000 RM-Tools-1.3.0/RMtools_1D/models_ns/m2.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     4069 2022-12-19 02:59:13.000000 RM-Tools-1.3.0/RMtools_1D/models_ns/m3.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     4420 2022-12-19 02:59:13.000000 RM-Tools-1.3.0/RMtools_1D/models_ns/m4.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    56826 2022-12-19 02:59:23.000000 RM-Tools-1.3.0/RMtools_1D/rmtools_bwdepol.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     7892 2022-12-19 02:59:23.000000 RM-Tools-1.3.0/RMtools_1D/rmtools_bwpredict.py
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2022-12-21 00:26:50.401484 RM-Tools-1.3.0/RMtools_3D/
--rw-r--r--   0 cvaneck    (503) staff       (20)     1239 2019-12-19 15:46:49.000000 RM-Tools-1.3.0/RMtools_3D/README.txt
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    15414 2022-12-21 00:11:19.000000 RM-Tools-1.3.0/RMtools_3D/RMpeakfit_3D.py
--rw-r--r--   0 cvaneck    (503) staff       (20)        0 2019-08-02 13:47:51.000000 RM-Tools-1.3.0/RMtools_3D/__init__.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     4623 2020-12-04 15:25:12.000000 RM-Tools-1.3.0/RMtools_3D/assemble_chunks.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     4053 2019-05-30 19:24:18.000000 RM-Tools-1.3.0/RMtools_3D/create_chunks.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    20350 2022-12-19 02:59:13.000000 RM-Tools-1.3.0/RMtools_3D/do_RMclean_3D.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    29337 2021-08-09 15:11:30.000000 RM-Tools-1.3.0/RMtools_3D/do_RMsynth_3D.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    17070 2022-12-19 02:59:13.000000 RM-Tools-1.3.0/RMtools_3D/do_fitIcube.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     5503 2020-06-08 13:35:35.000000 RM-Tools-1.3.0/RMtools_3D/extract_region.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     1804 2022-12-19 02:59:13.000000 RM-Tools-1.3.0/RMtools_3D/make_freq_file.py
--rwxr-xr-x   0 cvaneck    (503) staff       (20)    19473 2022-12-13 23:02:25.000000 RM-Tools-1.3.0/RMtools_3D/mk_test_cube_data.py
-drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2022-12-21 00:26:50.431640 RM-Tools-1.3.0/RMutils/
--rw-r--r--   0 cvaneck    (503) staff       (20)      251 2019-05-13 17:33:13.000000 RM-Tools-1.3.0/RMutils/__init__.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    22901 2019-05-13 17:33:13.000000 RM-Tools-1.3.0/RMutils/corner.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    78840 2019-05-13 17:33:13.000000 RM-Tools-1.3.0/RMutils/mpfit.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    36212 2019-05-13 17:33:13.000000 RM-Tools-1.3.0/RMutils/nestle.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     4842 2019-05-13 17:33:13.000000 RM-Tools-1.3.0/RMutils/normalize.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    17314 2019-05-13 17:33:13.000000 RM-Tools-1.3.0/RMutils/util_FITS.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    86423 2022-12-19 02:59:13.000000 RM-Tools-1.3.0/RMutils/util_RM.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    40930 2022-12-19 04:18:34.000000 RM-Tools-1.3.0/RMutils/util_misc.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    10191 2021-02-02 21:24:43.000000 RM-Tools-1.3.0/RMutils/util_plotFITS.py
--rw-r--r--   0 cvaneck    (503) staff       (20)    78650 2022-12-19 02:59:13.000000 RM-Tools-1.3.0/RMutils/util_plotTk.py
--rw-r--r--   0 cvaneck    (503) staff       (20)     4619 2019-05-13 17:33:13.000000 RM-Tools-1.3.0/RMutils/util_rec.py
--rw-r--r--   0 cvaneck    (503) staff       (20)       38 2022-12-21 00:26:50.432784 RM-Tools-1.3.0/setup.cfg
--rw-r--r--   0 cvaneck    (503) staff       (20)     3183 2022-12-20 05:11:00.000000 RM-Tools-1.3.0/setup.py
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-08-04 06:31:00.565989 RM-Tools-1.3.1/
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1106 2020-07-23 17:47:25.000000 RM-Tools-1.3.1/LICENSE.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)      162 2021-04-26 15:31:37.000000 RM-Tools-1.3.1/MANIFEST.in
+-rw-r--r--   0 cvaneck    (503) staff       (20)     2924 2023-08-04 06:31:00.564434 RM-Tools-1.3.1/PKG-INFO
+-rw-r--r--   0 cvaneck    (503) staff       (20)     2085 2022-12-19 02:59:13.000000 RM-Tools-1.3.1/README.md
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-08-04 06:31:00.502022 RM-Tools-1.3.1/RM_Tools.egg-info/
+-rw-r--r--   0 cvaneck    (503) staff       (20)     2924 2023-08-04 06:31:00.000000 RM-Tools-1.3.1/RM_Tools.egg-info/PKG-INFO
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1901 2023-08-04 06:31:00.000000 RM-Tools-1.3.1/RM_Tools.egg-info/SOURCES.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)        1 2023-08-04 06:31:00.000000 RM-Tools-1.3.1/RM_Tools.egg-info/dependency_links.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)      871 2023-08-04 06:31:00.000000 RM-Tools-1.3.1/RM_Tools.egg-info/entry_points.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)       92 2023-08-04 06:31:00.000000 RM-Tools-1.3.1/RM_Tools.egg-info/requires.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)       30 2023-08-04 06:31:00.000000 RM-Tools-1.3.1/RM_Tools.egg-info/top_level.txt
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-08-04 06:31:00.515233 RM-Tools-1.3.1/RMtools_1D/
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1593 2019-12-19 15:46:49.000000 RM-Tools-1.3.1/RMtools_1D/README.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)        0 2019-08-02 13:47:51.000000 RM-Tools-1.3.1/RMtools_1D/__init__.py
+-rwxr-xr-x   0 cvaneck    (503) staff       (20)     9428 2023-05-08 06:09:10.000000 RM-Tools-1.3.1/RMtools_1D/calculate_RMSF.py
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-08-04 06:31:00.520712 RM-Tools-1.3.1/RMtools_1D/cats/
+-rw-r--r--   0 cvaneck    (503) staff       (20)     2528 2019-05-13 17:33:13.000000 RM-Tools-1.3.1/RMtools_1D/cats/catComplex.csv
+-rw-r--r--   0 cvaneck    (503) staff       (20)     5692 2019-05-13 17:33:13.000000 RM-Tools-1.3.1/RMtools_1D/cats/cat_simple_doQUfit.bat
+-rw-r--r--   0 cvaneck    (503) staff       (20)     2104 2019-05-13 17:33:13.000000 RM-Tools-1.3.1/RMtools_1D/cats/catalogue.csv
+-rw-r--r--   0 cvaneck    (503) staff       (20)     2825 2019-05-13 17:33:13.000000 RM-Tools-1.3.1/RMtools_1D/cats/catalogue1.csv
+-rw-r--r--   0 cvaneck    (503) staff       (20)    10670 2019-05-13 17:33:13.000000 RM-Tools-1.3.1/RMtools_1D/cats/testCat.dat
+-rwxr-xr-x   0 cvaneck    (503) staff       (20)     4955 2022-07-04 18:23:39.000000 RM-Tools-1.3.1/RMtools_1D/clean_model.py
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-08-04 06:31:00.537310 RM-Tools-1.3.1/RMtools_1D/data/
+-rw-r--r--   0 cvaneck    (503) staff       (20)    50612 2020-09-17 20:30:02.000000 RM-Tools-1.3.1/RMtools_1D/data/Source1.dat
+-rw-r--r--   0 cvaneck    (503) staff       (20)   140348 2022-12-12 07:27:14.000000 RM-Tools-1.3.1/RMtools_1D/data/Source1_FDFdirty.dat
+-rw-r--r--   0 cvaneck    (503) staff       (20)   115502 2022-12-12 07:27:14.000000 RM-Tools-1.3.1/RMtools_1D/data/Source1_RMSF-dirtyFDF-plots.pdf
+-rw-r--r--   0 cvaneck    (503) staff       (20)   280809 2022-12-12 07:27:14.000000 RM-Tools-1.3.1/RMtools_1D/data/Source1_RMSF.dat
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1730 2022-12-12 07:27:14.000000 RM-Tools-1.3.1/RMtools_1D/data/Source1_RMsynth.dat
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1950 2022-12-12 07:27:14.000000 RM-Tools-1.3.1/RMtools_1D/data/Source1_RMsynth.json
+-rw-r--r--   0 cvaneck    (503) staff       (20)   136375 2022-12-12 07:27:13.000000 RM-Tools-1.3.1/RMtools_1D/data/Source1_spectra-plots.pdf
+-rw-r--r--   0 cvaneck    (503) staff       (20)    14400 2022-12-12 07:27:14.000000 RM-Tools-1.3.1/RMtools_1D/data/Source1_weight.dat
+-rw-r--r--   0 cvaneck    (503) staff       (20)    50728 2020-09-17 20:30:02.000000 RM-Tools-1.3.1/RMtools_1D/data/Source2.dat
+-rw-r--r--   0 cvaneck    (503) staff       (20)    50710 2020-09-17 20:30:02.000000 RM-Tools-1.3.1/RMtools_1D/data/Source3.dat
+-rw-r--r--   0 cvaneck    (503) staff       (20)    50677 2020-09-17 20:30:02.000000 RM-Tools-1.3.1/RMtools_1D/data/Source4.dat
+-rw-r--r--   0 cvaneck    (503) staff       (20)    50670 2020-09-17 20:30:02.000000 RM-Tools-1.3.1/RMtools_1D/data/Source5.dat
+-rw-r--r--   0 cvaneck    (503) staff       (20)    50727 2020-09-17 20:30:02.000000 RM-Tools-1.3.1/RMtools_1D/data/Source6.dat
+-rw-r--r--   0 cvaneck    (503) staff       (20)    50687 2020-09-17 20:30:02.000000 RM-Tools-1.3.1/RMtools_1D/data/Source7.dat
+-rw-r--r--   0 cvaneck    (503) staff       (20)    50589 2020-09-17 20:30:02.000000 RM-Tools-1.3.1/RMtools_1D/data/Source8.dat
+-rwxr-xr-x   0 cvaneck    (503) staff       (20)    26064 2023-08-01 23:31:47.000000 RM-Tools-1.3.1/RMtools_1D/do_QUfit_1D_mnest.py
+-rwxr-xr-x   0 cvaneck    (503) staff       (20)    21451 2022-12-19 02:59:13.000000 RM-Tools-1.3.1/RMtools_1D/do_RMclean_1D.py
+-rwxr-xr-x   0 cvaneck    (503) staff       (20)    31814 2023-08-04 06:15:02.000000 RM-Tools-1.3.1/RMtools_1D/do_RMsynth_1D.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)    10163 2023-05-08 06:09:10.000000 RM-Tools-1.3.1/RMtools_1D/do_RMsynth_1D_fromFITS.py
+-rwxr-xr-x   0 cvaneck    (503) staff       (20)    16089 2019-09-12 18:37:00.000000 RM-Tools-1.3.1/RMtools_1D/mk_test_ascii_data.py
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-08-04 06:31:00.542096 RM-Tools-1.3.1/RMtools_1D/models_ns/
+-rw-r--r--   0 cvaneck    (503) staff       (20)       38 2019-05-13 17:33:13.000000 RM-Tools-1.3.1/RMtools_1D/models_ns/__init__.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)     2038 2022-12-19 02:59:13.000000 RM-Tools-1.3.1/RMtools_1D/models_ns/m1.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)     3854 2022-12-19 02:59:13.000000 RM-Tools-1.3.1/RMtools_1D/models_ns/m11.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)     2365 2022-12-19 02:59:13.000000 RM-Tools-1.3.1/RMtools_1D/models_ns/m2.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)     4069 2022-12-19 02:59:13.000000 RM-Tools-1.3.1/RMtools_1D/models_ns/m3.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)     4420 2022-12-19 02:59:13.000000 RM-Tools-1.3.1/RMtools_1D/models_ns/m4.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)    56826 2023-02-06 04:19:40.000000 RM-Tools-1.3.1/RMtools_1D/rmtools_bwdepol.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)     7892 2022-12-19 02:59:23.000000 RM-Tools-1.3.1/RMtools_1D/rmtools_bwpredict.py
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-08-04 06:31:00.554401 RM-Tools-1.3.1/RMtools_3D/
+-rw-r--r--   0 cvaneck    (503) staff       (20)     2318 2023-04-18 00:08:34.000000 RM-Tools-1.3.1/RMtools_3D/README.txt
+-rw-r--r--   0 cvaneck    (503) staff       (20)    15185 2023-08-01 23:31:44.000000 RM-Tools-1.3.1/RMtools_3D/RMpeakfit_3D.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)        0 2019-08-02 13:47:51.000000 RM-Tools-1.3.1/RMtools_3D/__init__.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)     4106 2023-08-01 23:31:44.000000 RM-Tools-1.3.1/RMtools_3D/assemble_chunks.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)     3555 2023-08-01 23:31:44.000000 RM-Tools-1.3.1/RMtools_3D/create_chunks.py
+-rwxr-xr-x   0 cvaneck    (503) staff       (20)    20350 2022-12-19 02:59:13.000000 RM-Tools-1.3.1/RMtools_3D/do_RMclean_3D.py
+-rwxr-xr-x   0 cvaneck    (503) staff       (20)    30548 2023-08-04 06:22:51.000000 RM-Tools-1.3.1/RMtools_3D/do_RMsynth_3D.py
+-rwxr-xr-x   0 cvaneck    (503) staff       (20)    19285 2023-08-01 23:31:44.000000 RM-Tools-1.3.1/RMtools_3D/do_fitIcube.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)     5503 2020-06-08 13:35:35.000000 RM-Tools-1.3.1/RMtools_3D/extract_region.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)     1804 2022-12-19 02:59:13.000000 RM-Tools-1.3.1/RMtools_3D/make_freq_file.py
+-rwxr-xr-x   0 cvaneck    (503) staff       (20)    19234 2023-08-01 23:31:44.000000 RM-Tools-1.3.1/RMtools_3D/mk_test_cube_data.py
+drwxr-xr-x   0 cvaneck    (503) staff       (20)        0 2023-08-04 06:31:00.563548 RM-Tools-1.3.1/RMutils/
+-rw-r--r--   0 cvaneck    (503) staff       (20)      251 2019-05-13 17:33:13.000000 RM-Tools-1.3.1/RMutils/__init__.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)    22901 2019-05-13 17:33:13.000000 RM-Tools-1.3.1/RMutils/corner.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)    78840 2019-05-13 17:33:13.000000 RM-Tools-1.3.1/RMutils/mpfit.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)    36212 2019-05-13 17:33:13.000000 RM-Tools-1.3.1/RMutils/nestle.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)     4842 2019-05-13 17:33:13.000000 RM-Tools-1.3.1/RMutils/normalize.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)    17314 2019-05-13 17:33:13.000000 RM-Tools-1.3.1/RMutils/util_FITS.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)    84672 2023-08-01 23:31:47.000000 RM-Tools-1.3.1/RMutils/util_RM.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)    40930 2022-12-19 04:18:34.000000 RM-Tools-1.3.1/RMutils/util_misc.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)    10191 2021-02-02 21:24:43.000000 RM-Tools-1.3.1/RMutils/util_plotFITS.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)    78650 2022-12-19 02:59:13.000000 RM-Tools-1.3.1/RMutils/util_plotTk.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)     4619 2019-05-13 17:33:13.000000 RM-Tools-1.3.1/RMutils/util_rec.py
+-rw-r--r--   0 cvaneck    (503) staff       (20)       38 2023-08-04 06:31:00.566087 RM-Tools-1.3.1/setup.cfg
+-rw-r--r--   0 cvaneck    (503) staff       (20)     3183 2023-08-04 06:21:38.000000 RM-Tools-1.3.1/setup.py
```

### Comparing `RM-Tools-1.3.0/LICENSE.txt` & `RM-Tools-1.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/PKG-INFO` & `RM-Tools-1.3.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 Metadata-Version: 2.1
 Name: RM-Tools
-Version: 1.3.0
+Version: 1.3.1
 Summary: RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
 Home-page: https://github.com/CIRADA-Tools/RM-Tools
+Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.3.1.tar.gz
 Maintainer: Cameron Van Eck
 Maintainer-email: cameron.vaneck@anu.edu.au
 License: MIT
-Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.3.0.tar.gz
-Description: 
-        # RM-Tools
-        
-        RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
-        
-         Python scripts to perform RM-synthesis, RM-clean and QU-fitting on
-         polarised radio spectra.
-        
-        
-         Initial version by Cormac R. Purcell  
-         Currently maintained by CIRADA
-        
-        Version 1.2 is now released! Check the wiki for new functionality.
-        
-        Installation, usage instructions and detailed algorithm information can be found in the [wiki](https://github.com/CIRADA-Tools/RM-Tools/wiki).
-        
-        Structure:  
-        RMtools_1D  ... Toolkit to produce Faraday spectra of single pixels.  
-        RMtools_3D  ... Toolkit to produce Faraday depth cubes.  
-        RMutils     ... Utilities for interacting with polarized data and Faraday depth 
-        
-        This will make the following modules importable in Python: RMtools_1D, RMtools_3D, RMutil
-        
-        ![RM-Tools component diagram](https://github.com/CIRADA-Tools/RM-Tools/wiki/diagram.png)
-        
-        Five terminal commands are added to invoke the main tools:  
-        rmsynth1d  
-        rmclean1d  
-        rmsynth3d  
-        rmclean3d  
-        qufit
-        
-        Use these commands with a -h flag to get information on the usage of each. Full documentation is on the [wiki](https://github.com/CIRADA-Tools/RM-Tools/wiki).
-        
-        The following terminal commands are available to access the [additional tools](https://github.com/CIRADA-Tools/RM-Tools/wiki/Tools):  
-        rmtools_freqfile  
-        rmtools_calcRMSF  
-        rmtools_testdata1D  
-        rmtools_createchunks  
-        rmtools_assemblechunks  
-        rmtools_fitIcube  
-        rmtools_peakfitcube  
-        rmtools_testdata3D  
-        rmtools_extractregion
-        
-        
-        If you use this package in a publication, please cite the [ASCL entry](https://ui.adsabs.harvard.edu/abs/2020ascl.soft05003P/abstract) for the time being.  
-        A paper with a full description of the package is being prepared but is not available yet.
-        
-        Questions, bug reports, and feature requests can be posted to the GitHub issues page or sent to Cameron Van Eck, cameron.van.eck (at) dunlap.utoronto.ca.
-        
-        More information on the Canadian Initiative for Radio Astronomy Data Analysis (CIRADA) can be found at cirada.ca.
-        
-        ![Tests](https://github.com/CIRADA-Tools/RM-tools/actions/workflows/python-package.yml/badge.svg)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: QUfitting
 Provides-Extra: parallel
+License-File: LICENSE.txt
+
+
+# RM-Tools
+
+RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
+
+ Python scripts to perform RM-synthesis, RM-clean and QU-fitting on
+ polarised radio spectra.
+
+
+ Initial version by Cormac R. Purcell  
+ Currently maintained by CIRADA
+
+Version 1.2 is now released! Check the wiki for new functionality.
+
+Installation, usage instructions and detailed algorithm information can be found in the [wiki](https://github.com/CIRADA-Tools/RM-Tools/wiki).
+
+Structure:  
+RMtools_1D  ... Toolkit to produce Faraday spectra of single pixels.  
+RMtools_3D  ... Toolkit to produce Faraday depth cubes.  
+RMutils     ... Utilities for interacting with polarized data and Faraday depth 
+
+This will make the following modules importable in Python: RMtools_1D, RMtools_3D, RMutil
+
+![RM-Tools component diagram](https://github.com/CIRADA-Tools/RM-Tools/wiki/diagram.png)
+
+Five terminal commands are added to invoke the main tools:  
+rmsynth1d  
+rmclean1d  
+rmsynth3d  
+rmclean3d  
+qufit
+
+Use these commands with a -h flag to get information on the usage of each. Full documentation is on the [wiki](https://github.com/CIRADA-Tools/RM-Tools/wiki).
+
+The following terminal commands are available to access the [additional tools](https://github.com/CIRADA-Tools/RM-Tools/wiki/Tools):  
+rmtools_freqfile  
+rmtools_calcRMSF  
+rmtools_testdata1D  
+rmtools_createchunks  
+rmtools_assemblechunks  
+rmtools_fitIcube  
+rmtools_peakfitcube  
+rmtools_testdata3D  
+rmtools_extractregion
+
+
+If you use this package in a publication, please cite the [ASCL entry](https://ui.adsabs.harvard.edu/abs/2020ascl.soft05003P/abstract) for the time being.  
+A paper with a full description of the package is being prepared but is not available yet.
+
+Questions, bug reports, and feature requests can be posted to the GitHub issues page or sent to Cameron Van Eck, cameron.van.eck (at) dunlap.utoronto.ca.
+
+More information on the Canadian Initiative for Radio Astronomy Data Analysis (CIRADA) can be found at cirada.ca.
+
+![Tests](https://github.com/CIRADA-Tools/RM-tools/actions/workflows/python-package.yml/badge.svg)
```

### Comparing `RM-Tools-1.3.0/README.md` & `RM-Tools-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RM_Tools.egg-info/PKG-INFO` & `RM-Tools-1.3.1/RM_Tools.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 Metadata-Version: 2.1
 Name: RM-Tools
-Version: 1.3.0
+Version: 1.3.1
 Summary: RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
 Home-page: https://github.com/CIRADA-Tools/RM-Tools
+Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.3.1.tar.gz
 Maintainer: Cameron Van Eck
 Maintainer-email: cameron.vaneck@anu.edu.au
 License: MIT
-Download-URL: https://github.com/CIRADA-Tools/RM-Tools/archive/v1.3.0.tar.gz
-Description: 
-        # RM-Tools
-        
-        RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
-        
-         Python scripts to perform RM-synthesis, RM-clean and QU-fitting on
-         polarised radio spectra.
-        
-        
-         Initial version by Cormac R. Purcell  
-         Currently maintained by CIRADA
-        
-        Version 1.2 is now released! Check the wiki for new functionality.
-        
-        Installation, usage instructions and detailed algorithm information can be found in the [wiki](https://github.com/CIRADA-Tools/RM-Tools/wiki).
-        
-        Structure:  
-        RMtools_1D  ... Toolkit to produce Faraday spectra of single pixels.  
-        RMtools_3D  ... Toolkit to produce Faraday depth cubes.  
-        RMutils     ... Utilities for interacting with polarized data and Faraday depth 
-        
-        This will make the following modules importable in Python: RMtools_1D, RMtools_3D, RMutil
-        
-        ![RM-Tools component diagram](https://github.com/CIRADA-Tools/RM-Tools/wiki/diagram.png)
-        
-        Five terminal commands are added to invoke the main tools:  
-        rmsynth1d  
-        rmclean1d  
-        rmsynth3d  
-        rmclean3d  
-        qufit
-        
-        Use these commands with a -h flag to get information on the usage of each. Full documentation is on the [wiki](https://github.com/CIRADA-Tools/RM-Tools/wiki).
-        
-        The following terminal commands are available to access the [additional tools](https://github.com/CIRADA-Tools/RM-Tools/wiki/Tools):  
-        rmtools_freqfile  
-        rmtools_calcRMSF  
-        rmtools_testdata1D  
-        rmtools_createchunks  
-        rmtools_assemblechunks  
-        rmtools_fitIcube  
-        rmtools_peakfitcube  
-        rmtools_testdata3D  
-        rmtools_extractregion
-        
-        
-        If you use this package in a publication, please cite the [ASCL entry](https://ui.adsabs.harvard.edu/abs/2020ascl.soft05003P/abstract) for the time being.  
-        A paper with a full description of the package is being prepared but is not available yet.
-        
-        Questions, bug reports, and feature requests can be posted to the GitHub issues page or sent to Cameron Van Eck, cameron.van.eck (at) dunlap.utoronto.ca.
-        
-        More information on the Canadian Initiative for Radio Astronomy Data Analysis (CIRADA) can be found at cirada.ca.
-        
-        ![Tests](https://github.com/CIRADA-Tools/RM-tools/actions/workflows/python-package.yml/badge.svg)
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
 Provides-Extra: QUfitting
 Provides-Extra: parallel
+License-File: LICENSE.txt
+
+
+# RM-Tools
+
+RM-synthesis, RM-clean and QU-fitting on polarised radio spectra
+
+ Python scripts to perform RM-synthesis, RM-clean and QU-fitting on
+ polarised radio spectra.
+
+
+ Initial version by Cormac R. Purcell  
+ Currently maintained by CIRADA
+
+Version 1.2 is now released! Check the wiki for new functionality.
+
+Installation, usage instructions and detailed algorithm information can be found in the [wiki](https://github.com/CIRADA-Tools/RM-Tools/wiki).
+
+Structure:  
+RMtools_1D  ... Toolkit to produce Faraday spectra of single pixels.  
+RMtools_3D  ... Toolkit to produce Faraday depth cubes.  
+RMutils     ... Utilities for interacting with polarized data and Faraday depth 
+
+This will make the following modules importable in Python: RMtools_1D, RMtools_3D, RMutil
+
+![RM-Tools component diagram](https://github.com/CIRADA-Tools/RM-Tools/wiki/diagram.png)
+
+Five terminal commands are added to invoke the main tools:  
+rmsynth1d  
+rmclean1d  
+rmsynth3d  
+rmclean3d  
+qufit
+
+Use these commands with a -h flag to get information on the usage of each. Full documentation is on the [wiki](https://github.com/CIRADA-Tools/RM-Tools/wiki).
+
+The following terminal commands are available to access the [additional tools](https://github.com/CIRADA-Tools/RM-Tools/wiki/Tools):  
+rmtools_freqfile  
+rmtools_calcRMSF  
+rmtools_testdata1D  
+rmtools_createchunks  
+rmtools_assemblechunks  
+rmtools_fitIcube  
+rmtools_peakfitcube  
+rmtools_testdata3D  
+rmtools_extractregion
+
+
+If you use this package in a publication, please cite the [ASCL entry](https://ui.adsabs.harvard.edu/abs/2020ascl.soft05003P/abstract) for the time being.  
+A paper with a full description of the package is being prepared but is not available yet.
+
+Questions, bug reports, and feature requests can be posted to the GitHub issues page or sent to Cameron Van Eck, cameron.van.eck (at) dunlap.utoronto.ca.
+
+More information on the Canadian Initiative for Radio Astronomy Data Analysis (CIRADA) can be found at cirada.ca.
+
+![Tests](https://github.com/CIRADA-Tools/RM-tools/actions/workflows/python-package.yml/badge.svg)
```

### Comparing `RM-Tools-1.3.0/RM_Tools.egg-info/SOURCES.txt` & `RM-Tools-1.3.1/RM_Tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RM_Tools.egg-info/entry_points.txt` & `RM-Tools-1.3.1/RM_Tools.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,7 @@
 rmtools_createchunks = RMtools_3D.create_chunks:main
 rmtools_extractregion = RMtools_3D.extract_region:main
 rmtools_fitIcube = RMtools_3D.do_fitIcube:main
 rmtools_freqfile = RMtools_3D.make_freq_file:save_freq_file
 rmtools_peakfitcube = RMtools_3D.RMpeakfit_3D:main
 rmtools_testdata1D = RMtools_1D.mk_test_ascii_data:main
 rmtools_testdata3D = RMtools_3D.mk_test_cube_data:main
-
```

### Comparing `RM-Tools-1.3.0/RMtools_1D/README.txt` & `RM-Tools-1.3.1/RMtools_1D/README.txt`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/calculate_RMSF.py` & `RM-Tools-1.3.1/RMtools_1D/calculate_RMSF.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,36 +10,36 @@
 a file with channel frequencies and weights
 OR
 a file with channel frequencies (assumes equal weights)
 OR
 Input values for mininum frequency, maximum frequency, and channel width.
 (assumes equal weights and all channels present)
 
-The outputs are a list of relavant RMSF properties, and a plot of the RMSF 
+The outputs are a list of relavant RMSF properties, and a plot of the RMSF
 shape.
 """
 
 #import sys
 import argparse
 import numpy as np
 from RMutils.util_RM import get_rmsf_planes
 from matplotlib import pyplot as plt
 
 C = 2.997924538e8 # Speed of light [m/s]
 
 def main():
     """
-    Determines what set of input parameters were defined, reads in file or 
+    Determines what set of input parameters were defined, reads in file or
     generates frequency array as appropriate, and passes frequency and weight
     arrays to the function that works out the RMSF properties.
     """
 
     descStr = """
-    Calculate and plot RMSF and report main properties, given a supplied 
-    frequency coverage and optional weights (either as second column of 
+    Calculate and plot RMSF and report main properties, given a supplied
+    frequency coverage and optional weights (either as second column of
     frequency file, or as separate file)."""
 
     parser = argparse.ArgumentParser(description=descStr,
                                  formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument("freqFile", metavar="freqFile.dat", nargs='?',default=None,
                         help="ASCII file containing frequencies and optionally weights.")
     parser.add_argument("weightFile", metavar="weightFile.dat", nargs='?',
@@ -51,28 +51,30 @@
                         help="absolute max Faraday depth sampled [Auto, ~10xFWHM].")
     parser.add_argument("-d", dest="dphi_radm2", type=float, default=None,
                         help="Delta phi [Auto, ~10/FWHM].")
     parser.add_argument("-s", dest="plotfile", default=None,
                         help="Filename to save plot to. [do not save]")
     parser.add_argument("-n", dest="plotname", default=None,
                         help="Name of plot [\"Simulated RMSF\"]")
-
+    parser.add_argument("-r", "--super-resolution", action="store_true",
+                        help="Optimise the resolution of the RMSF (as per Rudnick & Cotton). "
+                        )
     args = parser.parse_args()
-    
-    
+
+
     #Check that at least one frequency input has been given:
     if args.freqFile == None and args.freq_parms == None:
         print("Please supply either a file with frequency values or use the -f flag.")
         raise(Exception("No frequency input! Use -h flag for help on inputs."))
-    
+
     # if args.phiMax_radm2 != None:
     #     if args.phiMax_radm2
-    
+
     #Order of priority: frequency file takes precedence over -i flag.
-    #                   weight file takes precedence over 2nd column of frequency file.       
+    #                   weight file takes precedence over 2nd column of frequency file.
     if args.freqFile != None:
         data=np.genfromtxt(args.freqFile,encoding=None,dtype=None)
         if len(data.shape) == 2:
             freq_array=data[:,0]
             weights_array=data[:,1]
         else:
             freq_array=data
@@ -84,19 +86,19 @@
         weights_array=np.ones_like(freq_array)
 
 
     if args.weightFile != None:
         weights_array=np.genfromtxt(args.weightFile,encoding=None,dtype=None)
         if len(weights_array) != len(freq_array):
             raise Exception('Weights file does not have same number of channels as frequency source')
-    
 
-    determine_RMSF_parameters(freq_array,weights_array,args.phiMax_radm2,args.dphi_radm2,args.plotfile,args.plotname)
-    
-def determine_RMSF_parameters(freq_array,weights_array,phi_max,dphi,plotfile=None,plotname=None):
+
+    determine_RMSF_parameters(freq_array,weights_array,args.phiMax_radm2,args.dphi_radm2,args.plotfile,args.plotname, args.super_resolution)
+
+def determine_RMSF_parameters(freq_array,weights_array,phi_max,dphi,plotfile=None,plotname=None, super_resolution=False):
     """
     Characterizes an RMSF given the supplied frequency and weight arrays.
     Prints the results to terminal and produces a plot.
     Inputs:
         freq_array: array of frequency values (in Hz)
         weights_array: array of channel weights (arbitrary units)
         phi_max (float): maximum Faraday depth to compute RMSF out to.
@@ -104,46 +106,53 @@
         plotfile (str): file name and path to save RMSF plot.
         plotname (str): title of plot
     """
     lambda2_array=C**2/freq_array**2
     l2_min=np.min(lambda2_array)
     l2_max=np.max(lambda2_array)
     dl2=np.median(np.abs(np.diff(lambda2_array)))
-    
+
     if phi_max == None:
         phi_max = 10*2*np.sqrt(3.0) / (l2_max-l2_min)  #~10*FWHM
     if dphi == None:
         dphi = 0.1*2*np.sqrt(3.0) / (l2_max-l2_min)  #~10*FWHM
 
     phi_array=np.arange(-1*phi_max/2,phi_max/2+1e-6,dphi) #division by two accounts for how RMSF is always twice as wide as FDF.
 
-    RMSFcube, phi2Arr, fwhmRMSFArr, statArr=get_rmsf_planes(lambda2_array,phi_array,weightArr=weights_array,fitRMSF=True)
-    
-    
+    RMSFcube, phi2Arr, fwhmRMSFArr, statArr=get_rmsf_planes(
+        lambda2_array,
+        phi_array,
+        weightArr=weights_array,
+        fitRMSF=True,
+        fitRMSFreal=super_resolution,
+        lam0Sq_m2=0 if super_resolution else None,
+    )
+
+
     #Output key results to terminal:
     print('RMSF PROPERTIES:')
     print('Theoretical (unweighted) FWHM:       {:.4g} rad m^-2'.format(3.8 / (l2_max-l2_min)))
     print('Measured FWHM:                       {:.4g} rad m^-2'.format(fwhmRMSFArr))
     print('Theoretical largest FD scale probed: {:.4g} rad m^-2'.format(np.pi/l2_min))
     print('Theoretical maximum FD*:             {:.4g} rad m^-2'.format(np.sqrt(3.0)/dl2))
     print('*50% bandwdith depolarization threshold, for median channel width in Delta-lambda^2')
     print('* may not be reliable over very large fractional bandwidths or in data with ')
     print('differing channel widths or many frequency gaps.')
-    #Explanation for below: This code find the local maxima in the positive half of the RMSF, 
+    #Explanation for below: This code find the local maxima in the positive half of the RMSF,
     #finds the highest amplitude one, and calls that the first sidelobe.
     try:
         x=np.diff(np.sign(np.diff(np.abs(RMSFcube[RMSFcube.size//2:])))) #-2=local max, +2=local min
         y=1+np.where(x==-2)[0]  #indices of peaks, +1 is because of offset from double differencing
-        peaks=np.abs(RMSFcube[RMSFcube.size//2:])[y] 
+        peaks=np.abs(RMSFcube[RMSFcube.size//2:])[y]
         print('First sidelobe FD and amplitude:     {:.4g} rad m^-2'.format(phi2Arr[phi2Arr.size//2:][y[np.argmax(peaks)]]))
         print('                                     {:.4g} % of peak'.format(np.max(peaks)*100))
     except:
         pass
-    
-    
+
+
     #Plotting:
     plt.figure(figsize=(7,7))
     plt.subplot(211)
     plt.axhline(0,color='k')
     if plotname==None:
         plt.title('Simulated RMSF')
     else:
@@ -173,31 +182,31 @@
             horizontalalignment='left',verticalalignment='top')
 
     try:
         ax.text(0.1,0.8,('\n\n\n\n'+'First sidelobe FD and amplitude:     {:.4g} rad m^-2\n'+
                  '                                     {:.4g} % of peak').format(phi2Arr[phi2Arr.size//2:][y[np.argmax(peaks)]],np.max(peaks)*100),
                 family='monospace',horizontalalignment='left',verticalalignment='top')
     except:
-        pass                    
-                                                                 
+        pass
+
 #    ax.text(0.,0.7,('Theoretical (unweighted) FWHM:      {:.4g} rad m^-2'.format(2*np.sqrt(3.0) / (l2_max-l2_min)))
 #    ax.text(0.,0.58,'Measured FWHM:                               {:.4g} rad m^-2'.format(fwhmRMSFArr))
 #    ax.text(0.,0.46,'Theoretical largest FD scale probed: {:.4g} rad m^-2'.format(np.pi/l2_min))
 #    ax.text(0.,0.34,'Theoretical maximum FD:                 {:.4g} rad m^-2'.format(np.sqrt(3.0)/dl2))
 #    ax.text(0.,0.22,'First sidelobe FD and amplitude:       {:.4g} rad m^-2'.format(phi2Arr[phi2Arr.size//2:][y[np.argmax(peaks)]]))
 #    ax.text(0.,0.1,'                                                           {:.4g} % of peak'.format(np.max(peaks)*100))
 
 
     if plotfile != None:
         plt.savefig(plotfile,bbox_inches='tight')
     else:
         plt.show()
-    
-    
-    
+
+
+
 if __name__ == "__main__":
     main()
```

### Comparing `RM-Tools-1.3.0/RMtools_1D/cats/catComplex.csv` & `RM-Tools-1.3.1/RMtools_1D/cats/catComplex.csv`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/cats/cat_simple_doQUfit.bat` & `RM-Tools-1.3.1/RMtools_1D/cats/cat_simple_doQUfit.bat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/cats/catalogue.csv` & `RM-Tools-1.3.1/RMtools_1D/cats/catalogue.csv`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/cats/catalogue1.csv` & `RM-Tools-1.3.1/RMtools_1D/cats/catalogue1.csv`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/cats/testCat.dat` & `RM-Tools-1.3.1/RMtools_1D/cats/testCat.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/clean_model.py` & `RM-Tools-1.3.1/RMtools_1D/clean_model.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source1.dat` & `RM-Tools-1.3.1/RMtools_1D/data/Source1.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source1_FDFdirty.dat` & `RM-Tools-1.3.1/RMtools_1D/data/Source1_FDFdirty.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source1_RMSF-dirtyFDF-plots.pdf` & `RM-Tools-1.3.1/RMtools_1D/data/Source1_RMSF-dirtyFDF-plots.pdf`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source1_RMSF.dat` & `RM-Tools-1.3.1/RMtools_1D/data/Source1_RMSF.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source1_RMsynth.dat` & `RM-Tools-1.3.1/RMtools_1D/data/Source1_RMsynth.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source1_RMsynth.json` & `RM-Tools-1.3.1/RMtools_1D/data/Source1_RMsynth.json`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source1_spectra-plots.pdf` & `RM-Tools-1.3.1/RMtools_1D/data/Source1_spectra-plots.pdf`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source1_weight.dat` & `RM-Tools-1.3.1/RMtools_1D/data/Source1_weight.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source2.dat` & `RM-Tools-1.3.1/RMtools_1D/data/Source2.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source3.dat` & `RM-Tools-1.3.1/RMtools_1D/data/Source3.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source4.dat` & `RM-Tools-1.3.1/RMtools_1D/data/Source4.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source5.dat` & `RM-Tools-1.3.1/RMtools_1D/data/Source5.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source6.dat` & `RM-Tools-1.3.1/RMtools_1D/data/Source6.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source7.dat` & `RM-Tools-1.3.1/RMtools_1D/data/Source7.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/data/Source8.dat` & `RM-Tools-1.3.1/RMtools_1D/data/Source8.dat`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/do_QUfit_1D_mnest.py` & `RM-Tools-1.3.1/RMtools_1D/do_QUfit_1D_mnest.py`

 * *Files 2% similar despite different names*

```diff
@@ -362,14 +362,23 @@
         pass
 
     # Display the figure
     if showPlots:
         specFig.canvas.draw()
         specFig.show()
 
+
+    print("Imodel:"+",".join([str(x.astype(np.float32)) for x in IfitDict["p"]]))
+    print("Imodel_errs:"+",".join([str(x.astype(np.float32)) for x in IfitDict["perror"]]))
+    print("IfitChiSq:"+str(toscalar(IfitDict["chiSq"])))
+    print("IfitChiSqRed:"+str(toscalar(IfitDict["chiSqRed"])))
+    print("IfitPolyOrd:"+str(toscalar(IfitDict["polyOrd"])))
+    print("Ifitfreq0:"+str(toscalar(IfitDict["reference_frequency_Hz"])))
+
+
     # -------------------------------------------------------------------------#
 
     # Load the model and parameters from the relevant file
     mod = load_model(modelNum, verbose=True)
 
     model = mod.model
```

### Comparing `RM-Tools-1.3.0/RMtools_1D/do_RMclean_1D.py` & `RM-Tools-1.3.1/RMtools_1D/do_RMclean_1D.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/do_RMsynth_1D.py` & `RM-Tools-1.3.1/RMtools_1D/do_RMsynth_1D.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,17 +66,18 @@
     exit()
 
 C = 2.997924538e8 # Speed of light [m/s]
 
 #-----------------------------------------------------------------------------#
 def run_rmsynth(data, polyOrd=2, phiMax_radm2=None, dPhi_radm2=None,
                 nSamples=10.0, weightType="variance", fitRMSF=False,
-                noStokesI=False, modStokesI=None, phiNoise_radm2=1e6, nBits=32, showPlots=False,
-                debug=False, verbose=False, log=print,units='Jy/beam', 
-                prefixOut="prefixOut", saveFigures=None,fit_function='log'):
+                noStokesI=False, modStokesI=None, phiNoise_radm2=1e6, nBits=32,
+                showPlots=False, debug=False, verbose=False, log=print,
+                units='Jy/beam', prefixOut="prefixOut", saveFigures=None,
+                fit_function='log', super_resolution=False):
     """Run RM synthesis on 1D data.
 
     Args:
         data (list): Contains frequency and polarization data as either:
             [freq_Hz, I, Q, U, dI, dQ, dU]
                 freq_Hz (array_like): Frequency of each channel in Hz.
                 I (array_like): Stokes I intensity in each channel.
@@ -164,23 +165,23 @@
                                  dUArr    = dUArr,
                                  polyOrd  = polyOrd,
                                  verbose  = True,
                                  debug    = debug,
                                  fit_function = fit_function,
                                  modStokesI = modStokesI,
                                  )
-             
+
     dquArr = (dqArr + duArr)/2.0
     dquArr= np.where(np.isfinite(dquArr),dquArr,np.nan)
 
 
     # Plot the data and the Stokes I model fit
     if verbose: log("Plotting the input data and spectral index fit.")
     freqHirArr_Hz =  np.linspace(freqArr_Hz[0], freqArr_Hz[-1], 10000)
-    if modStokesI is None:   
+    if modStokesI is None:
         IModHirArr = calculate_StokesI_model(fitDict,freqHirArr_Hz)
     elif modStokesI is not None:
         modStokesI_interp = interp1d(freqArr_Hz, modStokesI)
         IModHirArr = modStokesI_interp(freqHirArr_Hz)
     if showPlots or saveFigures:
         specFig = plt.figure(facecolor='w',figsize=(12.0, 8))
         plot_Ipqu_spectra_fig(freqArr_Hz     = freqArr_Hz,
@@ -235,15 +236,18 @@
     dFreq_Hz = np.nanmin(np.abs(np.diff(freqArr_Hz)))
     lambdaSqRange_m2 = ( np.nanmax(lambdaSqArr_m2) -
                          np.nanmin(lambdaSqArr_m2) )
     dLambdaSqMin_m2 = np.nanmin(np.abs(np.diff(lambdaSqArr_m2)))
     dLambdaSqMax_m2 = np.nanmax(np.abs(np.diff(lambdaSqArr_m2)))
 
     # Set the Faraday depth range
-    fwhmRMSF_radm2 = 2.0 * m.sqrt(3.0) / lambdaSqRange_m2
+    if not super_resolution:
+        fwhmRMSF_radm2 = 3.8 / lambdaSqRange_m2 #Dickey+2019 theoretical RMSF width
+    else: #If super resolution, use R&C23 theoretical width
+        fwhmRMSF_radm2 = 2.0 / (np.nanmax(lambdaSqArr_m2) + np.nanmin(lambdaSqArr_m2))
     if dPhi_radm2 is None:
         dPhi_radm2 = fwhmRMSF_radm2 / nSamples
     if phiMax_radm2 is None:
         phiMax_radm2 = m.sqrt(3.0) / dLambdaSqMax_m2
         phiMax_radm2 = max(phiMax_radm2, fwhmRMSF_radm2*10.)    # Force the minimum phiMax to 10 FWHM
 
     # Faraday depth sampling. Zero always centred on middle channel
@@ -271,26 +275,28 @@
     dirtyFDF, lam0Sq_m2 = do_rmsynth_planes(dataQ           = qArr,
                                             dataU           = uArr,
                                             lambdaSqArr_m2  = lambdaSqArr_m2,
                                             phiArr_radm2    = phiArr_radm2,
                                             weightArr       = weightArr,
                                             nBits           = nBits,
                                             verbose         = verbose,
-                                            log             = log)
+                                            log             = log,
+                                            lam0Sq_m2       = 0 if super_resolution else None,
+                                            )
 
     # Calculate the Rotation Measure Spread Function
     RMSFArr, phi2Arr_radm2, fwhmRMSFArr, fitStatArr = \
         get_rmsf_planes(lambdaSqArr_m2  = lambdaSqArr_m2,
                         phiArr_radm2    = phiArr_radm2,
                         weightArr       = weightArr,
                         mskArr          = ~np.isfinite(qArr),
                         lam0Sq_m2       = lam0Sq_m2,
                         double          = True,
-                        fitRMSF         = fitRMSF,
-                        fitRMSFreal     = False,
+                        fitRMSF         = fitRMSF or super_resolution,
+                        fitRMSFreal     = super_resolution,
                         nBits           = nBits,
                         verbose         = verbose,
                         log             = log)
     fwhmRMSF = float(fwhmRMSFArr)
 
     # ALTERNATE RM-SYNTHESIS CODE --------------------------------------------#
 
@@ -301,24 +307,25 @@
 
     endTime = time.time()
     cputime = (endTime - startTime)
     if verbose: log("> RM-synthesis completed in %.2f seconds." % cputime)
 
 
     # Determine the Stokes I value at lam0Sq_m2 from the Stokes I model
+    # This will break if lam0Sq_m2==0. Using the mean frequency in this case.
     # Multiply the dirty FDF by Ifreq0 to recover the PI
-    freq0_Hz = C / m.sqrt(lam0Sq_m2)
-    if modStokesI is None:   
+    freq0_Hz = C / m.sqrt(lam0Sq_m2) if lam0Sq_m2 > 0 else np.nanmean(freqArr_Hz)
+    if modStokesI is None:
         Ifreq0 = calculate_StokesI_model(fitDict,freq0_Hz)
     elif modStokesI is not None:
         modStokesI_interp = interp1d(freqArr_Hz, modStokesI)
         Ifreq0 = modStokesI_interp(freq0_Hz)
     dirtyFDF *= (Ifreq0)    # FDF is in fracpol units initially, convert back to flux
 
-    # if modStokesI is None:   
+    # if modStokesI is None:
     #     #Need to renormalize the Stokes I parameters here to the actual reference frequency.
     #     fitDict=renormalize_StokesI_model(fitDict,freq0_Hz)
 
     # Calculate the theoretical noise in the FDF !!Old formula only works for wariance weights!
     weightArr = np.where(np.isnan(weightArr), 0.0, weightArr)
     dFDFth = Ifreq0*np.sqrt( np.nansum(weightArr**2 * np.nan_to_num(dquArr)**2) / (np.sum(weightArr))**2 )
 
@@ -341,15 +348,15 @@
     mDict["fit_function"] = fit_function
     mDict["lam0Sq_m2"] = toscalar(lam0Sq_m2)
     mDict["freq0_Hz"] = toscalar(freq0_Hz)
     mDict["fwhmRMSF"] = toscalar(fwhmRMSF)
     mDict["dQU"] = toscalar(nanmedian(dQUArr))
     mDict["dFDFth"] = toscalar(dFDFth)
     mDict["units"] = units
-    
+
     if (fitDict["fitStatus"] >= 128) and verbose:
         log("WARNING: Stokes I model contains negative values!")
     elif (fitDict["fitStatus"] >= 64) and verbose:
         log("Caution: Stokes I model has low signal-to-noise.")
 
 
 
@@ -472,24 +479,24 @@
 #        input()
 
     return mDict, aDict
 
 def readFile(dataFile, nBits, verbose=True, debug=False):
     """
     Read the I, Q & U data from the ASCII file.
-    
+
     Inputs:
         datafile (str): relative or absolute path to file.
         nBits (int): number of bits to store the data as.
         verbose (bool): Print verbose messages to terminal?
         debug (bool): Print full traceback in case of failure?
-        
+
     Returns:
         data (list of arrays): List containing the columns found in the file.
-        If Stokes I is present, this will be [freq_Hz, I, Q, U, dI, dQ, dU], 
+        If Stokes I is present, this will be [freq_Hz, I, Q, U, dI, dQ, dU],
         else [freq_Hz, q, u,  dq, du].
     """
 
     # Default data types
     dtFloat = "float" + str(nBits)
     dtComplex = "complex" + str(2*nBits)
 
@@ -556,40 +563,40 @@
     FH.close()
 
 
     outFile = prefixOut + "_RMsynth.json"
 
     if verbose:
         print("> %s" % outFile)
-        
+
     for k, v in outdict.items():
         if isinstance(v, np.float_):
             outdict[k] = float(v)
         elif isinstance(v, np.int_):
             outdict[k] = int(v)
         elif isinstance(v, np.ndarray):
             outdict[k] = v.tolist()
         elif isinstance(v, np.bool_):
             outdict[k] = bool(v)
 
-        
+
     json.dump(dict(outdict), open(outFile, "w"))
 
 
 #-----------------------------------------------------------------------------#
 def main():
     import argparse
     """
     Start the function to perform RM-synthesis if called from the command line.
     """
 
     # Help string to be shown using the -h option
     descStr = """
     Run RM-synthesis on Stokes I, Q and U spectra (1D) stored in an ASCII
-    file. The Stokes I spectrum is first fit with a polynomial or power law 
+    file. The Stokes I spectrum is first fit with a polynomial or power law
     and the resulting model used to create fractional q = Q/I and u = U/I spectra.
 
     The ASCII file should the following columns, in a space separated format:
     [freq_Hz, I, Q, U, I_err, Q_err, U_err]
     OR
     [freq_Hz, Q, U, Q_err, U_err]
 
@@ -636,14 +643,17 @@
                         help="verbose output [False].")
     parser.add_argument("-S", dest="saveOutput", action="store_true",
                         help="save the arrays and plots [False].")
     parser.add_argument("-D", dest="debug", action="store_true",
                         help="turn on debugging messages & plots [False].")
     parser.add_argument("-U", dest="units", type=str, default="Jy/beam",
                         help="Intensity units of the data. [Jy/beam]")
+    parser.add_argument("-r", "--super-resolution", action="store_true",
+                        help="Optimise the resolution of the RMSF (as per Rudnick & Cotton). "
+                        )
     args = parser.parse_args()
 
     # Sanity checks
     if not os.path.exists(args.dataFile[0]):
         print("File does not exist: '%s'." % args.dataFile[0])
         sys.exit()
     prefixOut, ext = os.path.splitext(args.dataFile[0])
@@ -652,30 +662,33 @@
     nBits = 32
     if args.bit64:
         nBits = 64
     verbose=args.verbose
     data = readFile(args.dataFile[0],nBits, verbose=verbose, debug=args.debug)
 
     # Run RM-synthesis on the spectra
-    mDict, aDict = run_rmsynth(data           = data,
+    mDict, aDict = run_rmsynth(
+                data           = data,
                 polyOrd        = args.polyOrd,
                 phiMax_radm2   = args.phiMax_radm2,
                 dPhi_radm2     = args.dPhi_radm2,
                 nSamples       = args.nSamples,
                 weightType     = args.weightType,
                 fitRMSF        = args.fitRMSF,
                 noStokesI      = args.noStokesI,
                 nBits          = nBits,
                 showPlots      = args.showPlots,
                 debug          = args.debug,
                 verbose        = verbose,
                 units          = args.units,
                 prefixOut      = prefixOut,
                 saveFigures    = args.saveOutput,
-                fit_function   = args.fit_function)
+                fit_function   = args.fit_function,
+                super_resolution=args.super_resolution,
+    )
 
     if args.saveOutput:
         saveOutput(mDict, aDict, prefixOut, verbose)
 
 
 #-----------------------------------------------------------------------------#
 if __name__ == "__main__":
```

### Comparing `RM-Tools-1.3.0/RMtools_1D/do_RMsynth_1D_fromFITS.py` & `RM-Tools-1.3.1/RMtools_1D/do_RMsynth_1D_fromFITS.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE #
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER      #
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING     #
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER         #
 # DEALINGS IN THE SOFTWARE.                                                   #
 #                                                                             #
 #=============================================================================#
- 
+
 import sys
 import os
 #import time
 import argparse
 #import pdb
 
 if sys.version_info.major == 2:
@@ -73,15 +73,15 @@
     _FDFdirty.dat: Dirty FDF/RM Spectrum [Phi, Q, U]
     _RMSF.dat: Computed RMSF [Phi, Q, U]
     _RMsynth.dat: list of derived parameters for RM spectrum
                 (approximately equivalent to -v flag output)
     _RMsynth.json: dictionary of derived parameters for RM spectrum
     _weight.dat: Calculated channel weights [freq_Hz, weight]
     """
-    
+
     # Parse the command line options
     parser = argparse.ArgumentParser(description=descStr,epilog=epilog_text,
                                  formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument("dataFile", metavar="StokesQ.fits", nargs=1,
                         help="FITS cube with Stokes Q data.")
     parser.add_argument("UFile", metavar="StokesU.fits", nargs=1,
                         help="FITS cube with Stokes U data.")
@@ -114,18 +114,20 @@
     parser.add_argument("-v", dest="verbose", action="store_true",
                         help="verbose output [False].")
     parser.add_argument("-S", dest="saveOutput", action="store_true",
                         help="save the arrays [False].")
     parser.add_argument("-D", dest="debug", action="store_true",
                         help="turn on debugging messages & plots [False].")
     parser.add_argument("-U", dest="units", type=str, default=None,
-                        help="Intensity units of the data. [from FITS header]")    
-
+                        help="Intensity units of the data. [from FITS header]")
+    parser.add_argument("-r", "--super-resolution", action="store_true",
+                        help="Optimise the resolution of the RMSF (as per Rudnick & Cotton). "
+                        )
     args = parser.parse_args()
-    
+
     # Sanity checks
     if not os.path.exists(args.dataFile[0]):
         print("File does not exist: '%s'." % args.dataFile[0])
         sys.exit()
     prefixOut, ext = os.path.splitext(args.dataFile[0])
     dataDir, dummy = os.path.split(args.dataFile[0])
     # Set the floating point precision
@@ -145,15 +147,15 @@
         xcoords = int(args.xcoords)-1
         ycoords = int(args.ycoords)-1
     freq_array = get_freq_array(args.dataFile[0])
     Q_array = get_data_Q_U(args.dataFile[0], ycoords, xcoords)
     U_array = get_data_Q_U(args.UFile[0], ycoords, xcoords)
     dQ_array = np.full(freq_array.shape, 1*10**(-3))
     dU_array = np.full(freq_array.shape, 1*10**(-3))
-    
+
     Q_array[~np.isfinite(Q_array)]=np.nan
     U_array[~np.isfinite(U_array)]=np.nan
     data = [freq_array, Q_array, U_array, dQ_array, dU_array]
 
     if args.units == None:
         if 'BUNIT' in hduList[0].header:
             args.units=hduList[0].header['BUNIT']
@@ -164,31 +166,32 @@
         raise Exception("All QU values zero! Maybe invalid pixel?")
 
     if args.StokesI_fits is not None:
         I_array = get_data_Q_U(args.StokesI_fits, ycoords, xcoords)
         dI_array = np.full(freq_array.shape, 1 * 10 ** (-3))
         data=[freq_array,I_array, Q_array, U_array, dI_array, dQ_array, dU_array]
     # Run RM-synthesis on the spectra
-    dict, aDict = run_rmsynth(data           = data,
+    mDict, aDict = run_rmsynth(data           = data,
                 polyOrd        = args.polyOrd,
                 phiMax_radm2   = args.phiMax_radm2,
                 dPhi_radm2     = args.dPhi_radm2,
                 nSamples       = args.nSamples,
                 weightType     = args.weightType,
                 fitRMSF        = args.fitRMSF,
                 noStokesI      = args.noStokesI,
                 nBits          = nBits,
                 showPlots      = args.showPlots,
                 debug          = args.debug,
                 verbose        = verbose,
                 units          = args.units,
-                saveFigures    = args.saveOutput)
-    #pdb.set_trace()
+                saveFigures    = args.saveOutput,
+                super_resolution=args.super_resolution,
+            )
     if args.saveOutput:
-        saveOutput(dict, aDict, prefixOut, verbose)
+        saveOutput(mDict, aDict, prefixOut, verbose)
 
 def get_data_Q_U(filename, ycoords, xcoords):
     hduList = fits.open(filename)
     return hduList[0].data[:, ycoords, xcoords]
 
 
 #-----------------------------------------------------------------------------#
```

### Comparing `RM-Tools-1.3.0/RMtools_1D/mk_test_ascii_data.py` & `RM-Tools-1.3.1/RMtools_1D/mk_test_ascii_data.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/models_ns/m1.py` & `RM-Tools-1.3.1/RMtools_1D/models_ns/m1.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/models_ns/m11.py` & `RM-Tools-1.3.1/RMtools_1D/models_ns/m11.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/models_ns/m2.py` & `RM-Tools-1.3.1/RMtools_1D/models_ns/m2.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/models_ns/m3.py` & `RM-Tools-1.3.1/RMtools_1D/models_ns/m3.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/models_ns/m4.py` & `RM-Tools-1.3.1/RMtools_1D/models_ns/m4.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/rmtools_bwdepol.py` & `RM-Tools-1.3.1/RMtools_1D/rmtools_bwdepol.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_1D/rmtools_bwpredict.py` & `RM-Tools-1.3.1/RMtools_1D/rmtools_bwpredict.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_3D/RMpeakfit_3D.py` & `RM-Tools-1.3.1/RMtools_3D/RMpeakfit_3D.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 # Initial version: Cameron Van Eck, Dec 2020
 """
 
 import sys
 import os
 import numpy as np
 import astropy.io.fits as pf
+from tqdm.auto import tqdm, trange
 from RMutils.util_RM import measure_FDF_parms
-from RMutils.util_misc import interp_images,progress  
+from RMutils.util_misc import interp_images
 from RMutils.util_RM import fits_make_lin_axis
 from RMtools_3D.do_RMsynth_3D import readFitsCube, readFreqFile
 
 
 C = 2.997924538e8 # Speed of light [m/s]
 
 
@@ -26,52 +27,52 @@
 
 def pixelwise_peak_fitting(FDF, phiArr, fwhmRMSF,lamSqArr_m2, lam0Sq,
                            product_list,noiseArr=None,stokesIcube=None):
     """
     Performs the 1D FDF peak fitting used in RMsynth/RMclean_1D, pixelwise on
     all pixels in a 3D FDF cube.
 
-    Inputs: 
+    Inputs:
         FDF: FDF cube (3D array). This is assumed to be in astropy axis ordering
             (Phi, dec, ra)
         phiArr: (1D) array of phi values
         fwhmRMSF: 2D array of RMSF FWHM values
         lamSqArr_m2: 1D array of channel lambda^2 values.
         lam0Sq: scalar value for lambda^2_0, the reference wavelength squared.
         product_list: list containing the names of the fitting products to save.
-        dFDF: 2D array of theoretical noise values. If not supplied, the 
+        dFDF: 2D array of theoretical noise values. If not supplied, the
             peak fitting will default to using the measured noise.
     Outputs: dictionary of 2D maps, 1 per fit output
     """
 
     #FDF: output by synth3d or clean3d
     #phiArr: can be generated from FDF cube
     #fwhm: 2D map produced synth3D
     #dFDFth: not currently produced (default mode not to input noise!)
     #   If not present, measure_FDF_parms uses the corMAD noise.
-    #   
+    #
     #lamSqArr is only needed for computing errors in derotated angles
     #   This could be compressed to a map or single value from RMsynth?
     #lam0Sq is necessary for de-rotation
 
 
 
     map_size=FDF.shape[1:]
 
     #Create pixel location arrays:
     xarr,yarr=np.meshgrid(range(map_size[0]),range(map_size[1]))
     xarr=xarr.ravel()
     yarr=yarr.ravel()
-    
+
     #Create empty maps:
     map_dict={}
     for parameter in product_list:
         map_dict[parameter]=np.zeros(map_size)
-        
- 
+
+
 
     freqArr_Hz=C/np.sqrt(lamSqArr_m2)
     freq0_Hz=C/np.sqrt(lam0Sq)
     if stokesIcube is not None:
         idx = np.abs(freqArr_Hz - freq0_Hz).argmin()
         if freqArr_Hz[idx]<freq0_Hz:
             Ifreq0Arr = interp_images(
@@ -93,25 +94,24 @@
 
     else:
         weightArr = np.ones(lamSqArr_m2.shape, dtype=np.float32)
         dFDF = None
 
 
     #Run fitting pixel-wise:
-    progress(40, 0)
-    for i in range(xarr.size):
+    for i in trange(xarr.size):
         FDF_pix=FDF[:,xarr[i],yarr[i]]
         fwhmRMSF_pix=fwhmRMSF[xarr[i],yarr[i]]
         if type(dFDF) == type(None):
             dFDF_pix=None
         else:
             dFDF_pix=dFDF[xarr[i],yarr[i]]
         try:
-            mDict=measure_FDF_parms(FDF_pix, phiArr, fwhmRMSF_pix, dFDF=dFDF_pix, 
-                                lamSqArr_m2=lamSqArr_m2,lam0Sq=lam0Sq, 
+            mDict=measure_FDF_parms(FDF_pix, phiArr, fwhmRMSF_pix, dFDF=dFDF_pix,
+                                lamSqArr_m2=lamSqArr_m2,lam0Sq=lam0Sq,
                                 snrDoBiasCorrect=5.0)
         #Add keywords not included by the above function:
             mDict['lam0Sq_m2']=lam0Sq
             mDict['freq0_Hz']=freq0_Hz
             mDict['fwhmRMSF']=fwhmRMSF_pix
             mDict['Ifreq0']=Ifreq0Arr[xarr[i],yarr[i]]
             mDict['fracPol']=mDict["ampPeakPIfit"]/mDict['Ifreq0']
@@ -125,88 +125,86 @@
                 mDict['dFDFth']=np.nan
             for parameter in product_list:
                 map_dict[parameter][xarr[i],yarr[i]]=mDict[parameter]
         except:
             for parameter in product_list:
                 map_dict[parameter][xarr[i],yarr[i]]=np.nan
 
-        if i % 100 == 0:
-                progress(40, i/xarr.size*100)
     return map_dict
 
 
 
 def delete_FITSheader_axis(fitsheader,axis_number):
     """Deletes FITS keywords associated with the specified axis."""
     axis_keywords=['NAXIS','CRVAL','CRPIX','CDELT','CUNIT','CTYPE']
-    axis_str=str(axis_number)    
+    axis_str=str(axis_number)
     for keyword in axis_keywords:
-        try:            
+        try:
             del fitsheader[keyword+axis_str]
         except:
             pass
-    
+
 
 def save_maps(map_dict, prefix_path,FDFheader):
     """
-    Saves the selected 2D maps of the fit output. 
+    Saves the selected 2D maps of the fit output.
     Inputs:
         map_dict: a dictionary of 2D maps for the fitting outputs.
         prefix_path: the full or relative path to save the files, plus the file
             prefix to be given to the files.
     """
     #Set up generic FITS header
     product_header=FDFheader.copy()
     product_header["NAXIS"] = 2
     #Remove extra axes:
     if 'NAXIS3' in product_header:
         delete_FITSheader_axis(product_header, 3)
     if 'NAXIS4' in product_header:
         delete_FITSheader_axis(product_header, 4)
-    
+
 
     #Set flux unit from FITS header if possible
     if 'BUNIT' in FDFheader:
         flux_unit=FDFheader['BUNIT']
     else:
         flux_unit=''
 
-    
+
     #Dictionary of units for peak fitting output parameters (for FITS headers)
-    unit_dict={"dFDFcorMAD": flux_unit, "dFDFrms": flux_unit, 
+    unit_dict={"dFDFcorMAD": flux_unit, "dFDFrms": flux_unit,
            "phiPeakPIchan_rm2": 'rad/m^2', "dPhiPeakPIchan_rm2": 'rad/m^2',
-           "ampPeakPIchan": flux_unit, "ampPeakPIchanEff": flux_unit, 
-           "dAmpPeakPIchan": flux_unit, 
-           "snrPIchan": '', 
-           "indxPeakPIchan": '', 
-           "peakFDFimagChan": flux_unit, "peakFDFrealChan": flux_unit, 
-           "polAngleChan_deg": 'deg', "dPolAngleChan_deg": 'deg', 
-           "polAngle0Chan_deg": 'deg', "dPolAngle0Chan_deg": 'deg', 
-           "phiPeakPIfit_rm2": 'rad/m^2', "dPhiPeakPIfit_rm2": 'rad/m^2', 
+           "ampPeakPIchan": flux_unit, "ampPeakPIchanEff": flux_unit,
+           "dAmpPeakPIchan": flux_unit,
+           "snrPIchan": '',
+           "indxPeakPIchan": '',
+           "peakFDFimagChan": flux_unit, "peakFDFrealChan": flux_unit,
+           "polAngleChan_deg": 'deg', "dPolAngleChan_deg": 'deg',
+           "polAngle0Chan_deg": 'deg', "dPolAngle0Chan_deg": 'deg',
+           "phiPeakPIfit_rm2": 'rad/m^2', "dPhiPeakPIfit_rm2": 'rad/m^2',
            "ampPeakPIfit": flux_unit, "ampPeakPIfitEff": flux_unit,
-           "dAmpPeakPIfit": flux_unit, 
+           "dAmpPeakPIfit": flux_unit,
            "snrPIfit": '', "indxPeakPIfit": '',
-           "peakFDFimagFit": flux_unit, "peakFDFrealFit": flux_unit, 
-           "polAngleFit_deg": 'deg', "dPolAngleFit_deg": 'deg', 
-           "polAngle0Fit_deg": 'deg', "dPolAngle0Fit_deg": 'deg', 
-           "Ifreq0": flux_unit, "polyCoeffs": "", 
-           "IfitStat": '', "IfitChiSqRed": '', 
-           "lam0Sq_m2": 'm^2', "freq0_Hz": 'Hz', 
-           "fwhmRMSF": 'rad/m^2', "dQU": flux_unit, "dFDFth": flux_unit, 
+           "peakFDFimagFit": flux_unit, "peakFDFrealFit": flux_unit,
+           "polAngleFit_deg": 'deg', "dPolAngleFit_deg": 'deg',
+           "polAngle0Fit_deg": 'deg', "dPolAngle0Fit_deg": 'deg',
+           "Ifreq0": flux_unit, "polyCoeffs": "",
+           "IfitStat": '', "IfitChiSqRed": '',
+           "lam0Sq_m2": 'm^2', "freq0_Hz": 'Hz',
+           "fwhmRMSF": 'rad/m^2', "dQU": flux_unit, "dFDFth": flux_unit,
            "min_freq": 'Hz', "max_freq": 'Hz', "N_channels": '',
-           "median_channel_width": 'Hz', 
-           "fracPol": '', 
+           "median_channel_width": 'Hz',
+           "fracPol": '',
            "sigmaAddQ": '', "dSigmaAddMinusQ": '', "dSigmaAddPlusQ": '',
            "sigmaAddU": '', "dSigmaAddMinusU": '', "dSigmaAddPlusU": ''}
 
 
     #Check that directory exists (in case it is requested to save maps to new subdirectory):
     if not os.path.exists(os.path.dirname(prefix_path)):
         os.mkdir(os.path.dirname(prefix_path))
-    
+
     #per product, customize FITS header as needed and save file
     for product in map_dict.keys():
         if map_dict[product].dtype == np.float_:
             data = map_dict[product].astype(np.float32)
         else:
             data = map_dict[product]
         product_header['BUNIT']=unit_dict[product]
@@ -230,15 +228,15 @@
     return Ndim,FD_axis
 
 def read_files(FDF_filename,freq_filename):
     """
     Read in the files needed for peak fitting. Files assumed to be the standard
     outputs of RMsynth3D (and, optionally, RMclean3D). also, freq file.
     """
-    
+
     HDUreal = pf.open(FDF_filename.replace('_tot','_real').replace('_im','_real'), "readonly", memmap=True)
     head = HDUreal[0].header.copy()
     FDFreal = HDUreal[0].data
 
     HDUimag = pf.open(FDF_filename.replace('_tot','_im').replace('_real','_im'), "readonly", memmap=True)
     FDFimag = HDUimag[0].data
     complex_cube = FDFreal + 1j * FDFimag
@@ -248,55 +246,55 @@
 
     #Move FD axis to first place in numpy order.
     if FD_axis != Ndim:
         complex_cube=np.moveaxis(complex_cube,Ndim-FD_axis,0)
 
     #Remove degenerate axes to prevent problems with later steps.
     complex_cube=complex_cube.squeeze()
-    
+
     lam0Sq=head['LAMSQ0']
-    
+
     freqArr_Hz = np.loadtxt(freq_filename, dtype=float)
     lambdaSqArr_m2 = np.power(C/freqArr_Hz, 2.0)
-    
-    
+
+
     phiArr_radm2 = fits_make_lin_axis(head, axis=FD_axis-1)
-    
+
     HDUfwhm = pf.open(FDF_filename.replace('FDF_tot_dirty','RMSF_FWHM').replace(
         'FDF_real_dirty','RMSF_FWHM').replace('FDF_im_dirty','RMSF_FWHM').replace(
             'FDF_clean_tot','RMSF_FWHM').replace('FDF_clean_real','RMSF_FWHM').replace(
                 'FDF_clean_im','RMSF_FWHM'),
         "readonly", memmap=True)
     fwhmRMSF = HDUfwhm[0].data.squeeze()
 
-    
-    
+
+
     return complex_cube, phiArr_radm2, fwhmRMSF, lambdaSqArr_m2, lam0Sq, head
 
 
 
 
 
 
 def main():
     """
     Start peak fitting from the command line.
     """
 
     import argparse
-    
+
     descStr = """
     Perform pixel-wise fitting of the brightest peak in the FDF. This script
     performs the same fitting used in the RMsynth_1D for every pixel in a 3D
     FDF cube. The result is a set of 2D maps giving the fitting results (one
     map per fitting output). These are saved to a set of FITS files.
     """
 
     epilog_text="""
-    The script saves 2D maps of the parameters from the peak fitting and 
+    The script saves 2D maps of the parameters from the peak fitting and
     FDF characterization function. The user can select how many products are
     saved:
     no flag: a curated list of potentially interesting parameters is saved
          -a: all outputs are saved.
          -p: only parameters that describe the peak are saved.
     """
 
@@ -329,70 +327,70 @@
         sys.exit()
     if not os.path.exists(args.FDF_filename[0]):
         print('Cannot find FDF file. Please check filename/path.')
         sys.exit()
     if not os.path.exists(args.freq_file[0]):
         print('Cannot find frequency file. Please check filename/path.')
         sys.exit()
-    
+
     if args.output_name[0][0] != '/':
         args.output_name[0]='./'+args.output_name[0]
-    
+
     #Define default product lists:
     if args.peak_only:
         product_list=["dFDFcorMAD","phiPeakPIfit_rm2","dPhiPeakPIfit_rm2",
                       "ampPeakPIfitEff","dAmpPeakPIfit","snrPIfit",
                       "polAngle0Fit_deg","dPolAngle0Fit_deg"]
     elif args.all_products:
-        product_list=['dFDFcorMAD', 'dFDFrms', 'phiPeakPIchan_rm2', 
+        product_list=['dFDFcorMAD', 'dFDFrms', 'phiPeakPIchan_rm2',
                       'dPhiPeakPIchan_rm2', 'ampPeakPIchan', 'ampPeakPIchanEff',
                       'dAmpPeakPIchan', 'snrPIchan', 'indxPeakPIchan',
                       'peakFDFimagChan', 'peakFDFrealChan', 'polAngleChan_deg',
-                      'dPolAngleChan_deg', 'polAngle0Chan_deg', 
-                      'dPolAngle0Chan_deg', 'phiPeakPIfit_rm2', 
+                      'dPolAngleChan_deg', 'polAngle0Chan_deg',
+                      'dPolAngle0Chan_deg', 'phiPeakPIfit_rm2',
                       'dPhiPeakPIfit_rm2', 'ampPeakPIfit', 'ampPeakPIfitEff',
-                      'dAmpPeakPIfit', 'snrPIfit', 'indxPeakPIfit', 
-                      'peakFDFimagFit', 'peakFDFrealFit', 'polAngleFit_deg', 
+                      'dAmpPeakPIfit', 'snrPIfit', 'indxPeakPIfit',
+                      'peakFDFimagFit', 'peakFDFrealFit', 'polAngleFit_deg',
                       'dPolAngleFit_deg', 'polAngle0Fit_deg',
                       'dPolAngle0Fit_deg', 'Ifreq0','dFDFth',
-                      'lam0Sq_m2', 'freq0_Hz', 'fwhmRMSF', 
+                      'lam0Sq_m2', 'freq0_Hz', 'fwhmRMSF',
                       'min_freq', 'max_freq', 'N_channels',
                       'median_channel_width', 'fracPol']
     else: #Default option is a curated list of products I think are most useful.
         product_list=["dFDFcorMAD","phiPeakPIfit_rm2","dPhiPeakPIfit_rm2",
                       "ampPeakPIfitEff","dAmpPeakPIfit","snrPIfit",
                       "peakFDFimagFit","peakFDFrealFit",'Ifreq0','lam0Sq_m2',
                       "polAngle0Fit_deg","dPolAngle0Fit_deg"]
 
-    
+
 
     #Read in files
     FDF, phiArr_radm2, fwhmRMSF, lambdaSqArr_m2, lam0Sq, header=read_files(
                                         args.FDF_filename[0],args.freq_file[0])
 
     if args.fitsI is not None:
-        dataI = readFitsCube(args.fitsI, args.verbose)[1]    
+        dataI = readFitsCube(args.fitsI, args.verbose)[1]
     else:
         dataI=None
     if args.noiseFile is not None:
         rmsArr = readFreqFile(args.noiseFile, args.verbose)
     else:
         rmsArr=None
 
     #Fit peaks
     map_dict=pixelwise_peak_fitting(FDF, phiArr_radm2, fwhmRMSF,lambdaSqArr_m2,
                                     lam0Sq,product_list,noiseArr=rmsArr,
                                     stokesIcube=dataI)
-    
+
     save_maps(map_dict, args.output_name[0],header)
-    
-    
-    
-    
 
-    
+
+
+
+
+
 if __name__ == "__main__":
     main()
 
-    
-    
+
+
```

### Comparing `RM-Tools-1.3.0/RMtools_3D/assemble_chunks.py` & `RM-Tools-1.3.1/RMtools_3D/assemble_chunks.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,62 +12,45 @@
 import numpy as np
 import argparse
 import astropy.io.fits as pf
 import os.path as path
 from math import ceil, floor, log10
 from glob import glob
 import re
-#from RMutils.util_misc import progress  
-
-
-def progress(width, percent):
-    """
-    Print a progress bar to the terminal.
-    Stolen from Mike Bell.
-    """
-    import math as m
-    import sys
-    
-    marks = m.floor(width * (percent / 100.0))
-    spaces = m.floor(width - marks)
-    loader = '  [' + ('=' * int(marks)) + (' ' * int(spaces)) + ']'
-    sys.stdout.write("%s %d%%\r" % (loader, percent))
-    if percent >= 100:
-        sys.stdout.write("\n")
-    sys.stdout.flush()
+from tqdm.auto import tqdm, trange
 
 
 def main():
     """This function will assemble a large FITS file or cube from smaller chunks.
     """
 
     descStr="""
     Assemble a FITS image/cube from small pieces. The new image will be created
     in the running directory.
     Supply one of the chunk files (other files will be identified by name pattern).
     Output name will follow the name of the input chunk, minus the '.C??.'
     """
-    
+
     parser = argparse.ArgumentParser(description=descStr,
                              formatter_class=argparse.RawTextHelpFormatter)
-    parser.add_argument("chunkname", metavar="chunk.fits", 
+    parser.add_argument("chunkname", metavar="chunk.fits",
                         help="One of the chunks to be assembled")
     parser.add_argument("-f", dest="output", default=None,
                         help="Specify output file name [basename of chunk]")
     parser.add_argument("-o", dest="overwrite", action="store_true",
                         help="Overwrite existing file? [False].")
 
     args = parser.parse_args()
 
     if args.output == None:
-        output_filename='.'.join([ x for x in args.chunkname.split('.') if not 
+        output_filename='.'.join([ x for x in args.chunkname.split('.') if not
                               (x.startswith('C') and x[1:].isnumeric()) ])
     else:
         output_filename=args.output
-        
+
     #Get all the chunk filenames. Missing chunks will break things!
     filename=re.search('\.C\d+\.',args.chunkname)
     chunkfiles=glob(args.chunkname[0:filename.start()]+'.C*.'+args.chunkname[filename.end():])
     chunkfiles.sort()
 
 
     old_header=pf.getheader(chunkfiles[0])
@@ -98,24 +81,23 @@
         fobj.write(b'\0')
 
 
     if len(chunkfiles) != num_chunks:
         raise Exception('Number of chunk files found does not match expectations!')
 
     base_idx_arr=np.array(range(Nperchunk))
-    
+
     large=pf.open(output_filename,mode='update',memmap=True)
-    
-    for i in range(num_chunks-1):
-        progress(40,i/num_chunks*100)
+
+    for i in trange(num_chunks-1, desc='Assembling chunks'):
         file=chunkfiles[i]
         idx=base_idx_arr+i*Nperchunk
         xarr = idx // y_dim
         yarr = idx % y_dim
-        
+
         chunk=pf.open(file,memmap=True)
         if Ndim == 4:
             large[0].data[:,:,yarr,xarr]=chunk[0].data[:,:,0,:]
         elif Ndim == 3:
             large[0].data[:,yarr,xarr]=chunk[0].data[:,0,:]
         elif Ndim == 2:
             large[0].data[yarr,xarr]=chunk[0].data
@@ -134,17 +116,16 @@
         large[0].data[:,:,yarr,xarr]=chunk[0].data[:,:,0,:]
     elif Ndim == 3:
         large[0].data[:,yarr,xarr]=chunk[0].data[:,0,:]
     elif Ndim == 2:
         large[0].data[yarr,xarr]=chunk[0].data
     large.flush()
     chunk.close()
-    progress(40,100)
 
 
     large.close()
 
 if __name__ == "__main__":
     main()
-    
-    
+
+
```

### Comparing `RM-Tools-1.3.0/RMtools_3D/create_chunks.py` & `RM-Tools-1.3.1/RMtools_3D/create_chunks.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,69 +1,53 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Tue May 28 13:25:30 2019
 
 This code will divide a FITS cube into individual chunks.
-To minimize problems with how to divide the cube, it will convert the image 
+To minimize problems with how to divide the cube, it will convert the image
 plane into a 1D list of spectra.
 Then the file will divided into smaller files, with fewer pixels, in order to
-be run through RM synthesis and CLEAN. 
+be run through RM synthesis and CLEAN.
 A separate routine will re-assemble the individual chunks into a combined file again.
 This code attempts to minimize the memory profile: in principle it should never
 need more memory than the size of a single chunk, and perhaps not even that much.
 
 @author: cvaneck
 May 2019
 """
 
 import numpy as np
 import argparse
 import astropy.io.fits as pf
 import os.path as path
 from math import ceil, floor, log10
-#from RMutils.util_misc import progress  
-
-def progress(width, percent):
-    """
-    Print a progress bar to the terminal.
-    Stolen from Mike Bell.
-    """
-    import math as m
-    import sys
-    
-    marks = m.floor(width * (percent / 100.0))
-    spaces = m.floor(width - marks)
-    loader = '  [' + ('=' * int(marks)) + (' ' * int(spaces)) + ']'
-    sys.stdout.write("%s %d%%\r" % (loader, percent))
-    if percent >= 100:
-        sys.stdout.write("\n")
-    sys.stdout.flush()
+from tqdm.auto import trange
 
 def main():
     """This function will divide a large FITS file or cube into smaller chunks.
     It does so in a memory efficient way that requires only a small RAM overhead
     (approximately 1 chunk worth?).
     """
     descStr="""
     Divide a FITS cube into small pieces for memory-efficient RM synthesis.
     Files will be created in running directory.
     WARNING: ONLY WORKS ON FIRST HDU, OTHERS WILL BE LOST."""
-    
+
     parser = argparse.ArgumentParser(description=descStr,
                              formatter_class=argparse.RawTextHelpFormatter)
-    parser.add_argument("infile", metavar="filename.fits", 
+    parser.add_argument("infile", metavar="filename.fits",
                         help="FITS cube containing data")
-    parser.add_argument("Nperchunk", metavar="N_pixels", 
+    parser.add_argument("Nperchunk", metavar="N_pixels",
                         help="Number of pixels per chunk")
     parser.add_argument("-v", dest="verbose", action="store_true",
                         help="Verbose [False].")
     parser.add_argument("-p", dest="prefix", default=None,
                         help="Prefix of output files [filename]")
-        
+
     args = parser.parse_args()
 
     Nperchunk=int(args.Nperchunk)
 
     if not path.exists(args.infile):
         raise Exception('Input file not found!')
 
@@ -74,38 +58,37 @@
 
 
 
 
     hdu=pf.open(args.infile,memmap=True)
     header=hdu[0].header
     data=np.transpose(hdu[0].data)
-    
+
     x_image=header['NAXIS1']
     y_image=header['NAXIS2']
     Npix_image=x_image*y_image
 
     num_chunks=ceil(Npix_image/Nperchunk)
     digits=floor(log10(num_chunks))+1
     prntcode=':0'+str(digits)+'d'
-    
-    if args.verbose: 
+
+    if args.verbose:
         print(('Chunk name set to "{}.C{'+prntcode+'}.fits"').format(prefix,0))
         print('File will be divided into {} chunks'.format(num_chunks))
 
     base_idx_arr=np.array(range(Nperchunk))
 
     new_header=header.copy()
     new_header['NAXIS2']=1
     new_header['NAXIS1']=Nperchunk
     new_header['OLDXDIM']=x_image
     new_header['OLDYDIM']=y_image
 
     #Run for all but last. Last chunk requires some finessing.
-    for i in range(num_chunks-1):
-        progress(40,i/num_chunks*100)
+    for i in trange(num_chunks-1, desc="Creating chunks"):
         idx=base_idx_arr+i*Nperchunk
         xarr = idx // y_image
         yarr = idx % y_image
         newdata=np.expand_dims(data[xarr,yarr],1)
         filename=('{}.C{'+prntcode+'}.fits').format(prefix,i)
         pf.writeto(filename,np.transpose(newdata),new_header,overwrite=True)
 
@@ -119,9 +102,9 @@
     pf.writeto(filename,np.transpose(newdata),new_header,overwrite=True)
 
     hdu.close()
 
 
 if __name__ == "__main__":
     main()
-    
-    
+
+
```

### Comparing `RM-Tools-1.3.0/RMtools_3D/do_RMclean_3D.py` & `RM-Tools-1.3.1/RMtools_3D/do_RMclean_3D.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_3D/do_RMsynth_3D.py` & `RM-Tools-1.3.1/RMtools_3D/do_RMsynth_3D.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,31 +36,33 @@
 
 import sys
 import os
 import time
 import math as m
 import numpy as np
 import astropy.io.fits as pf
+import astropy.table as at
 
 from RMutils.util_RM import do_rmsynth_planes
 from RMutils.util_RM import get_rmsf_planes
 from RMutils.util_misc import interp_images
 
 
 if sys.version_info.major == 2:
     print('RM-tools will no longer run with Python 2! Please use Python 3.')
     exit()
 
 C = 2.997924538e8 # Speed of light [m/s]
 
 #-----------------------------------------------------------------------------#
+
 def run_rmsynth(dataQ, dataU, freqArr_Hz, dataI=None, rmsArr=None,
                 phiMax_radm2=None, dPhi_radm2=None, nSamples=10.0,
                 weightType="uniform", fitRMSF=False, nBits=32, verbose=True, not_rmsf = False,
-                log = print):
+                log = print, super_resolution=False):
 
     """Run RM-synthesis on 2/3D data.
 
     Args:
       dataQ (array_like): Stokes Q intensity cube.
       dataU (array_like): Stokes U intensity cube.
       freqArr_Hz (array_like): Frequency of each channel in Hz.
@@ -111,15 +113,18 @@
     dFreq_Hz = np.nanmin(np.abs(np.diff(freqArr_Hz)))
     lambdaSqRange_m2 = ( np.nanmax(lambdaSqArr_m2) -
                          np.nanmin(lambdaSqArr_m2) )
     dLambdaSqMin_m2 = np.nanmin(np.abs(np.diff(lambdaSqArr_m2)))
     dLambdaSqMax_m2 = np.nanmax(np.abs(np.diff(lambdaSqArr_m2)))
 
     # Set the Faraday depth range
-    fwhmRMSF_radm2 = 2.0 * m.sqrt(3.0) / lambdaSqRange_m2
+    if not super_resolution:
+        fwhmRMSF_radm2 = 3.8 / lambdaSqRange_m2 #Dickey+2019 theoretical RMSF width
+    else: #If super resolution, use R&C23 theoretical width
+        fwhmRMSF_radm2 = 2.0 / (np.nanmax(lambdaSqArr_m2) + np.nanmin(lambdaSqArr_m2))
     if dPhi_radm2 is None:
         dPhi_radm2 = fwhmRMSF_radm2 / nSamples
     if phiMax_radm2 is None:
         phiMax_radm2 = m.sqrt(3.0) / dLambdaSqMax_m2
         phiMax_radm2 = max(phiMax_radm2, fwhmRMSF_radm2*10.)    # Force the minimum phiMax to 10 FWHM
 
     # Faraday depth sampling. Zero always centred on middle channel
@@ -156,80 +161,68 @@
     # Perform RM-synthesis on the cube
     FDFcube, lam0Sq_m2 = do_rmsynth_planes(dataQ           = qArr,
                                            dataU           = uArr,
                                            lambdaSqArr_m2  = lambdaSqArr_m2,
                                            phiArr_radm2    = phiArr_radm2,
                                            weightArr       = weightArr,
                                            nBits           = 32,
-                                           verbose         = verbose)
+                                           verbose         = verbose,
+                                           lam0Sq_m2       = 0 if super_resolution else None,
+                                           )
     # Calculate the Rotation Measure Spread Function cube
     if not_rmsf is not True:
         RMSFcube, phi2Arr_radm2, fwhmRMSFCube, fitStatArr = \
             get_rmsf_planes(lambdaSqArr_m2   = lambdaSqArr_m2,
                             phiArr_radm2     = phiArr_radm2,
                             weightArr        = weightArr,
                             mskArr           = ~np.isfinite(dataQ),
                             lam0Sq_m2        = lam0Sq_m2,
                             double           = True,
-                            fitRMSF          = fitRMSF,
-                            fitRMSFreal      = False,
+                            fitRMSF          = fitRMSF or super_resolution,
+                            fitRMSFreal      = super_resolution,
                             nBits            = 32,
                             verbose          = verbose,
                             log              = log)
     endTime = time.time()
     cputime = (endTime - startTime)
     if(verbose): log("> RM-synthesis completed in %.2f seconds." % cputime)
 
 
     # Determine the Stokes I value at lam0Sq_m2 from the Stokes I model
     # Note: the Stokes I model MUST be continuous throughout the cube,
     # i.e., no NaNs as the amplitude at freq0_Hz is interpolated from the
     # nearest two planes.
     with np.errstate(divide='ignore', invalid='ignore'):
-        freq0_Hz = np.true_divide(C , m.sqrt(lam0Sq_m2))
-                                  
+        freq0_Hz = np.true_divide(C , m.sqrt(lam0Sq_m2)) if lam0Sq_m2 > 0 else np.nanmean(freqArr_Hz)
+
     if dataI is not None:
         idx = np.abs(freqArr_Hz - freq0_Hz).argmin()
         if freqArr_Hz[idx]<freq0_Hz:
             Ifreq0Arr = interp_images(dataI[idx, :, :], dataI[idx+1, :, :], f=0.5)
         elif freqArr_Hz[idx]>freq0_Hz:
             Ifreq0Arr = interp_images(dataI[idx-1, :, :], dataI[idx, :, :], f=0.5)
         else:
             Ifreq0Arr = dataI[idx, :, :]
 
         # Multiply the dirty FDF by Ifreq0 to recover the PI
         FDFcube *= Ifreq0Arr
 
-
     if not_rmsf:
         dataArr = [FDFcube, phiArr_radm2, lam0Sq_m2, lambdaSqArr_m2]
 
     else:
         dataArr = [FDFcube, phiArr_radm2, RMSFcube, phi2Arr_radm2, fwhmRMSFCube,fitStatArr, lam0Sq_m2, lambdaSqArr_m2]
 
     return dataArr
+    
 
 def writefits(dataArr, headtemplate, fitRMSF=False, prefixOut="", outDir="",
-                nBits = 32, write_seperate_FDF=False, not_rmsf=False, verbose=False, log=print):
+                nBits = 32, write_seperate_FDF=True, not_rmsf=False, verbose=False, log=print):
     """Write data to disk in FITS
 
-
-    Output files:
-        Default:
-        FDF_dirty.fits: FDF, in 3 extensions: Q,U, and PI.
-        FDF_maxPI.fits: 2D map of peak polarized intensity per pixel.
-        FDF_peakRM.fits: 2D map of Faraday depth of highest peak, per pixel.
-        RMSF.fits: 4 extensions; first 3 are RMSF cubes [Q, U, PI]
-                                 4th is 2D map of RMSF FWHM.
-        write_seperate_FDF=True:
-        FDF_dirty.fits is split into three constituent components:
-            FDF_real_dirty.fits: Stokes Q
-            FDF_im_dirty.fits: Stokes U
-            FDF_tot_dirty.fits: Polarizd Intensity (sqrt(Q^2+U^2))
-
     Args:
       dataArr (list): FDF and RMSF information
         if not_rmsf:
             dataArr = [FDFcube, phiArr_radm2, lam0Sq_m2, lambdaSqArr_m2]
         else:
             dataArr = [FDFcube, phiArr_radm2, RMSFcube, phi2Arr_radm2, fwhmRMSFCube,fitStatArr, lam0Sq_m2, lambdaSqArr_m2]
 
@@ -240,24 +233,47 @@
         prefixOut (str): Prefix for filenames.
         outDir (str): Directory to save files.
         write_seperate_FDF (bool): Write Q, U, and PI separately?
         verbose (bool): Verbosity.
         not_rmsf (bool): Just do RM synthesis and ignore RMSF?
         log (function): Which logging function to use.
 
+
+    Output files:
+        Default:
+        FDF_maxPI.fits: 2D map of peak polarized intensity per pixel.
+        FDF_peakRM.fits: 2D map of Faraday depth of highest peak, per pixel.
+
+        write_seperate_FDF=True: [default]
+        FDF_dirty.fits is split into three constituent components:
+            FDF_real_dirty.fits: Stokes Q
+            FDF_im_dirty.fits: Stokes U
+            FDF_tot_dirty.fits: Polarizd Intensity (sqrt(Q^2+U^2))
+            RMSF_real.fits: Real/Stokes Q component of RMSF
+            RMSF_im.fits: Imaginary/Stokes U component of RMSF
+            RM_tot.fits: polarized intensity view of RMSF
+            RMSF_FWHM.fits: 2D map of width of RMSF main lobe
+
+        write_seperate_FDF=False:
+            FDF_dirty.fits: FDF, in 3 extensions: Q,U, and PI.
+            RMSF.fits: 4 extensions; first 3 are RMSF cubes [Q, U, PI]
+                                 4th is 2D map of RMSF FWHM.
+
+
     """
     if not_rmsf:
         FDFcube, phiArr_radm2, lam0Sq_m2, lambdaSqArr_m2 = dataArr
 
     else:
         FDFcube, phiArr_radm2, RMSFcube, phi2Arr_radm2, fwhmRMSFCube,fitStatArr, lam0Sq_m2, lambdaSqArr_m2 = dataArr
 
-    # Default data types
+    # Default data typess
     dtFloat = "float" + str(nBits)
     dtComplex = "complex" + str(2*nBits)
+    
 
     if(verbose): log("Saving the dirty FDF, RMSF and ancillary FITS files.")
     # Make a copy of the Q header and alter frequency-axis as Faraday depth
     header = headtemplate.copy()
     Ndim=header['NAXIS']
     freq_axis=Ndim #If frequency axis not found, assume it's the last one.
     #Check for frequency axes. Because I don't know what different formatting
@@ -335,15 +351,18 @@
 
     #Header for outputs that are RM maps (peakRM, RMSF_FWHM)
 
 
     # Save the RMSF
     if not_rmsf is not True:
         header["NAXIS"+str(freq_axis)] = phi2Arr_radm2.size
-        header["CRVAL"+str(freq_axis)] = (phi2Arr_radm2[0],'[rad/m^2] Coordinate value at reference point')
+        header["CDELT"+str(freq_axis)] = (np.diff(phi2Arr_radm2)[0], '[rad/m^2] Coordinate increment at reference point')
+        header["CRPIX"+str(freq_axis)] = phi2Arr_radm2.size//2+1
+        header["CRVAL"+str(freq_axis)] = (phi2Arr_radm2[phi2Arr_radm2.size//2], '[rad/m^2] Coordinate value at reference point')
+
         header["DATAMAX"] = np.max(fwhmRMSFCube) + 1
         header["DATAMIN"] = np.max(fwhmRMSFCube) - 1
         rmheader=header.copy()
         rmheader['BUNIT']='rad/m^2'
         #Because there can be problems with different axes having different FITS keywords,
         #don't try to remove the FD axis, but just make it degenerate.
         # Also requires np.expand_dims to set the correct NAXIS.
@@ -380,30 +399,28 @@
             hdu2 = pf.ImageHDU(np.abs(RMSFcube).astype(dtFloat), header)
             hdu3 = pf.ImageHDU(fwhmRMSFCube.astype(dtFloat), rmheader)
             hduLst = pf.HDUList([hdu0, hdu1, hdu2, hdu3])
             if(verbose): log("> %s" % fitsFileOut)
             hduLst.writeto(fitsFileOut, output_verify="fix", overwrite=True)
             hduLst.close()
 
-
-
     #Because there can be problems with different axes having different FITS keywords,
     #don't try to remove the FD axis, but just make it degenerate.
     # Also requires np.expand_dims to set the correct NAXIS.
     header["NAXIS"+str(freq_axis)] = 1
     header["CRVAL"+str(freq_axis)] = (phiArr_radm2[0], '[rad/m^2] Coordinate value at reference point')
     if "DATAMAX" in header:
         del header["DATAMAX"]
     if "DATAMIN" in header:
         del header["DATAMIN"]
 
 
 
     #Generate peak maps:
-        
+
     maxPI,peakRM = create_peak_maps(FDFcube,phiArr_radm2,Ndim-freq_axis)
     # Save a maximum polarised intensity map
     fitsFileOut = outDir + "/" + prefixOut + "FDF_maxPI.fits"
     if(verbose): log("> %s" % fitsFileOut)
     pf.writeto(fitsFileOut,
                 np.expand_dims(maxPI.astype(dtFloat), axis=0),
                 header,
@@ -431,31 +448,31 @@
     """Finds the location and amplitude of the highest peak in the FDF (pixelwise)
     and returns maps of those parameters. Does not fit the peak, only finds
     the location in terms of the quantized Faraday depth slices of the cube.
     Used to produce the maxPI and peakRM maps.
     Inputs:
         FDFcube: output cube from run_rmsynth
         phiArr_radm2: array of Faraday depth values, from run_rmsynth
-        phi_axis (int): number of the axis for Faraday depth (in python order, 
+        phi_axis (int): number of the axis for Faraday depth (in python order,
                          not FITS order). Defaults to zero (first axis).
     Returns:
         maxPI: array of same dimensions as FDFcube exceppt collapsed along
                 first (Faraday depth) axis, containing the maximum polarized
                 intensity for each pixel
         peakRM: as maxPI, but with the Faraday depth location of the peak
     """
-    
+
     maxPI=np.max(np.abs(FDFcube), axis=phi_axis)
     peakRM_indices = np.argmax(np.abs(FDFcube), axis=phi_axis)
     peakRM=phiArr_radm2[peakRM_indices]
-    
+
     return maxPI, peakRM
 
-    
-    
+
+
 
 
 
 def find_freq_axis(header):
     """Finds the frequency axis in a FITS header.
     Input: header: a Pyfits header object.
     Returns the axis number (as recorded in the FITS file, **NOT** in numpy ordering.)
@@ -498,15 +515,15 @@
     N_dim=head['NAXIS'] #Get number of axes
     if verbose:
         print('Dimensions of the input cube are: ',end=' ')
         for i in range(1,N_dim+1):
             print('NAXIS{} = {}'.format(i,head['NAXIS'+str(i)]),end='  ')
         print()
 
-    freq_axis=find_freq_axis(head) 
+    freq_axis=find_freq_axis(head)
     #If the frequency axis isn't the last one, rotate the array until it is.
     #Recall that pyfits reverses the axis ordering, so we want frequency on
     #axis 0 of the numpy array.
     if freq_axis != 0 and freq_axis != N_dim:
         data=np.moveaxis(data,N_dim-freq_axis,0)
 
     if N_dim >= 4:
@@ -571,31 +588,34 @@
     parser.add_argument("freqFile", metavar="freqs_Hz.dat", nargs=1,
                         help="ASCII file containing the frequency vector.")
     parser.add_argument("-i", dest="fitsI", default=None,
                         help="FITS cube containing Stokes I model [None].")
     parser.add_argument("-n", dest="noiseFile", default=None,
                         help="Text file containing channel noise values [None].")
     parser.add_argument("-w", dest="weightType", default="uniform",
-                        help="weighting [uniform] (all 1s) or 'variance'.")
+                        help="weighting ['uniform'] (all 1s) or 'variance'.")
     parser.add_argument("-t", dest="fitRMSF", action="store_true",
                         help="Fit a Gaussian to the RMSF [False]")
     parser.add_argument("-l", dest="phiMax_radm2", type=float, default=None,
                         help="Absolute max Faraday depth sampled (overrides NSAMPLES) [Auto].")
     parser.add_argument("-d", dest="dPhi_radm2", type=float, default=None,
                         help="Width of Faraday depth channel [Auto].")
     parser.add_argument("-o", dest="prefixOut", default="",
                         help="Prefix to prepend to output files [None].")
     parser.add_argument("-s", dest="nSamples", type=float, default=5,
                         help="Number of samples across the FWHM RMSF.")
     parser.add_argument("-f", dest="write_seperate_FDF", action="store_false",
-                        help="Store different Stokes as FITS extensions [False, store as seperate files].")
+                        help="Store different Stokes as FITS extensions [False, store as separate files].")
     parser.add_argument("-v", dest="verbose", action="store_true",
                         help="Verbose [False].")
     parser.add_argument("-R", dest="not_RMSF", action="store_true",
                         help="Skip calculation of RMSF? [False]")
+    parser.add_argument("-r", "--super-resolution", action="store_true",
+                        help="Optimise the resolution of the RMSF (as per Rudnick & Cotton). "
+                        )
     args = parser.parse_args()
 
     # Sanity checks
     for f in args.fitsQ + args.fitsU:
         if not os.path.exists(f):
             print("File does not exist: '%s'." % f)
             sys.exit()
@@ -621,15 +641,17 @@
                           phiMax_radm2 = args.phiMax_radm2,
                           dPhi_radm2   = args.dPhi_radm2,
                           nSamples     = args.nSamples,
                           weightType   = args.weightType,
                           fitRMSF      = args.fitRMSF,
                           nBits        = 32,
                           verbose      = verbose,
-                          not_rmsf = args.not_RMSF)
+                          not_rmsf = args.not_RMSF,
+                          super_resolution=args.super_resolution,
+                        )
 
     # Write to files
     writefits(dataArr,
               headtemplate       = header,
               fitRMSF            = False,
               prefixOut          = args.prefixOut,
               outDir             = dataDir,
```

### Comparing `RM-Tools-1.3.0/RMtools_3D/do_fitIcube.py` & `RM-Tools-1.3.1/RMtools_3D/do_fitIcube.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #!/usr/bin/env python
 #=============================================================================#
 #                                                                             #
 # NAME:     do_fitIcube.py                                                    #
 #                                                                             #
 # PURPOSE:  Make a model Stokes I cube and a noise vector.                    #
 #                                                                             #
-# MODIFIED: 26-Feb-2017 by C. Purcell                                         #
+# MODIFIED: 26-Feb-2017 by C. Purcell
+# MODIFIED: 18 January 2023 by Lerato Baidoo  (re-structured and optimized)   #
 #                                                                             #
 #=============================================================================#
 #                                                                             #
 # The MIT License (MIT)                                                       #
 #                                                                             #
 # Copyright (c) 2016 Cormac R. Purcell                                        #
 #                                                                             #
@@ -37,20 +38,20 @@
 import os
 import time
 import traceback
 import argparse
 import math as m
 import numpy as np
 import astropy.io.fits as pf
+from tqdm.auto import tqdm, trange
 
 from RMutils.util_misc import MAD
 from RMutils.util_misc import fit_StokesI_model, calculate_StokesI_model
-from RMutils.util_misc import progress
 from RMutils.util_FITS import strip_fits_dims
-from RMtools_3D.do_RMsynth_3D import readFitsCube 
+from RMtools_3D.do_RMsynth_3D import readFitsCube
 from RMtools_3D.make_freq_file import  get_freq_array
 
 
 from functools import partial
 import multiprocessing as mp
 
 #-----------------------------------------------------------------------------#
@@ -59,395 +60,453 @@
     """
     Start the make_model_I function if called from the command line.
     """
 
     # Help string to be shown using the -h option
     descStr = """
     Create a model Stokes I dataset by fitting a polynomial to emitting regions
-    above a cutoff in the Stokes I cube. Also outputs a noise spectrum with the
-    Stokes I noise per channel.
+    above a cutoff threshold in the Stokes I cube. Also outputs a noise spectrum
+    with the Stokes I noise per channel.
 
     NOTE: Each pixel is fit independently, so there are no protections in place
     to ensure smoothness across the image-plane. Noise levels are estimated
     per-channel using 2 passes of the MAD.
     """
 
     # Parse the command line options
     parser = argparse.ArgumentParser(description=descStr,
                                  formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument("fitsI", metavar="StokesI.fits", nargs=1,
                         help="FITS cube containing Stokes I data.")
+    parser.add_argument("-freqFile", dest="freq_file", default="",type=str,
+                       help="Path + ASCII file containing the frequency vector. If not provided,\nfrequencies are derived from fits header.")
     parser.add_argument("-f", dest="fit_function", type=str, default="log",
                         help="Stokes I fitting function: 'linear' or ['log'] polynomials.")
     parser.add_argument("-p", dest="polyOrd", type=int, default=2,
                         help="polynomial order to fit to I spectrum: 0-5 supported, 2 is default.\nSet to negative number to enable dynamic order selection.")
     parser.add_argument("-c", dest="cutoff", type=float, default=-5,
                         help="emission cutoff (+ve = abs, -ve = sigma) [-5].")
     parser.add_argument("-t", dest="threshold", type=float, default=3,
                         help="threshold in factors of sigma used to estimate rms noise. Default is 3.")
     parser.add_argument("-n", dest="num_cores", type=int, default=10,
                         help="Number of cores to use for multiprocessing. Default is 10.")
     parser.add_argument("-m", dest="apply_mask", action='store_true',
                         help="Apply masking before spectral fitting. Default is False.")
     parser.add_argument("-o", dest="prefixOut", default="",
-                        help="Prefix to prepend to output files [None].")
+                        help="Prefix to use for to output file names.")
+    parser.add_argument("-odir", dest="outDir", default="",
+                        help="Output directory to save output files. If none, save inside input directory")
     parser.add_argument("-v", dest="verbose", action="store_true",
                         help="turn on verbose messages [False].")
     args = parser.parse_args()
-    
+
     # Sanity checks
     for f in [args.fitsI[0]]:
         if not os.path.exists(f):
             print("File does not exist: '%s'." % f)
             sys.exit()
-    dataDir, dummy = os.path.split(args.fitsI[0])
-    
+    out_directory = args. outDir
+    if not out_directory:
+        out_directory, dummy = os.path.split(args.fitsI[0])
+
     I_filename = args.fitsI[0]
-    
     datacube, headI = open_datacube(fitsI=I_filename, verbose=args.verbose)
-    freqArr_Hz = get_freq_array (I_filename) 
-       
+
+    #if frequency file is not provided, extract frequency information from the input fits header.
+    if args.freq_file:
+        freqArr_Hz = get_frequencies(datacube=datacube, header=headI, freqFile=args.freq_file)
+    else:
+        print("Frequency file not provided. Deriving frequencies from the fits header.")
+        freqArr_Hz = get_freq_array (I_filename)
+
     # Run polynomial fitting on the spectra
-    make_model_I(datacube     = datacube, 
-                 header       = headI, 
+    make_model_I(datacube     = datacube,
+                 header       = headI,
                  freqArr_Hz   = freqArr_Hz,
                  polyOrd      = args.polyOrd,
-                 cutoff       = args.cutoff,
                  prefixOut    = args.prefixOut,
-                 outDir       = dataDir,
+                 outDir       = out_directory,
                  nBits        = 32,
                  threshold    = args.threshold,
                  apply_mask   = args.apply_mask,
                  num_cores    = args.num_cores,
                  verbose        = args.verbose,
                  fit_function = args.fit_function)
 
 
 #-----------------------------------------------------------------------------#
 
 
 def open_datacube(fitsI, verbose=True):
+    """ Reads the image fits
+
+    Parameters:
+    fitsI : Input Stokes I cube fits image
+    verbose: If true, write logs
+
+    Returns:
+    datacube: Image data
+    header: Fits header
+    """
 
     # Default data type
-    
+
     # Sanity check on header dimensions
     print("Reading FITS cube header from '%s':" % fitsI)
     header, datacube = readFitsCube(fitsI, verbose)
-    
+
     nDim = datacube.ndim
     if nDim < 3 or nDim > 4:
-        print("Err: only 3 or 4 dimensions supported: D = %d." % headI["NAXIS"])
+        print("Err: only 3 or 4 dimensions supported: D = %d." % header["NAXIS"])
         sys.exit()
 
-    # freq_axis=find_freq_axis(headI) 
+    # freq_axis=find_freq_axis(header)
     # #If the frequency axis isn't the last one, rotate the array until it is.
     # #Recall that pyfits reverses the axis ordering, so we want frequency on
     # #axis 0 of the numpy array.
     # if freq_axis != 0 and freq_axis != nDim:
     #     datacube=np.moveaxis(datacube,nDim-freq_axis,0)
-    
+
     return datacube, header
-    
-    
-def get_frequencies(datacube, headI, freqFile):
 
-    nBits = np.abs(headI['BITPIX'])    
+
+def get_frequencies(datacube, header, freqFile):
+
+    """ Reads a frequency file
+
+    Parameters:
+    datacube: Image cube data
+    header: A header of the input datacube
+    freqFile: A frequency file in text format
+
+    Returns:
+    freqArr_Hz: frequency array
+    """
+
+    nBits = np.abs(header['BITPIX'])
     dtFloat = "float" + str(nBits)
 
     nChan = datacube.shape[0] # for now, assumes frequency is the first axis
-    
+
     # Read the frequency vector
     print("Reading frequency vector from '%s'." % freqFile)
     freqArr_Hz = np.loadtxt(freqFile, dtype=dtFloat)
     if nChan!=len(freqArr_Hz):
         print("Err: frequency vector and frequency axis of cube unequal length.")
         sys.exit()
-        
+
     return freqArr_Hz
-   
-   
-def cube_noise(datacube, header, freqArr_Hz, cutoff=-1, threshold=3):
 
 
+def cube_noise(datacube, header, freqArr_Hz, threshold=-5):
+
+
+    """Estimates noise of each channel in an image cube.
+
+    Parameters:
+    datacube: Input cube data
+    header : Header of a cube image
+    frequency: Frequency values of a cube image in Hz
+    threshold: Threshold to use for masking off pixels.
+            If the value is +ve, then it is taken as absolute value, and
+            -ve as sigma. E.g. threshold=-5, means consider pixels
+            with emission > noise_median - 5 * rms_noise.
+            Where the noise_median and rms_noise are obtained by computing
+            the median and MAD of the pixel emission > image median + 3 * image MAD.
+
+    Returns:
+    rms_Arr: An array containing rms values of each channel
+    mskSrc:  A 2D image data containing masking values (0s and 1s)
     """
-    Estimate channel noise of a cube data. Returns rms values and a mask 2D data.
-     
-    datacube: input cube data.
-    header : header of a cube image
-    frequency: frequency values of a cube image in Hz.
-    cutoff : cut off to use for creating the final mask. +ve cutoff means absolute, -ve sigma. 
-    threshold : Sigma cut off to use to remove emission pixels before calculating rms_noise.  
-     
-    """
-    nBits=np.abs(header['BITPIX'])    
-    dtFloat = "float" + str(nBits)    
+    nBits=np.abs(header['BITPIX'])
+    dtFloat = "float" + str(nBits)
     nChan = datacube.shape[0]
-    
+
 
     if nChan!=len(freqArr_Hz):
         print("Err: frequency vector and frequency axis of cube unequal length.")
         sys.exit()
-        
+
     # Measure the RMS spectrum using 2 passes of MAD on each plane
-    # Determine which pixels have emission above the cutoff
+    # Determine which pixels have emission above the threshold
     print("Measuring the RMS noise and creating an emission mask")
     rmsArr = np.zeros_like(freqArr_Hz)
     medSky = np.zeros_like(freqArr_Hz)
     mskSrc = np.zeros((header["NAXIS2"], header["NAXIS1"]), dtype=dtFloat)
-    
+
     start = time.time()
     for i in range(nChan):
         dataPlane = datacube[i]
-        if cutoff>0:
-            idxSky = np.where(dataPlane<cutoff)
+        if threshold >0:
+            idxSky = np.where(dataPlane<threshold) #replaced cutoff with threshold
         else:
             idxSky = np.where(dataPlane)
-        
+
         # Pass 1
         rmsTmp = MAD(dataPlane[idxSky])
         medTmp = np.nanmedian(dataPlane[idxSky])
-        
+
         # Pass 2: use a fixed 3-sigma cutoff to mask off emission
-        
-        idxSky = np.where(dataPlane < medTmp + rmsTmp * threshold)
+        idxSky = np.where(dataPlane < medTmp + rmsTmp * 3)
         medSky[i] = np.nanmedian(dataPlane[idxSky])
         rmsArr[i] = MAD(dataPlane[idxSky])
 
-        
-        # When building final emission mask treat +ve cutoffs as absolute
-        # values and negative cutoffs as sigma values
-        if cutoff > 0:
-            idxSrc = np.where(dataPlane > cutoff)
+
+        # When building final emission mask treat +ve threshold as absolute
+        # values and negative threshold as sigma values
+        if threshold > 0:
+            idxSrc = np.where(dataPlane > threshold)
         else:
-            idxSrc = np.where(dataPlane > medSky[i] -1 * rmsArr[i] * cutoff)
+            idxSrc = np.where(dataPlane > medSky[i] -1 * rmsArr[i] * threshold)
 
         mskSrc[idxSrc] +=1
 
     end = time.time()
     print(' For loop masking takes %.3fs'%(end-start))
     return rmsArr, mskSrc
 
-    
-    
-def channel_noise(chan, datacube, header, cutoff, threshold, nBits):
-    
-    dtFloat = "float" + str(nBits)    
- 
-    mask_channel = np.zeros((header["NAXIS2"], header["NAXIS1"]), dtype=dtFloat)
-    
-    dataPlane = datacube[chan]
-    if cutoff > 0:
-        idxSky = np.where(dataPlane < cutoff)
-    else:
-        idxSky = np.where(dataPlane)
-        
-    # Pass 1
-    rmsTmp = MAD(dataPlane[idxSky])
-    medTmp = np.nanmedian(dataPlane[idxSky])
-    idxSky = np.where(dataPlane < medTmp + rmsTmp * threshold)
-    
-    rms_noise    = MAD(dataPlane[idxSky])
-    median_noise =  np.nanmedian(dataPlane[idxSky])
-    
-    if cutoff > 0:
-        idxSrc = np.where(dataPlane > cutoff)
-    else:
-        idxSrc = np.where(dataPlane > median_noise -1 * rms_noise * cutoff)
-    mask_channel[idxSrc] = 1
-    
-    outs_noise = dict()
-    outs_noise['rms_noise']    = rms_noise
-    outs_noise['mask_data']    = mask_channel
-    
-    return outs_noise 
-    
-    
-    
+
 def savefits_mask(data, header, outDir, prefixOut):
-    
-       
+
+    """ Save the derived mask to a fits file
+
+    data:  2D data defining the mask.
+    header: header to describe the mask
+    outDir: directory to save the mask fits data
+    prefixOut: prefix to use on the output name
+    """
+
     headMask = strip_fits_dims(header=header, minDim=2)
     headMask["DATAMAX"] = 1
     headMask["DATAMIN"] = 0
     del headMask["BUNIT"]
-    
+
     mskArr = np.where(data > 0, 1.0, np.nan)
-    MaskfitsFile = outDir + "/"  + prefixOut + "Mask.fits"
+    MaskfitsFile = outDir + "/"  + prefixOut + "_mask.fits"
     print("> %s" % MaskfitsFile)
     pf.writeto(MaskfitsFile, mskArr, headMask, output_verify="fix",
                overwrite=True)
 
 
 def savefits_Coeffs(data, dataerr, header, polyOrd, outDir, prefixOut):
 
-                   
+    """ Save the derived coefficients to a fits file
+
+    data: 2D planes containing coeffs values.
+    dataerr: 2D planes containing error in coeffs values.
+    header: header to describe the coeffs and error in coeffs
+    polyOrd: the order of polynomial to fit
+    outDir: directory to save the (errors) coeffs fits data
+    prefixOut: prefix to use on the output name
+    """
+
     headcoeff = strip_fits_dims(header=header, minDim=2)
     del headcoeff["BUNIT"]
-    
+
     for i in range(np.abs(polyOrd)+1):
-        outname = outDir + "/"  + prefixOut + 'Icoeff'+str(i) + '.fits'
+        outname = outDir + "/"  + prefixOut + '_coeff'+str(i) + '.fits'
         pf.writeto(outname, data[i], headcoeff, overwrite=True)
-        
-        outname = outDir + "/"  + prefixOut + 'Icoeff'+str(i) + '_err.fits'
+
+        outname = outDir + "/"  + prefixOut + '_coeff'+str(i) + 'err.fits'
         pf.writeto(outname, dataerr[i], headcoeff, overwrite=True)
 
 
-    
+
 def savefits_model_I(data, header, outDir, prefixOut):
-    
-    
+
+    """ Save the derived Stokes cube model
+
+    data:  Stokes I cube model data
+    header: header to describe the model cube.
+    outDir: directory to save the model cube fits data
+    prefixOut: prefix to use on the output name
+    """
+
+
     nDim = data.ndim
     nBits = np.abs(header['BITPIX'])
-    
+
     headModelCube = strip_fits_dims(header=header, minDim=nDim)
     headModelCube["NAXIS1"] = header["NAXIS1"]
     headModelCube["NAXIS2"] = header["NAXIS2"]
     headModelCube["NAXIS3"] = header["NAXIS3"]
-    
+
     nVoxels = header["NAXIS1"] * header["NAXIS2"] * header["NAXIS3"]
     if nDim == 4:
         headModelCube["NAXIS4"] = header["NAXIS4"]
         nVoxels *= header["NAXIS4"]
     while len(headModelCube) < (36 * 4 - 1):
         headModelCube.append()
-        
-    fitsModelFile = outDir + "/"  + prefixOut + "Imodel.fits"
+
+    fitsModelFile = outDir + "/"  + prefixOut + "model.i.fits"
     headModelCube.tofile(fitsModelFile, overwrite=True)
     with open(fitsModelFile, "rb+") as f:
         f.seek(len(headModelCube.tostring()) + (nVoxels*int(nBits/8)) - 1)
         f.write(b"\0")
     HDULst = pf.open(fitsModelFile, "update", memmap=True)
     HDULst[0].data = data
     HDULst.close()
 
 
-def fit_spectra_I(xy, datacube, freqArr_Hz, rms_Arr, polyOrd, 
-                 fit_function, nDetectPix, verbose=True):
-    
-    i, x, y = xy 
-    
+def fit_spectra_I(xy, datacube, freqArr_Hz, rms_Arr, polyOrd,
+                 fit_function, nDetectPix, pbar, verbose=True):
+    """ Fits polynomial function to Stokes I data
+
+    xy: Position of pixel to fit (in pixels).
+        The xy consists of pixel number, x and y pixel position.
+    datacube:  Stokes I data cube to model.
+    freqArr_Hz: Frequency array in Hz.
+    rms_Arr: An array containing rms values of each channel.
+    polyOrd: the order of polynomial to fit.
+    fit_function: A type of function to fit.
+         It can be log or linear.
+    nDetectPix:  the total number of pixels to be fit.
+    """
+
+    i, x, y = xy
+
     Ispectrum = datacube[:, x, y]
-    
+
     pixFitDict = fit_StokesI_model(freqArr_Hz, Ispectrum, rms_Arr,
                  polyOrd=polyOrd, fit_function=fit_function)
-        
+
     pixImodel = calculate_StokesI_model(pixFitDict, freqArr_Hz)
-        
+
     outs = dict()
-        
+
     outs['I'] = pixImodel
     outs['coeffs'] = pixFitDict['p']
     outs['coeffs_err'] = pixFitDict['perror']
     outs['chiSq']    = pixFitDict['chiSq']
     outs['chiSqRed'] = pixFitDict['chiSqRed']
     outs['nIter']    = pixFitDict['nIter']
     outs['AIC']      = pixFitDict['AIC']
-    
-    if verbose:
-       progress(40, i/nDetectPix*100.)
-    
-    return outs         
-       
-
-def make_model_I(datacube, header, freqArr_Hz, polyOrd=2, cutoff=-1,  
-                 nBits=32, threshold=3, num_cores = 10,verbose=True, fit_function='log', 
-                 apply_mask=False, outDir=None, prefixOut=None):  
-                
-                 
-    """
-    Estimates Stokes I model data by fitting polynomial function and predicting I
-    using the derived coeffiencients. 
-    
-    datacube:  Stokes I data cube.
-    header: header of the data cube. 
-    freqArr_Hz: frequency values of the cube in Hz. 
-    polyOrd: the order of the polynomial to fit. 0-5 supported, 2 is default.
-    fit_function: fit log or linear.
-    
-    apply_mask: if true a mask will be applied. 
-    See channel_noise for definitions of cutoff, threshold.
-    
+
+    pbar.update(1)
+
+    return outs
+
+def make_model_I(datacube, header, freqArr_Hz, polyOrd=2,
+                 nBits=32, threshold=3, num_cores = 10,verbose=True,
+                 fit_function='log', apply_mask=False, outDir=None,
+                 prefixOut=None):
+
+
+    """Fits a polynomial function to Stokes I data, derives coefficients,
+       predicts model I, and save the respective fits file.
+
+    datacube:  Stokes I data cube
+    header: header of the data cube
+    freqArr_Hz: frequency values of the cube in Hz
+    polyOrd: the order of the polynomial to fit. 0-5 supported, 2 is default
+    fit_function: fit log or linear
+
+    num_cores: Number of cores to use for parallel processing
+    verbose: Write to log
+    apply_mask: If true, a mask will be applied
+    threshold: Threshold to use for masking off pixels
+
+            If the value is +ve, then it is taken as absolute value, and
+            -ve as sigma. E.g. threshold=-5, means consider pixels
+            with emission > noise_median - 5 * rms_noise.
+            Where the noise_median and rms_noise are obtained by computing
+            the median and MAD of the pixel emission > image median + 3 * image MAD
+    outDir: Directory to save all outputs
+    prefixOut: Prefix name to use in all output names
+
+    Returns:
+    ModelIcube: Model I cube data array
+    Mask fits data
+    Coefficients fits data
+    Error in coefficients fits data
     """
+
     nChan = datacube.shape[0]
-    dtFloat = "float" + str(nBits) 
-    
-    rms_Arr, mskSrc = cube_noise(datacube, header, freqArr_Hz, cutoff=cutoff,
+    dtFloat = "float" + str(nBits)
+
+    rms_Arr, mskSrc = cube_noise(datacube, header, freqArr_Hz,
             threshold=threshold)
-    
+
     mskArr = np.where(mskSrc > 0, 1.0, np.nan)
-        
+
     if not apply_mask:
         mskSrc = np.ones((header['naxis2'], header['naxis1']), dtype=dtFloat)
         mskArr = np.where(mskSrc > 0, 1.0, np.nan)
 
     srcCoords = np.rot90(np.where(mskSrc > 0))
-    
+
     nPix = mskSrc.shape[-1] * mskSrc.shape[-2]
     nDetectPix = len(srcCoords)
-    
+
     if verbose:
         print("Emission present in %d spectra (%.1f percent)." % \
               (nDetectPix, (nDetectPix*100.0/nPix)))
 
     modelIcube = np.zeros_like(datacube)
     modelIcube[:] = np.nan
     results = []
-    
+
     coeffs = np.array([mskArr] * 6)
     coeffs_error = np.array([mskArr] * 6)
     datacube = np.squeeze(datacube)
-   
+
     # Inform user job magnitude
     startTime = time.time()
-    
+
     xy = list(zip(np.arange(1, len(srcCoords)), srcCoords[:, 0], srcCoords[:, 1]))
-    #print(xy)
-    
-    if verbose:
-        print("Fitting %d/%d spectra." % (nDetectPix, nPix))
-        progress(40, 0)
-        
-    with mp.Pool(num_cores) as pool_:
-        results = pool_.map( partial(fit_spectra_I, datacube=datacube, freqArr_Hz=freqArr_Hz, 
-                    rms_Arr=rms_Arr, polyOrd=polyOrd, fit_function=fit_function,
-                    nDetectPix=nDetectPix),
-           xy)
-    
+
+    with mp.Pool(num_cores) as pool_, tqdm(total=nDetectPix, desc=f"Fitting {nDetectPix}/{nPix} spectra", disable=not verbose) as pbar:
+        results = pool_.map(
+            partial(
+                fit_spectra_I,
+                datacube=datacube,
+                freqArr_Hz=freqArr_Hz,
+                rms_Arr=rms_Arr,
+                polyOrd=polyOrd,
+                fit_function=fit_function,
+                nDetectPix=nDetectPix,
+                pbar=pbar,
+            ),
+            xy
+        )
+
     results = list(results)
-    
+
     #print(results)
     headcoeff = strip_fits_dims(header=header, minDim=2)
     del headcoeff["BUNIT"]
-                   
+
     endTime = time.time()
     cputime = (endTime - startTime)
     print("Fitting completed in %.2f seconds." % cputime)
-    
-    print('Saving results ...')
+
+
     for _, an in enumerate(xy):
         i, x, y =  an
-        
+
         modelIcube[:, x, y] =  results[_]['I']
-        
-        for k,j,l in zip(range(len(coeffs)), results[_]['coeffs'], 
+
+        for k,j,l in zip(range(len(coeffs)), results[_]['coeffs'],
                          results[_]['coeffs_err']):
-            coeffs[5-k,x,y] = j     
-            coeffs_error[5-k,x,y] = l         
+            coeffs[5-k,x,y] = j
+            coeffs_error[5-k,x,y] = l
+
 
-    #if apply_mask:
-    print('Saving mask image.')
+    print("Saving mask image.")
     savefits_mask(data=mskSrc, header=header, outDir=outDir, prefixOut=prefixOut)
+
     print("Saving model I coefficients.")
     savefits_Coeffs(data=coeffs, dataerr=coeffs_error, header=header,
-         polyOrd=polyOrd, outDir=outDir, prefixOut=prefixOut)
+             polyOrd=polyOrd, outDir=outDir, prefixOut=prefixOut)
+
     print("Saving model I cube image. ")
-    savefits_model_I(data=modelIcube, header=header, 
-         outDir=outDir, prefixOut=prefixOut)
-        
+    savefits_model_I(data=modelIcube, header=header,
+             outDir=outDir, prefixOut=prefixOut)
+
     return modelIcube
-    
 
 
-    
+
+
 #-----------------------------------------------------------------------------#
 if __name__ == "__main__":
     main()
```

### Comparing `RM-Tools-1.3.0/RMtools_3D/extract_region.py` & `RM-Tools-1.3.1/RMtools_3D/extract_region.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_3D/make_freq_file.py` & `RM-Tools-1.3.1/RMtools_3D/make_freq_file.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMtools_3D/mk_test_cube_data.py` & `RM-Tools-1.3.1/RMtools_3D/mk_test_cube_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,43 +77,43 @@
 import os
 import sys
 import argparse
 import shutil
 import math as m
 import numpy as np
 import astropy.wcs.wcs as pw
+from tqdm.auto import tqdm, trange
 
 from RMutils.util_misc import twodgaussian
 from RMutils.util_misc import create_IQU_spectra_burn
-from RMutils.util_misc import create_IQU_spectra_diff 
+from RMutils.util_misc import create_IQU_spectra_diff
 from RMutils.util_misc import csv_read_to_list
 from RMutils.util_misc import split_repeat_lst
 from RMutils.util_misc import calc_stats
-from RMutils.util_misc import progress
 from RMutils.util_misc import extrap
 from RMutils.util_FITS import strip_fits_dims
 from RMutils.util_FITS import create_simple_fits_hdu
 
 C = 2.99792458e8
 
 #-----------------------------------------------------------------------------#
 def main():
     """
     Start the create_IQU_fits_data function if called from the command line.
     """
-    
+
     # Help string to be shown using the -h option
     descStr = """
-    Create a new dataset directory and populate it with data cubes in FITS 
-    format. Three FITS files are produced, one for each of the Stokes I, Q 
+    Create a new dataset directory and populate it with data cubes in FITS
+    format. Three FITS files are produced, one for each of the Stokes I, Q
     and U parameters. A vector of frequency channels is also saved as an
     ASCII file 'freqs_Hz.dat'.
-    
+
     The data is populated with polarised sources whose properties are given
-    in an external CSV-format catalogue file. Two types of model may be 
+    in an external CSV-format catalogue file. Two types of model may be
     specified, assuming a total flux & spectral index:
 
         # MODEL TYPE 1: One or more components affected by Burn depolarisation.
         #
         # Column  |  Description
         #---------------------------------------------------
         # [0]     |  Model type [1]
@@ -171,19 +171,19 @@
     function of frequency (i.e., assumes all data has been convolved to the
     same resolution). Please edit the variables at the top of the script to
     change the properties of the output data.
 
     Examples:
 
     ./mk_test_cube_data.py catalogue.csv data/
-    
+
     ./mk_test_cube_data.py catalogue.csv -f 1.10e9,1.20e9,1.60e9,1.65e9
-    
+
     ./mk_test_cube_data.py catalogue.csv -n NOISE.TXT
-    
+
     """
 
     # Parse the command line options
     parser = argparse.ArgumentParser(description=descStr,
                                  formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument("inCatFile", metavar="catalogue.csv", nargs=1,
                         help="Input catalogue file in CSV format")
@@ -208,15 +208,15 @@
             "Warn: Failed to parse frequency flagging string!"
 
     # Read the RMS noise template
     try:
         noiseTmpArr = np.loadtxt(noiseTmpFile, unpack=True)
     except Exception:
         noiseTmpArr = None
-    
+
     # Call the function to create FITS data
     nSrc = create_IQU_cube_data(dataPath, inCatFile, startFreq_Hz, endFreq_Hz,
                                 nChans, rmsNoise, beamMinFWHM_deg,
                                 beamMajFWHM_deg, beamPA_deg, pixScale_deg,
                                 xCent_deg, yCent_deg, nPixX, nPixY,
                                 coordSys, noiseTmpArr, flagRanges_Hz)
 
@@ -237,30 +237,30 @@
     dFreq_Hz = (endFreq_Hz - startFreq_Hz)/ (nChans-1)
     print("\nSampling frequencies %.2f - %.2f MHz by %.2f MHz." % \
           (freqArr_Hz[0]/1e6, freqArr_Hz[-1]/1e6, dFreq_Hz/1e6))
     if len(flagRanges_Hz)>0:
         print("Flagging frequency ranges:")
         print("> ", flagRanges_Hz)
     for i in range(len(freqArr_Hz)):
-        for fRng in flagRanges_Hz:            
+        for fRng in flagRanges_Hz:
             if freqArr_Hz[i]>=fRng[0] and freqArr_Hz[i]<=fRng[1]:
                 freqArr_Hz[i]=np.nan
 
     # Create normalised noise array from a template or assume all ones.
     if noiseTmpArr is None:
         print("Assuming flat noise versus frequency curve.")
         noiseArr = np.ones(freqArr_Hz.shape, dtype="f4")
     else:
         print("Scaling noise curve by external template.")
         xp = noiseTmpArr[0]
         yp = noiseTmpArr[1]
         mDict = calc_stats(yp)
         yp /= mDict["median"]
         noiseArr = extrap(freqArr_Hz, xp, yp)
-        
+
     # Check the catalogue file exists
     if not os.path.exists(inCatFile):
         print("Err: File does not exist '%s'." % inCatFile)
         sys.exit()
     catInLst = csv_read_to_list(inCatFile, doFloat=True)
     print("Found %d entries in the catalogue." % len(catInLst))
 
@@ -296,100 +296,97 @@
     head2D = strip_fits_dims(header=hduI.header, minDim=2, forceCheckDims=4)
     wcs2D = pw.WCS(head2D)
     shape2D = (nPixY, nPixX)
     hduQ = hduI.copy()
     hduQ.header["CRVAL4"] = 2.0
     hduU = hduI.copy()
     hduU.header["CRVAL4"] = 3.0
-    
+
     # Calculate some beam parameters
     gfactor = 2.0*m.sqrt(2.0*m.log(2.0))
     beamMinSigma_deg = beamMinFWHM_deg/gfactor
     beamMajSigma_deg = beamMajFWHM_deg/gfactor
     beamMinSigma_pix = beamMinSigma_deg/pixScale_deg
     beamMajSigma_pix = beamMajSigma_deg/pixScale_deg
     beamPA_rad = m.radians(beamPA_deg)
-    
+
     # Loop through the sources, calculate the spectra and pixel position
     spectraILst = []
     spectraQLst = []
     spectraULst = []
     coordLst_deg = []
     coordLst_pix = []
     successCount = 0
     for i in range(len(catInLst)):
         e = catInLst[i]
         modelType = int(e[0])
 
         # Type 1 = multiple Burn depolarisation affected components
         if modelType==1:
-            
+
             # Parse the parameters of multiple components
             preLst, parmArr = split_repeat_lst(e[1:],7,4)
-            
+
             # Create the model spectra from multiple thin components
             # modified by external depolarisation
             IArr, QArr, UArr = \
                 create_IQU_spectra_burn(freqArr_Hz = freqArr_Hz,
-                                        fluxI = preLst[5], 
+                                        fluxI = preLst[5],
                                         SI = preLst[6],
                                         fracPolArr = parmArr[0],
                                         psi0Arr_deg = parmArr[1],
                                         RMArr_radm2 = parmArr[2],
                                         sigmaRMArr_radm2 = parmArr[3],
                                         freq0_Hz = freq0_Hz)
-                
+
         # Type 2 = multiple internal depolarisation affected components
         elif modelType==2:
-            
+
             # Parse the parameters of multiple components
             preLst, parmArr = split_repeat_lst(e[1:],7,3)
-            
+
             # Create the model spectra from multiple components
             # modified by internal Faraday depolarisation
             IArr, QArr, UArr = \
                 create_IQU_spectra_diff(freqArr_Hz = freqArr_Hz,
-                                        fluxI = preLst[5], 
+                                        fluxI = preLst[5],
                                         SI = preLst[6],
                                         fracPolArr = parmArr[0],
                                         psi0Arr_deg = parmArr[1],
                                         RMArr_radm2 = parmArr[2],
                                         freq0_Hz = freq0_Hz)
         else:
             continue
-        
+
         spectraILst.append(IArr)
         spectraQLst.append(QArr)
         spectraULst.append(UArr)
-        coordLst_deg.append([preLst[0], preLst[1]])        
+        coordLst_deg.append([preLst[0], preLst[1]])
         [ (x_pix, y_pix) ] = wcs2D.wcs_world2pix([ (preLst[0], preLst[1]) ], 0)
-        coordLst_pix.append([x_pix, y_pix])        
+        coordLst_pix.append([x_pix, y_pix])
         successCount +=1
 
     # Loop through the frequency channels & insert the IQU planes
-    print("Looping through %d frequency channels:" % nChans)
-    progress(40, 0.0)    
-    for iChan in range(len(freqArr_Hz)):
-        progress(40, (100.0 * (iChan + 1) / nChans))
-        for iSrc in range(len(spectraILst)):
+    for iChan, _ in enumerate(tqdm(freqArr_Hz), desc=f"Looping through {nChans} frequency channels"):
+        for iSrc, _ in enumerate(spectraILst):
             params = [spectraILst[iSrc][iChan],  # amplitude
                       coordLst_pix[iSrc][0],     # X centre (pix)
                       coordLst_pix[iSrc][1],     # Y centre
                       beamMinSigma_pix,          # width (sigma)
                       beamMajSigma_pix,          # height (sigma)
                       beamPA_rad]                # PA (rad) W of N (clockwise)
             planeI = twodgaussian(params, shape2D).reshape((nPixY, nPixX))
             params[0] = spectraQLst[iSrc][iChan]
             planeQ = twodgaussian(params, shape2D).reshape((nPixY, nPixX))
             params[0] = spectraULst[iSrc][iChan]
             planeU = twodgaussian(params, shape2D).reshape((nPixY, nPixX))
             hduI.data[0, iChan, :, :] += planeI
             hduQ.data[0, iChan, :, :] += planeQ
             hduU.data[0, iChan, :, :] += planeU
-        
+
         # Add the noise
         hduI.data[0, iChan, :, :] += (np.random.normal(scale=rmsNoise,
                                       size=(nPixY, nPixX))* noiseArr[iChan])
         hduQ.data[0, iChan, :, :] += (np.random.normal(scale=rmsNoise,
                                       size=(nPixY, nPixX))* noiseArr[iChan])
         hduU.data[0, iChan, :, :] += (np.random.normal(scale=rmsNoise,
                                       size=(nPixY, nPixX))* noiseArr[iChan])
@@ -428,14 +425,14 @@
     print("> %s" % fitsFileOut)
     hduU.writeto(fitsFileOut, overwrite=True)
 
     # Save a vector of frequency values
     freqFileOut =  dataPath + "/freqs_Hz.dat"
     print("> %s" % freqFileOut)
     np.savetxt(freqFileOut,freqNoFlgArr_Hz)
-    
+
     return successCount
 
 
 #-----------------------------------------------------------------------------#
 if __name__=="__main__":
     main()
```

### Comparing `RM-Tools-1.3.0/RMutils/corner.py` & `RM-Tools-1.3.1/RMutils/corner.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMutils/mpfit.py` & `RM-Tools-1.3.1/RMutils/mpfit.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMutils/nestle.py` & `RM-Tools-1.3.1/RMutils/nestle.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMutils/normalize.py` & `RM-Tools-1.3.1/RMutils/normalize.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMutils/util_FITS.py` & `RM-Tools-1.3.1/RMutils/util_FITS.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMutils/util_RM.py` & `RM-Tools-1.3.1/RMutils/util_RM.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,29 +66,29 @@
 from scipy.stats import kurtosis
 from scipy.stats import skew
 from scipy.stats import skewtest
 from scipy.stats import kurtosistest
 from scipy.stats import anderson
 from scipy.stats import kstest
 from scipy.stats import norm
+from tqdm.auto import tqdm, trange
 
 from RMutils.mpfit import mpfit
-from RMutils.util_misc import progress  
 from RMutils.util_misc import toscalar
 from RMutils.util_misc import calc_parabola_vertex
 from RMutils.util_misc import create_pqu_spectra_burn
 from RMutils.util_misc import calc_mom2_FDF
 from RMutils.util_misc import MAD
 
 # Constants
 C = 2.99792458e8
 
 
 #-----------------------------------------------------------------------------#
-def do_rmsynth_planes(dataQ, dataU, lambdaSqArr_m2, phiArr_radm2, 
+def do_rmsynth_planes(dataQ, dataU, lambdaSqArr_m2, phiArr_radm2,
                       weightArr=None, lam0Sq_m2=None, nBits=32, verbose=False,
                       log=print):
     """Perform RM-synthesis on Stokes Q and U cubes (1,2 or 3D). This version
     of the routine loops through spectral planes and is faster than the pixel-
     by-pixel code. This version also correctly deals with isolated clumps of
     NaN-flagged voxels within the data-cube (unlikely in interferometric cubes,
     but possible in single-dish cubes). Input data must be in standard python
@@ -98,26 +98,26 @@
     dataU           ... 1, 2 or 3D Stokes U data array
     lambdaSqArr_m2  ... vector of wavelength^2 values (assending freq order)
     phiArr_radm2    ... vector of trial Faraday depth values
     weightArr       ... vector of weights, default [None] is Uniform (all 1s)
     nBits           ... precision of data arrays [32]
     verbose         ... print feedback during calculation [False]
     log             ... function to be used to output messages [print]
-    
+
     """
-    
+
     # Default data types
     dtFloat = "float" + str(nBits)
     dtComplex = "complex" + str(2*nBits)
 
     # Set the weight array
     if weightArr is None:
         weightArr = np.ones(lambdaSqArr_m2.shape, dtype=dtFloat)
     weightArr = np.where(np.isnan(weightArr), 0.0, weightArr)
-    
+
     # Sanity check on array sizes
     if not weightArr.shape  == lambdaSqArr_m2.shape:
         log("Err: Lambda^2 and weight arrays must be the same shape.")
         return None, None
     if not dataQ.shape == dataU.shape:
         log("Err: Stokes Q and U data arrays must be the same shape.")
         return None, None
@@ -125,108 +125,103 @@
     if not nDims <= 3:
         log("Err: data dimensions must be <= 3.")
         return None, None
     if not dataQ.shape[0] == lambdaSqArr_m2.shape[0]:
         log("Err: Data depth does not match lambda^2 vector ({} vs {}).".format(dataQ.shape[0], lambdaSqArr_m2.shape[0]), end=' ')
         log("     Check that data is in [z, y, x] order.")
         return None, None
-    
+
     # Reshape the data arrays to 3 dimensions
     if nDims==1:
         dataQ = np.reshape(dataQ, (dataQ.shape[0], 1, 1))
         dataU = np.reshape(dataU, (dataU.shape[0], 1, 1))
     elif nDims==2:
         dataQ = np.reshape(dataQ, (dataQ.shape[0], dataQ.shape[1], 1))
         dataU = np.reshape(dataU, (dataU.shape[0], dataU.shape[1], 1))
-    
+
     # Create a complex polarised cube, B&dB Eqns. (8) and (14)
     # Array has dimensions [nFreq, nY, nX]
     pCube = (dataQ + 1j * dataU) * weightArr[:, np.newaxis, np.newaxis]
-    
+
     # Check for NaNs (flagged data) in the cube & set to zero
     mskCube = np.isnan(pCube)
     pCube = np.nan_to_num(pCube)
-    
+
     # If full planes are flagged then set corresponding weights to zero
     mskPlanes =  np.sum(np.sum(~mskCube, axis=1), axis=1)
     mskPlanes = np.where(mskPlanes==0, 0, 1)
     weightArr *= mskPlanes
-    
+
     # Initialise the complex Faraday Dispersion Function cube
     nX = dataQ.shape[-1]
     nY = dataQ.shape[-2]
     nPhi = phiArr_radm2.shape[0]
     FDFcube = np.zeros((nPhi, nY, nX), dtype=dtComplex)
 
     # lam0Sq_m2 is the weighted mean of lambda^2 distribution (B&dB Eqn. 32)
     # Calculate a global lam0Sq_m2 value, ignoring isolated flagged voxels
     K = 1.0 / np.sum(weightArr)
     if lam0Sq_m2 is None:
         lam0Sq_m2 = K * np.sum(weightArr * lambdaSqArr_m2)
     if not np.isfinite(lam0Sq_m2): #Can happen if all channels are NaNs/zeros
         lam0Sq_m2=0.
-    
+
     # The K value used to scale each FDF spectrum must take into account
     # flagged voxels data in the datacube and can be position dependent
     weightCube =  np.invert(mskCube) * weightArr[:, np.newaxis, np.newaxis]
     with np.errstate(divide='ignore', invalid='ignore'):
         KArr = np.true_divide(1.0, np.sum(weightCube, axis=0))
         KArr[KArr == np.inf] = 0
         KArr = np.nan_to_num(KArr)
-        
+
     # Do the RM-synthesis on each plane
-    if verbose:
-        log("Running RM-synthesis by channel.")
-        progress(40, 0)
     a = lambdaSqArr_m2 - lam0Sq_m2
-    for i in range(nPhi):
-        if verbose:
-            progress(40, ((i+1)*100.0/nPhi))
+    for i in trange(nPhi, desc="Running RM-synthesis by channel", disable=not verbose):
         arg = np.exp(-2.0j * phiArr_radm2[i] * a)[:, np.newaxis,np.newaxis]
         FDFcube[i,:,:] =  KArr * np.sum(pCube * arg, axis=0)
-        
+
     # Remove redundant dimensions in the FDF array
     FDFcube = np.squeeze(FDFcube)
 
     return FDFcube, lam0Sq_m2
 
 
 #-----------------------------------------------------------------------------#
-def get_rmsf_planes(lambdaSqArr_m2, phiArr_radm2, weightArr=None, mskArr=None, 
+def get_rmsf_planes(lambdaSqArr_m2, phiArr_radm2, weightArr=None, mskArr=None,
                     lam0Sq_m2= None, double=True, fitRMSF=False,
                     fitRMSFreal=False, nBits=32, verbose=False,
                     log=print):
     """Calculate the Rotation Measure Spread Function from inputs. This version
     returns a cube (1, 2 or 3D) of RMSF spectra based on the shape of a
     boolean mask array, where flagged data are True and unflagged data False.
     If only whole planes (wavelength channels) are flagged then the RMSF is the
     same for all pixels and the calculation is done once and replicated to the
     dimensions of the mask. If some isolated voxels are flagged then the RMSF
     is calculated by looping through each wavelength plane, which can take some
     time. By default the routine returns the analytical width of the RMSF main
     lobe but can also use MPFIT to fit a Gaussian.
-    
+
     lambdaSqArr_m2  ... vector of wavelength^2 values (assending freq order)
     phiArr_radm2    ... vector of trial Faraday depth values
-    weightArr       ... vector of weights, default [None] is no weighting    
+    weightArr       ... vector of weights, default [None] is no weighting
     maskArr         ... cube of mask values used to shape return cube [None]
     lam0Sq_m2       ... force a reference lambda^2 value (def=calculate) [None]
     double          ... pad the Faraday depth to double-size [True]
     fitRMSF         ... fit the main lobe of the RMSF with a Gaussian [False]
     fitRMSFreal     ... fit RMSF.real, rather than abs(RMSF) [False]
     nBits           ... precision of data arrays [32]
     verbose         ... print feedback during calculation [False]
     log             ... function to be used to output messages [print]
 
     """
-    
+
     # Default data types
     dtFloat = "float" + str(nBits)
     dtComplex = "complex" + str(2*nBits)
-    
+
     # For cleaning the RMSF should extend by 1/2 on each side in phi-space
     if double:
         nPhi = phiArr_radm2.shape[0]
         nExt = np.ceil(nPhi/2.0)
         resampIndxArr = np.arange(2.0 * nExt + nPhi) - nExt
         phi2Arr = extrap(resampIndxArr, np.arange(nPhi, dtype='int'),
                          phiArr_radm2)
@@ -241,156 +236,148 @@
     # Set the mask array (default to 1D, no masked channels)
     if mskArr is None:
         mskArr = np.zeros_like(lambdaSqArr_m2, dtype="bool")
         nDims = 1
     else:
         mskArr = mskArr.astype("bool")
         nDims = len(mskArr.shape)
-    
+
     # Sanity checks on array sizes
     if not weightArr.shape  == lambdaSqArr_m2.shape:
         log("Err: wavelength^2 and weight arrays must be the same shape.")
         return None, None, None, None
     if not nDims <= 3:
         log("Err: mask dimensions must be <= 3.")
         return None, None, None, None
     if not mskArr.shape[0] == lambdaSqArr_m2.shape[0]:
-        log("Err: mask depth does not match lambda^2 vector (%d vs %d).", end=' ')
-        (mskArr.shape[0], lambdaSqArr_m2.shape[-1])
+        log(f"Err: mask depth does not match lambda^2 vector ({mskArr.shape[0]} vs {lambdaSqArr_m2.shape[-1]}).", end=' ')
         log("     Check that the mask is in [z, y, x] order.")
         return None, None, None, None
-    
+
     # Reshape the mask array to 3 dimensions
     if nDims==1:
         mskArr = np.reshape(mskArr, (mskArr.shape[0], 1, 1))
     elif nDims==2:
         mskArr = np.reshape(mskArr, (mskArr.shape[0], mskArr.shape[1], 1))
-    
+
     # Create a unit cube for use in RMSF calculation (negative of mask)
     #CVE: unit cube removed: it wasn't accurate for non-uniform weights, and was no longer used
-    
+
     # Initialise the complex RM Spread Function cube
     nX = mskArr.shape[-1]
     nY = mskArr.shape[-2]
     nPix = nX * nY
     nPhi = phi2Arr.shape[0]
     RMSFcube = np.ones((nPhi, nY, nX), dtype=dtComplex)
 
     # If full planes are flagged then set corresponding weights to zero
     xySum =  np.sum(np.sum(mskArr, axis=1), axis=1)
     mskPlanes = np.where(xySum==nPix, 0, 1)
     weightArr *= mskPlanes
-    
+
     # Check for isolated clumps of flags (# flags in a plane not 0 or nPix)
     flagTotals = np.unique(xySum).tolist()
     try:
         flagTotals.remove(0)
     except Exception:
         pass
     try:
         flagTotals.remove(nPix)
     except Exception:
         pass
     do1Dcalc = True
     if len(flagTotals)>0:
         do1Dcalc = False
-    
+
     # lam0Sq is the weighted mean of LambdaSq distribution (B&dB Eqn. 32)
     # Calculate a single lam0Sq_m2 value, ignoring isolated flagged voxels
     K = 1.0 / np.nansum(weightArr)
-    lam0Sq_m2 = K * np.nansum(weightArr * lambdaSqArr_m2)
+    if lam0Sq_m2 is None:
+        lam0Sq_m2 = K * np.nansum(weightArr * lambdaSqArr_m2)
 
-    # Calculate the analytical FWHM width of the main lobe    
+    # Calculate the analytical FWHM width of the main lobe
     fwhmRMSF = 3.8/(np.nanmax(lambdaSqArr_m2) -
                                   np.nanmin(lambdaSqArr_m2))
 
     # Do a simple 1D calculation and replicate along X & Y axes
     if do1Dcalc:
         if verbose:
             log("Calculating 1D RMSF and replicating along X & Y axes.")
 
         # Calculate the RMSF
         a = (-2.0 * 1j * phi2Arr).astype(dtComplex)
         b = (lambdaSqArr_m2 - lam0Sq_m2)
         RMSFArr = K * np.sum(weightArr * np.exp( np.outer(a, b) ), 1)
-        
+
         # Fit the RMSF main lobe
         fitStatus = -1
         if fitRMSF:
             if verbose:
                 log("Fitting Gaussian to the main lobe.")
-            if fitRMSFreal:
-                mp = fit_rmsf(phi2Arr, RMSFArr.real)
-            else:
-                mp = fit_rmsf(phi2Arr, np.abs(RMSFArr))
+            mp = fit_rmsf(
+                phi2Arr,
+                RMSFArr.real if fitRMSFreal else np.abs(RMSFArr)
+            )
             if mp is None or mp.status<1:
-                 pass
                  log("Err: failed to fit the RMSF.")
                  log("     Defaulting to analytical value.")
             else:
                 fwhmRMSF = mp.params[2]
                 fitStatus = mp.status
 
         # Replicate along X and Y axes
         RMSFcube = np.tile(RMSFArr[:, np.newaxis, np.newaxis], (1, nY, nX))
         fwhmRMSFArr = np.ones((nY,nX), dtype=dtFloat) * fwhmRMSF
         statArr = np.ones((nY, nX), dtype="int") * fitStatus
 
     # Calculate the RMSF at each pixel
     else:
         if verbose:
-            log("Calculating RMSF by channel.")
+            log()
 
         # The K value used to scale each RMSF must take into account
         # isolated flagged voxels data in the datacube
         weightCube =  np.invert(mskArr) * weightArr[:, np.newaxis, np.newaxis]
         with np.errstate(divide='ignore', invalid='ignore'):
             KArr = np.true_divide(1.0, np.sum(weightCube, axis=0))
             KArr[KArr == np.inf] = 0
             KArr = np.nan_to_num(KArr)
 
         # Calculate the RMSF for each plane
-        if verbose:
-            progress(40, 0)
         a = (lambdaSqArr_m2 - lam0Sq_m2)
-        for i in range(nPhi):
-            if verbose:
-                progress(40, ((i+1)*100.0/nPhi))
+        for i in trange(nPhi, desc="Calculating RMSF by channel", disable=not verbose):
             arg = np.exp(-2.0j * phi2Arr[i] * a)[:, np.newaxis, np.newaxis]
             RMSFcube[i, :, :] = KArr * np.sum(weightCube * arg, axis=0)
 
         # Default to the analytical RMSF
         fwhmRMSFArr = np.ones((nY, nX), dtype=dtFloat) * fwhmRMSF
         statArr = np.ones((nY, nX), dtype="int") * (-1)
-    
+
         # Fit the RMSF main lobe
         if fitRMSF:
             if verbose:
                 log("Fitting main lobe in each RMSF spectrum.")
                 log("> This may take some time!")
-                progress(40, 0)
             k = 0
-            for i in range(nX):
+            for i in trange(nX, desc="Fitting RMSF by pixel", disable=not verbose):
                 for j in range(nY):
                     k += 1
-                    if verbose:
-                        progress(40, ((i+1)*100.0/nPhi))
                     if fitRMSFreal:
                         mp = fit_rmsf(phi2Arr, RMSFcube[:,j,i].real)
                     else:
                         mp = fit_rmsf(phi2Arr, np.abs(RMSFcube[:, j, i]))
                     if not (mp is None or mp.status < 1):
                         fwhmRMSFArr[j, i] = mp.params[2]
                         statArr[j, i] = mp.status
 
     # Remove redundant dimensions
     RMSFcube = np.squeeze(RMSFcube)
     fwhmRMSFArr = np.squeeze(fwhmRMSFArr)
     statArr = np.squeeze(statArr)
-    
+
     return RMSFcube, phi2Arr, fwhmRMSFArr, statArr
 
 
 #-----------------------------------------------------------------------------#
 def do_rmclean_hogbom(dirtyFDF, phiArr_radm2, RMSFArr, phi2Arr_radm2,
                       fwhmRMSFArr, cutoff, maxIter=1000, gain=0.1,
                       mskArr=None, nBits=32, verbose=False, doPlots=False,
@@ -420,43 +407,43 @@
     # Default data types
     dtFloat = "float" + str(nBits)
     dtComplex = "complex" + str(2*nBits)
 
     # Sanity checks on array sizes
     nPhi = phiArr_radm2.shape[0]
     if nPhi != dirtyFDF.shape[0]:
-        log("Err: 'phi2Arr_radm2' and 'dirtyFDF' are not the same length.")
-        return None, None, None
+        log("Err: 'phiArr_radm2' and 'dirtyFDF' are not the same length.")
+        return None, None, None, None
     nPhi2 = phi2Arr_radm2.shape[0]
     if not nPhi2 == RMSFArr.shape[0]:
         log("Err: missmatch in 'phi2Arr_radm2' and 'RMSFArr' length.")
-        return None, None, None
+        return None, None, None, None
     if not (nPhi2 >= 2 * nPhi):
         log("Err: the Faraday depth of the RMSF must be twice the FDF.")
-        return None, None, None
+        return None, None, None, None
     nDims = len(dirtyFDF.shape)
     if not nDims <= 3:
         log("Err: FDF array dimensions must be <= 3.")
-        return None, None, None
+        return None, None, None, None
     if not nDims == len(RMSFArr.shape):
         log("Err: the input RMSF and FDF must have the same number of axes.")
-        return None, None, None
+        return None, None, None, None
     if not RMSFArr.shape[1:] == dirtyFDF.shape[1:]:
         log("Err: the xy dimesions of the RMSF and FDF must match.")
-        return None, None, None
+        return None, None, None, None
     if mskArr is not None:
         if not mskArr.shape == dirtyFDF.shape[1:]:
             log("Err: pixel mask must match xy dimesnisons of FDF cube.")
             log("     FDF[z,y,z] = {:}, Mask[y,x] = {:}.".format(
                 dirtyFDF.shape, mskArr.shape), end=' ')
 
-            return None, None, None
+            return None, None, None, None
     else:
-        mskArr = np.ones(dirtyFDF.shape[1:], dtype="bool") 
-        
+        mskArr = np.ones(dirtyFDF.shape[1:], dtype="bool")
+
     # Reshape the FDF & RMSF array to 3 dimensions and mask array to 2
     if nDims==1:
         dirtyFDF = np.reshape(dirtyFDF, (dirtyFDF.shape[0], 1, 1))
         RMSFArr = np.reshape(RMSFArr, (RMSFArr.shape[0], 1, 1))
         mskArr = np.reshape(mskArr,  (1, 1))
         fwhmRMSFArr = np.reshape(fwhmRMSFArr,  (1, 1))
     elif nDims==2:
@@ -483,35 +470,31 @@
     residFDF = dirtyFDF.copy()
     ccArr = np.zeros(dirtyFDF.shape, dtype=dtComplex)
     cleanFDF = np.zeros_like(dirtyFDF)
 
 
     # Loop through the pixels containing a polarised signal
     inputs = [[yi, xi, dirtyFDF] for yi, xi in xyCoords]
-    rmc = RMcleaner(RMSFArr, phi2Arr_radm2, phiArr_radm2, fwhmRMSFArr, 
+    rmc = RMcleaner(RMSFArr, phi2Arr_radm2, phiArr_radm2, fwhmRMSFArr,
                     iterCountArr, maxIter, gain, cutoff, nBits, verbose, window)
 
 
     if pool is None:
-        if verbose:
-            progress(40,0)
-            i=0
         output=[]
-        for pix in inputs:    
+        for pix in inputs:
             output.append(rmc.cleanloop(pix))
-            if verbose:
-                progress(40, ((i)*100.0/nCleanPix))
-                i+=1
     else:
-        if verbose:
-            log('(Progress bar is not supported for parallel mode. Please wait for the code to finish.')
-        if chunksize is not None:
-            output = list(pool.map(rmc.cleanloop, inputs, chunksize=chunksize))
-        else:
-                output = list(pool.map(rmc.cleanloop, inputs))
+        output = list(
+            tqdm(
+                pool.imap(rmc.cleanloop, inputs, chunksize=chunksize if chunksize is not None else 1),
+                desc="RM-CLEANing",
+                disable=not verbose,
+                total=len(inputs),
+            )
+        )
         pool.close()
     # Put data back in correct shape
 #    ccArr = np.reshape(np.rot90(np.stack([model for _, _, model in output]), k=-1),dirtyFDF.shape)
 #    cleanFDF = np.reshape(np.rot90(np.stack([clean for clean, _, _ in output]), k=-1),dirtyFDF.shape)
 #    residFDF = np.reshape(np.rot90(np.stack([resid for _, resid, _ in output]), k=-1),dirtyFDF.shape)
     for i in range(len(inputs)):
         yi=inputs[i][0]
@@ -536,16 +519,16 @@
 
 
 class RMcleaner:
     """Allows do_rmclean_hogbom to be run in parallel
     Designed around use of schwimmbad parallelization tools.
     """
 
-    def __init__(self, RMSFArr, phi2Arr_radm2, phiArr_radm2, fwhmRMSFArr, 
-                 iterCountArr, maxIter=1000, gain=0.1, cutoff=0,nbits=32, 
+    def __init__(self, RMSFArr, phi2Arr_radm2, phiArr_radm2, fwhmRMSFArr,
+                 iterCountArr, maxIter=1000, gain=0.1, cutoff=0,nbits=32,
                  verbose=False, window=0):
         self.RMSFArr = RMSFArr
         self.phi2Arr_radm2 = phi2Arr_radm2
         self.phiArr_radm2 = phiArr_radm2
         self.fwhmRMSFArr = fwhmRMSFArr
         self.iterCountArr = iterCountArr
         self.maxIter = maxIter
@@ -571,15 +554,15 @@
         indxMaxRMSF = np.nanargmax(RMSFArr)
 
         # Calculate the padding in the sampled RMSF
         # Assumes only integer shifts and symmetric
         nPhiPad = int((len(self.phi2Arr_radm2)-len(self.phiArr_radm2))/2)
 
         iterCount = 0
-        while (np.max(np.abs(residFDF)) >= self.cutoff and iterCount <= self.maxIter):
+        while (np.max(np.abs(residFDF)) >= self.cutoff and iterCount < self.maxIter):
             # Get the absolute peak channel, values and Faraday depth
             indxPeakFDF = np.argmax(np.abs(residFDF))
             peakFDFval = residFDF[indxPeakFDF]
             phiPeak = self.phiArr_radm2[indxPeakFDF]
 
             # A clean component is "loop-gain * peakFDFval
             CC = self.gain * peakFDFval
@@ -607,15 +590,15 @@
         fwhmRMSFArr_pix = fwhmRMSFArr / dPhi
         for i in np.where(mask)[0]:
             start = int(i - fwhmRMSFArr_pix /2)
             end = int(i + fwhmRMSFArr_pix /2)
             mask[start:end] = True
         residFDF_mask = np.ma.array(residFDF, mask=~mask)
         # Clean again within mask
-        while (np.ma.max(np.ma.abs(residFDF_mask)) >= self.window and iterCount <= self.maxIter):
+        while (np.ma.max(np.ma.abs(residFDF_mask)) >= self.window and iterCount < self.maxIter):
             if residFDF_mask.mask.all():
                 break
             # Get the absolute peak channel, values and Faraday depth
             indxPeakFDF = np.ma.argmax(np.abs(residFDF_mask))
             peakFDFval = residFDF_mask[indxPeakFDF]
             phiPeak = self.phiArr_radm2[indxPeakFDF]
 
@@ -650,33 +633,33 @@
 
 
 
 #-----------------------------------------------------------------------------#
 def fits_make_lin_axis(head, axis=0, dtype="f4"):
     """Create an array containing the axis values, assuming a simple linear
     projection scheme. Axis selection is zero-indexed."""
-    
-    axis = int(axis)    
+
+    axis = int(axis)
     if head['NAXIS'] < axis + 1:
         return []
-    
+
     i = str(int(axis) + 1)
     start = head['CRVAL' + i] + (1 - head['CRPIX' + i]) * head['CDELT' + i]
-    stop = (head['CRVAL' + i] + (head['NAXIS' + i] - head['CRPIX' + i]) * 
+    stop = (head['CRVAL' + i] + (head['NAXIS' + i] - head['CRPIX' + i]) *
             head['CDELT' + i])
     nChan = int(abs(start - stop)/head['CDELT' + i] +1)
-    
+
     return np.linspace(start, stop, nChan).astype(dtype)
- 
+
 
 #-----------------------------------------------------------------------------#
 def extrap(x, xp, yp):
     """
     Wrapper to allow np.interp to linearly extrapolate at function ends.
-    
+
     np.interp function with linear extrapolation
     http://stackoverflow.com/questions/2745329/how-to-make-scipy-interpolate
     -give-a-an-extrapolated-result-beyond-the-input-ran
 
     """
     y = np.interp(x, xp, yp)
     y = np.where(x < xp[0], yp[0]+(x-xp[0])*(yp[0]-yp[1])/(xp[0]-xp[1]), y)
@@ -684,67 +667,67 @@
                  y)
     return y
 
 
 #-----------------------------------------------------------------------------#
 def fit_rmsf(xData, yData, thresh=0.4, ampThresh=0.4):
     """
-    Fit the main lobe of the RMSF with a Gaussian function. 
+    Fit the main lobe of the RMSF with a Gaussian function.
     """
 
     try:
-        
+
         # Detect the peak and mask off the sidelobes
         msk1 = detect_peak(yData, thresh)
         msk2 = np.where(yData<ampThresh, 0.0, msk1)
         if sum(msk2)<4:
             msk2 = msk1
         validIndx = np.where(msk2==1.0)
         xData = xData[validIndx]
         yData = yData[validIndx]
-        
+
         # Estimate starting parameters
         a = 1.0
         b = xData[np.argmax(yData)]
         w = np.nanmax(xData)-np.nanmin(xData)
         inParms=[ {'value': a, 'fixed':False, 'parname': 'amp'},
                   {'value': b, 'fixed':False, 'parname': 'offset'},
                   {'value': w, 'fixed':False, 'parname': 'width'}]
 
         # Function which returns another function to evaluate a Gaussian
         def gauss(p):
             a, b, w = p
             gfactor = 2.0 * m.sqrt(2.0 * m.log(2.0))
-            s = w / gfactor    
+            s = w / gfactor
             def rfunc(x):
                 y = a * np.exp(-(x-b)**2.0 /(2.0 * s**2.0))
                 return y
             return rfunc
-    
+
         # Function to evaluate the difference between the model and data.
         # This is minimised in the least-squared sense by the fitter
         def errFn(p, fjac=None):
             status = 0
             return status, gauss(p)(xData) - yData
-    
+
         # Use mpfit to perform the fitting
         mp = mpfit(errFn, parinfo=inParms, quiet=True)
 
         return mp
-    
+
     except Exception:
         return None
 
 
 #-----------------------------------------------------------------------------#
 def gauss1D(amp=1.0, mean=0.0, fwhm=1.0):
     """Function which returns another function to evaluate a Gaussian"""
 
     gfactor = 2.0 * m.sqrt(2.0 * m.log(2.0))
-    sigma = fwhm / gfactor    
+    sigma = fwhm / gfactor
     def rfunc(x):
         return amp * np.exp(-(x-mean)**2.0 /(2.0 * sigma**2.0))
     return rfunc
 
 
 #-----------------------------------------------------------------------------#
 
@@ -761,15 +744,15 @@
     # find first point below threshold right of peak
     ishift = np.where(a[iPk:]<thresh)[0][0]
     iR = iPk+ishift
     iL = iPk-ishift+1
 
     msk = np.zeros_like(a)
     msk[iL:iR] = 1
-    
+
     # DEBUG PLOTTING
     if False:
         from matplotlib import pyplot as plt
         fig = plt.figure()
         ax = fig.add_subplot(111)
         ax.step(np.arange(len(a)),a, where="mid", label="arr")
         ax.step(np.arange(len(msk)), msk*0.5, where="mid", label="msk")
@@ -802,21 +785,21 @@
 
 #     # Determine the right-most index of flat peaks
 #     iPkR = iPkL
 #     d = np.diff(a)
 #     flatIndxLst = np.argwhere(d[iPkL:]==0).flatten()
 #     if len(flatIndxLst)>0:
 #         iPkR += (np.max(flatIndxLst)+1)
-        
+
 #     # Search for the left & right crossing point
 #     iL = np.max(np.argwhere(g1[:iPkL]<=threshPos).flatten())
 #     iR = iPkR + np.min(np.argwhere(g1[iPkR+1:]<=threshPos).flatten()) + 2
 #     msk = np.zeros_like(a)
 #     msk[iL:iR] = 1
-    
+
 #     # DEBUG PLOTTING
 #     if False:
 #         from matplotlib import pyplot as plt
 #         fig = plt.figure()
 #         ax = fig.add_subplot(111)
 #         ax.step(np.arange(len(a)),a, where="mid", label="arr")
 #         ax.step(np.arange(len(g1)), np.abs(g1), where="mid", label="g1")
@@ -839,15 +822,15 @@
                       lam0Sq=None, snrDoBiasCorrect=5.0):
     """
     Measure standard parameters from a complex Faraday Dispersion Function.
     Currently this function assumes that the noise levels in the Stokes Q
     and U spectra are the same.
     Returns a dictionary containing measured parameters.
     """
-    
+
     # Determine the peak channel in the FDF, its amplitude and index
     absFDF = np.abs(FDF)
     indxPeakPIchan = np.nanargmax(absFDF[1:-1])+1  #Masks out the edge channels, since they can't be fit to.
     ampPeakPIchan = absFDF[indxPeakPIchan]
 
     # Measure the RMS noise in the spectrum after masking the peak
     dPhi = np.nanmin(np.diff(phiArr))
@@ -863,20 +846,20 @@
     else:
         dFDFcorMAD = MAD(absFDFmsked)
         dFDFrms = np.sqrt( np.mean(absFDFmsked**2) )
 
     # Default to using the measured FDF if a noise value has not been provided
     if dFDF is None:
         dFDF = dFDFcorMAD
-    
+
     # Measure the RM of the peak channel
     phiPeakPIchan = phiArr[indxPeakPIchan]
     dPhiPeakPIchan = fwhmRMSF * dFDF / (2.0 * ampPeakPIchan)
     snrPIchan = ampPeakPIchan / dFDF
-    
+
     # Correct the peak for polarisation bias (POSSUM report 11)
     ampPeakPIchanEff = ampPeakPIchan
     if snrPIchan >= snrDoBiasCorrect:
         ampPeakPIchanEff = np.sqrt(ampPeakPIchan**2.0 - 2.3 * dFDF**2.0)
 
     # Calculate the polarisation angle from the channel
     peakFDFimagChan = FDF.imag[indxPeakPIchan]
@@ -891,59 +874,59 @@
     nChansGood = np.sum(np.where(lamSqArr_m2==lamSqArr_m2, 1.0, 0.0))
     varLamSqArr_m2 = (np.sum(lamSqArr_m2**2.0) -
                       np.sum(lamSqArr_m2)**2.0/nChansGood) / (nChansGood-1)
     dPolAngle0Chan_rad = \
         np.sqrt( dFDF**2.0*nChansGood / (4.0*(nChansGood-2.0)*ampPeakPIchan**2.0) *
                  ((nChansGood-1)/nChansGood + lam0Sq**2.0/varLamSqArr_m2) )
     dPolAngle0Chan_deg = np.degrees(dPolAngle0Chan_rad)
-    
+
     # Determine the peak in the FDF, its amplitude and Phi using a
     # 3-point parabolic interpolation
     phiPeakPIfit = None
     dPhiPeakPIfit = None
     ampPeakPIfit = None
     snrPIfit = None
     ampPeakPIfitEff = None
     indxPeakPIfit = None
-    peakFDFimagFit = None 
-    peakFDFrealFit = None 
+    peakFDFimagFit = None
+    peakFDFrealFit = None
     polAngleFit_deg = None
     dPolAngleFit_deg = None
     polAngle0Fit_deg = None
     dPolAngle0Fit_deg = None
 
     # Only do the 3-point fit if peak is 1-channel from either edge
     if indxPeakPIchan > 0 and indxPeakPIchan < len(FDF)-1:
         phiPeakPIfit, ampPeakPIfit = \
                       calc_parabola_vertex(phiArr[indxPeakPIchan-1],
                                            absFDF[indxPeakPIchan-1],
                                            phiArr[indxPeakPIchan],
                                            absFDF[indxPeakPIchan],
                                            phiArr[indxPeakPIchan+1],
                                            absFDF[indxPeakPIchan+1])
-        
+
         snrPIfit = ampPeakPIfit / dFDF
-        
+
         #In rare cases, a parabola can be fitted to the edge of the spectrum,
         #producing a unreasonably large RM and polarized intensity.
         #In these cases, everything should get NaN'd out.
         if np.abs(phiPeakPIfit) > np.max(np.abs(phiArr)):
             phiPeakPIfit=np.nan
             ampPeakPIfit=np.nan
-        
-        
+
+
         # Error on fitted Faraday depth (RM) is same as channel, but using fitted PI
         dPhiPeakPIfit = fwhmRMSF * dFDF / (2.0 * ampPeakPIfit)
-        
-        
+
+
         # Correct the peak for polarisation bias (POSSUM report 11)
         ampPeakPIfitEff = ampPeakPIfit
         if snrPIfit >= snrDoBiasCorrect:
             ampPeakPIfitEff = np.sqrt(ampPeakPIfit**2.0 - 2.3 * dFDF**2.0)
-            
+
         # Calculate the polarisation angle from the fitted peak
         # Uncertainty from Eqn A.12 in Brentjens & De Bruyn 2005
         indxPeakPIfit = np.interp(phiPeakPIfit, phiArr,
                                   np.arange(phiArr.shape[-1], dtype='f4'))
         peakFDFimagFit = np.interp(phiPeakPIfit, phiArr, FDF.imag)
         peakFDFrealFit = np.interp(phiPeakPIfit, phiArr, FDF.real)
         polAngleFit_deg = 0.5 * np.degrees(np.arctan2(peakFDFimagFit,
@@ -992,21 +975,21 @@
     return mDict
 
 
 #-----------------------------------------------------------------------------#
 def norm_cdf(mean=0.0, std=1.0, N=50, xArr=None):
     """Return the CDF of a normal distribution between -6 and 6 sigma, or at
     the values of an input array."""
-    
+
     if xArr is None:
         x = np.linspace(-6.0*std, 6.0*std, N)
     else:
         x = xArr
     y = norm.cdf(x, loc=mean, scale=std)
-    
+
     return x, y
 
 
 #-----------------------------------------------------------------------------#
 def cdf_percentile(x, p, q=50.0):
     """Return the value at a given percentile of a cumulative distribution
     function."""
@@ -1022,35 +1005,35 @@
         return x[i]
 
     # or interpolate between the two bracketing values in the CDF
     else:
         m = (p[i]-p[i-1])/(x[i]-x[i-1])
         c = p[i] - m*x[i]
         return (q/100.0-c)/m
-    
+
 
 #-----------------------------------------------------------------------------#
 def calc_sigma_add(xArr, yArr, dyArr, yMed=None, noise=None, nSamp=1000,
                    suffix=""):
     """Calculate the most likely value of additional scatter, assuming the
     input data is drawn from a normal distribution. The total uncertainty on
     each data point Y_i is modelled as dYtot_i**2 = dY_i**2 + dYadd**2."""
-    
+
     # Measure the median and MADFM of the input data if not provided.
     # Used to overplot a normal distribution when debugging.
     if yMed is None:
         yMed = np.median(yArr)
     if noise is None:
         noise = MAD(yArr)
 
     # Sample the PDF of the additional noise term from a limit near zero to
     # a limit of the range of the data, including error bars
     yRng = np.nanmax(yArr+dyArr) - np.nanmin(yArr-dyArr)
     sigmaAddArr = np.linspace(yRng/nSamp, yRng, nSamp)
-    
+
     # Model deviation from Gaussian as an additional noise term.
     # Loop through the range of i additional noise samples and calculate
     # chi-squared and sum(ln(sigma_total)), used later to calculate likelihood.
     nData = len(xArr)
     chiSqArr = np.zeros_like(sigmaAddArr)
     lnSigmaSumArr = np.zeros_like(sigmaAddArr)
     for i, sigmaAdd in enumerate(sigmaAddArr):
@@ -1061,19 +1044,19 @@
     chiSqRedArr = chiSqArr/dof
 
     # Calculate the PDF in log space and normalise the peak to 1
     lnProbArr = (-np.log(sigmaAddArr) -nData * np.log(2.0*np.pi)/2.0
                  -lnSigmaSumArr -chiSqArr/2.0)
     lnProbArr -= np.nanmax(lnProbArr)
     probArr = np.exp(lnProbArr)
-    
+
     # Normalise the area under the PDF to be 1
     A = np.nansum(probArr * np.diff(sigmaAddArr)[0])
     probArr /= A
-    
+
     # Calculate the cumulative PDF
     CPDF = np.cumsum(probArr)/np.nansum(probArr)
 
     # Calculate the mean of the distribution and the +/- 1-sigma limits
     sigmaAdd = cdf_percentile(x=sigmaAddArr, p=CPDF, q=50.0)
     sigmaAddMinus = cdf_percentile(x=sigmaAddArr, p=CPDF, q=15.72)
     sigmaAddPlus = cdf_percentile(x=sigmaAddArr, p=CPDF, q=84.27)
@@ -1084,22 +1067,22 @@
     # Return the curves to be plotted in a separate dictionary
     pltDict = {"sigmaAddArr" + suffix: sigmaAddArr,
                "chiSqRedArr" + suffix: chiSqRedArr,
                "probArr" + suffix: probArr,
                "xArr" + suffix: xArr,
                "yArr" + suffix: yArr,
                "dyArr" + suffix: dyArr}
-    
+
     # DEBUG PLOTS
     if False:
 
         # Setup for the figure
         import matplotlib.pyplot as plt
         fig = plt.figure(figsize=(18.0, 10.0))
-        
+
         # Plot the data and the +/- 1-sigma levels
         ax1 = fig.add_subplot(231)
         ax1.errorbar(x=xArr, y=yArr, yerr=dyArr, ms=4, fmt='o')
         ax1.axhline(yMed, color='grey', zorder=10)
         ax1.axhline(yMed+noise, color='r', linestyle="--", zorder=10)
         ax1.axhline(yMed-noise, color='r', linestyle="--", zorder=10)
         ax1.set_title(r'Input Data')
@@ -1117,15 +1100,15 @@
         ax2.plot(xNorm, yNorm, color='k', linestyle="--", linewidth=2)
         ax2.axvline(yMed, color='grey', zorder=11)
         ax2.axvline(yMed+fwhm/2.0, color='r', linestyle="--", zorder=11)
         ax2.axvline(yMed-fwhm/2.0, color='r', linestyle="--", zorder=11)
         ax2.set_title(r'Distribution of Data Compared to Normal')
         ax2.set_xlabel(r'Amplitude')
         ax2.set_ylabel(r'Normalised Counts')
-    
+
         # Plot the ECDF versus a normal CDF
         ecdfArr = np.array(list(range(nData)))/float(nData)
         ySrtArr = np.sort(yArr)
         ax3 = fig.add_subplot(233)
         ax3.step(ySrtArr, ecdfArr, where="mid")
         x, y = norm_cdf(mean=yMed, std=noise, N=1000)
         ax3.plot(x, y, color='k', linewidth=2, linestyle="--", zorder=1)
@@ -1162,47 +1145,47 @@
         ax6.set_title('Cumulative Likelihood')
         ax6.set_xlabel(r"$\sigma_{\rm additional}$")
         ax6.set_ylabel(r"Cumulative Likelihood")
 
         # Zoom in
         ax5.set_xlim(0, sigmaAdd + (sigmaAddPlus-sigmaAdd)*4.0)
         ax6.set_xlim(0, sigmaAdd + (sigmaAddPlus-sigmaAdd)*4.0)
-        
+
         # Show the figure
         fig.subplots_adjust(left=0.07, bottom=0.07, right=0.97, top=0.94,
                             wspace=0.25, hspace=0.25)
         fig.show()
-        
+
         # Feedback to user
         print("sigma_add(q) = %.4g (+%3g, -%3g)" %
               (mDict["sigmaAddQ"], mDict["dSigmaAddPlusQ"],
                mDict["dSigmaAddMinusQ"]))
         print("sigma_add(u) = %.4g (+%3g, -%3g)" %
               (mDict["sigmaAddU"], mDict["dSigmaAddPlusU"],
                mDict["dSigmaAddMinusU"]))
         input()
-            
+
     return mDict, pltDict
 
 
 #-----------------------------------------------------------------------------#
 def calc_normal_tests(inArr, suffix=""):
     """Calculate metrics measuring deviation of an array from Normal."""
 
     # Perfrorm the KS-test
     KS_z, KS_p = kstest(inArr, "norm")
-        
+
     # Calculate the Anderson test
     AD_z, AD_crit, AD_sig = anderson(inArr, "norm")
-    
+
     # Calculate the skewness (measure of symmetry)
     # abs(skewness) < 0.5 =  approx symmetric
     skewVal = skew(inArr)
     SK_z, SK_p = skewtest(inArr)
-    
+
     # Calculate the kurtosis (tails compared to a normal distribution)
     kurtosisVal = kurtosis(inArr)
     KUR_z, KUR_p = kurtosistest(inArr)
 
     # Return dictionary
     mDict = {"KSz" + suffix:  toscalar(KS_z),
              "KSp" + suffix:  toscalar(KS_p),
@@ -1219,53 +1202,53 @@
 
     return mDict
 
 
 #-----------------------------------------------------------------------------#
 def measure_qu_complexity(freqArr_Hz, qArr, uArr, dqArr, duArr, fracPol,
                           psi0_deg, RM_radm2, specF=1):
-    
+
     # Create a RM-thin model to subtract
     pModArr, qModArr, uModArr = \
              create_pqu_spectra_burn(freqArr_Hz   = freqArr_Hz,
                                      fracPolArr   = [fracPol],
                                      psi0Arr_deg  = [psi0_deg],
                                      RMArr_radm2  = [RM_radm2])
     lamSqArr_m2 = np.power(C/freqArr_Hz, 2.0)
     ndata = len(lamSqArr_m2)
-    
+
     # Subtract the RM-thin model to create a residual q & u
     qResidArr = qArr - qModArr
     uResidArr = uArr - uModArr
 
     # Calculate value of additional scatter term for q & u (max likelihood)
     mDict = {}
     pDict = {}
     m1D, p1D = calc_sigma_add(xArr=lamSqArr_m2[:int(ndata/specF)],
                               yArr=(qResidArr/dqArr)[:int(ndata/specF)],
                               dyArr=(dqArr/dqArr)[:int(ndata/specF)],
                               yMed=0.0,
                               noise=1.0,
                               suffix="Q")
     mDict.update(m1D)
-    pDict.update(p1D)    
+    pDict.update(p1D)
     m2D, p2D = calc_sigma_add(xArr=lamSqArr_m2[:int(ndata/specF)],
                               yArr=(uResidArr/duArr)[:int(ndata/specF)],
                               dyArr=(duArr/duArr)[:int(ndata/specF)],
                               yMed=0.0,
                               noise=1.0,
                               suffix="U")
     mDict.update(m2D)
     pDict.update(p2D)
-    
+
     # Calculate the deviations statistics
     # Done as a test for the paper, not usually offered to user.
     #mDict.update( calc_normal_tests(qResidArr/dqArr, suffix="Q") )
     #mDict.update( calc_normal_tests(uResidArr/duArr, suffix="U") )
-    
+
     return mDict, pDict
 
 
 #-----------------------------------------------------------------------------#
 def measure_fdf_complexity(phiArr, FDF):
 
     # Second moment of clean component spectrum
@@ -1281,23 +1264,23 @@
 
 #-----------------------------------------------------------------------------#
 def do_rmsynth(dataQ, dataU, lamSqArr, phiArr, weight=None, dtype='float32'):
     """Perform RM-synthesis on Stokes Q and U cubes. This version operates on
     data in spectral order, i.e., [zyx] => [yxz] (np.transpose(dataQ, (1,2,0)).
 
     *** Depricated by the faster 'do_rmsynth_planes' routine, above. ***
-    
+
     """
-    
+
     # Parse the weight argument
     if weight is None:
         weightArr = np.ones(lamSqArr.shape, dtype=dtype)
     else:
         weightArr = np.array(weight, dtype=dtype)
-    
+
     # Sanity check on array sizes
     if not weightArr.shape  == lamSqArr.shape:
         print("Err: Lambda^2 and weight arrays must be the same shape.")
         return None, [None, None], None, None
     if not dataQ.shape == dataU.shape:
         print("Err: Stokes Q and U data arrays must be the same shape.")
         return None, [None, None], None, None
@@ -1321,102 +1304,96 @@
 
     # Create a blanking mask assuming NaNs are blanked in the input data
     # Set the weight = 0 in fully blanked planes
     dataMsk = np.where(np.isnan(dataQ) + np.isnan(dataU), 0, 1)
     dataMsk = np.where(np.sum(np.sum(dataMsk, 0), 0)==0, 1, 0)
     weightArr = np.where(dataMsk==1, 0.0, weightArr)
     del dataMsk
-    
+
     # Create a complex polarised cube, B&dB Eqns. (8) and (14)
     # Cube has dimensions (nY, nX, nFreq)
     pCube = (dataQ + 1j * dataU) * weightArr
-    
+
     # Initialise the complex Faraday Dispersion Function (FDF) cube
     # Remember, python index order is reversed [2,1,0] = [y,x,phi]
     nY = dataQ.shape[0]
     nX = dataQ.shape[1]
     nPhi = phiArr.shape[0]
     FDFcube = np.ndarray((nY, nX, nPhi), dtype='complex')
-    
+
     # B&dB equations (24) and (38) give the inverse sum of the weights
     # Get the weighted mean of the LambdaSq distribution (B&dB Eqn. 32)
     K = 1.0 / np.nansum(weightArr)
     lam0Sq_m2 = K * np.nansum(weightArr * lamSqArr)
-    
+
     # Mininize the number of inner-loop operations by calculating the
     # argument of the EXP term in B&dB Eqns. (25) and (36) for the FDF
     # Returned array has dimensions (nPhi x nFreq)
     a = (-2.0 * 1j * phiArr)
-    b = (lamSqArr - lam0Sq_m2) 
+    b = (lamSqArr - lam0Sq_m2)
     arg = np.exp( np.outer(a, b) )
 
     # Do the synthesis at each pixel of the image
-    nPix = nX * nY
-    j = 0
-    progress(40, 0)
-    for k in range(nY):
+    for k in trange(nY, desc='RM-synthesis'):
         for i in range(nX):
-            j += 1
-            progress(40, ((j)*100.0/nPix))
-                
             # Calculate the FDF, B&dB Eqns. (25) and (36)
             # B&dB Eqns. (25) and (36)
             FDFcube[k,i,:] = K * np.nansum(pCube[k,i,:] * arg, axis=1)
-            
+
     # Calculate the complex Rotation Measure Spread Function
     RMSFArr, phiSamp, fwhmRMSF = get_RMSF(lamSqArr, phiArr, weightArr,
                                           lam0Sq_m2)
 
     # Reshape the data and FDF cube back to their original shapes
     if nDims==1:
         dataQ = np.reshape(dataQ, (dataQ.shape[-1]))
         dataU = np.reshape(dataU, (dataU.shape[-1]))
         FDFcube = np.reshape(FDFcube, (FDFcube.shape[-1]))
     elif nDims==2:
         dataQ = np.reshape(dataQ, (dataQ.shape[-2], dataQ.shape[-1]))
         dataU = np.reshape(dataU, (dataU.shape[-2], dataU.shape[-1]))
         FDFcube = np.reshape(FDFcube, (FDFcube.shape[-2], FDFcube.shape[-1]))
-    
+
     return FDFcube, [phiSamp, RMSFArr], lam0Sq_m2, fwhmRMSF
 
 
 #-----------------------------------------------------------------------------#
 def get_RMSF(lamSqArr, phiArr, weightArr=None, lam0Sq_m2=None, double=True,
              fitRMSFreal=False, dtype="float32"):
     """Calculate the RMSF from 1D wavelength^2 and Faraday depth arrays.
-    
+
     *** Depricated by the faster 'get_rmsf_planes' routine, above. ***
 
     """
 
     # Set the weight array
     if weightArr is None:
         uniformWt = True
         weightArr = np.ones(lamSqArr.shape, dtype=dtype)
     else:
         uniformWt = False
         weightArr = np.array(weightArr, dtype=dtype)
-            
+
     # lam0Sq is the weighted mean of the LambdaSq distribution (B&dB Eqn. 32)
     K = 1.0 / np.nansum(weightArr)
     if lam0Sq_m2 is None:
         lam0Sq_m2 = K * np.nansum(weightArr * lamSqArr)
 
     # For cleaning the RMSF should extend by 1/2 on each side in phi-space
     if double:
         nPhi = phiArr.shape[0]
         nExt = np.ceil(nPhi/2.0)
         resampIndxArr = np.arange(2.0 * nExt + nPhi) - nExt
         phi2Arr = extrap(resampIndxArr, np.arange(nPhi, dtype='int'), phiArr)
     else:
         phi2Arr = phiArr
-        
+
     # Calculate the RM spread function
     a = (-2.0 * 1j * phi2Arr)
-    b = (lamSqArr - lam0Sq_m2) 
+    b = (lamSqArr - lam0Sq_m2)
     RMSFArr = K * np.nansum(weightArr * np.exp( np.outer(a, b) ), 1)
 
     # Calculate (B&dB Equation 61) or fit the main-lobe FWHM of the RMSF
     fwhmRMSF = 3.8/(np.nanmax(lamSqArr) - np.nanmin(lamSqArr))
     if not uniformWt:
         if fitRMSFreal:
             mp = fit_rmsf(phi2Arr, RMSFArr.real)
@@ -1424,39 +1401,39 @@
             mp = fit_rmsf(phi2Arr, np.abs(RMSFArr))
         if mp is None or mp.status<1:
             pass
             print("Err: failed to fit the RMSF.")
             print("Defaulting to analytical value in uniform case.")
         else:
             fwhmRMSF = mp.params[2]
-            
+
     return RMSFArr, phi2Arr, fwhmRMSF
 
 
 #-----------------------------------------------------------------------------#
 def do_rmclean(dirtyFDF, phiArr, lamSqArr, cutoff, maxIter=1000, gain=0.1,
                weight=None, RMSFArr=None, RMSFphiArr=None, fwhmRMSF=None,
                fitRMSFreal=False, dtype='float32', doPlots=True):
     """Perform Hogbom (Heald) clean on a single RM spectrum.
 
         *** Depricated by the 'do_rmsynth_hogbom' routine, above. ***"""
-    
+
     # Initial sanity checks --------------------------------------------------#
-   
+
     # Check that dirtyFDF is ID and get its length
     if len(dirtyFDF.shape) != 1:
         print("Err: the dirty FDF is not a 1D array.")
         sys.exit(1)
     nFDF = dirtyFDF.shape[0]
 
     # Check that dirtyFDF is a complex array
     if not np.iscomplexobj(dirtyFDF):
         print("Err: the dirty FDF is not a complex array.")
         sys.exit(1)
-        
+
     # Check that phiArr is 1D and get its length
     if len(phiArr.shape) != 1:
         print("Err: the phi array is not a 1D array.")
         sys.exit(1)
     nPhi = phiArr.shape[0]
 
     # Check that the lamSqArr is 1D and get its length
@@ -1465,112 +1442,112 @@
         sys.exit(1)
     nlamSq = lamSqArr.shape[0]
 
     # Check that phiArr and FDF arrays are the same length
     if nPhi != nFDF:
         print('Err: the phiArr and dirty FDF are not the same length.')
         sys.exit(1)
-    
+
     # If the RMSF has been passed in then check for correct formatting:
     #  - Twice the number of channels as dirtyFDF
     #  - Must be complex
     if not RMSFArr is None:
 
         # Check 1D
         if len(RMSFArr.shape) != 1:
             print("Err: input RMSF must be a 1D array.")
             sys.exit(1)
         nRMSF = RMSFArr.shape[0]
-        
+
         # Check complex
         if not np.iscomplexobj(RMSFArr):
             print("Err: the RMSF is not a complex array.")
             sys.exit(1)
-    
+
         # Check RMSF is at least double the FDF spectrum
         if not (nRMSF >= 2 * nFDF):
             print('Err: the RMSF must be twice the length of the FDF.')
             sys.exit(1)
 
         # Check that phiSampArr is also present and the same length
         if RMSFphiArr is None:
             print('Err: the phi sampling array must be passed with the RMSF.')
             sys.exit(1)
         nRMSFphi = RMSFphiArr.shape[0]
         if not nRMSF==nRMSFphi:
             print('Err: the RMSF and phi sampling array must be equal length.')
             sys.exit(1)
-            
+
         # Calculate or fit the main-lobe FWHM of the RMSF
         # B&dB Equation (61)
         fwhmRMSF = 2.0 * m.sqrt(3.0)/(np.nanmax(lamSqArr) -
                                   np.nanmin(lamSqArr))
         if fitRMSFreal:
             mp = fit_rmsf(RMSFphiArr, RMSFArr.real)
         else:
             mp = fit_rmsf(RMSFphiArr, np.abs(RMSFArr))
         if mp is None or mp.status<1:
             pass
             print('Err: failed to fit the RMSF.')
             print("Defaulting to analytical value in uniform case.")
         else:
             fwhmRMSF = mp.params[2]
-    
+
     # If the weight array has been passed in ...
     if not weight is None:
-        
+
         uniformWt = False
         weightArr = np.array(weight, dtype=dtype)
-    
+
         # Check weightArr and lamSqArr have the same length
         if not weightArr.shape[0] == lamSqArr.shape[0]:
             print('Err: the lamSqArr and weightArr are not the same length.')
             sys.exit(1)
-            
+
     # or else use uniform weighting
     else:
         uniformWt = True
         weightArr = np.ones(lamSqArr.shape, dtype=dtype)
 
     if doPlots:
-        
+
         from matplotlib import pyplot as plt
-        
+
         # Setup the figure to track the clean
         fig = plt.figure(figsize=(12.0, 8))
         ax = fig.add_subplot(111)
         yMaxPlot = np.nanmax(np.abs(dirtyFDF))
         yMinPlot = np.nanmin(np.abs(dirtyFDF))
         yRangePlot = yMaxPlot - yMinPlot
         yMaxPlot +=  yRangePlot * 0.05
         yMinPlot -=  yRangePlot * 0.05
         ax.set_ylim([yMinPlot, yMaxPlot])
         fig.show()
-        
+
     # Prerequisite calculations ----------------------------------------------#
-    
+
     # Calculate the normalisation constant.
     # BdB Equations (24) and (38) give the inverse sum of the weights.
     K = 1.0 / np.nansum(weightArr)
-    
+
     # Calculate the default lambda_0^2:
     # the weighted mean of the LambdaSq distribution (B&dB Eqn. 32).
     lam0Sq_m2 = K * np.nansum(weightArr * lamSqArr)
 
-    # Calculate the RMSF if it has not been passed in 
+    # Calculate the RMSF if it has not been passed in
     # Equation (26) OF BdB05
     if RMSFArr is None:
         RMSFArr, phi2Arr, fwhmRMSF= get_RMSF(lamSqArr, phiArr, weightArr,
                                              lam0Sq_m2)
     else:
         phi2Arr = RMSFphiArr
-    
+
     # Find the index of the peak of the RMSF
     indxMaxRMSF = np.nanargmax(RMSFArr)
-    
+
     # Initialise arrays to hold the residual FDF, clean components, clean FDF
     residFDF = dirtyFDF.copy()
     ccArr = np.zeros(phiArr.shape, dtype='complex')
     cleanFDF = np.zeros(phiArr.shape, dtype='complex')
 
     # HOGBOM CLEAN -----------------------------------------------------------#
 
@@ -1585,130 +1562,130 @@
         print(np.max(np.abs(residFDF)), cutoff)
         # Get the absolute peak channel and values of the residual FDF at peak
         indxPeakFDF = np.nanargmax(np.abs(residFDF))
         peakFDFvals = residFDF[indxPeakFDF]
 
         # What is the faraday depth at this channel?
         phiPeak = phiArr[indxPeakFDF]
-        
+
         # A clean component (CC) is the max absolute amplitude * loop-gain
         #cc = gain * maxAbsResidFDF
         cc = gain * peakFDFvals
         ccArr[indxPeakFDF] += cc
-        
+
         # At which channel is the CC located at in the RMSF?
         indxPeakRMSF = np.argwhere(phi2Arr==phiPeak)[0][0]
-        
+
         # Shift the RMSF in Faraday Depth so that its peak is centred above
         # this CC
         shiftedRMSFArr = np.roll(RMSFArr, indxPeakRMSF-indxMaxRMSF)
-        
+
         # Clip the shifted RMSF to correspond to our FD range
         shiftedRMSFArr = shiftedRMSFArr[nPhiPad:-nPhiPad]
-        
+
         # Subtract the product of the CC shifted RMSF from the residual FDF
         residFDF -= cc * shiftedRMSFArr
- 
+
         # Restore the CC * a Gaussian 'main peak' RMSF to the cleaned FDF
         cleanFDF += cc * np.exp(-2.77258872224 *
-                                np.power( (phiArr - phiPeak)/fwhmRMSF, 2.0)) 
-        
+                                np.power( (phiArr - phiPeak)/fwhmRMSF, 2.0))
+
         # Plot the progress of the clean
         if doPlots:
             ax.cla()
             ax.step(phiArr, np.abs(ccArr), color='g',marker='None',mfc='w',
                     mec='g', ms=10, label='none')
             ax.step(phiArr, np.abs(residFDF), color='r',marker='None',mfc='w',
                     mec='g', ms=10, label='none')
             ax.step(phiArr, np.abs(shiftedRMSFArr), color='b',marker='None',
                     mfc='w', mec='g', ms=10, label='none')
             ax.step(phiArr, np.abs(cleanFDF), color='k',marker='None',mfc='w',
                     mec='g', ms=10, label='none')
-        
+
             ax.set_ylim(yMinPlot, yMaxPlot)
             plt.draw()
 
         # Iterate ...
         iterCount += 1
         print("Iteration %d", end=' ')
         iterCount
 
     # End clean loop ---------------------------------------------------------#
 
     # Restore the final residuals to the cleaned FDF
     cleanFDF += residFDF
-    
+
     # Plot the final spectrum
     if doPlots:
         ax.cla()
         ax.step(phiArr, np.abs(dirtyFDF), color='grey',marker='None',mfc='w',
                 mec='g', ms=10, label='none')
         ax.step(phiArr, np.abs(cleanFDF), color='k',marker='None',mfc='w',
                 mec='g', ms=10, label='none')
         ax.step(phiArr, np.abs(ccArr), color='g',marker='None',mfc='w',
                 mec='g', ms=10, label='none')
         ax.step(phiArr, cleanFDF.real, color='r',marker='None',mfc='w',
                 mec='g', ms=10, label='none')
         ax.step(phiArr, cleanFDF.imag, color='b',marker='None',mfc='w',
                 mec='g', ms=10, label='none')
-            
+
         ax.set_xlabel('phi')
         ax.set_ylabel('Amplitude')
         ax.set_ylim(yMinPlot, yMaxPlot)
         fig.show()
         input()
 
     return cleanFDF, ccArr, fwhmRMSF, iterCount
 
 
 #-----------------------------------------------------------------------------#
 def plot_complexity(freqArr_Hz, qArr, uArr, dqArr, duArr, fracPol, psi0_deg,
                     RM_radm2):
-    
+
     import matplotlib.pyplot as plt
     from matplotlib.ticker import MaxNLocator
     from .util_plotTk import plot_pqu_vs_lamsq_ax
-    
+
     lamSqArr_m2 = np.power(C/freqArr_Hz, 2.0)
 
     # Create a RM-thin model to subtract
     pModArr, qModArr, uModArr = \
              create_pqu_spectra_burn(freqArr_Hz   = freqArr_Hz,
                                      fracPolArr   = [fracPol],
                                      psi0Arr_deg  = [psi0_deg],
                                      RMArr_radm2  = [RM_radm2])
-        
+
     # Subtract the RM-thin model to create a residual q & u
     qResidArr = qArr - qModArr
     uResidArr = uArr - uModArr
     qResidNorm = qResidArr/dqArr
     uResidNorm = uResidArr/duArr
-    
+
     # High resolution models
-    freqHirArr_Hz =  np.linspace(freqArr_Hz[0], freqArr_Hz[-1], 10000) 
+    freqHirArr_Hz =  np.linspace(freqArr_Hz[0], freqArr_Hz[-1], 10000)
     lamSqHirArr_m2 = np.power(C/freqHirArr_Hz, 2.0)
     pModArr, qModArr, uModArr = \
              create_pqu_spectra_burn(freqArr_Hz   = freqHirArr_Hz,
                                      fracPolArr   = [fracPol],
                                      psi0Arr_deg  = [psi0_deg],
                                      RMArr_radm2  = [RM_radm2])
-    
+
     # Plot the fractional spectra
-    fig = plt.figure(figsize=(12.0, 10.0))        
+    fig = plt.figure(figsize=(12.0, 10.0))
     ax1 = fig.add_subplot(221)
     plot_pqu_vs_lamsq_ax(ax=ax1,
                          lamSqArr_m2 = lamSqArr_m2,
                          qArr        = qArr,
                          uArr        = uArr,
                          dqArr       = dqArr,
-                         duArr       = duArr,                             
+                         duArr       = duArr,
                          qModArr     = qModArr,
                          uModArr     = uModArr,
                          lamSqHirArr_m2 = lamSqHirArr_m2)
-    
+
     # Plot the residual in lambda-sq space
     ax2 = fig.add_subplot(222)
     ax2.errorbar(x=lamSqArr_m2, y=qResidArr, mec='none', mfc='b', ms=4,
                  fmt='o', label='q Residual')
     ax2.errorbar(x=lamSqArr_m2, y=uResidArr, mec='none', mfc='r', ms=4,
                  fmt='o', label='u Residual')
     ax2.axhline(0, color='grey')
@@ -1721,19 +1698,19 @@
     # Plot the distribution of the residual
     ax3 = fig.add_subplot(223)
     nBins = 30
     n, b, p = ax3.hist(qResidNorm, nBins, normed=1, edgecolor="b",
                        histtype='step', linewidth=1.0, zorder=2)
     n, b, p = ax3.hist(uResidNorm, nBins, normed=1, edgecolor="r",
                        histtype='step', linewidth=1.0, zorder=2)
-    
+
     # Overlay a Gaussian
     H = 1.0/m.sqrt(2.0*m.pi)                  # Normalised height
     FWHM = 2.0 * m.sqrt(2.0 * m.log(2.0))     # 1-sigma
-    
+
     x = np.linspace(b[0], b[-1], 1000)
     g = gauss1D(amp=H, mean=0.0, fwhm=FWHM)(x)
     ax3.plot(x, g, color='k', linewidth=2, linestyle="--", zorder=1)
     ax3.set_ylabel('Normalised Units')
     ax3.set_xlabel('Residual ($\sigma$)')
 
     # Plot the cumulative distribution function
@@ -1749,15 +1726,15 @@
     ax4.set_ylabel('CDF')
     ax4.set_xlabel('Residual ($\sigma$)')
 
     return fig
 
 
 
-def threeDnoise_do_rmsynth_planes(dataQ, dataU, lambdaSqArr_m2, phiArr_radm2, 
+def threeDnoise_do_rmsynth_planes(dataQ, dataU, lambdaSqArr_m2, phiArr_radm2,
                       weightArr=None, lam0Sq_m2=None, nBits=32, verbose=False,log=print):
     """Perform RM-synthesis on Stokes Q and U cubes (1,2 or 3D). This version
     of the routine loops through spectral planes and is faster than the pixel-
     by-pixel code. This version also correctly deals with isolated clumps of
     NaN-flagged voxels within the data-cube (unlikely in interferometric cubes,
     but possible in single-dish cubes). Input data must be in standard python
     [z,y,x] order, where z is the frequency axis in ascending order.
@@ -1765,30 +1742,30 @@
     dataQ           ... 1, 2 or 3D Stokes Q data array
     dataU           ... 1, 2 or 3D Stokes U data array
     lambdaSqArr_m2  ... vector of wavelength^2 values (assending freq order)
     phiArr_radm2    ... vector of trial Faraday depth values
     weightArr       ... 1, 2 or 3D array of weights, default [None] is Uniform (all 1s)
     nBits           ... precision of data arrays [32]
     verbose         ... print feedback during calculation [False]
-    
+
     Returns:
         FDFcube     ... 1, 2, or 3D complex array of Faraday spectra
         lam0Sq_m2   ... 0, 1, or 2D array of lambda_0^2 values.
     """
-    
+
     log('3D noise functions are still in prototype stage! Proper function is not guaranteed!')
     # Default data types
     dtFloat = "float" + str(nBits)
     dtComplex = "complex" + str(2*nBits)
 
     # Set the weight array
     if weightArr is None:
         weightArr = np.ones(dataQ.shape, dtype=dtFloat)
     weightArr = np.where(np.isnan(weightArr), 0.0, weightArr)
-    
+
     # Sanity check on array sizes
     if (not weightArr.shape  == lambdaSqArr_m2.shape) and (not weightArr.shape == dataQ.shape):
         log("Err: Weight array must have same size as lambda^2 or Q/U arrays.")
         return None, None
     if not dataQ.shape == dataU.shape:
         log("Err: Stokes Q and U data arrays must be the same shape.")
         return None, None
@@ -1800,112 +1777,107 @@
         log("Err: data dimensions must be <= 3.")
         return None, None
     if not dataQ.shape[0] == lambdaSqArr_m2.shape[0]:
         log("Err: Data depth does not match lambda^2 vector (%d vs %d).", end=' ')
         (dataQ.shape[0], lambdaSqArr_m2.shape[0])
         print("     Check that data is in [z, y, x] order.")
         return None, None
-    
+
     # Reshape the data arrays to 3 dimensions
     if nDims==1:
         dataQ = np.reshape(dataQ, (dataQ.shape[0], 1, 1))
         dataU = np.reshape(dataU, (dataU.shape[0], 1, 1))
     elif nDims==2:
         dataQ = np.reshape(dataQ, (dataQ.shape[0], dataQ.shape[1], 1))
         dataU = np.reshape(dataU, (dataU.shape[0], dataU.shape[1], 1))
-    
+
     #Check shape of weight array and pad if necessary:
     if weightArr.ndim < 3:
         weightArr=np.repeat(weightArr,dataQ.shape)
-    
-    
+
+
     # Create a complex polarised cube, B&dB Eqns. (8) and (14)
     # Array has dimensions [nFreq, nY, nX]
     pCube = (dataQ + 1j * dataU) * weightArr
-    
+
     # Check for NaNs (flagged data) in the cube & set to zero
     mskCube = np.isnan(pCube)
     pCube = np.nan_to_num(pCube)
-    
+
     # If full planes are flagged then set corresponding weights to zero
     mskPlanes =  np.sum(np.sum(~mskCube, axis=1), axis=1)
     mskPlanes = np.where(mskPlanes==0, 0, 1)
     weightArr *= mskPlanes[:,np.newaxis,np.newaxis]
-    
+
     # Initialise the complex Faraday Dispersion Function cube
     nX = dataQ.shape[-1]
     nY = dataQ.shape[-2]
     nPhi = phiArr_radm2.shape[0]
     FDFcube = np.zeros((nPhi, nY, nX), dtype=dtComplex)
 
     # lam0Sq_m2 is the weighted mean of lambda^2 distribution (B&dB Eqn. 32)
     # Calculate a per-pixel lam0Sq_m2 value, ignoring isolated flagged voxels
     K = 1.0 / np.sum(weightArr,axis=0)
     if lam0Sq_m2 is None:
         lam0Sq_m2 = K * np.sum(weightArr * lambdaSqArr_m2[:,np.newaxis,np.newaxis],axis=0)
-    
+
     # The K value used to scale each FDF spectrum must take into account
     # flagged voxels data in the datacube and can be position dependent
     weightCube =  np.invert(mskCube) * weightArr
     with np.errstate(divide='ignore', invalid='ignore'):
         KArr = np.true_divide(1.0, np.sum(weightCube, axis=0))
         KArr[KArr == np.inf] = 0
         KArr = np.nan_to_num(KArr)
-        
+
     # Do the RM-synthesis on each plane
-    if verbose:
-        log("Running RM-synthesis by channel.")
-        progress(40, 0)
     a = lambdaSqArr_m2[:, np.newaxis, np.newaxis] - lam0Sq_m2[np.newaxis, :, :]
-    for i in range(nPhi):
-        if verbose:
-            progress(40, ((i+1)*100.0/nPhi))
+    for i in trange(nPhi, desc="Running RM-synthesis by channel", disable=not verbose):
         arg = np.exp(-2.0j * phiArr_radm2[i] * a)
         FDFcube[i, :, :] = KArr * np.sum(pCube * arg, axis=0)
     # Remove redundant dimensions in the FDF array
     FDFcube = np.squeeze(FDFcube)
     lam0Sq_m2=np.squeeze(lam0Sq_m2)
 
     return FDFcube, lam0Sq_m2
 
 
 #-----------------------------------------------------------------------------#
 #3D noise functions are still in prototype stage! Proper function is not guaranteed!
-def threeDnoise_get_rmsf_planes(lambdaSqArr_m2, phiArr_radm2, weightArr=None, 
+def threeDnoise_get_rmsf_planes(lambdaSqArr_m2, phiArr_radm2, weightArr=None,
                     lam0Sq_m2=None, double=True, fitRMSF=False,
                     fitRMSFreal=False, nBits=32, verbose=False,log=print):
     """Calculate the Rotation Measure Spread Function from inputs. This version
     returns a cube (1, 2 or 3D) of RMSF spectra based on the shape of a
     boolean mask and/or weight array, where flagged data are True and unflagged data False.
     If only whole planes (wavelength channels) are flagged then the RMSF is the
     same for all pixels and the calculation is done once and replicated to the
     dimensions of the mask. If some isolated voxels are flagged then the RMSF
     is calculated by looping through each wavelength plane, which can take some
     time. By default the routine returns the analytical width of the RMSF main
     lobe but can also use MPFIT to fit a Gaussian.
     This version assumes that masking for bad voxels has already been applied to the
     weight array (as zeros or NaNs).
     If no weight array is supplied, uniform (equal) weights are assumed.
-    
+
     lambdaSqArr_m2  ... vector of wavelength^2 values (assending freq order)
     phiArr_radm2    ... vector of trial Faraday depth values
-    weightArr       ... array (1/2/3D) of weights, default [None] is no weighting    
+    weightArr       ... array (1/2/3D) of weights, default [None] is no weighting
     lam0Sq_m2       ... force a reference lambda^2 value (def=calculate) [None]
     double          ... pad the Faraday depth to double-size [True]
     fitRMSF         ... fit the main lobe of the RMSF with a Gaussian [False]
     fitRMSFreal     ... fit RMSF.real, rather than abs(RMSF) [False]
     nBits           ... precision of data arrays [32]
     verbose         ... print feedback during calculation [False]
-    
+
     """
     log('3D noise functions are still in prototype stage! Proper function is not guaranteed!')
     # Default data types
     dtFloat = "float" + str(nBits)
     dtComplex = "complex" + str(2*nBits)
-    
+
     # For cleaning the RMSF should extend by 1/2 on each side in phi-space
     if double:
         nPhi = phiArr_radm2.shape[0]
         nExt = np.ceil(nPhi/2.0)
         resampIndxArr = np.arange(2.0 * nExt + nPhi) - nExt
         phi2Arr = extrap(resampIndxArr, np.arange(nPhi, dtype='int'),
                          phiArr_radm2)
@@ -1917,72 +1889,72 @@
         weightArr = np.ones(lambdaSqArr_m2.shape, dtype=dtFloat)
     weightArr = np.where(np.isnan(weightArr), 0.0, weightArr)
     nDims = weightArr.ndim
 
 
 
     # Set the mask array (default to 1D, no masked channels)
-    
-    
+
+
     # Sanity checks on array sizes
 #    if not weightArr.shape  == lambdaSqArr_m2.shape:
 #        print("Err: wavelength^2 and weight arrays must be the same shape.")
 #        return None, None, None, None
     if not nDims <= 3:
         log("Err: mask dimensions must be <= 3.")
         return None, None, None, None
     if not weightArr.shape[0] == lambdaSqArr_m2.shape[0]:
         log("Error: Weight depth does not match lambda^2 vector ({} vs {}).".format(weightArr.shape[0], lambdaSqArr_m2.shape[-1]))
 
         log("Check that the mask is in [z, y, x] order.")
         return None, None, None, None
-    
+
 
     #Adjust dimensions of weightArr to be 3D no matter what, for convenience/generality below
     if nDims == 1:
         weightArr=weightArr[:,np.newaxis,np.newaxis]
     elif nDims == 2:
         weightArr=weightArr[:,:,np.newaxis]
-    
-    
+
+
     # Initialise the complex RM Spread Function cube
     nX = weightArr.shape[-1]
     nY = weightArr.shape[-2]
     nPix = nX * nY
     nPhi = phi2Arr.shape[0]
     RMSFcube = np.ones((nPhi, nY, nX), dtype=dtComplex)
 
     # If full planes are flagged then set corresponding weights to zero
     #Check if weights are uniform across the image plane:
     pixel_variation=np.sum(np.std(weightArr,axis=(1,2)))
     if pixel_variation == 0.:
         do1Dcalc=True
     else:
         do1Dcalc=False
-    
-    
+
+
     # lam0Sq is the weighted mean of LambdaSq distribution (B&dB Eqn. 32)
     # Calculate a lam0Sq_m2 value per pixel, ignoring isolated flagged voxels
     K = 1.0 / np.nansum(weightArr,axis=0)
     lam0Sq_m2 = K * np.nansum(weightArr * lambdaSqArr_m2[:,np.newaxis,np.newaxis],axis=0)
 
-    # Calculate the analytical FWHM width of the main lobe    
+    # Calculate the analytical FWHM width of the main lobe
     fwhmRMSF = 2.0 * m.sqrt(3.0)/(np.nanmax(lambdaSqArr_m2) -
                                   np.nanmin(lambdaSqArr_m2))
 
     # Do a simple 1D calculation and replicate along X & Y axes
     if do1Dcalc:
         if verbose:
             log("Calculating 1D RMSF and replicating along X & Y axes.")
 
         # Calculate the RMSF
         a = (-2.0 * 1j * phi2Arr).astype(dtComplex)
         b = (lambdaSqArr_m2 - lam0Sq_m2[0,0])
         RMSFArr = K[0,0] * np.sum(weightArr[:,0,0] * np.exp( np.outer(a, b) ), 1)
-        
+
         # Fit the RMSF main lobe
         fitStatus = -1
         if fitRMSF:
             if verbose:
                 log("Fitting Gaussian to the main lobe.")
             if fitRMSFreal:
                 mp = fit_rmsf(phi2Arr, RMSFcube.real)
@@ -1999,60 +1971,48 @@
         # Replicate along X and Y axes
         RMSFcube = np.tile(RMSFArr[:, np.newaxis, np.newaxis], (1, nY, nX))
         fwhmRMSFArr = np.ones((nY,nX), dtype=dtFloat) * fwhmRMSF
         statArr = np.ones((nY, nX), dtype="int") * fitStatus
 
     # Calculate the RMSF at each pixel
     else:
-        if verbose:
-            log("Calculating RMSF in 3D.")
-
         # The K value used to scale each RMSF must take into account
         # isolated flagged voxels data in the datacube
         with np.errstate(divide='ignore', invalid='ignore'):
             KArr = np.true_divide(1.0, np.sum(weightArr, axis=0))
             KArr[KArr == np.inf] = 0
             KArr = np.nan_to_num(KArr)
 
         # Calculate the RMSF for each plane
-        if verbose:
-            progress(40, 0)
         a = lambdaSqArr_m2[:, np.newaxis, np.newaxis] - \
             lam0Sq_m2[np.newaxis, :, :]
-        for i in range(nPhi):
-            if verbose:
-                progress(40, ((i+1)*100.0/nPhi))
+        for i in trange(nPhi, desc="Calculating RMSF in 3D", disable=not verbose):
             arg = np.exp(-2.0j * phi2Arr[i] * a)
 #            RMSFcube[i,:,:] =  KArr * np.sum(uCube * arg, axis=0)
             RMSFcube[i,:,:] =  KArr * np.sum(weightArr * arg, axis=0)
         # Default to the analytical RMSF
         fwhmRMSFArr = np.ones((nY, nX), dtype=dtFloat) * fwhmRMSF
         statArr = np.ones((nY, nX), dtype="int") * (-1)
-    
+
         # Fit the RMSF main lobe
         if fitRMSF:
             if verbose:
                 log("Fitting main lobe in each RMSF spectrum.")
                 log("> This may take some time!")
-            progress(40, 0)
-            k = 0
-            for i in range(nX):
+            for i in trange(nX, desc="Fitting RMSF", disable=not verbose):
                 for j in range(nY):
-                    k += 1
-                    if verbose:
-                        progress(40, (k*100.0/nPix))
                     if fitRMSFreal:
                         mp = fit_rmsf(phi2Arr, RMSFcube[:,j,i].real)
                     else:
                         mp = fit_rmsf(phi2Arr, np.abs(RMSFcube[:,j,i]))
                     if not (mp is None or mp.status<1):
                         fwhmRMSFArr[j,i] = mp.params[2]
                         statArr[j,i]  = mp.status
-    
+
     # Remove redundant dimensions
     RMSFcube = np.squeeze(RMSFcube)
     fwhmRMSFArr = np.squeeze(fwhmRMSFArr)
     statArr = np.squeeze(statArr)
-    
+
     return RMSFcube, phi2Arr, fwhmRMSFArr, statArr
 
-    
+
```

### Comparing `RM-Tools-1.3.0/RMutils/util_misc.py` & `RM-Tools-1.3.1/RMutils/util_misc.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMutils/util_plotFITS.py` & `RM-Tools-1.3.1/RMutils/util_plotFITS.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMutils/util_plotTk.py` & `RM-Tools-1.3.1/RMutils/util_plotTk.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/RMutils/util_rec.py` & `RM-Tools-1.3.1/RMutils/util_rec.py`

 * *Files identical despite different names*

### Comparing `RM-Tools-1.3.0/setup.py` & `RM-Tools-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from setuptools import find_packages, setup, Command
 
 NAME = 'RM-Tools'
 DESCRIPTION = 'RM-synthesis, RM-clean and QU-fitting on polarised radio spectra'
 URL = 'https://github.com/CIRADA-Tools/RM-Tools'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.3.0'
+VERSION = '1.3.1'
 DOWNLOAD_URL = 'https://github.com/CIRADA-Tools/RM-Tools/archive/v'+VERSION+'.tar.gz'
 
 REQUIRED = [
     'numpy<1.24', 'scipy', 'matplotlib>=3.4.0', 'astropy',
 ]
 
 # Using AT's fork for now - includes tiny bug fix for bilby
```

