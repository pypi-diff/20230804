# Comparing `tmp/geofileops-0.8.0a7.tar.gz` & `tmp/geofileops-0.8.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geofileops-0.8.0a7.tar", last modified: Wed Jul 19 12:57:04 2023, max compression
+gzip compressed data, was "geofileops-0.8.0a8.tar", last modified: Thu Aug  3 23:04:48 2023, max compression
```

## Comparing `geofileops-0.8.0a7.tar` & `geofileops-0.8.0a8.tar`

### file list

```diff
@@ -1,93 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:57:04.817308 geofileops-0.8.0a7/
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-19 12:57:04.817308 geofileops-0.8.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:57:04.801308 geofileops-0.8.0a7/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/benchmark/benchmark_all.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/benchmark/benchmark_geofileops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/benchmark/benchmarker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:57:04.801308 geofileops-0.8.0a7/benchmark/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/benchmark/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/benchmark/benchmarks/benchmarks_geofileops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/benchmark/benchmarks/testdata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/benchmark/reporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:57:04.801308 geofileops-0.8.0a7/geofileops/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    88730 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/fileops.py
--rw-r--r--   0 runner    (1001) docker     (123)   109425 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/geoops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:57:04.801308 geofileops-0.8.0a7/geofileops/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/helpers/_parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/helpers/layerstyles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:57:04.805308 geofileops-0.8.0a7/geofileops/util/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/_general_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    80460 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/_geoops_gpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/_geoops_ogr.py
--rw-r--r--   0 runner    (1001) docker     (123)   119200 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/_geoops_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/_io_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/_ogr_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    23060 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/_ogr_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/_processing_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    22585 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/_sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/geodataframe_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/geofiletype.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/geofiletypes.csv
--rw-r--r--   0 runner    (1001) docker     (123)    30454 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12114 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/geoseries_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/grid_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/util/test.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/geofileops/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:57:04.801308 geofileops-0.8.0a7/geofileops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-19 12:57:04.000000 geofileops-0.8.0a7/geofileops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-19 12:57:04.000000 geofileops-0.8.0a7/geofileops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-19 12:57:04.000000 geofileops-0.8.0a7/geofileops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-19 12:57:04.000000 geofileops-0.8.0a7/geofileops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-19 12:57:04.000000 geofileops-0.8.0a7/geofileops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-19 12:57:04.817308 geofileops-0.8.0a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:57:04.813308 geofileops-0.8.0a7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-19 12:57:04.817308 geofileops-0.8.0a7/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   114688 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/BEFL-kbl.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/geofileops_testdata.qgz
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/linestring-row-trees.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   765952 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/linestring-watercourse.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/linestrings_hedges.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   106496 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/point.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   139264 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/polygon-invalid.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/polygon-no-rows.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/polygon-overlappingcircles-all.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/polygon-overlappingcircles-one.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/polygon-overlappingcircles-two+three.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   122880 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/polygon-parcel.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   126976 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/polygon-simplify-onborder-testcase.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/polygon-twolayers.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/polygon-zone.gpkg
--rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/polygonstyle.qml
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/data/polygonstyle.sld
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_general_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    51559 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_geofile.py
--rw-r--r--   0 runner    (1001) docker     (123)    21819 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_geofileops_singlelayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    44028 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_geofileops_singlelayer_gpd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_geofileops_singlelayer_ogr.py
--rw-r--r--   0 runner    (1001) docker     (123)    22235 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_geofileops_singlelayer_sql.py
--rw-r--r--   0 runner    (1001) docker     (123)    46731 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_geofileops_twolayers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_geofiletype.py
--rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_geometry_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_geoseries_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_grid_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_io_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_layerstyles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_ogr_sql_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_ogr_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_parameter_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_processing_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_spatialite.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_sqlite_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-19 12:56:51.000000 geofileops-0.8.0a7/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:04:48.574428 geofileops-0.8.0a8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-03 23:04:48.574428 geofileops-0.8.0a8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:04:48.558427 geofileops-0.8.0a8/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/benchmark/benchmark_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/benchmark/benchmark_geofileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/benchmark/benchmarker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:04:48.558427 geofileops-0.8.0a8/benchmark/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/benchmark/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10954 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/benchmark/benchmarks/benchmarks_geofileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/benchmark/benchmarks/testdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9121 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/benchmark/reporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:04:48.562427 geofileops-0.8.0a8/geofileops/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88730 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/fileops.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109464 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/geoops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:04:48.562427 geofileops-0.8.0a8/geofileops/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/helpers/_parameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/helpers/layerstyles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:04:48.566428 geofileops-0.8.0a8/geofileops/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/_general_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80416 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/_geoops_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/_geoops_ogr.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120919 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/_geoops_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4487 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/_io_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/_ogr_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23060 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/_ogr_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/_processing_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/_sqlite_userdefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24355 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/_sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/geodataframe_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/geofiletype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/geofiletypes.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    30454 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12089 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/geoseries_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/grid_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/util/test.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/geofileops/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:04:48.562427 geofileops-0.8.0a8/geofileops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-08-03 23:04:48.000000 geofileops-0.8.0a8/geofileops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-08-03 23:04:48.000000 geofileops-0.8.0a8/geofileops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 23:04:48.000000 geofileops-0.8.0a8/geofileops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-08-03 23:04:48.000000 geofileops-0.8.0a8/geofileops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-03 23:04:48.000000 geofileops-0.8.0a8/geofileops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 23:04:48.574428 geofileops-0.8.0a8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:04:48.570428 geofileops-0.8.0a8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:04:48.574428 geofileops-0.8.0a8/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   114688 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/BEFL-kbl.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    17534 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/geofileops_testdata.qgz
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/linestring-row-trees.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   765952 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/linestring-watercourse.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/linestrings_hedges.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   106496 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/point.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   139264 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/polygon-invalid.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/polygon-no-rows.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/polygon-overlappingcircles-all.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/polygon-overlappingcircles-one.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/polygon-overlappingcircles-two+three.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   122880 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/polygon-parcel.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   126976 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/polygon-simplify-onborder-testcase.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)   143360 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/polygon-twolayers.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    98304 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/polygon-zone.gpkg
+-rw-r--r--   0 runner    (1001) docker     (123)    19428 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/polygonstyle.qml
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/data/polygonstyle.sld
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_general_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51559 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_geofile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22578 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_geofileops_singlelayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44028 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_geofileops_singlelayer_gpd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_geofileops_singlelayer_ogr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22224 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_geofileops_singlelayer_sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47471 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_geofileops_twolayers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_geofiletype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28000 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_geometry_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11412 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_geoseries_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_grid_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12822 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_io_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_layerstyles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_ogr_sql_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_ogr_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_parameter_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_processing_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_spatialite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_sqlite_userdefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_sqlite_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-03 23:04:38.000000 geofileops-0.8.0a8/tests/test_version.py
```

### Comparing `geofileops-0.8.0a7/LICENSE.txt` & `geofileops-0.8.0a8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/PKG-INFO` & `geofileops-0.8.0a8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geofileops
-Version: 0.8.0a7
+Version: 0.8.0a8
 Summary: Package to do spatial operations on large geo files.
 Home-page: https://github.com/geofileops/geofileops
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `geofileops-0.8.0a7/README.md` & `geofileops-0.8.0a8/README.md`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/benchmark/benchmarker.py` & `geofileops-0.8.0a8/benchmark/benchmarker.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/benchmark/benchmarks/benchmarks_geofileops.py` & `geofileops-0.8.0a8/benchmark/benchmarks/benchmarks_geofileops.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/benchmark/benchmarks/testdata.py` & `geofileops-0.8.0a8/benchmark/benchmarks/testdata.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/benchmark/reporter.py` & `geofileops-0.8.0a8/benchmark/reporter.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/__init__.py` & `geofileops-0.8.0a8/geofileops/__init__.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/fileops.py` & `geofileops-0.8.0a8/geofileops/fileops.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/geoops.py` & `geofileops-0.8.0a8/geofileops/geoops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1177,15 +1177,15 @@
     )
 
 
 def simplify(
     input_path: Union[str, "os.PathLike[Any]"],
     output_path: Union[str, "os.PathLike[Any]"],
     tolerance: float,
-    algorithm: SimplifyAlgorithm = SimplifyAlgorithm.RAMER_DOUGLAS_PEUCKER,
+    algorithm: Union[str, SimplifyAlgorithm] = "rdp",
     lookahead: int = 8,
     input_layer: Optional[str] = None,
     output_layer: Optional[str] = None,
     columns: Optional[List[str]] = None,
     explodecollections: bool = False,
     gridsize: float = 0.0,
     keep_empty_geoms: Optional[bool] = None,
@@ -1206,16 +1206,16 @@
 
                 * RAMER_DOUGLAS_PEUCKER: distance to use as tolerance.
                 * LANG: distance to use as tolerance.
                 * VISVALINGAM_WHYATT: area to use as tolerance.
 
             In projected coordinate systems this tolerance will typically be
             in meter, in geodetic systems this is typically in degrees.
-        algorithm (SimplifyAlgorithm, optional): algorithm to use.
-            Defaults to SimplifyAlgorithm.RAMER_DOUGLAS_PEUCKER.
+        algorithm (str, optional): algorithm to use. Defaults to "rdp"
+            (Ramer Douglas Peucker).
         lookahead (int, optional): used for LANG algorithm. Defaults to 8.
         input_layer (str, optional): input layer name. Optional if the input
             file only contains one layer.
         output_layer (str, optional): input layer name. Optional if the input
             file only contains one layer.
         columns (List[str], optional): list of columns to retain. If None, all standard
             columns are retained. In addition to standard columns, it is also possible
@@ -1243,14 +1243,17 @@
 
     .. |spatialite_reference_link| raw:: html
 
         <a href="https://www.gaia-gis.it/gaia-sins/spatialite-sql-latest.html" target="_blank">spatialite reference</a>
 
     """  # noqa: E501
     logger.info(f"Start simplify on {input_path} with tolerance {tolerance}")
+    if isinstance(algorithm, str):
+        algorithm = SimplifyAlgorithm(algorithm)
+
     if keep_empty_geoms is None:
         keep_empty_geoms = False
         warnings.warn(
             "keep_empty_geoms defaults to False now for backwards compatibility, but "
             "this will change to True in a future version. If keep_empty_geoms is "
             "specified, this warning isn't shown anymore",
             FutureWarning,
```

### Comparing `geofileops-0.8.0a7/geofileops/helpers/_parameter_helper.py` & `geofileops-0.8.0a8/geofileops/helpers/_parameter_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/helpers/layerstyles.py` & `geofileops-0.8.0a8/geofileops/helpers/layerstyles.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/util/_general_util.py` & `geofileops-0.8.0a8/geofileops/util/_general_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,7 +162,20 @@
         return "{0:.2f} KB".format(bytes_float / KB)
     elif MB <= bytes_float < GB:
         return "{0:.2f} MB".format(bytes_float / MB)
     elif GB <= bytes_float < TB:
         return "{0:.2f} GB".format(bytes_float / GB)
     elif TB <= bytes_float:
         return "{0:.2f} TB".format(bytes_float / TB)
+
+
+def prepare_for_serialize(data: dict) -> dict:
+    prepared = {}
+    for key, value in data.items():
+        if isinstance(value, (dict)):
+            prepared[key] = prepare_for_serialize(value)
+        elif isinstance(value, (list, tuple)):
+            prepared[key] = value
+        else:
+            prepared[key] = str(value)
+
+    return prepared
```

### Comparing `geofileops-0.8.0a7/geofileops/util/_geoops_gpd.py` & `geofileops-0.8.0a8/geofileops/util/_geoops_gpd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1822,3208 +1822,3205 @@
 000071d0: 7461 5f67 6466 2c20 6770 642e 4765 6f44  ta_gdf, gpd.GeoD
 000071e0: 6174 6146 7261 6d65 290a 2020 2020 2020  ataFrame).      
 000071f0: 2020 6461 7461 5f67 6466 2e67 656f 6d65    data_gdf.geome
 00007200: 7472 7920 3d20 7368 6170 656c 7932 5f6f  try = shapely2_o
 00007210: 725f 7079 6765 6f73 2e73 6574 5f70 7265  r_pygeos.set_pre
 00007220: 6369 7369 6f6e 280a 2020 2020 2020 2020  cision(.        
 00007230: 2020 2020 6461 7461 5f67 6466 2e67 656f      data_gdf.geo
-00007240: 6d65 7472 792e 6172 7261 792e 6461 7461  metry.array.data
-00007250: 2c20 6772 6964 5f73 697a 653d 6772 6964  , grid_size=grid
-00007260: 7369 7a65 0a20 2020 2020 2020 2029 0a0a  size.        )..
-00007270: 2020 2020 2320 4966 2074 6865 2072 6573      # If the res
-00007280: 756c 7420 6973 2065 6d70 7479 2c20 616e  ult is empty, an
-00007290: 6420 6e6f 206f 7574 7075 7420 6765 6f6d  d no output geom
-000072a0: 6574 7279 7479 7065 2073 7065 6369 6669  etrytype specifi
-000072b0: 6564 2c20 7573 6520 696e 7075 740a 2020  ed, use input.  
-000072c0: 2020 2320 6765 6f6d 6574 7279 7479 7065    # geometrytype
-000072d0: 0a20 2020 2066 6f72 6365 5f6f 7574 7075  .    force_outpu
-000072e0: 745f 6765 6f6d 6574 7279 7479 7065 203d  t_geometrytype =
-000072f0: 204e 6f6e 650a 2020 2020 6966 206c 656e   None.    if len
-00007300: 2864 6174 615f 6764 6629 203d 3d20 303a  (data_gdf) == 0:
-00007310: 0a20 2020 2020 2020 2069 6e70 7574 5f6c  .        input_l
-00007320: 6179 6572 696e 666f 203d 2067 666f 2e67  ayerinfo = gfo.g
-00007330: 6574 5f6c 6179 6572 696e 666f 2869 6e70  et_layerinfo(inp
-00007340: 7574 5f70 6174 682c 2069 6e70 7574 5f6c  ut_path, input_l
-00007350: 6179 6572 290a 2020 2020 2020 2020 666f  ayer).        fo
-00007360: 7263 655f 6f75 7470 7574 5f67 656f 6d65  rce_output_geome
-00007370: 7472 7974 7970 6520 3d20 696e 7075 745f  trytype = input_
-00007380: 6c61 7965 7269 6e66 6f2e 6765 6f6d 6574  layerinfo.geomet
-00007390: 7279 7479 7065 2e74 6f5f 6d75 6c74 6974  rytype.to_multit
-000073a0: 7970 652e 6e61 6d65 0a0a 2020 2020 2320  ype.name..    # 
-000073b0: 6173 7365 7274 2074 6f20 6576 6164 6520  assert to evade 
-000073c0: 7079 4c61 6e63 6520 7761 726e 696e 670a  pyLance warning.
-000073d0: 2020 2020 6173 7365 7274 2069 7369 6e73      assert isins
-000073e0: 7461 6e63 6528 6461 7461 5f67 6466 2c20  tance(data_gdf, 
-000073f0: 6770 642e 4765 6f44 6174 6146 7261 6d65  gpd.GeoDataFrame
-00007400: 290a 2020 2020 2320 5573 6520 666f 7263  ).    # Use forc
-00007410: 655f 6d75 6c74 6974 7970 652c 2074 6f20  e_multitype, to 
-00007420: 6576 6164 6520 7761 726e 696e 6773 2077  evade warnings w
-00007430: 6865 6e20 736f 6d65 2062 6174 6368 6573  hen some batches
-00007440: 2063 6f6e 7461 696e 0a20 2020 2023 2073   contain.    # s
-00007450: 696e 676c 6574 7970 6520 616e 6420 736f  ingletype and so
-00007460: 6d65 2063 6f6e 7461 696e 206d 756c 7469  me contain multi
-00007470: 7479 7065 2067 656f 6d65 7472 6965 730a  type geometries.
-00007480: 2020 2020 6766 6f2e 746f 5f66 696c 6528      gfo.to_file(
-00007490: 0a20 2020 2020 2020 2067 6466 3d64 6174  .        gdf=dat
-000074a0: 615f 6764 662c 0a20 2020 2020 2020 2070  a_gdf,.        p
-000074b0: 6174 683d 6f75 7470 7574 5f70 6174 682c  ath=output_path,
-000074c0: 0a20 2020 2020 2020 206c 6179 6572 3d6f  .        layer=o
-000074d0: 7574 7075 745f 6c61 7965 722c 0a20 2020  utput_layer,.   
-000074e0: 2020 2020 2069 6e64 6578 3d46 616c 7365       index=False
-000074f0: 2c0a 2020 2020 2020 2020 666f 7263 655f  ,.        force_
-00007500: 6f75 7470 7574 5f67 656f 6d65 7472 7974  output_geometryt
-00007510: 7970 653d 666f 7263 655f 6f75 7470 7574  ype=force_output
-00007520: 5f67 656f 6d65 7472 7974 7970 652c 0a20  _geometrytype,. 
-00007530: 2020 2020 2020 2066 6f72 6365 5f6d 756c         force_mul
-00007540: 7469 7479 7065 3d54 7275 652c 0a20 2020  titype=True,.   
-00007550: 2020 2020 2063 7265 6174 655f 7370 6174       create_spat
-00007560: 6961 6c5f 696e 6465 783d 4661 6c73 652c  ial_index=False,
-00007570: 0a20 2020 2029 0a0a 2020 2020 6d65 7373  .    )..    mess
-00007580: 6167 6520 3d20 6622 546f 6f6b 207b 6461  age = f"Took {da
-00007590: 7465 7469 6d65 2e6e 6f77 2829 2d73 7461  tetime.now()-sta
-000075a0: 7274 5f74 696d 657d 2066 6f72 207b 6c65  rt_time} for {le
-000075b0: 6e28 6461 7461 5f67 6466 297d 2072 6f77  n(data_gdf)} row
-000075c0: 7320 287b 726f 7773 7d29 2122 0a20 2020  s ({rows})!".   
-000075d0: 2072 6574 7572 6e20 6d65 7373 6167 650a   return message.
-000075e0: 0a0a 6465 6620 6469 7373 6f6c 7665 280a  ..def dissolve(.
-000075f0: 2020 2020 696e 7075 745f 7061 7468 3a20      input_path: 
-00007600: 5061 7468 2c0a 2020 2020 6f75 7470 7574  Path,.    output
-00007610: 5f70 6174 683a 2050 6174 682c 0a20 2020  _path: Path,.   
-00007620: 2067 726f 7570 6279 5f63 6f6c 756d 6e73   groupby_columns
-00007630: 3a20 4f70 7469 6f6e 616c 5b49 7465 7261  : Optional[Itera
-00007640: 626c 655b 7374 725d 5d20 3d20 4e6f 6e65  ble[str]] = None
-00007650: 2c0a 2020 2020 6167 675f 636f 6c75 6d6e  ,.    agg_column
-00007660: 733a 204f 7074 696f 6e61 6c5b 6469 6374  s: Optional[dict
-00007670: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6578  ] = None,.    ex
-00007680: 706c 6f64 6563 6f6c 6c65 6374 696f 6e73  plodecollections
-00007690: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
-000076a0: 2020 2074 696c 6573 5f70 6174 683a 204f     tiles_path: O
-000076b0: 7074 696f 6e61 6c5b 5061 7468 5d20 3d20  ptional[Path] = 
-000076c0: 4e6f 6e65 2c0a 2020 2020 6e62 5f73 7175  None,.    nb_squ
-000076d0: 6172 6973 685f 7469 6c65 733a 2069 6e74  arish_tiles: int
-000076e0: 203d 2031 2c0a 2020 2020 696e 7075 745f   = 1,.    input_
-000076f0: 6c61 7965 723a 204f 7074 696f 6e61 6c5b  layer: Optional[
-00007700: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00007710: 206f 7574 7075 745f 6c61 7965 723a 204f   output_layer: O
-00007720: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
-00007730: 6f6e 652c 0a20 2020 2067 7269 6473 697a  one,.    gridsiz
-00007740: 653a 2066 6c6f 6174 203d 2030 2e30 2c0a  e: float = 0.0,.
-00007750: 2020 2020 7768 6572 653a 204f 7074 696f      where: Optio
-00007760: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00007770: 0a20 2020 206e 625f 7061 7261 6c6c 656c  .    nb_parallel
-00007780: 3a20 696e 7420 3d20 2d31 2c0a 2020 2020  : int = -1,.    
-00007790: 6261 7463 6873 697a 653a 2069 6e74 203d  batchsize: int =
-000077a0: 202d 312c 0a20 2020 2066 6f72 6365 3a20   -1,.    force: 
-000077b0: 626f 6f6c 203d 2046 616c 7365 2c0a 2920  bool = False,.) 
-000077c0: 2d3e 2064 6963 743a 0a20 2020 2022 2222  -> dict:.    """
-000077d0: 0a20 2020 2046 756e 6374 696f 6e20 7468  .    Function th
-000077e0: 6174 2061 7070 6c69 6573 2061 2064 6973  at applies a dis
-000077f0: 736f 6c76 652e 0a0a 2020 2020 4d6f 7265  solve...    More
-00007800: 2064 6574 6169 6c65 6420 646f 6375 6d65   detailed docume
-00007810: 6e74 6174 696f 6e20 696e 206d 6f64 756c  ntation in modul
-00007820: 6520 6765 6f6f 7073 210a 0a20 2020 2052  e geoops!..    R
-00007830: 656d 6172 6b3a 206b 6565 705f 656d 7074  emark: keep_empt
-00007840: 795f 6765 6f6d 7320 6973 206e 6f74 2069  y_geoms is not i
-00007850: 6d70 6c65 6d65 6e74 6564 2062 6563 6175  mplemented becau
-00007860: 7365 2074 6869 7320 6973 206e 6f74 2073  se this is not s
-00007870: 6f20 6561 7379 2062 6563 6175 7365 0a20  o easy because. 
-00007880: 2020 2028 666f 7220 706f 6c79 676f 6e20     (for polygon 
-00007890: 6469 7373 6f6c 7665 2920 7468 6520 6261  dissolve) the ba
-000078a0: 7463 6865 7320 6172 6520 6c6f 6361 7469  tches are locati
-000078b0: 6f6e 2062 6173 6564 2c20 616e 6420 6e75  on based, and nu
-000078c0: 6c6c 2f65 6d70 7479 2067 656f 6d65 7472  ll/empty geometr
-000078d0: 6965 730a 2020 2020 646f 6e27 7420 6861  ies.    don't ha
-000078e0: 7665 2061 206c 6f63 6174 696f 6e2e 2049  ve a location. I
-000078f0: 7420 636f 756c 6420 6265 2069 6d70 6c65  t could be imple
-00007900: 6d65 6e74 6564 2c20 6275 7420 6173 206c  mented, but as l
-00007910: 6f6e 6720 6173 206e 6f62 6f64 7920 6e65  ong as nobody ne
-00007920: 6564 7320 6974 2e2e 2e0a 2020 2020 2222  eds it....    ""
-00007930: 220a 0a20 2020 2023 2049 6e69 7420 616e  "..    # Init an
-00007940: 6420 7661 6c69 6461 7465 2069 6e70 7574  d validate input
-00007950: 2070 6172 616d 6574 6572 730a 2020 2020   parameters.    
-00007960: 2320 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  # --------------
-00007970: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00007980: 2d2d 2d2d 0a20 2020 2073 7461 7274 5f74  ----.    start_t
-00007990: 696d 6520 3d20 6461 7465 7469 6d65 2e6e  ime = datetime.n
-000079a0: 6f77 2829 0a20 2020 206f 7065 7261 7469  ow().    operati
-000079b0: 6f6e 203d 2022 6469 7373 6f6c 7665 220a  on = "dissolve".
-000079c0: 2020 2020 7265 7375 6c74 5f69 6e66 6f20      result_info 
-000079d0: 3d20 7b7d 0a0a 2020 2020 2320 4368 6563  = {}..    # Chec
-000079e0: 6b20 696e 7075 7420 7061 7261 6d65 7465  k input paramete
-000079f0: 7273 0a20 2020 2069 6620 6772 6f75 7062  rs.    if groupb
-00007a00: 795f 636f 6c75 6d6e 7320 6973 206e 6f74  y_columns is not
-00007a10: 204e 6f6e 6520 616e 6420 6c65 6e28 6c69   None and len(li
-00007a20: 7374 2867 726f 7570 6279 5f63 6f6c 756d  st(groupby_colum
-00007a30: 6e73 2929 203d 3d20 303a 0a20 2020 2020  ns)) == 0:.     
-00007a40: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00007a50: 726f 7228 2267 726f 7570 6279 5f63 6f6c  ror("groupby_col
-00007a60: 756d 6e73 3d5b 5d20 6973 206e 6f74 2073  umns=[] is not s
-00007a70: 7570 706f 7274 6564 2e20 5573 6520 4e6f  upported. Use No
-00007a80: 6e65 2e22 290a 2020 2020 6966 206e 6f74  ne.").    if not
-00007a90: 2069 6e70 7574 5f70 6174 682e 6578 6973   input_path.exis
-00007aa0: 7473 2829 3a0a 2020 2020 2020 2020 7261  ts():.        ra
-00007ab0: 6973 6520 5661 6c75 6545 7272 6f72 2866  ise ValueError(f
-00007ac0: 2269 6e70 7574 5f70 6174 6820 646f 6573  "input_path does
-00007ad0: 6e27 7420 6578 6973 743a 207b 696e 7075  n't exist: {inpu
-00007ae0: 745f 7061 7468 7d22 290a 2020 2020 6966  t_path}").    if
-00007af0: 2069 6e70 7574 5f70 6174 6820 3d3d 206f   input_path == o
-00007b00: 7574 7075 745f 7061 7468 3a0a 2020 2020  utput_path:.    
-00007b10: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00007b20: 7272 6f72 2822 6f75 7470 7574 5f70 6174  rror("output_pat
-00007b30: 6820 6d75 7374 206e 6f74 2065 7175 616c  h must not equal
-00007b40: 2069 6e70 7574 5f70 6174 6822 290a 0a20   input_path").. 
-00007b50: 2020 2069 6e70 7574 5f6c 6179 6572 696e     input_layerin
-00007b60: 666f 203d 2067 666f 2e67 6574 5f6c 6179  fo = gfo.get_lay
-00007b70: 6572 696e 666f 2869 6e70 7574 5f70 6174  erinfo(input_pat
-00007b80: 682c 2069 6e70 7574 5f6c 6179 6572 290a  h, input_layer).
-00007b90: 2020 2020 6966 2069 6e70 7574 5f6c 6179      if input_lay
-00007ba0: 6572 696e 666f 2e67 656f 6d65 7472 7974  erinfo.geometryt
-00007bb0: 7970 652e 746f 5f70 7269 6d69 7469 7665  ype.to_primitive
-00007bc0: 7479 7065 2069 6e20 5b0a 2020 2020 2020  type in [.      
-00007bd0: 2020 5072 696d 6974 6976 6554 7970 652e    PrimitiveType.
-00007be0: 504f 494e 542c 0a20 2020 2020 2020 2050  POINT,.        P
-00007bf0: 7269 6d69 7469 7665 5479 7065 2e4c 494e  rimitiveType.LIN
-00007c00: 4553 5452 494e 472c 0a20 2020 205d 3a0a  ESTRING,.    ]:.
-00007c10: 2020 2020 2020 2020 6966 2074 696c 6573          if tiles
-00007c20: 5f70 6174 6820 6973 206e 6f74 204e 6f6e  _path is not Non
-00007c30: 6520 6f72 206e 625f 7371 7561 7269 7368  e or nb_squarish
-00007c40: 5f74 696c 6573 203e 2031 3a0a 2020 2020  _tiles > 1:.    
-00007c50: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00007c60: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
-00007c70: 2020 2020 2020 2020 2020 6622 4469 7373            f"Diss
-00007c80: 6f6c 7665 2074 6f20 7469 6c65 7320 6973  olve to tiles is
-00007c90: 206e 6f74 2073 7570 706f 7274 6564 2066   not supported f
-00007ca0: 6f72 207b 696e 7075 745f 6c61 7965 7269  or {input_layeri
-00007cb0: 6e66 6f2e 6765 6f6d 6574 7279 7479 7065  nfo.geometrytype
-00007cc0: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
-00007cd0: 2020 2022 2c20 736f 2074 696c 6573 5f70     ", so tiles_p
-00007ce0: 6174 6820 7368 6f75 6c64 2062 6520 4e6f  ath should be No
-00007cf0: 6e65 2061 6e64 206e 625f 7371 7561 7269  ne and nb_squari
-00007d00: 7368 5f74 696c 6573 2073 686f 756c 6420  sh_tiles should 
-00007d10: 6265 2031 2922 0a20 2020 2020 2020 2020  be 1)".         
-00007d20: 2020 2029 0a0a 2020 2020 6966 2069 6e70     )..    if inp
-00007d30: 7574 5f6c 6179 6572 2069 7320 4e6f 6e65  ut_layer is None
-00007d40: 3a0a 2020 2020 2020 2020 696e 7075 745f  :.        input_
-00007d50: 6c61 7965 7220 3d20 6766 6f2e 6765 745f  layer = gfo.get_
-00007d60: 6f6e 6c79 5f6c 6179 6572 2869 6e70 7574  only_layer(input
-00007d70: 5f70 6174 6829 0a20 2020 2069 6620 6f75  _path).    if ou
-00007d80: 7470 7574 5f6c 6179 6572 2069 7320 4e6f  tput_layer is No
-00007d90: 6e65 3a0a 2020 2020 2020 2020 6f75 7470  ne:.        outp
-00007da0: 7574 5f6c 6179 6572 203d 2067 666f 2e67  ut_layer = gfo.g
-00007db0: 6574 5f64 6566 6175 6c74 5f6c 6179 6572  et_default_layer
-00007dc0: 286f 7574 7075 745f 7061 7468 290a 0a20  (output_path).. 
-00007dd0: 2020 2023 2043 6865 636b 2063 6f6c 756d     # Check colum
-00007de0: 6e73 2069 6e20 6772 6f75 7062 795f 636f  ns in groupby_co
-00007df0: 6c75 6d6e 730a 2020 2020 6966 2067 726f  lumns.    if gro
-00007e00: 7570 6279 5f63 6f6c 756d 6e73 2069 7320  upby_columns is 
-00007e10: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00007e20: 2020 636f 6c75 6d6e 735f 696e 5f6c 6179    columns_in_lay
-00007e30: 6572 5f75 7070 6572 203d 205b 0a20 2020  er_upper = [.   
-00007e40: 2020 2020 2020 2020 2063 6f6c 756d 6e2e           column.
-00007e50: 7570 7065 7228 2920 666f 7220 636f 6c75  upper() for colu
-00007e60: 6d6e 2069 6e20 6c69 7374 2869 6e70 7574  mn in list(input
-00007e70: 5f6c 6179 6572 696e 666f 2e63 6f6c 756d  _layerinfo.colum
-00007e80: 6e73 2920 2b20 5b22 6669 6422 5d0a 2020  ns) + ["fid"].  
-00007e90: 2020 2020 2020 5d0a 2020 2020 2020 2020        ].        
-00007ea0: 666f 7220 636f 6c75 6d6e 2069 6e20 6772  for column in gr
-00007eb0: 6f75 7062 795f 636f 6c75 6d6e 733a 0a20  oupby_columns:. 
-00007ec0: 2020 2020 2020 2020 2020 2069 6620 636f             if co
-00007ed0: 6c75 6d6e 2e75 7070 6572 2829 206e 6f74  lumn.upper() not
-00007ee0: 2069 6e20 636f 6c75 6d6e 735f 696e 5f6c   in columns_in_l
-00007ef0: 6179 6572 5f75 7070 6572 3a0a 2020 2020  ayer_upper:.    
-00007f00: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00007f10: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
-00007f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f30: 2020 6622 636f 6c75 6d6e 2069 6e20 6772    f"column in gr
-00007f40: 6f75 7062 795f 636f 6c75 6d6e 7320 6e6f  oupby_columns no
-00007f50: 7420 6176 6169 6c61 626c 6520 696e 206c  t available in l
-00007f60: 6179 6572 3a20 7b63 6f6c 756d 6e7d 220a  ayer: {column}".
-00007f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f80: 290a 0a20 2020 2023 2043 6865 636b 2061  )..    # Check a
-00007f90: 6767 5f63 6f6c 756d 6e73 2070 6172 616d  gg_columns param
-00007fa0: 0a20 2020 2069 6620 6167 675f 636f 6c75  .    if agg_colu
-00007fb0: 6d6e 7320 6973 206e 6f74 204e 6f6e 653a  mns is not None:
-00007fc0: 0a20 2020 2020 2020 2023 2056 616c 6964  .        # Valid
-00007fd0: 6174 6520 7468 6520 6469 6374 2073 7472  ate the dict str
-00007fe0: 7563 7475 7265 2c20 736f 2077 6520 6361  ucture, so we ca
-00007ff0: 6e20 6173 7375 6d65 2065 7665 7279 7468  n assume everyth
-00008000: 696e 6720 6973 204f 4b20 6675 7274 6865  ing is OK furthe
-00008010: 7220 6f6e 0a20 2020 2020 2020 205f 7061  r on.        _pa
-00008020: 7261 6d65 7465 725f 6865 6c70 6572 2e76  rameter_helper.v
-00008030: 616c 6964 6174 655f 6167 675f 636f 6c75  alidate_agg_colu
-00008040: 6d6e 7328 6167 675f 636f 6c75 6d6e 7329  mns(agg_columns)
-00008050: 0a0a 2020 2020 2020 2020 2320 4669 7273  ..        # Firs
-00008060: 7420 7461 6b65 2061 2064 6565 7020 636f  t take a deep co
-00008070: 7079 2c20 6173 2076 616c 7565 7320 6361  py, as values ca
-00008080: 6e20 6265 2063 6861 6e67 6564 2066 7572  n be changed fur
-00008090: 7468 6572 206f 6e20 746f 2074 7265 6174  ther on to treat
-000080a0: 2063 6f6c 756d 6e73 0a20 2020 2020 2020   columns.       
-000080b0: 2023 2063 6173 6520 696e 7365 6e73 6974   # case insensit
-000080c0: 6976 650a 2020 2020 2020 2020 6167 675f  ive.        agg_
-000080d0: 636f 6c75 6d6e 7320 3d20 6a73 6f6e 2e6c  columns = json.l
-000080e0: 6f61 6473 286a 736f 6e2e 6475 6d70 7328  oads(json.dumps(
-000080f0: 6167 675f 636f 6c75 6d6e 7329 290a 2020  agg_columns)).  
-00008100: 2020 2020 2020 6173 7365 7274 2061 6767        assert agg
-00008110: 5f63 6f6c 756d 6e73 2069 7320 6e6f 7420  _columns is not 
-00008120: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
-00008130: 226a 736f 6e22 2069 6e20 6167 675f 636f  "json" in agg_co
-00008140: 6c75 6d6e 733a 0a20 2020 2020 2020 2020  lumns:.         
-00008150: 2020 2069 6620 6167 675f 636f 6c75 6d6e     if agg_column
-00008160: 735b 226a 736f 6e22 5d20 6973 204e 6f6e  s["json"] is Non
-00008170: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00008180: 2020 2061 6767 5f63 6f6c 756d 6e73 5b22     agg_columns["
-00008190: 6a73 6f6e 225d 203d 205b 0a20 2020 2020  json"] = [.     
-000081a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-000081b0: 6f6c 2066 6f72 2063 6f6c 2069 6e20 696e  ol for col in in
-000081c0: 7075 745f 6c61 7965 7269 6e66 6f2e 636f  put_layerinfo.co
-000081d0: 6c75 6d6e 7320 6966 2063 6f6c 2e75 7070  lumns if col.upp
-000081e0: 6572 2829 2021 3d20 2249 4e44 4558 220a  er() != "INDEX".
-000081f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008200: 5d0a 2020 2020 2020 2020 2020 2020 656c  ].            el
-00008210: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00008220: 2020 2020 2320 416c 6967 6e20 6361 7369      # Align casi
-00008230: 6e67 206f 6620 636f 6c75 6d6e 206e 616d  ng of column nam
-00008240: 6573 2074 6f20 6461 7461 0a20 2020 2020  es to data.     
-00008250: 2020 2020 2020 2020 2020 2061 6767 5f63             agg_c
-00008260: 6f6c 756d 6e73 5b22 6a73 6f6e 225d 203d  olumns["json"] =
-00008270: 205f 6765 6e65 7261 6c5f 7574 696c 2e61   _general_util.a
-00008280: 6c69 676e 5f63 6173 696e 675f 6c69 7374  lign_casing_list
-00008290: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-000082a0: 2020 2020 2020 6167 675f 636f 6c75 6d6e        agg_column
-000082b0: 735b 226a 736f 6e22 5d2c 206c 6973 7428  s["json"], list(
-000082c0: 696e 7075 745f 6c61 7965 7269 6e66 6f2e  input_layerinfo.
-000082d0: 636f 6c75 6d6e 7329 202b 205b 2266 6964  columns) + ["fid
-000082e0: 225d 0a20 2020 2020 2020 2020 2020 2020  "].             
-000082f0: 2020 2029 0a20 2020 2020 2020 2065 6c69     ).        eli
-00008300: 6620 2263 6f6c 756d 6e73 2220 696e 2061  f "columns" in a
-00008310: 6767 5f63 6f6c 756d 6e73 3a0a 2020 2020  gg_columns:.    
-00008320: 2020 2020 2020 2020 2320 4c6f 6f70 2074          # Loop t
-00008330: 6872 6f75 6768 2061 6c6c 2072 6f77 730a  hrough all rows.
-00008340: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00008350: 6167 675f 636f 6c75 6d6e 2069 6e20 6167  agg_column in ag
-00008360: 675f 636f 6c75 6d6e 735b 2263 6f6c 756d  g_columns["colum
-00008370: 6e73 225d 3a0a 2020 2020 2020 2020 2020  ns"]:.          
-00008380: 2020 2020 2020 2320 4368 6563 6b20 6966        # Check if
-00008390: 2063 6f6c 756d 6e20 6578 6973 7473 202b   column exists +
-000083a0: 2073 6574 2063 6173 696e 6720 7361 6d65   set casing same
-000083b0: 2061 7320 696e 2064 6174 610a 2020 2020   as in data.    
-000083c0: 2020 2020 2020 2020 2020 2020 6167 675f              agg_
-000083d0: 636f 6c75 6d6e 5b22 636f 6c75 6d6e 225d  column["column"]
-000083e0: 203d 205f 6765 6e65 7261 6c5f 7574 696c   = _general_util
-000083f0: 2e61 6c69 676e 5f63 6173 696e 6728 0a20  .align_casing(. 
-00008400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008410: 2020 2061 6767 5f63 6f6c 756d 6e5b 2263     agg_column["c
-00008420: 6f6c 756d 6e22 5d2c 206c 6973 7428 696e  olumn"], list(in
-00008430: 7075 745f 6c61 7965 7269 6e66 6f2e 636f  put_layerinfo.co
-00008440: 6c75 6d6e 7329 202b 205b 2266 6964 225d  lumns) + ["fid"]
-00008450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008460: 2029 0a0a 2020 2020 2320 4e6f 7720 696e   )..    # Now in
-00008470: 7075 7420 7061 7261 6d65 7465 7273 2061  put parameters a
-00008480: 7265 2063 6865 636b 6564 2c20 6368 6563  re checked, chec
-00008490: 6b20 6966 2077 6520 6e65 6564 2074 6f20  k if we need to 
-000084a0: 6361 6c63 756c 6174 6520 616e 7977 6179  calculate anyway
-000084b0: 0a20 2020 2069 6620 6f75 7470 7574 5f70  .    if output_p
-000084c0: 6174 682e 6578 6973 7473 2829 3a0a 2020  ath.exists():.  
-000084d0: 2020 2020 2020 6966 2066 6f72 6365 2069        if force i
-000084e0: 7320 4661 6c73 653a 0a20 2020 2020 2020  s False:.       
-000084f0: 2020 2020 2072 6573 756c 745f 696e 666f       result_info
-00008500: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00008510: 2020 226d 6573 7361 6765 220a 2020 2020    "message".    
-00008520: 2020 2020 2020 2020 5d20 3d20 6622 6f75          ] = f"ou
-00008530: 7470 7574 2065 7869 7374 7320 616c 7265  tput exists alre
-00008540: 6164 7920 7b6f 7574 7075 745f 7061 7468  ady {output_path
-00008550: 7d20 616e 6420 666f 7263 6520 6973 2066  } and force is f
-00008560: 616c 7365 220a 2020 2020 2020 2020 2020  alse".          
-00008570: 2020 6c6f 6767 6572 2e69 6e66 6f28 7265    logger.info(re
-00008580: 7375 6c74 5f69 6e66 6f5b 226d 6573 7361  sult_info["messa
-00008590: 6765 225d 290a 2020 2020 2020 2020 2020  ge"]).          
-000085a0: 2020 7265 7475 726e 2072 6573 756c 745f    return result_
-000085b0: 696e 666f 0a20 2020 2020 2020 2065 6c73  info.        els
-000085c0: 653a 0a20 2020 2020 2020 2020 2020 2067  e:.            g
-000085d0: 666f 2e72 656d 6f76 6528 6f75 7470 7574  fo.remove(output
-000085e0: 5f70 6174 6829 0a0a 2020 2020 2320 4e6f  _path)..    # No
-000085f0: 7720 7374 6172 7420 6469 7373 6f6c 7669  w start dissolvi
-00008600: 6e67 0a20 2020 2023 202d 2d2d 2d2d 2d2d  ng.    # -------
-00008610: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 2020  -------------.  
-00008620: 2020 2320 456d 7074 7920 6f72 204c 696e    # Empty or Lin
-00008630: 6520 616e 6420 706f 696e 7420 6c61 7965  e and point laye
-00008640: 7273 2061 7265 3a0a 2020 2020 2320 2020  rs are:.    #   
-00008650: 2a20 6e6f 7420 736f 206c 6172 6765 2028  * not so large (
-00008660: 6d65 6d6f 7279 2d77 6973 6529 0a20 2020  memory-wise).   
-00008670: 2023 2020 202a 2061 7265 6e27 7420 636f   #   * aren't co
-00008680: 6d70 7574 6174 696f 6e61 6c6c 7920 6865  mputationally he
-00008690: 6176 790a 2020 2020 2320 4164 6469 7469  avy.    # Additi
-000086a0: 6f6e 616c 6c79 206c 696e 6520 6c61 7965  onally line laye
-000086b0: 7273 2061 7265 2061 2070 6169 6e20 746f  rs are a pain to
-000086c0: 2068 616e 646c 6520 636f 7272 6563 746c   handle correctl
-000086d0: 7920 6265 6361 7573 6520 6f66 0a20 2020  y because of.   
-000086e0: 2023 2072 6f75 6e64 696e 6720 6973 7375   # rounding issu
-000086f0: 6573 2061 7420 7468 6520 626f 7264 6572  es at the border
-00008700: 7320 6f66 2074 696c 6573 2e2e 2e20 736f  s of tiles... so
-00008710: 206a 7573 7420 6469 7373 6f6c 7665 2074   just dissolve t
-00008720: 6865 6d20 696e 206f 6e65 2067 6f2e 0a20  hem in one go.. 
-00008730: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-00008740: 696e 7075 745f 6c61 7965 7269 6e66 6f2e  input_layerinfo.
-00008750: 6665 6174 7572 6563 6f75 6e74 203d 3d20  featurecount == 
-00008760: 300a 2020 2020 2020 2020 6f72 2069 6e70  0.        or inp
-00008770: 7574 5f6c 6179 6572 696e 666f 2e67 656f  ut_layerinfo.geo
-00008780: 6d65 7472 7974 7970 652e 746f 5f70 7269  metrytype.to_pri
-00008790: 6d69 7469 7665 7479 7065 0a20 2020 2020  mitivetype.     
-000087a0: 2020 2069 6e20 5b0a 2020 2020 2020 2020     in [.        
-000087b0: 2020 2020 5072 696d 6974 6976 6554 7970      PrimitiveTyp
-000087c0: 652e 504f 494e 542c 0a20 2020 2020 2020  e.POINT,.       
-000087d0: 2020 2020 2050 7269 6d69 7469 7665 5479       PrimitiveTy
-000087e0: 7065 2e4c 494e 4553 5452 494e 472c 0a20  pe.LINESTRING,. 
-000087f0: 2020 2020 2020 205d 0a20 2020 2029 3a0a         ].    ):.
-00008800: 2020 2020 2020 2020 5f67 656f 6f70 735f          _geoops_
-00008810: 7371 6c2e 6469 7373 6f6c 7665 5f73 696e  sql.dissolve_sin
-00008820: 676c 6574 6872 6561 6428 0a20 2020 2020  glethread(.     
-00008830: 2020 2020 2020 2069 6e70 7574 5f70 6174         input_pat
-00008840: 683d 696e 7075 745f 7061 7468 2c0a 2020  h=input_path,.  
-00008850: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00008860: 5f70 6174 683d 6f75 7470 7574 5f70 6174  _path=output_pat
-00008870: 682c 0a20 2020 2020 2020 2020 2020 2065  h,.            e
-00008880: 7870 6c6f 6465 636f 6c6c 6563 7469 6f6e  xplodecollection
-00008890: 733d 6578 706c 6f64 6563 6f6c 6c65 6374  s=explodecollect
-000088a0: 696f 6e73 2c0a 2020 2020 2020 2020 2020  ions,.          
-000088b0: 2020 6772 6f75 7062 795f 636f 6c75 6d6e    groupby_column
-000088c0: 733d 6772 6f75 7062 795f 636f 6c75 6d6e  s=groupby_column
-000088d0: 732c 0a20 2020 2020 2020 2020 2020 2061  s,.            a
-000088e0: 6767 5f63 6f6c 756d 6e73 3d61 6767 5f63  gg_columns=agg_c
-000088f0: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
-00008900: 2020 2020 696e 7075 745f 6c61 7965 723d      input_layer=
-00008910: 696e 7075 745f 6c61 7965 722c 0a20 2020  input_layer,.   
-00008920: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-00008930: 6c61 7965 723d 6f75 7470 7574 5f6c 6179  layer=output_lay
-00008940: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
-00008950: 6772 6964 7369 7a65 3d67 7269 6473 697a  gridsize=gridsiz
-00008960: 652c 0a20 2020 2020 2020 2020 2020 206b  e,.            k
-00008970: 6565 705f 656d 7074 795f 6765 6f6d 733d  eep_empty_geoms=
-00008980: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-00008990: 2020 2077 6865 7265 3d77 6865 7265 2c0a     where=where,.
-000089a0: 2020 2020 2020 2020 2020 2020 666f 7263              forc
-000089b0: 653d 666f 7263 652c 0a20 2020 2020 2020  e=force,.       
-000089c0: 2029 0a0a 2020 2020 656c 6966 2069 6e70   )..    elif inp
-000089d0: 7574 5f6c 6179 6572 696e 666f 2e67 656f  ut_layerinfo.geo
-000089e0: 6d65 7472 7974 7970 652e 746f 5f70 7269  metrytype.to_pri
-000089f0: 6d69 7469 7665 7479 7065 2069 7320 5072  mitivetype is Pr
-00008a00: 696d 6974 6976 6554 7970 652e 504f 4c59  imitiveType.POLY
-00008a10: 474f 4e3a 0a20 2020 2020 2020 2023 2050  GON:.        # P
-00008a20: 7265 7061 7265 2077 6865 7265 0a20 2020  repare where.   
-00008a30: 2020 2020 2069 6620 7768 6572 6520 6973       if where is
-00008a40: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00008a50: 2020 2020 2020 2069 6620 7768 6572 6520         if where 
-00008a60: 3d3d 2022 223a 0a20 2020 2020 2020 2020  == "":.         
-00008a70: 2020 2020 2020 2077 6865 7265 203d 204e         where = N
-00008a80: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00008a90: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00008aa0: 2020 2020 2020 2320 5365 7420 6765 6f6d        # Set geom
-00008ab0: 6574 7279 636f 6c75 6d6e 2074 6f20 2267  etrycolumn to "g
-00008ac0: 656f 6d22 2c20 6265 6361 7573 6520 7465  eom", because te
-00008ad0: 6d70 2066 696c 6573 2061 7265 2073 6176  mp files are sav
-00008ae0: 6564 2061 7320 6770 6b67 2e0a 2020 2020  ed as gpkg..    
-00008af0: 2020 2020 2020 2020 2020 2020 7768 6572              wher
-00008b00: 6520 3d20 7768 6572 652e 666f 726d 6174  e = where.format
-00008b10: 2867 656f 6d65 7472 7963 6f6c 756d 6e3d  (geometrycolumn=
-00008b20: 2267 656f 6d22 290a 0a20 2020 2020 2020  "geom")..       
-00008b30: 2023 2049 6620 6120 7469 6c65 735f 7061   # If a tiles_pa
-00008b40: 7468 2069 7320 7370 6563 6966 6965 642c  th is specified,
-00008b50: 2072 6561 6420 7468 6f73 6520 7469 6c65   read those tile
-00008b60: 732e 2e2e 0a20 2020 2020 2020 2072 6573  s....        res
-00008b70: 756c 745f 7469 6c65 735f 6764 6620 3d20  ult_tiles_gdf = 
-00008b80: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
-00008b90: 7469 6c65 735f 7061 7468 2069 7320 6e6f  tiles_path is no
-00008ba0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00008bb0: 2020 2020 7265 7375 6c74 5f74 696c 6573      result_tiles
-00008bc0: 5f67 6466 203d 2067 666f 2e72 6561 645f  _gdf = gfo.read_
-00008bd0: 6669 6c65 2874 696c 6573 5f70 6174 6829  file(tiles_path)
-00008be0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00008bf0: 6e62 5f70 6172 616c 6c65 6c20 3d3d 202d  nb_parallel == -
-00008c00: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-00008c10: 2020 206e 625f 6370 7520 3d20 6d75 6c74     nb_cpu = mult
-00008c20: 6970 726f 6365 7373 696e 672e 6370 755f  iprocessing.cpu_
-00008c30: 636f 756e 7428 290a 2020 2020 2020 2020  count().        
-00008c40: 2020 2020 2020 2020 6e62 5f70 6172 616c          nb_paral
-00008c50: 6c65 6c20 3d20 6e62 5f63 7075 2020 2320  lel = nb_cpu  # 
-00008c60: 696e 7428 312e 3235 202a 206e 625f 6370  int(1.25 * nb_cp
-00008c70: 7529 0a20 2020 2020 2020 2020 2020 2020  u).             
-00008c80: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-00008c90: 6622 4e62 2063 7075 7320 666f 756e 643a  f"Nb cpus found:
-00008ca0: 207b 6e62 5f63 7075 7d2c 206e 625f 7061   {nb_cpu}, nb_pa
-00008cb0: 7261 6c6c 656c 3a20 7b6e 625f 7061 7261  rallel: {nb_para
-00008cc0: 6c6c 656c 7d22 290a 2020 2020 2020 2020  llel}").        
-00008cd0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00008ce0: 2020 2320 456c 7365 2c20 6372 6561 7465    # Else, create
-00008cf0: 2061 2067 7269 6420 6261 7365 6420 6f6e   a grid based on
-00008d00: 2074 6865 206e 756d 6265 7220 6f66 2074   the number of t
-00008d10: 696c 6573 2077 616e 7465 6420 6173 2072  iles wanted as r
-00008d20: 6573 756c 740a 2020 2020 2020 2020 2020  esult.          
-00008d30: 2020 2320 5573 6520 6120 6d61 7267 696e    # Use a margin
-00008d40: 206f 6620 3120 6d65 7465 7220 6172 6f75   of 1 meter arou
-00008d50: 6e64 2074 6865 2062 6f75 6e64 730a 2020  nd the bounds.  
-00008d60: 2020 2020 2020 2020 2020 6d61 7267 696e            margin
-00008d70: 203d 2031 2e30 0a20 2020 2020 2020 2020   = 1.0.         
-00008d80: 2020 2069 6620 696e 7075 745f 6c61 7965     if input_laye
-00008d90: 7269 6e66 6f2e 6372 7320 6973 206e 6f74  rinfo.crs is not
-00008da0: 204e 6f6e 6520 616e 6420 6e6f 7420 696e   None and not in
-00008db0: 7075 745f 6c61 7965 7269 6e66 6f2e 6372  put_layerinfo.cr
-00008dc0: 732e 6973 5f70 726f 6a65 6374 6564 3a0a  s.is_projected:.
-00008dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008de0: 2320 4966 2067 656f 6772 6170 6869 6320  # If geographic 
-00008df0: 6372 732c 2031 2064 6567 7265 6520 3d20  crs, 1 degree = 
-00008e00: 3131 3120 6b6d 206f 7220 3131 3130 3030  111 km or 111000
-00008e10: 206d 0a20 2020 2020 2020 2020 2020 2020   m.             
-00008e20: 2020 206d 6172 6769 6e20 2f3d 2031 3131     margin /= 111
-00008e30: 3030 300a 2020 2020 2020 2020 2020 2020  000.            
-00008e40: 626f 756e 6473 203d 2069 6e70 7574 5f6c  bounds = input_l
-00008e50: 6179 6572 696e 666f 2e74 6f74 616c 5f62  ayerinfo.total_b
-00008e60: 6f75 6e64 730a 2020 2020 2020 2020 2020  ounds.          
-00008e70: 2020 626f 756e 6473 203d 2028 0a20 2020    bounds = (.   
-00008e80: 2020 2020 2020 2020 2020 2020 2062 6f75               bou
-00008e90: 6e64 735b 305d 202d 206d 6172 6769 6e2c  nds[0] - margin,
-00008ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008eb0: 2062 6f75 6e64 735b 315d 202d 206d 6172   bounds[1] - mar
-00008ec0: 6769 6e2c 0a20 2020 2020 2020 2020 2020  gin,.           
-00008ed0: 2020 2020 2062 6f75 6e64 735b 325d 202b       bounds[2] +
-00008ee0: 206d 6172 6769 6e2c 0a20 2020 2020 2020   margin,.       
-00008ef0: 2020 2020 2020 2020 2062 6f75 6e64 735b           bounds[
-00008f00: 335d 202b 206d 6172 6769 6e2c 0a20 2020  3] + margin,.   
-00008f10: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00008f20: 2020 2020 2020 2072 6573 756c 745f 7469         result_ti
-00008f30: 6c65 735f 6764 6620 3d20 6772 6964 5f75  les_gdf = grid_u
-00008f40: 7469 6c2e 6372 6561 7465 5f67 7269 6432  til.create_grid2
-00008f50: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00008f60: 2020 626f 756e 6473 2c20 6e62 5f73 7175    bounds, nb_squ
-00008f70: 6172 6973 685f 7469 6c65 732c 2069 6e70  arish_tiles, inp
-00008f80: 7574 5f6c 6179 6572 696e 666f 2e63 7273  ut_layerinfo.crs
-00008f90: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00008fa0: 2020 2020 2020 2020 2320 4170 706c 7920          # Apply 
-00008fb0: 6772 6964 7369 7a65 2074 6f6c 6572 616e  gridsize toleran
-00008fc0: 6365 206f 6e20 7469 6c65 732c 206f 7468  ce on tiles, oth
-00008fd0: 6572 7769 7365 2074 6865 2062 6f72 6465  erwise the borde
-00008fe0: 7220 706f 6c79 676f 6e73 2063 616e 2774  r polygons can't
-00008ff0: 2062 650a 2020 2020 2020 2020 2320 756e   be.        # un
-00009000: 696f 6e65 6420 7072 6f70 6572 6c79 2062  ioned properly b
-00009010: 6563 6175 7365 2067 6170 7320 6170 7065  ecause gaps appe
-00009020: 6172 2061 6674 6572 2072 6f75 6e64 696e  ar after roundin
-00009030: 6720 636f 6f72 6469 6e61 7465 732e 0a20  g coordinates.. 
-00009040: 2020 2020 2020 2069 6620 6772 6964 7369         if gridsi
-00009050: 7a65 2021 3d20 302e 303a 0a20 2020 2020  ze != 0.0:.     
-00009060: 2020 2020 2020 2072 6573 756c 745f 7469         result_ti
-00009070: 6c65 735f 6764 662e 6765 6f6d 6574 7279  les_gdf.geometry
-00009080: 203d 2073 6861 7065 6c79 325f 6f72 5f70   = shapely2_or_p
-00009090: 7967 656f 732e 7365 745f 7072 6563 6973  ygeos.set_precis
-000090a0: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-000090b0: 2020 2020 2072 6573 756c 745f 7469 6c65       result_tile
-000090c0: 735f 6764 662e 6765 6f6d 6574 7279 2e61  s_gdf.geometry.a
-000090d0: 7272 6179 2e64 6174 612c 2067 7269 645f  rray.data, grid_
-000090e0: 7369 7a65 3d67 7269 6473 697a 650a 2020  size=gridsize.  
-000090f0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00009100: 2020 2020 6966 206c 656e 2872 6573 756c      if len(resul
-00009110: 745f 7469 6c65 735f 6764 6629 203e 2031  t_tiles_gdf) > 1
-00009120: 3a0a 2020 2020 2020 2020 2020 2020 6766  :.            gf
-00009130: 6f2e 746f 5f66 696c 6528 0a20 2020 2020  o.to_file(.     
-00009140: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-00009150: 745f 7469 6c65 735f 6764 662c 0a20 2020  t_tiles_gdf,.   
-00009160: 2020 2020 2020 2020 2020 2020 206f 7574               out
-00009170: 7075 745f 7061 7468 2e70 6172 656e 7420  put_path.parent 
-00009180: 2f20 6622 7b6f 7574 7075 745f 7061 7468  / f"{output_path
-00009190: 2e73 7465 6d7d 5f74 696c 6573 2e67 706b  .stem}_tiles.gpk
-000091a0: 6722 2c0a 2020 2020 2020 2020 2020 2020  g",.            
-000091b0: 290a 0a20 2020 2020 2020 2023 2049 6620  )..        # If 
-000091c0: 6120 7469 6c65 6420 7265 7375 6c74 2069  a tiled result i
-000091d0: 7320 6173 6b65 642c 2061 6464 2074 696c  s asked, add til
-000091e0: 655f 6964 2074 6f20 6772 6f75 7020 6f6e  e_id to group on
-000091f0: 2066 6f72 2074 6865 2072 6573 756c 740a   for the result.
-00009200: 2020 2020 2020 2020 6966 206c 656e 2872          if len(r
-00009210: 6573 756c 745f 7469 6c65 735f 6764 6629  esult_tiles_gdf)
-00009220: 203e 2031 3a0a 2020 2020 2020 2020 2020   > 1:.          
-00009230: 2020 7265 7375 6c74 5f74 696c 6573 5f67    result_tiles_g
-00009240: 6466 5b22 7469 6c65 5f69 6422 5d20 3d20  df["tile_id"] = 
-00009250: 7265 7375 6c74 5f74 696c 6573 5f67 6466  result_tiles_gdf
-00009260: 2e72 6573 6574 5f69 6e64 6578 2829 2e69  .reset_index().i
-00009270: 6e64 6578 0a0a 2020 2020 2020 2020 2320  ndex..        # 
-00009280: 5468 6520 6469 7373 6f6c 7665 2066 6f72  The dissolve for
-00009290: 2070 6f6c 7967 6f6e 7320 6973 2064 6f6e   polygons is don
-000092a0: 6520 696e 2073 6576 6572 616c 2070 6173  e in several pas
-000092b0: 7365 732c 2061 6e64 2061 6674 6572 2074  ses, and after t
-000092c0: 6865 2066 6972 7374 0a20 2020 2020 2020  he first.       
-000092d0: 2023 2070 6173 732c 206f 6e6c 7920 7468   # pass, only th
-000092e0: 6520 276f 6e62 6f72 6465 7227 2066 6561  e 'onborder' fea
-000092f0: 7475 7265 7320 6172 6520 6675 7274 6865  tures are furthe
-00009300: 7220 6469 7373 6f6c 7665 642c 2061 7320  r dissolved, as 
-00009310: 7468 650a 2020 2020 2020 2020 2320 276e  the.        # 'n
-00009320: 6f74 6f6e 626f 7264 6572 2720 6665 6174  otonborder' feat
-00009330: 7572 6573 2061 7265 2061 6c72 6561 6479  ures are already
-00009340: 204f 4b2e 0a20 2020 2020 2020 2074 656d   OK..        tem
-00009350: 7064 6972 203d 205f 696f 5f75 7469 6c2e  pdir = _io_util.
-00009360: 6372 6561 7465 5f74 656d 7064 6972 2866  create_tempdir(f
-00009370: 2267 656f 6669 6c65 6f70 732f 7b6f 7065  "geofileops/{ope
-00009380: 7261 7469 6f6e 7d22 290a 2020 2020 2020  ration}").      
-00009390: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
-000093a0: 2020 2069 6620 6f75 7470 7574 5f6c 6179     if output_lay
-000093b0: 6572 2069 7320 4e6f 6e65 3a0a 2020 2020  er is None:.    
-000093c0: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-000093d0: 7574 5f6c 6179 6572 203d 2067 666f 2e67  ut_layer = gfo.g
-000093e0: 6574 5f64 6566 6175 6c74 5f6c 6179 6572  et_default_layer
-000093f0: 286f 7574 7075 745f 7061 7468 290a 2020  (output_path).  
-00009400: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00009410: 5f74 6d70 5f70 6174 6820 3d20 7465 6d70  _tmp_path = temp
-00009420: 6469 7220 2f20 226f 7574 7075 745f 746d  dir / "output_tm
-00009430: 702e 6770 6b67 220a 2020 2020 2020 2020  p.gpkg".        
-00009440: 2020 2020 7072 6576 5f6e 625f 6261 7463      prev_nb_batc
-00009450: 6865 7320 3d20 4e6f 6e65 0a20 2020 2020  hes = None.     
-00009460: 2020 2020 2020 206c 6173 745f 7061 7373         last_pass
-00009470: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-00009480: 2020 2020 2070 6173 735f 6964 203d 2030       pass_id = 0
-00009490: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-000094a0: 6765 722e 696e 666f 2866 2253 7461 7274  ger.info(f"Start
-000094b0: 2064 6973 736f 6c76 6520 6f6e 2066 696c   dissolve on fil
-000094c0: 6520 7b69 6e70 7574 5f70 6174 687d 2229  e {input_path}")
-000094d0: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
-000094e0: 7574 5f70 6173 735f 6c61 7965 7220 3d20  ut_pass_layer = 
-000094f0: 696e 7075 745f 6c61 7965 720a 2020 2020  input_layer.    
-00009500: 2020 2020 2020 2020 7768 696c 6520 5472          while Tr
-00009510: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
-00009520: 2020 2020 2320 4765 7420 696e 666f 206f      # Get info o
-00009530: 6620 7468 6520 6375 7272 656e 7420 6669  f the current fi
-00009540: 6c65 2074 6861 7420 6e65 6564 7320 746f  le that needs to
-00009550: 2062 6520 6469 7373 6f6c 7665 640a 2020   be dissolved.  
-00009560: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00009570: 7075 745f 7061 7373 5f6c 6179 6572 696e  put_pass_layerin
-00009580: 666f 203d 2067 666f 2e67 6574 5f6c 6179  fo = gfo.get_lay
-00009590: 6572 696e 666f 2869 6e70 7574 5f70 6174  erinfo(input_pat
-000095a0: 682c 2069 6e70 7574 5f70 6173 735f 6c61  h, input_pass_la
-000095b0: 7965 7229 0a20 2020 2020 2020 2020 2020  yer).           
-000095c0: 2020 2020 206e 625f 726f 7773 5f74 6f74       nb_rows_tot
-000095d0: 616c 203d 2069 6e70 7574 5f70 6173 735f  al = input_pass_
-000095e0: 6c61 7965 7269 6e66 6f2e 6665 6174 7572  layerinfo.featur
-000095f0: 6563 6f75 6e74 0a0a 2020 2020 2020 2020  ecount..        
-00009600: 2020 2020 2020 2020 2320 4361 6c63 756c          # Calcul
-00009610: 6174 6520 7468 6520 6265 7374 206e 756d  ate the best num
-00009620: 6265 7220 6f66 2070 6172 616c 6c65 6c20  ber of parallel 
-00009630: 7072 6f63 6573 7365 7320 616e 6420 6261  processes and ba
-00009640: 7463 6865 7320 666f 720a 2020 2020 2020  tches for.      
-00009650: 2020 2020 2020 2020 2020 2320 7468 6520            # the 
-00009660: 6176 6169 6c61 626c 6520 7265 736f 7572  available resour
-00009670: 6365 7320 666f 7220 7468 6520 6375 7272  ces for the curr
-00009680: 656e 7420 7061 7373 0a20 2020 2020 2020  ent pass.       
-00009690: 2020 2020 2020 2020 2069 6620 6261 7463           if batc
-000096a0: 6873 697a 6520 3e20 303a 0a20 2020 2020  hsize > 0:.     
-000096b0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-000096c0: 6172 616c 6c65 6c69 7a61 7469 6f6e 5f63  arallelization_c
-000096d0: 6f6e 6669 6720 3d20 5061 7261 6c6c 656c  onfig = Parallel
-000096e0: 697a 6174 696f 6e43 6f6e 6669 6728 0a20  izationConfig(. 
-000096f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009700: 2020 2020 2020 206d 696e 5f61 7667 5f72         min_avg_r
-00009710: 6f77 735f 7065 725f 6261 7463 683d 696e  ows_per_batch=in
-00009720: 7428 6d61 7468 2e63 6569 6c28 6261 7463  t(math.ceil(batc
-00009730: 6873 697a 6520 2f20 3229 292c 0a20 2020  hsize / 2)),.   
-00009740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009750: 2020 2020 206d 6178 5f61 7667 5f72 6f77       max_avg_row
-00009760: 735f 7065 725f 6261 7463 683d 6261 7463  s_per_batch=batc
-00009770: 6873 697a 652c 0a20 2020 2020 2020 2020  hsize,.         
-00009780: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00009790: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-000097a0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-000097b0: 2020 2020 2020 2070 6172 616c 6c65 6c69         paralleli
-000097c0: 7a61 7469 6f6e 5f63 6f6e 6669 6720 3d20  zation_config = 
-000097d0: 5061 7261 6c6c 656c 697a 6174 696f 6e43  ParallelizationC
-000097e0: 6f6e 6669 6728 290a 2020 2020 2020 2020  onfig().        
-000097f0: 2020 2020 2020 2020 6e62 5f70 6172 616c          nb_paral
-00009800: 6c65 6c2c 206e 625f 6261 7463 6865 735f  lel, nb_batches_
-00009810: 7265 636f 6d6d 656e 6465 642c 205f 203d  recommended, _ =
-00009820: 2067 6574 5f70 6172 616c 6c65 6c69 7a61   get_paralleliza
-00009830: 7469 6f6e 5f70 6172 616d 7328 0a20 2020  tion_params(.   
-00009840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009850: 206e 625f 726f 7773 5f74 6f74 616c 3d6e   nb_rows_total=n
-00009860: 625f 726f 7773 5f74 6f74 616c 2c0a 2020  b_rows_total,.  
-00009870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009880: 2020 6e62 5f70 6172 616c 6c65 6c3d 6e62    nb_parallel=nb
-00009890: 5f70 6172 616c 6c65 6c2c 0a20 2020 2020  _parallel,.     
-000098a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-000098b0: 625f 6261 7463 6865 735f 7072 6576 696f  b_batches_previo
-000098c0: 7573 5f70 6173 733d 7072 6576 5f6e 625f  us_pass=prev_nb_
-000098d0: 6261 7463 6865 732c 0a20 2020 2020 2020  batches,.       
-000098e0: 2020 2020 2020 2020 2020 2020 2070 6172               par
-000098f0: 616c 6c65 6c69 7a61 7469 6f6e 5f63 6f6e  allelization_con
-00009900: 6669 673d 7061 7261 6c6c 656c 697a 6174  fig=parallelizat
-00009910: 696f 6e5f 636f 6e66 6967 2c0a 2020 2020  ion_config,.    
-00009920: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00009930: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00009940: 2049 6620 7468 6520 6964 6561 6c20 6e75   If the ideal nu
-00009950: 6d62 6572 206f 6620 6261 7463 6865 7320  mber of batches 
-00009960: 6973 2063 6c6f 7365 2074 6f20 7468 6520  is close to the 
-00009970: 6e62 2e20 7265 7375 6c74 2074 696c 6573  nb. result tiles
-00009980: 2061 736b 6564 2c0a 2020 2020 2020 2020   asked,.        
-00009990: 2020 2020 2020 2020 2320 6469 7373 6f6c          # dissol
-000099a0: 7665 2074 6f77 6172 6473 2074 6865 2061  ve towards the a
-000099b0: 736b 6564 2072 6573 756c 7421 0a20 2020  sked result!.   
-000099c0: 2020 2020 2020 2020 2020 2020 2023 2049               # I
-000099d0: 6620 6e6f 742c 2061 2074 656d 706f 7261  f not, a tempora
-000099e0: 7279 2072 6573 756c 7420 6973 2063 7265  ry result is cre
-000099f0: 6174 6564 2075 7369 6e67 2073 6d61 6c6c  ated using small
-00009a00: 6572 2074 696c 6573 0a20 2020 2020 2020  er tiles.       
-00009a10: 2020 2020 2020 2020 2069 6620 6e62 5f62           if nb_b
-00009a20: 6174 6368 6573 5f72 6563 6f6d 6d65 6e64  atches_recommend
-00009a30: 6564 203c 3d20 6c65 6e28 7265 7375 6c74  ed <= len(result
-00009a40: 5f74 696c 6573 5f67 6466 2920 2a20 312e  _tiles_gdf) * 1.
-00009a50: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
-00009a60: 2020 2020 2020 2074 696c 6573 5f67 6466         tiles_gdf
-00009a70: 203d 2072 6573 756c 745f 7469 6c65 735f   = result_tiles_
-00009a80: 6764 660a 2020 2020 2020 2020 2020 2020  gdf.            
-00009a90: 2020 2020 2020 2020 6c61 7374 5f70 6173          last_pas
-00009aa0: 7320 3d20 5472 7565 0a20 2020 2020 2020  s = True.       
-00009ab0: 2020 2020 2020 2020 2020 2020 206e 625f               nb_
-00009ac0: 7061 7261 6c6c 656c 203d 206d 696e 286c  parallel = min(l
-00009ad0: 656e 2872 6573 756c 745f 7469 6c65 735f  en(result_tiles_
-00009ae0: 6764 6629 2c20 6e62 5f70 6172 616c 6c65  gdf), nb_paralle
-00009af0: 6c29 0a20 2020 2020 2020 2020 2020 2020  l).             
-00009b00: 2020 2065 6c69 6620 6c65 6e28 7265 7375     elif len(resu
-00009b10: 6c74 5f74 696c 6573 5f67 6466 2920 3d3d  lt_tiles_gdf) ==
-00009b20: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-00009b30: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
-00009b40: 2061 2067 7269 6420 6261 7365 6420 6f6e   a grid based on
-00009b50: 2074 6865 2069 6465 616c 206e 756d 6265   the ideal numbe
-00009b60: 7220 6f66 2062 6174 6368 6573 2c20 6275  r of batches, bu
-00009b70: 7420 6d61 6b65 0a20 2020 2020 2020 2020  t make.         
-00009b80: 2020 2020 2020 2020 2020 2023 2073 7572             # sur
-00009b90: 6520 7468 6520 6e75 6d62 6572 2069 7320  e the number is 
-00009ba0: 736d 616c 6c65 7220 7468 616e 2074 6865  smaller than the
-00009bb0: 206d 6178 696d 756d 2e2e 2e0a 2020 2020   maximum....    
-00009bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bd0: 6e62 5f73 7175 6172 6973 685f 7469 6c65  nb_squarish_tile
-00009be0: 735f 6d61 7820 3d20 4e6f 6e65 0a20 2020  s_max = None.   
-00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c00: 2069 6620 7072 6576 5f6e 625f 6261 7463   if prev_nb_batc
-00009c10: 6865 7320 6973 206e 6f74 204e 6f6e 653a  hes is not None:
-00009c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009c30: 2020 2020 2020 2020 206e 625f 7371 7561           nb_squa
-00009c40: 7269 7368 5f74 696c 6573 5f6d 6178 203d  rish_tiles_max =
-00009c50: 206d 6178 2870 7265 765f 6e62 5f62 6174   max(prev_nb_bat
-00009c60: 6368 6573 202d 2031 2c20 3129 0a20 2020  ches - 1, 1).   
-00009c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009c80: 2074 696c 6573 5f67 6466 203d 2067 7269   tiles_gdf = gri
-00009c90: 645f 7574 696c 2e63 7265 6174 655f 6772  d_util.create_gr
-00009ca0: 6964 3228 0a20 2020 2020 2020 2020 2020  id2(.           
-00009cb0: 2020 2020 2020 2020 2020 2020 2074 6f74               tot
-00009cc0: 616c 5f62 6f75 6e64 733d 696e 7075 745f  al_bounds=input_
-00009cd0: 7061 7373 5f6c 6179 6572 696e 666f 2e74  pass_layerinfo.t
-00009ce0: 6f74 616c 5f62 6f75 6e64 732c 0a20 2020  otal_bounds,.   
-00009cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d00: 2020 2020 206e 625f 7371 7561 7269 7368       nb_squarish
-00009d10: 5f74 696c 6573 3d6e 625f 6261 7463 6865  _tiles=nb_batche
-00009d20: 735f 7265 636f 6d6d 656e 6465 642c 0a20  s_recommended,. 
-00009d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d40: 2020 2020 2020 206e 625f 7371 7561 7269         nb_squari
-00009d50: 7368 5f74 696c 6573 5f6d 6178 3d6e 625f  sh_tiles_max=nb_
-00009d60: 7371 7561 7269 7368 5f74 696c 6573 5f6d  squarish_tiles_m
-00009d70: 6178 2c0a 2020 2020 2020 2020 2020 2020  ax,.            
-00009d80: 2020 2020 2020 2020 2020 2020 6372 733d              crs=
-00009d90: 696e 7075 745f 7061 7373 5f6c 6179 6572  input_pass_layer
-00009da0: 696e 666f 2e63 7273 2c0a 2020 2020 2020  info.crs,.      
-00009db0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00007240: 6d65 7472 792c 2067 7269 645f 7369 7a65  metry, grid_size
+00007250: 3d67 7269 6473 697a 650a 2020 2020 2020  =gridsize.      
+00007260: 2020 290a 0a20 2020 2023 2049 6620 7468    )..    # If th
+00007270: 6520 7265 7375 6c74 2069 7320 656d 7074  e result is empt
+00007280: 792c 2061 6e64 206e 6f20 6f75 7470 7574  y, and no output
+00007290: 2067 656f 6d65 7472 7974 7970 6520 7370   geometrytype sp
+000072a0: 6563 6966 6965 642c 2075 7365 2069 6e70  ecified, use inp
+000072b0: 7574 0a20 2020 2023 2067 656f 6d65 7472  ut.    # geometr
+000072c0: 7974 7970 650a 2020 2020 666f 7263 655f  ytype.    force_
+000072d0: 6f75 7470 7574 5f67 656f 6d65 7472 7974  output_geometryt
+000072e0: 7970 6520 3d20 4e6f 6e65 0a20 2020 2069  ype = None.    i
+000072f0: 6620 6c65 6e28 6461 7461 5f67 6466 2920  f len(data_gdf) 
+00007300: 3d3d 2030 3a0a 2020 2020 2020 2020 696e  == 0:.        in
+00007310: 7075 745f 6c61 7965 7269 6e66 6f20 3d20  put_layerinfo = 
+00007320: 6766 6f2e 6765 745f 6c61 7965 7269 6e66  gfo.get_layerinf
+00007330: 6f28 696e 7075 745f 7061 7468 2c20 696e  o(input_path, in
+00007340: 7075 745f 6c61 7965 7229 0a20 2020 2020  put_layer).     
+00007350: 2020 2066 6f72 6365 5f6f 7574 7075 745f     force_output_
+00007360: 6765 6f6d 6574 7279 7479 7065 203d 2069  geometrytype = i
+00007370: 6e70 7574 5f6c 6179 6572 696e 666f 2e67  nput_layerinfo.g
+00007380: 656f 6d65 7472 7974 7970 652e 746f 5f6d  eometrytype.to_m
+00007390: 756c 7469 7479 7065 2e6e 616d 650a 0a20  ultitype.name.. 
+000073a0: 2020 2023 2061 7373 6572 7420 746f 2065     # assert to e
+000073b0: 7661 6465 2070 794c 616e 6365 2077 6172  vade pyLance war
+000073c0: 6e69 6e67 0a20 2020 2061 7373 6572 7420  ning.    assert 
+000073d0: 6973 696e 7374 616e 6365 2864 6174 615f  isinstance(data_
+000073e0: 6764 662c 2067 7064 2e47 656f 4461 7461  gdf, gpd.GeoData
+000073f0: 4672 616d 6529 0a20 2020 2023 2055 7365  Frame).    # Use
+00007400: 2066 6f72 6365 5f6d 756c 7469 7479 7065   force_multitype
+00007410: 2c20 746f 2065 7661 6465 2077 6172 6e69  , to evade warni
+00007420: 6e67 7320 7768 656e 2073 6f6d 6520 6261  ngs when some ba
+00007430: 7463 6865 7320 636f 6e74 6169 6e0a 2020  tches contain.  
+00007440: 2020 2320 7369 6e67 6c65 7479 7065 2061    # singletype a
+00007450: 6e64 2073 6f6d 6520 636f 6e74 6169 6e20  nd some contain 
+00007460: 6d75 6c74 6974 7970 6520 6765 6f6d 6574  multitype geomet
+00007470: 7269 6573 0a20 2020 2067 666f 2e74 6f5f  ries.    gfo.to_
+00007480: 6669 6c65 280a 2020 2020 2020 2020 6764  file(.        gd
+00007490: 663d 6461 7461 5f67 6466 2c0a 2020 2020  f=data_gdf,.    
+000074a0: 2020 2020 7061 7468 3d6f 7574 7075 745f      path=output_
+000074b0: 7061 7468 2c0a 2020 2020 2020 2020 6c61  path,.        la
+000074c0: 7965 723d 6f75 7470 7574 5f6c 6179 6572  yer=output_layer
+000074d0: 2c0a 2020 2020 2020 2020 696e 6465 783d  ,.        index=
+000074e0: 4661 6c73 652c 0a20 2020 2020 2020 2066  False,.        f
+000074f0: 6f72 6365 5f6f 7574 7075 745f 6765 6f6d  orce_output_geom
+00007500: 6574 7279 7479 7065 3d66 6f72 6365 5f6f  etrytype=force_o
+00007510: 7574 7075 745f 6765 6f6d 6574 7279 7479  utput_geometryty
+00007520: 7065 2c0a 2020 2020 2020 2020 666f 7263  pe,.        forc
+00007530: 655f 6d75 6c74 6974 7970 653d 5472 7565  e_multitype=True
+00007540: 2c0a 2020 2020 2020 2020 6372 6561 7465  ,.        create
+00007550: 5f73 7061 7469 616c 5f69 6e64 6578 3d46  _spatial_index=F
+00007560: 616c 7365 2c0a 2020 2020 290a 0a20 2020  alse,.    )..   
+00007570: 206d 6573 7361 6765 203d 2066 2254 6f6f   message = f"Too
+00007580: 6b20 7b64 6174 6574 696d 652e 6e6f 7728  k {datetime.now(
+00007590: 292d 7374 6172 745f 7469 6d65 7d20 666f  )-start_time} fo
+000075a0: 7220 7b6c 656e 2864 6174 615f 6764 6629  r {len(data_gdf)
+000075b0: 7d20 726f 7773 2028 7b72 6f77 737d 2921  } rows ({rows})!
+000075c0: 220a 2020 2020 7265 7475 726e 206d 6573  ".    return mes
+000075d0: 7361 6765 0a0a 0a64 6566 2064 6973 736f  sage...def disso
+000075e0: 6c76 6528 0a20 2020 2069 6e70 7574 5f70  lve(.    input_p
+000075f0: 6174 683a 2050 6174 682c 0a20 2020 206f  ath: Path,.    o
+00007600: 7574 7075 745f 7061 7468 3a20 5061 7468  utput_path: Path
+00007610: 2c0a 2020 2020 6772 6f75 7062 795f 636f  ,.    groupby_co
+00007620: 6c75 6d6e 733a 204f 7074 696f 6e61 6c5b  lumns: Optional[
+00007630: 4974 6572 6162 6c65 5b73 7472 5d5d 203d  Iterable[str]] =
+00007640: 204e 6f6e 652c 0a20 2020 2061 6767 5f63   None,.    agg_c
+00007650: 6f6c 756d 6e73 3a20 4f70 7469 6f6e 616c  olumns: Optional
+00007660: 5b64 6963 745d 203d 204e 6f6e 652c 0a20  [dict] = None,. 
+00007670: 2020 2065 7870 6c6f 6465 636f 6c6c 6563     explodecollec
+00007680: 7469 6f6e 733a 2062 6f6f 6c20 3d20 5472  tions: bool = Tr
+00007690: 7565 2c0a 2020 2020 7469 6c65 735f 7061  ue,.    tiles_pa
+000076a0: 7468 3a20 4f70 7469 6f6e 616c 5b50 6174  th: Optional[Pat
+000076b0: 685d 203d 204e 6f6e 652c 0a20 2020 206e  h] = None,.    n
+000076c0: 625f 7371 7561 7269 7368 5f74 696c 6573  b_squarish_tiles
+000076d0: 3a20 696e 7420 3d20 312c 0a20 2020 2069  : int = 1,.    i
+000076e0: 6e70 7574 5f6c 6179 6572 3a20 4f70 7469  nput_layer: Opti
+000076f0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00007700: 2c0a 2020 2020 6f75 7470 7574 5f6c 6179  ,.    output_lay
+00007710: 6572 3a20 4f70 7469 6f6e 616c 5b73 7472  er: Optional[str
+00007720: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 6772  ] = None,.    gr
+00007730: 6964 7369 7a65 3a20 666c 6f61 7420 3d20  idsize: float = 
+00007740: 302e 302c 0a20 2020 2077 6865 7265 3a20  0.0,.    where: 
+00007750: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00007760: 4e6f 6e65 2c0a 2020 2020 6e62 5f70 6172  None,.    nb_par
+00007770: 616c 6c65 6c3a 2069 6e74 203d 202d 312c  allel: int = -1,
+00007780: 0a20 2020 2062 6174 6368 7369 7a65 3a20  .    batchsize: 
+00007790: 696e 7420 3d20 2d31 2c0a 2020 2020 666f  int = -1,.    fo
+000077a0: 7263 653a 2062 6f6f 6c20 3d20 4661 6c73  rce: bool = Fals
+000077b0: 652c 0a29 202d 3e20 6469 6374 3a0a 2020  e,.) -> dict:.  
+000077c0: 2020 2222 220a 2020 2020 4675 6e63 7469    """.    Functi
+000077d0: 6f6e 2074 6861 7420 6170 706c 6965 7320  on that applies 
+000077e0: 6120 6469 7373 6f6c 7665 2e0a 0a20 2020  a dissolve...   
+000077f0: 204d 6f72 6520 6465 7461 696c 6564 2064   More detailed d
+00007800: 6f63 756d 656e 7461 7469 6f6e 2069 6e20  ocumentation in 
+00007810: 6d6f 6475 6c65 2067 656f 6f70 7321 0a0a  module geoops!..
+00007820: 2020 2020 5265 6d61 726b 3a20 6b65 6570      Remark: keep
+00007830: 5f65 6d70 7479 5f67 656f 6d73 2069 7320  _empty_geoms is 
+00007840: 6e6f 7420 696d 706c 656d 656e 7465 6420  not implemented 
+00007850: 6265 6361 7573 6520 7468 6973 2069 7320  because this is 
+00007860: 6e6f 7420 736f 2065 6173 7920 6265 6361  not so easy beca
+00007870: 7573 650a 2020 2020 2866 6f72 2070 6f6c  use.    (for pol
+00007880: 7967 6f6e 2064 6973 736f 6c76 6529 2074  ygon dissolve) t
+00007890: 6865 2062 6174 6368 6573 2061 7265 206c  he batches are l
+000078a0: 6f63 6174 696f 6e20 6261 7365 642c 2061  ocation based, a
+000078b0: 6e64 206e 756c 6c2f 656d 7074 7920 6765  nd null/empty ge
+000078c0: 6f6d 6574 7269 6573 0a20 2020 2064 6f6e  ometries.    don
+000078d0: 2774 2068 6176 6520 6120 6c6f 6361 7469  't have a locati
+000078e0: 6f6e 2e20 4974 2063 6f75 6c64 2062 6520  on. It could be 
+000078f0: 696d 706c 656d 656e 7465 642c 2062 7574  implemented, but
+00007900: 2061 7320 6c6f 6e67 2061 7320 6e6f 626f   as long as nobo
+00007910: 6479 206e 6565 6473 2069 742e 2e2e 0a20  dy needs it.... 
+00007920: 2020 2022 2222 0a0a 2020 2020 2320 496e     """..    # In
+00007930: 6974 2061 6e64 2076 616c 6964 6174 6520  it and validate 
+00007940: 696e 7075 7420 7061 7261 6d65 7465 7273  input parameters
+00007950: 0a20 2020 2023 202d 2d2d 2d2d 2d2d 2d2d  .    # ---------
+00007960: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00007970: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7374  ---------.    st
+00007980: 6172 745f 7469 6d65 203d 2064 6174 6574  art_time = datet
+00007990: 696d 652e 6e6f 7728 290a 2020 2020 6f70  ime.now().    op
+000079a0: 6572 6174 696f 6e20 3d20 2264 6973 736f  eration = "disso
+000079b0: 6c76 6522 0a20 2020 2072 6573 756c 745f  lve".    result_
+000079c0: 696e 666f 203d 207b 7d0a 0a20 2020 2023  info = {}..    #
+000079d0: 2043 6865 636b 2069 6e70 7574 2070 6172   Check input par
+000079e0: 616d 6574 6572 730a 2020 2020 6966 2067  ameters.    if g
+000079f0: 726f 7570 6279 5f63 6f6c 756d 6e73 2069  roupby_columns i
+00007a00: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206c  s not None and l
+00007a10: 656e 286c 6973 7428 6772 6f75 7062 795f  en(list(groupby_
+00007a20: 636f 6c75 6d6e 7329 2920 3d3d 2030 3a0a  columns)) == 0:.
+00007a30: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00007a40: 6c75 6545 7272 6f72 2822 6772 6f75 7062  lueError("groupb
+00007a50: 795f 636f 6c75 6d6e 733d 5b5d 2069 7320  y_columns=[] is 
+00007a60: 6e6f 7420 7375 7070 6f72 7465 642e 2055  not supported. U
+00007a70: 7365 204e 6f6e 652e 2229 0a20 2020 2069  se None.").    i
+00007a80: 6620 6e6f 7420 696e 7075 745f 7061 7468  f not input_path
+00007a90: 2e65 7869 7374 7328 293a 0a20 2020 2020  .exists():.     
+00007aa0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00007ab0: 726f 7228 6622 696e 7075 745f 7061 7468  ror(f"input_path
+00007ac0: 2064 6f65 736e 2774 2065 7869 7374 3a20   doesn't exist: 
+00007ad0: 7b69 6e70 7574 5f70 6174 687d 2229 0a20  {input_path}"). 
+00007ae0: 2020 2069 6620 696e 7075 745f 7061 7468     if input_path
+00007af0: 203d 3d20 6f75 7470 7574 5f70 6174 683a   == output_path:
+00007b00: 0a20 2020 2020 2020 2072 6169 7365 2056  .        raise V
+00007b10: 616c 7565 4572 726f 7228 226f 7574 7075  alueError("outpu
+00007b20: 745f 7061 7468 206d 7573 7420 6e6f 7420  t_path must not 
+00007b30: 6571 7561 6c20 696e 7075 745f 7061 7468  equal input_path
+00007b40: 2229 0a0a 2020 2020 696e 7075 745f 6c61  ")..    input_la
+00007b50: 7965 7269 6e66 6f20 3d20 6766 6f2e 6765  yerinfo = gfo.ge
+00007b60: 745f 6c61 7965 7269 6e66 6f28 696e 7075  t_layerinfo(inpu
+00007b70: 745f 7061 7468 2c20 696e 7075 745f 6c61  t_path, input_la
+00007b80: 7965 7229 0a20 2020 2069 6620 696e 7075  yer).    if inpu
+00007b90: 745f 6c61 7965 7269 6e66 6f2e 6765 6f6d  t_layerinfo.geom
+00007ba0: 6574 7279 7479 7065 2e74 6f5f 7072 696d  etrytype.to_prim
+00007bb0: 6974 6976 6574 7970 6520 696e 205b 0a20  itivetype in [. 
+00007bc0: 2020 2020 2020 2050 7269 6d69 7469 7665         Primitive
+00007bd0: 5479 7065 2e50 4f49 4e54 2c0a 2020 2020  Type.POINT,.    
+00007be0: 2020 2020 5072 696d 6974 6976 6554 7970      PrimitiveTyp
+00007bf0: 652e 4c49 4e45 5354 5249 4e47 2c0a 2020  e.LINESTRING,.  
+00007c00: 2020 5d3a 0a20 2020 2020 2020 2069 6620    ]:.        if 
+00007c10: 7469 6c65 735f 7061 7468 2069 7320 6e6f  tiles_path is no
+00007c20: 7420 4e6f 6e65 206f 7220 6e62 5f73 7175  t None or nb_squ
+00007c30: 6172 6973 685f 7469 6c65 7320 3e20 313a  arish_tiles > 1:
+00007c40: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00007c50: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+00007c60: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00007c70: 2244 6973 736f 6c76 6520 746f 2074 696c  "Dissolve to til
+00007c80: 6573 2069 7320 6e6f 7420 7375 7070 6f72  es is not suppor
+00007c90: 7465 6420 666f 7220 7b69 6e70 7574 5f6c  ted for {input_l
+00007ca0: 6179 6572 696e 666f 2e67 656f 6d65 7472  ayerinfo.geometr
+00007cb0: 7974 7970 657d 220a 2020 2020 2020 2020  ytype}".        
+00007cc0: 2020 2020 2020 2020 222c 2073 6f20 7469          ", so ti
+00007cd0: 6c65 735f 7061 7468 2073 686f 756c 6420  les_path should 
+00007ce0: 6265 204e 6f6e 6520 616e 6420 6e62 5f73  be None and nb_s
+00007cf0: 7175 6172 6973 685f 7469 6c65 7320 7368  quarish_tiles sh
+00007d00: 6f75 6c64 2062 6520 3129 220a 2020 2020  ould be 1)".    
+00007d10: 2020 2020 2020 2020 290a 0a20 2020 2069          )..    i
+00007d20: 6620 696e 7075 745f 6c61 7965 7220 6973  f input_layer is
+00007d30: 204e 6f6e 653a 0a20 2020 2020 2020 2069   None:.        i
+00007d40: 6e70 7574 5f6c 6179 6572 203d 2067 666f  nput_layer = gfo
+00007d50: 2e67 6574 5f6f 6e6c 795f 6c61 7965 7228  .get_only_layer(
+00007d60: 696e 7075 745f 7061 7468 290a 2020 2020  input_path).    
+00007d70: 6966 206f 7574 7075 745f 6c61 7965 7220  if output_layer 
+00007d80: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00007d90: 206f 7574 7075 745f 6c61 7965 7220 3d20   output_layer = 
+00007da0: 6766 6f2e 6765 745f 6465 6661 756c 745f  gfo.get_default_
+00007db0: 6c61 7965 7228 6f75 7470 7574 5f70 6174  layer(output_pat
+00007dc0: 6829 0a0a 2020 2020 2320 4368 6563 6b20  h)..    # Check 
+00007dd0: 636f 6c75 6d6e 7320 696e 2067 726f 7570  columns in group
+00007de0: 6279 5f63 6f6c 756d 6e73 0a20 2020 2069  by_columns.    i
+00007df0: 6620 6772 6f75 7062 795f 636f 6c75 6d6e  f groupby_column
+00007e00: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00007e10: 2020 2020 2020 2063 6f6c 756d 6e73 5f69         columns_i
+00007e20: 6e5f 6c61 7965 725f 7570 7065 7220 3d20  n_layer_upper = 
+00007e30: 5b0a 2020 2020 2020 2020 2020 2020 636f  [.            co
+00007e40: 6c75 6d6e 2e75 7070 6572 2829 2066 6f72  lumn.upper() for
+00007e50: 2063 6f6c 756d 6e20 696e 206c 6973 7428   column in list(
+00007e60: 696e 7075 745f 6c61 7965 7269 6e66 6f2e  input_layerinfo.
+00007e70: 636f 6c75 6d6e 7329 202b 205b 2266 6964  columns) + ["fid
+00007e80: 225d 0a20 2020 2020 2020 205d 0a20 2020  "].        ].   
+00007e90: 2020 2020 2066 6f72 2063 6f6c 756d 6e20       for column 
+00007ea0: 696e 2067 726f 7570 6279 5f63 6f6c 756d  in groupby_colum
+00007eb0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00007ec0: 6966 2063 6f6c 756d 6e2e 7570 7065 7228  if column.upper(
+00007ed0: 2920 6e6f 7420 696e 2063 6f6c 756d 6e73  ) not in columns
+00007ee0: 5f69 6e5f 6c61 7965 725f 7570 7065 723a  _in_layer_upper:
+00007ef0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007f00: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00007f10: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
+00007f20: 2020 2020 2020 2066 2263 6f6c 756d 6e20         f"column 
+00007f30: 696e 2067 726f 7570 6279 5f63 6f6c 756d  in groupby_colum
+00007f40: 6e73 206e 6f74 2061 7661 696c 6162 6c65  ns not available
+00007f50: 2069 6e20 6c61 7965 723a 207b 636f 6c75   in layer: {colu
+00007f60: 6d6e 7d22 0a20 2020 2020 2020 2020 2020  mn}".           
+00007f70: 2020 2020 2029 0a0a 2020 2020 2320 4368       )..    # Ch
+00007f80: 6563 6b20 6167 675f 636f 6c75 6d6e 7320  eck agg_columns 
+00007f90: 7061 7261 6d0a 2020 2020 6966 2061 6767  param.    if agg
+00007fa0: 5f63 6f6c 756d 6e73 2069 7320 6e6f 7420  _columns is not 
+00007fb0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2320  None:.        # 
+00007fc0: 5661 6c69 6461 7465 2074 6865 2064 6963  Validate the dic
+00007fd0: 7420 7374 7275 6374 7572 652c 2073 6f20  t structure, so 
+00007fe0: 7765 2063 616e 2061 7373 756d 6520 6576  we can assume ev
+00007ff0: 6572 7974 6869 6e67 2069 7320 4f4b 2066  erything is OK f
+00008000: 7572 7468 6572 206f 6e0a 2020 2020 2020  urther on.      
+00008010: 2020 5f70 6172 616d 6574 6572 5f68 656c    _parameter_hel
+00008020: 7065 722e 7661 6c69 6461 7465 5f61 6767  per.validate_agg
+00008030: 5f63 6f6c 756d 6e73 2861 6767 5f63 6f6c  _columns(agg_col
+00008040: 756d 6e73 290a 0a20 2020 2020 2020 2023  umns)..        #
+00008050: 2046 6972 7374 2074 616b 6520 6120 6465   First take a de
+00008060: 6570 2063 6f70 792c 2061 7320 7661 6c75  ep copy, as valu
+00008070: 6573 2063 616e 2062 6520 6368 616e 6765  es can be change
+00008080: 6420 6675 7274 6865 7220 6f6e 2074 6f20  d further on to 
+00008090: 7472 6561 7420 636f 6c75 6d6e 730a 2020  treat columns.  
+000080a0: 2020 2020 2020 2320 6361 7365 2069 6e73        # case ins
+000080b0: 656e 7369 7469 7665 0a20 2020 2020 2020  ensitive.       
+000080c0: 2061 6767 5f63 6f6c 756d 6e73 203d 206a   agg_columns = j
+000080d0: 736f 6e2e 6c6f 6164 7328 6a73 6f6e 2e64  son.loads(json.d
+000080e0: 756d 7073 2861 6767 5f63 6f6c 756d 6e73  umps(agg_columns
+000080f0: 2929 0a20 2020 2020 2020 2061 7373 6572  )).        asser
+00008100: 7420 6167 675f 636f 6c75 6d6e 7320 6973  t agg_columns is
+00008110: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
+00008120: 2020 6966 2022 6a73 6f6e 2220 696e 2061    if "json" in a
+00008130: 6767 5f63 6f6c 756d 6e73 3a0a 2020 2020  gg_columns:.    
+00008140: 2020 2020 2020 2020 6966 2061 6767 5f63          if agg_c
+00008150: 6f6c 756d 6e73 5b22 6a73 6f6e 225d 2069  olumns["json"] i
+00008160: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00008170: 2020 2020 2020 2020 6167 675f 636f 6c75          agg_colu
+00008180: 6d6e 735b 226a 736f 6e22 5d20 3d20 5b0a  mns["json"] = [.
+00008190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000081a0: 2020 2020 636f 6c20 666f 7220 636f 6c20      col for col 
+000081b0: 696e 2069 6e70 7574 5f6c 6179 6572 696e  in input_layerin
+000081c0: 666f 2e63 6f6c 756d 6e73 2069 6620 636f  fo.columns if co
+000081d0: 6c2e 7570 7065 7228 2920 213d 2022 494e  l.upper() != "IN
+000081e0: 4445 5822 0a20 2020 2020 2020 2020 2020  DEX".           
+000081f0: 2020 2020 205d 0a20 2020 2020 2020 2020       ].         
+00008200: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00008210: 2020 2020 2020 2020 2023 2041 6c69 676e           # Align
+00008220: 2063 6173 696e 6720 6f66 2063 6f6c 756d   casing of colum
+00008230: 6e20 6e61 6d65 7320 746f 2064 6174 610a  n names to data.
+00008240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008250: 6167 675f 636f 6c75 6d6e 735b 226a 736f  agg_columns["jso
+00008260: 6e22 5d20 3d20 5f67 656e 6572 616c 5f75  n"] = _general_u
+00008270: 7469 6c2e 616c 6967 6e5f 6361 7369 6e67  til.align_casing
+00008280: 5f6c 6973 7428 0a20 2020 2020 2020 2020  _list(.         
+00008290: 2020 2020 2020 2020 2020 2061 6767 5f63             agg_c
+000082a0: 6f6c 756d 6e73 5b22 6a73 6f6e 225d 2c20  olumns["json"], 
+000082b0: 6c69 7374 2869 6e70 7574 5f6c 6179 6572  list(input_layer
+000082c0: 696e 666f 2e63 6f6c 756d 6e73 2920 2b20  info.columns) + 
+000082d0: 5b22 6669 6422 5d0a 2020 2020 2020 2020  ["fid"].        
+000082e0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000082f0: 2020 656c 6966 2022 636f 6c75 6d6e 7322    elif "columns"
+00008300: 2069 6e20 6167 675f 636f 6c75 6d6e 733a   in agg_columns:
+00008310: 0a20 2020 2020 2020 2020 2020 2023 204c  .            # L
+00008320: 6f6f 7020 7468 726f 7567 6820 616c 6c20  oop through all 
+00008330: 726f 7773 0a20 2020 2020 2020 2020 2020  rows.           
+00008340: 2066 6f72 2061 6767 5f63 6f6c 756d 6e20   for agg_column 
+00008350: 696e 2061 6767 5f63 6f6c 756d 6e73 5b22  in agg_columns["
+00008360: 636f 6c75 6d6e 7322 5d3a 0a20 2020 2020  columns"]:.     
+00008370: 2020 2020 2020 2020 2020 2023 2043 6865             # Che
+00008380: 636b 2069 6620 636f 6c75 6d6e 2065 7869  ck if column exi
+00008390: 7374 7320 2b20 7365 7420 6361 7369 6e67  sts + set casing
+000083a0: 2073 616d 6520 6173 2069 6e20 6461 7461   same as in data
+000083b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000083c0: 2061 6767 5f63 6f6c 756d 6e5b 2263 6f6c   agg_column["col
+000083d0: 756d 6e22 5d20 3d20 5f67 656e 6572 616c  umn"] = _general
+000083e0: 5f75 7469 6c2e 616c 6967 6e5f 6361 7369  _util.align_casi
+000083f0: 6e67 280a 2020 2020 2020 2020 2020 2020  ng(.            
+00008400: 2020 2020 2020 2020 6167 675f 636f 6c75          agg_colu
+00008410: 6d6e 5b22 636f 6c75 6d6e 225d 2c20 6c69  mn["column"], li
+00008420: 7374 2869 6e70 7574 5f6c 6179 6572 696e  st(input_layerin
+00008430: 666f 2e63 6f6c 756d 6e73 2920 2b20 5b22  fo.columns) + ["
+00008440: 6669 6422 5d0a 2020 2020 2020 2020 2020  fid"].          
+00008450: 2020 2020 2020 290a 0a20 2020 2023 204e        )..    # N
+00008460: 6f77 2069 6e70 7574 2070 6172 616d 6574  ow input paramet
+00008470: 6572 7320 6172 6520 6368 6563 6b65 642c  ers are checked,
+00008480: 2063 6865 636b 2069 6620 7765 206e 6565   check if we nee
+00008490: 6420 746f 2063 616c 6375 6c61 7465 2061  d to calculate a
+000084a0: 6e79 7761 790a 2020 2020 6966 206f 7574  nyway.    if out
+000084b0: 7075 745f 7061 7468 2e65 7869 7374 7328  put_path.exists(
+000084c0: 293a 0a20 2020 2020 2020 2069 6620 666f  ):.        if fo
+000084d0: 7263 6520 6973 2046 616c 7365 3a0a 2020  rce is False:.  
+000084e0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000084f0: 5f69 6e66 6f5b 0a20 2020 2020 2020 2020  _info[.         
+00008500: 2020 2020 2020 2022 6d65 7373 6167 6522         "message"
+00008510: 0a20 2020 2020 2020 2020 2020 205d 203d  .            ] =
+00008520: 2066 226f 7574 7075 7420 6578 6973 7473   f"output exists
+00008530: 2061 6c72 6561 6479 207b 6f75 7470 7574   already {output
+00008540: 5f70 6174 687d 2061 6e64 2066 6f72 6365  _path} and force
+00008550: 2069 7320 6661 6c73 6522 0a20 2020 2020   is false".     
+00008560: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+00008570: 666f 2872 6573 756c 745f 696e 666f 5b22  fo(result_info["
+00008580: 6d65 7373 6167 6522 5d29 0a20 2020 2020  message"]).     
+00008590: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+000085a0: 7375 6c74 5f69 6e66 6f0a 2020 2020 2020  sult_info.      
+000085b0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000085c0: 2020 2020 6766 6f2e 7265 6d6f 7665 286f      gfo.remove(o
+000085d0: 7574 7075 745f 7061 7468 290a 0a20 2020  utput_path)..   
+000085e0: 2023 204e 6f77 2073 7461 7274 2064 6973   # Now start dis
+000085f0: 736f 6c76 696e 670a 2020 2020 2320 2d2d  solving.    # --
+00008600: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00008610: 2d2d 0a20 2020 2023 2045 6d70 7479 206f  --.    # Empty o
+00008620: 7220 4c69 6e65 2061 6e64 2070 6f69 6e74  r Line and point
+00008630: 206c 6179 6572 7320 6172 653a 0a20 2020   layers are:.   
+00008640: 2023 2020 202a 206e 6f74 2073 6f20 6c61   #   * not so la
+00008650: 7267 6520 286d 656d 6f72 792d 7769 7365  rge (memory-wise
+00008660: 290a 2020 2020 2320 2020 2a20 6172 656e  ).    #   * aren
+00008670: 2774 2063 6f6d 7075 7461 7469 6f6e 616c  't computational
+00008680: 6c79 2068 6561 7679 0a20 2020 2023 2041  ly heavy.    # A
+00008690: 6464 6974 696f 6e61 6c6c 7920 6c69 6e65  dditionally line
+000086a0: 206c 6179 6572 7320 6172 6520 6120 7061   layers are a pa
+000086b0: 696e 2074 6f20 6861 6e64 6c65 2063 6f72  in to handle cor
+000086c0: 7265 6374 6c79 2062 6563 6175 7365 206f  rectly because o
+000086d0: 660a 2020 2020 2320 726f 756e 6469 6e67  f.    # rounding
+000086e0: 2069 7373 7565 7320 6174 2074 6865 2062   issues at the b
+000086f0: 6f72 6465 7273 206f 6620 7469 6c65 732e  orders of tiles.
+00008700: 2e2e 2073 6f20 6a75 7374 2064 6973 736f  .. so just disso
+00008710: 6c76 6520 7468 656d 2069 6e20 6f6e 6520  lve them in one 
+00008720: 676f 2e0a 2020 2020 6966 2028 0a20 2020  go..    if (.   
+00008730: 2020 2020 2069 6e70 7574 5f6c 6179 6572       input_layer
+00008740: 696e 666f 2e66 6561 7475 7265 636f 756e  info.featurecoun
+00008750: 7420 3d3d 2030 0a20 2020 2020 2020 206f  t == 0.        o
+00008760: 7220 696e 7075 745f 6c61 7965 7269 6e66  r input_layerinf
+00008770: 6f2e 6765 6f6d 6574 7279 7479 7065 2e74  o.geometrytype.t
+00008780: 6f5f 7072 696d 6974 6976 6574 7970 650a  o_primitivetype.
+00008790: 2020 2020 2020 2020 696e 205b 0a20 2020          in [.   
+000087a0: 2020 2020 2020 2020 2050 7269 6d69 7469           Primiti
+000087b0: 7665 5479 7065 2e50 4f49 4e54 2c0a 2020  veType.POINT,.  
+000087c0: 2020 2020 2020 2020 2020 5072 696d 6974            Primit
+000087d0: 6976 6554 7970 652e 4c49 4e45 5354 5249  iveType.LINESTRI
+000087e0: 4e47 2c0a 2020 2020 2020 2020 5d0a 2020  NG,.        ].  
+000087f0: 2020 293a 0a20 2020 2020 2020 205f 6765    ):.        _ge
+00008800: 6f6f 7073 5f73 716c 2e64 6973 736f 6c76  oops_sql.dissolv
+00008810: 655f 7369 6e67 6c65 7468 7265 6164 280a  e_singlethread(.
+00008820: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
+00008830: 745f 7061 7468 3d69 6e70 7574 5f70 6174  t_path=input_pat
+00008840: 682c 0a20 2020 2020 2020 2020 2020 206f  h,.            o
+00008850: 7574 7075 745f 7061 7468 3d6f 7574 7075  utput_path=outpu
+00008860: 745f 7061 7468 2c0a 2020 2020 2020 2020  t_path,.        
+00008870: 2020 2020 6578 706c 6f64 6563 6f6c 6c65      explodecolle
+00008880: 6374 696f 6e73 3d65 7870 6c6f 6465 636f  ctions=explodeco
+00008890: 6c6c 6563 7469 6f6e 732c 0a20 2020 2020  llections,.     
+000088a0: 2020 2020 2020 2067 726f 7570 6279 5f63         groupby_c
+000088b0: 6f6c 756d 6e73 3d67 726f 7570 6279 5f63  olumns=groupby_c
+000088c0: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
+000088d0: 2020 2020 6167 675f 636f 6c75 6d6e 733d      agg_columns=
+000088e0: 6167 675f 636f 6c75 6d6e 732c 0a20 2020  agg_columns,.   
+000088f0: 2020 2020 2020 2020 2069 6e70 7574 5f6c           input_l
+00008900: 6179 6572 3d69 6e70 7574 5f6c 6179 6572  ayer=input_layer
+00008910: 2c0a 2020 2020 2020 2020 2020 2020 6f75  ,.            ou
+00008920: 7470 7574 5f6c 6179 6572 3d6f 7574 7075  tput_layer=outpu
+00008930: 745f 6c61 7965 722c 0a20 2020 2020 2020  t_layer,.       
+00008940: 2020 2020 2067 7269 6473 697a 653d 6772       gridsize=gr
+00008950: 6964 7369 7a65 2c0a 2020 2020 2020 2020  idsize,.        
+00008960: 2020 2020 6b65 6570 5f65 6d70 7479 5f67      keep_empty_g
+00008970: 656f 6d73 3d46 616c 7365 2c0a 2020 2020  eoms=False,.    
+00008980: 2020 2020 2020 2020 7768 6572 653d 7768          where=wh
+00008990: 6572 652c 0a20 2020 2020 2020 2020 2020  ere,.           
+000089a0: 2066 6f72 6365 3d66 6f72 6365 2c0a 2020   force=force,.  
+000089b0: 2020 2020 2020 290a 0a20 2020 2065 6c69        )..    eli
+000089c0: 6620 696e 7075 745f 6c61 7965 7269 6e66  f input_layerinf
+000089d0: 6f2e 6765 6f6d 6574 7279 7479 7065 2e74  o.geometrytype.t
+000089e0: 6f5f 7072 696d 6974 6976 6574 7970 6520  o_primitivetype 
+000089f0: 6973 2050 7269 6d69 7469 7665 5479 7065  is PrimitiveType
+00008a00: 2e50 4f4c 5947 4f4e 3a0a 2020 2020 2020  .POLYGON:.      
+00008a10: 2020 2320 5072 6570 6172 6520 7768 6572    # Prepare wher
+00008a20: 650a 2020 2020 2020 2020 6966 2077 6865  e.        if whe
+00008a30: 7265 2069 7320 6e6f 7420 4e6f 6e65 3a0a  re is not None:.
+00008a40: 2020 2020 2020 2020 2020 2020 6966 2077              if w
+00008a50: 6865 7265 203d 3d20 2222 3a0a 2020 2020  here == "":.    
+00008a60: 2020 2020 2020 2020 2020 2020 7768 6572              wher
+00008a70: 6520 3d20 4e6f 6e65 0a20 2020 2020 2020  e = None.       
+00008a80: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00008a90: 2020 2020 2020 2020 2020 2023 2053 6574             # Set
+00008aa0: 2067 656f 6d65 7472 7963 6f6c 756d 6e20   geometrycolumn 
+00008ab0: 746f 2022 6765 6f6d 222c 2062 6563 6175  to "geom", becau
+00008ac0: 7365 2074 656d 7020 6669 6c65 7320 6172  se temp files ar
+00008ad0: 6520 7361 7665 6420 6173 2067 706b 672e  e saved as gpkg.
+00008ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008af0: 2077 6865 7265 203d 2077 6865 7265 2e66   where = where.f
+00008b00: 6f72 6d61 7428 6765 6f6d 6574 7279 636f  ormat(geometryco
+00008b10: 6c75 6d6e 3d22 6765 6f6d 2229 0a0a 2020  lumn="geom")..  
+00008b20: 2020 2020 2020 2320 4966 2061 2074 696c        # If a til
+00008b30: 6573 5f70 6174 6820 6973 2073 7065 6369  es_path is speci
+00008b40: 6669 6564 2c20 7265 6164 2074 686f 7365  fied, read those
+00008b50: 2074 696c 6573 2e2e 2e0a 2020 2020 2020   tiles....      
+00008b60: 2020 7265 7375 6c74 5f74 696c 6573 5f67    result_tiles_g
+00008b70: 6466 203d 204e 6f6e 650a 2020 2020 2020  df = None.      
+00008b80: 2020 6966 2074 696c 6573 5f70 6174 6820    if tiles_path 
+00008b90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00008ba0: 2020 2020 2020 2020 2072 6573 756c 745f           result_
+00008bb0: 7469 6c65 735f 6764 6620 3d20 6766 6f2e  tiles_gdf = gfo.
+00008bc0: 7265 6164 5f66 696c 6528 7469 6c65 735f  read_file(tiles_
+00008bd0: 7061 7468 290a 2020 2020 2020 2020 2020  path).          
+00008be0: 2020 6966 206e 625f 7061 7261 6c6c 656c    if nb_parallel
+00008bf0: 203d 3d20 2d31 3a0a 2020 2020 2020 2020   == -1:.        
+00008c00: 2020 2020 2020 2020 6e62 5f63 7075 203d          nb_cpu =
+00008c10: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
+00008c20: 2e63 7075 5f63 6f75 6e74 2829 0a20 2020  .cpu_count().   
+00008c30: 2020 2020 2020 2020 2020 2020 206e 625f               nb_
+00008c40: 7061 7261 6c6c 656c 203d 206e 625f 6370  parallel = nb_cp
+00008c50: 7520 2023 2069 6e74 2831 2e32 3520 2a20  u  # int(1.25 * 
+00008c60: 6e62 5f63 7075 290a 2020 2020 2020 2020  nb_cpu).        
+00008c70: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00008c80: 6562 7567 2866 224e 6220 6370 7573 2066  ebug(f"Nb cpus f
+00008c90: 6f75 6e64 3a20 7b6e 625f 6370 757d 2c20  ound: {nb_cpu}, 
+00008ca0: 6e62 5f70 6172 616c 6c65 6c3a 207b 6e62  nb_parallel: {nb
+00008cb0: 5f70 6172 616c 6c65 6c7d 2229 0a20 2020  _parallel}").   
+00008cc0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00008cd0: 2020 2020 2020 2023 2045 6c73 652c 2063         # Else, c
+00008ce0: 7265 6174 6520 6120 6772 6964 2062 6173  reate a grid bas
+00008cf0: 6564 206f 6e20 7468 6520 6e75 6d62 6572  ed on the number
+00008d00: 206f 6620 7469 6c65 7320 7761 6e74 6564   of tiles wanted
+00008d10: 2061 7320 7265 7375 6c74 0a20 2020 2020   as result.     
+00008d20: 2020 2020 2020 2023 2055 7365 2061 206d         # Use a m
+00008d30: 6172 6769 6e20 6f66 2031 206d 6574 6572  argin of 1 meter
+00008d40: 2061 726f 756e 6420 7468 6520 626f 756e   around the boun
+00008d50: 6473 0a20 2020 2020 2020 2020 2020 206d  ds.            m
+00008d60: 6172 6769 6e20 3d20 312e 300a 2020 2020  argin = 1.0.    
+00008d70: 2020 2020 2020 2020 6966 2069 6e70 7574          if input
+00008d80: 5f6c 6179 6572 696e 666f 2e63 7273 2069  _layerinfo.crs i
+00008d90: 7320 6e6f 7420 4e6f 6e65 2061 6e64 206e  s not None and n
+00008da0: 6f74 2069 6e70 7574 5f6c 6179 6572 696e  ot input_layerin
+00008db0: 666f 2e63 7273 2e69 735f 7072 6f6a 6563  fo.crs.is_projec
+00008dc0: 7465 643a 0a20 2020 2020 2020 2020 2020  ted:.           
+00008dd0: 2020 2020 2023 2049 6620 6765 6f67 7261       # If geogra
+00008de0: 7068 6963 2063 7273 2c20 3120 6465 6772  phic crs, 1 degr
+00008df0: 6565 203d 2031 3131 206b 6d20 6f72 2031  ee = 111 km or 1
+00008e00: 3131 3030 3020 6d0a 2020 2020 2020 2020  11000 m.        
+00008e10: 2020 2020 2020 2020 6d61 7267 696e 202f          margin /
+00008e20: 3d20 3131 3130 3030 0a20 2020 2020 2020  = 111000.       
+00008e30: 2020 2020 2062 6f75 6e64 7320 3d20 696e       bounds = in
+00008e40: 7075 745f 6c61 7965 7269 6e66 6f2e 746f  put_layerinfo.to
+00008e50: 7461 6c5f 626f 756e 6473 0a20 2020 2020  tal_bounds.     
+00008e60: 2020 2020 2020 2062 6f75 6e64 7320 3d20         bounds = 
+00008e70: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00008e80: 2020 626f 756e 6473 5b30 5d20 2d20 6d61    bounds[0] - ma
+00008e90: 7267 696e 2c0a 2020 2020 2020 2020 2020  rgin,.          
+00008ea0: 2020 2020 2020 626f 756e 6473 5b31 5d20        bounds[1] 
+00008eb0: 2d20 6d61 7267 696e 2c0a 2020 2020 2020  - margin,.      
+00008ec0: 2020 2020 2020 2020 2020 626f 756e 6473            bounds
+00008ed0: 5b32 5d20 2b20 6d61 7267 696e 2c0a 2020  [2] + margin,.  
+00008ee0: 2020 2020 2020 2020 2020 2020 2020 626f                bo
+00008ef0: 756e 6473 5b33 5d20 2b20 6d61 7267 696e  unds[3] + margin
+00008f00: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
+00008f10: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00008f20: 6c74 5f74 696c 6573 5f67 6466 203d 2067  lt_tiles_gdf = g
+00008f30: 7269 645f 7574 696c 2e63 7265 6174 655f  rid_util.create_
+00008f40: 6772 6964 3228 0a20 2020 2020 2020 2020  grid2(.         
+00008f50: 2020 2020 2020 2062 6f75 6e64 732c 206e         bounds, n
+00008f60: 625f 7371 7561 7269 7368 5f74 696c 6573  b_squarish_tiles
+00008f70: 2c20 696e 7075 745f 6c61 7965 7269 6e66  , input_layerinf
+00008f80: 6f2e 6372 730a 2020 2020 2020 2020 2020  o.crs.          
+00008f90: 2020 290a 0a20 2020 2020 2020 2023 2041    )..        # A
+00008fa0: 7070 6c79 2067 7269 6473 697a 6520 746f  pply gridsize to
+00008fb0: 6c65 7261 6e63 6520 6f6e 2074 696c 6573  lerance on tiles
+00008fc0: 2c20 6f74 6865 7277 6973 6520 7468 6520  , otherwise the 
+00008fd0: 626f 7264 6572 2070 6f6c 7967 6f6e 7320  border polygons 
+00008fe0: 6361 6e27 7420 6265 0a20 2020 2020 2020  can't be.       
+00008ff0: 2023 2075 6e69 6f6e 6564 2070 726f 7065   # unioned prope
+00009000: 726c 7920 6265 6361 7573 6520 6761 7073  rly because gaps
+00009010: 2061 7070 6561 7220 6166 7465 7220 726f   appear after ro
+00009020: 756e 6469 6e67 2063 6f6f 7264 696e 6174  unding coordinat
+00009030: 6573 2e0a 2020 2020 2020 2020 6966 2067  es..        if g
+00009040: 7269 6473 697a 6520 213d 2030 2e30 3a0a  ridsize != 0.0:.
+00009050: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00009060: 6c74 5f74 696c 6573 5f67 6466 2e67 656f  lt_tiles_gdf.geo
+00009070: 6d65 7472 7920 3d20 7368 6170 656c 7932  metry = shapely2
+00009080: 5f6f 725f 7079 6765 6f73 2e73 6574 5f70  _or_pygeos.set_p
+00009090: 7265 6369 7369 6f6e 280a 2020 2020 2020  recision(.      
+000090a0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000090b0: 5f74 696c 6573 5f67 6466 2e67 656f 6d65  _tiles_gdf.geome
+000090c0: 7472 792c 2067 7269 645f 7369 7a65 3d67  try, grid_size=g
+000090d0: 7269 6473 697a 650a 2020 2020 2020 2020  ridsize.        
+000090e0: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
+000090f0: 206c 656e 2872 6573 756c 745f 7469 6c65   len(result_tile
+00009100: 735f 6764 6629 203e 2031 3a0a 2020 2020  s_gdf) > 1:.    
+00009110: 2020 2020 2020 2020 6766 6f2e 746f 5f66          gfo.to_f
+00009120: 696c 6528 0a20 2020 2020 2020 2020 2020  ile(.           
+00009130: 2020 2020 2072 6573 756c 745f 7469 6c65       result_tile
+00009140: 735f 6764 662c 0a20 2020 2020 2020 2020  s_gdf,.         
+00009150: 2020 2020 2020 206f 7574 7075 745f 7061         output_pa
+00009160: 7468 2e70 6172 656e 7420 2f20 6622 7b6f  th.parent / f"{o
+00009170: 7574 7075 745f 7061 7468 2e73 7465 6d7d  utput_path.stem}
+00009180: 5f74 696c 6573 2e67 706b 6722 2c0a 2020  _tiles.gpkg",.  
+00009190: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000091a0: 2020 2020 2023 2049 6620 6120 7469 6c65       # If a tile
+000091b0: 6420 7265 7375 6c74 2069 7320 6173 6b65  d result is aske
+000091c0: 642c 2061 6464 2074 696c 655f 6964 2074  d, add tile_id t
+000091d0: 6f20 6772 6f75 7020 6f6e 2066 6f72 2074  o group on for t
+000091e0: 6865 2072 6573 756c 740a 2020 2020 2020  he result.      
+000091f0: 2020 6966 206c 656e 2872 6573 756c 745f    if len(result_
+00009200: 7469 6c65 735f 6764 6629 203e 2031 3a0a  tiles_gdf) > 1:.
+00009210: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+00009220: 6c74 5f74 696c 6573 5f67 6466 5b22 7469  lt_tiles_gdf["ti
+00009230: 6c65 5f69 6422 5d20 3d20 7265 7375 6c74  le_id"] = result
+00009240: 5f74 696c 6573 5f67 6466 2e72 6573 6574  _tiles_gdf.reset
+00009250: 5f69 6e64 6578 2829 2e69 6e64 6578 0a0a  _index().index..
+00009260: 2020 2020 2020 2020 2320 5468 6520 6469          # The di
+00009270: 7373 6f6c 7665 2066 6f72 2070 6f6c 7967  ssolve for polyg
+00009280: 6f6e 7320 6973 2064 6f6e 6520 696e 2073  ons is done in s
+00009290: 6576 6572 616c 2070 6173 7365 732c 2061  everal passes, a
+000092a0: 6e64 2061 6674 6572 2074 6865 2066 6972  nd after the fir
+000092b0: 7374 0a20 2020 2020 2020 2023 2070 6173  st.        # pas
+000092c0: 732c 206f 6e6c 7920 7468 6520 276f 6e62  s, only the 'onb
+000092d0: 6f72 6465 7227 2066 6561 7475 7265 7320  order' features 
+000092e0: 6172 6520 6675 7274 6865 7220 6469 7373  are further diss
+000092f0: 6f6c 7665 642c 2061 7320 7468 650a 2020  olved, as the.  
+00009300: 2020 2020 2020 2320 276e 6f74 6f6e 626f        # 'notonbo
+00009310: 7264 6572 2720 6665 6174 7572 6573 2061  rder' features a
+00009320: 7265 2061 6c72 6561 6479 204f 4b2e 0a20  re already OK.. 
+00009330: 2020 2020 2020 2074 656d 7064 6972 203d         tempdir =
+00009340: 205f 696f 5f75 7469 6c2e 6372 6561 7465   _io_util.create
+00009350: 5f74 656d 7064 6972 2866 2267 656f 6669  _tempdir(f"geofi
+00009360: 6c65 6f70 732f 7b6f 7065 7261 7469 6f6e  leops/{operation
+00009370: 7d22 290a 2020 2020 2020 2020 7472 793a  }").        try:
+00009380: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00009390: 6f75 7470 7574 5f6c 6179 6572 2069 7320  output_layer is 
+000093a0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000093b0: 2020 2020 2020 6f75 7470 7574 5f6c 6179        output_lay
+000093c0: 6572 203d 2067 666f 2e67 6574 5f64 6566  er = gfo.get_def
+000093d0: 6175 6c74 5f6c 6179 6572 286f 7574 7075  ault_layer(outpu
+000093e0: 745f 7061 7468 290a 2020 2020 2020 2020  t_path).        
+000093f0: 2020 2020 6f75 7470 7574 5f74 6d70 5f70      output_tmp_p
+00009400: 6174 6820 3d20 7465 6d70 6469 7220 2f20  ath = tempdir / 
+00009410: 226f 7574 7075 745f 746d 702e 6770 6b67  "output_tmp.gpkg
+00009420: 220a 2020 2020 2020 2020 2020 2020 7072  ".            pr
+00009430: 6576 5f6e 625f 6261 7463 6865 7320 3d20  ev_nb_batches = 
+00009440: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
+00009450: 206c 6173 745f 7061 7373 203d 2046 616c   last_pass = Fal
+00009460: 7365 0a20 2020 2020 2020 2020 2020 2070  se.            p
+00009470: 6173 735f 6964 203d 2030 0a20 2020 2020  ass_id = 0.     
+00009480: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+00009490: 666f 2866 2253 7461 7274 2064 6973 736f  fo(f"Start disso
+000094a0: 6c76 6520 6f6e 2066 696c 6520 7b69 6e70  lve on file {inp
+000094b0: 7574 5f70 6174 687d 2229 0a20 2020 2020  ut_path}").     
+000094c0: 2020 2020 2020 2069 6e70 7574 5f70 6173         input_pas
+000094d0: 735f 6c61 7965 7220 3d20 696e 7075 745f  s_layer = input_
+000094e0: 6c61 7965 720a 2020 2020 2020 2020 2020  layer.          
+000094f0: 2020 7768 696c 6520 5472 7565 3a0a 2020    while True:.  
+00009500: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00009510: 4765 7420 696e 666f 206f 6620 7468 6520  Get info of the 
+00009520: 6375 7272 656e 7420 6669 6c65 2074 6861  current file tha
+00009530: 7420 6e65 6564 7320 746f 2062 6520 6469  t needs to be di
+00009540: 7373 6f6c 7665 640a 2020 2020 2020 2020  ssolved.        
+00009550: 2020 2020 2020 2020 696e 7075 745f 7061          input_pa
+00009560: 7373 5f6c 6179 6572 696e 666f 203d 2067  ss_layerinfo = g
+00009570: 666f 2e67 6574 5f6c 6179 6572 696e 666f  fo.get_layerinfo
+00009580: 2869 6e70 7574 5f70 6174 682c 2069 6e70  (input_path, inp
+00009590: 7574 5f70 6173 735f 6c61 7965 7229 0a20  ut_pass_layer). 
+000095a0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+000095b0: 625f 726f 7773 5f74 6f74 616c 203d 2069  b_rows_total = i
+000095c0: 6e70 7574 5f70 6173 735f 6c61 7965 7269  nput_pass_layeri
+000095d0: 6e66 6f2e 6665 6174 7572 6563 6f75 6e74  nfo.featurecount
+000095e0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000095f0: 2020 2320 4361 6c63 756c 6174 6520 7468    # Calculate th
+00009600: 6520 6265 7374 206e 756d 6265 7220 6f66  e best number of
+00009610: 2070 6172 616c 6c65 6c20 7072 6f63 6573   parallel proces
+00009620: 7365 7320 616e 6420 6261 7463 6865 7320  ses and batches 
+00009630: 666f 720a 2020 2020 2020 2020 2020 2020  for.            
+00009640: 2020 2020 2320 7468 6520 6176 6169 6c61      # the availa
+00009650: 626c 6520 7265 736f 7572 6365 7320 666f  ble resources fo
+00009660: 7220 7468 6520 6375 7272 656e 7420 7061  r the current pa
+00009670: 7373 0a20 2020 2020 2020 2020 2020 2020  ss.             
+00009680: 2020 2069 6620 6261 7463 6873 697a 6520     if batchsize 
+00009690: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
+000096a0: 2020 2020 2020 2020 2070 6172 616c 6c65           paralle
+000096b0: 6c69 7a61 7469 6f6e 5f63 6f6e 6669 6720  lization_config 
+000096c0: 3d20 5061 7261 6c6c 656c 697a 6174 696f  = Parallelizatio
+000096d0: 6e43 6f6e 6669 6728 0a20 2020 2020 2020  nConfig(.       
+000096e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000096f0: 206d 696e 5f61 7667 5f72 6f77 735f 7065   min_avg_rows_pe
+00009700: 725f 6261 7463 683d 696e 7428 6d61 7468  r_batch=int(math
+00009710: 2e63 6569 6c28 6261 7463 6873 697a 6520  .ceil(batchsize 
+00009720: 2f20 3229 292c 0a20 2020 2020 2020 2020  / 2)),.         
+00009730: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00009740: 6178 5f61 7667 5f72 6f77 735f 7065 725f  ax_avg_rows_per_
+00009750: 6261 7463 683d 6261 7463 6873 697a 652c  batch=batchsize,
+00009760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009770: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00009780: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00009790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000097a0: 2070 6172 616c 6c65 6c69 7a61 7469 6f6e   parallelization
+000097b0: 5f63 6f6e 6669 6720 3d20 5061 7261 6c6c  _config = Parall
+000097c0: 656c 697a 6174 696f 6e43 6f6e 6669 6728  elizationConfig(
+000097d0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+000097e0: 2020 6e62 5f70 6172 616c 6c65 6c2c 206e    nb_parallel, n
+000097f0: 625f 6261 7463 6865 735f 7265 636f 6d6d  b_batches_recomm
+00009800: 656e 6465 642c 205f 203d 2067 6574 5f70  ended, _ = get_p
+00009810: 6172 616c 6c65 6c69 7a61 7469 6f6e 5f70  arallelization_p
+00009820: 6172 616d 7328 0a20 2020 2020 2020 2020  arams(.         
+00009830: 2020 2020 2020 2020 2020 206e 625f 726f             nb_ro
+00009840: 7773 5f74 6f74 616c 3d6e 625f 726f 7773  ws_total=nb_rows
+00009850: 5f74 6f74 616c 2c0a 2020 2020 2020 2020  _total,.        
+00009860: 2020 2020 2020 2020 2020 2020 6e62 5f70              nb_p
+00009870: 6172 616c 6c65 6c3d 6e62 5f70 6172 616c  arallel=nb_paral
+00009880: 6c65 6c2c 0a20 2020 2020 2020 2020 2020  lel,.           
+00009890: 2020 2020 2020 2020 206e 625f 6261 7463           nb_batc
+000098a0: 6865 735f 7072 6576 696f 7573 5f70 6173  hes_previous_pas
+000098b0: 733d 7072 6576 5f6e 625f 6261 7463 6865  s=prev_nb_batche
+000098c0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+000098d0: 2020 2020 2020 2070 6172 616c 6c65 6c69         paralleli
+000098e0: 7a61 7469 6f6e 5f63 6f6e 6669 673d 7061  zation_config=pa
+000098f0: 7261 6c6c 656c 697a 6174 696f 6e5f 636f  rallelization_co
+00009900: 6e66 6967 2c0a 2020 2020 2020 2020 2020  nfig,.          
+00009910: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00009920: 2020 2020 2020 2020 2023 2049 6620 7468           # If th
+00009930: 6520 6964 6561 6c20 6e75 6d62 6572 206f  e ideal number o
+00009940: 6620 6261 7463 6865 7320 6973 2063 6c6f  f batches is clo
+00009950: 7365 2074 6f20 7468 6520 6e62 2e20 7265  se to the nb. re
+00009960: 7375 6c74 2074 696c 6573 2061 736b 6564  sult tiles asked
+00009970: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00009980: 2020 2320 6469 7373 6f6c 7665 2074 6f77    # dissolve tow
+00009990: 6172 6473 2074 6865 2061 736b 6564 2072  ards the asked r
+000099a0: 6573 756c 7421 0a20 2020 2020 2020 2020  esult!.         
+000099b0: 2020 2020 2020 2023 2049 6620 6e6f 742c         # If not,
+000099c0: 2061 2074 656d 706f 7261 7279 2072 6573   a temporary res
+000099d0: 756c 7420 6973 2063 7265 6174 6564 2075  ult is created u
+000099e0: 7369 6e67 2073 6d61 6c6c 6572 2074 696c  sing smaller til
+000099f0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00009a00: 2020 2069 6620 6e62 5f62 6174 6368 6573     if nb_batches
+00009a10: 5f72 6563 6f6d 6d65 6e64 6564 203c 3d20  _recommended <= 
+00009a20: 6c65 6e28 7265 7375 6c74 5f74 696c 6573  len(result_tiles
+00009a30: 5f67 6466 2920 2a20 312e 313a 0a20 2020  _gdf) * 1.1:.   
+00009a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a50: 2074 696c 6573 5f67 6466 203d 2072 6573   tiles_gdf = res
+00009a60: 756c 745f 7469 6c65 735f 6764 660a 2020  ult_tiles_gdf.  
+00009a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009a80: 2020 6c61 7374 5f70 6173 7320 3d20 5472    last_pass = Tr
+00009a90: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
+00009aa0: 2020 2020 2020 206e 625f 7061 7261 6c6c         nb_parall
+00009ab0: 656c 203d 206d 696e 286c 656e 2872 6573  el = min(len(res
+00009ac0: 756c 745f 7469 6c65 735f 6764 6629 2c20  ult_tiles_gdf), 
+00009ad0: 6e62 5f70 6172 616c 6c65 6c29 0a20 2020  nb_parallel).   
+00009ae0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00009af0: 6620 6c65 6e28 7265 7375 6c74 5f74 696c  f len(result_til
+00009b00: 6573 5f67 6466 2920 3d3d 2031 3a0a 2020  es_gdf) == 1:.  
+00009b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009b20: 2020 2320 4372 6561 7465 2061 2067 7269    # Create a gri
+00009b30: 6420 6261 7365 6420 6f6e 2074 6865 2069  d based on the i
+00009b40: 6465 616c 206e 756d 6265 7220 6f66 2062  deal number of b
+00009b50: 6174 6368 6573 2c20 6275 7420 6d61 6b65  atches, but make
+00009b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009b70: 2020 2020 2023 2073 7572 6520 7468 6520       # sure the 
+00009b80: 6e75 6d62 6572 2069 7320 736d 616c 6c65  number is smalle
+00009b90: 7220 7468 616e 2074 6865 206d 6178 696d  r than the maxim
+00009ba0: 756d 2e2e 2e0a 2020 2020 2020 2020 2020  um....          
+00009bb0: 2020 2020 2020 2020 2020 6e62 5f73 7175            nb_squ
+00009bc0: 6172 6973 685f 7469 6c65 735f 6d61 7820  arish_tiles_max 
+00009bd0: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+00009be0: 2020 2020 2020 2020 2020 2069 6620 7072             if pr
+00009bf0: 6576 5f6e 625f 6261 7463 6865 7320 6973  ev_nb_batches is
+00009c00: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00009c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c20: 2020 206e 625f 7371 7561 7269 7368 5f74     nb_squarish_t
+00009c30: 696c 6573 5f6d 6178 203d 206d 6178 2870  iles_max = max(p
+00009c40: 7265 765f 6e62 5f62 6174 6368 6573 202d  rev_nb_batches -
+00009c50: 2031 2c20 3129 0a20 2020 2020 2020 2020   1, 1).         
+00009c60: 2020 2020 2020 2020 2020 2074 696c 6573             tiles
+00009c70: 5f67 6466 203d 2067 7269 645f 7574 696c  _gdf = grid_util
+00009c80: 2e63 7265 6174 655f 6772 6964 3228 0a20  .create_grid2(. 
+00009c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ca0: 2020 2020 2020 2074 6f74 616c 5f62 6f75         total_bou
+00009cb0: 6e64 733d 696e 7075 745f 7061 7373 5f6c  nds=input_pass_l
+00009cc0: 6179 6572 696e 666f 2e74 6f74 616c 5f62  ayerinfo.total_b
+00009cd0: 6f75 6e64 732c 0a20 2020 2020 2020 2020  ounds,.         
+00009ce0: 2020 2020 2020 2020 2020 2020 2020 206e                 n
+00009cf0: 625f 7371 7561 7269 7368 5f74 696c 6573  b_squarish_tiles
+00009d00: 3d6e 625f 6261 7463 6865 735f 7265 636f  =nb_batches_reco
+00009d10: 6d6d 656e 6465 642c 0a20 2020 2020 2020  mmended,.       
+00009d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d30: 206e 625f 7371 7561 7269 7368 5f74 696c   nb_squarish_til
+00009d40: 6573 5f6d 6178 3d6e 625f 7371 7561 7269  es_max=nb_squari
+00009d50: 7368 5f74 696c 6573 5f6d 6178 2c0a 2020  sh_tiles_max,.  
+00009d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009d70: 2020 2020 2020 6372 733d 696e 7075 745f        crs=input_
+00009d80: 7061 7373 5f6c 6179 6572 696e 666f 2e63  pass_layerinfo.c
+00009d90: 7273 2c0a 2020 2020 2020 2020 2020 2020  rs,.            
+00009da0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+00009db0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
 00009dc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dd0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00009de0: 2020 2020 2020 2020 2020 2320 4966 2061            # If a
-00009df0: 2067 7269 6420 6973 2073 7065 6369 6669   grid is specifi
-00009e00: 6564 2061 6c72 6561 6479 2c20 6164 6420  ed already, add 
-00009e10: 6578 7472 6120 636f 6c75 6d6e 732f 726f  extra columns/ro
-00009e20: 7773 2069 6e73 7465 6164 206f 660a 2020  ws instead of.  
-00009e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009e40: 2020 2320 6372 6561 7469 6e67 206e 6577    # creating new
-00009e50: 206f 6e65 2e2e 2e0a 2020 2020 2020 2020   one....        
-00009e60: 2020 2020 2020 2020 2020 2020 7469 6c65              tile
-00009e70: 735f 6764 6620 3d20 6772 6964 5f75 7469  s_gdf = grid_uti
-00009e80: 6c2e 7370 6c69 745f 7469 6c65 7328 0a20  l.split_tiles(. 
-00009e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ea0: 2020 2020 2020 2072 6573 756c 745f 7469         result_ti
-00009eb0: 6c65 735f 6764 662c 206e 625f 6261 7463  les_gdf, nb_batc
-00009ec0: 6865 735f 7265 636f 6d6d 656e 6465 640a  hes_recommended.
-00009ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009ee0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-00009ef0: 2020 2020 2020 2023 2041 7070 6c79 2067         # Apply g
-00009f00: 7269 6473 697a 6520 746f 6c65 7261 6e63  ridsize toleranc
-00009f10: 6520 6f6e 2074 696c 6573 2c20 6f74 6865  e on tiles, othe
-00009f20: 7277 6973 6520 7468 6520 626f 7264 6572  rwise the border
-00009f30: 2070 6f6c 7967 6f6e 7320 6361 6e27 740a   polygons can't.
-00009f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f50: 2320 6265 2075 6e69 6f6e 6564 2070 726f  # be unioned pro
-00009f60: 7065 726c 7920 6265 6361 7573 6520 6761  perly because ga
-00009f70: 7073 2061 7070 6561 7220 6166 7465 7220  ps appear after 
-00009f80: 726f 756e 6469 6e67 2063 6f6f 7264 696e  rounding coordin
-00009f90: 6174 6573 2e0a 2020 2020 2020 2020 2020  ates..          
-00009fa0: 2020 2020 2020 6966 2067 7269 6473 697a        if gridsiz
-00009fb0: 6520 213d 2030 2e30 3a0a 2020 2020 2020  e != 0.0:.      
-00009fc0: 2020 2020 2020 2020 2020 2020 2020 7469                ti
-00009fd0: 6c65 735f 6764 662e 6765 6f6d 6574 7279  les_gdf.geometry
-00009fe0: 203d 2073 6861 7065 6c79 325f 6f72 5f70   = shapely2_or_p
-00009ff0: 7967 656f 732e 7365 745f 7072 6563 6973  ygeos.set_precis
-0000a000: 696f 6e28 0a20 2020 2020 2020 2020 2020  ion(.           
-0000a010: 2020 2020 2020 2020 2020 2020 2074 696c               til
-0000a020: 6573 5f67 6466 2e67 656f 6d65 7472 792e  es_gdf.geometry.
-0000a030: 6172 7261 792e 6461 7461 2c20 6772 6964  array.data, grid
-0000a040: 5f73 697a 653d 6772 6964 7369 7a65 0a20  _size=gridsize. 
-0000a050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a060: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000a070: 2020 2020 2067 666f 2e74 6f5f 6669 6c65       gfo.to_file
-0000a080: 2874 696c 6573 5f67 6466 2c20 7465 6d70  (tiles_gdf, temp
-0000a090: 6469 7220 2f20 6622 6f75 7470 7574 5f7b  dir / f"output_{
-0000a0a0: 7061 7373 5f69 647d 5f74 696c 6573 2e67  pass_id}_tiles.g
-0000a0b0: 706b 6722 290a 0a20 2020 2020 2020 2020  pkg")..         
-0000a0c0: 2020 2020 2020 2023 2049 6620 7468 6520         # If the 
-0000a0d0: 6e75 6d62 6572 206f 6620 7469 6c65 7320  number of tiles 
-0000a0e0: 656e 6473 2075 7020 6173 2031 2c20 6974  ends up as 1, it
-0000a0f0: 2069 7320 7468 6520 6c61 7374 2070 6173   is the last pas
-0000a100: 7320 616e 7977 6179 2e2e 2e0a 2020 2020  s anyway....    
-0000a110: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-0000a120: 656e 2874 696c 6573 5f67 6466 2920 3d3d  en(tiles_gdf) ==
-0000a130: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-0000a140: 2020 2020 2020 2020 6c61 7374 5f70 6173          last_pas
-0000a150: 7320 3d20 5472 7565 0a0a 2020 2020 2020  s = True..      
-0000a160: 2020 2020 2020 2020 2020 2320 4966 2077            # If w
-0000a170: 6520 6172 6520 6e6f 7420 696e 2074 6865  e are not in the
-0000a180: 206c 6173 7420 7061 7373 2c20 6f6e 626f   last pass, onbo
-0000a190: 7264 6572 2070 6172 6365 6c73 2077 696c  rder parcels wil
-0000a1a0: 6c20 6e65 6564 2065 7874 7261 0a20 2020  l need extra.   
-0000a1b0: 2020 2020 2020 2020 2020 2020 2023 2070               # p
-0000a1c0: 726f 6365 7373 696e 6720 7374 696c 6c20  rocessing still 
-0000a1d0: 696e 2066 7572 7468 6572 2070 6173 7365  in further passe
-0000a1e0: 732c 2073 6f20 6172 6520 7361 7665 6420  s, so are saved 
-0000a1f0: 696e 2061 2073 6570 6572 6174 650a 2020  in a seperate.  
-0000a200: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000a210: 6766 6f2e 2054 6865 206e 6f74 6f6e 626f  gfo. The notonbo
-0000a220: 7264 6572 2072 6f77 7320 6172 6520 6669  rder rows are fi
-0000a230: 6e61 6c20 696d 6d65 6469 6174 656c 790a  nal immediately.
-0000a240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a250: 6966 206c 6173 745f 7061 7373 2069 7320  if last_pass is 
-0000a260: 6e6f 7420 5472 7565 3a0a 2020 2020 2020  not True:.      
-0000a270: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-0000a280: 7470 7574 5f74 6d70 5f6f 6e62 6f72 6465  tput_tmp_onborde
-0000a290: 725f 7061 7468 203d 2028 0a20 2020 2020  r_path = (.     
-0000a2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2b0: 2020 2074 656d 7064 6972 202f 2066 226f     tempdir / f"o
-0000a2c0: 7574 7075 745f 7b70 6173 735f 6964 7d5f  utput_{pass_id}_
-0000a2d0: 6f6e 626f 7264 6572 2e67 706b 6722 0a20  onborder.gpkg". 
-0000a2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a2f0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
-0000a300: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000a310: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-0000a320: 7574 7075 745f 746d 705f 6f6e 626f 7264  utput_tmp_onbord
-0000a330: 6572 5f70 6174 6820 3d20 6f75 7470 7574  er_path = output
-0000a340: 5f74 6d70 5f70 6174 680a 0a20 2020 2020  _tmp_path..     
-0000a350: 2020 2020 2020 2020 2020 2023 204e 6f77             # Now
-0000a360: 2067 6f21 0a20 2020 2020 2020 2020 2020   go!.           
-0000a370: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-0000a380: 2866 2253 7461 7274 2064 6973 736f 6c76  (f"Start dissolv
-0000a390: 6520 7061 7373 207b 7061 7373 5f69 647d  e pass {pass_id}
-0000a3a0: 2074 6f20 7b6c 656e 2874 696c 6573 5f67   to {len(tiles_g
-0000a3b0: 6466 297d 2074 696c 6573 2229 0a20 2020  df)} tiles").   
-0000a3c0: 2020 2020 2020 2020 2020 2020 205f 203d               _ =
-0000a3d0: 205f 6469 7373 6f6c 7665 5f70 6f6c 7967   _dissolve_polyg
-0000a3e0: 6f6e 735f 7061 7373 280a 2020 2020 2020  ons_pass(.      
-0000a3f0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000a400: 7075 745f 7061 7468 3d69 6e70 7574 5f70  put_path=input_p
-0000a410: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
-0000a420: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-0000a430: 6e6f 746f 6e62 6f72 6465 725f 7061 7468  notonborder_path
-0000a440: 3d6f 7574 7075 745f 746d 705f 7061 7468  =output_tmp_path
-0000a450: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000a460: 2020 2020 2020 6f75 7470 7574 5f6f 6e62        output_onb
-0000a470: 6f72 6465 725f 7061 7468 3d6f 7574 7075  order_path=outpu
-0000a480: 745f 746d 705f 6f6e 626f 7264 6572 5f70  t_tmp_onborder_p
-0000a490: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
-0000a4a0: 2020 2020 2020 2020 2065 7870 6c6f 6465           explode
-0000a4b0: 636f 6c6c 6563 7469 6f6e 733d 6578 706c  collections=expl
-0000a4c0: 6f64 6563 6f6c 6c65 6374 696f 6e73 2c0a  odecollections,.
-0000a4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a4e0: 2020 2020 6772 6f75 7062 795f 636f 6c75      groupby_colu
-0000a4f0: 6d6e 733d 6772 6f75 7062 795f 636f 6c75  mns=groupby_colu
-0000a500: 6d6e 732c 0a20 2020 2020 2020 2020 2020  mns,.           
-0000a510: 2020 2020 2020 2020 2061 6767 5f63 6f6c           agg_col
-0000a520: 756d 6e73 3d61 6767 5f63 6f6c 756d 6e73  umns=agg_columns
-0000a530: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000a540: 2020 2020 2020 7469 6c65 735f 6764 663d        tiles_gdf=
-0000a550: 7469 6c65 735f 6764 662c 0a20 2020 2020  tiles_gdf,.     
-0000a560: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000a570: 6e70 7574 5f6c 6179 6572 3d69 6e70 7574  nput_layer=input
-0000a580: 5f70 6173 735f 6c61 7965 722c 0a20 2020  _pass_layer,.   
-0000a590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5a0: 206f 7574 7075 745f 6c61 7965 723d 6f75   output_layer=ou
-0000a5b0: 7470 7574 5f6c 6179 6572 2c0a 2020 2020  tput_layer,.    
-0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5d0: 6772 6964 7369 7a65 3d67 7269 6473 697a  gridsize=gridsiz
-0000a5e0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-0000a5f0: 2020 2020 2020 206b 6565 705f 656d 7074         keep_empt
-0000a600: 795f 6765 6f6d 733d 4661 6c73 652c 0a20  y_geoms=False,. 
-0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a620: 2020 206e 625f 7061 7261 6c6c 656c 3d6e     nb_parallel=n
-0000a630: 625f 7061 7261 6c6c 656c 2c0a 2020 2020  b_parallel,.    
-0000a640: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-0000a650: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000a660: 2050 7265 7061 7265 2074 6865 206e 6578   Prepare the nex
-0000a670: 7420 7061 7373 0a20 2020 2020 2020 2020  t pass.         
-0000a680: 2020 2020 2020 2023 2054 6865 2069 6e70         # The inp
-0000a690: 7574 2070 6174 6820 6973 2074 6865 206f  ut path is the o
-0000a6a0: 6e62 6f72 6465 7220 6669 6c65 0a20 2020  nborder file.   
-0000a6b0: 2020 2020 2020 2020 2020 2020 2070 7265               pre
-0000a6c0: 765f 6e62 5f62 6174 6368 6573 203d 206c  v_nb_batches = l
-0000a6d0: 656e 2874 696c 6573 5f67 6466 290a 2020  en(tiles_gdf).  
-0000a6e0: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000a6f0: 7075 745f 7061 7468 203d 206f 7574 7075  put_path = outpu
-0000a700: 745f 746d 705f 6f6e 626f 7264 6572 5f70  t_tmp_onborder_p
-0000a710: 6174 680a 2020 2020 2020 2020 2020 2020  ath.            
-0000a720: 2020 2020 7061 7373 5f69 6420 2b3d 2031      pass_id += 1
-0000a730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a740: 2069 6e70 7574 5f70 6173 735f 6c61 7965   input_pass_laye
-0000a750: 7220 3d20 4e6f 6e65 0a0a 2020 2020 2020  r = None..      
-0000a760: 2020 2020 2020 2020 2020 2320 4966 2077            # If w
-0000a770: 6520 6172 6520 7265 6164 792e 2e2e 0a20  e are ready.... 
-0000a780: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000a790: 6620 6c61 7374 5f70 6173 7320 6973 2054  f last_pass is T
-0000a7a0: 7275 653a 0a20 2020 2020 2020 2020 2020  rue:.           
-0000a7b0: 2020 2020 2020 2020 2062 7265 616b 0a0a           break..
-0000a7c0: 2020 2020 2020 2020 2020 2020 2320 4361              # Ca
-0000a7d0: 6c63 756c 6174 696f 6e20 7265 6164 7921  lculation ready!
-0000a7e0: 204e 6f77 2066 696e 616c 6973 6520 6f75   Now finalise ou
-0000a7f0: 7470 7574 210a 2020 2020 2020 2020 2020  tput!.          
-0000a800: 2020 2320 4966 2074 6865 7265 2069 7320    # If there is 
-0000a810: 6120 7265 7375 6c74 206f 6e20 626f 7264  a result on bord
-0000a820: 6572 2c20 6170 7065 6e64 2069 7420 746f  er, append it to
-0000a830: 2074 6865 2072 6573 740a 2020 2020 2020   the rest.      
-0000a840: 2020 2020 2020 6966 2028 0a20 2020 2020        if (.     
-0000a850: 2020 2020 2020 2020 2020 2073 7472 286f             str(o
-0000a860: 7574 7075 745f 746d 705f 6f6e 626f 7264  utput_tmp_onbord
-0000a870: 6572 5f70 6174 6829 2021 3d20 7374 7228  er_path) != str(
-0000a880: 6f75 7470 7574 5f74 6d70 5f70 6174 6829  output_tmp_path)
-0000a890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a8a0: 2061 6e64 206f 7574 7075 745f 746d 705f   and output_tmp_
-0000a8b0: 6f6e 626f 7264 6572 5f70 6174 682e 6578  onborder_path.ex
-0000a8c0: 6973 7473 2829 0a20 2020 2020 2020 2020  ists().         
-0000a8d0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-0000a8e0: 2020 2020 2020 6766 6f2e 6170 7065 6e64        gfo.append
-0000a8f0: 5f74 6f28 0a20 2020 2020 2020 2020 2020  _to(.           
-0000a900: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-0000a910: 746d 705f 6f6e 626f 7264 6572 5f70 6174  tmp_onborder_pat
-0000a920: 682c 206f 7574 7075 745f 746d 705f 7061  h, output_tmp_pa
-0000a930: 7468 2c20 6473 745f 6c61 7965 723d 6f75  th, dst_layer=ou
-0000a940: 7470 7574 5f6c 6179 6572 0a20 2020 2020  tput_layer.     
-0000a950: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0000a960: 2020 2020 2020 2020 2020 2320 4966 2074            # If t
-0000a970: 6865 7265 2069 7320 6120 7265 7375 6c74  here is a result
-0000a980: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-0000a990: 6966 206f 7574 7075 745f 746d 705f 7061  if output_tmp_pa
-0000a9a0: 7468 2e65 7869 7374 7328 293a 0a20 2020  th.exists():.   
-0000a9b0: 2020 2020 2020 2020 2020 2020 2023 2049               # I
-0000a9c0: 6620 7469 6c65 6420 6f75 7470 7574 2061  f tiled output a
-0000a9d0: 736b 6564 2c20 6164 6420 2274 696c 655f  sked, add "tile_
-0000a9e0: 6964 2220 746f 2067 726f 7570 6279 5f63  id" to groupby_c
-0000a9f0: 6f6c 756d 6e73 0a20 2020 2020 2020 2020  olumns.         
-0000aa00: 2020 2020 2020 2069 6620 6c65 6e28 7265         if len(re
-0000aa10: 7375 6c74 5f74 696c 6573 5f67 6466 2920  sult_tiles_gdf) 
-0000aa20: 3e20 313a 0a20 2020 2020 2020 2020 2020  > 1:.           
-0000aa30: 2020 2020 2020 2020 2069 6620 6772 6f75           if grou
-0000aa40: 7062 795f 636f 6c75 6d6e 7320 6973 204e  pby_columns is N
-0000aa50: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000aa60: 2020 2020 2020 2020 2020 2020 2067 726f               gro
-0000aa70: 7570 6279 5f63 6f6c 756d 6e73 203d 205b  upby_columns = [
-0000aa80: 2274 696c 655f 6964 225d 0a20 2020 2020  "tile_id"].     
-0000aa90: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000aaa0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000aab0: 2020 2020 2020 2020 2020 2020 2067 726f               gro
-0000aac0: 7570 6279 5f63 6f6c 756d 6e73 203d 206c  upby_columns = l
-0000aad0: 6973 7428 6772 6f75 7062 795f 636f 6c75  ist(groupby_colu
-0000aae0: 6d6e 7329 2e63 6f70 7928 290a 2020 2020  mns).copy().    
-0000aaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab00: 2020 2020 6772 6f75 7062 795f 636f 6c75      groupby_colu
-0000ab10: 6d6e 732e 6170 7065 6e64 2822 7469 6c65  mns.append("tile
-0000ab20: 5f69 6422 290a 0a20 2020 2020 2020 2020  _id")..         
-0000ab30: 2020 2020 2020 2023 2050 7265 7061 7265         # Prepare
-0000ab40: 2073 7472 696e 6773 2074 6f20 7573 6520   strings to use 
-0000ab50: 696e 2073 656c 6563 7420 6261 7365 6420  in select based 
-0000ab60: 6f6e 2067 726f 7570 6279 5f63 6f6c 756d  on groupby_colum
-0000ab70: 6e73 0a20 2020 2020 2020 2020 2020 2020  ns.             
-0000ab80: 2020 2069 6620 6772 6f75 7062 795f 636f     if groupby_co
-0000ab90: 6c75 6d6e 7320 6973 206e 6f74 204e 6f6e  lumns is not Non
-0000aba0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000abb0: 2020 2020 2020 2067 726f 7570 6279 5f70         groupby_p
-0000abc0: 7265 6669 7865 645f 6c69 7374 203d 205b  refixed_list = [
-0000abd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000abe0: 2020 2020 2020 2020 2066 277b 7b70 7265           f'{{pre
-0000abf0: 6669 787d 7d22 7b63 6f6c 756d 6e7d 2227  fix}}"{column}"'
-0000ac00: 2066 6f72 2063 6f6c 756d 6e20 696e 2067   for column in g
-0000ac10: 726f 7570 6279 5f63 6f6c 756d 6e73 0a20  roupby_columns. 
-0000ac20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac30: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
-0000ac40: 2020 2020 2020 2020 2067 726f 7570 6279           groupby
-0000ac50: 5f73 656c 6563 745f 7072 6566 6978 6564  _select_prefixed
-0000ac60: 5f73 7472 203d 2028 0a20 2020 2020 2020  _str = (.       
-0000ac70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac80: 2066 222c 207b 272c 2027 2e6a 6f69 6e28   f", {', '.join(
-0000ac90: 6772 6f75 7062 795f 7072 6566 6978 6564  groupby_prefixed
-0000aca0: 5f6c 6973 7429 7d22 0a20 2020 2020 2020  _list)}".       
-0000acb0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000acc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000acd0: 2020 2067 726f 7570 6279 5f67 726f 7570     groupby_group
-0000ace0: 6279 5f70 7265 6669 7865 645f 7374 7220  by_prefixed_str 
-0000acf0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0000ad00: 2020 2020 2020 2020 2020 2020 6622 4752              f"GR
-0000ad10: 4f55 5020 4259 207b 272c 2027 2e6a 6f69  OUP BY {', '.joi
-0000ad20: 6e28 6772 6f75 7062 795f 7072 6566 6978  n(groupby_prefix
-0000ad30: 6564 5f6c 6973 7429 7d22 0a20 2020 2020  ed_list)}".     
-0000ad40: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000ad50: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000ad60: 2020 2020 2020 6772 6f75 7062 795f 6669        groupby_fi
-0000ad70: 6c74 6572 5f6c 6973 7420 3d20 5b0a 2020  lter_list = [.  
-0000ad80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ad90: 2020 2020 2020 6627 2041 4e44 2067 656f        f' AND geo
-0000ada0: 5f64 6174 612e 227b 636f 6c75 6d6e 7d22  _data."{column}"
-0000adb0: 203d 206a 736f 6e5f 6461 7461 2e22 7b63   = json_data."{c
-0000adc0: 6f6c 756d 6e7d 2227 0a20 2020 2020 2020  olumn}"'.       
-0000add0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ade0: 2066 6f72 2063 6f6c 756d 6e20 696e 2067   for column in g
-0000adf0: 726f 7570 6279 5f63 6f6c 756d 6e73 0a20  roupby_columns. 
-0000ae00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae10: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
-0000ae20: 2020 2020 2020 2020 2067 726f 7570 6279           groupby
-0000ae30: 5f66 696c 7465 725f 7374 7220 3d20 2220  _filter_str = " 
-0000ae40: 222e 6a6f 696e 2867 726f 7570 6279 5f66  ".join(groupby_f
-0000ae50: 696c 7465 725f 6c69 7374 290a 2020 2020  ilter_list).    
-0000ae60: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000ae70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ae80: 2020 2020 2020 6772 6f75 7062 795f 7365        groupby_se
-0000ae90: 6c65 6374 5f70 7265 6669 7865 645f 7374  lect_prefixed_st
-0000aea0: 7220 3d20 2222 0a20 2020 2020 2020 2020  r = "".         
-0000aeb0: 2020 2020 2020 2020 2020 2067 726f 7570             group
-0000aec0: 6279 5f67 726f 7570 6279 5f70 7265 6669  by_groupby_prefi
-0000aed0: 7865 645f 7374 7220 3d20 2222 0a20 2020  xed_str = "".   
-0000aee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aef0: 2067 726f 7570 6279 5f66 696c 7465 725f   groupby_filter_
-0000af00: 7374 7220 3d20 2222 0a0a 2020 2020 2020  str = ""..      
-0000af10: 2020 2020 2020 2020 2020 2320 5072 6570            # Prep
-0000af20: 6172 6520 7374 7269 6e67 7320 746f 2075  are strings to u
-0000af30: 7365 2069 6e20 7365 6c65 6374 2062 6173  se in select bas
-0000af40: 6564 206f 6e20 6167 675f 636f 6c75 6d6e  ed on agg_column
-0000af50: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0000af60: 2020 6167 675f 636f 6c75 6d6e 735f 7374    agg_columns_st
-0000af70: 7220 3d20 2222 0a20 2020 2020 2020 2020  r = "".         
-0000af80: 2020 2020 2020 2069 6620 6167 675f 636f         if agg_co
-0000af90: 6c75 6d6e 7320 6973 206e 6f74 204e 6f6e  lumns is not Non
-0000afa0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000afb0: 2020 2020 2020 2069 6620 226a 736f 6e22         if "json"
-0000afc0: 2069 6e20 6167 675f 636f 6c75 6d6e 733a   in agg_columns:
-0000afd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000afe0: 2020 2020 2020 2020 2023 2054 6865 2061           # The a
-0000aff0: 6767 7265 6761 7469 6f6e 2069 7320 746f  ggregation is to
-0000b000: 2061 206a 736f 6e20 636f 6c75 6d6e 2c20   a json column, 
-0000b010: 736f 2061 6464 0a20 2020 2020 2020 2020  so add.         
-0000b020: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0000b030: 6767 5f63 6f6c 756d 6e73 5f73 7472 202b  gg_columns_str +
-0000b040: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-0000b050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b060: 222c 6a73 6f6e 5f67 726f 7570 5f61 7272  ",json_group_arr
-0000b070: 6179 2844 4953 5449 4e43 5420 6a73 6f6e  ay(DISTINCT json
-0000b080: 5f64 6174 612e 6a73 6f6e 5f72 6f77 2920  _data.json_row) 
-0000b090: 6173 206a 736f 6e22 0a20 2020 2020 2020  as json".       
-0000b0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0b0: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000b0c0: 2020 2020 2020 2065 6c69 6620 2263 6f6c         elif "col
-0000b0d0: 756d 6e73 2220 696e 2061 6767 5f63 6f6c  umns" in agg_col
-0000b0e0: 756d 6e73 3a0a 2020 2020 2020 2020 2020  umns:.          
-0000b0f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000b100: 7220 6167 675f 636f 6c75 6d6e 2069 6e20  r agg_column in 
-0000b110: 6167 675f 636f 6c75 6d6e 735b 2263 6f6c  agg_columns["col
-0000b120: 756d 6e73 225d 3a0a 2020 2020 2020 2020  umns"]:.        
+00009dd0: 2020 2020 2320 4966 2061 2067 7269 6420      # If a grid 
+00009de0: 6973 2073 7065 6369 6669 6564 2061 6c72  is specified alr
+00009df0: 6561 6479 2c20 6164 6420 6578 7472 6120  eady, add extra 
+00009e00: 636f 6c75 6d6e 732f 726f 7773 2069 6e73  columns/rows ins
+00009e10: 7465 6164 206f 660a 2020 2020 2020 2020  tead of.        
+00009e20: 2020 2020 2020 2020 2020 2020 2320 6372              # cr
+00009e30: 6561 7469 6e67 206e 6577 206f 6e65 2e2e  eating new one..
+00009e40: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00009e50: 2020 2020 2020 7469 6c65 735f 6764 6620        tiles_gdf 
+00009e60: 3d20 6772 6964 5f75 7469 6c2e 7370 6c69  = grid_util.spli
+00009e70: 745f 7469 6c65 7328 0a20 2020 2020 2020  t_tiles(.       
+00009e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e90: 2072 6573 756c 745f 7469 6c65 735f 6764   result_tiles_gd
+00009ea0: 662c 206e 625f 6261 7463 6865 735f 7265  f, nb_batches_re
+00009eb0: 636f 6d6d 656e 6465 640a 2020 2020 2020  commended.      
+00009ec0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+00009ed0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009ee0: 2023 2041 7070 6c79 2067 7269 6473 697a   # Apply gridsiz
+00009ef0: 6520 746f 6c65 7261 6e63 6520 6f6e 2074  e tolerance on t
+00009f00: 696c 6573 2c20 6f74 6865 7277 6973 6520  iles, otherwise 
+00009f10: 7468 6520 626f 7264 6572 2070 6f6c 7967  the border polyg
+00009f20: 6f6e 7320 6361 6e27 740a 2020 2020 2020  ons can't.      
+00009f30: 2020 2020 2020 2020 2020 2320 6265 2075            # be u
+00009f40: 6e69 6f6e 6564 2070 726f 7065 726c 7920  nioned properly 
+00009f50: 6265 6361 7573 6520 6761 7073 2061 7070  because gaps app
+00009f60: 6561 7220 6166 7465 7220 726f 756e 6469  ear after roundi
+00009f70: 6e67 2063 6f6f 7264 696e 6174 6573 2e0a  ng coordinates..
+00009f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f90: 6966 2067 7269 6473 697a 6520 213d 2030  if gridsize != 0
+00009fa0: 2e30 3a0a 2020 2020 2020 2020 2020 2020  .0:.            
+00009fb0: 2020 2020 2020 2020 7469 6c65 735f 6764          tiles_gd
+00009fc0: 662e 6765 6f6d 6574 7279 203d 2073 6861  f.geometry = sha
+00009fd0: 7065 6c79 325f 6f72 5f70 7967 656f 732e  pely2_or_pygeos.
+00009fe0: 7365 745f 7072 6563 6973 696f 6e28 0a20  set_precision(. 
+00009ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a000: 2020 2020 2020 2074 696c 6573 5f67 6466         tiles_gdf
+0000a010: 2e67 656f 6d65 7472 792c 2067 7269 645f  .geometry, grid_
+0000a020: 7369 7a65 3d67 7269 6473 697a 650a 2020  size=gridsize.  
+0000a030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a040: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000a050: 2020 2020 6766 6f2e 746f 5f66 696c 6528      gfo.to_file(
+0000a060: 7469 6c65 735f 6764 662c 2074 656d 7064  tiles_gdf, tempd
+0000a070: 6972 202f 2066 226f 7574 7075 745f 7b70  ir / f"output_{p
+0000a080: 6173 735f 6964 7d5f 7469 6c65 732e 6770  ass_id}_tiles.gp
+0000a090: 6b67 2229 0a0a 2020 2020 2020 2020 2020  kg")..          
+0000a0a0: 2020 2020 2020 2320 4966 2074 6865 206e        # If the n
+0000a0b0: 756d 6265 7220 6f66 2074 696c 6573 2065  umber of tiles e
+0000a0c0: 6e64 7320 7570 2061 7320 312c 2069 7420  nds up as 1, it 
+0000a0d0: 6973 2074 6865 206c 6173 7420 7061 7373  is the last pass
+0000a0e0: 2061 6e79 7761 792e 2e2e 0a20 2020 2020   anyway....     
+0000a0f0: 2020 2020 2020 2020 2020 2069 6620 6c65             if le
+0000a100: 6e28 7469 6c65 735f 6764 6629 203d 3d20  n(tiles_gdf) == 
+0000a110: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+0000a120: 2020 2020 2020 206c 6173 745f 7061 7373         last_pass
+0000a130: 203d 2054 7275 650a 0a20 2020 2020 2020   = True..       
+0000a140: 2020 2020 2020 2020 2023 2049 6620 7765           # If we
+0000a150: 2061 7265 206e 6f74 2069 6e20 7468 6520   are not in the 
+0000a160: 6c61 7374 2070 6173 732c 206f 6e62 6f72  last pass, onbor
+0000a170: 6465 7220 7061 7263 656c 7320 7769 6c6c  der parcels will
+0000a180: 206e 6565 6420 6578 7472 610a 2020 2020   need extra.    
+0000a190: 2020 2020 2020 2020 2020 2020 2320 7072              # pr
+0000a1a0: 6f63 6573 7369 6e67 2073 7469 6c6c 2069  ocessing still i
+0000a1b0: 6e20 6675 7274 6865 7220 7061 7373 6573  n further passes
+0000a1c0: 2c20 736f 2061 7265 2073 6176 6564 2069  , so are saved i
+0000a1d0: 6e20 6120 7365 7065 7261 7465 0a20 2020  n a seperate.   
+0000a1e0: 2020 2020 2020 2020 2020 2020 2023 2067               # g
+0000a1f0: 666f 2e20 5468 6520 6e6f 746f 6e62 6f72  fo. The notonbor
+0000a200: 6465 7220 726f 7773 2061 7265 2066 696e  der rows are fin
+0000a210: 616c 2069 6d6d 6564 6961 7465 6c79 0a20  al immediately. 
+0000a220: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000a230: 6620 6c61 7374 5f70 6173 7320 6973 206e  f last_pass is n
+0000a240: 6f74 2054 7275 653a 0a20 2020 2020 2020  ot True:.       
+0000a250: 2020 2020 2020 2020 2020 2020 206f 7574               out
+0000a260: 7075 745f 746d 705f 6f6e 626f 7264 6572  put_tmp_onborder
+0000a270: 5f70 6174 6820 3d20 280a 2020 2020 2020  _path = (.      
+0000a280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a290: 2020 7465 6d70 6469 7220 2f20 6622 6f75    tempdir / f"ou
+0000a2a0: 7470 7574 5f7b 7061 7373 5f69 647d 5f6f  tput_{pass_id}_o
+0000a2b0: 6e62 6f72 6465 722e 6770 6b67 220a 2020  nborder.gpkg".  
+0000a2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a2d0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+0000a2e0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000a2f0: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
+0000a300: 7470 7574 5f74 6d70 5f6f 6e62 6f72 6465  tput_tmp_onborde
+0000a310: 725f 7061 7468 203d 206f 7574 7075 745f  r_path = output_
+0000a320: 746d 705f 7061 7468 0a0a 2020 2020 2020  tmp_path..      
+0000a330: 2020 2020 2020 2020 2020 2320 4e6f 7720            # Now 
+0000a340: 676f 210a 2020 2020 2020 2020 2020 2020  go!.            
+0000a350: 2020 2020 6c6f 6767 6572 2e69 6e66 6f28      logger.info(
+0000a360: 6622 5374 6172 7420 6469 7373 6f6c 7665  f"Start dissolve
+0000a370: 2070 6173 7320 7b70 6173 735f 6964 7d20   pass {pass_id} 
+0000a380: 746f 207b 6c65 6e28 7469 6c65 735f 6764  to {len(tiles_gd
+0000a390: 6629 7d20 7469 6c65 7322 290a 2020 2020  f)} tiles").    
+0000a3a0: 2020 2020 2020 2020 2020 2020 5f20 3d20              _ = 
+0000a3b0: 5f64 6973 736f 6c76 655f 706f 6c79 676f  _dissolve_polygo
+0000a3c0: 6e73 5f70 6173 7328 0a20 2020 2020 2020  ns_pass(.       
+0000a3d0: 2020 2020 2020 2020 2020 2020 2069 6e70               inp
+0000a3e0: 7574 5f70 6174 683d 696e 7075 745f 7061  ut_path=input_pa
+0000a3f0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+0000a400: 2020 2020 2020 2020 6f75 7470 7574 5f6e          output_n
+0000a410: 6f74 6f6e 626f 7264 6572 5f70 6174 683d  otonborder_path=
+0000a420: 6f75 7470 7574 5f74 6d70 5f70 6174 682c  output_tmp_path,
+0000a430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a440: 2020 2020 206f 7574 7075 745f 6f6e 626f       output_onbo
+0000a450: 7264 6572 5f70 6174 683d 6f75 7470 7574  rder_path=output
+0000a460: 5f74 6d70 5f6f 6e62 6f72 6465 725f 7061  _tmp_onborder_pa
+0000a470: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+0000a480: 2020 2020 2020 2020 6578 706c 6f64 6563          explodec
+0000a490: 6f6c 6c65 6374 696f 6e73 3d65 7870 6c6f  ollections=explo
+0000a4a0: 6465 636f 6c6c 6563 7469 6f6e 732c 0a20  decollections,. 
+0000a4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a4c0: 2020 2067 726f 7570 6279 5f63 6f6c 756d     groupby_colum
+0000a4d0: 6e73 3d67 726f 7570 6279 5f63 6f6c 756d  ns=groupby_colum
+0000a4e0: 6e73 2c0a 2020 2020 2020 2020 2020 2020  ns,.            
+0000a4f0: 2020 2020 2020 2020 6167 675f 636f 6c75          agg_colu
+0000a500: 6d6e 733d 6167 675f 636f 6c75 6d6e 732c  mns=agg_columns,
+0000a510: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a520: 2020 2020 2074 696c 6573 5f67 6466 3d74       tiles_gdf=t
+0000a530: 696c 6573 5f67 6466 2c0a 2020 2020 2020  iles_gdf,.      
+0000a540: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000a550: 7075 745f 6c61 7965 723d 696e 7075 745f  put_layer=input_
+0000a560: 7061 7373 5f6c 6179 6572 2c0a 2020 2020  pass_layer,.    
+0000a570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a580: 6f75 7470 7574 5f6c 6179 6572 3d6f 7574  output_layer=out
+0000a590: 7075 745f 6c61 7965 722c 0a20 2020 2020  put_layer,.     
+0000a5a0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+0000a5b0: 7269 6473 697a 653d 6772 6964 7369 7a65  ridsize=gridsize
+0000a5c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a5d0: 2020 2020 2020 6b65 6570 5f65 6d70 7479        keep_empty
+0000a5e0: 5f67 656f 6d73 3d46 616c 7365 2c0a 2020  _geoms=False,.  
+0000a5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a600: 2020 6e62 5f70 6172 616c 6c65 6c3d 6e62    nb_parallel=nb
+0000a610: 5f70 6172 616c 6c65 6c2c 0a20 2020 2020  _parallel,.     
+0000a620: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000a630: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000a640: 5072 6570 6172 6520 7468 6520 6e65 7874  Prepare the next
+0000a650: 2070 6173 730a 2020 2020 2020 2020 2020   pass.          
+0000a660: 2020 2020 2020 2320 5468 6520 696e 7075        # The inpu
+0000a670: 7420 7061 7468 2069 7320 7468 6520 6f6e  t path is the on
+0000a680: 626f 7264 6572 2066 696c 650a 2020 2020  border file.    
+0000a690: 2020 2020 2020 2020 2020 2020 7072 6576              prev
+0000a6a0: 5f6e 625f 6261 7463 6865 7320 3d20 6c65  _nb_batches = le
+0000a6b0: 6e28 7469 6c65 735f 6764 6629 0a20 2020  n(tiles_gdf).   
+0000a6c0: 2020 2020 2020 2020 2020 2020 2069 6e70               inp
+0000a6d0: 7574 5f70 6174 6820 3d20 6f75 7470 7574  ut_path = output
+0000a6e0: 5f74 6d70 5f6f 6e62 6f72 6465 725f 7061  _tmp_onborder_pa
+0000a6f0: 7468 0a20 2020 2020 2020 2020 2020 2020  th.             
+0000a700: 2020 2070 6173 735f 6964 202b 3d20 310a     pass_id += 1.
+0000a710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a720: 696e 7075 745f 7061 7373 5f6c 6179 6572  input_pass_layer
+0000a730: 203d 204e 6f6e 650a 0a20 2020 2020 2020   = None..       
+0000a740: 2020 2020 2020 2020 2023 2049 6620 7765           # If we
+0000a750: 2061 7265 2072 6561 6479 2e2e 2e0a 2020   are ready....  
+0000a760: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000a770: 206c 6173 745f 7061 7373 2069 7320 5472   last_pass is Tr
+0000a780: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
+0000a790: 2020 2020 2020 2020 6272 6561 6b0a 0a20          break.. 
+0000a7a0: 2020 2020 2020 2020 2020 2023 2043 616c             # Cal
+0000a7b0: 6375 6c61 7469 6f6e 2072 6561 6479 2120  culation ready! 
+0000a7c0: 4e6f 7720 6669 6e61 6c69 7365 206f 7574  Now finalise out
+0000a7d0: 7075 7421 0a20 2020 2020 2020 2020 2020  put!.           
+0000a7e0: 2023 2049 6620 7468 6572 6520 6973 2061   # If there is a
+0000a7f0: 2072 6573 756c 7420 6f6e 2062 6f72 6465   result on borde
+0000a800: 722c 2061 7070 656e 6420 6974 2074 6f20  r, append it to 
+0000a810: 7468 6520 7265 7374 0a20 2020 2020 2020  the rest.       
+0000a820: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
+0000a830: 2020 2020 2020 2020 2020 7374 7228 6f75            str(ou
+0000a840: 7470 7574 5f74 6d70 5f6f 6e62 6f72 6465  tput_tmp_onborde
+0000a850: 725f 7061 7468 2920 213d 2073 7472 286f  r_path) != str(o
+0000a860: 7574 7075 745f 746d 705f 7061 7468 290a  utput_tmp_path).
+0000a870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a880: 616e 6420 6f75 7470 7574 5f74 6d70 5f6f  and output_tmp_o
+0000a890: 6e62 6f72 6465 725f 7061 7468 2e65 7869  nborder_path.exi
+0000a8a0: 7374 7328 290a 2020 2020 2020 2020 2020  sts().          
+0000a8b0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+0000a8c0: 2020 2020 2067 666f 2e61 7070 656e 645f       gfo.append_
+0000a8d0: 746f 280a 2020 2020 2020 2020 2020 2020  to(.            
+0000a8e0: 2020 2020 2020 2020 6f75 7470 7574 5f74          output_t
+0000a8f0: 6d70 5f6f 6e62 6f72 6465 725f 7061 7468  mp_onborder_path
+0000a900: 2c20 6f75 7470 7574 5f74 6d70 5f70 6174  , output_tmp_pat
+0000a910: 682c 2064 7374 5f6c 6179 6572 3d6f 7574  h, dst_layer=out
+0000a920: 7075 745f 6c61 7965 720a 2020 2020 2020  put_layer.      
+0000a930: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000a940: 2020 2020 2020 2020 2023 2049 6620 7468           # If th
+0000a950: 6572 6520 6973 2061 2072 6573 756c 742e  ere is a result.
+0000a960: 2e2e 0a20 2020 2020 2020 2020 2020 2069  ...            i
+0000a970: 6620 6f75 7470 7574 5f74 6d70 5f70 6174  f output_tmp_pat
+0000a980: 682e 6578 6973 7473 2829 3a0a 2020 2020  h.exists():.    
+0000a990: 2020 2020 2020 2020 2020 2020 2320 4966              # If
+0000a9a0: 2074 696c 6564 206f 7574 7075 7420 6173   tiled output as
+0000a9b0: 6b65 642c 2061 6464 2022 7469 6c65 5f69  ked, add "tile_i
+0000a9c0: 6422 2074 6f20 6772 6f75 7062 795f 636f  d" to groupby_co
+0000a9d0: 6c75 6d6e 730a 2020 2020 2020 2020 2020  lumns.          
+0000a9e0: 2020 2020 2020 6966 206c 656e 2872 6573        if len(res
+0000a9f0: 756c 745f 7469 6c65 735f 6764 6629 203e  ult_tiles_gdf) >
+0000aa00: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
+0000aa10: 2020 2020 2020 2020 6966 2067 726f 7570          if group
+0000aa20: 6279 5f63 6f6c 756d 6e73 2069 7320 4e6f  by_columns is No
+0000aa30: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000aa40: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
+0000aa50: 7062 795f 636f 6c75 6d6e 7320 3d20 5b22  pby_columns = ["
+0000aa60: 7469 6c65 5f69 6422 5d0a 2020 2020 2020  tile_id"].      
+0000aa70: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000aa80: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000aa90: 2020 2020 2020 2020 2020 2020 6772 6f75              grou
+0000aaa0: 7062 795f 636f 6c75 6d6e 7320 3d20 6c69  pby_columns = li
+0000aab0: 7374 2867 726f 7570 6279 5f63 6f6c 756d  st(groupby_colum
+0000aac0: 6e73 292e 636f 7079 2829 0a20 2020 2020  ns).copy().     
+0000aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aae0: 2020 2067 726f 7570 6279 5f63 6f6c 756d     groupby_colum
+0000aaf0: 6e73 2e61 7070 656e 6428 2274 696c 655f  ns.append("tile_
+0000ab00: 6964 2229 0a0a 2020 2020 2020 2020 2020  id")..          
+0000ab10: 2020 2020 2020 2320 5072 6570 6172 6520        # Prepare 
+0000ab20: 7374 7269 6e67 7320 746f 2075 7365 2069  strings to use i
+0000ab30: 6e20 7365 6c65 6374 2062 6173 6564 206f  n select based o
+0000ab40: 6e20 6772 6f75 7062 795f 636f 6c75 6d6e  n groupby_column
+0000ab50: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+0000ab60: 2020 6966 2067 726f 7570 6279 5f63 6f6c    if groupby_col
+0000ab70: 756d 6e73 2069 7320 6e6f 7420 4e6f 6e65  umns is not None
+0000ab80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000ab90: 2020 2020 2020 6772 6f75 7062 795f 7072        groupby_pr
+0000aba0: 6566 6978 6564 5f6c 6973 7420 3d20 5b0a  efixed_list = [.
+0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000abc0: 2020 2020 2020 2020 6627 7b7b 7072 6566          f'{{pref
+0000abd0: 6978 7d7d 227b 636f 6c75 6d6e 7d22 2720  ix}}"{column}"' 
+0000abe0: 666f 7220 636f 6c75 6d6e 2069 6e20 6772  for column in gr
+0000abf0: 6f75 7062 795f 636f 6c75 6d6e 730a 2020  oupby_columns.  
+0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac10: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+0000ac20: 2020 2020 2020 2020 6772 6f75 7062 795f          groupby_
+0000ac30: 7365 6c65 6374 5f70 7265 6669 7865 645f  select_prefixed_
+0000ac40: 7374 7220 3d20 280a 2020 2020 2020 2020  str = (.        
+0000ac50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ac60: 6622 2c20 7b27 2c20 272e 6a6f 696e 2867  f", {', '.join(g
+0000ac70: 726f 7570 6279 5f70 7265 6669 7865 645f  roupby_prefixed_
+0000ac80: 6c69 7374 297d 220a 2020 2020 2020 2020  list)}".        
+0000ac90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000aca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000acb0: 2020 6772 6f75 7062 795f 6772 6f75 7062    groupby_groupb
+0000acc0: 795f 7072 6566 6978 6564 5f73 7472 203d  y_prefixed_str =
+0000acd0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0000ace0: 2020 2020 2020 2020 2020 2066 2247 524f             f"GRO
+0000acf0: 5550 2042 5920 7b27 2c20 272e 6a6f 696e  UP BY {', '.join
+0000ad00: 2867 726f 7570 6279 5f70 7265 6669 7865  (groupby_prefixe
+0000ad10: 645f 6c69 7374 297d 220a 2020 2020 2020  d_list)}".      
+0000ad20: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000ad30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ad40: 2020 2020 2067 726f 7570 6279 5f66 696c       groupby_fil
+0000ad50: 7465 725f 6c69 7374 203d 205b 0a20 2020  ter_list = [.   
+0000ad60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ad70: 2020 2020 2066 2720 414e 4420 6765 6f5f       f' AND geo_
+0000ad80: 6461 7461 2e22 7b63 6f6c 756d 6e7d 2220  data."{column}" 
+0000ad90: 3d20 6a73 6f6e 5f64 6174 612e 227b 636f  = json_data."{co
+0000ada0: 6c75 6d6e 7d22 270a 2020 2020 2020 2020  lumn}"'.        
+0000adb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000adc0: 666f 7220 636f 6c75 6d6e 2069 6e20 6772  for column in gr
+0000add0: 6f75 7062 795f 636f 6c75 6d6e 730a 2020  oupby_columns.  
+0000ade0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000adf0: 2020 5d0a 2020 2020 2020 2020 2020 2020    ].            
+0000ae00: 2020 2020 2020 2020 6772 6f75 7062 795f          groupby_
+0000ae10: 6669 6c74 6572 5f73 7472 203d 2022 2022  filter_str = " "
+0000ae20: 2e6a 6f69 6e28 6772 6f75 7062 795f 6669  .join(groupby_fi
+0000ae30: 6c74 6572 5f6c 6973 7429 0a20 2020 2020  lter_list).     
+0000ae40: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000ae50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ae60: 2020 2020 2067 726f 7570 6279 5f73 656c       groupby_sel
+0000ae70: 6563 745f 7072 6566 6978 6564 5f73 7472  ect_prefixed_str
+0000ae80: 203d 2022 220a 2020 2020 2020 2020 2020   = "".          
+0000ae90: 2020 2020 2020 2020 2020 6772 6f75 7062            groupb
+0000aea0: 795f 6772 6f75 7062 795f 7072 6566 6978  y_groupby_prefix
+0000aeb0: 6564 5f73 7472 203d 2022 220a 2020 2020  ed_str = "".    
+0000aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000aed0: 6772 6f75 7062 795f 6669 6c74 6572 5f73  groupby_filter_s
+0000aee0: 7472 203d 2022 220a 0a20 2020 2020 2020  tr = ""..       
+0000aef0: 2020 2020 2020 2020 2023 2050 7265 7061           # Prepa
+0000af00: 7265 2073 7472 696e 6773 2074 6f20 7573  re strings to us
+0000af10: 6520 696e 2073 656c 6563 7420 6261 7365  e in select base
+0000af20: 6420 6f6e 2061 6767 5f63 6f6c 756d 6e73  d on agg_columns
+0000af30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000af40: 2061 6767 5f63 6f6c 756d 6e73 5f73 7472   agg_columns_str
+0000af50: 203d 2022 220a 2020 2020 2020 2020 2020   = "".          
+0000af60: 2020 2020 2020 6966 2061 6767 5f63 6f6c        if agg_col
+0000af70: 756d 6e73 2069 7320 6e6f 7420 4e6f 6e65  umns is not None
+0000af80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000af90: 2020 2020 2020 6966 2022 6a73 6f6e 2220        if "json" 
+0000afa0: 696e 2061 6767 5f63 6f6c 756d 6e73 3a0a  in agg_columns:.
+0000afb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000afc0: 2020 2020 2020 2020 2320 5468 6520 6167          # The ag
+0000afd0: 6772 6567 6174 696f 6e20 6973 2074 6f20  gregation is to 
+0000afe0: 6120 6a73 6f6e 2063 6f6c 756d 6e2c 2073  a json column, s
+0000aff0: 6f20 6164 640a 2020 2020 2020 2020 2020  o add.          
+0000b000: 2020 2020 2020 2020 2020 2020 2020 6167                ag
+0000b010: 675f 636f 6c75 6d6e 735f 7374 7220 2b3d  g_columns_str +=
+0000b020: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+0000b030: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000b040: 2c6a 736f 6e5f 6772 6f75 705f 6172 7261  ,json_group_arra
+0000b050: 7928 4449 5354 494e 4354 206a 736f 6e5f  y(DISTINCT json_
+0000b060: 6461 7461 2e6a 736f 6e5f 726f 7729 2061  data.json_row) a
+0000b070: 7320 6a73 6f6e 220a 2020 2020 2020 2020  s json".        
+0000b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b090: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000b0a0: 2020 2020 2020 656c 6966 2022 636f 6c75        elif "colu
+0000b0b0: 6d6e 7322 2069 6e20 6167 675f 636f 6c75  mns" in agg_colu
+0000b0c0: 6d6e 733a 0a20 2020 2020 2020 2020 2020  mns:.           
+0000b0d0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000b0e0: 2061 6767 5f63 6f6c 756d 6e20 696e 2061   agg_column in a
+0000b0f0: 6767 5f63 6f6c 756d 6e73 5b22 636f 6c75  gg_columns["colu
+0000b100: 6d6e 7322 5d3a 0a20 2020 2020 2020 2020  mns"]:.         
+0000b110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b120: 2020 2023 2049 6e69 740a 2020 2020 2020     # Init.      
 0000b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b140: 2020 2020 2320 496e 6974 0a20 2020 2020      # Init.     
-0000b150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b160: 2020 2020 2020 2064 6973 7469 6e63 745f         distinct_
-0000b170: 7374 7220 3d20 2222 0a20 2020 2020 2020  str = "".       
-0000b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b190: 2020 2020 2065 7874 7261 5f70 6172 616d       extra_param
-0000b1a0: 5f73 7472 203d 2022 220a 0a20 2020 2020  _str = ""..     
-0000b1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b1c0: 2020 2020 2020 2023 2050 7265 7061 7265         # Prepare
-0000b1d0: 2061 6767 7265 6761 7469 6f6e 206b 6579   aggregation key
-0000b1e0: 776f 7264 2e0a 2020 2020 2020 2020 2020  word..          
-0000b1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b200: 2020 6966 2061 6767 5f63 6f6c 756d 6e5b    if agg_column[
-0000b210: 2261 6767 225d 2e6c 6f77 6572 2829 2069  "agg"].lower() i
-0000b220: 6e20 5b0a 2020 2020 2020 2020 2020 2020  n [.            
+0000b140: 2020 2020 2020 6469 7374 696e 6374 5f73        distinct_s
+0000b150: 7472 203d 2022 220a 2020 2020 2020 2020  tr = "".        
+0000b160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b170: 2020 2020 6578 7472 615f 7061 7261 6d5f      extra_param_
+0000b180: 7374 7220 3d20 2222 0a0a 2020 2020 2020  str = ""..      
+0000b190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1a0: 2020 2020 2020 2320 5072 6570 6172 6520        # Prepare 
+0000b1b0: 6167 6772 6567 6174 696f 6e20 6b65 7977  aggregation keyw
+0000b1c0: 6f72 642e 0a20 2020 2020 2020 2020 2020  ord..           
+0000b1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b1e0: 2069 6620 6167 675f 636f 6c75 6d6e 5b22   if agg_column["
+0000b1f0: 6167 6722 5d2e 6c6f 7765 7228 2920 696e  agg"].lower() in
+0000b200: 205b 0a20 2020 2020 2020 2020 2020 2020   [.             
+0000b210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b220: 2020 2022 636f 756e 7422 2c0a 2020 2020     "count",.    
 0000b230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b240: 2020 2020 2263 6f75 6e74 222c 0a20 2020      "count",.   
-0000b250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b260: 2020 2020 2020 2020 2020 2020 2022 7375               "su
-0000b270: 6d22 2c0a 2020 2020 2020 2020 2020 2020  m",.            
+0000b240: 2020 2020 2020 2020 2020 2020 2273 756d              "sum
+0000b250: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b270: 2020 2022 6d69 6e22 2c0a 2020 2020 2020     "min",.      
 0000b280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b290: 2020 2020 226d 696e 222c 0a20 2020 2020      "min",.     
-0000b2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2b0: 2020 2020 2020 2020 2020 2022 6d61 7822             "max"
-0000b2c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000b290: 2020 2020 2020 2020 2020 226d 6178 222c            "max",
+0000b2a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b2c0: 2022 6d65 6469 616e 222c 0a20 2020 2020   "median",.     
 0000b2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b2e0: 2020 226d 6564 6961 6e22 2c0a 2020 2020    "median",.    
+0000b2e0: 2020 2020 2020 205d 3a0a 2020 2020 2020         ]:.      
 0000b2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b300: 2020 2020 2020 2020 5d3a 0a20 2020 2020          ]:.     
-0000b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b320: 2020 2020 2020 2020 2020 2061 6767 7265             aggre
-0000b330: 6761 7469 6f6e 5f73 7472 203d 2061 6767  gation_str = agg
-0000b340: 5f63 6f6c 756d 6e5b 2261 6767 225d 0a20  _column["agg"]. 
-0000b350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b360: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000b370: 6167 675f 636f 6c75 6d6e 5b22 6167 6722  agg_column["agg"
-0000b380: 5d2e 6c6f 7765 7228 2920 696e 205b 226d  ].lower() in ["m
-0000b390: 6561 6e22 2c20 2261 7667 225d 3a0a 2020  ean", "avg"]:.  
-0000b3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3b0: 2020 2020 2020 2020 2020 2020 2020 6167                ag
-0000b3c0: 6772 6567 6174 696f 6e5f 7374 7220 3d20  gregation_str = 
-0000b3d0: 2261 7667 220a 2020 2020 2020 2020 2020  "avg".          
-0000b3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b3f0: 2020 656c 6966 2061 6767 5f63 6f6c 756d    elif agg_colum
-0000b400: 6e5b 2261 6767 225d 2e6c 6f77 6572 2829  n["agg"].lower()
-0000b410: 203d 3d20 2263 6f6e 6361 7422 3a0a 2020   == "concat":.  
-0000b420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b430: 2020 2020 2020 2020 2020 2020 2020 6167                ag
-0000b440: 6772 6567 6174 696f 6e5f 7374 7220 3d20  gregation_str = 
-0000b450: 2267 726f 7570 5f63 6f6e 6361 7422 0a20  "group_concat". 
-0000b460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b470: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000b480: 6620 2273 6570 2220 696e 2061 6767 5f63  f "sep" in agg_c
-0000b490: 6f6c 756d 6e3a 0a20 2020 2020 2020 2020  olumn:.         
-0000b4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b4b0: 2020 2020 2020 2020 2020 2065 7874 7261             extra
-0000b4c0: 5f70 6172 616d 5f73 7472 203d 2066 222c  _param_str = f",
-0000b4d0: 2027 7b61 6767 5f63 6f6c 756d 6e5b 2773   '{agg_column['s
-0000b4e0: 6570 275d 7d27 220a 2020 2020 2020 2020  ep']}'".        
+0000b300: 2020 2020 2020 2020 2020 6167 6772 6567            aggreg
+0000b310: 6174 696f 6e5f 7374 7220 3d20 6167 675f  ation_str = agg_
+0000b320: 636f 6c75 6d6e 5b22 6167 6722 5d0a 2020  column["agg"].  
+0000b330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b340: 2020 2020 2020 2020 2020 656c 6966 2061            elif a
+0000b350: 6767 5f63 6f6c 756d 6e5b 2261 6767 225d  gg_column["agg"]
+0000b360: 2e6c 6f77 6572 2829 2069 6e20 5b22 6d65  .lower() in ["me
+0000b370: 616e 222c 2022 6176 6722 5d3a 0a20 2020  an", "avg"]:.   
+0000b380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b390: 2020 2020 2020 2020 2020 2020 2061 6767               agg
+0000b3a0: 7265 6761 7469 6f6e 5f73 7472 203d 2022  regation_str = "
+0000b3b0: 6176 6722 0a20 2020 2020 2020 2020 2020  avg".           
+0000b3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b3d0: 2065 6c69 6620 6167 675f 636f 6c75 6d6e   elif agg_column
+0000b3e0: 5b22 6167 6722 5d2e 6c6f 7765 7228 2920  ["agg"].lower() 
+0000b3f0: 3d3d 2022 636f 6e63 6174 223a 0a20 2020  == "concat":.   
+0000b400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b410: 2020 2020 2020 2020 2020 2020 2061 6767               agg
+0000b420: 7265 6761 7469 6f6e 5f73 7472 203d 2022  regation_str = "
+0000b430: 6772 6f75 705f 636f 6e63 6174 220a 2020  group_concat".  
+0000b440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b450: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0000b460: 2022 7365 7022 2069 6e20 6167 675f 636f   "sep" in agg_co
+0000b470: 6c75 6d6e 3a0a 2020 2020 2020 2020 2020  lumn:.          
+0000b480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b490: 2020 2020 2020 2020 2020 6578 7472 615f            extra_
+0000b4a0: 7061 7261 6d5f 7374 7220 3d20 6622 2c20  param_str = f", 
+0000b4b0: 277b 6167 675f 636f 6c75 6d6e 5b27 7365  '{agg_column['se
+0000b4c0: 7027 5d7d 2722 0a20 2020 2020 2020 2020  p']}'".         
+0000b4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b4e0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
 0000b4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b500: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000b510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b520: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000b530: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-0000b540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b560: 6622 6167 6772 6567 6174 696f 6e20 7b61  f"aggregation {a
-0000b570: 6767 5f63 6f6c 756d 6e5b 2761 6767 275d  gg_column['agg']
-0000b580: 7d20 6973 206e 6f74 2073 7570 706f 7274  } is not support
-0000b590: 6564 220a 2020 2020 2020 2020 2020 2020  ed".            
+0000b500: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000b510: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+0000b520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b530: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000b540: 2261 6767 7265 6761 7469 6f6e 207b 6167  "aggregation {ag
+0000b550: 675f 636f 6c75 6d6e 5b27 6167 6727 5d7d  g_column['agg']}
+0000b560: 2069 7320 6e6f 7420 7375 7070 6f72 7465   is not supporte
+0000b570: 6422 0a20 2020 2020 2020 2020 2020 2020  d".             
+0000b580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b590: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
 0000b5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5b0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-0000b5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b5d0: 2020 2023 2049 6620 6469 7374 696e 6374     # If distinct
-0000b5e0: 2069 7320 7370 6563 6966 6965 642c 2061   is specified, a
-0000b5f0: 6464 2074 6865 2064 6973 7469 6e63 7420  dd the distinct 
-0000b600: 6b65 7977 6f72 640a 2020 2020 2020 2020  keyword.        
+0000b5b0: 2020 2320 4966 2064 6973 7469 6e63 7420    # If distinct 
+0000b5c0: 6973 2073 7065 6369 6669 6564 2c20 6164  is specified, ad
+0000b5d0: 6420 7468 6520 6469 7374 696e 6374 206b  d the distinct k
+0000b5e0: 6579 776f 7264 0a20 2020 2020 2020 2020  eyword.         
+0000b5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b600: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
 0000b610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b620: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
-0000b630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b640: 2020 2020 2020 2020 2022 6469 7374 696e           "distin
-0000b650: 6374 2220 696e 2061 6767 5f63 6f6c 756d  ct" in agg_colum
-0000b660: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-0000b670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b680: 2020 616e 6420 6167 675f 636f 6c75 6d6e    and agg_column
-0000b690: 5b22 6469 7374 696e 6374 225d 2069 7320  ["distinct"] is 
-0000b6a0: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+0000b620: 2020 2020 2020 2020 2264 6973 7469 6e63          "distinc
+0000b630: 7422 2069 6e20 6167 675f 636f 6c75 6d6e  t" in agg_column
+0000b640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b660: 2061 6e64 2061 6767 5f63 6f6c 756d 6e5b   and agg_column[
+0000b670: 2264 6973 7469 6e63 7422 5d20 6973 2054  "distinct"] is T
+0000b680: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0000b690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
 0000b6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6c0: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
-0000b6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6e0: 2020 2020 6469 7374 696e 6374 5f73 7472      distinct_str
-0000b6f0: 203d 2022 4449 5354 494e 4354 2022 0a0a   = "DISTINCT "..
-0000b700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b710: 2020 2020 2020 2020 2020 2020 2320 5072              # Pr
-0000b720: 6570 6172 6520 636f 6c75 6d6e 206e 616d  epare column nam
-0000b730: 6520 7374 7269 6e67 2e0a 2020 2020 2020  e string..      
-0000b740: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b750: 2020 2020 2020 636f 6c75 6d6e 5f73 7472        column_str
-0000b760: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-0000b770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b780: 2020 2020 2022 6a73 6f6e 5f65 7874 7261       "json_extra
-0000b790: 6374 286a 736f 6e5f 6461 7461 2e6a 736f  ct(json_data.jso
-0000b7a0: 6e5f 726f 772c 2022 0a20 2020 2020 2020  n_row, ".       
-0000b7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b7c0: 2020 2020 2020 2020 2066 2722 242e 7b61           f'"$.{a
-0000b7d0: 6767 5f63 6f6c 756d 6e5b 2263 6f6c 756d  gg_column["colum
-0000b7e0: 6e22 5d7d 2229 270a 2020 2020 2020 2020  n"]}")'.        
+0000b6c0: 2020 2064 6973 7469 6e63 745f 7374 7220     distinct_str 
+0000b6d0: 3d20 2244 4953 5449 4e43 5420 220a 0a20  = "DISTINCT ".. 
+0000b6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b6f0: 2020 2020 2020 2020 2020 2023 2050 7265             # Pre
+0000b700: 7061 7265 2063 6f6c 756d 6e20 6e61 6d65  pare column name
+0000b710: 2073 7472 696e 672e 0a20 2020 2020 2020   string..       
+0000b720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b730: 2020 2020 2063 6f6c 756d 6e5f 7374 7220       column_str 
+0000b740: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
+0000b750: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b760: 2020 2020 226a 736f 6e5f 6578 7472 6163      "json_extrac
+0000b770: 7428 6a73 6f6e 5f64 6174 612e 6a73 6f6e  t(json_data.json
+0000b780: 5f72 6f77 2c20 220a 2020 2020 2020 2020  _row, ".        
+0000b790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7a0: 2020 2020 2020 2020 6627 2224 2e7b 6167          f'"$.{ag
+0000b7b0: 675f 636f 6c75 6d6e 5b22 636f 6c75 6d6e  g_column["column
+0000b7c0: 225d 7d22 2927 0a20 2020 2020 2020 2020  "]}")'.         
+0000b7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b7e0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
 0000b7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b800: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-0000b810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b820: 2020 2023 204e 6f77 2070 7574 2065 7665     # Now put eve
-0000b830: 7279 7468 696e 6720 746f 6765 7468 6572  rything together
-0000b840: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b850: 2020 2020 2020 2020 2020 2020 2061 6767               agg
-0000b860: 5f63 6f6c 756d 6e73 5f73 7472 202b 3d20  _columns_str += 
-0000b870: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000b880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b890: 2020 6622 2c20 7b61 6767 7265 6761 7469    f", {aggregati
-0000b8a0: 6f6e 5f73 7472 7d28 7b64 6973 7469 6e63  on_str}({distinc
-0000b8b0: 745f 7374 727d 7b63 6f6c 756d 6e5f 7374  t_str}{column_st
-0000b8c0: 727d 220a 2020 2020 2020 2020 2020 2020  r}".            
-0000b8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b8e0: 2020 2020 6627 7b65 7874 7261 5f70 6172      f'{extra_par
-0000b8f0: 616d 5f73 7472 7d29 2041 5320 227b 6167  am_str}) AS "{ag
-0000b900: 675f 636f 6c75 6d6e 5b22 6173 225d 7d22  g_column["as"]}"
-0000b910: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
-0000b920: 2020 2020 2020 2020 2020 2020 2020 290a                ).
-0000b930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b940: 2023 2041 6464 2061 2063 6f6c 756d 6e20   # Add a column 
-0000b950: 746f 206f 7264 6572 2074 6865 2072 6573  to order the res
-0000b960: 756c 7420 6279 2074 6f20 6576 6164 6520  ult by to evade 
-0000b970: 6861 7669 6e67 2061 6c6c 0a20 2020 2020  having all.     
-0000b980: 2020 2020 2020 2020 2020 2023 2063 6f6d             # com
-0000b990: 706c 6578 2067 656f 6d65 7472 6965 7320  plex geometries 
-0000b9a0: 746f 6765 7468 6572 2069 6e20 7468 6520  together in the 
-0000b9b0: 6f75 7470 7574 2066 696c 652e 0a20 2020  output file..   
-0000b9c0: 2020 2020 2020 2020 2020 2020 206f 7264               ord
-0000b9d0: 6572 6279 5f63 6f6c 756d 6e20 3d20 2274  erby_column = "t
-0000b9e0: 656d 705f 6f72 6465 7263 6f6c 756d 6e5f  emp_ordercolumn_
-0000b9f0: 6765 6f68 6173 6822 0a20 2020 2020 2020  geohash".       
-0000ba00: 2020 2020 2020 2020 205f 6164 645f 6f72           _add_or
-0000ba10: 6465 7262 795f 636f 6c75 6d6e 280a 2020  derby_column(.  
-0000ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba30: 2020 7061 7468 3d6f 7574 7075 745f 746d    path=output_tm
-0000ba40: 705f 7061 7468 2c20 6c61 7965 723d 6f75  p_path, layer=ou
-0000ba50: 7470 7574 5f6c 6179 6572 2c20 6e61 6d65  tput_layer, name
-0000ba60: 3d6f 7264 6572 6279 5f63 6f6c 756d 6e0a  =orderby_column.
-0000ba70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba80: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
-0000ba90: 2020 2023 2050 7265 7061 7265 2053 514c     # Prepare SQL
-0000baa0: 2073 7461 7465 6d65 6e74 2066 6f72 2066   statement for f
-0000bab0: 696e 616c 206f 7574 7075 7420 6669 6c65  inal output file
-0000bac0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bad0: 2020 2320 416c 6c20 7469 6c65 7320 6172    # All tiles ar
-0000bae0: 6520 616c 7265 6164 7920 6469 7373 6f6c  e already dissol
-0000baf0: 7665 6420 746f 2067 726f 7570 732c 2062  ved to groups, b
-0000bb00: 7574 206e 6f77 2074 6865 0a20 2020 2020  ut now the.     
-0000bb10: 2020 2020 2020 2020 2020 2023 2072 6573             # res
-0000bb20: 756c 7473 2066 726f 6d20 616c 6c20 7469  ults from all ti
-0000bb30: 6c65 7320 7374 696c 6c20 6e65 6564 2074  les still need t
-0000bb40: 6f20 6265 0a20 2020 2020 2020 2020 2020  o be.           
-0000bb50: 2020 2020 2023 2067 726f 7570 6564 2f63       # grouped/c
-0000bb60: 6f6c 6c65 6374 6564 2074 6f67 6574 6865  ollected togethe
-0000bb70: 722e 0a20 2020 2020 2020 2020 2020 2020  r..             
-0000bb80: 2020 206c 6f67 6765 722e 696e 666f 2822     logger.info("
-0000bb90: 506f 7374 7072 6f63 6573 7320 7072 6570  Postprocess prep
-0000bba0: 6172 6564 2066 6561 7475 7265 732e 2e2e  ared features...
-0000bbb0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0000bbc0: 2020 2069 6620 6167 675f 636f 6c75 6d6e     if agg_column
-0000bbd0: 7320 6973 204e 6f6e 653a 0a20 2020 2020  s is None:.     
-0000bbe0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000bbf0: 2049 6620 7468 6572 6520 6172 6520 6e6f   If there are no
-0000bc00: 2061 6767 7265 6761 7469 6f6e 2063 6f6c   aggregation col
-0000bc10: 756d 6e73 2c20 7468 696e 6773 2061 7265  umns, things are
-0000bc20: 206e 6f74 2074 6f6f 0a20 2020 2020 2020   not too.       
-0000bc30: 2020 2020 2020 2020 2020 2020 2023 2063               # c
-0000bc40: 6f6d 706c 6963 6174 6564 2e0a 2020 2020  omplicated..    
-0000bc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc60: 6966 2065 7870 6c6f 6465 636f 6c6c 6563  if explodecollec
-0000bc70: 7469 6f6e 7320 6973 2054 7275 653a 0a20  tions is True:. 
-0000bc80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc90: 2020 2020 2020 2023 2049 6620 6578 706c         # If expl
-0000bca0: 6f64 6563 6f6c 6c65 6374 696f 6e73 2069  odecollections i
-0000bcb0: 7320 7472 7565 2c20 6974 2069 7320 7573  s true, it is us
-0000bcc0: 656c 6573 7320 746f 0a20 2020 2020 2020  eless to.       
-0000bcd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bce0: 2023 2066 6972 7374 2067 726f 7570 2074   # first group t
-0000bcf0: 6865 6d20 6865 7265 2c20 6173 2074 6865  hem here, as the
-0000bd00: 7920 7769 6c6c 2062 6520 6578 706c 6f64  y will be explod
-0000bd10: 6564 2061 6761 696e 0a20 2020 2020 2020  ed again.       
-0000bd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd30: 2023 2069 6e20 7468 6520 7365 6c65 6374   # in the select
-0000bd40: 2829 2063 616c 6c20 6c61 7465 7220 6f6e  () call later on
-0000bd50: 2e2e 2e20 736f 206a 7573 7420 6f72 6465  ... so just orde
-0000bd60: 7220 7468 656d 2e0a 2020 2020 2020 2020  r them..        
-0000bd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bd80: 2320 4966 2061 2074 696c 6564 2072 6573  # If a tiled res
-0000bd90: 756c 7420 6973 2061 736b 6564 2c20 616c  ult is asked, al
-0000bda0: 736f 2064 6f6e 2774 2063 6f6c 6c65 6374  so don't collect
-0000bdb0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000bdc0: 2020 2020 2020 2020 2020 7371 6c5f 7374            sql_st
-0000bdd0: 6d74 203d 2066 2222 220a 2020 2020 2020  mt = f""".      
-0000bde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bdf0: 2020 2020 2020 5345 4c45 4354 207b 7b67        SELECT {{g
-0000be00: 656f 6d65 7472 7963 6f6c 756d 6e7d 7d0a  eometrycolumn}}.
-0000be10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be30: 2020 7b67 726f 7570 6279 5f73 656c 6563    {groupby_selec
-0000be40: 745f 7072 6566 6978 6564 5f73 7472 2e66  t_prefixed_str.f
-0000be50: 6f72 6d61 7428 7072 6566 6978 3d22 6c61  ormat(prefix="la
-0000be60: 7965 722e 2229 7d0a 2020 2020 2020 2020  yer.")}.        
-0000be70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000be80: 2020 2020 2020 4652 4f4d 2022 7b7b 696e        FROM "{{in
-0000be90: 7075 745f 6c61 7965 727d 7d22 206c 6179  put_layer}}" lay
-0000bea0: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
-0000beb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bec0: 4f52 4445 5220 4259 206c 6179 6572 2e7b  ORDER BY layer.{
-0000bed0: 6f72 6465 7262 795f 636f 6c75 6d6e 7d0a  orderby_column}.
-0000bee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bef0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000bf00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bf10: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000bf20: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000bf30: 4e6f 2065 7870 6c6f 6465 636f 6c6c 6563  No explodecollec
-0000bf40: 7469 6f6e 732c 2073 6f20 636f 6c6c 6563  tions, so collec
-0000bf50: 7420 746f 206f 6e65 2067 656f 6d65 7472  t to one geometr
-0000bf60: 790a 2020 2020 2020 2020 2020 2020 2020  y.              
-0000bf70: 2020 2020 2020 2020 2020 2320 2870 6572            # (per
-0000bf80: 2067 726f 7570 6279 2069 6620 6170 706c   groupby if appl
-0000bf90: 6963 6162 6c65 292e 0a20 2020 2020 2020  icable)..       
+0000b800: 2020 2320 4e6f 7720 7075 7420 6576 6572    # Now put ever
+0000b810: 7974 6869 6e67 2074 6f67 6574 6865 720a  ything together.
+0000b820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b830: 2020 2020 2020 2020 2020 2020 6167 675f              agg_
+0000b840: 636f 6c75 6d6e 735f 7374 7220 2b3d 2028  columns_str += (
+0000b850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b870: 2066 222c 207b 6167 6772 6567 6174 696f   f", {aggregatio
+0000b880: 6e5f 7374 727d 287b 6469 7374 696e 6374  n_str}({distinct
+0000b890: 5f73 7472 7d7b 636f 6c75 6d6e 5f73 7472  _str}{column_str
+0000b8a0: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+0000b8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b8c0: 2020 2066 277b 6578 7472 615f 7061 7261     f'{extra_para
+0000b8d0: 6d5f 7374 727d 2920 4153 2022 7b61 6767  m_str}) AS "{agg
+0000b8e0: 5f63 6f6c 756d 6e5b 2261 7322 5d7d 2227  _column["as"]}"'
+0000b8f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b900: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
+0000b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b920: 2320 4164 6420 6120 636f 6c75 6d6e 2074  # Add a column t
+0000b930: 6f20 6f72 6465 7220 7468 6520 7265 7375  o order the resu
+0000b940: 6c74 2062 7920 746f 2065 7661 6465 2068  lt by to evade h
+0000b950: 6176 696e 6720 616c 6c0a 2020 2020 2020  aving all.      
+0000b960: 2020 2020 2020 2020 2020 2320 636f 6d70            # comp
+0000b970: 6c65 7820 6765 6f6d 6574 7269 6573 2074  lex geometries t
+0000b980: 6f67 6574 6865 7220 696e 2074 6865 206f  ogether in the o
+0000b990: 7574 7075 7420 6669 6c65 2e0a 2020 2020  utput file..    
+0000b9a0: 2020 2020 2020 2020 2020 2020 6f72 6465              orde
+0000b9b0: 7262 795f 636f 6c75 6d6e 203d 2022 7465  rby_column = "te
+0000b9c0: 6d70 5f6f 7264 6572 636f 6c75 6d6e 5f67  mp_ordercolumn_g
+0000b9d0: 656f 6861 7368 220a 2020 2020 2020 2020  eohash".        
+0000b9e0: 2020 2020 2020 2020 5f61 6464 5f6f 7264          _add_ord
+0000b9f0: 6572 6279 5f63 6f6c 756d 6e28 0a20 2020  erby_column(.   
+0000ba00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba10: 2070 6174 683d 6f75 7470 7574 5f74 6d70   path=output_tmp
+0000ba20: 5f70 6174 682c 206c 6179 6572 3d6f 7574  _path, layer=out
+0000ba30: 7075 745f 6c61 7965 722c 206e 616d 653d  put_layer, name=
+0000ba40: 6f72 6465 7262 795f 636f 6c75 6d6e 0a20  orderby_column. 
+0000ba50: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000ba60: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000ba70: 2020 2320 5072 6570 6172 6520 5351 4c20    # Prepare SQL 
+0000ba80: 7374 6174 656d 656e 7420 666f 7220 6669  statement for fi
+0000ba90: 6e61 6c20 6f75 7470 7574 2066 696c 652e  nal output file.
+0000baa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bab0: 2023 2041 6c6c 2074 696c 6573 2061 7265   # All tiles are
+0000bac0: 2061 6c72 6561 6479 2064 6973 736f 6c76   already dissolv
+0000bad0: 6564 2074 6f20 6772 6f75 7073 2c20 6275  ed to groups, bu
+0000bae0: 7420 6e6f 7720 7468 650a 2020 2020 2020  t now the.      
+0000baf0: 2020 2020 2020 2020 2020 2320 7265 7375            # resu
+0000bb00: 6c74 7320 6672 6f6d 2061 6c6c 2074 696c  lts from all til
+0000bb10: 6573 2073 7469 6c6c 206e 6565 6420 746f  es still need to
+0000bb20: 2062 650a 2020 2020 2020 2020 2020 2020   be.            
+0000bb30: 2020 2020 2320 6772 6f75 7065 642f 636f      # grouped/co
+0000bb40: 6c6c 6563 7465 6420 746f 6765 7468 6572  llected together
+0000bb50: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000bb60: 2020 6c6f 6767 6572 2e69 6e66 6f28 2250    logger.info("P
+0000bb70: 6f73 7470 726f 6365 7373 2070 7265 7061  ostprocess prepa
+0000bb80: 7265 6420 6665 6174 7572 6573 2e2e 2e22  red features..."
+0000bb90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000bba0: 2020 6966 2061 6767 5f63 6f6c 756d 6e73    if agg_columns
+0000bbb0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000bbc0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000bbd0: 4966 2074 6865 7265 2061 7265 206e 6f20  If there are no 
+0000bbe0: 6167 6772 6567 6174 696f 6e20 636f 6c75  aggregation colu
+0000bbf0: 6d6e 732c 2074 6869 6e67 7320 6172 6520  mns, things are 
+0000bc00: 6e6f 7420 746f 6f0a 2020 2020 2020 2020  not too.        
+0000bc10: 2020 2020 2020 2020 2020 2020 2320 636f              # co
+0000bc20: 6d70 6c69 6361 7465 642e 0a20 2020 2020  mplicated..     
+0000bc30: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000bc40: 6620 6578 706c 6f64 6563 6f6c 6c65 6374  f explodecollect
+0000bc50: 696f 6e73 2069 7320 5472 7565 3a0a 2020  ions is True:.  
+0000bc60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bc70: 2020 2020 2020 2320 4966 2065 7870 6c6f        # If explo
+0000bc80: 6465 636f 6c6c 6563 7469 6f6e 7320 6973  decollections is
+0000bc90: 2074 7275 652c 2069 7420 6973 2075 7365   true, it is use
+0000bca0: 6c65 7373 2074 6f0a 2020 2020 2020 2020  less to.        
+0000bcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bcc0: 2320 6669 7273 7420 6772 6f75 7020 7468  # first group th
+0000bcd0: 656d 2068 6572 652c 2061 7320 7468 6579  em here, as they
+0000bce0: 2077 696c 6c20 6265 2065 7870 6c6f 6465   will be explode
+0000bcf0: 6420 6167 6169 6e0a 2020 2020 2020 2020  d again.        
+0000bd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bd10: 2320 696e 2074 6865 2073 656c 6563 7428  # in the select(
+0000bd20: 2920 6361 6c6c 206c 6174 6572 206f 6e2e  ) call later on.
+0000bd30: 2e2e 2073 6f20 6a75 7374 206f 7264 6572  .. so just order
+0000bd40: 2074 6865 6d2e 0a20 2020 2020 2020 2020   them..         
+0000bd50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000bd60: 2049 6620 6120 7469 6c65 6420 7265 7375   If a tiled resu
+0000bd70: 6c74 2069 7320 6173 6b65 642c 2061 6c73  lt is asked, als
+0000bd80: 6f20 646f 6e27 7420 636f 6c6c 6563 742e  o don't collect.
+0000bd90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bda0: 2020 2020 2020 2020 2073 716c 5f73 746d           sql_stm
+0000bdb0: 7420 3d20 6622 2222 0a20 2020 2020 2020  t = f""".       
+0000bdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bdd0: 2020 2020 2053 454c 4543 5420 7b7b 6765       SELECT {{ge
+0000bde0: 6f6d 6574 7279 636f 6c75 6d6e 7d7d 0a20  ometrycolumn}}. 
+0000bdf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be10: 207b 6772 6f75 7062 795f 7365 6c65 6374   {groupby_select
+0000be20: 5f70 7265 6669 7865 645f 7374 722e 666f  _prefixed_str.fo
+0000be30: 726d 6174 2870 7265 6669 783d 226c 6179  rmat(prefix="lay
+0000be40: 6572 2e22 297d 0a20 2020 2020 2020 2020  er.")}.         
+0000be50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000be60: 2020 2020 2046 524f 4d20 227b 7b69 6e70       FROM "{{inp
+0000be70: 7574 5f6c 6179 6572 7d7d 2220 6c61 7965  ut_layer}}" laye
+0000be80: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+0000be90: 2020 2020 2020 2020 2020 2020 2020 204f                 O
+0000bea0: 5244 4552 2042 5920 6c61 7965 722e 7b6f  RDER BY layer.{o
+0000beb0: 7264 6572 6279 5f63 6f6c 756d 6e7d 0a20  rderby_column}. 
+0000bec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bed0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000bee0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000bef0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000bf00: 2020 2020 2020 2020 2020 2020 2023 204e               # N
+0000bf10: 6f20 6578 706c 6f64 6563 6f6c 6c65 6374  o explodecollect
+0000bf20: 696f 6e73 2c20 736f 2063 6f6c 6c65 6374  ions, so collect
+0000bf30: 2074 6f20 6f6e 6520 6765 6f6d 6574 7279   to one geometry
+0000bf40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bf50: 2020 2020 2020 2020 2023 2028 7065 7220           # (per 
+0000bf60: 6772 6f75 7062 7920 6966 2061 7070 6c69  groupby if appli
+0000bf70: 6361 626c 6529 2e0a 2020 2020 2020 2020  cable)..        
+0000bf80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf90: 7371 6c5f 7374 6d74 203d 2066 2222 220a  sql_stmt = f""".
 0000bfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bfb0: 2073 716c 5f73 746d 7420 3d20 6622 2222   sql_stmt = f"""
-0000bfc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000bfd0: 2020 2020 2020 2020 2020 2020 2053 454c               SEL
-0000bfe0: 4543 5420 5354 5f43 6f6c 6c65 6374 287b  ECT ST_Collect({
-0000bff0: 7b67 656f 6d65 7472 7963 6f6c 756d 6e7d  {geometrycolumn}
-0000c000: 7d29 2041 5320 7b7b 6765 6f6d 6574 7279  }) AS {{geometry
-0000c010: 636f 6c75 6d6e 7d7d 0a20 2020 2020 2020  column}}.       
-0000c020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c030: 2020 2020 2020 2020 2020 207b 6772 6f75             {grou
-0000c040: 7062 795f 7365 6c65 6374 5f70 7265 6669  pby_select_prefi
-0000c050: 7865 645f 7374 722e 666f 726d 6174 2870  xed_str.format(p
-0000c060: 7265 6669 783d 226c 6179 6572 2e22 297d  refix="layer.")}
-0000c070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c080: 2020 2020 2020 2020 2020 2020 2020 2046                 F
-0000c090: 524f 4d20 227b 7b69 6e70 7574 5f6c 6179  ROM "{{input_lay
-0000c0a0: 6572 7d7d 2220 6c61 7965 720a 2020 2020  er}}" layer.    
-0000c0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0c0: 2020 2020 2020 2020 2020 7b67 726f 7570            {group
-0000c0d0: 6279 5f67 726f 7570 6279 5f70 7265 6669  by_groupby_prefi
-0000c0e0: 7865 645f 7374 722e 666f 726d 6174 2870  xed_str.format(p
-0000c0f0: 7265 6669 783d 226c 6179 6572 2e22 297d  refix="layer.")}
-0000c100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c110: 2020 2020 2020 2020 2020 2020 2020 4f52                OR
-0000c120: 4445 5220 4259 204d 494e 286c 6179 6572  DER BY MIN(layer
-0000c130: 2e7b 6f72 6465 7262 795f 636f 6c75 6d6e  .{orderby_column
-0000c140: 7d29 0a20 2020 2020 2020 2020 2020 2020  }).             
-0000c150: 2020 2020 2020 2020 2020 2022 2222 0a20             """. 
-0000c160: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000c170: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000c180: 2020 2020 2020 2020 2023 2049 6620 6167           # If ag
-0000c190: 675f 636f 6c75 6d6e 7320 7370 6563 6966  g_columns specif
-0000c1a0: 6965 642c 2070 6f73 7470 726f 6365 7373  ied, postprocess
-0000c1b0: 696e 6720 6973 2061 2062 6974 206d 6f72  ing is a bit mor
-0000c1c0: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000c1d0: 2020 2020 2020 2320 636f 6d70 6c69 6361        # complica
-0000c1e0: 7465 642e 0a20 2020 2020 2020 2020 2020  ted..           
-0000c1f0: 2020 2020 2020 2020 2073 716c 5f73 746d           sql_stm
-0000c200: 7420 3d20 6622 2222 0a20 2020 2020 2020  t = f""".       
-0000c210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c220: 2053 454c 4543 5420 6765 6f5f 6461 7461   SELECT geo_data
-0000c230: 2e7b 7b67 656f 6d65 7472 7963 6f6c 756d  .{{geometrycolum
-0000c240: 6e7d 7d0a 2020 2020 2020 2020 2020 2020  n}}.            
-0000c250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c260: 2020 7b67 726f 7570 6279 5f73 656c 6563    {groupby_selec
-0000c270: 745f 7072 6566 6978 6564 5f73 7472 2e66  t_prefixed_str.f
-0000c280: 6f72 6d61 7428 7072 6566 6978 3d22 6765  ormat(prefix="ge
-0000c290: 6f5f 6461 7461 2e22 297d 0a20 2020 2020  o_data.")}.     
-0000c2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2b0: 2020 2020 2020 2020 207b 6167 675f 636f           {agg_co
-0000c2c0: 6c75 6d6e 735f 7374 727d 0a20 2020 2020  lumns_str}.     
+0000bfb0: 2020 2020 2020 2020 2020 2020 5345 4c45              SELE
+0000bfc0: 4354 2053 545f 436f 6c6c 6563 7428 7b7b  CT ST_Collect({{
+0000bfd0: 6765 6f6d 6574 7279 636f 6c75 6d6e 7d7d  geometrycolumn}}
+0000bfe0: 2920 4153 207b 7b67 656f 6d65 7472 7963  ) AS {{geometryc
+0000bff0: 6f6c 756d 6e7d 7d0a 2020 2020 2020 2020  olumn}}.        
+0000c000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c010: 2020 2020 2020 2020 2020 7b67 726f 7570            {group
+0000c020: 6279 5f73 656c 6563 745f 7072 6566 6978  by_select_prefix
+0000c030: 6564 5f73 7472 2e66 6f72 6d61 7428 7072  ed_str.format(pr
+0000c040: 6566 6978 3d22 6c61 7965 722e 2229 7d0a  efix="layer.")}.
+0000c050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c060: 2020 2020 2020 2020 2020 2020 2020 4652                FR
+0000c070: 4f4d 2022 7b7b 696e 7075 745f 6c61 7965  OM "{{input_laye
+0000c080: 727d 7d22 206c 6179 6572 0a20 2020 2020  r}}" layer.     
+0000c090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0a0: 2020 2020 2020 2020 207b 6772 6f75 7062           {groupb
+0000c0b0: 795f 6772 6f75 7062 795f 7072 6566 6978  y_groupby_prefix
+0000c0c0: 6564 5f73 7472 2e66 6f72 6d61 7428 7072  ed_str.format(pr
+0000c0d0: 6566 6978 3d22 6c61 7965 722e 2229 7d0a  efix="layer.")}.
+0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c0f0: 2020 2020 2020 2020 2020 2020 204f 5244               ORD
+0000c100: 4552 2042 5920 4d49 4e28 6c61 7965 722e  ER BY MIN(layer.
+0000c110: 7b6f 7264 6572 6279 5f63 6f6c 756d 6e7d  {orderby_column}
+0000c120: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000c130: 2020 2020 2020 2020 2020 2222 220a 2020            """.  
+0000c140: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000c150: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000c160: 2020 2020 2020 2020 2320 4966 2061 6767          # If agg
+0000c170: 5f63 6f6c 756d 6e73 2073 7065 6369 6669  _columns specifi
+0000c180: 6564 2c20 706f 7374 7072 6f63 6573 7369  ed, postprocessi
+0000c190: 6e67 2069 7320 6120 6269 7420 6d6f 7265  ng is a bit more
+0000c1a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c1b0: 2020 2020 2023 2063 6f6d 706c 6963 6174       # complicat
+0000c1c0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+0000c1d0: 2020 2020 2020 2020 7371 6c5f 7374 6d74          sql_stmt
+0000c1e0: 203d 2066 2222 220a 2020 2020 2020 2020   = f""".        
+0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c200: 5345 4c45 4354 2067 656f 5f64 6174 612e  SELECT geo_data.
+0000c210: 7b7b 6765 6f6d 6574 7279 636f 6c75 6d6e  {{geometrycolumn
+0000c220: 7d7d 0a20 2020 2020 2020 2020 2020 2020  }}.             
+0000c230: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c240: 207b 6772 6f75 7062 795f 7365 6c65 6374   {groupby_select
+0000c250: 5f70 7265 6669 7865 645f 7374 722e 666f  _prefixed_str.fo
+0000c260: 726d 6174 2870 7265 6669 783d 2267 656f  rmat(prefix="geo
+0000c270: 5f64 6174 612e 2229 7d0a 2020 2020 2020  _data.")}.      
+0000c280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c290: 2020 2020 2020 2020 7b61 6767 5f63 6f6c          {agg_col
+0000c2a0: 756d 6e73 5f73 7472 7d0a 2020 2020 2020  umns_str}.      
+0000c2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c2c0: 2020 2020 4652 4f4d 2028 0a20 2020 2020      FROM (.     
 0000c2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c2e0: 2020 2020 2046 524f 4d20 280a 2020 2020       FROM (.    
-0000c2f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c300: 2020 2020 2020 2020 5345 4c45 4354 2053          SELECT S
-0000c310: 545f 436f 6c6c 6563 7428 6c61 7965 725f  T_Collect(layer_
-0000c320: 6765 6f2e 7b7b 6765 6f6d 6574 7279 636f  geo.{{geometryco
-0000c330: 6c75 6d6e 7d7d 0a20 2020 2020 2020 2020  lumn}}.         
-0000c340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c350: 2020 2020 2020 2020 2020 2920 4153 207b            ) AS {
-0000c360: 7b67 656f 6d65 7472 7963 6f6c 756d 6e7d  {geometrycolumn}
-0000c370: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c390: 2020 2020 7b67 726f 7570 6279 5f73 656c      {groupby_sel
-0000c3a0: 6563 745f 7072 6566 6978 6564 5f73 7472  ect_prefixed_str
-0000c3b0: 2e66 6f72 6d61 7428 7072 6566 6978 3d22  .format(prefix="
-0000c3c0: 6c61 7965 725f 6765 6f2e 2229 7d0a 2020  layer_geo.")}.  
-0000c3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3f0: 2c4d 494e 286c 6179 6572 5f67 656f 2e7b  ,MIN(layer_geo.{
-0000c400: 6f72 6465 7262 795f 636f 6c75 6d6e 7d29  orderby_column})
-0000c410: 2061 7320 7b6f 7264 6572 6279 5f63 6f6c   as {orderby_col
-0000c420: 756d 6e7d 0a20 2020 2020 2020 2020 2020  umn}.           
-0000c430: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c440: 2020 2046 524f 4d20 227b 7b69 6e70 7574     FROM "{{input
-0000c450: 5f6c 6179 6572 7d7d 2220 6c61 7965 725f  _layer}}" layer_
-0000c460: 6765 6f0a 2020 2020 2020 2020 2020 2020  geo.            
-0000c470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c480: 2020 7b67 726f 7570 6279 5f67 726f 7570    {groupby_group
-0000c490: 6279 5f70 7265 6669 7865 645f 7374 722e  by_prefixed_str.
-0000c4a0: 666f 726d 6174 2870 7265 6669 783d 226c  format(prefix="l
-0000c4b0: 6179 6572 5f67 656f 2e22 297d 0a20 2020  ayer_geo.")}.   
-0000c4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4d0: 2020 2020 2020 2020 2029 2067 656f 5f64           ) geo_d
-0000c4e0: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
-0000c4f0: 2020 2020 2020 2020 2020 2020 2020 4a4f                JO
-0000c500: 494e 2028 0a20 2020 2020 2020 2020 2020  IN (.           
-0000c510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c520: 2053 454c 4543 5420 4449 5354 494e 4354   SELECT DISTINCT
-0000c530: 206a 736f 6e5f 726f 7773 5f74 6162 6c65   json_rows_table
-0000c540: 2e76 616c 7565 2061 7320 6a73 6f6e 5f72  .value as json_r
-0000c550: 6f77 0a20 2020 2020 2020 2020 2020 2020  ow.             
-0000c560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c570: 2020 207b 6772 6f75 7062 795f 7365 6c65     {groupby_sele
-0000c580: 6374 5f70 7265 6669 7865 645f 7374 722e  ct_prefixed_str.
-0000c590: 666f 726d 6174 2870 7265 6669 783d 226c  format(prefix="l
-0000c5a0: 6179 6572 5f66 6f72 5f6a 736f 6e2e 2229  ayer_for_json.")
-0000c5b0: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000c5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5d0: 4652 4f4d 2022 7b7b 696e 7075 745f 6c61  FROM "{{input_la
-0000c5e0: 7965 727d 7d22 206c 6179 6572 5f66 6f72  yer}}" layer_for
-0000c5f0: 5f6a 736f 6e0a 2020 2020 2020 2020 2020  _json.          
-0000c600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c610: 2020 2020 4352 4f53 5320 4a4f 494e 206a      CROSS JOIN j
-0000c620: 736f 6e5f 6561 6368 280a 2020 2020 2020  son_each(.      
-0000c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c640: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
-0000c650: 725f 666f 725f 6a73 6f6e 2e5f 5f44 4953  r_for_json.__DIS
-0000c660: 534f 4c56 455f 544f 4a53 4f4e 2c20 2224  SOLVE_TOJSON, "$
-0000c670: 2229 206a 736f 6e5f 726f 7773 5f74 6162  ") json_rows_tab
-0000c680: 6c65 0a20 2020 2020 2020 2020 2020 2020  le.             
-0000c690: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000c6a0: 206a 736f 6e5f 6461 7461 0a20 2020 2020   json_data.     
+0000c2e0: 2020 2020 2020 2053 454c 4543 5420 5354         SELECT ST
+0000c2f0: 5f43 6f6c 6c65 6374 286c 6179 6572 5f67  _Collect(layer_g
+0000c300: 656f 2e7b 7b67 656f 6d65 7472 7963 6f6c  eo.{{geometrycol
+0000c310: 756d 6e7d 7d0a 2020 2020 2020 2020 2020  umn}}.          
+0000c320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c330: 2020 2020 2020 2020 2029 2041 5320 7b7b           ) AS {{
+0000c340: 6765 6f6d 6574 7279 636f 6c75 6d6e 7d7d  geometrycolumn}}
+0000c350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c370: 2020 207b 6772 6f75 7062 795f 7365 6c65     {groupby_sele
+0000c380: 6374 5f70 7265 6669 7865 645f 7374 722e  ct_prefixed_str.
+0000c390: 666f 726d 6174 2870 7265 6669 783d 226c  format(prefix="l
+0000c3a0: 6179 6572 5f67 656f 2e22 297d 0a20 2020  ayer_geo.")}.   
+0000c3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c3c0: 2020 2020 2020 2020 2020 2020 2020 202c                 ,
+0000c3d0: 4d49 4e28 6c61 7965 725f 6765 6f2e 7b6f  MIN(layer_geo.{o
+0000c3e0: 7264 6572 6279 5f63 6f6c 756d 6e7d 2920  rderby_column}) 
+0000c3f0: 6173 207b 6f72 6465 7262 795f 636f 6c75  as {orderby_colu
+0000c400: 6d6e 7d0a 2020 2020 2020 2020 2020 2020  mn}.            
+0000c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c420: 2020 4652 4f4d 2022 7b7b 696e 7075 745f    FROM "{{input_
+0000c430: 6c61 7965 727d 7d22 206c 6179 6572 5f67  layer}}" layer_g
+0000c440: 656f 0a20 2020 2020 2020 2020 2020 2020  eo.             
+0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c460: 207b 6772 6f75 7062 795f 6772 6f75 7062   {groupby_groupb
+0000c470: 795f 7072 6566 6978 6564 5f73 7472 2e66  y_prefixed_str.f
+0000c480: 6f72 6d61 7428 7072 6566 6978 3d22 6c61  ormat(prefix="la
+0000c490: 7965 725f 6765 6f2e 2229 7d0a 2020 2020  yer_geo.")}.    
+0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c4b0: 2020 2020 2020 2020 2920 6765 6f5f 6461          ) geo_da
+0000c4c0: 7461 0a20 2020 2020 2020 2020 2020 2020  ta.             
+0000c4d0: 2020 2020 2020 2020 2020 2020 204a 4f49               JOI
+0000c4e0: 4e20 280a 2020 2020 2020 2020 2020 2020  N (.            
+0000c4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c500: 5345 4c45 4354 2044 4953 5449 4e43 5420  SELECT DISTINCT 
+0000c510: 6a73 6f6e 5f72 6f77 735f 7461 626c 652e  json_rows_table.
+0000c520: 7661 6c75 6520 6173 206a 736f 6e5f 726f  value as json_ro
+0000c530: 770a 2020 2020 2020 2020 2020 2020 2020  w.              
+0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c550: 2020 7b67 726f 7570 6279 5f73 656c 6563    {groupby_selec
+0000c560: 745f 7072 6566 6978 6564 5f73 7472 2e66  t_prefixed_str.f
+0000c570: 6f72 6d61 7428 7072 6566 6978 3d22 6c61  ormat(prefix="la
+0000c580: 7965 725f 666f 725f 6a73 6f6e 2e22 297d  yer_for_json.")}
+0000c590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2046                 F
+0000c5b0: 524f 4d20 227b 7b69 6e70 7574 5f6c 6179  ROM "{{input_lay
+0000c5c0: 6572 7d7d 2220 6c61 7965 725f 666f 725f  er}}" layer_for_
+0000c5d0: 6a73 6f6e 0a20 2020 2020 2020 2020 2020  json.           
+0000c5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c5f0: 2020 2043 524f 5353 204a 4f49 4e20 6a73     CROSS JOIN js
+0000c600: 6f6e 5f65 6163 6828 0a20 2020 2020 2020  on_each(.       
+0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c620: 2020 2020 2020 2020 2020 206c 6179 6572             layer
+0000c630: 5f66 6f72 5f6a 736f 6e2e 5f5f 4449 5353  _for_json.__DISS
+0000c640: 4f4c 5645 5f54 4f4a 534f 4e2c 2022 2422  OLVE_TOJSON, "$"
+0000c650: 2920 6a73 6f6e 5f72 6f77 735f 7461 626c  ) json_rows_tabl
+0000c660: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000c670: 2020 2020 2020 2020 2020 2020 2020 2920                ) 
+0000c680: 6a73 6f6e 5f64 6174 610a 2020 2020 2020  json_data.      
+0000c690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6a0: 2020 2057 4845 5245 2031 3d31 0a20 2020     WHERE 1=1.   
 0000c6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6c0: 2020 2020 5748 4552 4520 313d 310a 2020      WHERE 1=1.  
-0000c6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c6e0: 2020 2020 2020 2020 2020 7b67 726f 7570            {group
-0000c6f0: 6279 5f66 696c 7465 725f 7374 727d 0a20  by_filter_str}. 
-0000c700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c710: 2020 2020 2020 2020 207b 6772 6f75 7062           {groupb
-0000c720: 795f 6772 6f75 7062 795f 7072 6566 6978  y_groupby_prefix
-0000c730: 6564 5f73 7472 2e66 6f72 6d61 7428 7072  ed_str.format(pr
-0000c740: 6566 6978 3d22 6765 6f5f 6461 7461 2e22  efix="geo_data."
-0000c750: 297d 0a20 2020 2020 2020 2020 2020 2020  )}.             
-0000c760: 2020 2020 2020 2020 2020 2020 204f 5244               ORD
-0000c770: 4552 2042 5920 6765 6f5f 6461 7461 2e7b  ER BY geo_data.{
-0000c780: 6f72 6465 7262 795f 636f 6c75 6d6e 7d0a  orderby_column}.
-0000c790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c7a0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-0000c7b0: 2020 2020 2020 2020 2023 2041 7070 6c79           # Apply
-0000c7c0: 2077 6865 7265 2070 6172 616d 6574 6572   where parameter
-0000c7d0: 2069 6620 6e65 6564 6564 2f70 6f73 7369   if needed/possi
-0000c7e0: 626c 650a 2020 2020 2020 2020 2020 2020  ble.            
-0000c7f0: 2020 2020 6966 2077 6865 7265 2069 7320      if where is 
-0000c800: 6e6f 7420 4e6f 6e65 2061 6e64 206e 6f74  not None and not
-0000c810: 206e 6f74 2065 7870 6c6f 6465 636f 6c6c   not explodecoll
-0000c820: 6563 7469 6f6e 733a 0a20 2020 2020 2020  ections:.       
-0000c830: 2020 2020 2020 2020 2020 2020 2023 2065               # e
-0000c840: 7870 6c6f 6465 636f 6c6c 6563 7469 6f6e  xplodecollection
-0000c850: 7320 6973 206e 6f74 2054 7275 652c 2073  s is not True, s
-0000c860: 6f20 7765 2063 616e 2061 6464 2069 7420  o we can add it 
-0000c870: 746f 2073 716c 5f73 746d 742e 0a20 2020  to sql_stmt..   
-0000c880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c890: 2023 2049 6620 6578 706c 6f64 6563 6f6c   # If explodecol
-0000c8a0: 6c65 6374 696f 6e73 2077 6f75 6c64 2062  lections would b
-0000c8b0: 6520 5472 7565 2c20 7765 206e 6565 6420  e True, we need 
-0000c8c0: 746f 2077 6169 7420 746f 2061 7070 6c79  to wait to apply
-0000c8d0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-0000c8e0: 2020 2020 2020 2020 2023 2077 6865 7265           # where
-0000c8f0: 2074 696c 6c20 6166 7465 7220 6578 706c   till after expl
-0000c900: 6f64 6563 6f6c 6c65 6374 696f 6e73 2069  odecollections i
-0000c910: 7320 6170 706c 6965 642c 2073 6f20 7768  s applied, so wh
-0000c920: 656e 2061 7070 656e 6469 6e67 0a20 2020  en appending.   
-0000c930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c940: 2023 2074 6865 2070 6172 7469 616c 2072   # the partial r
-0000c950: 6573 756c 7473 2074 6f20 7468 6520 6f75  esults to the ou
-0000c960: 7470 7574 2066 696c 652e 0a20 2020 2020  tput file..     
-0000c970: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000c980: 6865 7265 203d 2077 6865 7265 2e66 6f72  here = where.for
-0000c990: 6d61 7428 6765 6f6d 6574 7279 636f 6c75  mat(geometrycolu
-0000c9a0: 6d6e 3d22 6765 6f6d 2229 0a20 2020 2020  mn="geom").     
-0000c9b0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000c9c0: 716c 5f73 746d 7420 3d20 6622 2222 0a20  ql_stmt = f""". 
-0000c9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c9e0: 2020 2020 2020 2053 454c 4543 5420 2a20         SELECT * 
-0000c9f0: 4652 4f4d 0a20 2020 2020 2020 2020 2020  FROM.           
+0000c6c0: 2020 2020 2020 2020 207b 6772 6f75 7062           {groupb
+0000c6d0: 795f 6669 6c74 6572 5f73 7472 7d0a 2020  y_filter_str}.  
+0000c6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c6f0: 2020 2020 2020 2020 7b67 726f 7570 6279          {groupby
+0000c700: 5f67 726f 7570 6279 5f70 7265 6669 7865  _groupby_prefixe
+0000c710: 645f 7374 722e 666f 726d 6174 2870 7265  d_str.format(pre
+0000c720: 6669 783d 2267 656f 5f64 6174 612e 2229  fix="geo_data.")
+0000c730: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+0000c740: 2020 2020 2020 2020 2020 2020 4f52 4445              ORDE
+0000c750: 5220 4259 2067 656f 5f64 6174 612e 7b6f  R BY geo_data.{o
+0000c760: 7264 6572 6279 5f63 6f6c 756d 6e7d 0a20  rderby_column}. 
+0000c770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c780: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
+0000c790: 2020 2020 2020 2020 2320 4170 706c 7920          # Apply 
+0000c7a0: 7768 6572 6520 7061 7261 6d65 7465 7220  where parameter 
+0000c7b0: 6966 206e 6565 6465 642f 706f 7373 6962  if needed/possib
+0000c7c0: 6c65 0a20 2020 2020 2020 2020 2020 2020  le.             
+0000c7d0: 2020 2069 6620 7768 6572 6520 6973 206e     if where is n
+0000c7e0: 6f74 204e 6f6e 6520 616e 6420 6e6f 7420  ot None and not 
+0000c7f0: 6e6f 7420 6578 706c 6f64 6563 6f6c 6c65  not explodecolle
+0000c800: 6374 696f 6e73 3a0a 2020 2020 2020 2020  ctions:.        
+0000c810: 2020 2020 2020 2020 2020 2020 2320 6578              # ex
+0000c820: 706c 6f64 6563 6f6c 6c65 6374 696f 6e73  plodecollections
+0000c830: 2069 7320 6e6f 7420 5472 7565 2c20 736f   is not True, so
+0000c840: 2077 6520 6361 6e20 6164 6420 6974 2074   we can add it t
+0000c850: 6f20 7371 6c5f 7374 6d74 2e0a 2020 2020  o sql_stmt..    
+0000c860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c870: 2320 4966 2065 7870 6c6f 6465 636f 6c6c  # If explodecoll
+0000c880: 6563 7469 6f6e 7320 776f 756c 6420 6265  ections would be
+0000c890: 2054 7275 652c 2077 6520 6e65 6564 2074   True, we need t
+0000c8a0: 6f20 7761 6974 2074 6f20 6170 706c 7920  o wait to apply 
+0000c8b0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+0000c8c0: 2020 2020 2020 2020 2320 7768 6572 6520          # where 
+0000c8d0: 7469 6c6c 2061 6674 6572 2065 7870 6c6f  till after explo
+0000c8e0: 6465 636f 6c6c 6563 7469 6f6e 7320 6973  decollections is
+0000c8f0: 2061 7070 6c69 6564 2c20 736f 2077 6865   applied, so whe
+0000c900: 6e20 6170 7065 6e64 696e 670a 2020 2020  n appending.    
+0000c910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c920: 2320 7468 6520 7061 7274 6961 6c20 7265  # the partial re
+0000c930: 7375 6c74 7320 746f 2074 6865 206f 7574  sults to the out
+0000c940: 7075 7420 6669 6c65 2e0a 2020 2020 2020  put file..      
+0000c950: 2020 2020 2020 2020 2020 2020 2020 7768                wh
+0000c960: 6572 6520 3d20 7768 6572 652e 666f 726d  ere = where.form
+0000c970: 6174 2867 656f 6d65 7472 7963 6f6c 756d  at(geometrycolum
+0000c980: 6e3d 2267 656f 6d22 290a 2020 2020 2020  n="geom").      
+0000c990: 2020 2020 2020 2020 2020 2020 2020 7371                sq
+0000c9a0: 6c5f 7374 6d74 203d 2066 2222 220a 2020  l_stmt = f""".  
+0000c9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9c0: 2020 2020 2020 5345 4c45 4354 202a 2046        SELECT * F
+0000c9d0: 524f 4d0a 2020 2020 2020 2020 2020 2020  ROM.            
+0000c9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c9f0: 2820 7b73 716c 5f73 746d 747d 0a20 2020  ( {sql_stmt}.   
 0000ca00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca10: 2028 207b 7371 6c5f 7374 6d74 7d0a 2020   ( {sql_stmt}.  
+0000ca10: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
 0000ca20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca30: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000ca40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ca50: 2020 2020 5748 4552 4520 7b77 6865 7265      WHERE {where
-0000ca60: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
-0000ca70: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000ca80: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000ca90: 5768 6572 6520 6861 7320 6265 656e 2061  Where has been a
-0000caa0: 7070 6c69 6564 2061 6c72 6561 6479 2073  pplied already s
-0000cab0: 6f20 7365 7420 746f 204e 6f6e 652e 0a20  o set to None.. 
+0000ca30: 2020 2057 4845 5245 207b 7768 6572 657d     WHERE {where}
+0000ca40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ca50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000ca60: 2020 2020 2020 2020 2020 2020 2023 2057               # W
+0000ca70: 6865 7265 2068 6173 2062 6565 6e20 6170  here has been ap
+0000ca80: 706c 6965 6420 616c 7265 6164 7920 736f  plied already so
+0000ca90: 2073 6574 2074 6f20 4e6f 6e65 2e0a 2020   set to None..  
+0000caa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cab0: 2020 7768 6572 6520 3d20 4e6f 6e65 0a0a    where = None..
 0000cac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cad0: 2020 2077 6865 7265 203d 204e 6f6e 650a     where = None.
-0000cae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000caf0: 206c 6f67 6765 722e 696e 666f 2822 506f   logger.info("Po
-0000cb00: 7374 7072 6f63 6573 7320 6f75 7470 7574  stprocess output
-0000cb10: 2066 696c 6522 290a 2020 2020 2020 2020   file").        
-0000cb20: 2020 2020 2020 2020 6966 2077 6865 7265          if where
-0000cb30: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
-0000cb40: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-0000cb50: 6d65 203d 2066 226f 7574 7075 745f 746d  me = f"output_tm
-0000cb60: 7032 5f66 696e 616c 7b6f 7574 7075 745f  p2_final{output_
-0000cb70: 7061 7468 2e73 7566 6669 787d 220a 2020  path.suffix}".  
-0000cb80: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000cb90: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000cba0: 2020 2020 2020 2020 6e61 6d65 203d 2066          name = f
-0000cbb0: 226f 7574 7075 745f 746d 7032 5f66 696e  "output_tmp2_fin
-0000cbc0: 616c 7b6f 7574 7075 745f 746d 705f 7061  al{output_tmp_pa
-0000cbd0: 7468 2e73 7566 6669 787d 220a 2020 2020  th.suffix}".    
-0000cbe0: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-0000cbf0: 7574 5f74 6d70 325f 6669 6e61 6c5f 7061  ut_tmp2_final_pa
-0000cc00: 7468 203d 2074 656d 7064 6972 202f 206e  th = tempdir / n
-0000cc10: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
-0000cc20: 2020 2020 7371 6c5f 7374 6d74 203d 2073      sql_stmt = s
-0000cc30: 716c 5f73 746d 742e 666f 726d 6174 280a  ql_stmt.format(.
-0000cc40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc50: 2020 2020 6765 6f6d 6574 7279 636f 6c75      geometrycolu
-0000cc60: 6d6e 3d22 6765 6f6d 222c 2069 6e70 7574  mn="geom", input
-0000cc70: 5f6c 6179 6572 3d6f 7574 7075 745f 6c61  _layer=output_la
-0000cc80: 7965 720a 2020 2020 2020 2020 2020 2020  yer.            
-0000cc90: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000cca0: 2020 2020 2020 6372 6561 7465 5f73 7061        create_spa
-0000ccb0: 7469 616c 5f69 6e64 6578 203d 2054 7275  tial_index = Tru
-0000ccc0: 6520 6966 2077 6865 7265 2069 7320 4e6f  e if where is No
-0000ccd0: 6e65 2065 6c73 6520 4661 6c73 650a 2020  ne else False.  
-0000cce0: 2020 2020 2020 2020 2020 2020 2020 5f6f                _o
-0000ccf0: 6772 5f75 7469 6c2e 7665 6374 6f72 5f74  gr_util.vector_t
-0000cd00: 7261 6e73 6c61 7465 280a 2020 2020 2020  ranslate(.      
-0000cd10: 2020 2020 2020 2020 2020 2020 2020 696e                in
-0000cd20: 7075 745f 7061 7468 3d6f 7574 7075 745f  put_path=output_
-0000cd30: 746d 705f 7061 7468 2c0a 2020 2020 2020  tmp_path,.      
-0000cd40: 2020 2020 2020 2020 2020 2020 2020 6f75                ou
-0000cd50: 7470 7574 5f70 6174 683d 6f75 7470 7574  tput_path=output
-0000cd60: 5f74 6d70 325f 6669 6e61 6c5f 7061 7468  _tmp2_final_path
-0000cd70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000cd80: 2020 2020 2020 6f75 7470 7574 5f6c 6179        output_lay
-0000cd90: 6572 3d6f 7574 7075 745f 6c61 7965 722c  er=output_layer,
-0000cda0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cdb0: 2020 2020 2073 716c 5f73 746d 743d 7371       sql_stmt=sq
-0000cdc0: 6c5f 7374 6d74 2c0a 2020 2020 2020 2020  l_stmt,.        
-0000cdd0: 2020 2020 2020 2020 2020 2020 7371 6c5f              sql_
-0000cde0: 6469 616c 6563 743d 2253 514c 4954 4522  dialect="SQLITE"
-0000cdf0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000ce00: 2020 2020 2020 666f 7263 655f 6f75 7470        force_outp
-0000ce10: 7574 5f67 656f 6d65 7472 7974 7970 653d  ut_geometrytype=
-0000ce20: 696e 7075 745f 6c61 7965 7269 6e66 6f2e  input_layerinfo.
-0000ce30: 6765 6f6d 6574 7279 7479 7065 2c0a 2020  geometrytype,.  
-0000ce40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce50: 2020 6578 706c 6f64 6563 6f6c 6c65 6374    explodecollect
-0000ce60: 696f 6e73 3d65 7870 6c6f 6465 636f 6c6c  ions=explodecoll
-0000ce70: 6563 7469 6f6e 732c 0a20 2020 2020 2020  ections,.       
-0000ce80: 2020 2020 2020 2020 2020 2020 206f 7074               opt
-0000ce90: 696f 6e73 3d7b 224c 4159 4552 5f43 5245  ions={"LAYER_CRE
-0000cea0: 4154 494f 4e2e 5350 4154 4941 4c5f 494e  ATION.SPATIAL_IN
-0000ceb0: 4445 5822 3a20 6372 6561 7465 5f73 7061  DEX": create_spa
-0000cec0: 7469 616c 5f69 6e64 6578 7d2c 0a20 2020  tial_index},.   
-0000ced0: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-0000cee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cef0: 2320 5765 2073 7469 6c6c 206e 6565 6420  # We still need 
-0000cf00: 746f 2061 7070 6c79 2074 6865 2077 6865  to apply the whe
-0000cf10: 7265 2066 696c 7465 720a 2020 2020 2020  re filter.      
-0000cf20: 2020 2020 2020 2020 2020 6966 2077 6865            if whe
-0000cf30: 7265 2069 7320 6e6f 7420 4e6f 6e65 3a0a  re is not None:.
-0000cf40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf50: 2020 2020 6e61 6d65 203d 2066 226f 7574      name = f"out
-0000cf60: 7075 745f 746d 7033 5f77 6865 7265 7b6f  put_tmp3_where{o
-0000cf70: 7574 7075 745f 7061 7468 2e73 7566 6669  utput_path.suffi
-0000cf80: 787d 220a 2020 2020 2020 2020 2020 2020  x}".            
-0000cf90: 2020 2020 2020 2020 6f75 7470 7574 5f74          output_t
-0000cfa0: 6d70 335f 7768 6572 655f 7061 7468 203d  mp3_where_path =
-0000cfb0: 2074 656d 7064 6972 202f 206e 616d 650a   tempdir / name.
-0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfd0: 2020 2020 6f75 7470 7574 5f74 6d70 325f      output_tmp2_
-0000cfe0: 696e 666f 203d 2067 666f 2e67 6574 5f6c  info = gfo.get_l
-0000cff0: 6179 6572 696e 666f 286f 7574 7075 745f  ayerinfo(output_
-0000d000: 746d 7032 5f66 696e 616c 5f70 6174 6829  tmp2_final_path)
-0000d010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d020: 2020 2020 2077 6865 7265 203d 2077 6865       where = whe
-0000d030: 7265 2e66 6f72 6d61 7428 6765 6f6d 6574  re.format(geomet
-0000d040: 7279 636f 6c75 6d6e 3d6f 7574 7075 745f  rycolumn=output_
-0000d050: 746d 7032 5f69 6e66 6f2e 6765 6f6d 6574  tmp2_info.geomet
-0000d060: 7279 636f 6c75 6d6e 290a 2020 2020 2020  rycolumn).      
-0000d070: 2020 2020 2020 2020 2020 2020 2020 7371                sq
-0000d080: 6c5f 7374 6d74 203d 2066 2222 220a 2020  l_stmt = f""".  
-0000d090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0a0: 2020 2020 2020 5345 4c45 4354 202a 2046        SELECT * F
-0000d0b0: 524f 4d20 227b 6f75 7470 7574 5f6c 6179  ROM "{output_lay
-0000d0c0: 6572 7d22 0a20 2020 2020 2020 2020 2020  er}".           
-0000d0d0: 2020 2020 2020 2020 2020 2020 2020 5748                WH
-0000d0e0: 4552 4520 7b77 6865 7265 7d0a 2020 2020  ERE {where}.    
-0000d0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d100: 2222 220a 2020 2020 2020 2020 2020 2020  """.            
-0000d110: 2020 2020 2020 2020 746d 705f 696e 666f          tmp_info
-0000d120: 203d 2067 666f 2e67 6574 5f6c 6179 6572   = gfo.get_layer
-0000d130: 696e 666f 286f 7574 7075 745f 746d 7032  info(output_tmp2
-0000d140: 5f66 696e 616c 5f70 6174 682c 206f 7574  _final_path, out
-0000d150: 7075 745f 6c61 7965 7229 0a20 2020 2020  put_layer).     
-0000d160: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d170: 716c 5f73 746d 7420 3d20 7371 6c5f 7374  ql_stmt = sql_st
-0000d180: 6d74 2e66 6f72 6d61 7428 6765 6f6d 6574  mt.format(geomet
-0000d190: 7279 636f 6c75 6d6e 3d74 6d70 5f69 6e66  rycolumn=tmp_inf
-0000d1a0: 6f2e 6765 6f6d 6574 7279 636f 6c75 6d6e  o.geometrycolumn
-0000d1b0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000d1c0: 2020 2020 2020 5f6f 6772 5f75 7469 6c2e        _ogr_util.
-0000d1d0: 7665 6374 6f72 5f74 7261 6e73 6c61 7465  vector_translate
-0000d1e0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000d1f0: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-0000d200: 7061 7468 3d6f 7574 7075 745f 746d 7032  path=output_tmp2
-0000d210: 5f66 696e 616c 5f70 6174 682c 0a20 2020  _final_path,.   
-0000d220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d230: 2020 2020 206f 7574 7075 745f 7061 7468       output_path
-0000d240: 3d6f 7574 7075 745f 746d 7033 5f77 6865  =output_tmp3_whe
-0000d250: 7265 5f70 6174 682c 0a20 2020 2020 2020  re_path,.       
-0000d260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d270: 206f 7574 7075 745f 6c61 7965 723d 6f75   output_layer=ou
-0000d280: 7470 7574 5f6c 6179 6572 2c0a 2020 2020  tput_layer,.    
-0000d290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2a0: 2020 2020 666f 7263 655f 6f75 7470 7574      force_output
-0000d2b0: 5f67 656f 6d65 7472 7974 7970 653d 696e  _geometrytype=in
-0000d2c0: 7075 745f 6c61 7965 7269 6e66 6f2e 6765  put_layerinfo.ge
-0000d2d0: 6f6d 6574 7279 7479 7065 2c0a 2020 2020  ometrytype,.    
-0000d2e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d2f0: 2020 2020 7371 6c5f 7374 6d74 3d73 716c      sql_stmt=sql
-0000d300: 5f73 746d 742c 0a20 2020 2020 2020 2020  _stmt,.         
-0000d310: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d320: 716c 5f64 6961 6c65 6374 3d22 5351 4c49  ql_dialect="SQLI
-0000d330: 5445 222c 0a20 2020 2020 2020 2020 2020  TE",.           
-0000d340: 2020 2020 2020 2020 2020 2020 206f 7074               opt
-0000d350: 696f 6e73 3d7b 224c 4159 4552 5f43 5245  ions={"LAYER_CRE
-0000d360: 4154 494f 4e2e 5350 4154 4941 4c5f 494e  ATION.SPATIAL_IN
-0000d370: 4445 5822 3a20 5472 7565 7d2c 0a20 2020  DEX": True},.   
-0000d380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d390: 2029 0a20 2020 2020 2020 2020 2020 2020   ).             
-0000d3a0: 2020 2020 2020 206f 7574 7075 745f 746d         output_tm
-0000d3b0: 7032 5f66 696e 616c 5f70 6174 6820 3d20  p2_final_path = 
-0000d3c0: 6f75 7470 7574 5f74 6d70 335f 7768 6572  output_tmp3_wher
-0000d3d0: 655f 7061 7468 0a0a 2020 2020 2020 2020  e_path..        
-0000d3e0: 2020 2020 2020 2020 2320 4e6f 7720 7765          # Now we
-0000d3f0: 2061 7265 2072 6561 6479 2074 6f20 6d6f   are ready to mo
-0000d400: 7665 2074 6865 2072 6573 756c 7420 746f  ve the result to
-0000d410: 2074 6865 2066 696e 616c 2073 706f 742e   the final spot.
-0000d420: 2e2e 0a20 2020 2020 2020 2020 2020 2020  ...             
-0000d430: 2020 2067 666f 2e6d 6f76 6528 6f75 7470     gfo.move(outp
-0000d440: 7574 5f74 6d70 325f 6669 6e61 6c5f 7061  ut_tmp2_final_pa
-0000d450: 7468 2c20 6f75 7470 7574 5f70 6174 6829  th, output_path)
-0000d460: 0a0a 2020 2020 2020 2020 6669 6e61 6c6c  ..        finall
-0000d470: 793a 0a20 2020 2020 2020 2020 2020 2073  y:.            s
-0000d480: 6875 7469 6c2e 726d 7472 6565 2874 656d  hutil.rmtree(tem
-0000d490: 7064 6972 2c20 6967 6e6f 7265 5f65 7272  pdir, ignore_err
-0000d4a0: 6f72 733d 5472 7565 290a 2020 2020 656c  ors=True).    el
-0000d4b0: 7365 3a0a 2020 2020 2020 2020 7261 6973  se:.        rais
-0000d4c0: 6520 4e6f 7449 6d70 6c65 6d65 6e74 6564  e NotImplemented
-0000d4d0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-0000d4e0: 2020 2066 2255 6e73 7570 706f 7274 6564     f"Unsupported
-0000d4f0: 2069 6e70 7574 2067 656f 6d65 7472 7974   input geometryt
-0000d500: 7970 653a 207b 696e 7075 745f 6c61 7965  ype: {input_laye
-0000d510: 7269 6e66 6f2e 6765 6f6d 6574 7279 7479  rinfo.geometryty
-0000d520: 7065 7d22 0a20 2020 2020 2020 2029 0a0a  pe}".        )..
-0000d530: 2020 2020 2320 5265 7475 726e 2072 6573      # Return res
-0000d540: 756c 7420 696e 666f 0a20 2020 2072 6573  ult info.    res
-0000d550: 756c 745f 696e 666f 5b0a 2020 2020 2020  ult_info[.      
-0000d560: 2020 226d 6573 7361 6765 220a 2020 2020    "message".    
-0000d570: 5d20 3d20 6622 4469 7373 6f6c 7665 2063  ] = f"Dissolve c
-0000d580: 6f6d 706c 6574 656c 7920 7265 6164 792c  ompletely ready,
-0000d590: 2074 6f6f 6b20 7b64 6174 6574 696d 652e   took {datetime.
-0000d5a0: 6e6f 7728 292d 7374 6172 745f 7469 6d65  now()-start_time
-0000d5b0: 7d21 220a 2020 2020 6c6f 6767 6572 2e69  }!".    logger.i
-0000d5c0: 6e66 6f28 7265 7375 6c74 5f69 6e66 6f5b  nfo(result_info[
-0000d5d0: 226d 6573 7361 6765 225d 290a 2020 2020  "message"]).    
-0000d5e0: 7265 7475 726e 2072 6573 756c 745f 696e  return result_in
-0000d5f0: 666f 0a0a 0a64 6566 205f 6469 7373 6f6c  fo...def _dissol
-0000d600: 7665 5f70 6f6c 7967 6f6e 735f 7061 7373  ve_polygons_pass
-0000d610: 280a 2020 2020 696e 7075 745f 7061 7468  (.    input_path
-0000d620: 3a20 5061 7468 2c0a 2020 2020 6f75 7470  : Path,.    outp
-0000d630: 7574 5f6e 6f74 6f6e 626f 7264 6572 5f70  ut_notonborder_p
-0000d640: 6174 683a 2050 6174 682c 0a20 2020 206f  ath: Path,.    o
-0000d650: 7574 7075 745f 6f6e 626f 7264 6572 5f70  utput_onborder_p
-0000d660: 6174 683a 2050 6174 682c 0a20 2020 2065  ath: Path,.    e
-0000d670: 7870 6c6f 6465 636f 6c6c 6563 7469 6f6e  xplodecollection
-0000d680: 733a 2062 6f6f 6c2c 0a20 2020 2067 726f  s: bool,.    gro
-0000d690: 7570 6279 5f63 6f6c 756d 6e73 3a20 4f70  upby_columns: Op
-0000d6a0: 7469 6f6e 616c 5b49 7465 7261 626c 655b  tional[Iterable[
-0000d6b0: 7374 725d 5d2c 0a20 2020 2061 6767 5f63  str]],.    agg_c
-0000d6c0: 6f6c 756d 6e73 3a20 4f70 7469 6f6e 616c  olumns: Optional
-0000d6d0: 5b64 6963 745d 2c0a 2020 2020 7469 6c65  [dict],.    tile
-0000d6e0: 735f 6764 663a 2067 7064 2e47 656f 4461  s_gdf: gpd.GeoDa
-0000d6f0: 7461 4672 616d 652c 0a20 2020 2069 6e70  taFrame,.    inp
+0000cad0: 6c6f 6767 6572 2e69 6e66 6f28 2250 6f73  logger.info("Pos
+0000cae0: 7470 726f 6365 7373 206f 7574 7075 7420  tprocess output 
+0000caf0: 6669 6c65 2229 0a20 2020 2020 2020 2020  file").         
+0000cb00: 2020 2020 2020 2069 6620 7768 6572 6520         if where 
+0000cb10: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+0000cb20: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+0000cb30: 6520 3d20 6622 6f75 7470 7574 5f74 6d70  e = f"output_tmp
+0000cb40: 325f 6669 6e61 6c7b 6f75 7470 7574 5f70  2_final{output_p
+0000cb50: 6174 682e 7375 6666 6978 7d22 0a20 2020  ath.suffix}".   
+0000cb60: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000cb70: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000cb80: 2020 2020 2020 206e 616d 6520 3d20 6622         name = f"
+0000cb90: 6f75 7470 7574 5f74 6d70 325f 6669 6e61  output_tmp2_fina
+0000cba0: 6c7b 6f75 7470 7574 5f74 6d70 5f70 6174  l{output_tmp_pat
+0000cbb0: 682e 7375 6666 6978 7d22 0a20 2020 2020  h.suffix}".     
+0000cbc0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+0000cbd0: 745f 746d 7032 5f66 696e 616c 5f70 6174  t_tmp2_final_pat
+0000cbe0: 6820 3d20 7465 6d70 6469 7220 2f20 6e61  h = tempdir / na
+0000cbf0: 6d65 0a20 2020 2020 2020 2020 2020 2020  me.             
+0000cc00: 2020 2073 716c 5f73 746d 7420 3d20 7371     sql_stmt = sq
+0000cc10: 6c5f 7374 6d74 2e66 6f72 6d61 7428 0a20  l_stmt.format(. 
+0000cc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cc30: 2020 2067 656f 6d65 7472 7963 6f6c 756d     geometrycolum
+0000cc40: 6e3d 2267 656f 6d22 2c20 696e 7075 745f  n="geom", input_
+0000cc50: 6c61 7965 723d 6f75 7470 7574 5f6c 6179  layer=output_lay
+0000cc60: 6572 0a20 2020 2020 2020 2020 2020 2020  er.             
+0000cc70: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000cc80: 2020 2020 2063 7265 6174 655f 7370 6174       create_spat
+0000cc90: 6961 6c5f 696e 6465 7820 3d20 5472 7565  ial_index = True
+0000cca0: 2069 6620 7768 6572 6520 6973 204e 6f6e   if where is Non
+0000ccb0: 6520 656c 7365 2046 616c 7365 0a20 2020  e else False.   
+0000ccc0: 2020 2020 2020 2020 2020 2020 205f 6f67               _og
+0000ccd0: 725f 7574 696c 2e76 6563 746f 725f 7472  r_util.vector_tr
+0000cce0: 616e 736c 6174 6528 0a20 2020 2020 2020  anslate(.       
+0000ccf0: 2020 2020 2020 2020 2020 2020 2069 6e70               inp
+0000cd00: 7574 5f70 6174 683d 6f75 7470 7574 5f74  ut_path=output_t
+0000cd10: 6d70 5f70 6174 682c 0a20 2020 2020 2020  mp_path,.       
+0000cd20: 2020 2020 2020 2020 2020 2020 206f 7574               out
+0000cd30: 7075 745f 7061 7468 3d6f 7574 7075 745f  put_path=output_
+0000cd40: 746d 7032 5f66 696e 616c 5f70 6174 682c  tmp2_final_path,
+0000cd50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cd60: 2020 2020 206f 7574 7075 745f 6c61 7965       output_laye
+0000cd70: 723d 6f75 7470 7574 5f6c 6179 6572 2c0a  r=output_layer,.
+0000cd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cd90: 2020 2020 7371 6c5f 7374 6d74 3d73 716c      sql_stmt=sql
+0000cda0: 5f73 746d 742c 0a20 2020 2020 2020 2020  _stmt,.         
+0000cdb0: 2020 2020 2020 2020 2020 2073 716c 5f64             sql_d
+0000cdc0: 6961 6c65 6374 3d22 5351 4c49 5445 222c  ialect="SQLITE",
+0000cdd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cde0: 2020 2020 2066 6f72 6365 5f6f 7574 7075       force_outpu
+0000cdf0: 745f 6765 6f6d 6574 7279 7479 7065 3d69  t_geometrytype=i
+0000ce00: 6e70 7574 5f6c 6179 6572 696e 666f 2e67  nput_layerinfo.g
+0000ce10: 656f 6d65 7472 7974 7970 652c 0a20 2020  eometrytype,.   
+0000ce20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce30: 2065 7870 6c6f 6465 636f 6c6c 6563 7469   explodecollecti
+0000ce40: 6f6e 733d 6578 706c 6f64 6563 6f6c 6c65  ons=explodecolle
+0000ce50: 6374 696f 6e73 2c0a 2020 2020 2020 2020  ctions,.        
+0000ce60: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
+0000ce70: 6f6e 733d 7b22 4c41 5945 525f 4352 4541  ons={"LAYER_CREA
+0000ce80: 5449 4f4e 2e53 5041 5449 414c 5f49 4e44  TION.SPATIAL_IND
+0000ce90: 4558 223a 2063 7265 6174 655f 7370 6174  EX": create_spat
+0000cea0: 6961 6c5f 696e 6465 787d 2c0a 2020 2020  ial_index},.    
+0000ceb0: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+0000cec0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000ced0: 2057 6520 7374 696c 6c20 6e65 6564 2074   We still need t
+0000cee0: 6f20 6170 706c 7920 7468 6520 7768 6572  o apply the wher
+0000cef0: 6520 6669 6c74 6572 0a20 2020 2020 2020  e filter.       
+0000cf00: 2020 2020 2020 2020 2069 6620 7768 6572           if wher
+0000cf10: 6520 6973 206e 6f74 204e 6f6e 653a 0a20  e is not None:. 
+0000cf20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf30: 2020 206e 616d 6520 3d20 6622 6f75 7470     name = f"outp
+0000cf40: 7574 5f74 6d70 335f 7768 6572 657b 6f75  ut_tmp3_where{ou
+0000cf50: 7470 7574 5f70 6174 682e 7375 6666 6978  tput_path.suffix
+0000cf60: 7d22 0a20 2020 2020 2020 2020 2020 2020  }".             
+0000cf70: 2020 2020 2020 206f 7574 7075 745f 746d         output_tm
+0000cf80: 7033 5f77 6865 7265 5f70 6174 6820 3d20  p3_where_path = 
+0000cf90: 7465 6d70 6469 7220 2f20 6e61 6d65 0a20  tempdir / name. 
+0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfb0: 2020 206f 7574 7075 745f 746d 7032 5f69     output_tmp2_i
+0000cfc0: 6e66 6f20 3d20 6766 6f2e 6765 745f 6c61  nfo = gfo.get_la
+0000cfd0: 7965 7269 6e66 6f28 6f75 7470 7574 5f74  yerinfo(output_t
+0000cfe0: 6d70 325f 6669 6e61 6c5f 7061 7468 290a  mp2_final_path).
+0000cff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d000: 2020 2020 7768 6572 6520 3d20 7768 6572      where = wher
+0000d010: 652e 666f 726d 6174 2867 656f 6d65 7472  e.format(geometr
+0000d020: 7963 6f6c 756d 6e3d 6f75 7470 7574 5f74  ycolumn=output_t
+0000d030: 6d70 325f 696e 666f 2e67 656f 6d65 7472  mp2_info.geometr
+0000d040: 7963 6f6c 756d 6e29 0a20 2020 2020 2020  ycolumn).       
+0000d050: 2020 2020 2020 2020 2020 2020 2073 716c               sql
+0000d060: 5f73 746d 7420 3d20 6622 2222 0a20 2020  _stmt = f""".   
+0000d070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d080: 2020 2020 2053 454c 4543 5420 2a20 4652       SELECT * FR
+0000d090: 4f4d 2022 7b6f 7574 7075 745f 6c61 7965  OM "{output_laye
+0000d0a0: 727d 220a 2020 2020 2020 2020 2020 2020  r}".            
+0000d0b0: 2020 2020 2020 2020 2020 2020 2057 4845               WHE
+0000d0c0: 5245 207b 7768 6572 657d 0a20 2020 2020  RE {where}.     
+0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000d0e0: 2222 0a20 2020 2020 2020 2020 2020 2020  "".             
+0000d0f0: 2020 2020 2020 2074 6d70 5f69 6e66 6f20         tmp_info 
+0000d100: 3d20 6766 6f2e 6765 745f 6c61 7965 7269  = gfo.get_layeri
+0000d110: 6e66 6f28 6f75 7470 7574 5f74 6d70 325f  nfo(output_tmp2_
+0000d120: 6669 6e61 6c5f 7061 7468 2c20 6f75 7470  final_path, outp
+0000d130: 7574 5f6c 6179 6572 290a 2020 2020 2020  ut_layer).      
+0000d140: 2020 2020 2020 2020 2020 2020 2020 7371                sq
+0000d150: 6c5f 7374 6d74 203d 2073 716c 5f73 746d  l_stmt = sql_stm
+0000d160: 742e 666f 726d 6174 2867 656f 6d65 7472  t.format(geometr
+0000d170: 7963 6f6c 756d 6e3d 746d 705f 696e 666f  ycolumn=tmp_info
+0000d180: 2e67 656f 6d65 7472 7963 6f6c 756d 6e29  .geometrycolumn)
+0000d190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d1a0: 2020 2020 205f 6f67 725f 7574 696c 2e76       _ogr_util.v
+0000d1b0: 6563 746f 725f 7472 616e 736c 6174 6528  ector_translate(
+0000d1c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d1d0: 2020 2020 2020 2020 2069 6e70 7574 5f70           input_p
+0000d1e0: 6174 683d 6f75 7470 7574 5f74 6d70 325f  ath=output_tmp2_
+0000d1f0: 6669 6e61 6c5f 7061 7468 2c0a 2020 2020  final_path,.    
+0000d200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d210: 2020 2020 6f75 7470 7574 5f70 6174 683d      output_path=
+0000d220: 6f75 7470 7574 5f74 6d70 335f 7768 6572  output_tmp3_wher
+0000d230: 655f 7061 7468 2c0a 2020 2020 2020 2020  e_path,.        
+0000d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d250: 6f75 7470 7574 5f6c 6179 6572 3d6f 7574  output_layer=out
+0000d260: 7075 745f 6c61 7965 722c 0a20 2020 2020  put_layer,.     
+0000d270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d280: 2020 2066 6f72 6365 5f6f 7574 7075 745f     force_output_
+0000d290: 6765 6f6d 6574 7279 7479 7065 3d69 6e70  geometrytype=inp
+0000d2a0: 7574 5f6c 6179 6572 696e 666f 2e67 656f  ut_layerinfo.geo
+0000d2b0: 6d65 7472 7974 7970 652c 0a20 2020 2020  metrytype,.     
+0000d2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d2d0: 2020 2073 716c 5f73 746d 743d 7371 6c5f     sql_stmt=sql_
+0000d2e0: 7374 6d74 2c0a 2020 2020 2020 2020 2020  stmt,.          
+0000d2f0: 2020 2020 2020 2020 2020 2020 2020 7371                sq
+0000d300: 6c5f 6469 616c 6563 743d 2253 514c 4954  l_dialect="SQLIT
+0000d310: 4522 2c0a 2020 2020 2020 2020 2020 2020  E",.            
+0000d320: 2020 2020 2020 2020 2020 2020 6f70 7469              opti
+0000d330: 6f6e 733d 7b22 4c41 5945 525f 4352 4541  ons={"LAYER_CREA
+0000d340: 5449 4f4e 2e53 5041 5449 414c 5f49 4e44  TION.SPATIAL_IND
+0000d350: 4558 223a 2054 7275 657d 2c0a 2020 2020  EX": True},.    
+0000d360: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d370: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000d380: 2020 2020 2020 6f75 7470 7574 5f74 6d70        output_tmp
+0000d390: 325f 6669 6e61 6c5f 7061 7468 203d 206f  2_final_path = o
+0000d3a0: 7574 7075 745f 746d 7033 5f77 6865 7265  utput_tmp3_where
+0000d3b0: 5f70 6174 680a 0a20 2020 2020 2020 2020  _path..         
+0000d3c0: 2020 2020 2020 2023 204e 6f77 2077 6520         # Now we 
+0000d3d0: 6172 6520 7265 6164 7920 746f 206d 6f76  are ready to mov
+0000d3e0: 6520 7468 6520 7265 7375 6c74 2074 6f20  e the result to 
+0000d3f0: 7468 6520 6669 6e61 6c20 7370 6f74 2e2e  the final spot..
+0000d400: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000d410: 2020 6766 6f2e 6d6f 7665 286f 7574 7075    gfo.move(outpu
+0000d420: 745f 746d 7032 5f66 696e 616c 5f70 6174  t_tmp2_final_pat
+0000d430: 682c 206f 7574 7075 745f 7061 7468 290a  h, output_path).
+0000d440: 0a20 2020 2020 2020 2066 696e 616c 6c79  .        finally
+0000d450: 3a0a 2020 2020 2020 2020 2020 2020 7368  :.            sh
+0000d460: 7574 696c 2e72 6d74 7265 6528 7465 6d70  util.rmtree(temp
+0000d470: 6469 722c 2069 676e 6f72 655f 6572 726f  dir, ignore_erro
+0000d480: 7273 3d54 7275 6529 0a20 2020 2065 6c73  rs=True).    els
+0000d490: 653a 0a20 2020 2020 2020 2072 6169 7365  e:.        raise
+0000d4a0: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
+0000d4b0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+0000d4c0: 2020 6622 556e 7375 7070 6f72 7465 6420    f"Unsupported 
+0000d4d0: 696e 7075 7420 6765 6f6d 6574 7279 7479  input geometryty
+0000d4e0: 7065 3a20 7b69 6e70 7574 5f6c 6179 6572  pe: {input_layer
+0000d4f0: 696e 666f 2e67 656f 6d65 7472 7974 7970  info.geometrytyp
+0000d500: 657d 220a 2020 2020 2020 2020 290a 0a20  e}".        ).. 
+0000d510: 2020 2023 2052 6574 7572 6e20 7265 7375     # Return resu
+0000d520: 6c74 2069 6e66 6f0a 2020 2020 7265 7375  lt info.    resu
+0000d530: 6c74 5f69 6e66 6f5b 0a20 2020 2020 2020  lt_info[.       
+0000d540: 2022 6d65 7373 6167 6522 0a20 2020 205d   "message".    ]
+0000d550: 203d 2066 2244 6973 736f 6c76 6520 636f   = f"Dissolve co
+0000d560: 6d70 6c65 7465 6c79 2072 6561 6479 2c20  mpletely ready, 
+0000d570: 746f 6f6b 207b 6461 7465 7469 6d65 2e6e  took {datetime.n
+0000d580: 6f77 2829 2d73 7461 7274 5f74 696d 657d  ow()-start_time}
+0000d590: 2122 0a20 2020 206c 6f67 6765 722e 696e  !".    logger.in
+0000d5a0: 666f 2872 6573 756c 745f 696e 666f 5b22  fo(result_info["
+0000d5b0: 6d65 7373 6167 6522 5d29 0a20 2020 2072  message"]).    r
+0000d5c0: 6574 7572 6e20 7265 7375 6c74 5f69 6e66  eturn result_inf
+0000d5d0: 6f0a 0a0a 6465 6620 5f64 6973 736f 6c76  o...def _dissolv
+0000d5e0: 655f 706f 6c79 676f 6e73 5f70 6173 7328  e_polygons_pass(
+0000d5f0: 0a20 2020 2069 6e70 7574 5f70 6174 683a  .    input_path:
+0000d600: 2050 6174 682c 0a20 2020 206f 7574 7075   Path,.    outpu
+0000d610: 745f 6e6f 746f 6e62 6f72 6465 725f 7061  t_notonborder_pa
+0000d620: 7468 3a20 5061 7468 2c0a 2020 2020 6f75  th: Path,.    ou
+0000d630: 7470 7574 5f6f 6e62 6f72 6465 725f 7061  tput_onborder_pa
+0000d640: 7468 3a20 5061 7468 2c0a 2020 2020 6578  th: Path,.    ex
+0000d650: 706c 6f64 6563 6f6c 6c65 6374 696f 6e73  plodecollections
+0000d660: 3a20 626f 6f6c 2c0a 2020 2020 6772 6f75  : bool,.    grou
+0000d670: 7062 795f 636f 6c75 6d6e 733a 204f 7074  pby_columns: Opt
+0000d680: 696f 6e61 6c5b 4974 6572 6162 6c65 5b73  ional[Iterable[s
+0000d690: 7472 5d5d 2c0a 2020 2020 6167 675f 636f  tr]],.    agg_co
+0000d6a0: 6c75 6d6e 733a 204f 7074 696f 6e61 6c5b  lumns: Optional[
+0000d6b0: 6469 6374 5d2c 0a20 2020 2074 696c 6573  dict],.    tiles
+0000d6c0: 5f67 6466 3a20 6770 642e 4765 6f44 6174  _gdf: gpd.GeoDat
+0000d6d0: 6146 7261 6d65 2c0a 2020 2020 696e 7075  aFrame,.    inpu
+0000d6e0: 745f 6c61 7965 723a 204f 7074 696f 6e61  t_layer: Optiona
+0000d6f0: 6c5b 7374 725d 2c0a 2020 2020 6f75 7470  l[str],.    outp
 0000d700: 7574 5f6c 6179 6572 3a20 4f70 7469 6f6e  ut_layer: Option
-0000d710: 616c 5b73 7472 5d2c 0a20 2020 206f 7574  al[str],.    out
-0000d720: 7075 745f 6c61 7965 723a 204f 7074 696f  put_layer: Optio
-0000d730: 6e61 6c5b 7374 725d 2c0a 2020 2020 6772  nal[str],.    gr
-0000d740: 6964 7369 7a65 3a20 666c 6f61 742c 0a20  idsize: float,. 
-0000d750: 2020 206b 6565 705f 656d 7074 795f 6765     keep_empty_ge
-0000d760: 6f6d 733a 2062 6f6f 6c2c 0a20 2020 206e  oms: bool,.    n
-0000d770: 625f 7061 7261 6c6c 656c 3a20 696e 742c  b_parallel: int,
-0000d780: 0a29 202d 3e20 6469 6374 3a0a 2020 2020  .) -> dict:.    
-0000d790: 2320 4d61 6b65 2073 7572 6520 7468 6520  # Make sure the 
-0000d7a0: 696e 7075 7420 6669 6c65 2068 6173 2061  input file has a
-0000d7b0: 2073 7061 7469 616c 2069 6e64 6578 0a20   spatial index. 
-0000d7c0: 2020 2067 666f 2e63 7265 6174 655f 7370     gfo.create_sp
-0000d7d0: 6174 6961 6c5f 696e 6465 7828 696e 7075  atial_index(inpu
-0000d7e0: 745f 7061 7468 2c20 6578 6973 745f 6f6b  t_path, exist_ok
-0000d7f0: 3d54 7275 6529 0a0a 2020 2020 2320 5374  =True)..    # St
-0000d800: 6172 7420 6361 6c63 756c 6174 696f 6e20  art calculation 
-0000d810: 696e 2070 6172 616c 6c65 6c0a 2020 2020  in parallel.    
-0000d820: 7374 6172 745f 7469 6d65 203d 2064 6174  start_time = dat
-0000d830: 6574 696d 652e 6e6f 7728 290a 2020 2020  etime.now().    
-0000d840: 7265 7375 6c74 5f69 6e66 6f20 3d20 7b7d  result_info = {}
-0000d850: 0a20 2020 2073 7461 7274 5f74 696d 6520  .    start_time 
-0000d860: 3d20 6461 7465 7469 6d65 2e6e 6f77 2829  = datetime.now()
-0000d870: 0a20 2020 2069 6e70 7574 5f6c 6179 6572  .    input_layer
-0000d880: 696e 666f 203d 2067 666f 2e67 6574 5f6c  info = gfo.get_l
-0000d890: 6179 6572 696e 666f 2869 6e70 7574 5f70  ayerinfo(input_p
-0000d8a0: 6174 682c 2069 6e70 7574 5f6c 6179 6572  ath, input_layer
-0000d8b0: 290a 0a20 2020 2023 2050 726f 6365 7373  )..    # Process
-0000d8c0: 696e 6720 696e 2074 6872 6561 6473 2069  ing in threads i
-0000d8d0: 7320 3278 2066 6173 7465 7220 666f 7220  s 2x faster for 
-0000d8e0: 736d 616c 6c20 6461 7461 7365 7473 2028  small datasets (
-0000d8f0: 6f6e 2057 696e 646f 7773 290a 2020 2020  on Windows).    
-0000d900: 6361 6c63 756c 6174 655f 696e 5f74 6872  calculate_in_thr
-0000d910: 6561 6473 203d 2054 7275 6520 6966 2069  eads = True if i
-0000d920: 6e70 7574 5f6c 6179 6572 696e 666f 2e66  nput_layerinfo.f
-0000d930: 6561 7475 7265 636f 756e 7420 3c3d 2031  eaturecount <= 1
-0000d940: 3030 2065 6c73 6520 4661 6c73 650a 2020  00 else False.  
-0000d950: 2020 7769 7468 205f 7072 6f63 6573 7369    with _processi
-0000d960: 6e67 5f75 7469 6c2e 506f 6f6c 6564 4578  ng_util.PooledEx
-0000d970: 6563 7574 6f72 4661 6374 6f72 7928 0a20  ecutorFactory(. 
-0000d980: 2020 2020 2020 2074 6872 6561 6470 6f6f         threadpoo
-0000d990: 6c3d 6361 6c63 756c 6174 655f 696e 5f74  l=calculate_in_t
-0000d9a0: 6872 6561 6473 2c0a 2020 2020 2020 2020  hreads,.        
-0000d9b0: 6d61 785f 776f 726b 6572 733d 6e62 5f70  max_workers=nb_p
-0000d9c0: 6172 616c 6c65 6c2c 0a20 2020 2020 2020  arallel,.       
-0000d9d0: 2069 6e69 7469 616c 697a 6572 3d5f 7072   initializer=_pr
-0000d9e0: 6f63 6573 7369 6e67 5f75 7469 6c2e 696e  ocessing_util.in
-0000d9f0: 6974 6961 6c69 7a65 5f77 6f72 6b65 7228  itialize_worker(
-0000da00: 292c 0a20 2020 2029 2061 7320 6361 6c63  ),.    ) as calc
-0000da10: 756c 6174 655f 706f 6f6c 3a0a 2020 2020  ulate_pool:.    
-0000da20: 2020 2020 2320 5072 6570 6172 6520 6f75      # Prepare ou
-0000da30: 7470 7574 2066 696c 656e 616d 650a 2020  tput filename.  
-0000da40: 2020 2020 2020 7465 6d70 6469 7220 3d20        tempdir = 
-0000da50: 6f75 7470 7574 5f6f 6e62 6f72 6465 725f  output_onborder_
-0000da60: 7061 7468 2e70 6172 656e 740a 0a20 2020  path.parent..   
-0000da70: 2020 2020 2062 6174 6368 6573 203d 207b       batches = {
-0000da80: 7d0a 2020 2020 2020 2020 6e62 5f62 6174  }.        nb_bat
-0000da90: 6368 6573 203d 206c 656e 2874 696c 6573  ches = len(tiles
-0000daa0: 5f67 6466 290a 2020 2020 2020 2020 6e62  _gdf).        nb
-0000dab0: 5f62 6174 6368 6573 5f64 6f6e 6520 3d20  _batches_done = 
-0000dac0: 300a 2020 2020 2020 2020 6675 7475 7265  0.        future
-0000dad0: 5f74 6f5f 6261 7463 685f 6964 203d 207b  _to_batch_id = {
-0000dae0: 7d0a 2020 2020 2020 2020 6e62 5f72 6f77  }.        nb_row
-0000daf0: 735f 646f 6e65 203d 2030 0a20 2020 2020  s_done = 0.     
-0000db00: 2020 2066 6f72 2062 6174 6368 5f69 642c     for batch_id,
-0000db10: 2074 696c 655f 726f 7720 696e 2065 6e75   tile_row in enu
-0000db20: 6d65 7261 7465 2874 696c 6573 5f67 6466  merate(tiles_gdf
-0000db30: 2e69 7465 7274 7570 6c65 7328 2929 3a0a  .itertuples()):.
-0000db40: 2020 2020 2020 2020 2020 2020 6261 7463              batc
-0000db50: 6865 735b 6261 7463 685f 6964 5d20 3d20  hes[batch_id] = 
-0000db60: 7b7d 0a20 2020 2020 2020 2020 2020 2062  {}.            b
-0000db70: 6174 6368 6573 5b62 6174 6368 5f69 645d  atches[batch_id]
-0000db80: 5b22 6c61 7965 7222 5d20 3d20 6f75 7470  ["layer"] = outp
-0000db90: 7574 5f6c 6179 6572 0a20 2020 2020 2020  ut_layer.       
-0000dba0: 2020 2020 2062 6174 6368 6573 5b62 6174       batches[bat
-0000dbb0: 6368 5f69 645d 5b22 626f 756e 6473 225d  ch_id]["bounds"]
-0000dbc0: 203d 2074 696c 655f 726f 772e 6765 6f6d   = tile_row.geom
-0000dbd0: 6574 7279 2e62 6f75 6e64 730a 0a20 2020  etry.bounds..   
-0000dbe0: 2020 2020 2020 2020 2023 204f 7574 7075           # Outpu
-0000dbf0: 7420 6561 6368 2062 6174 6368 2074 6f20  t each batch to 
-0000dc00: 6120 7365 7065 7261 7465 2074 656d 706f  a seperate tempo
-0000dc10: 7261 7279 2066 696c 652c 206f 7468 6572  rary file, other
-0000dc20: 7769 7365 2074 6865 7265 0a20 2020 2020  wise there.     
-0000dc30: 2020 2020 2020 2023 2061 7265 2074 696d         # are tim
-0000dc40: 656f 7574 2069 7373 7565 7320 7768 656e  eout issues when
-0000dc50: 2070 726f 6365 7373 696e 6720 6c61 7267   processing larg
-0000dc60: 6520 6669 6c65 730a 2020 2020 2020 2020  e files.        
-0000dc70: 2020 2020 7375 6666 6978 203d 206f 7574      suffix = out
-0000dc80: 7075 745f 6e6f 746f 6e62 6f72 6465 725f  put_notonborder_
-0000dc90: 7061 7468 2e73 7566 6669 780a 2020 2020  path.suffix.    
-0000dca0: 2020 2020 2020 2020 6e61 6d65 203d 2066          name = f
-0000dcb0: 227b 6f75 7470 7574 5f6e 6f74 6f6e 626f  "{output_notonbo
-0000dcc0: 7264 6572 5f70 6174 682e 7374 656d 7d5f  rder_path.stem}_
-0000dcd0: 7b62 6174 6368 5f69 647d 7b73 7566 6669  {batch_id}{suffi
-0000dce0: 787d 220a 2020 2020 2020 2020 2020 2020  x}".            
-0000dcf0: 6f75 7470 7574 5f6e 6f74 6f6e 626f 7264  output_notonbord
-0000dd00: 6572 5f74 6d70 5f70 6172 7469 616c 5f70  er_tmp_partial_p
-0000dd10: 6174 6820 3d20 7465 6d70 6469 7220 2f20  ath = tempdir / 
-0000dd20: 6e61 6d65 0a20 2020 2020 2020 2020 2020  name.           
-0000dd30: 2062 6174 6368 6573 5b62 6174 6368 5f69   batches[batch_i
-0000dd40: 645d 5b0a 2020 2020 2020 2020 2020 2020  d][.            
-0000dd50: 2020 2020 226f 7574 7075 745f 6e6f 746f      "output_noto
-0000dd60: 6e62 6f72 6465 725f 746d 705f 7061 7274  nborder_tmp_part
-0000dd70: 6961 6c5f 7061 7468 220a 2020 2020 2020  ial_path".      
-0000dd80: 2020 2020 2020 5d20 3d20 6f75 7470 7574        ] = output
-0000dd90: 5f6e 6f74 6f6e 626f 7264 6572 5f74 6d70  _notonborder_tmp
-0000dda0: 5f70 6172 7469 616c 5f70 6174 680a 2020  _partial_path.  
-0000ddb0: 2020 2020 2020 2020 2020 6e61 6d65 203d            name =
-0000ddc0: 2066 227b 6f75 7470 7574 5f6f 6e62 6f72   f"{output_onbor
-0000ddd0: 6465 725f 7061 7468 2e73 7465 6d7d 5f7b  der_path.stem}_{
-0000dde0: 6261 7463 685f 6964 7d7b 7375 6666 6978  batch_id}{suffix
-0000ddf0: 7d22 0a20 2020 2020 2020 2020 2020 206f  }".            o
-0000de00: 7574 7075 745f 6f6e 626f 7264 6572 5f74  utput_onborder_t
-0000de10: 6d70 5f70 6172 7469 616c 5f70 6174 6820  mp_partial_path 
-0000de20: 3d20 7465 6d70 6469 7220 2f20 6e61 6d65  = tempdir / name
-0000de30: 0a20 2020 2020 2020 2020 2020 2062 6174  .            bat
-0000de40: 6368 6573 5b62 6174 6368 5f69 645d 5b0a  ches[batch_id][.
-0000de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de60: 226f 7574 7075 745f 6f6e 626f 7264 6572  "output_onborder
-0000de70: 5f74 6d70 5f70 6172 7469 616c 5f70 6174  _tmp_partial_pat
-0000de80: 6822 0a20 2020 2020 2020 2020 2020 205d  h".            ]
-0000de90: 203d 206f 7574 7075 745f 6f6e 626f 7264   = output_onbord
-0000dea0: 6572 5f74 6d70 5f70 6172 7469 616c 5f70  er_tmp_partial_p
-0000deb0: 6174 680a 0a20 2020 2020 2020 2020 2020  ath..           
-0000dec0: 2023 2047 6574 2074 696c 655f 6964 2069   # Get tile_id i
-0000ded0: 6620 7072 6573 656e 740a 2020 2020 2020  f present.      
-0000dee0: 2020 2020 2020 7469 6c65 5f69 6420 3d20        tile_id = 
-0000def0: 7469 6c65 5f72 6f77 2e74 696c 655f 6964  tile_row.tile_id
-0000df00: 2069 6620 2274 696c 655f 6964 2220 696e   if "tile_id" in
-0000df10: 2074 696c 655f 726f 772e 5f66 6965 6c64   tile_row._field
-0000df20: 7320 656c 7365 204e 6f6e 650a 0a20 2020  s else None..   
-0000df30: 2020 2020 2020 2020 2066 7574 7572 6520           future 
-0000df40: 3d20 6361 6c63 756c 6174 655f 706f 6f6c  = calculate_pool
-0000df50: 2e73 7562 6d69 7428 0a20 2020 2020 2020  .submit(.       
-0000df60: 2020 2020 2020 2020 205f 6469 7373 6f6c           _dissol
-0000df70: 7665 5f70 6f6c 7967 6f6e 732c 0a20 2020  ve_polygons,.   
-0000df80: 2020 2020 2020 2020 2020 2020 2069 6e70               inp
-0000df90: 7574 5f70 6174 683d 696e 7075 745f 7061  ut_path=input_pa
-0000dfa0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-0000dfb0: 2020 2020 6f75 7470 7574 5f6e 6f74 6f6e      output_noton
-0000dfc0: 626f 7264 6572 5f70 6174 683d 6f75 7470  border_path=outp
-0000dfd0: 7574 5f6e 6f74 6f6e 626f 7264 6572 5f74  ut_notonborder_t
-0000dfe0: 6d70 5f70 6172 7469 616c 5f70 6174 682c  mp_partial_path,
-0000dff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e000: 206f 7574 7075 745f 6f6e 626f 7264 6572   output_onborder
-0000e010: 5f70 6174 683d 6f75 7470 7574 5f6f 6e62  _path=output_onb
-0000e020: 6f72 6465 725f 746d 705f 7061 7274 6961  order_tmp_partia
-0000e030: 6c5f 7061 7468 2c0a 2020 2020 2020 2020  l_path,.        
-0000e040: 2020 2020 2020 2020 6578 706c 6f64 6563          explodec
-0000e050: 6f6c 6c65 6374 696f 6e73 3d65 7870 6c6f  ollections=explo
-0000e060: 6465 636f 6c6c 6563 7469 6f6e 732c 0a20  decollections,. 
-0000e070: 2020 2020 2020 2020 2020 2020 2020 2067                 g
-0000e080: 726f 7570 6279 5f63 6f6c 756d 6e73 3d67  roupby_columns=g
-0000e090: 726f 7570 6279 5f63 6f6c 756d 6e73 2c0a  roupby_columns,.
-0000e0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0b0: 6167 675f 636f 6c75 6d6e 733d 6167 675f  agg_columns=agg_
-0000e0c0: 636f 6c75 6d6e 732c 0a20 2020 2020 2020  columns,.       
-0000e0d0: 2020 2020 2020 2020 2069 6e70 7574 5f67           input_g
-0000e0e0: 656f 6d65 7472 7974 7970 653d 696e 7075  eometrytype=inpu
-0000e0f0: 745f 6c61 7965 7269 6e66 6f2e 6765 6f6d  t_layerinfo.geom
-0000e100: 6574 7279 7479 7065 2c0a 2020 2020 2020  etrytype,.      
-0000e110: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-0000e120: 6c61 7965 723d 696e 7075 745f 6c61 7965  layer=input_laye
-0000e130: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000e140: 2020 206f 7574 7075 745f 6c61 7965 723d     output_layer=
-0000e150: 6f75 7470 7574 5f6c 6179 6572 2c0a 2020  output_layer,.  
-0000e160: 2020 2020 2020 2020 2020 2020 2020 6262                bb
-0000e170: 6f78 3d74 696c 655f 726f 772e 6765 6f6d  ox=tile_row.geom
-0000e180: 6574 7279 2e62 6f75 6e64 732c 0a20 2020  etry.bounds,.   
-0000e190: 2020 2020 2020 2020 2020 2020 2074 696c               til
-0000e1a0: 655f 6964 3d74 696c 655f 6964 2c0a 2020  e_id=tile_id,.  
-0000e1b0: 2020 2020 2020 2020 2020 2020 2020 6772                gr
-0000e1c0: 6964 7369 7a65 3d67 7269 6473 697a 652c  idsize=gridsize,
-0000e1d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e1e0: 206b 6565 705f 656d 7074 795f 6765 6f6d   keep_empty_geom
-0000e1f0: 733d 6b65 6570 5f65 6d70 7479 5f67 656f  s=keep_empty_geo
-0000e200: 6d73 2c0a 2020 2020 2020 2020 2020 2020  ms,.            
-0000e210: 290a 2020 2020 2020 2020 2020 2020 6675  ).            fu
-0000e220: 7475 7265 5f74 6f5f 6261 7463 685f 6964  ture_to_batch_id
-0000e230: 5b66 7574 7572 655d 203d 2062 6174 6368  [future] = batch
-0000e240: 5f69 640a 0a20 2020 2020 2020 2023 204c  _id..        # L
-0000e250: 6f6f 7020 7469 6c6c 2061 6c6c 2070 6172  oop till all par
-0000e260: 616c 6c65 6c20 7072 6f63 6573 7365 7320  allel processes 
-0000e270: 6172 6520 7265 6164 792c 2062 7574 2070  are ready, but p
-0000e280: 726f 6365 7373 2065 6163 6820 6f6e 650a  rocess each one.
-0000e290: 2020 2020 2020 2020 2320 7468 6174 2069          # that i
-0000e2a0: 7320 7265 6164 7920 616c 7265 6164 790a  s ready already.
-0000e2b0: 2020 2020 2020 2020 5f67 656e 6572 616c          _general
-0000e2c0: 5f75 7469 6c2e 7265 706f 7274 5f70 726f  _util.report_pro
-0000e2d0: 6772 6573 7328 0a20 2020 2020 2020 2020  gress(.         
-0000e2e0: 2020 2073 7461 7274 5f74 696d 652c 206e     start_time, n
-0000e2f0: 625f 6261 7463 6865 735f 646f 6e65 2c20  b_batches_done, 
-0000e300: 6e62 5f62 6174 6368 6573 2c20 2264 6973  nb_batches, "dis
-0000e310: 736f 6c76 6522 0a20 2020 2020 2020 2029  solve".        )
-0000e320: 0a20 2020 2020 2020 2066 6f72 2066 7574  .        for fut
-0000e330: 7572 6520 696e 2066 7574 7572 6573 2e61  ure in futures.a
-0000e340: 735f 636f 6d70 6c65 7465 6428 6675 7475  s_completed(futu
-0000e350: 7265 5f74 6f5f 6261 7463 685f 6964 293a  re_to_batch_id):
-0000e360: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-0000e370: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e380: 2020 2320 4966 2074 6865 2063 616c 6375    # If the calcu
-0000e390: 6c61 7465 2067 6176 6520 7265 7375 6c74  late gave result
-0000e3a0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0000e3b0: 2020 6e62 5f62 6174 6368 6573 5f64 6f6e    nb_batches_don
-0000e3c0: 6520 2b3d 2031 0a20 2020 2020 2020 2020  e += 1.         
-0000e3d0: 2020 2020 2020 2062 6174 6368 5f69 6420         batch_id 
-0000e3e0: 3d20 6675 7475 7265 5f74 6f5f 6261 7463  = future_to_batc
-0000e3f0: 685f 6964 5b66 7574 7572 655d 0a20 2020  h_id[future].   
-0000e400: 2020 2020 2020 2020 2020 2020 2072 6573               res
-0000e410: 756c 7420 3d20 6675 7475 7265 2e72 6573  ult = future.res
-0000e420: 756c 7428 290a 0a20 2020 2020 2020 2020  ult()..         
-0000e430: 2020 2020 2020 2069 6620 7265 7375 6c74         if result
-0000e440: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e460: 2020 6e62 5f72 6f77 735f 646f 6e65 202b    nb_rows_done +
-0000e470: 3d20 7265 7375 6c74 5b22 6e62 5f72 6f77  = result["nb_row
-0000e480: 735f 646f 6e65 225d 0a20 2020 2020 2020  s_done"].       
-0000e490: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000e4a0: 7265 7375 6c74 5b22 6e62 5f72 6f77 735f  result["nb_rows_
-0000e4b0: 646f 6e65 225d 203e 2030 2061 6e64 2072  done"] > 0 and r
-0000e4c0: 6573 756c 745b 2274 6f74 616c 5f74 696d  esult["total_tim
-0000e4d0: 6522 5d20 3e20 303a 0a20 2020 2020 2020  e"] > 0:.       
-0000e4e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e4f0: 2072 6f77 735f 7065 725f 7365 6320 3d20   rows_per_sec = 
-0000e500: 726f 756e 6428 0a20 2020 2020 2020 2020  round(.         
-0000e510: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e520: 2020 2072 6573 756c 745b 226e 625f 726f     result["nb_ro
-0000e530: 7773 5f64 6f6e 6522 5d20 2f20 7265 7375  ws_done"] / resu
-0000e540: 6c74 5b22 746f 7461 6c5f 7469 6d65 225d  lt["total_time"]
-0000e550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e560: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000d710: 616c 5b73 7472 5d2c 0a20 2020 2067 7269  al[str],.    gri
+0000d720: 6473 697a 653a 2066 6c6f 6174 2c0a 2020  dsize: float,.  
+0000d730: 2020 6b65 6570 5f65 6d70 7479 5f67 656f    keep_empty_geo
+0000d740: 6d73 3a20 626f 6f6c 2c0a 2020 2020 6e62  ms: bool,.    nb
+0000d750: 5f70 6172 616c 6c65 6c3a 2069 6e74 2c0a  _parallel: int,.
+0000d760: 2920 2d3e 2064 6963 743a 0a20 2020 2023  ) -> dict:.    #
+0000d770: 204d 616b 6520 7375 7265 2074 6865 2069   Make sure the i
+0000d780: 6e70 7574 2066 696c 6520 6861 7320 6120  nput file has a 
+0000d790: 7370 6174 6961 6c20 696e 6465 780a 2020  spatial index.  
+0000d7a0: 2020 6766 6f2e 6372 6561 7465 5f73 7061    gfo.create_spa
+0000d7b0: 7469 616c 5f69 6e64 6578 2869 6e70 7574  tial_index(input
+0000d7c0: 5f70 6174 682c 2065 7869 7374 5f6f 6b3d  _path, exist_ok=
+0000d7d0: 5472 7565 290a 0a20 2020 2023 2053 7461  True)..    # Sta
+0000d7e0: 7274 2063 616c 6375 6c61 7469 6f6e 2069  rt calculation i
+0000d7f0: 6e20 7061 7261 6c6c 656c 0a20 2020 2073  n parallel.    s
+0000d800: 7461 7274 5f74 696d 6520 3d20 6461 7465  tart_time = date
+0000d810: 7469 6d65 2e6e 6f77 2829 0a20 2020 2072  time.now().    r
+0000d820: 6573 756c 745f 696e 666f 203d 207b 7d0a  esult_info = {}.
+0000d830: 2020 2020 7374 6172 745f 7469 6d65 203d      start_time =
+0000d840: 2064 6174 6574 696d 652e 6e6f 7728 290a   datetime.now().
+0000d850: 2020 2020 696e 7075 745f 6c61 7965 7269      input_layeri
+0000d860: 6e66 6f20 3d20 6766 6f2e 6765 745f 6c61  nfo = gfo.get_la
+0000d870: 7965 7269 6e66 6f28 696e 7075 745f 7061  yerinfo(input_pa
+0000d880: 7468 2c20 696e 7075 745f 6c61 7965 7229  th, input_layer)
+0000d890: 0a0a 2020 2020 2320 5072 6f63 6573 7369  ..    # Processi
+0000d8a0: 6e67 2069 6e20 7468 7265 6164 7320 6973  ng in threads is
+0000d8b0: 2032 7820 6661 7374 6572 2066 6f72 2073   2x faster for s
+0000d8c0: 6d61 6c6c 2064 6174 6173 6574 7320 286f  mall datasets (o
+0000d8d0: 6e20 5769 6e64 6f77 7329 0a20 2020 2063  n Windows).    c
+0000d8e0: 616c 6375 6c61 7465 5f69 6e5f 7468 7265  alculate_in_thre
+0000d8f0: 6164 7320 3d20 5472 7565 2069 6620 696e  ads = True if in
+0000d900: 7075 745f 6c61 7965 7269 6e66 6f2e 6665  put_layerinfo.fe
+0000d910: 6174 7572 6563 6f75 6e74 203c 3d20 3130  aturecount <= 10
+0000d920: 3020 656c 7365 2046 616c 7365 0a20 2020  0 else False.   
+0000d930: 2077 6974 6820 5f70 726f 6365 7373 696e   with _processin
+0000d940: 675f 7574 696c 2e50 6f6f 6c65 6445 7865  g_util.PooledExe
+0000d950: 6375 746f 7246 6163 746f 7279 280a 2020  cutorFactory(.  
+0000d960: 2020 2020 2020 7468 7265 6164 706f 6f6c        threadpool
+0000d970: 3d63 616c 6375 6c61 7465 5f69 6e5f 7468  =calculate_in_th
+0000d980: 7265 6164 732c 0a20 2020 2020 2020 206d  reads,.        m
+0000d990: 6178 5f77 6f72 6b65 7273 3d6e 625f 7061  ax_workers=nb_pa
+0000d9a0: 7261 6c6c 656c 2c0a 2020 2020 2020 2020  rallel,.        
+0000d9b0: 696e 6974 6961 6c69 7a65 723d 5f70 726f  initializer=_pro
+0000d9c0: 6365 7373 696e 675f 7574 696c 2e69 6e69  cessing_util.ini
+0000d9d0: 7469 616c 697a 655f 776f 726b 6572 2829  tialize_worker()
+0000d9e0: 2c0a 2020 2020 2920 6173 2063 616c 6375  ,.    ) as calcu
+0000d9f0: 6c61 7465 5f70 6f6f 6c3a 0a20 2020 2020  late_pool:.     
+0000da00: 2020 2023 2050 7265 7061 7265 206f 7574     # Prepare out
+0000da10: 7075 7420 6669 6c65 6e61 6d65 0a20 2020  put filename.   
+0000da20: 2020 2020 2074 656d 7064 6972 203d 206f       tempdir = o
+0000da30: 7574 7075 745f 6f6e 626f 7264 6572 5f70  utput_onborder_p
+0000da40: 6174 682e 7061 7265 6e74 0a0a 2020 2020  ath.parent..    
+0000da50: 2020 2020 6261 7463 6865 7320 3d20 7b7d      batches = {}
+0000da60: 0a20 2020 2020 2020 206e 625f 6261 7463  .        nb_batc
+0000da70: 6865 7320 3d20 6c65 6e28 7469 6c65 735f  hes = len(tiles_
+0000da80: 6764 6629 0a20 2020 2020 2020 206e 625f  gdf).        nb_
+0000da90: 6261 7463 6865 735f 646f 6e65 203d 2030  batches_done = 0
+0000daa0: 0a20 2020 2020 2020 2066 7574 7572 655f  .        future_
+0000dab0: 746f 5f62 6174 6368 5f69 6420 3d20 7b7d  to_batch_id = {}
+0000dac0: 0a20 2020 2020 2020 206e 625f 726f 7773  .        nb_rows
+0000dad0: 5f64 6f6e 6520 3d20 300a 2020 2020 2020  _done = 0.      
+0000dae0: 2020 666f 7220 6261 7463 685f 6964 2c20    for batch_id, 
+0000daf0: 7469 6c65 5f72 6f77 2069 6e20 656e 756d  tile_row in enum
+0000db00: 6572 6174 6528 7469 6c65 735f 6764 662e  erate(tiles_gdf.
+0000db10: 6974 6572 7475 706c 6573 2829 293a 0a20  itertuples()):. 
+0000db20: 2020 2020 2020 2020 2020 2062 6174 6368             batch
+0000db30: 6573 5b62 6174 6368 5f69 645d 203d 207b  es[batch_id] = {
+0000db40: 7d0a 2020 2020 2020 2020 2020 2020 6261  }.            ba
+0000db50: 7463 6865 735b 6261 7463 685f 6964 5d5b  tches[batch_id][
+0000db60: 226c 6179 6572 225d 203d 206f 7574 7075  "layer"] = outpu
+0000db70: 745f 6c61 7965 720a 2020 2020 2020 2020  t_layer.        
+0000db80: 2020 2020 6261 7463 6865 735b 6261 7463      batches[batc
+0000db90: 685f 6964 5d5b 2262 6f75 6e64 7322 5d20  h_id]["bounds"] 
+0000dba0: 3d20 7469 6c65 5f72 6f77 2e67 656f 6d65  = tile_row.geome
+0000dbb0: 7472 792e 626f 756e 6473 0a0a 2020 2020  try.bounds..    
+0000dbc0: 2020 2020 2020 2020 2320 4f75 7470 7574          # Output
+0000dbd0: 2065 6163 6820 6261 7463 6820 746f 2061   each batch to a
+0000dbe0: 2073 6570 6572 6174 6520 7465 6d70 6f72   seperate tempor
+0000dbf0: 6172 7920 6669 6c65 2c20 6f74 6865 7277  ary file, otherw
+0000dc00: 6973 6520 7468 6572 650a 2020 2020 2020  ise there.      
+0000dc10: 2020 2020 2020 2320 6172 6520 7469 6d65        # are time
+0000dc20: 6f75 7420 6973 7375 6573 2077 6865 6e20  out issues when 
+0000dc30: 7072 6f63 6573 7369 6e67 206c 6172 6765  processing large
+0000dc40: 2066 696c 6573 0a20 2020 2020 2020 2020   files.         
+0000dc50: 2020 2073 7566 6669 7820 3d20 6f75 7470     suffix = outp
+0000dc60: 7574 5f6e 6f74 6f6e 626f 7264 6572 5f70  ut_notonborder_p
+0000dc70: 6174 682e 7375 6666 6978 0a20 2020 2020  ath.suffix.     
+0000dc80: 2020 2020 2020 206e 616d 6520 3d20 6622         name = f"
+0000dc90: 7b6f 7574 7075 745f 6e6f 746f 6e62 6f72  {output_notonbor
+0000dca0: 6465 725f 7061 7468 2e73 7465 6d7d 5f7b  der_path.stem}_{
+0000dcb0: 6261 7463 685f 6964 7d7b 7375 6666 6978  batch_id}{suffix
+0000dcc0: 7d22 0a20 2020 2020 2020 2020 2020 206f  }".            o
+0000dcd0: 7574 7075 745f 6e6f 746f 6e62 6f72 6465  utput_notonborde
+0000dce0: 725f 746d 705f 7061 7274 6961 6c5f 7061  r_tmp_partial_pa
+0000dcf0: 7468 203d 2074 656d 7064 6972 202f 206e  th = tempdir / n
+0000dd00: 616d 650a 2020 2020 2020 2020 2020 2020  ame.            
+0000dd10: 6261 7463 6865 735b 6261 7463 685f 6964  batches[batch_id
+0000dd20: 5d5b 0a20 2020 2020 2020 2020 2020 2020  ][.             
+0000dd30: 2020 2022 6f75 7470 7574 5f6e 6f74 6f6e     "output_noton
+0000dd40: 626f 7264 6572 5f74 6d70 5f70 6172 7469  border_tmp_parti
+0000dd50: 616c 5f70 6174 6822 0a20 2020 2020 2020  al_path".       
+0000dd60: 2020 2020 205d 203d 206f 7574 7075 745f       ] = output_
+0000dd70: 6e6f 746f 6e62 6f72 6465 725f 746d 705f  notonborder_tmp_
+0000dd80: 7061 7274 6961 6c5f 7061 7468 0a20 2020  partial_path.   
+0000dd90: 2020 2020 2020 2020 206e 616d 6520 3d20           name = 
+0000dda0: 6622 7b6f 7574 7075 745f 6f6e 626f 7264  f"{output_onbord
+0000ddb0: 6572 5f70 6174 682e 7374 656d 7d5f 7b62  er_path.stem}_{b
+0000ddc0: 6174 6368 5f69 647d 7b73 7566 6669 787d  atch_id}{suffix}
+0000ddd0: 220a 2020 2020 2020 2020 2020 2020 6f75  ".            ou
+0000dde0: 7470 7574 5f6f 6e62 6f72 6465 725f 746d  tput_onborder_tm
+0000ddf0: 705f 7061 7274 6961 6c5f 7061 7468 203d  p_partial_path =
+0000de00: 2074 656d 7064 6972 202f 206e 616d 650a   tempdir / name.
+0000de10: 2020 2020 2020 2020 2020 2020 6261 7463              batc
+0000de20: 6865 735b 6261 7463 685f 6964 5d5b 0a20  hes[batch_id][. 
+0000de30: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000de40: 6f75 7470 7574 5f6f 6e62 6f72 6465 725f  output_onborder_
+0000de50: 746d 705f 7061 7274 6961 6c5f 7061 7468  tmp_partial_path
+0000de60: 220a 2020 2020 2020 2020 2020 2020 5d20  ".            ] 
+0000de70: 3d20 6f75 7470 7574 5f6f 6e62 6f72 6465  = output_onborde
+0000de80: 725f 746d 705f 7061 7274 6961 6c5f 7061  r_tmp_partial_pa
+0000de90: 7468 0a0a 2020 2020 2020 2020 2020 2020  th..            
+0000dea0: 2320 4765 7420 7469 6c65 5f69 6420 6966  # Get tile_id if
+0000deb0: 2070 7265 7365 6e74 0a20 2020 2020 2020   present.       
+0000dec0: 2020 2020 2074 696c 655f 6964 203d 2074       tile_id = t
+0000ded0: 696c 655f 726f 772e 7469 6c65 5f69 6420  ile_row.tile_id 
+0000dee0: 6966 2022 7469 6c65 5f69 6422 2069 6e20  if "tile_id" in 
+0000def0: 7469 6c65 5f72 6f77 2e5f 6669 656c 6473  tile_row._fields
+0000df00: 2065 6c73 6520 4e6f 6e65 0a0a 2020 2020   else None..    
+0000df10: 2020 2020 2020 2020 6675 7475 7265 203d          future =
+0000df20: 2063 616c 6375 6c61 7465 5f70 6f6f 6c2e   calculate_pool.
+0000df30: 7375 626d 6974 280a 2020 2020 2020 2020  submit(.        
+0000df40: 2020 2020 2020 2020 5f64 6973 736f 6c76          _dissolv
+0000df50: 655f 706f 6c79 676f 6e73 2c0a 2020 2020  e_polygons,.    
+0000df60: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
+0000df70: 745f 7061 7468 3d69 6e70 7574 5f70 6174  t_path=input_pat
+0000df80: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
+0000df90: 2020 206f 7574 7075 745f 6e6f 746f 6e62     output_notonb
+0000dfa0: 6f72 6465 725f 7061 7468 3d6f 7574 7075  order_path=outpu
+0000dfb0: 745f 6e6f 746f 6e62 6f72 6465 725f 746d  t_notonborder_tm
+0000dfc0: 705f 7061 7274 6961 6c5f 7061 7468 2c0a  p_partial_path,.
+0000dfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dfe0: 6f75 7470 7574 5f6f 6e62 6f72 6465 725f  output_onborder_
+0000dff0: 7061 7468 3d6f 7574 7075 745f 6f6e 626f  path=output_onbo
+0000e000: 7264 6572 5f74 6d70 5f70 6172 7469 616c  rder_tmp_partial
+0000e010: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
+0000e020: 2020 2020 2020 2065 7870 6c6f 6465 636f         explodeco
+0000e030: 6c6c 6563 7469 6f6e 733d 6578 706c 6f64  llections=explod
+0000e040: 6563 6f6c 6c65 6374 696f 6e73 2c0a 2020  ecollections,.  
+0000e050: 2020 2020 2020 2020 2020 2020 2020 6772                gr
+0000e060: 6f75 7062 795f 636f 6c75 6d6e 733d 6772  oupby_columns=gr
+0000e070: 6f75 7062 795f 636f 6c75 6d6e 732c 0a20  oupby_columns,. 
+0000e080: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+0000e090: 6767 5f63 6f6c 756d 6e73 3d61 6767 5f63  gg_columns=agg_c
+0000e0a0: 6f6c 756d 6e73 2c0a 2020 2020 2020 2020  olumns,.        
+0000e0b0: 2020 2020 2020 2020 696e 7075 745f 6765          input_ge
+0000e0c0: 6f6d 6574 7279 7479 7065 3d69 6e70 7574  ometrytype=input
+0000e0d0: 5f6c 6179 6572 696e 666f 2e67 656f 6d65  _layerinfo.geome
+0000e0e0: 7472 7974 7970 652c 0a20 2020 2020 2020  trytype,.       
+0000e0f0: 2020 2020 2020 2020 2069 6e70 7574 5f6c           input_l
+0000e100: 6179 6572 3d69 6e70 7574 5f6c 6179 6572  ayer=input_layer
+0000e110: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e120: 2020 6f75 7470 7574 5f6c 6179 6572 3d6f    output_layer=o
+0000e130: 7574 7075 745f 6c61 7965 722c 0a20 2020  utput_layer,.   
+0000e140: 2020 2020 2020 2020 2020 2020 2062 626f               bbo
+0000e150: 783d 7469 6c65 5f72 6f77 2e67 656f 6d65  x=tile_row.geome
+0000e160: 7472 792e 626f 756e 6473 2c0a 2020 2020  try.bounds,.    
+0000e170: 2020 2020 2020 2020 2020 2020 7469 6c65              tile
+0000e180: 5f69 643d 7469 6c65 5f69 642c 0a20 2020  _id=tile_id,.   
+0000e190: 2020 2020 2020 2020 2020 2020 2067 7269               gri
+0000e1a0: 6473 697a 653d 6772 6964 7369 7a65 2c0a  dsize=gridsize,.
+0000e1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1c0: 6b65 6570 5f65 6d70 7479 5f67 656f 6d73  keep_empty_geoms
+0000e1d0: 3d6b 6565 705f 656d 7074 795f 6765 6f6d  =keep_empty_geom
+0000e1e0: 732c 0a20 2020 2020 2020 2020 2020 2029  s,.            )
+0000e1f0: 0a20 2020 2020 2020 2020 2020 2066 7574  .            fut
+0000e200: 7572 655f 746f 5f62 6174 6368 5f69 645b  ure_to_batch_id[
+0000e210: 6675 7475 7265 5d20 3d20 6261 7463 685f  future] = batch_
+0000e220: 6964 0a0a 2020 2020 2020 2020 2320 4c6f  id..        # Lo
+0000e230: 6f70 2074 696c 6c20 616c 6c20 7061 7261  op till all para
+0000e240: 6c6c 656c 2070 726f 6365 7373 6573 2061  llel processes a
+0000e250: 7265 2072 6561 6479 2c20 6275 7420 7072  re ready, but pr
+0000e260: 6f63 6573 7320 6561 6368 206f 6e65 0a20  ocess each one. 
+0000e270: 2020 2020 2020 2023 2074 6861 7420 6973         # that is
+0000e280: 2072 6561 6479 2061 6c72 6561 6479 0a20   ready already. 
+0000e290: 2020 2020 2020 205f 6765 6e65 7261 6c5f         _general_
+0000e2a0: 7574 696c 2e72 6570 6f72 745f 7072 6f67  util.report_prog
+0000e2b0: 7265 7373 280a 2020 2020 2020 2020 2020  ress(.          
+0000e2c0: 2020 7374 6172 745f 7469 6d65 2c20 6e62    start_time, nb
+0000e2d0: 5f62 6174 6368 6573 5f64 6f6e 652c 206e  _batches_done, n
+0000e2e0: 625f 6261 7463 6865 732c 2022 6469 7373  b_batches, "diss
+0000e2f0: 6f6c 7665 220a 2020 2020 2020 2020 290a  olve".        ).
+0000e300: 2020 2020 2020 2020 666f 7220 6675 7475          for futu
+0000e310: 7265 2069 6e20 6675 7475 7265 732e 6173  re in futures.as
+0000e320: 5f63 6f6d 706c 6574 6564 2866 7574 7572  _completed(futur
+0000e330: 655f 746f 5f62 6174 6368 5f69 6429 3a0a  e_to_batch_id):.
+0000e340: 2020 2020 2020 2020 2020 2020 7472 793a              try:
+0000e350: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e360: 2023 2049 6620 7468 6520 6361 6c63 756c   # If the calcul
+0000e370: 6174 6520 6761 7665 2072 6573 756c 7473  ate gave results
+0000e380: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e390: 206e 625f 6261 7463 6865 735f 646f 6e65   nb_batches_done
+0000e3a0: 202b 3d20 310a 2020 2020 2020 2020 2020   += 1.          
+0000e3b0: 2020 2020 2020 6261 7463 685f 6964 203d        batch_id =
+0000e3c0: 2066 7574 7572 655f 746f 5f62 6174 6368   future_to_batch
+0000e3d0: 5f69 645b 6675 7475 7265 5d0a 2020 2020  _id[future].    
+0000e3e0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
+0000e3f0: 6c74 203d 2066 7574 7572 652e 7265 7375  lt = future.resu
+0000e400: 6c74 2829 0a0a 2020 2020 2020 2020 2020  lt()..          
+0000e410: 2020 2020 2020 6966 2072 6573 756c 7420        if result 
+0000e420: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000e430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e440: 206e 625f 726f 7773 5f64 6f6e 6520 2b3d   nb_rows_done +=
+0000e450: 2072 6573 756c 745b 226e 625f 726f 7773   result["nb_rows
+0000e460: 5f64 6f6e 6522 5d0a 2020 2020 2020 2020  _done"].        
+0000e470: 2020 2020 2020 2020 2020 2020 6966 2072              if r
+0000e480: 6573 756c 745b 226e 625f 726f 7773 5f64  esult["nb_rows_d
+0000e490: 6f6e 6522 5d20 3e20 3020 616e 6420 7265  one"] > 0 and re
+0000e4a0: 7375 6c74 5b22 746f 7461 6c5f 7469 6d65  sult["total_time
+0000e4b0: 225d 203e 2030 3a0a 2020 2020 2020 2020  "] > 0:.        
+0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4d0: 726f 7773 5f70 6572 5f73 6563 203d 2072  rows_per_sec = r
+0000e4e0: 6f75 6e64 280a 2020 2020 2020 2020 2020  ound(.          
+0000e4f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e500: 2020 7265 7375 6c74 5b22 6e62 5f72 6f77    result["nb_row
+0000e510: 735f 646f 6e65 225d 202f 2072 6573 756c  s_done"] / resul
+0000e520: 745b 2274 6f74 616c 5f74 696d 6522 5d0a  t["total_time"].
+0000e530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e540: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000e550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e560: 2020 6c6f 6767 6572 2e64 6562 7567 280a    logger.debug(.
 0000e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e580: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
-0000e590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e5a0: 2020 2020 2020 2020 2020 2020 2066 2242               f"B
-0000e5b0: 6174 6368 207b 6261 7463 685f 6964 7d20  atch {batch_id} 
-0000e5c0: 7072 6f63 6573 7365 6420 7b72 6573 756c  processed {resul
-0000e5d0: 745b 276e 625f 726f 7773 5f64 6f6e 6527  t['nb_rows_done'
-0000e5e0: 5d7d 2072 6f77 7320 220a 2020 2020 2020  ]} rows ".      
-0000e5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e600: 2020 2020 2020 6622 287b 726f 7773 5f70        f"({rows_p
-0000e610: 6572 5f73 6563 7d2f 7365 6329 220a 2020  er_sec}/sec)".  
-0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e630: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e650: 6966 2022 7065 7266 7374 7269 6e67 2220  if "perfstring" 
-0000e660: 696e 2072 6573 756c 743a 0a20 2020 2020  in result:.     
-0000e670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e680: 2020 2020 2020 206c 6f67 6765 722e 6465         logger.de
-0000e690: 6275 6728 6622 5065 7266 7374 7269 6e67  bug(f"Perfstring
-0000e6a0: 3a20 7b72 6573 756c 745b 2770 6572 6673  : {result['perfs
-0000e6b0: 7472 696e 6727 5d7d 2229 0a0a 2020 2020  tring']}")..    
-0000e6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6d0: 2320 5374 6172 7420 636f 7079 206f 6620  # Start copy of 
-0000e6e0: 7468 6520 7265 7375 6c74 2074 6f20 6120  the result to a 
-0000e6f0: 636f 6d6d 6f6e 2066 696c 650a 2020 2020  common file.    
-0000e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e710: 6261 7463 685f 6964 203d 2066 7574 7572  batch_id = futur
-0000e720: 655f 746f 5f62 6174 6368 5f69 645b 6675  e_to_batch_id[fu
-0000e730: 7475 7265 5d0a 0a20 2020 2020 2020 2020  ture]..         
-0000e740: 2020 2020 2020 2020 2020 2023 2049 6620             # If 
-0000e750: 6361 6c63 756c 6174 6520 6761 7665 206e  calculate gave n
-0000e760: 6f74 6f6e 626f 7264 6572 2072 6573 756c  otonborder resul
-0000e770: 7473 2c20 6170 7065 6e64 2074 6f20 6f75  ts, append to ou
-0000e780: 7470 7574 0a20 2020 2020 2020 2020 2020  tput.           
-0000e790: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-0000e7a0: 6e6f 746f 6e62 6f72 6465 725f 746d 705f  notonborder_tmp_
-0000e7b0: 7061 7274 6961 6c5f 7061 7468 203d 2062  partial_path = b
-0000e7c0: 6174 6368 6573 5b62 6174 6368 5f69 645d  atches[batch_id]
-0000e7d0: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-0000e7e0: 2020 2020 2020 2020 2020 226f 7574 7075            "outpu
-0000e7f0: 745f 6e6f 746f 6e62 6f72 6465 725f 746d  t_notonborder_tm
-0000e800: 705f 7061 7274 6961 6c5f 7061 7468 220a  p_partial_path".
-0000e810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e820: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
-0000e830: 2020 2020 2020 2020 2020 6966 2028 0a20            if (. 
-0000e840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e850: 2020 2020 2020 206f 7574 7075 745f 6e6f         output_no
-0000e860: 746f 6e62 6f72 6465 725f 746d 705f 7061  tonborder_tmp_pa
-0000e870: 7274 6961 6c5f 7061 7468 2e65 7869 7374  rtial_path.exist
-0000e880: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
-0000e890: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-0000e8a0: 6f75 7470 7574 5f6e 6f74 6f6e 626f 7264  output_notonbord
-0000e8b0: 6572 5f74 6d70 5f70 6172 7469 616c 5f70  er_tmp_partial_p
-0000e8c0: 6174 682e 7374 6174 2829 2e73 745f 7369  ath.stat().st_si
-0000e8d0: 7a65 203e 2030 0a20 2020 2020 2020 2020  ze > 0.         
-0000e8e0: 2020 2020 2020 2020 2020 2029 3a0a 2020             ):.  
-0000e8f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e900: 2020 2020 2020 6669 6c65 6f70 732e 5f61        fileops._a
-0000e910: 7070 656e 645f 746f 5f6e 6f6c 6f63 6b28  ppend_to_nolock(
-0000e920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e930: 2020 2020 2020 2020 2020 2020 2073 7263               src
-0000e940: 3d6f 7574 7075 745f 6e6f 746f 6e62 6f72  =output_notonbor
-0000e950: 6465 725f 746d 705f 7061 7274 6961 6c5f  der_tmp_partial_
-0000e960: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
-0000e970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e980: 2020 6473 743d 6f75 7470 7574 5f6e 6f74    dst=output_not
-0000e990: 6f6e 626f 7264 6572 5f70 6174 682c 0a20  onborder_path,. 
-0000e9a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9b0: 2020 2020 2020 2020 2020 2063 7265 6174             creat
-0000e9c0: 655f 7370 6174 6961 6c5f 696e 6465 783d  e_spatial_index=
-0000e9d0: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
-0000e9e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000e9f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ea00: 2020 2020 2020 2020 2067 666f 2e72 656d           gfo.rem
-0000ea10: 6f76 6528 6f75 7470 7574 5f6e 6f74 6f6e  ove(output_noton
-0000ea20: 626f 7264 6572 5f74 6d70 5f70 6172 7469  border_tmp_parti
-0000ea30: 616c 5f70 6174 6829 0a0a 2020 2020 2020  al_path)..      
-0000ea40: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0000ea50: 4966 2063 616c 6375 6c61 7465 2067 6176  If calculate gav
-0000ea60: 6520 6f6e 626f 7264 6572 2072 6573 756c  e onborder resul
-0000ea70: 7473 2c20 6170 7065 6e64 2074 6f20 6f75  ts, append to ou
-0000ea80: 7470 7574 0a20 2020 2020 2020 2020 2020  tput.           
-0000ea90: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-0000eaa0: 6f6e 626f 7264 6572 5f74 6d70 5f70 6172  onborder_tmp_par
-0000eab0: 7469 616c 5f70 6174 6820 3d20 6261 7463  tial_path = batc
-0000eac0: 6865 735b 6261 7463 685f 6964 5d5b 0a20  hes[batch_id][. 
-0000ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eae0: 2020 2020 2020 2022 6f75 7470 7574 5f6f         "output_o
-0000eaf0: 6e62 6f72 6465 725f 746d 705f 7061 7274  nborder_tmp_part
-0000eb00: 6961 6c5f 7061 7468 220a 2020 2020 2020  ial_path".      
-0000eb10: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
+0000e580: 2020 2020 2020 2020 2020 2020 6622 4261              f"Ba
+0000e590: 7463 6820 7b62 6174 6368 5f69 647d 2070  tch {batch_id} p
+0000e5a0: 726f 6365 7373 6564 207b 7265 7375 6c74  rocessed {result
+0000e5b0: 5b27 6e62 5f72 6f77 735f 646f 6e65 275d  ['nb_rows_done']
+0000e5c0: 7d20 726f 7773 2022 0a20 2020 2020 2020  } rows ".       
+0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5e0: 2020 2020 2066 2228 7b72 6f77 735f 7065       f"({rows_pe
+0000e5f0: 725f 7365 637d 2f73 6563 2922 0a20 2020  r_sec}/sec)".   
+0000e600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e610: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+0000e620: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000e630: 6620 2270 6572 6673 7472 696e 6722 2069  f "perfstring" i
+0000e640: 6e20 7265 7375 6c74 3a0a 2020 2020 2020  n result:.      
+0000e650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e660: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
+0000e670: 7567 2866 2250 6572 6673 7472 696e 673a  ug(f"Perfstring:
+0000e680: 207b 7265 7375 6c74 5b27 7065 7266 7374   {result['perfst
+0000e690: 7269 6e67 275d 7d22 290a 0a20 2020 2020  ring']}")..     
+0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000e6b0: 2053 7461 7274 2063 6f70 7920 6f66 2074   Start copy of t
+0000e6c0: 6865 2072 6573 756c 7420 746f 2061 2063  he result to a c
+0000e6d0: 6f6d 6d6f 6e20 6669 6c65 0a20 2020 2020  ommon file.     
+0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0000e6f0: 6174 6368 5f69 6420 3d20 6675 7475 7265  atch_id = future
+0000e700: 5f74 6f5f 6261 7463 685f 6964 5b66 7574  _to_batch_id[fut
+0000e710: 7572 655d 0a0a 2020 2020 2020 2020 2020  ure]..          
+0000e720: 2020 2020 2020 2020 2020 2320 4966 2063            # If c
+0000e730: 616c 6375 6c61 7465 2067 6176 6520 6e6f  alculate gave no
+0000e740: 746f 6e62 6f72 6465 7220 7265 7375 6c74  tonborder result
+0000e750: 732c 2061 7070 656e 6420 746f 206f 7574  s, append to out
+0000e760: 7075 740a 2020 2020 2020 2020 2020 2020  put.            
+0000e770: 2020 2020 2020 2020 6f75 7470 7574 5f6e          output_n
+0000e780: 6f74 6f6e 626f 7264 6572 5f74 6d70 5f70  otonborder_tmp_p
+0000e790: 6172 7469 616c 5f70 6174 6820 3d20 6261  artial_path = ba
+0000e7a0: 7463 6865 735b 6261 7463 685f 6964 5d5b  tches[batch_id][
+0000e7b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e7c0: 2020 2020 2020 2020 2022 6f75 7470 7574           "output
+0000e7d0: 5f6e 6f74 6f6e 626f 7264 6572 5f74 6d70  _notonborder_tmp
+0000e7e0: 5f70 6172 7469 616c 5f70 6174 6822 0a20  _partial_path". 
+0000e7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e800: 2020 205d 0a20 2020 2020 2020 2020 2020     ].           
+0000e810: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
+0000e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e830: 2020 2020 2020 6f75 7470 7574 5f6e 6f74        output_not
+0000e840: 6f6e 626f 7264 6572 5f74 6d70 5f70 6172  onborder_tmp_par
+0000e850: 7469 616c 5f70 6174 682e 6578 6973 7473  tial_path.exists
+0000e860: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+0000e870: 2020 2020 2020 2020 2020 2061 6e64 206f             and o
+0000e880: 7574 7075 745f 6e6f 746f 6e62 6f72 6465  utput_notonborde
+0000e890: 725f 746d 705f 7061 7274 6961 6c5f 7061  r_tmp_partial_pa
+0000e8a0: 7468 2e73 7461 7428 292e 7374 5f73 697a  th.stat().st_siz
+0000e8b0: 6520 3e20 300a 2020 2020 2020 2020 2020  e > 0.          
+0000e8c0: 2020 2020 2020 2020 2020 293a 0a20 2020            ):.   
+0000e8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e8e0: 2020 2020 2066 696c 656f 7073 2e5f 6170       fileops._ap
+0000e8f0: 7065 6e64 5f74 6f5f 6e6f 6c6f 636b 280a  pend_to_nolock(.
+0000e900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e910: 2020 2020 2020 2020 2020 2020 7372 633d              src=
+0000e920: 6f75 7470 7574 5f6e 6f74 6f6e 626f 7264  output_notonbord
+0000e930: 6572 5f74 6d70 5f70 6172 7469 616c 5f70  er_tmp_partial_p
+0000e940: 6174 682c 0a20 2020 2020 2020 2020 2020  ath,.           
+0000e950: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e960: 2064 7374 3d6f 7574 7075 745f 6e6f 746f   dst=output_noto
+0000e970: 6e62 6f72 6465 725f 7061 7468 2c0a 2020  nborder_path,.  
+0000e980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e990: 2020 2020 2020 2020 2020 6372 6561 7465            create
+0000e9a0: 5f73 7061 7469 616c 5f69 6e64 6578 3d46  _spatial_index=F
+0000e9b0: 616c 7365 2c0a 2020 2020 2020 2020 2020  alse,.          
+0000e9c0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000e9d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9e0: 2020 2020 2020 2020 6766 6f2e 7265 6d6f          gfo.remo
+0000e9f0: 7665 286f 7574 7075 745f 6e6f 746f 6e62  ve(output_notonb
+0000ea00: 6f72 6465 725f 746d 705f 7061 7274 6961  order_tmp_partia
+0000ea10: 6c5f 7061 7468 290a 0a20 2020 2020 2020  l_path)..       
+0000ea20: 2020 2020 2020 2020 2020 2020 2023 2049               # I
+0000ea30: 6620 6361 6c63 756c 6174 6520 6761 7665  f calculate gave
+0000ea40: 206f 6e62 6f72 6465 7220 7265 7375 6c74   onborder result
+0000ea50: 732c 2061 7070 656e 6420 746f 206f 7574  s, append to out
+0000ea60: 7075 740a 2020 2020 2020 2020 2020 2020  put.            
+0000ea70: 2020 2020 2020 2020 6f75 7470 7574 5f6f          output_o
+0000ea80: 6e62 6f72 6465 725f 746d 705f 7061 7274  nborder_tmp_part
+0000ea90: 6961 6c5f 7061 7468 203d 2062 6174 6368  ial_path = batch
+0000eaa0: 6573 5b62 6174 6368 5f69 645d 5b0a 2020  es[batch_id][.  
+0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eac0: 2020 2020 2020 226f 7574 7075 745f 6f6e        "output_on
+0000ead0: 626f 7264 6572 5f74 6d70 5f70 6172 7469  border_tmp_parti
+0000eae0: 616c 5f70 6174 6822 0a20 2020 2020 2020  al_path".       
+0000eaf0: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
+0000eb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb10: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
 0000eb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb30: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
-0000eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb50: 206f 7574 7075 745f 6f6e 626f 7264 6572   output_onborder
-0000eb60: 5f74 6d70 5f70 6172 7469 616c 5f70 6174  _tmp_partial_pat
-0000eb70: 682e 6578 6973 7473 2829 0a20 2020 2020  h.exists().     
-0000eb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eb90: 2020 2061 6e64 206f 7574 7075 745f 6f6e     and output_on
-0000eba0: 626f 7264 6572 5f74 6d70 5f70 6172 7469  border_tmp_parti
-0000ebb0: 616c 5f70 6174 682e 7374 6174 2829 2e73  al_path.stat().s
-0000ebc0: 745f 7369 7a65 203e 2030 0a20 2020 2020  t_size > 0.     
-0000ebd0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000ebe0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ebf0: 2020 2020 2020 2020 2020 6669 6c65 6f70            fileop
-0000ec00: 732e 5f61 7070 656e 645f 746f 5f6e 6f6c  s._append_to_nol
-0000ec10: 6f63 6b28 0a20 2020 2020 2020 2020 2020  ock(.           
-0000ec20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec30: 2073 7263 3d6f 7574 7075 745f 6f6e 626f   src=output_onbo
-0000ec40: 7264 6572 5f74 6d70 5f70 6172 7469 616c  rder_tmp_partial
-0000ec50: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
-0000ec60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec70: 2020 2064 7374 3d6f 7574 7075 745f 6f6e     dst=output_on
-0000ec80: 626f 7264 6572 5f70 6174 682c 0a20 2020  border_path,.   
-0000ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eca0: 2020 2020 2020 2020 2063 7265 6174 655f           create_
-0000ecb0: 7370 6174 6961 6c5f 696e 6465 783d 4661  spatial_index=Fa
-0000ecc0: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-0000ecd0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000ece0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ecf0: 2020 2020 2020 2067 666f 2e72 656d 6f76         gfo.remov
-0000ed00: 6528 6f75 7470 7574 5f6f 6e62 6f72 6465  e(output_onborde
-0000ed10: 725f 746d 705f 7061 7274 6961 6c5f 7061  r_tmp_partial_pa
-0000ed20: 7468 290a 0a20 2020 2020 2020 2020 2020  th)..           
-0000ed30: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
-0000ed40: 6e20 6173 2065 783a 0a20 2020 2020 2020  n as ex:.       
-0000ed50: 2020 2020 2020 2020 2062 6174 6368 5f69           batch_i
-0000ed60: 6420 3d20 6675 7475 7265 5f74 6f5f 6261  d = future_to_ba
-0000ed70: 7463 685f 6964 5b66 7574 7572 655d 0a20  tch_id[future]. 
-0000ed80: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000ed90: 6573 7361 6765 203d 2066 2245 7272 6f72  essage = f"Error
-0000eda0: 2065 7865 6375 7469 6e67 207b 6261 7463   executing {batc
-0000edb0: 6865 735b 6261 7463 685f 6964 5d7d 3a20  hes[batch_id]}: 
-0000edc0: 7b65 787d 220a 2020 2020 2020 2020 2020  {ex}".          
-0000edd0: 2020 2020 2020 6c6f 6767 6572 2e65 7863        logger.exc
-0000ede0: 6570 7469 6f6e 286d 6573 7361 6765 290a  eption(message).
-0000edf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee00: 6361 6c63 756c 6174 655f 706f 6f6c 2e73  calculate_pool.s
-0000ee10: 6875 7464 6f77 6e28 290a 2020 2020 2020  hutdown().      
-0000ee20: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000ee30: 4578 6365 7074 696f 6e28 6d65 7373 6167  Exception(messag
-0000ee40: 6529 2066 726f 6d20 6578 0a0a 2020 2020  e) from ex..    
-0000ee50: 2020 2020 2020 2020 2320 4c6f 6720 7468          # Log th
-0000ee60: 6520 7072 6f67 7265 7373 2061 6e64 2070  e progress and p
-0000ee70: 7265 6469 6374 696f 6e20 7370 6565 640a  rediction speed.
-0000ee80: 2020 2020 2020 2020 2020 2020 5f67 656e              _gen
-0000ee90: 6572 616c 5f75 7469 6c2e 7265 706f 7274  eral_util.report
-0000eea0: 5f70 726f 6772 6573 7328 0a20 2020 2020  _progress(.     
-0000eeb0: 2020 2020 2020 2020 2020 2073 7461 7274             start
-0000eec0: 5f74 696d 652c 206e 625f 6261 7463 6865  _time, nb_batche
-0000eed0: 735f 646f 6e65 2c20 6e62 5f62 6174 6368  s_done, nb_batch
-0000eee0: 6573 2c20 2264 6973 736f 6c76 6522 0a20  es, "dissolve". 
-0000eef0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0000ef00: 2020 6c6f 6767 6572 2e69 6e66 6f28 6622    logger.info(f"
-0000ef10: 4469 7373 6f6c 7665 2070 6173 7320 7265  Dissolve pass re
-0000ef20: 6164 792c 2074 6f6f 6b20 7b64 6174 6574  ady, took {datet
-0000ef30: 696d 652e 6e6f 7728 292d 7374 6172 745f  ime.now()-start_
-0000ef40: 7469 6d65 7d21 2229 0a0a 2020 2020 7265  time}!")..    re
-0000ef50: 7475 726e 2072 6573 756c 745f 696e 666f  turn result_info
-0000ef60: 0a0a 0a64 6566 205f 6469 7373 6f6c 7665  ...def _dissolve
-0000ef70: 5f70 6f6c 7967 6f6e 7328 0a20 2020 2069  _polygons(.    i
-0000ef80: 6e70 7574 5f70 6174 683a 2050 6174 682c  nput_path: Path,
-0000ef90: 0a20 2020 206f 7574 7075 745f 6e6f 746f  .    output_noto
-0000efa0: 6e62 6f72 6465 725f 7061 7468 3a20 5061  nborder_path: Pa
-0000efb0: 7468 2c0a 2020 2020 6f75 7470 7574 5f6f  th,.    output_o
-0000efc0: 6e62 6f72 6465 725f 7061 7468 3a20 5061  nborder_path: Pa
-0000efd0: 7468 2c0a 2020 2020 6578 706c 6f64 6563  th,.    explodec
-0000efe0: 6f6c 6c65 6374 696f 6e73 3a20 626f 6f6c  ollections: bool
-0000eff0: 2c0a 2020 2020 6772 6f75 7062 795f 636f  ,.    groupby_co
-0000f000: 6c75 6d6e 733a 204f 7074 696f 6e61 6c5b  lumns: Optional[
-0000f010: 4974 6572 6162 6c65 5b73 7472 5d5d 2c0a  Iterable[str]],.
-0000f020: 2020 2020 6167 675f 636f 6c75 6d6e 733a      agg_columns:
-0000f030: 204f 7074 696f 6e61 6c5b 6469 6374 5d2c   Optional[dict],
-0000f040: 0a20 2020 2069 6e70 7574 5f67 656f 6d65  .    input_geome
-0000f050: 7472 7974 7970 653a 2047 656f 6d65 7472  trytype: Geometr
-0000f060: 7954 7970 652c 0a20 2020 2069 6e70 7574  yType,.    input
+0000eb30: 6f75 7470 7574 5f6f 6e62 6f72 6465 725f  output_onborder_
+0000eb40: 746d 705f 7061 7274 6961 6c5f 7061 7468  tmp_partial_path
+0000eb50: 2e65 7869 7374 7328 290a 2020 2020 2020  .exists().      
+0000eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb70: 2020 616e 6420 6f75 7470 7574 5f6f 6e62    and output_onb
+0000eb80: 6f72 6465 725f 746d 705f 7061 7274 6961  order_tmp_partia
+0000eb90: 6c5f 7061 7468 2e73 7461 7428 292e 7374  l_path.stat().st
+0000eba0: 5f73 697a 6520 3e20 300a 2020 2020 2020  _size > 0.      
+0000ebb0: 2020 2020 2020 2020 2020 2020 2020 293a                ):
+0000ebc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ebd0: 2020 2020 2020 2020 2066 696c 656f 7073           fileops
+0000ebe0: 2e5f 6170 7065 6e64 5f74 6f5f 6e6f 6c6f  ._append_to_nolo
+0000ebf0: 636b 280a 2020 2020 2020 2020 2020 2020  ck(.            
+0000ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec10: 7372 633d 6f75 7470 7574 5f6f 6e62 6f72  src=output_onbor
+0000ec20: 6465 725f 746d 705f 7061 7274 6961 6c5f  der_tmp_partial_
+0000ec30: 7061 7468 2c0a 2020 2020 2020 2020 2020  path,.          
+0000ec40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec50: 2020 6473 743d 6f75 7470 7574 5f6f 6e62    dst=output_onb
+0000ec60: 6f72 6465 725f 7061 7468 2c0a 2020 2020  order_path,.    
+0000ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ec80: 2020 2020 2020 2020 6372 6561 7465 5f73          create_s
+0000ec90: 7061 7469 616c 5f69 6e64 6578 3d46 616c  patial_index=Fal
+0000eca0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
+0000ecb0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+0000ecc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ecd0: 2020 2020 2020 6766 6f2e 7265 6d6f 7665        gfo.remove
+0000ece0: 286f 7574 7075 745f 6f6e 626f 7264 6572  (output_onborder
+0000ecf0: 5f74 6d70 5f70 6172 7469 616c 5f70 6174  _tmp_partial_pat
+0000ed00: 6829 0a0a 2020 2020 2020 2020 2020 2020  h)..            
+0000ed10: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+0000ed20: 2061 7320 6578 3a0a 2020 2020 2020 2020   as ex:.        
+0000ed30: 2020 2020 2020 2020 6261 7463 685f 6964          batch_id
+0000ed40: 203d 2066 7574 7572 655f 746f 5f62 6174   = future_to_bat
+0000ed50: 6368 5f69 645b 6675 7475 7265 5d0a 2020  ch_id[future].  
+0000ed60: 2020 2020 2020 2020 2020 2020 2020 6d65                me
+0000ed70: 7373 6167 6520 3d20 6622 4572 726f 7220  ssage = f"Error 
+0000ed80: 6578 6563 7574 696e 6720 7b62 6174 6368  executing {batch
+0000ed90: 6573 5b62 6174 6368 5f69 645d 7d3a 207b  es[batch_id]}: {
+0000eda0: 6578 7d22 0a20 2020 2020 2020 2020 2020  ex}".           
+0000edb0: 2020 2020 206c 6f67 6765 722e 6578 6365       logger.exce
+0000edc0: 7074 696f 6e28 6d65 7373 6167 6529 0a20  ption(message). 
+0000edd0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000ede0: 616c 6375 6c61 7465 5f70 6f6f 6c2e 7368  alculate_pool.sh
+0000edf0: 7574 646f 776e 2829 0a20 2020 2020 2020  utdown().       
+0000ee00: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+0000ee10: 7863 6570 7469 6f6e 286d 6573 7361 6765  xception(message
+0000ee20: 2920 6672 6f6d 2065 780a 0a20 2020 2020  ) from ex..     
+0000ee30: 2020 2020 2020 2023 204c 6f67 2074 6865         # Log the
+0000ee40: 2070 726f 6772 6573 7320 616e 6420 7072   progress and pr
+0000ee50: 6564 6963 7469 6f6e 2073 7065 6564 0a20  ediction speed. 
+0000ee60: 2020 2020 2020 2020 2020 205f 6765 6e65             _gene
+0000ee70: 7261 6c5f 7574 696c 2e72 6570 6f72 745f  ral_util.report_
+0000ee80: 7072 6f67 7265 7373 280a 2020 2020 2020  progress(.      
+0000ee90: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+0000eea0: 7469 6d65 2c20 6e62 5f62 6174 6368 6573  time, nb_batches
+0000eeb0: 5f64 6f6e 652c 206e 625f 6261 7463 6865  _done, nb_batche
+0000eec0: 732c 2022 6469 7373 6f6c 7665 220a 2020  s, "dissolve".  
+0000eed0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+0000eee0: 206c 6f67 6765 722e 696e 666f 2866 2244   logger.info(f"D
+0000eef0: 6973 736f 6c76 6520 7061 7373 2072 6561  issolve pass rea
+0000ef00: 6479 2c20 746f 6f6b 207b 6461 7465 7469  dy, took {dateti
+0000ef10: 6d65 2e6e 6f77 2829 2d73 7461 7274 5f74  me.now()-start_t
+0000ef20: 696d 657d 2122 290a 0a20 2020 2072 6574  ime}!")..    ret
+0000ef30: 7572 6e20 7265 7375 6c74 5f69 6e66 6f0a  urn result_info.
+0000ef40: 0a0a 6465 6620 5f64 6973 736f 6c76 655f  ..def _dissolve_
+0000ef50: 706f 6c79 676f 6e73 280a 2020 2020 696e  polygons(.    in
+0000ef60: 7075 745f 7061 7468 3a20 5061 7468 2c0a  put_path: Path,.
+0000ef70: 2020 2020 6f75 7470 7574 5f6e 6f74 6f6e      output_noton
+0000ef80: 626f 7264 6572 5f70 6174 683a 2050 6174  border_path: Pat
+0000ef90: 682c 0a20 2020 206f 7574 7075 745f 6f6e  h,.    output_on
+0000efa0: 626f 7264 6572 5f70 6174 683a 2050 6174  border_path: Pat
+0000efb0: 682c 0a20 2020 2065 7870 6c6f 6465 636f  h,.    explodeco
+0000efc0: 6c6c 6563 7469 6f6e 733a 2062 6f6f 6c2c  llections: bool,
+0000efd0: 0a20 2020 2067 726f 7570 6279 5f63 6f6c  .    groupby_col
+0000efe0: 756d 6e73 3a20 4f70 7469 6f6e 616c 5b49  umns: Optional[I
+0000eff0: 7465 7261 626c 655b 7374 725d 5d2c 0a20  terable[str]],. 
+0000f000: 2020 2061 6767 5f63 6f6c 756d 6e73 3a20     agg_columns: 
+0000f010: 4f70 7469 6f6e 616c 5b64 6963 745d 2c0a  Optional[dict],.
+0000f020: 2020 2020 696e 7075 745f 6765 6f6d 6574      input_geomet
+0000f030: 7279 7479 7065 3a20 4765 6f6d 6574 7279  rytype: Geometry
+0000f040: 5479 7065 2c0a 2020 2020 696e 7075 745f  Type,.    input_
+0000f050: 6c61 7965 723a 204f 7074 696f 6e61 6c5b  layer: Optional[
+0000f060: 7374 725d 2c0a 2020 2020 6f75 7470 7574  str],.    output
 0000f070: 5f6c 6179 6572 3a20 4f70 7469 6f6e 616c  _layer: Optional
-0000f080: 5b73 7472 5d2c 0a20 2020 206f 7574 7075  [str],.    outpu
-0000f090: 745f 6c61 7965 723a 204f 7074 696f 6e61  t_layer: Optiona
-0000f0a0: 6c5b 7374 725d 2c0a 2020 2020 6262 6f78  l[str],.    bbox
-0000f0b0: 3a20 5475 706c 655b 666c 6f61 742c 2066  : Tuple[float, f
-0000f0c0: 6c6f 6174 2c20 666c 6f61 742c 2066 6c6f  loat, float, flo
-0000f0d0: 6174 5d2c 0a20 2020 2074 696c 655f 6964  at],.    tile_id
-0000f0e0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d2c  : Optional[int],
-0000f0f0: 0a20 2020 2067 7269 6473 697a 653a 2066  .    gridsize: f
-0000f100: 6c6f 6174 2c0a 2020 2020 6b65 6570 5f65  loat,.    keep_e
-0000f110: 6d70 7479 5f67 656f 6d73 3a20 626f 6f6c  mpty_geoms: bool
-0000f120: 2c0a 2920 2d3e 2064 6963 743a 0a20 2020  ,.) -> dict:.   
-0000f130: 2023 2049 6e69 740a 2020 2020 7065 7266   # Init.    perf
-0000f140: 696e 666f 203d 207b 7d0a 2020 2020 7374  info = {}.    st
-0000f150: 6172 745f 7469 6d65 203d 2064 6174 6574  art_time = datet
-0000f160: 696d 652e 6e6f 7728 290a 2020 2020 7265  ime.now().    re
-0000f170: 7475 726e 5f69 6e66 6f20 3d20 7b0a 2020  turn_info = {.  
-0000f180: 2020 2020 2020 2269 6e70 7574 5f70 6174        "input_pat
-0000f190: 6822 3a20 696e 7075 745f 7061 7468 2c0a  h": input_path,.
-0000f1a0: 2020 2020 2020 2020 226f 7574 7075 745f          "output_
-0000f1b0: 6e6f 746f 6e62 6f72 6465 725f 7061 7468  notonborder_path
-0000f1c0: 223a 206f 7574 7075 745f 6e6f 746f 6e62  ": output_notonb
-0000f1d0: 6f72 6465 725f 7061 7468 2c0a 2020 2020  order_path,.    
-0000f1e0: 2020 2020 226f 7574 7075 745f 6f6e 626f      "output_onbo
-0000f1f0: 7264 6572 5f70 6174 6822 3a20 6f75 7470  rder_path": outp
-0000f200: 7574 5f6f 6e62 6f72 6465 725f 7061 7468  ut_onborder_path
-0000f210: 2c0a 2020 2020 2020 2020 2262 626f 7822  ,.        "bbox"
-0000f220: 3a20 6262 6f78 2c0a 2020 2020 2020 2020  : bbox,.        
-0000f230: 2274 696c 655f 6964 223a 2074 696c 655f  "tile_id": tile_
-0000f240: 6964 2c0a 2020 2020 2020 2020 2267 7269  id,.        "gri
-0000f250: 6473 697a 6522 3a20 6772 6964 7369 7a65  dsize": gridsize
-0000f260: 2c0a 2020 2020 2020 2020 226e 625f 726f  ,.        "nb_ro
-0000f270: 7773 5f64 6f6e 6522 3a20 302c 0a20 2020  ws_done": 0,.   
-0000f280: 2020 2020 2022 746f 7461 6c5f 7469 6d65       "total_time
-0000f290: 223a 2030 2c0a 2020 2020 2020 2020 2270  ": 0,.        "p
-0000f2a0: 6572 6669 6e66 6f22 3a20 2222 2c0a 2020  erfinfo": "",.  
-0000f2b0: 2020 7d0a 0a20 2020 2023 2052 6561 6420    }..    # Read 
-0000f2c0: 616c 6c20 7265 636f 7264 7320 7468 6174  all records that
-0000f2d0: 2061 7265 2069 6e20 7468 6520 6262 6f78   are in the bbox
-0000f2e0: 0a20 2020 2072 6574 7279 5f63 6f75 6e74  .    retry_count
-0000f2f0: 203d 2030 0a20 2020 2073 7461 7274 5f72   = 0.    start_r
-0000f300: 6561 6420 3d20 6461 7465 7469 6d65 2e6e  ead = datetime.n
-0000f310: 6f77 2829 0a20 2020 2061 6767 5f63 6f6c  ow().    agg_col
-0000f320: 756d 6e73 5f6e 6565 6465 6420 3d20 4e6f  umns_needed = No
-0000f330: 6e65 0a20 2020 2077 6869 6c65 2054 7275  ne.    while Tru
-0000f340: 653a 0a20 2020 2020 2020 2074 7279 3a0a  e:.        try:.
-0000f350: 2020 2020 2020 2020 2020 2020 636f 6c75              colu
-0000f360: 6d6e 735f 746f 5f72 6561 6420 3d20 7365  mns_to_read = se
-0000f370: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-0000f380: 696e 666f 203d 2067 666f 2e67 6574 5f6c  info = gfo.get_l
-0000f390: 6179 6572 696e 666f 2869 6e70 7574 5f70  ayerinfo(input_p
-0000f3a0: 6174 682c 2069 6e70 7574 5f6c 6179 6572  ath, input_layer
-0000f3b0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
-0000f3c0: 2067 726f 7570 6279 5f63 6f6c 756d 6e73   groupby_columns
-0000f3d0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-0000f3e0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000f3f0: 6c75 6d6e 735f 746f 5f72 6561 642e 7570  lumns_to_read.up
-0000f400: 6461 7465 2867 726f 7570 6279 5f63 6f6c  date(groupby_col
-0000f410: 756d 6e73 290a 2020 2020 2020 2020 2020  umns).          
-0000f420: 2020 6669 645f 6173 5f69 6e64 6578 203d    fid_as_index =
-0000f430: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-0000f440: 2020 2069 6620 6167 675f 636f 6c75 6d6e     if agg_column
-0000f450: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
-0000f460: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000f470: 6964 5f61 735f 696e 6465 7820 3d20 5472  id_as_index = Tr
-0000f480: 7565 0a20 2020 2020 2020 2020 2020 2020  ue.             
-0000f490: 2020 2069 6620 225f 5f44 4953 534f 4c56     if "__DISSOLV
-0000f4a0: 455f 544f 4a53 4f4e 2220 696e 2069 6e66  E_TOJSON" in inf
-0000f4b0: 6f2e 636f 6c75 6d6e 733a 0a20 2020 2020  o.columns:.     
-0000f4c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000f4d0: 2049 6620 7765 2061 7265 206e 6f74 2069   If we are not i
-0000f4e0: 6e20 7468 6520 6669 7273 7420 7061 7373  n the first pass
-0000f4f0: 2c20 7468 6520 636f 6c75 6d6e 7320 746f  , the columns to
-0000f500: 2062 6520 7265 6164 0a20 2020 2020 2020   be read.       
-0000f510: 2020 2020 2020 2020 2020 2020 2023 2061               # a
-0000f520: 7265 2061 6c72 6561 6479 2069 6e20 7468  re already in th
-0000f530: 6520 6a73 6f6e 2063 6f6c 756d 6e0a 2020  e json column.  
-0000f540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f550: 2020 636f 6c75 6d6e 735f 746f 5f72 6561    columns_to_rea
-0000f560: 642e 6164 6428 225f 5f44 4953 534f 4c56  d.add("__DISSOLV
-0000f570: 455f 544f 4a53 4f4e 2229 0a20 2020 2020  E_TOJSON").     
-0000f580: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000f590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f5a0: 2020 2020 2023 2054 6865 2066 6972 7374       # The first
-0000f5b0: 2070 6173 732c 2073 6f20 7265 6164 2061   pass, so read a
-0000f5c0: 6c6c 2072 656c 6576 616e 7420 636f 6c75  ll relevant colu
-0000f5d0: 6d6e 7320 746f 2063 6f64 650a 2020 2020  mns to code.    
+0000f080: 5b73 7472 5d2c 0a20 2020 2062 626f 783a  [str],.    bbox:
+0000f090: 2054 7570 6c65 5b66 6c6f 6174 2c20 666c   Tuple[float, fl
+0000f0a0: 6f61 742c 2066 6c6f 6174 2c20 666c 6f61  oat, float, floa
+0000f0b0: 745d 2c0a 2020 2020 7469 6c65 5f69 643a  t],.    tile_id:
+0000f0c0: 204f 7074 696f 6e61 6c5b 696e 745d 2c0a   Optional[int],.
+0000f0d0: 2020 2020 6772 6964 7369 7a65 3a20 666c      gridsize: fl
+0000f0e0: 6f61 742c 0a20 2020 206b 6565 705f 656d  oat,.    keep_em
+0000f0f0: 7074 795f 6765 6f6d 733a 2062 6f6f 6c2c  pty_geoms: bool,
+0000f100: 0a29 202d 3e20 6469 6374 3a0a 2020 2020  .) -> dict:.    
+0000f110: 2320 496e 6974 0a20 2020 2070 6572 6669  # Init.    perfi
+0000f120: 6e66 6f20 3d20 7b7d 0a20 2020 2073 7461  nfo = {}.    sta
+0000f130: 7274 5f74 696d 6520 3d20 6461 7465 7469  rt_time = dateti
+0000f140: 6d65 2e6e 6f77 2829 0a20 2020 2072 6574  me.now().    ret
+0000f150: 7572 6e5f 696e 666f 203d 207b 0a20 2020  urn_info = {.   
+0000f160: 2020 2020 2022 696e 7075 745f 7061 7468       "input_path
+0000f170: 223a 2069 6e70 7574 5f70 6174 682c 0a20  ": input_path,. 
+0000f180: 2020 2020 2020 2022 6f75 7470 7574 5f6e         "output_n
+0000f190: 6f74 6f6e 626f 7264 6572 5f70 6174 6822  otonborder_path"
+0000f1a0: 3a20 6f75 7470 7574 5f6e 6f74 6f6e 626f  : output_notonbo
+0000f1b0: 7264 6572 5f70 6174 682c 0a20 2020 2020  rder_path,.     
+0000f1c0: 2020 2022 6f75 7470 7574 5f6f 6e62 6f72     "output_onbor
+0000f1d0: 6465 725f 7061 7468 223a 206f 7574 7075  der_path": outpu
+0000f1e0: 745f 6f6e 626f 7264 6572 5f70 6174 682c  t_onborder_path,
+0000f1f0: 0a20 2020 2020 2020 2022 6262 6f78 223a  .        "bbox":
+0000f200: 2062 626f 782c 0a20 2020 2020 2020 2022   bbox,.        "
+0000f210: 7469 6c65 5f69 6422 3a20 7469 6c65 5f69  tile_id": tile_i
+0000f220: 642c 0a20 2020 2020 2020 2022 6772 6964  d,.        "grid
+0000f230: 7369 7a65 223a 2067 7269 6473 697a 652c  size": gridsize,
+0000f240: 0a20 2020 2020 2020 2022 6e62 5f72 6f77  .        "nb_row
+0000f250: 735f 646f 6e65 223a 2030 2c0a 2020 2020  s_done": 0,.    
+0000f260: 2020 2020 2274 6f74 616c 5f74 696d 6522      "total_time"
+0000f270: 3a20 302c 0a20 2020 2020 2020 2022 7065  : 0,.        "pe
+0000f280: 7266 696e 666f 223a 2022 222c 0a20 2020  rfinfo": "",.   
+0000f290: 207d 0a0a 2020 2020 2320 5265 6164 2061   }..    # Read a
+0000f2a0: 6c6c 2072 6563 6f72 6473 2074 6861 7420  ll records that 
+0000f2b0: 6172 6520 696e 2074 6865 2062 626f 780a  are in the bbox.
+0000f2c0: 2020 2020 7265 7472 795f 636f 756e 7420      retry_count 
+0000f2d0: 3d20 300a 2020 2020 7374 6172 745f 7265  = 0.    start_re
+0000f2e0: 6164 203d 2064 6174 6574 696d 652e 6e6f  ad = datetime.no
+0000f2f0: 7728 290a 2020 2020 6167 675f 636f 6c75  w().    agg_colu
+0000f300: 6d6e 735f 6e65 6564 6564 203d 204e 6f6e  mns_needed = Non
+0000f310: 650a 2020 2020 7768 696c 6520 5472 7565  e.    while True
+0000f320: 3a0a 2020 2020 2020 2020 7472 793a 0a20  :.        try:. 
+0000f330: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
+0000f340: 6e73 5f74 6f5f 7265 6164 203d 2073 6574  ns_to_read = set
+0000f350: 2829 0a20 2020 2020 2020 2020 2020 2069  ().            i
+0000f360: 6e66 6f20 3d20 6766 6f2e 6765 745f 6c61  nfo = gfo.get_la
+0000f370: 7965 7269 6e66 6f28 696e 7075 745f 7061  yerinfo(input_pa
+0000f380: 7468 2c20 696e 7075 745f 6c61 7965 7229  th, input_layer)
+0000f390: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000f3a0: 6772 6f75 7062 795f 636f 6c75 6d6e 7320  groupby_columns 
+0000f3b0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000f3c0: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
+0000f3d0: 756d 6e73 5f74 6f5f 7265 6164 2e75 7064  umns_to_read.upd
+0000f3e0: 6174 6528 6772 6f75 7062 795f 636f 6c75  ate(groupby_colu
+0000f3f0: 6d6e 7329 0a20 2020 2020 2020 2020 2020  mns).           
+0000f400: 2066 6964 5f61 735f 696e 6465 7820 3d20   fid_as_index = 
+0000f410: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+0000f420: 2020 6966 2061 6767 5f63 6f6c 756d 6e73    if agg_columns
+0000f430: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000f440: 2020 2020 2020 2020 2020 2020 2020 6669                fi
+0000f450: 645f 6173 5f69 6e64 6578 203d 2054 7275  d_as_index = Tru
+0000f460: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000f470: 2020 6966 2022 5f5f 4449 5353 4f4c 5645    if "__DISSOLVE
+0000f480: 5f54 4f4a 534f 4e22 2069 6e20 696e 666f  _TOJSON" in info
+0000f490: 2e63 6f6c 756d 6e73 3a0a 2020 2020 2020  .columns:.      
+0000f4a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000f4b0: 4966 2077 6520 6172 6520 6e6f 7420 696e  If we are not in
+0000f4c0: 2074 6865 2066 6972 7374 2070 6173 732c   the first pass,
+0000f4d0: 2074 6865 2063 6f6c 756d 6e73 2074 6f20   the columns to 
+0000f4e0: 6265 2072 6561 640a 2020 2020 2020 2020  be read.        
+0000f4f0: 2020 2020 2020 2020 2020 2020 2320 6172              # ar
+0000f500: 6520 616c 7265 6164 7920 696e 2074 6865  e already in the
+0000f510: 206a 736f 6e20 636f 6c75 6d6e 0a20 2020   json column.   
+0000f520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f530: 2063 6f6c 756d 6e73 5f74 6f5f 7265 6164   columns_to_read
+0000f540: 2e61 6464 2822 5f5f 4449 5353 4f4c 5645  .add("__DISSOLVE
+0000f550: 5f54 4f4a 534f 4e22 290a 2020 2020 2020  _TOJSON").      
+0000f560: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000f570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f580: 2020 2020 2320 5468 6520 6669 7273 7420      # The first 
+0000f590: 7061 7373 2c20 736f 2072 6561 6420 616c  pass, so read al
+0000f5a0: 6c20 7265 6c65 7661 6e74 2063 6f6c 756d  l relevant colum
+0000f5b0: 6e73 2074 6f20 636f 6465 0a20 2020 2020  ns to code.     
+0000f5c0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000f5d0: 2074 6865 6d20 696e 206a 736f 6e0a 2020   them in json.  
 0000f5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f5f0: 2320 7468 656d 2069 6e20 6a73 6f6e 0a20  # them in json. 
-0000f600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f610: 2020 2069 6620 226a 736f 6e22 2069 6e20     if "json" in 
-0000f620: 6167 675f 636f 6c75 6d6e 733a 0a20 2020  agg_columns:.   
-0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f640: 2020 2020 2061 6767 5f63 6f6c 756d 6e73       agg_columns
-0000f650: 5f6e 6565 6465 6420 3d20 6167 675f 636f  _needed = agg_co
-0000f660: 6c75 6d6e 735b 226a 736f 6e22 5d0a 2020  lumns["json"].  
-0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f680: 2020 656c 6966 2022 636f 6c75 6d6e 7322    elif "columns"
-0000f690: 2069 6e20 6167 675f 636f 6c75 6d6e 733a   in agg_columns:
-0000f6a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f6b0: 2020 2020 2020 2020 2061 6767 5f63 6f6c           agg_col
-0000f6c0: 756d 6e73 5f6e 6565 6465 6420 3d20 5b0a  umns_needed = [.
-0000f6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6e0: 2020 2020 2020 2020 2020 2020 6167 675f              agg_
-0000f6f0: 636f 6c75 6d6e 5b22 636f 6c75 6d6e 225d  column["column"]
-0000f700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f710: 2020 2020 2020 2020 2020 2020 2066 6f72               for
-0000f720: 2061 6767 5f63 6f6c 756d 6e20 696e 2061   agg_column in a
-0000f730: 6767 5f63 6f6c 756d 6e73 5b22 636f 6c75  gg_columns["colu
-0000f740: 6d6e 7322 5d0a 2020 2020 2020 2020 2020  mns"].          
-0000f750: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-0000f760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f770: 2020 2020 6966 2061 6767 5f63 6f6c 756d      if agg_colum
-0000f780: 6e73 5f6e 6565 6465 6420 6973 206e 6f74  ns_needed is not
-0000f790: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000f7a0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000f7b0: 6f6c 756d 6e73 5f74 6f5f 7265 6164 2e75  olumns_to_read.u
-0000f7c0: 7064 6174 6528 6167 675f 636f 6c75 6d6e  pdate(agg_column
-0000f7d0: 735f 6e65 6564 6564 290a 0a20 2020 2020  s_needed)..     
-0000f7e0: 2020 2020 2020 2069 6e70 7574 5f67 6466         input_gdf
-0000f7f0: 203d 2067 666f 2e72 6561 645f 6669 6c65   = gfo.read_file
-0000f800: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000f810: 2020 7061 7468 3d69 6e70 7574 5f70 6174    path=input_pat
-0000f820: 682c 0a20 2020 2020 2020 2020 2020 2020  h,.             
-0000f830: 2020 206c 6179 6572 3d69 6e70 7574 5f6c     layer=input_l
-0000f840: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
-0000f850: 2020 2020 2020 6262 6f78 3d62 626f 782c        bbox=bbox,
-0000f860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f870: 2063 6f6c 756d 6e73 3d63 6f6c 756d 6e73   columns=columns
-0000f880: 5f74 6f5f 7265 6164 2c0a 2020 2020 2020  _to_read,.      
-0000f890: 2020 2020 2020 2020 2020 6669 645f 6173            fid_as
-0000f8a0: 5f69 6e64 6578 3d66 6964 5f61 735f 696e  _index=fid_as_in
-0000f8b0: 6465 782c 0a20 2020 2020 2020 2020 2020  dex,.           
-0000f8c0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-0000f8d0: 6966 2061 6767 5f63 6f6c 756d 6e73 2069  if agg_columns i
-0000f8e0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000f8f0: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
-0000f900: 745f 6764 665b 2266 6964 5f6f 7269 6722  t_gdf["fid_orig"
-0000f910: 5d20 3d20 696e 7075 745f 6764 662e 696e  ] = input_gdf.in
-0000f920: 6465 780a 2020 2020 2020 2020 2020 2020  dex.            
-0000f930: 2020 2020 6966 2061 6767 5f63 6f6c 756d      if agg_colum
-0000f940: 6e73 5f6e 6565 6465 6420 6973 206e 6f74  ns_needed is not
-0000f950: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000f960: 2020 2020 2020 2020 2020 2061 6767 5f63             agg_c
-0000f970: 6f6c 756d 6e73 5f6e 6565 6465 642e 6170  olumns_needed.ap
-0000f980: 7065 6e64 2822 6669 645f 6f72 6967 2229  pend("fid_orig")
-0000f990: 0a0a 2020 2020 2020 2020 2020 2020 6272  ..            br
-0000f9a0: 6561 6b0a 2020 2020 2020 2020 6578 6365  eak.        exce
-0000f9b0: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-0000f9c0: 6578 3a0a 2020 2020 2020 2020 2020 2020  ex:.            
-0000f9d0: 6966 2073 7472 2865 7829 203d 3d20 2264  if str(ex) == "d
-0000f9e0: 6174 6162 6173 6520 6973 206c 6f63 6b65  atabase is locke
-0000f9f0: 6422 3a0a 2020 2020 2020 2020 2020 2020  d":.            
-0000fa00: 2020 2020 6966 2072 6574 7279 5f63 6f75      if retry_cou
-0000fa10: 6e74 203c 2031 303a 0a20 2020 2020 2020  nt < 10:.       
-0000fa20: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000fa30: 7279 5f63 6f75 6e74 202b 3d20 310a 2020  ry_count += 1.  
-0000fa40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa50: 2020 7469 6d65 2e73 6c65 6570 2831 290a    time.sleep(1).
-0000fa60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fa70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000fa80: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000fa90: 4578 6365 7074 696f 6e28 2272 6574 7269  Exception("retri
-0000faa0: 6564 2031 3020 7469 6d65 732c 2064 6174  ed 10 times, dat
-0000fab0: 6162 6173 6520 7374 696c 6c20 6c6f 636b  abase still lock
-0000fac0: 6564 2229 2066 726f 6d20 6578 0a20 2020  ed") from ex.   
-0000fad0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-0000fae0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000faf0: 6169 7365 2065 780a 0a20 2020 2023 2043  aise ex..    # C
-0000fb00: 6865 636b 2072 6573 756c 740a 2020 2020  heck result.    
-0000fb10: 7065 7266 696e 666f 5b22 7469 6d65 5f72  perfinfo["time_r
-0000fb20: 6561 6422 5d20 3d20 2864 6174 6574 696d  ead"] = (datetim
-0000fb30: 652e 6e6f 7728 2920 2d20 7374 6172 745f  e.now() - start_
-0000fb40: 7265 6164 292e 746f 7461 6c5f 7365 636f  read).total_seco
-0000fb50: 6e64 7328 290a 2020 2020 7265 7475 726e  nds().    return
-0000fb60: 5f69 6e66 6f5b 226e 625f 726f 7773 5f64  _info["nb_rows_d
-0000fb70: 6f6e 6522 5d20 3d20 6c65 6e28 696e 7075  one"] = len(inpu
-0000fb80: 745f 6764 6629 0a20 2020 2069 6620 7265  t_gdf).    if re
-0000fb90: 7475 726e 5f69 6e66 6f5b 226e 625f 726f  turn_info["nb_ro
-0000fba0: 7773 5f64 6f6e 6522 5d20 3d3d 2030 3a0a  ws_done"] == 0:.
-0000fbb0: 2020 2020 2020 2020 6d65 7373 6167 6520          message 
-0000fbc0: 3d20 6622 4e6f 2069 6e70 7574 2067 656f  = f"No input geo
-0000fbd0: 6d65 7472 6965 7320 666f 756e 6420 696e  metries found in
-0000fbe0: 207b 696e 7075 745f 7061 7468 7d22 0a20   {input_path}". 
-0000fbf0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-0000fc00: 666f 286d 6573 7361 6765 290a 2020 2020  fo(message).    
-0000fc10: 2020 2020 7265 7475 726e 5f69 6e66 6f5b      return_info[
-0000fc20: 226d 6573 7361 6765 225d 203d 206d 6573  "message"] = mes
-0000fc30: 7361 6765 0a20 2020 2020 2020 2072 6574  sage.        ret
-0000fc40: 7572 6e5f 696e 666f 5b22 746f 7461 6c5f  urn_info["total_
-0000fc50: 7469 6d65 225d 203d 2028 6461 7465 7469  time"] = (dateti
-0000fc60: 6d65 2e6e 6f77 2829 202d 2073 7461 7274  me.now() - start
-0000fc70: 5f74 696d 6529 2e74 6f74 616c 5f73 6563  _time).total_sec
-0000fc80: 6f6e 6473 2829 0a20 2020 2020 2020 2072  onds().        r
-0000fc90: 6574 7572 6e20 7265 7475 726e 5f69 6e66  eturn return_inf
-0000fca0: 6f0a 0a20 2020 2023 204e 6f77 2074 6865  o..    # Now the
-0000fcb0: 2072 6561 6c20 7072 6f63 6573 7369 6e67   real processing
-0000fcc0: 0a20 2020 2069 6620 6167 675f 636f 6c75  .    if agg_colu
-0000fcd0: 6d6e 7320 6973 206e 6f74 204e 6f6e 653a  mns is not None:
-0000fce0: 0a20 2020 2020 2020 2069 6620 225f 5f44  .        if "__D
-0000fcf0: 4953 534f 4c56 455f 544f 4a53 4f4e 2220  ISSOLVE_TOJSON" 
-0000fd00: 6e6f 7420 696e 2069 6e70 7574 5f67 6466  not in input_gdf
-0000fd10: 2e63 6f6c 756d 6e73 3a0a 2020 2020 2020  .columns:.      
-0000fd20: 2020 2020 2020 2320 4669 7273 7420 7061        # First pa
-0000fd30: 7373 202d 3e20 7075 7420 7265 6c65 7661  ss -> put releva
-0000fd40: 6e74 2063 6f6c 756d 6e73 2069 6e20 6a73  nt columns in js
-0000fd50: 6f6e 2066 6965 6c64 0a20 2020 2020 2020  on field.       
-0000fd60: 2020 2020 2061 6767 6675 6e63 203d 207b       aggfunc = {
-0000fd70: 2274 6f5f 6a73 6f6e 223a 2061 6767 5f63  "to_json": agg_c
-0000fd80: 6f6c 756d 6e73 5f6e 6565 6465 647d 0a20  olumns_needed}. 
-0000fd90: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000fda0: 2020 2020 2020 2020 2023 2043 6f6c 756d           # Colum
-0000fdb0: 6e73 2061 6c72 6561 6479 2063 6f64 6564  ns already coded
-0000fdc0: 2069 6e20 6120 6a73 6f6e 2063 6f6c 756d   in a json colum
-0000fdd0: 6e2c 2073 6f20 6d65 7267 6520 6a73 6f6e  n, so merge json
-0000fde0: 206c 6973 7473 0a20 2020 2020 2020 2020   lists.         
-0000fdf0: 2020 2061 6767 6675 6e63 203d 2022 6d65     aggfunc = "me
-0000fe00: 7267 655f 6a73 6f6e 5f6c 6973 7473 220a  rge_json_lists".
-0000fe10: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000fe20: 2020 6167 6766 756e 6320 3d20 2266 6972    aggfunc = "fir
-0000fe30: 7374 220a 2020 2020 7374 6172 745f 6469  st".    start_di
-0000fe40: 7373 6f6c 7665 203d 2064 6174 6574 696d  ssolve = datetim
-0000fe50: 652e 6e6f 7728 290a 2020 2020 6469 7373  e.now().    diss
-0000fe60: 5f67 6466 203d 205f 6469 7373 6f6c 7665  _gdf = _dissolve
-0000fe70: 280a 2020 2020 2020 2020 6466 3d69 6e70  (.        df=inp
-0000fe80: 7574 5f67 6466 2c20 6279 3d67 726f 7570  ut_gdf, by=group
-0000fe90: 6279 5f63 6f6c 756d 6e73 2c20 6167 6766  by_columns, aggf
-0000fea0: 756e 633d 6167 6766 756e 632c 2061 735f  unc=aggfunc, as_
-0000feb0: 696e 6465 783d 4661 6c73 652c 2064 726f  index=False, dro
-0000fec0: 706e 613d 4661 6c73 650a 2020 2020 290a  pna=False.    ).
-0000fed0: 2020 2020 7065 7266 696e 666f 5b22 7469      perfinfo["ti
-0000fee0: 6d65 5f64 6973 736f 6c76 6522 5d20 3d20  me_dissolve"] = 
-0000fef0: 2864 6174 6574 696d 652e 6e6f 7728 2920  (datetime.now() 
-0000ff00: 2d20 7374 6172 745f 6469 7373 6f6c 7665  - start_dissolve
-0000ff10: 292e 746f 7461 6c5f 7365 636f 6e64 7328  ).total_seconds(
-0000ff20: 290a 0a20 2020 2023 2049 6620 6578 706c  )..    # If expl
-0000ff30: 6f64 6563 6f6c 6c65 6374 696f 6e73 2069  odecollections i
-0000ff40: 7320 5472 7565 2061 6e64 2046 6f72 2070  s True and For p
-0000ff50: 6f6c 7967 6f6e 732c 2065 7870 6c6f 6465  olygons, explode
-0000ff60: 206d 756c 7469 2d67 656f 6d65 7472 6965   multi-geometrie
-0000ff70: 732e 0a20 2020 2023 2049 6620 6e65 6564  s..    # If need
-0000ff80: 6564 2074 6865 7920 7769 6c6c 2062 6520  ed they will be 
-0000ff90: 2763 6f6c 6c65 6374 6564 2720 6166 7465  'collected' afte
-0000ffa0: 7277 6172 6473 2074 6f20 6d75 6c74 6970  rwards to multip
-0000ffb0: 6f6c 7967 6f6e 7320 6167 6169 6e2e 0a20  olygons again.. 
-0000ffc0: 2020 2069 6620 6578 706c 6f64 6563 6f6c     if explodecol
-0000ffd0: 6c65 6374 696f 6e73 2069 7320 5472 7565  lections is True
-0000ffe0: 206f 7220 696e 7075 745f 6765 6f6d 6574   or input_geomet
-0000fff0: 7279 7479 7065 2069 6e20 5b0a 2020 2020  rytype in [.    
-00010000: 2020 2020 4765 6f6d 6574 7279 5479 7065      GeometryType
-00010010: 2e50 4f4c 5947 4f4e 2c0a 2020 2020 2020  .POLYGON,.      
-00010020: 2020 4765 6f6d 6574 7279 5479 7065 2e4d    GeometryType.M
-00010030: 554c 5449 504f 4c59 474f 4e2c 0a20 2020  ULTIPOLYGON,.   
-00010040: 205d 3a0a 2020 2020 2020 2020 2320 6173   ]:.        # as
-00010050: 7365 7274 2074 6f20 6576 6164 6520 7079  sert to evade py
-00010060: 4c61 6e63 6520 7761 726e 696e 670a 2020  Lance warning.  
-00010070: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
-00010080: 6e73 7461 6e63 6528 6469 7373 5f67 6466  nstance(diss_gdf
-00010090: 2c20 6770 642e 4765 6f44 6174 6146 7261  , gpd.GeoDataFra
-000100a0: 6d65 290a 2020 2020 2020 2020 6469 7373  me).        diss
-000100b0: 5f67 6466 203d 2064 6973 735f 6764 662e  _gdf = diss_gdf.
-000100c0: 6578 706c 6f64 6528 6967 6e6f 7265 5f69  explode(ignore_i
-000100d0: 6e64 6578 3d54 7275 6529 0a0a 2020 2020  ndex=True)..    
-000100e0: 2320 436c 6970 2074 6865 2072 6573 756c  # Clip the resul
-000100f0: 7420 6f6e 2074 6865 2062 6f72 6465 7273  t on the borders
-00010100: 206f 6620 7468 6520 6262 6f78 206e 6f74   of the bbox not
-00010110: 2074 6f20 6861 7665 206f 7665 726c 6170   to have overlap
-00010120: 730a 2020 2020 2320 6265 7477 6565 6e20  s.    # between 
-00010130: 7468 6520 6469 6666 6572 656e 7420 7469  the different ti
-00010140: 6c65 732e 0a20 2020 2023 2049 6620 7468  les..    # If th
-00010150: 6973 2069 7320 6e6f 7420 6170 706c 6965  is is not applie
-00010160: 642c 2074 6869 7320 7265 7375 6c74 7320  d, this results 
-00010170: 696e 2073 6f6d 6520 6765 6f6d 6574 7269  in some geometri
-00010180: 6573 206e 6f74 2062 6569 6e67 206d 6572  es not being mer
-00010190: 6765 640a 2020 2020 2320 6f72 2069 6e20  ged.    # or in 
-000101a0: 6475 706c 6963 6174 6573 2e0a 2020 2020  duplicates..    
-000101b0: 2320 5245 4d41 524b 3a20 666f 7220 286d  # REMARK: for (m
-000101c0: 756c 7469 296c 696e 6573 7472 696e 6773  ulti)linestrings
-000101d0: 2c20 7468 6520 656e 6470 6f69 6e74 7320  , the endpoints 
-000101e0: 6372 6561 7465 6420 6279 2074 6865 2063  created by the c
-000101f0: 6c69 7020 6172 6520 6e6f 740a 2020 2020  lip are not.    
-00010200: 2320 616c 7761 7973 2074 6865 2073 616d  # always the sam
-00010210: 6520 6475 6520 746f 2072 6f75 6e64 696e  e due to roundin
-00010220: 672c 2073 6f20 6469 7373 6f6c 7669 6e67  g, so dissolving
-00010230: 2069 6e20 6120 6e65 7874 2070 6173 7320   in a next pass 
-00010240: 646f 6573 6e27 740a 2020 2020 2320 616c  doesn't.    # al
-00010250: 7761 7973 2072 6573 756c 7420 696e 206c  ways result in l
-00010260: 696e 6573 7472 696e 6773 2062 6569 6e67  inestrings being
-00010270: 2072 652d 636f 6e6e 6563 7465 642e 2e2e   re-connected...
-00010280: 2042 6563 6175 7365 2064 6973 736f 6c76   Because dissolv
-00010290: 696e 670a 2020 2020 2320 6c69 6e65 7320  ing.    # lines 
-000102a0: 6973 6e27 7420 736f 2063 6f6d 7075 7461  isn't so computa
-000102b0: 7469 6f6e 616c 6c79 2068 6561 7679 2061  tionally heavy a
-000102c0: 6e79 7761 792c 2064 726f 7020 7375 7070  nyway, drop supp
-000102d0: 6f72 7420 6865 7265 2e0a 2020 2020 6966  ort here..    if
-000102e0: 2062 626f 7820 6973 206e 6f74 204e 6f6e   bbox is not Non
-000102f0: 653a 0a20 2020 2020 2020 2073 7461 7274  e:.        start
-00010300: 5f63 6c69 7020 3d20 6461 7465 7469 6d65  _clip = datetime
-00010310: 2e6e 6f77 2829 0a20 2020 2020 2020 2062  .now().        b
-00010320: 626f 785f 706f 6c79 676f 6e20 3d20 7368  box_polygon = sh
-00010330: 5f67 656f 6d2e 506f 6c79 676f 6e28 0a20  _geom.Polygon(. 
-00010340: 2020 2020 2020 2020 2020 205b 0a20 2020             [.   
-00010350: 2020 2020 2020 2020 2020 2020 2028 6262               (bb
-00010360: 6f78 5b30 5d2c 2062 626f 785b 315d 292c  ox[0], bbox[1]),
-00010370: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010380: 2028 6262 6f78 5b30 5d2c 2062 626f 785b   (bbox[0], bbox[
-00010390: 335d 292c 0a20 2020 2020 2020 2020 2020  3]),.           
-000103a0: 2020 2020 2028 6262 6f78 5b32 5d2c 2062       (bbox[2], b
-000103b0: 626f 785b 335d 292c 0a20 2020 2020 2020  box[3]),.       
-000103c0: 2020 2020 2020 2020 2028 6262 6f78 5b32           (bbox[2
-000103d0: 5d2c 2062 626f 785b 315d 292c 0a20 2020  ], bbox[1]),.   
-000103e0: 2020 2020 2020 2020 2020 2020 2028 6262               (bb
-000103f0: 6f78 5b30 5d2c 2062 626f 785b 315d 292c  ox[0], bbox[1]),
-00010400: 0a20 2020 2020 2020 2020 2020 205d 0a20  .            ]. 
-00010410: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00010420: 2062 626f 785f 6764 6620 3d20 6770 642e   bbox_gdf = gpd.
-00010430: 4765 6f44 6174 6146 7261 6d65 280a 2020  GeoDataFrame(.  
-00010440: 2020 2020 2020 2020 2020 6461 7461 3d5b            data=[
-00010450: 315d 2c20 6765 6f6d 6574 7279 3d5b 6262  1], geometry=[bb
-00010460: 6f78 5f70 6f6c 7967 6f6e 5d2c 2063 7273  ox_polygon], crs
-00010470: 3d69 6e70 7574 5f67 6466 2e63 7273 0a20  =input_gdf.crs. 
-00010480: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00010490: 2020 2320 4361 7463 6820 6972 7265 6c65    # Catch irrele
-000104a0: 7661 6e74 2070 616e 6461 7320 6675 7475  vant pandas futu
-000104b0: 7265 2077 6172 6e69 6e67 0a20 2020 2020  re warning.     
-000104c0: 2020 2023 2054 4f44 4f3a 2077 6865 6e20     # TODO: when 
-000104d0: 7265 6d6f 7665 6420 696e 206c 6174 6572  removed in later
-000104e0: 2076 6572 7369 6f6e 206f 6620 7061 6e64   version of pand
-000104f0: 6173 2c20 6361 6e20 6265 2072 656d 6f76  as, can be remov
-00010500: 6564 2068 6572 650a 2020 2020 2020 2020  ed here.        
-00010510: 7769 7468 2077 6172 6e69 6e67 732e 6361  with warnings.ca
-00010520: 7463 685f 7761 726e 696e 6773 2829 3a0a  tch_warnings():.
-00010530: 2020 2020 2020 2020 2020 2020 6d65 7373              mess
-00010540: 6167 6520 3d20 280a 2020 2020 2020 2020  age = (.        
-00010550: 2020 2020 2020 2020 2249 6e20 6120 6675          "In a fu
-00010560: 7475 7265 2076 6572 7369 6f6e 2c20 6064  ture version, `d
-00010570: 662e 696c 6f63 5b3a 2c20 695d 203d 206e  f.iloc[:, i] = n
-00010580: 6577 7661 6c73 6020 7769 6c6c 2061 7474  ewvals` will att
-00010590: 656d 7074 2074 6f20 220a 2020 2020 2020  empt to ".      
-000105a0: 2020 2020 2020 2020 2020 2273 6574 2074            "set t
-000105b0: 6865 2076 616c 7565 7320 696e 706c 6163  he values inplac
-000105c0: 6520 696e 7374 6561 6420 6f66 2061 6c77  e instead of alw
-000105d0: 6179 7320 7365 7474 696e 6720 6120 6e65  ays setting a ne
-000105e0: 7720 6172 7261 792e 220a 2020 2020 2020  w array.".      
-000105f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00010600: 2020 2020 7761 726e 696e 6773 2e66 696c      warnings.fil
-00010610: 7465 7277 6172 6e69 6e67 7328 0a20 2020  terwarnings(.   
-00010620: 2020 2020 2020 2020 2020 2020 2061 6374               act
-00010630: 696f 6e3d 2269 676e 6f72 6522 2c20 6361  ion="ignore", ca
-00010640: 7465 676f 7279 3d46 7574 7572 6557 6172  tegory=FutureWar
-00010650: 6e69 6e67 2c20 6d65 7373 6167 653d 7265  ning, message=re
-00010660: 2e65 7363 6170 6528 6d65 7373 6167 6529  .escape(message)
-00010670: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-00010680: 2020 2020 2020 2020 2020 2023 206b 6565             # kee
-00010690: 705f 6765 6f6d 5f74 7970 653d 5472 7565  p_geom_type=True
-000106a0: 2067 6176 6520 736f 6d65 7469 6d65 7320   gave sometimes 
-000106b0: 6572 726f 722c 2061 6e64 2073 7469 6c6c  error, and still
-000106c0: 2064 6f65 7320 696e 2030 2e39 2e30 0a20   does in 0.9.0. 
-000106d0: 2020 2020 2020 2020 2020 2023 2073 6f20             # so 
-000106e0: 7573 6520 6f77 6e20 696d 706c 656d 656e  use own implemen
-000106f0: 7461 7469 6f6e 206f 6620 6b65 6570 5f67  tation of keep_g
-00010700: 656f 6d5f 7479 7065 0a20 2020 2020 2020  eom_type.       
-00010710: 2020 2020 2064 6973 735f 6764 6620 3d20       diss_gdf = 
-00010720: 6770 642e 636c 6970 2864 6973 735f 6764  gpd.clip(diss_gd
-00010730: 662c 2062 626f 785f 6764 6629 2020 2320  f, bbox_gdf)  # 
-00010740: 2c20 6b65 6570 5f67 656f 6d5f 7479 7065  , keep_geom_type
-00010750: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00010760: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
-00010770: 616e 6365 2864 6973 735f 6764 662c 2067  ance(diss_gdf, g
-00010780: 7064 2e47 656f 4461 7461 4672 616d 6529  pd.GeoDataFrame)
-00010790: 0a0a 2020 2020 2020 2020 2320 4f6e 6c79  ..        # Only
-000107a0: 206b 6565 7020 6765 6f6d 6574 7269 6573   keep geometries
-000107b0: 206f 6620 7468 6520 7072 696d 6974 6976   of the primitiv
-000107c0: 6520 7479 7065 2073 7065 6369 6669 6564  e type specified
-000107d0: 2061 6674 6572 2063 6c69 702e 2e2e 0a20   after clip.... 
-000107e0: 2020 2020 2020 2061 7373 6572 7420 6973         assert is
-000107f0: 696e 7374 616e 6365 2864 6973 735f 6764  instance(diss_gd
-00010800: 662c 2067 7064 2e47 656f 4461 7461 4672  f, gpd.GeoDataFr
-00010810: 616d 6529 0a20 2020 2020 2020 2064 6973  ame).        dis
-00010820: 735f 6764 662e 6765 6f6d 6574 7279 203d  s_gdf.geometry =
-00010830: 2067 656f 7365 7269 6573 5f75 7469 6c2e   geoseries_util.
-00010840: 6765 6f6d 6574 7279 5f63 6f6c 6c65 6374  geometry_collect
-00010850: 696f 6e5f 6578 7472 6163 7428 0a20 2020  ion_extract(.   
-00010860: 2020 2020 2020 2020 2064 6973 735f 6764           diss_gd
-00010870: 662e 6765 6f6d 6574 7279 2c20 696e 7075  f.geometry, inpu
-00010880: 745f 6765 6f6d 6574 7279 7479 7065 2e74  t_geometrytype.t
-00010890: 6f5f 7072 696d 6974 6976 6574 7970 650a  o_primitivetype.
-000108a0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-000108b0: 2020 2070 6572 6669 6e66 6f5b 2274 696d     perfinfo["tim
-000108c0: 655f 636c 6970 225d 203d 2028 6461 7465  e_clip"] = (date
-000108d0: 7469 6d65 2e6e 6f77 2829 202d 2073 7461  time.now() - sta
-000108e0: 7274 5f63 6c69 7029 2e74 6f74 616c 5f73  rt_clip).total_s
-000108f0: 6563 6f6e 6473 2829 0a0a 2020 2020 2320  econds()..    # 
-00010900: 5365 7420 656d 7074 7920 6765 6f6d 6574  Set empty geomet
-00010910: 7269 6573 2074 6f20 6e75 6c6c 2f4e 6f6e  ries to null/Non
-00010920: 650a 2020 2020 6173 7365 7274 2064 6973  e.    assert dis
-00010930: 735f 6764 662e 6765 6f6d 6574 7279 2069  s_gdf.geometry i
-00010940: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2064  s not None.    d
-00010950: 6973 735f 6764 662e 6c6f 635b 6469 7373  iss_gdf.loc[diss
-00010960: 5f67 6466 2e67 656f 6d65 7472 792e 6973  _gdf.geometry.is
-00010970: 5f65 6d70 7479 2c20 5b22 6765 6f6d 6574  _empty, ["geomet
-00010980: 7279 225d 5d20 3d20 4e6f 6e65 0a0a 2020  ry"]] = None..  
-00010990: 2020 2320 5265 6d6f 7665 2072 6f77 7320    # Remove rows 
-000109a0: 7768 6572 6520 6765 6f6d 2069 7320 4e6f  where geom is No
-000109b0: 6e65 2f6e 756c 6c2f 656d 7074 790a 2020  ne/null/empty.  
-000109c0: 2020 6966 206e 6f74 206b 6565 705f 656d    if not keep_em
-000109d0: 7074 795f 6765 6f6d 733a 0a20 2020 2020  pty_geoms:.     
-000109e0: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
-000109f0: 616e 6365 2864 6973 735f 6764 662c 2067  ance(diss_gdf, g
-00010a00: 7064 2e47 656f 4461 7461 4672 616d 6529  pd.GeoDataFrame)
-00010a10: 0a20 2020 2020 2020 2064 6973 735f 6764  .        diss_gd
-00010a20: 6620 3d20 6469 7373 5f67 6466 5b7e 6469  f = diss_gdf[~di
-00010a30: 7373 5f67 6466 2e67 656f 6d65 7472 792e  ss_gdf.geometry.
-00010a40: 6973 6e61 2829 5d0a 0a20 2020 2023 2049  isna()]..    # I
-00010a50: 6620 7468 6572 6520 6973 206e 6f20 7265  f there is no re
-00010a60: 7375 6c74 2c20 7265 7475 726e 0a20 2020  sult, return.   
-00010a70: 2069 6620 6c65 6e28 6469 7373 5f67 6466   if len(diss_gdf
-00010a80: 2920 3d3d 2030 3a0a 2020 2020 2020 2020  ) == 0:.        
-00010a90: 6d65 7373 6167 6520 3d20 6622 5265 7375  message = f"Resu
-00010aa0: 6c74 2069 7320 656d 7074 7920 666f 7220  lt is empty for 
-00010ab0: 7b69 6e70 7574 5f70 6174 687d 220a 2020  {input_path}".  
-00010ac0: 2020 2020 2020 7265 7475 726e 5f69 6e66        return_inf
-00010ad0: 6f5b 226d 6573 7361 6765 225d 203d 206d  o["message"] = m
-00010ae0: 6573 7361 6765 0a20 2020 2020 2020 2072  essage.        r
-00010af0: 6574 7572 6e5f 696e 666f 5b22 7065 7266  eturn_info["perf
-00010b00: 696e 666f 225d 203d 2070 6572 6669 6e66  info"] = perfinf
-00010b10: 6f0a 2020 2020 2020 2020 7265 7475 726e  o.        return
-00010b20: 5f69 6e66 6f5b 2274 6f74 616c 5f74 696d  _info["total_tim
-00010b30: 6522 5d20 3d20 2864 6174 6574 696d 652e  e"] = (datetime.
-00010b40: 6e6f 7728 2920 2d20 7374 6172 745f 7469  now() - start_ti
-00010b50: 6d65 292e 746f 7461 6c5f 7365 636f 6e64  me).total_second
-00010b60: 7328 290a 2020 2020 2020 2020 7265 7475  s().        retu
-00010b70: 726e 2072 6574 7572 6e5f 696e 666f 0a0a  rn return_info..
-00010b80: 2020 2020 2320 4164 6420 636f 6c75 6d6e      # Add column
-00010b90: 2077 6974 6820 7469 6c65 5f69 640a 2020   with tile_id.  
-00010ba0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
-00010bb0: 6e63 6528 6469 7373 5f67 6466 2c20 6770  nce(diss_gdf, gp
-00010bc0: 642e 4765 6f44 6174 6146 7261 6d65 290a  d.GeoDataFrame).
-00010bd0: 2020 2020 6966 2074 696c 655f 6964 2069      if tile_id i
-00010be0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00010bf0: 2020 2020 6469 7373 5f67 6466 5b22 7469      diss_gdf["ti
-00010c00: 6c65 5f69 6422 5d20 3d20 7469 6c65 5f69  le_id"] = tile_i
-00010c10: 640a 0a20 2020 2069 6620 6772 6964 7369  d..    if gridsi
-00010c20: 7a65 2021 3d20 302e 303a 0a20 2020 2020  ze != 0.0:.     
-00010c30: 2020 2064 6973 735f 6764 662e 6765 6f6d     diss_gdf.geom
-00010c40: 6574 7279 203d 2073 6861 7065 6c79 325f  etry = shapely2_
-00010c50: 6f72 5f70 7967 656f 732e 7365 745f 7072  or_pygeos.set_pr
-00010c60: 6563 6973 696f 6e28 0a20 2020 2020 2020  ecision(.       
-00010c70: 2020 2020 2064 6973 735f 6764 662e 6765       diss_gdf.ge
-00010c80: 6f6d 6574 7279 2e61 7272 6179 2e64 6174  ometry.array.dat
-00010c90: 612c 2067 7269 645f 7369 7a65 3d67 7269  a, grid_size=gri
-00010ca0: 6473 697a 650a 2020 2020 2020 2020 290a  dsize.        ).
-00010cb0: 0a20 2020 2023 2053 6176 6520 7468 6520  .    # Save the 
-00010cc0: 7265 7375 6c74 2074 6f20 6465 7374 696e  result to destin
-00010cd0: 6174 696f 6e20 6669 6c65 2873 290a 2020  ation file(s).  
-00010ce0: 2020 7374 6172 745f 746f 5f66 696c 6520    start_to_file 
-00010cf0: 3d20 6461 7465 7469 6d65 2e6e 6f77 2829  = datetime.now()
-00010d00: 0a0a 2020 2020 2320 4966 2074 6865 2074  ..    # If the t
-00010d10: 696c 6573 2064 6f6e 2774 206e 6565 6420  iles don't need 
-00010d20: 746f 2062 6520 6d65 7267 6564 2061 6674  to be merged aft
-00010d30: 6572 7761 7264 732c 2077 6520 6361 6e20  erwards, we can 
-00010d40: 6a75 7374 2073 6176 6520 7468 6520 7265  just save the re
-00010d50: 7375 6c74 2061 730a 2020 2020 2320 6974  sult as.    # it
-00010d60: 2069 732e 0a20 2020 2069 6620 7374 7228   is..    if str(
-00010d70: 6f75 7470 7574 5f6e 6f74 6f6e 626f 7264  output_notonbord
-00010d80: 6572 5f70 6174 6829 203d 3d20 7374 7228  er_path) == str(
-00010d90: 6f75 7470 7574 5f6f 6e62 6f72 6465 725f  output_onborder_
-00010da0: 7061 7468 293a 0a20 2020 2020 2020 2023  path):.        #
-00010db0: 2061 7373 6572 7420 746f 2065 7661 6465   assert to evade
-00010dc0: 2070 794c 616e 6365 2077 6172 6e69 6e67   pyLance warning
-00010dd0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00010de0: 6973 696e 7374 616e 6365 2864 6973 735f  isinstance(diss_
-00010df0: 6764 662c 2067 7064 2e47 656f 4461 7461  gdf, gpd.GeoData
-00010e00: 4672 616d 6529 0a20 2020 2020 2020 2023  Frame).        #
-00010e10: 2055 7365 2066 6f72 6365 5f6d 756c 7469   Use force_multi
-00010e20: 7479 7065 2c20 746f 2065 7661 6465 2077  type, to evade w
-00010e30: 6172 6e69 6e67 7320 7768 656e 2073 6f6d  arnings when som
-00010e40: 6520 6261 7463 6865 7320 636f 6e74 6169  e batches contai
-00010e50: 6e0a 2020 2020 2020 2020 2320 7369 6e67  n.        # sing
-00010e60: 6c65 7479 7065 2061 6e64 2073 6f6d 6520  letype and some 
-00010e70: 636f 6e74 6169 6e20 6d75 6c74 6974 7970  contain multityp
-00010e80: 6520 6765 6f6d 6574 7269 6573 0a20 2020  e geometries.   
-00010e90: 2020 2020 2067 666f 2e74 6f5f 6669 6c65       gfo.to_file
-00010ea0: 280a 2020 2020 2020 2020 2020 2020 6469  (.            di
-00010eb0: 7373 5f67 6466 2c0a 2020 2020 2020 2020  ss_gdf,.        
-00010ec0: 2020 2020 6f75 7470 7574 5f6e 6f74 6f6e      output_noton
-00010ed0: 626f 7264 6572 5f70 6174 682c 0a20 2020  border_path,.   
-00010ee0: 2020 2020 2020 2020 206c 6179 6572 3d6f           layer=o
-00010ef0: 7574 7075 745f 6c61 7965 722c 0a20 2020  utput_layer,.   
-00010f00: 2020 2020 2020 2020 2066 6f72 6365 5f6d           force_m
-00010f10: 756c 7469 7479 7065 3d54 7275 652c 0a20  ultitype=True,. 
-00010f20: 2020 2020 2020 2020 2020 2069 6e64 6578             index
-00010f30: 3d46 616c 7365 2c0a 2020 2020 2020 2020  =False,.        
-00010f40: 2020 2020 6372 6561 7465 5f73 7061 7469      create_spati
-00010f50: 616c 5f69 6e64 6578 3d46 616c 7365 2c0a  al_index=False,.
-00010f60: 2020 2020 2020 2020 290a 2020 2020 656c          ).    el
-00010f70: 7365 3a0a 2020 2020 2020 2020 2320 4966  se:.        # If
-00010f80: 206e 6f74 2c20 7361 7665 2074 6865 2070   not, save the p
-00010f90: 6f6c 7967 6f6e 7320 6f6e 2074 6865 2062  olygons on the b
-00010fa0: 6f72 6465 7220 7365 7065 7261 7465 6c79  order seperately
-00010fb0: 0a20 2020 2020 2020 2062 626f 785f 6c69  .        bbox_li
-00010fc0: 6e65 735f 6764 6620 3d20 6770 642e 4765  nes_gdf = gpd.Ge
-00010fd0: 6f44 6174 6146 7261 6d65 280a 2020 2020  oDataFrame(.    
-00010fe0: 2020 2020 2020 2020 6765 6f6d 6574 7279          geometry
-00010ff0: 3d67 656f 7365 7269 6573 5f75 7469 6c2e  =geoseries_util.
-00011000: 706f 6c79 676f 6e73 5f74 6f5f 6c69 6e65  polygons_to_line
-00011010: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
-00011020: 2020 2067 7064 2e47 656f 5365 7269 6573     gpd.GeoSeries
-00011030: 285b 7368 5f67 656f 6d2e 626f 7828 6262  ([sh_geom.box(bb
-00011040: 6f78 5b30 5d2c 2062 626f 785b 315d 2c20  ox[0], bbox[1], 
-00011050: 6262 6f78 5b32 5d2c 2062 626f 785b 335d  bbox[2], bbox[3]
-00011060: 295d 290a 2020 2020 2020 2020 2020 2020  )]).            
-00011070: 292c 0a20 2020 2020 2020 2020 2020 2063  ),.            c
-00011080: 7273 3d69 6e70 7574 5f67 6466 2e63 7273  rs=input_gdf.crs
-00011090: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
-000110a0: 2020 2020 6f6e 626f 7264 6572 5f67 6466      onborder_gdf
-000110b0: 203d 2067 7064 2e73 6a6f 696e 2864 6973   = gpd.sjoin(dis
-000110c0: 735f 6764 662c 2062 626f 785f 6c69 6e65  s_gdf, bbox_line
-000110d0: 735f 6764 662c 2070 7265 6469 6361 7465  s_gdf, predicate
-000110e0: 3d22 696e 7465 7273 6563 7473 2229 0a20  ="intersects"). 
-000110f0: 2020 2020 2020 206f 6e62 6f72 6465 725f         onborder_
-00011100: 6764 662e 6472 6f70 2822 696e 6465 785f  gdf.drop("index_
-00011110: 7269 6768 7422 2c20 6178 6973 3d31 2c20  right", axis=1, 
-00011120: 696e 706c 6163 653d 5472 7565 290a 2020  inplace=True).  
-00011130: 2020 2020 2020 6966 206c 656e 286f 6e62        if len(onb
-00011140: 6f72 6465 725f 6764 6629 203e 2030 3a0a  order_gdf) > 0:.
-00011150: 2020 2020 2020 2020 2020 2020 2320 6173              # as
-00011160: 7365 7274 2074 6f20 6576 6164 6520 7079  sert to evade py
-00011170: 4c61 6e63 6520 7761 726e 696e 670a 2020  Lance warning.  
-00011180: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00011190: 2069 7369 6e73 7461 6e63 6528 6f6e 626f   isinstance(onbo
-000111a0: 7264 6572 5f67 6466 2c20 6770 642e 4765  rder_gdf, gpd.Ge
-000111b0: 6f44 6174 6146 7261 6d65 290a 2020 2020  oDataFrame).    
-000111c0: 2020 2020 2020 2020 2320 5573 6520 666f          # Use fo
-000111d0: 7263 655f 6d75 6c74 6974 7970 652c 2074  rce_multitype, t
-000111e0: 6f20 6576 6164 6520 7761 726e 696e 6773  o evade warnings
-000111f0: 2077 6865 6e20 736f 6d65 2062 6174 6368   when some batch
-00011200: 6573 2063 6f6e 7461 696e 0a20 2020 2020  es contain.     
-00011210: 2020 2020 2020 2023 2073 696e 676c 6574         # singlet
-00011220: 7970 6520 616e 6420 736f 6d65 2063 6f6e  ype and some con
-00011230: 7461 696e 206d 756c 7469 7479 7065 2067  tain multitype g
-00011240: 656f 6d65 7472 6965 730a 2020 2020 2020  eometries.      
-00011250: 2020 2020 2020 6766 6f2e 746f 5f66 696c        gfo.to_fil
-00011260: 6528 0a20 2020 2020 2020 2020 2020 2020  e(.             
-00011270: 2020 206f 6e62 6f72 6465 725f 6764 662c     onborder_gdf,
-00011280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011290: 206f 7574 7075 745f 6f6e 626f 7264 6572   output_onborder
-000112a0: 5f70 6174 682c 0a20 2020 2020 2020 2020  _path,.         
-000112b0: 2020 2020 2020 206c 6179 6572 3d6f 7574         layer=out
-000112c0: 7075 745f 6c61 7965 722c 0a20 2020 2020  put_layer,.     
-000112d0: 2020 2020 2020 2020 2020 2066 6f72 6365             force
-000112e0: 5f6d 756c 7469 7479 7065 3d54 7275 652c  _multitype=True,
-000112f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011300: 2063 7265 6174 655f 7370 6174 6961 6c5f   create_spatial_
-00011310: 696e 6465 783d 4661 6c73 652c 0a20 2020  index=False,.   
-00011320: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00011330: 2020 2020 6e6f 746f 6e62 6f72 6465 725f      notonborder_
-00011340: 6764 6620 3d20 6469 7373 5f67 6466 5b7e  gdf = diss_gdf[~
-00011350: 6469 7373 5f67 6466 2e69 6e64 6578 2e69  diss_gdf.index.i
-00011360: 7369 6e28 6f6e 626f 7264 6572 5f67 6466  sin(onborder_gdf
-00011370: 2e69 6e64 6578 295d 0a20 2020 2020 2020  .index)].       
-00011380: 2069 6620 6c65 6e28 6e6f 746f 6e62 6f72   if len(notonbor
-00011390: 6465 725f 6764 6629 203e 2030 3a0a 2020  der_gdf) > 0:.  
-000113a0: 2020 2020 2020 2020 2020 2320 6173 7365            # asse
-000113b0: 7274 2074 6f20 6576 6164 6520 7079 4c61  rt to evade pyLa
-000113c0: 6e63 6520 7761 726e 696e 670a 2020 2020  nce warning.    
-000113d0: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-000113e0: 7369 6e73 7461 6e63 6528 6e6f 746f 6e62  sinstance(notonb
-000113f0: 6f72 6465 725f 6764 662c 2067 7064 2e47  order_gdf, gpd.G
-00011400: 656f 4461 7461 4672 616d 6529 0a20 2020  eoDataFrame).   
-00011410: 2020 2020 2020 2020 2023 2055 7365 2066           # Use f
-00011420: 6f72 6365 5f6d 756c 7469 7479 7065 2c20  orce_multitype, 
-00011430: 746f 2065 7661 6465 2077 6172 6e69 6e67  to evade warning
-00011440: 7320 7768 656e 2073 6f6d 6520 6261 7463  s when some batc
-00011450: 6865 7320 636f 6e74 6169 6e0a 2020 2020  hes contain.    
-00011460: 2020 2020 2020 2020 2320 7369 6e67 6c65          # single
-00011470: 7479 7065 2061 6e64 2073 6f6d 6520 636f  type and some co
-00011480: 6e74 6169 6e20 6d75 6c74 6974 7970 6520  ntain multitype 
-00011490: 6765 6f6d 6574 7269 6573 0a20 2020 2020  geometries.     
-000114a0: 2020 2020 2020 2067 666f 2e74 6f5f 6669         gfo.to_fi
-000114b0: 6c65 280a 2020 2020 2020 2020 2020 2020  le(.            
-000114c0: 2020 2020 6e6f 746f 6e62 6f72 6465 725f      notonborder_
-000114d0: 6764 662c 0a20 2020 2020 2020 2020 2020  gdf,.           
-000114e0: 2020 2020 206f 7574 7075 745f 6e6f 746f       output_noto
-000114f0: 6e62 6f72 6465 725f 7061 7468 2c0a 2020  nborder_path,.  
-00011500: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-00011510: 7965 723d 6f75 7470 7574 5f6c 6179 6572  yer=output_layer
-00011520: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011530: 2020 666f 7263 655f 6d75 6c74 6974 7970    force_multityp
-00011540: 653d 5472 7565 2c0a 2020 2020 2020 2020  e=True,.        
-00011550: 2020 2020 2020 2020 696e 6465 783d 4661          index=Fa
+0000f5f0: 2020 6966 2022 6a73 6f6e 2220 696e 2061    if "json" in a
+0000f600: 6767 5f63 6f6c 756d 6e73 3a0a 2020 2020  gg_columns:.    
+0000f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f620: 2020 2020 6167 675f 636f 6c75 6d6e 735f      agg_columns_
+0000f630: 6e65 6564 6564 203d 2061 6767 5f63 6f6c  needed = agg_col
+0000f640: 756d 6e73 5b22 6a73 6f6e 225d 0a20 2020  umns["json"].   
+0000f650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f660: 2065 6c69 6620 2263 6f6c 756d 6e73 2220   elif "columns" 
+0000f670: 696e 2061 6767 5f63 6f6c 756d 6e73 3a0a  in agg_columns:.
+0000f680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f690: 2020 2020 2020 2020 6167 675f 636f 6c75          agg_colu
+0000f6a0: 6d6e 735f 6e65 6564 6564 203d 205b 0a20  mns_needed = [. 
+0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6c0: 2020 2020 2020 2020 2020 2061 6767 5f63             agg_c
+0000f6d0: 6f6c 756d 6e5b 2263 6f6c 756d 6e22 5d0a  olumn["column"].
+0000f6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000f700: 6167 675f 636f 6c75 6d6e 2069 6e20 6167  agg_column in ag
+0000f710: 675f 636f 6c75 6d6e 735b 2263 6f6c 756d  g_columns["colum
+0000f720: 6e73 225d 0a20 2020 2020 2020 2020 2020  ns"].           
+0000f730: 2020 2020 2020 2020 2020 2020 205d 0a20               ]. 
+0000f740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f750: 2020 2069 6620 6167 675f 636f 6c75 6d6e     if agg_column
+0000f760: 735f 6e65 6564 6564 2069 7320 6e6f 7420  s_needed is not 
+0000f770: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000f780: 2020 2020 2020 2020 2020 2020 2020 636f                co
+0000f790: 6c75 6d6e 735f 746f 5f72 6561 642e 7570  lumns_to_read.up
+0000f7a0: 6461 7465 2861 6767 5f63 6f6c 756d 6e73  date(agg_columns
+0000f7b0: 5f6e 6565 6465 6429 0a0a 2020 2020 2020  _needed)..      
+0000f7c0: 2020 2020 2020 696e 7075 745f 6764 6620        input_gdf 
+0000f7d0: 3d20 6766 6f2e 7265 6164 5f66 696c 6528  = gfo.read_file(
+0000f7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f7f0: 2070 6174 683d 696e 7075 745f 7061 7468   path=input_path
+0000f800: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000f810: 2020 6c61 7965 723d 696e 7075 745f 6c61    layer=input_la
+0000f820: 7965 722c 0a20 2020 2020 2020 2020 2020  yer,.           
+0000f830: 2020 2020 2062 626f 783d 6262 6f78 2c0a       bbox=bbox,.
+0000f840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f850: 636f 6c75 6d6e 733d 636f 6c75 6d6e 735f  columns=columns_
+0000f860: 746f 5f72 6561 642c 0a20 2020 2020 2020  to_read,.       
+0000f870: 2020 2020 2020 2020 2066 6964 5f61 735f           fid_as_
+0000f880: 696e 6465 783d 6669 645f 6173 5f69 6e64  index=fid_as_ind
+0000f890: 6578 2c0a 2020 2020 2020 2020 2020 2020  ex,.            
+0000f8a0: 290a 0a20 2020 2020 2020 2020 2020 2069  )..            i
+0000f8b0: 6620 6167 675f 636f 6c75 6d6e 7320 6973  f agg_columns is
+0000f8c0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+0000f8d0: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+0000f8e0: 5f67 6466 5b22 6669 645f 6f72 6967 225d  _gdf["fid_orig"]
+0000f8f0: 203d 2069 6e70 7574 5f67 6466 2e69 6e64   = input_gdf.ind
+0000f900: 6578 0a20 2020 2020 2020 2020 2020 2020  ex.             
+0000f910: 2020 2069 6620 6167 675f 636f 6c75 6d6e     if agg_column
+0000f920: 735f 6e65 6564 6564 2069 7320 6e6f 7420  s_needed is not 
+0000f930: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000f940: 2020 2020 2020 2020 2020 6167 675f 636f            agg_co
+0000f950: 6c75 6d6e 735f 6e65 6564 6564 2e61 7070  lumns_needed.app
+0000f960: 656e 6428 2266 6964 5f6f 7269 6722 290a  end("fid_orig").
+0000f970: 0a20 2020 2020 2020 2020 2020 2062 7265  .            bre
+0000f980: 616b 0a20 2020 2020 2020 2065 7863 6570  ak.        excep
+0000f990: 7420 4578 6365 7074 696f 6e20 6173 2065  t Exception as e
+0000f9a0: 783a 0a20 2020 2020 2020 2020 2020 2069  x:.            i
+0000f9b0: 6620 7374 7228 6578 2920 3d3d 2022 6461  f str(ex) == "da
+0000f9c0: 7461 6261 7365 2069 7320 6c6f 636b 6564  tabase is locked
+0000f9d0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0000f9e0: 2020 2069 6620 7265 7472 795f 636f 756e     if retry_coun
+0000f9f0: 7420 3c20 3130 3a0a 2020 2020 2020 2020  t < 10:.        
+0000fa00: 2020 2020 2020 2020 2020 2020 7265 7472              retr
+0000fa10: 795f 636f 756e 7420 2b3d 2031 0a20 2020  y_count += 1.   
+0000fa20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fa30: 2074 696d 652e 736c 6565 7028 3129 0a20   time.sleep(1). 
+0000fa40: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000fa50: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000fa60: 2020 2020 2020 2020 2072 6169 7365 2045           raise E
+0000fa70: 7863 6570 7469 6f6e 2822 7265 7472 6965  xception("retrie
+0000fa80: 6420 3130 2074 696d 6573 2c20 6461 7461  d 10 times, data
+0000fa90: 6261 7365 2073 7469 6c6c 206c 6f63 6b65  base still locke
+0000faa0: 6422 2920 6672 6f6d 2065 780a 2020 2020  d") from ex.    
+0000fab0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000fac0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000fad0: 6973 6520 6578 0a0a 2020 2020 2320 4368  ise ex..    # Ch
+0000fae0: 6563 6b20 7265 7375 6c74 0a20 2020 2070  eck result.    p
+0000faf0: 6572 6669 6e66 6f5b 2274 696d 655f 7265  erfinfo["time_re
+0000fb00: 6164 225d 203d 2028 6461 7465 7469 6d65  ad"] = (datetime
+0000fb10: 2e6e 6f77 2829 202d 2073 7461 7274 5f72  .now() - start_r
+0000fb20: 6561 6429 2e74 6f74 616c 5f73 6563 6f6e  ead).total_secon
+0000fb30: 6473 2829 0a20 2020 2072 6574 7572 6e5f  ds().    return_
+0000fb40: 696e 666f 5b22 6e62 5f72 6f77 735f 646f  info["nb_rows_do
+0000fb50: 6e65 225d 203d 206c 656e 2869 6e70 7574  ne"] = len(input
+0000fb60: 5f67 6466 290a 2020 2020 6966 2072 6574  _gdf).    if ret
+0000fb70: 7572 6e5f 696e 666f 5b22 6e62 5f72 6f77  urn_info["nb_row
+0000fb80: 735f 646f 6e65 225d 203d 3d20 303a 0a20  s_done"] == 0:. 
+0000fb90: 2020 2020 2020 206d 6573 7361 6765 203d         message =
+0000fba0: 2066 224e 6f20 696e 7075 7420 6765 6f6d   f"No input geom
+0000fbb0: 6574 7269 6573 2066 6f75 6e64 2069 6e20  etries found in 
+0000fbc0: 7b69 6e70 7574 5f70 6174 687d 220a 2020  {input_path}".  
+0000fbd0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+0000fbe0: 6f28 6d65 7373 6167 6529 0a20 2020 2020  o(message).     
+0000fbf0: 2020 2072 6574 7572 6e5f 696e 666f 5b22     return_info["
+0000fc00: 6d65 7373 6167 6522 5d20 3d20 6d65 7373  message"] = mess
+0000fc10: 6167 650a 2020 2020 2020 2020 7265 7475  age.        retu
+0000fc20: 726e 5f69 6e66 6f5b 2274 6f74 616c 5f74  rn_info["total_t
+0000fc30: 696d 6522 5d20 3d20 2864 6174 6574 696d  ime"] = (datetim
+0000fc40: 652e 6e6f 7728 2920 2d20 7374 6172 745f  e.now() - start_
+0000fc50: 7469 6d65 292e 746f 7461 6c5f 7365 636f  time).total_seco
+0000fc60: 6e64 7328 290a 2020 2020 2020 2020 7265  nds().        re
+0000fc70: 7475 726e 2072 6574 7572 6e5f 696e 666f  turn return_info
+0000fc80: 0a0a 2020 2020 2320 4e6f 7720 7468 6520  ..    # Now the 
+0000fc90: 7265 616c 2070 726f 6365 7373 696e 670a  real processing.
+0000fca0: 2020 2020 6966 2061 6767 5f63 6f6c 756d      if agg_colum
+0000fcb0: 6e73 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ns is not None:.
+0000fcc0: 2020 2020 2020 2020 6966 2022 5f5f 4449          if "__DI
+0000fcd0: 5353 4f4c 5645 5f54 4f4a 534f 4e22 206e  SSOLVE_TOJSON" n
+0000fce0: 6f74 2069 6e20 696e 7075 745f 6764 662e  ot in input_gdf.
+0000fcf0: 636f 6c75 6d6e 733a 0a20 2020 2020 2020  columns:.       
+0000fd00: 2020 2020 2023 2046 6972 7374 2070 6173       # First pas
+0000fd10: 7320 2d3e 2070 7574 2072 656c 6576 616e  s -> put relevan
+0000fd20: 7420 636f 6c75 6d6e 7320 696e 206a 736f  t columns in jso
+0000fd30: 6e20 6669 656c 640a 2020 2020 2020 2020  n field.        
+0000fd40: 2020 2020 6167 6766 756e 6320 3d20 7b22      aggfunc = {"
+0000fd50: 746f 5f6a 736f 6e22 3a20 6167 675f 636f  to_json": agg_co
+0000fd60: 6c75 6d6e 735f 6e65 6564 6564 7d0a 2020  lumns_needed}.  
+0000fd70: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000fd80: 2020 2020 2020 2020 2320 436f 6c75 6d6e          # Column
+0000fd90: 7320 616c 7265 6164 7920 636f 6465 6420  s already coded 
+0000fda0: 696e 2061 206a 736f 6e20 636f 6c75 6d6e  in a json column
+0000fdb0: 2c20 736f 206d 6572 6765 206a 736f 6e20  , so merge json 
+0000fdc0: 6c69 7374 730a 2020 2020 2020 2020 2020  lists.          
+0000fdd0: 2020 6167 6766 756e 6320 3d20 226d 6572    aggfunc = "mer
+0000fde0: 6765 5f6a 736f 6e5f 6c69 7374 7322 0a20  ge_json_lists". 
+0000fdf0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000fe00: 2061 6767 6675 6e63 203d 2022 6669 7273   aggfunc = "firs
+0000fe10: 7422 0a20 2020 2073 7461 7274 5f64 6973  t".    start_dis
+0000fe20: 736f 6c76 6520 3d20 6461 7465 7469 6d65  solve = datetime
+0000fe30: 2e6e 6f77 2829 0a20 2020 2064 6973 735f  .now().    diss_
+0000fe40: 6764 6620 3d20 5f64 6973 736f 6c76 6528  gdf = _dissolve(
+0000fe50: 0a20 2020 2020 2020 2064 663d 696e 7075  .        df=inpu
+0000fe60: 745f 6764 662c 2062 793d 6772 6f75 7062  t_gdf, by=groupb
+0000fe70: 795f 636f 6c75 6d6e 732c 2061 6767 6675  y_columns, aggfu
+0000fe80: 6e63 3d61 6767 6675 6e63 2c20 6173 5f69  nc=aggfunc, as_i
+0000fe90: 6e64 6578 3d46 616c 7365 2c20 6472 6f70  ndex=False, drop
+0000fea0: 6e61 3d46 616c 7365 0a20 2020 2029 0a20  na=False.    ). 
+0000feb0: 2020 2070 6572 6669 6e66 6f5b 2274 696d     perfinfo["tim
+0000fec0: 655f 6469 7373 6f6c 7665 225d 203d 2028  e_dissolve"] = (
+0000fed0: 6461 7465 7469 6d65 2e6e 6f77 2829 202d  datetime.now() -
+0000fee0: 2073 7461 7274 5f64 6973 736f 6c76 6529   start_dissolve)
+0000fef0: 2e74 6f74 616c 5f73 6563 6f6e 6473 2829  .total_seconds()
+0000ff00: 0a0a 2020 2020 2320 4966 2065 7870 6c6f  ..    # If explo
+0000ff10: 6465 636f 6c6c 6563 7469 6f6e 7320 6973  decollections is
+0000ff20: 2054 7275 6520 616e 6420 466f 7220 706f   True and For po
+0000ff30: 6c79 676f 6e73 2c20 6578 706c 6f64 6520  lygons, explode 
+0000ff40: 6d75 6c74 692d 6765 6f6d 6574 7269 6573  multi-geometries
+0000ff50: 2e0a 2020 2020 2320 4966 206e 6565 6465  ..    # If neede
+0000ff60: 6420 7468 6579 2077 696c 6c20 6265 2027  d they will be '
+0000ff70: 636f 6c6c 6563 7465 6427 2061 6674 6572  collected' after
+0000ff80: 7761 7264 7320 746f 206d 756c 7469 706f  wards to multipo
+0000ff90: 6c79 676f 6e73 2061 6761 696e 2e0a 2020  lygons again..  
+0000ffa0: 2020 6966 2065 7870 6c6f 6465 636f 6c6c    if explodecoll
+0000ffb0: 6563 7469 6f6e 7320 6973 2054 7275 6520  ections is True 
+0000ffc0: 6f72 2069 6e70 7574 5f67 656f 6d65 7472  or input_geometr
+0000ffd0: 7974 7970 6520 696e 205b 0a20 2020 2020  ytype in [.     
+0000ffe0: 2020 2047 656f 6d65 7472 7954 7970 652e     GeometryType.
+0000fff0: 504f 4c59 474f 4e2c 0a20 2020 2020 2020  POLYGON,.       
+00010000: 2047 656f 6d65 7472 7954 7970 652e 4d55   GeometryType.MU
+00010010: 4c54 4950 4f4c 5947 4f4e 2c0a 2020 2020  LTIPOLYGON,.    
+00010020: 5d3a 0a20 2020 2020 2020 2023 2061 7373  ]:.        # ass
+00010030: 6572 7420 746f 2065 7661 6465 2070 794c  ert to evade pyL
+00010040: 616e 6365 2077 6172 6e69 6e67 0a20 2020  ance warning.   
+00010050: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
+00010060: 7374 616e 6365 2864 6973 735f 6764 662c  stance(diss_gdf,
+00010070: 2067 7064 2e47 656f 4461 7461 4672 616d   gpd.GeoDataFram
+00010080: 6529 0a20 2020 2020 2020 2064 6973 735f  e).        diss_
+00010090: 6764 6620 3d20 6469 7373 5f67 6466 2e65  gdf = diss_gdf.e
+000100a0: 7870 6c6f 6465 2869 676e 6f72 655f 696e  xplode(ignore_in
+000100b0: 6465 783d 5472 7565 290a 0a20 2020 2023  dex=True)..    #
+000100c0: 2043 6c69 7020 7468 6520 7265 7375 6c74   Clip the result
+000100d0: 206f 6e20 7468 6520 626f 7264 6572 7320   on the borders 
+000100e0: 6f66 2074 6865 2062 626f 7820 6e6f 7420  of the bbox not 
+000100f0: 746f 2068 6176 6520 6f76 6572 6c61 7073  to have overlaps
+00010100: 0a20 2020 2023 2062 6574 7765 656e 2074  .    # between t
+00010110: 6865 2064 6966 6665 7265 6e74 2074 696c  he different til
+00010120: 6573 2e0a 2020 2020 2320 4966 2074 6869  es..    # If thi
+00010130: 7320 6973 206e 6f74 2061 7070 6c69 6564  s is not applied
+00010140: 2c20 7468 6973 2072 6573 756c 7473 2069  , this results i
+00010150: 6e20 736f 6d65 2067 656f 6d65 7472 6965  n some geometrie
+00010160: 7320 6e6f 7420 6265 696e 6720 6d65 7267  s not being merg
+00010170: 6564 0a20 2020 2023 206f 7220 696e 2064  ed.    # or in d
+00010180: 7570 6c69 6361 7465 732e 0a20 2020 2023  uplicates..    #
+00010190: 2052 454d 4152 4b3a 2066 6f72 2028 6d75   REMARK: for (mu
+000101a0: 6c74 6929 6c69 6e65 7374 7269 6e67 732c  lti)linestrings,
+000101b0: 2074 6865 2065 6e64 706f 696e 7473 2063   the endpoints c
+000101c0: 7265 6174 6564 2062 7920 7468 6520 636c  reated by the cl
+000101d0: 6970 2061 7265 206e 6f74 0a20 2020 2023  ip are not.    #
+000101e0: 2061 6c77 6179 7320 7468 6520 7361 6d65   always the same
+000101f0: 2064 7565 2074 6f20 726f 756e 6469 6e67   due to rounding
+00010200: 2c20 736f 2064 6973 736f 6c76 696e 6720  , so dissolving 
+00010210: 696e 2061 206e 6578 7420 7061 7373 2064  in a next pass d
+00010220: 6f65 736e 2774 0a20 2020 2023 2061 6c77  oesn't.    # alw
+00010230: 6179 7320 7265 7375 6c74 2069 6e20 6c69  ays result in li
+00010240: 6e65 7374 7269 6e67 7320 6265 696e 6720  nestrings being 
+00010250: 7265 2d63 6f6e 6e65 6374 6564 2e2e 2e20  re-connected... 
+00010260: 4265 6361 7573 6520 6469 7373 6f6c 7669  Because dissolvi
+00010270: 6e67 0a20 2020 2023 206c 696e 6573 2069  ng.    # lines i
+00010280: 736e 2774 2073 6f20 636f 6d70 7574 6174  sn't so computat
+00010290: 696f 6e61 6c6c 7920 6865 6176 7920 616e  ionally heavy an
+000102a0: 7977 6179 2c20 6472 6f70 2073 7570 706f  yway, drop suppo
+000102b0: 7274 2068 6572 652e 0a20 2020 2069 6620  rt here..    if 
+000102c0: 6262 6f78 2069 7320 6e6f 7420 4e6f 6e65  bbox is not None
+000102d0: 3a0a 2020 2020 2020 2020 7374 6172 745f  :.        start_
+000102e0: 636c 6970 203d 2064 6174 6574 696d 652e  clip = datetime.
+000102f0: 6e6f 7728 290a 2020 2020 2020 2020 6262  now().        bb
+00010300: 6f78 5f70 6f6c 7967 6f6e 203d 2073 685f  ox_polygon = sh_
+00010310: 6765 6f6d 2e50 6f6c 7967 6f6e 280a 2020  geom.Polygon(.  
+00010320: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
+00010330: 2020 2020 2020 2020 2020 2020 2862 626f              (bbo
+00010340: 785b 305d 2c20 6262 6f78 5b31 5d29 2c0a  x[0], bbox[1]),.
+00010350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010360: 2862 626f 785b 305d 2c20 6262 6f78 5b33  (bbox[0], bbox[3
+00010370: 5d29 2c0a 2020 2020 2020 2020 2020 2020  ]),.            
+00010380: 2020 2020 2862 626f 785b 325d 2c20 6262      (bbox[2], bb
+00010390: 6f78 5b33 5d29 2c0a 2020 2020 2020 2020  ox[3]),.        
+000103a0: 2020 2020 2020 2020 2862 626f 785b 325d          (bbox[2]
+000103b0: 2c20 6262 6f78 5b31 5d29 2c0a 2020 2020  , bbox[1]),.    
+000103c0: 2020 2020 2020 2020 2020 2020 2862 626f              (bbo
+000103d0: 785b 305d 2c20 6262 6f78 5b31 5d29 2c0a  x[0], bbox[1]),.
+000103e0: 2020 2020 2020 2020 2020 2020 5d0a 2020              ].  
+000103f0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00010400: 6262 6f78 5f67 6466 203d 2067 7064 2e47  bbox_gdf = gpd.G
+00010410: 656f 4461 7461 4672 616d 6528 0a20 2020  eoDataFrame(.   
+00010420: 2020 2020 2020 2020 2064 6174 613d 5b31           data=[1
+00010430: 5d2c 2067 656f 6d65 7472 793d 5b62 626f  ], geometry=[bbo
+00010440: 785f 706f 6c79 676f 6e5d 2c20 6372 733d  x_polygon], crs=
+00010450: 696e 7075 745f 6764 662e 6372 730a 2020  input_gdf.crs.  
+00010460: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00010470: 2023 2043 6174 6368 2069 7272 656c 6576   # Catch irrelev
+00010480: 616e 7420 7061 6e64 6173 2066 7574 7572  ant pandas futur
+00010490: 6520 7761 726e 696e 670a 2020 2020 2020  e warning.      
+000104a0: 2020 2320 544f 444f 3a20 7768 656e 2072    # TODO: when r
+000104b0: 656d 6f76 6564 2069 6e20 6c61 7465 7220  emoved in later 
+000104c0: 7665 7273 696f 6e20 6f66 2070 616e 6461  version of panda
+000104d0: 732c 2063 616e 2062 6520 7265 6d6f 7665  s, can be remove
+000104e0: 6420 6865 7265 0a20 2020 2020 2020 2077  d here.        w
+000104f0: 6974 6820 7761 726e 696e 6773 2e63 6174  ith warnings.cat
+00010500: 6368 5f77 6172 6e69 6e67 7328 293a 0a20  ch_warnings():. 
+00010510: 2020 2020 2020 2020 2020 206d 6573 7361             messa
+00010520: 6765 203d 2028 0a20 2020 2020 2020 2020  ge = (.         
+00010530: 2020 2020 2020 2022 496e 2061 2066 7574         "In a fut
+00010540: 7572 6520 7665 7273 696f 6e2c 2060 6466  ure version, `df
+00010550: 2e69 6c6f 635b 3a2c 2069 5d20 3d20 6e65  .iloc[:, i] = ne
+00010560: 7776 616c 7360 2077 696c 6c20 6174 7465  wvals` will atte
+00010570: 6d70 7420 746f 2022 0a20 2020 2020 2020  mpt to ".       
+00010580: 2020 2020 2020 2020 2022 7365 7420 7468           "set th
+00010590: 6520 7661 6c75 6573 2069 6e70 6c61 6365  e values inplace
+000105a0: 2069 6e73 7465 6164 206f 6620 616c 7761   instead of alwa
+000105b0: 7973 2073 6574 7469 6e67 2061 206e 6577  ys setting a new
+000105c0: 2061 7272 6179 2e22 0a20 2020 2020 2020   array.".       
+000105d0: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+000105e0: 2020 2077 6172 6e69 6e67 732e 6669 6c74     warnings.filt
+000105f0: 6572 7761 726e 696e 6773 280a 2020 2020  erwarnings(.    
+00010600: 2020 2020 2020 2020 2020 2020 6163 7469              acti
+00010610: 6f6e 3d22 6967 6e6f 7265 222c 2063 6174  on="ignore", cat
+00010620: 6567 6f72 793d 4675 7475 7265 5761 726e  egory=FutureWarn
+00010630: 696e 672c 206d 6573 7361 6765 3d72 652e  ing, message=re.
+00010640: 6573 6361 7065 286d 6573 7361 6765 290a  escape(message).
+00010650: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00010660: 2020 2020 2020 2020 2020 2320 6b65 6570            # keep
+00010670: 5f67 656f 6d5f 7479 7065 3d54 7275 6520  _geom_type=True 
+00010680: 6761 7665 2073 6f6d 6574 696d 6573 2065  gave sometimes e
+00010690: 7272 6f72 2c20 616e 6420 7374 696c 6c20  rror, and still 
+000106a0: 646f 6573 2069 6e20 302e 392e 300a 2020  does in 0.9.0.  
+000106b0: 2020 2020 2020 2020 2020 2320 736f 2075            # so u
+000106c0: 7365 206f 776e 2069 6d70 6c65 6d65 6e74  se own implement
+000106d0: 6174 696f 6e20 6f66 206b 6565 705f 6765  ation of keep_ge
+000106e0: 6f6d 5f74 7970 650a 2020 2020 2020 2020  om_type.        
+000106f0: 2020 2020 6469 7373 5f67 6466 203d 2067      diss_gdf = g
+00010700: 7064 2e63 6c69 7028 6469 7373 5f67 6466  pd.clip(diss_gdf
+00010710: 2c20 6262 6f78 5f67 6466 2920 2023 202c  , bbox_gdf)  # ,
+00010720: 206b 6565 705f 6765 6f6d 5f74 7970 653d   keep_geom_type=
+00010730: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+00010740: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+00010750: 6e63 6528 6469 7373 5f67 6466 2c20 6770  nce(diss_gdf, gp
+00010760: 642e 4765 6f44 6174 6146 7261 6d65 290a  d.GeoDataFrame).
+00010770: 0a20 2020 2020 2020 2023 204f 6e6c 7920  .        # Only 
+00010780: 6b65 6570 2067 656f 6d65 7472 6965 7320  keep geometries 
+00010790: 6f66 2074 6865 2070 7269 6d69 7469 7665  of the primitive
+000107a0: 2074 7970 6520 7370 6563 6966 6965 6420   type specified 
+000107b0: 6166 7465 7220 636c 6970 2e2e 2e0a 2020  after clip....  
+000107c0: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
+000107d0: 6e73 7461 6e63 6528 6469 7373 5f67 6466  nstance(diss_gdf
+000107e0: 2c20 6770 642e 4765 6f44 6174 6146 7261  , gpd.GeoDataFra
+000107f0: 6d65 290a 2020 2020 2020 2020 6469 7373  me).        diss
+00010800: 5f67 6466 2e67 656f 6d65 7472 7920 3d20  _gdf.geometry = 
+00010810: 6765 6f73 6572 6965 735f 7574 696c 2e67  geoseries_util.g
+00010820: 656f 6d65 7472 795f 636f 6c6c 6563 7469  eometry_collecti
+00010830: 6f6e 5f65 7874 7261 6374 280a 2020 2020  on_extract(.    
+00010840: 2020 2020 2020 2020 6469 7373 5f67 6466          diss_gdf
+00010850: 2e67 656f 6d65 7472 792c 2069 6e70 7574  .geometry, input
+00010860: 5f67 656f 6d65 7472 7974 7970 652e 746f  _geometrytype.to
+00010870: 5f70 7269 6d69 7469 7665 7479 7065 0a20  _primitivetype. 
+00010880: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00010890: 2020 7065 7266 696e 666f 5b22 7469 6d65    perfinfo["time
+000108a0: 5f63 6c69 7022 5d20 3d20 2864 6174 6574  _clip"] = (datet
+000108b0: 696d 652e 6e6f 7728 2920 2d20 7374 6172  ime.now() - star
+000108c0: 745f 636c 6970 292e 746f 7461 6c5f 7365  t_clip).total_se
+000108d0: 636f 6e64 7328 290a 0a20 2020 2023 2053  conds()..    # S
+000108e0: 6574 2065 6d70 7479 2067 656f 6d65 7472  et empty geometr
+000108f0: 6965 7320 746f 206e 756c 6c2f 4e6f 6e65  ies to null/None
+00010900: 0a20 2020 2061 7373 6572 7420 6469 7373  .    assert diss
+00010910: 5f67 6466 2e67 656f 6d65 7472 7920 6973  _gdf.geometry is
+00010920: 206e 6f74 204e 6f6e 650a 2020 2020 6469   not None.    di
+00010930: 7373 5f67 6466 2e6c 6f63 5b64 6973 735f  ss_gdf.loc[diss_
+00010940: 6764 662e 6765 6f6d 6574 7279 2e69 735f  gdf.geometry.is_
+00010950: 656d 7074 792c 205b 2267 656f 6d65 7472  empty, ["geometr
+00010960: 7922 5d5d 203d 204e 6f6e 650a 0a20 2020  y"]] = None..   
+00010970: 2023 2052 656d 6f76 6520 726f 7773 2077   # Remove rows w
+00010980: 6865 7265 2067 656f 6d20 6973 204e 6f6e  here geom is Non
+00010990: 652f 6e75 6c6c 2f65 6d70 7479 0a20 2020  e/null/empty.   
+000109a0: 2069 6620 6e6f 7420 6b65 6570 5f65 6d70   if not keep_emp
+000109b0: 7479 5f67 656f 6d73 3a0a 2020 2020 2020  ty_geoms:.      
+000109c0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+000109d0: 6e63 6528 6469 7373 5f67 6466 2c20 6770  nce(diss_gdf, gp
+000109e0: 642e 4765 6f44 6174 6146 7261 6d65 290a  d.GeoDataFrame).
+000109f0: 2020 2020 2020 2020 6469 7373 5f67 6466          diss_gdf
+00010a00: 203d 2064 6973 735f 6764 665b 7e64 6973   = diss_gdf[~dis
+00010a10: 735f 6764 662e 6765 6f6d 6574 7279 2e69  s_gdf.geometry.i
+00010a20: 736e 6128 295d 0a0a 2020 2020 2320 4966  sna()]..    # If
+00010a30: 2074 6865 7265 2069 7320 6e6f 2072 6573   there is no res
+00010a40: 756c 742c 2072 6574 7572 6e0a 2020 2020  ult, return.    
+00010a50: 6966 206c 656e 2864 6973 735f 6764 6629  if len(diss_gdf)
+00010a60: 203d 3d20 303a 0a20 2020 2020 2020 206d   == 0:.        m
+00010a70: 6573 7361 6765 203d 2066 2252 6573 756c  essage = f"Resul
+00010a80: 7420 6973 2065 6d70 7479 2066 6f72 207b  t is empty for {
+00010a90: 696e 7075 745f 7061 7468 7d22 0a20 2020  input_path}".   
+00010aa0: 2020 2020 2072 6574 7572 6e5f 696e 666f       return_info
+00010ab0: 5b22 6d65 7373 6167 6522 5d20 3d20 6d65  ["message"] = me
+00010ac0: 7373 6167 650a 2020 2020 2020 2020 7265  ssage.        re
+00010ad0: 7475 726e 5f69 6e66 6f5b 2270 6572 6669  turn_info["perfi
+00010ae0: 6e66 6f22 5d20 3d20 7065 7266 696e 666f  nfo"] = perfinfo
+00010af0: 0a20 2020 2020 2020 2072 6574 7572 6e5f  .        return_
+00010b00: 696e 666f 5b22 746f 7461 6c5f 7469 6d65  info["total_time
+00010b10: 225d 203d 2028 6461 7465 7469 6d65 2e6e  "] = (datetime.n
+00010b20: 6f77 2829 202d 2073 7461 7274 5f74 696d  ow() - start_tim
+00010b30: 6529 2e74 6f74 616c 5f73 6563 6f6e 6473  e).total_seconds
+00010b40: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+00010b50: 6e20 7265 7475 726e 5f69 6e66 6f0a 0a20  n return_info.. 
+00010b60: 2020 2023 2041 6464 2063 6f6c 756d 6e20     # Add column 
+00010b70: 7769 7468 2074 696c 655f 6964 0a20 2020  with tile_id.   
+00010b80: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
+00010b90: 6365 2864 6973 735f 6764 662c 2067 7064  ce(diss_gdf, gpd
+00010ba0: 2e47 656f 4461 7461 4672 616d 6529 0a20  .GeoDataFrame). 
+00010bb0: 2020 2069 6620 7469 6c65 5f69 6420 6973     if tile_id is
+00010bc0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00010bd0: 2020 2064 6973 735f 6764 665b 2274 696c     diss_gdf["til
+00010be0: 655f 6964 225d 203d 2074 696c 655f 6964  e_id"] = tile_id
+00010bf0: 0a0a 2020 2020 6966 2067 7269 6473 697a  ..    if gridsiz
+00010c00: 6520 213d 2030 2e30 3a0a 2020 2020 2020  e != 0.0:.      
+00010c10: 2020 6469 7373 5f67 6466 2e67 656f 6d65    diss_gdf.geome
+00010c20: 7472 7920 3d20 7368 6170 656c 7932 5f6f  try = shapely2_o
+00010c30: 725f 7079 6765 6f73 2e73 6574 5f70 7265  r_pygeos.set_pre
+00010c40: 6369 7369 6f6e 280a 2020 2020 2020 2020  cision(.        
+00010c50: 2020 2020 6469 7373 5f67 6466 2e67 656f      diss_gdf.geo
+00010c60: 6d65 7472 792c 2067 7269 645f 7369 7a65  metry, grid_size
+00010c70: 3d67 7269 6473 697a 650a 2020 2020 2020  =gridsize.      
+00010c80: 2020 290a 0a20 2020 2023 2053 6176 6520    )..    # Save 
+00010c90: 7468 6520 7265 7375 6c74 2074 6f20 6465  the result to de
+00010ca0: 7374 696e 6174 696f 6e20 6669 6c65 2873  stination file(s
+00010cb0: 290a 2020 2020 7374 6172 745f 746f 5f66  ).    start_to_f
+00010cc0: 696c 6520 3d20 6461 7465 7469 6d65 2e6e  ile = datetime.n
+00010cd0: 6f77 2829 0a0a 2020 2020 2320 4966 2074  ow()..    # If t
+00010ce0: 6865 2074 696c 6573 2064 6f6e 2774 206e  he tiles don't n
+00010cf0: 6565 6420 746f 2062 6520 6d65 7267 6564  eed to be merged
+00010d00: 2061 6674 6572 7761 7264 732c 2077 6520   afterwards, we 
+00010d10: 6361 6e20 6a75 7374 2073 6176 6520 7468  can just save th
+00010d20: 6520 7265 7375 6c74 2061 730a 2020 2020  e result as.    
+00010d30: 2320 6974 2069 732e 0a20 2020 2069 6620  # it is..    if 
+00010d40: 7374 7228 6f75 7470 7574 5f6e 6f74 6f6e  str(output_noton
+00010d50: 626f 7264 6572 5f70 6174 6829 203d 3d20  border_path) == 
+00010d60: 7374 7228 6f75 7470 7574 5f6f 6e62 6f72  str(output_onbor
+00010d70: 6465 725f 7061 7468 293a 0a20 2020 2020  der_path):.     
+00010d80: 2020 2023 2061 7373 6572 7420 746f 2065     # assert to e
+00010d90: 7661 6465 2070 794c 616e 6365 2077 6172  vade pyLance war
+00010da0: 6e69 6e67 0a20 2020 2020 2020 2061 7373  ning.        ass
+00010db0: 6572 7420 6973 696e 7374 616e 6365 2864  ert isinstance(d
+00010dc0: 6973 735f 6764 662c 2067 7064 2e47 656f  iss_gdf, gpd.Geo
+00010dd0: 4461 7461 4672 616d 6529 0a20 2020 2020  DataFrame).     
+00010de0: 2020 2023 2055 7365 2066 6f72 6365 5f6d     # Use force_m
+00010df0: 756c 7469 7479 7065 2c20 746f 2065 7661  ultitype, to eva
+00010e00: 6465 2077 6172 6e69 6e67 7320 7768 656e  de warnings when
+00010e10: 2073 6f6d 6520 6261 7463 6865 7320 636f   some batches co
+00010e20: 6e74 6169 6e0a 2020 2020 2020 2020 2320  ntain.        # 
+00010e30: 7369 6e67 6c65 7479 7065 2061 6e64 2073  singletype and s
+00010e40: 6f6d 6520 636f 6e74 6169 6e20 6d75 6c74  ome contain mult
+00010e50: 6974 7970 6520 6765 6f6d 6574 7269 6573  itype geometries
+00010e60: 0a20 2020 2020 2020 2067 666f 2e74 6f5f  .        gfo.to_
+00010e70: 6669 6c65 280a 2020 2020 2020 2020 2020  file(.          
+00010e80: 2020 6469 7373 5f67 6466 2c0a 2020 2020    diss_gdf,.    
+00010e90: 2020 2020 2020 2020 6f75 7470 7574 5f6e          output_n
+00010ea0: 6f74 6f6e 626f 7264 6572 5f70 6174 682c  otonborder_path,
+00010eb0: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
+00010ec0: 6572 3d6f 7574 7075 745f 6c61 7965 722c  er=output_layer,
+00010ed0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00010ee0: 6365 5f6d 756c 7469 7479 7065 3d54 7275  ce_multitype=Tru
+00010ef0: 652c 0a20 2020 2020 2020 2020 2020 2069  e,.            i
+00010f00: 6e64 6578 3d46 616c 7365 2c0a 2020 2020  ndex=False,.    
+00010f10: 2020 2020 2020 2020 6372 6561 7465 5f73          create_s
+00010f20: 7061 7469 616c 5f69 6e64 6578 3d46 616c  patial_index=Fal
+00010f30: 7365 2c0a 2020 2020 2020 2020 290a 2020  se,.        ).  
+00010f40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00010f50: 2320 4966 206e 6f74 2c20 7361 7665 2074  # If not, save t
+00010f60: 6865 2070 6f6c 7967 6f6e 7320 6f6e 2074  he polygons on t
+00010f70: 6865 2062 6f72 6465 7220 7365 7065 7261  he border sepera
+00010f80: 7465 6c79 0a20 2020 2020 2020 2062 626f  tely.        bbo
+00010f90: 785f 6c69 6e65 735f 6764 6620 3d20 6770  x_lines_gdf = gp
+00010fa0: 642e 4765 6f44 6174 6146 7261 6d65 280a  d.GeoDataFrame(.
+00010fb0: 2020 2020 2020 2020 2020 2020 6765 6f6d              geom
+00010fc0: 6574 7279 3d67 656f 7365 7269 6573 5f75  etry=geoseries_u
+00010fd0: 7469 6c2e 706f 6c79 676f 6e73 5f74 6f5f  til.polygons_to_
+00010fe0: 6c69 6e65 7328 0a20 2020 2020 2020 2020  lines(.         
+00010ff0: 2020 2020 2020 2067 7064 2e47 656f 5365         gpd.GeoSe
+00011000: 7269 6573 285b 7368 5f67 656f 6d2e 626f  ries([sh_geom.bo
+00011010: 7828 6262 6f78 5b30 5d2c 2062 626f 785b  x(bbox[0], bbox[
+00011020: 315d 2c20 6262 6f78 5b32 5d2c 2062 626f  1], bbox[2], bbo
+00011030: 785b 335d 295d 290a 2020 2020 2020 2020  x[3])]).        
+00011040: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
+00011050: 2020 2063 7273 3d69 6e70 7574 5f67 6466     crs=input_gdf
+00011060: 2e63 7273 2c0a 2020 2020 2020 2020 290a  .crs,.        ).
+00011070: 2020 2020 2020 2020 6f6e 626f 7264 6572          onborder
+00011080: 5f67 6466 203d 2067 7064 2e73 6a6f 696e  _gdf = gpd.sjoin
+00011090: 2864 6973 735f 6764 662c 2062 626f 785f  (diss_gdf, bbox_
+000110a0: 6c69 6e65 735f 6764 662c 2070 7265 6469  lines_gdf, predi
+000110b0: 6361 7465 3d22 696e 7465 7273 6563 7473  cate="intersects
+000110c0: 2229 0a20 2020 2020 2020 206f 6e62 6f72  ").        onbor
+000110d0: 6465 725f 6764 662e 6472 6f70 2822 696e  der_gdf.drop("in
+000110e0: 6465 785f 7269 6768 7422 2c20 6178 6973  dex_right", axis
+000110f0: 3d31 2c20 696e 706c 6163 653d 5472 7565  =1, inplace=True
+00011100: 290a 2020 2020 2020 2020 6966 206c 656e  ).        if len
+00011110: 286f 6e62 6f72 6465 725f 6764 6629 203e  (onborder_gdf) >
+00011120: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00011130: 2320 6173 7365 7274 2074 6f20 6576 6164  # assert to evad
+00011140: 6520 7079 4c61 6e63 6520 7761 726e 696e  e pyLance warnin
+00011150: 670a 2020 2020 2020 2020 2020 2020 6173  g.            as
+00011160: 7365 7274 2069 7369 6e73 7461 6e63 6528  sert isinstance(
+00011170: 6f6e 626f 7264 6572 5f67 6466 2c20 6770  onborder_gdf, gp
+00011180: 642e 4765 6f44 6174 6146 7261 6d65 290a  d.GeoDataFrame).
+00011190: 2020 2020 2020 2020 2020 2020 2320 5573              # Us
+000111a0: 6520 666f 7263 655f 6d75 6c74 6974 7970  e force_multityp
+000111b0: 652c 2074 6f20 6576 6164 6520 7761 726e  e, to evade warn
+000111c0: 696e 6773 2077 6865 6e20 736f 6d65 2062  ings when some b
+000111d0: 6174 6368 6573 2063 6f6e 7461 696e 0a20  atches contain. 
+000111e0: 2020 2020 2020 2020 2020 2023 2073 696e             # sin
+000111f0: 676c 6574 7970 6520 616e 6420 736f 6d65  gletype and some
+00011200: 2063 6f6e 7461 696e 206d 756c 7469 7479   contain multity
+00011210: 7065 2067 656f 6d65 7472 6965 730a 2020  pe geometries.  
+00011220: 2020 2020 2020 2020 2020 6766 6f2e 746f            gfo.to
+00011230: 5f66 696c 6528 0a20 2020 2020 2020 2020  _file(.         
+00011240: 2020 2020 2020 206f 6e62 6f72 6465 725f         onborder_
+00011250: 6764 662c 0a20 2020 2020 2020 2020 2020  gdf,.           
+00011260: 2020 2020 206f 7574 7075 745f 6f6e 626f       output_onbo
+00011270: 7264 6572 5f70 6174 682c 0a20 2020 2020  rder_path,.     
+00011280: 2020 2020 2020 2020 2020 206c 6179 6572             layer
+00011290: 3d6f 7574 7075 745f 6c61 7965 722c 0a20  =output_layer,. 
+000112a0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+000112b0: 6f72 6365 5f6d 756c 7469 7479 7065 3d54  orce_multitype=T
+000112c0: 7275 652c 0a20 2020 2020 2020 2020 2020  rue,.           
+000112d0: 2020 2020 2063 7265 6174 655f 7370 6174       create_spat
+000112e0: 6961 6c5f 696e 6465 783d 4661 6c73 652c  ial_index=False,
+000112f0: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
+00011300: 2020 2020 2020 2020 6e6f 746f 6e62 6f72          notonbor
+00011310: 6465 725f 6764 6620 3d20 6469 7373 5f67  der_gdf = diss_g
+00011320: 6466 5b7e 6469 7373 5f67 6466 2e69 6e64  df[~diss_gdf.ind
+00011330: 6578 2e69 7369 6e28 6f6e 626f 7264 6572  ex.isin(onborder
+00011340: 5f67 6466 2e69 6e64 6578 295d 0a20 2020  _gdf.index)].   
+00011350: 2020 2020 2069 6620 6c65 6e28 6e6f 746f       if len(noto
+00011360: 6e62 6f72 6465 725f 6764 6629 203e 2030  nborder_gdf) > 0
+00011370: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00011380: 6173 7365 7274 2074 6f20 6576 6164 6520  assert to evade 
+00011390: 7079 4c61 6e63 6520 7761 726e 696e 670a  pyLance warning.
+000113a0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+000113b0: 7274 2069 7369 6e73 7461 6e63 6528 6e6f  rt isinstance(no
+000113c0: 746f 6e62 6f72 6465 725f 6764 662c 2067  tonborder_gdf, g
+000113d0: 7064 2e47 656f 4461 7461 4672 616d 6529  pd.GeoDataFrame)
+000113e0: 0a20 2020 2020 2020 2020 2020 2023 2055  .            # U
+000113f0: 7365 2066 6f72 6365 5f6d 756c 7469 7479  se force_multity
+00011400: 7065 2c20 746f 2065 7661 6465 2077 6172  pe, to evade war
+00011410: 6e69 6e67 7320 7768 656e 2073 6f6d 6520  nings when some 
+00011420: 6261 7463 6865 7320 636f 6e74 6169 6e0a  batches contain.
+00011430: 2020 2020 2020 2020 2020 2020 2320 7369              # si
+00011440: 6e67 6c65 7479 7065 2061 6e64 2073 6f6d  ngletype and som
+00011450: 6520 636f 6e74 6169 6e20 6d75 6c74 6974  e contain multit
+00011460: 7970 6520 6765 6f6d 6574 7269 6573 0a20  ype geometries. 
+00011470: 2020 2020 2020 2020 2020 2067 666f 2e74             gfo.t
+00011480: 6f5f 6669 6c65 280a 2020 2020 2020 2020  o_file(.        
+00011490: 2020 2020 2020 2020 6e6f 746f 6e62 6f72          notonbor
+000114a0: 6465 725f 6764 662c 0a20 2020 2020 2020  der_gdf,.       
+000114b0: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+000114c0: 6e6f 746f 6e62 6f72 6465 725f 7061 7468  notonborder_path
+000114d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000114e0: 2020 6c61 7965 723d 6f75 7470 7574 5f6c    layer=output_l
+000114f0: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
+00011500: 2020 2020 2020 666f 7263 655f 6d75 6c74        force_mult
+00011510: 6974 7970 653d 5472 7565 2c0a 2020 2020  itype=True,.    
+00011520: 2020 2020 2020 2020 2020 2020 696e 6465              inde
+00011530: 783d 4661 6c73 652c 0a20 2020 2020 2020  x=False,.       
+00011540: 2020 2020 2020 2020 2063 7265 6174 655f           create_
+00011550: 7370 6174 6961 6c5f 696e 6465 783d 4661  spatial_index=Fa
 00011560: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
-00011570: 2020 2020 2063 7265 6174 655f 7370 6174       create_spat
-00011580: 6961 6c5f 696e 6465 783d 4661 6c73 652c  ial_index=False,
-00011590: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-000115a0: 2020 2070 6572 6669 6e66 6f5b 2274 696d     perfinfo["tim
-000115b0: 655f 746f 5f66 696c 6522 5d20 3d20 2864  e_to_file"] = (d
-000115c0: 6174 6574 696d 652e 6e6f 7728 2920 2d20  atetime.now() - 
-000115d0: 7374 6172 745f 746f 5f66 696c 6529 2e74  start_to_file).t
-000115e0: 6f74 616c 5f73 6563 6f6e 6473 2829 0a0a  otal_seconds()..
-000115f0: 2020 2020 2320 4669 6e61 6c69 7365 2e2e      # Finalise..
-00011600: 2e0a 2020 2020 6d65 7373 6167 6520 3d20  ..    message = 
-00011610: 6622 6469 7373 6f6c 7665 2072 6561 6479  f"dissolve ready
-00011620: 2069 6e20 7b64 6174 6574 696d 652e 6e6f   in {datetime.no
-00011630: 7728 292d 7374 6172 745f 7469 6d65 7d20  w()-start_time} 
-00011640: 6f6e 207b 696e 7075 745f 7061 7468 7d21  on {input_path}!
-00011650: 220a 2020 2020 6c6f 6767 6572 2e64 6562  ".    logger.deb
-00011660: 7567 286d 6573 7361 6765 290a 0a20 2020  ug(message)..   
-00011670: 2023 2043 6f6c 6c65 6374 2070 6572 6669   # Collect perfi
-00011680: 6e66 6f0a 2020 2020 746f 7461 6c5f 7065  nfo.    total_pe
-00011690: 7266 5f74 696d 6520 3d20 300a 2020 2020  rf_time = 0.    
-000116a0: 7065 7266 7374 7269 6e67 203d 2022 220a  perfstring = "".
-000116b0: 2020 2020 666f 7220 7065 7266 636f 6465      for perfcode
-000116c0: 2069 6e20 7065 7266 696e 666f 3a0a 2020   in perfinfo:.  
-000116d0: 2020 2020 2020 746f 7461 6c5f 7065 7266        total_perf
-000116e0: 5f74 696d 6520 2b3d 2070 6572 6669 6e66  _time += perfinf
-000116f0: 6f5b 7065 7266 636f 6465 5d0a 2020 2020  o[perfcode].    
-00011700: 2020 2020 7065 7266 7374 7269 6e67 202b      perfstring +
-00011710: 3d20 6622 7b70 6572 6663 6f64 657d 3a20  = f"{perfcode}: 
-00011720: 7b70 6572 6669 6e66 6f5b 7065 7266 636f  {perfinfo[perfco
-00011730: 6465 5d3a 2e32 667d 2c20 220a 2020 2020  de]:.2f}, ".    
-00011740: 7265 7475 726e 5f69 6e66 6f5b 2274 6f74  return_info["tot
-00011750: 616c 5f74 696d 6522 5d20 3d20 2864 6174  al_time"] = (dat
-00011760: 6574 696d 652e 6e6f 7728 2920 2d20 7374  etime.now() - st
-00011770: 6172 745f 7469 6d65 292e 746f 7461 6c5f  art_time).total_
-00011780: 7365 636f 6e64 7328 290a 2020 2020 7065  seconds().    pe
-00011790: 7266 696e 666f 5b22 756e 6163 636f 756e  rfinfo["unaccoun
-000117a0: 7465 6422 5d20 3d20 7265 7475 726e 5f69  ted"] = return_i
-000117b0: 6e66 6f5b 2274 6f74 616c 5f74 696d 6522  nfo["total_time"
-000117c0: 5d20 2d20 746f 7461 6c5f 7065 7266 5f74  ] - total_perf_t
-000117d0: 696d 650a 2020 2020 7065 7266 7374 7269  ime.    perfstri
-000117e0: 6e67 202b 3d20 6622 756e 6163 636f 756e  ng += f"unaccoun
-000117f0: 7465 643a 207b 7065 7266 696e 666f 5b27  ted: {perfinfo['
-00011800: 756e 6163 636f 756e 7465 6427 5d3a 2e32  unaccounted']:.2
-00011810: 667d 220a 0a20 2020 2023 2052 6574 7572  f}"..    # Retur
-00011820: 6e0a 2020 2020 7265 7475 726e 5f69 6e66  n.    return_inf
-00011830: 6f5b 2270 6572 6669 6e66 6f22 5d20 3d20  o["perfinfo"] = 
-00011840: 7065 7266 696e 666f 0a20 2020 2072 6574  perfinfo.    ret
-00011850: 7572 6e5f 696e 666f 5b22 7065 7266 7374  urn_info["perfst
-00011860: 7269 6e67 225d 203d 2070 6572 6673 7472  ring"] = perfstr
-00011870: 696e 670a 2020 2020 7265 7475 726e 5f69  ing.    return_i
-00011880: 6e66 6f5b 226d 6573 7361 6765 225d 203d  nfo["message"] =
-00011890: 206d 6573 7361 6765 0a20 2020 2072 6574   message.    ret
-000118a0: 7572 6e20 7265 7475 726e 5f69 6e66 6f0a  urn return_info.
-000118b0: 0a0a 6465 6620 5f64 6973 736f 6c76 6528  ..def _dissolve(
-000118c0: 0a20 2020 2064 663a 2067 7064 2e47 656f  .    df: gpd.Geo
-000118d0: 4461 7461 4672 616d 652c 0a20 2020 2062  DataFrame,.    b
-000118e0: 793d 4e6f 6e65 2c0a 2020 2020 6167 6766  y=None,.    aggf
-000118f0: 756e 633a 204f 7074 696f 6e61 6c5b 556e  unc: Optional[Un
-00011900: 696f 6e5b 7374 722c 2064 6963 745d 5d20  ion[str, dict]] 
-00011910: 3d20 2266 6972 7374 222c 0a20 2020 2061  = "first",.    a
-00011920: 735f 696e 6465 783d 5472 7565 2c0a 2020  s_index=True,.  
-00011930: 2020 6c65 7665 6c3d 4e6f 6e65 2c0a 2020    level=None,.  
-00011940: 2020 736f 7274 3d54 7275 652c 0a20 2020    sort=True,.   
-00011950: 206f 6273 6572 7665 643d 4661 6c73 652c   observed=False,
-00011960: 0a20 2020 2064 726f 706e 613d 5472 7565  .    dropna=True
-00011970: 2c0a 2920 2d3e 2067 7064 2e47 656f 4461  ,.) -> gpd.GeoDa
-00011980: 7461 4672 616d 653a 0a20 2020 2022 2222  taFrame:.    """
-00011990: 0a20 2020 2044 6973 736f 6c76 6520 6765  .    Dissolve ge
-000119a0: 6f6d 6574 7269 6573 2077 6974 6869 6e20  ometries within 
-000119b0: 6067 726f 7570 6279 6020 696e 746f 2073  `groupby` into s
-000119c0: 696e 676c 6520 6f62 7365 7276 6174 696f  ingle observatio
-000119d0: 6e2e 0a20 2020 2054 6869 7320 6973 2061  n..    This is a
-000119e0: 6363 6f6d 706c 6973 6865 6420 6279 2061  ccomplished by a
-000119f0: 7070 6c79 696e 6720 7468 6520 6075 6e61  pplying the `una
-00011a00: 7279 5f75 6e69 6f6e 6020 6d65 7468 6f64  ry_union` method
-00011a10: 0a20 2020 2074 6f20 616c 6c20 6765 6f6d  .    to all geom
-00011a20: 6574 7269 6573 2077 6974 6869 6e20 6120  etries within a 
-00011a30: 6772 6f75 7073 656c 662e 0a20 2020 204f  groupself..    O
-00011a40: 6273 6572 7661 7469 6f6e 7320 6173 736f  bservations asso
-00011a50: 6369 6174 6564 2077 6974 6820 6561 6368  ciated with each
-00011a60: 2060 6772 6f75 7062 7960 2067 726f 7570   `groupby` group
-00011a70: 2077 696c 6c20 6265 2061 6767 7265 6761   will be aggrega
-00011a80: 7465 640a 2020 2020 7573 696e 6720 7468  ted.    using th
-00011a90: 6520 6061 6767 6675 6e63 602e 0a20 2020  e `aggfunc`..   
-00011aa0: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
-00011ab0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2062  ----------.    b
-00011ac0: 7920 3a20 7374 7269 6e67 2c20 6465 6661  y : string, defa
-00011ad0: 756c 7420 4e6f 6e65 0a20 2020 2020 2020  ult None.       
-00011ae0: 2043 6f6c 756d 6e20 7768 6f73 6520 7661   Column whose va
-00011af0: 6c75 6573 2064 6566 696e 6520 6772 6f75  lues define grou
-00011b00: 7073 2074 6f20 6265 2064 6973 736f 6c76  ps to be dissolv
-00011b10: 6564 2e20 4966 204e 6f6e 652c 0a20 2020  ed. If None,.   
-00011b20: 2020 2020 2077 686f 6c65 2047 656f 4461       whole GeoDa
-00011b30: 7461 4672 616d 6520 6973 2063 6f6e 7369  taFrame is consi
-00011b40: 6465 7265 6420 6120 7369 6e67 6c65 2067  dered a single g
-00011b50: 726f 7570 2e0a 2020 2020 6167 6766 756e  roup..    aggfun
-00011b60: 6320 3a20 6675 6e63 7469 6f6e 2c20 7374  c : function, st
-00011b70: 7269 6e67 206f 7220 6469 6374 2c20 6465  ring or dict, de
-00011b80: 6661 756c 7420 2266 6972 7374 220a 2020  fault "first".  
-00011b90: 2020 2020 2020 4167 6772 6567 6174 696f        Aggregatio
-00011ba0: 6e20 6675 6e63 7469 6f6e 2066 6f72 206d  n function for m
-00011bb0: 616e 6970 756c 6174 696f 6e20 6f66 2064  anipulation of d
-00011bc0: 6174 6120 6173 736f 6369 6174 6564 0a20  ata associated. 
-00011bd0: 2020 2020 2020 2077 6974 6820 6561 6368         with each
-00011be0: 2067 726f 7570 2e20 5061 7373 6564 2074   group. Passed t
-00011bf0: 6f20 7061 6e64 6173 2060 6772 6f75 7062  o pandas `groupb
-00011c00: 792e 6167 6760 206d 6574 686f 642e 0a20  y.agg` method.. 
-00011c10: 2020 2061 735f 696e 6465 7820 3a20 626f     as_index : bo
-00011c20: 6f6c 6561 6e2c 2064 6566 6175 6c74 2054  olean, default T
-00011c30: 7275 650a 2020 2020 2020 2020 4966 2074  rue.        If t
-00011c40: 7275 652c 2067 726f 7570 6279 2063 6f6c  rue, groupby col
-00011c50: 756d 6e73 2062 6563 6f6d 6520 696e 6465  umns become inde
-00011c60: 7820 6f66 2072 6573 756c 742e 0a20 2020  x of result..   
-00011c70: 206c 6576 656c 203a 2069 6e74 206f 7220   level : int or 
-00011c80: 7374 7220 6f72 2073 6571 7565 6e63 6520  str or sequence 
-00011c90: 6f66 2069 6e74 206f 7220 7365 7175 656e  of int or sequen
-00011ca0: 6365 206f 6620 7374 722c 2064 6566 6175  ce of str, defau
-00011cb0: 6c74 204e 6f6e 650a 2020 2020 2020 2020  lt None.        
-00011cc0: 4966 2074 6865 2061 7869 7320 6973 2061  If the axis is a
-00011cd0: 204d 756c 7469 496e 6465 7820 2868 6965   MultiIndex (hie
-00011ce0: 7261 7263 6869 6361 6c29 2c20 6772 6f75  rarchical), grou
-00011cf0: 7020 6279 2061 0a20 2020 2020 2020 2070  p by a.        p
-00011d00: 6172 7469 6375 6c61 7220 6c65 7665 6c20  articular level 
-00011d10: 6f72 206c 6576 656c 732e 0a20 2020 2020  or levels..     
-00011d20: 2020 202e 2e20 7665 7273 696f 6e61 6464     .. versionadd
-00011d30: 6564 3a3a 2030 2e39 2e30 0a20 2020 2073  ed:: 0.9.0.    s
-00011d40: 6f72 7420 3a20 626f 6f6c 2c20 6465 6661  ort : bool, defa
-00011d50: 756c 7420 5472 7565 0a20 2020 2020 2020  ult True.       
-00011d60: 2053 6f72 7420 6772 6f75 7020 6b65 7973   Sort group keys
-00011d70: 2e20 4765 7420 6265 7474 6572 2070 6572  . Get better per
-00011d80: 666f 726d 616e 6365 2062 7920 7475 726e  formance by turn
-00011d90: 696e 6720 7468 6973 206f 6666 2e0a 2020  ing this off..  
-00011da0: 2020 2020 2020 4e6f 7465 2074 6869 7320        Note this 
-00011db0: 646f 6573 206e 6f74 2069 6e66 6c75 656e  does not influen
-00011dc0: 6365 2074 6865 206f 7264 6572 206f 6620  ce the order of 
-00011dd0: 6f62 7365 7276 6174 696f 6e73 2077 6974  observations wit
-00011de0: 6869 6e0a 2020 2020 2020 2020 6561 6368  hin.        each
-00011df0: 2067 726f 7570 2e20 4772 6f75 7062 7920   group. Groupby 
-00011e00: 7072 6573 6572 7665 7320 7468 6520 6f72  preserves the or
-00011e10: 6465 7220 6f66 2072 6f77 7320 7769 7468  der of rows with
-00011e20: 696e 2065 6163 6820 6772 6f75 702e 0a20  in each group.. 
-00011e30: 2020 2020 2020 202e 2e20 7665 7273 696f         .. versio
-00011e40: 6e61 6464 6564 3a3a 2030 2e39 2e30 0a20  nadded:: 0.9.0. 
-00011e50: 2020 206f 6273 6572 7665 6420 3a20 626f     observed : bo
-00011e60: 6f6c 2c20 6465 6661 756c 7420 4661 6c73  ol, default Fals
-00011e70: 650a 2020 2020 2020 2020 5468 6973 206f  e.        This o
-00011e80: 6e6c 7920 6170 706c 6965 7320 6966 2061  nly applies if a
-00011e90: 6e79 206f 6620 7468 6520 6772 6f75 7065  ny of the groupe
-00011ea0: 7273 2061 7265 2043 6174 6567 6f72 6963  rs are Categoric
-00011eb0: 616c 732e 0a20 2020 2020 2020 2049 6620  als..        If 
-00011ec0: 5472 7565 3a20 6f6e 6c79 2073 686f 7720  True: only show 
-00011ed0: 6f62 7365 7276 6564 2076 616c 7565 7320  observed values 
-00011ee0: 666f 7220 6361 7465 676f 7269 6361 6c20  for categorical 
-00011ef0: 6772 6f75 7065 7273 2e0a 2020 2020 2020  groupers..      
-00011f00: 2020 4966 2046 616c 7365 3a20 7368 6f77    If False: show
-00011f10: 2061 6c6c 2076 616c 7565 7320 666f 7220   all values for 
-00011f20: 6361 7465 676f 7269 6361 6c20 6772 6f75  categorical grou
-00011f30: 7065 7273 2e0a 2020 2020 2020 2020 2e2e  pers..        ..
-00011f40: 2076 6572 7369 6f6e 6164 6465 643a 3a20   versionadded:: 
-00011f50: 302e 392e 300a 2020 2020 6472 6f70 6e61  0.9.0.    dropna
-00011f60: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-00011f70: 2054 7275 650a 2020 2020 2020 2020 4966   True.        If
-00011f80: 2054 7275 652c 2061 6e64 2069 6620 6772   True, and if gr
-00011f90: 6f75 7020 6b65 7973 2063 6f6e 7461 696e  oup keys contain
-00011fa0: 204e 4120 7661 6c75 6573 2c20 4e41 2076   NA values, NA v
-00011fb0: 616c 7565 730a 2020 2020 2020 2020 746f  alues.        to
-00011fc0: 6765 7468 6572 2077 6974 6820 726f 772f  gether with row/
-00011fd0: 636f 6c75 6d6e 2077 696c 6c20 6265 2064  column will be d
-00011fe0: 726f 7070 6564 2e20 4966 2046 616c 7365  ropped. If False
-00011ff0: 2c20 4e41 0a20 2020 2020 2020 2076 616c  , NA.        val
-00012000: 7565 7320 7769 6c6c 2061 6c73 6f20 6265  ues will also be
-00012010: 2074 7265 6174 6564 2061 7320 7468 6520   treated as the 
-00012020: 6b65 7920 696e 2067 726f 7570 732e 0a20  key in groups.. 
-00012030: 2020 2020 2020 2054 6869 7320 7061 7261         This para
-00012040: 6d65 7465 7220 6973 206e 6f74 2073 7570  meter is not sup
-00012050: 706f 7274 6564 2066 6f72 2070 616e 6461  ported for panda
-00012060: 7320 3c20 312e 312e 302e 0a20 2020 2020  s < 1.1.0..     
-00012070: 2020 2041 2077 6172 6e69 6e67 2077 696c     A warning wil
-00012080: 6c20 6265 2065 6d69 7474 6564 2066 6f72  l be emitted for
-00012090: 2065 6172 6c69 6572 2070 616e 6461 7320   earlier pandas 
-000120a0: 7665 7273 696f 6e73 0a20 2020 2020 2020  versions.       
-000120b0: 2069 6620 6120 6e6f 6e2d 6465 6661 756c   if a non-defaul
-000120c0: 7420 7661 6c75 6520 6973 2067 6976 656e  t value is given
-000120d0: 2066 6f72 2074 6869 7320 7061 7261 6d65   for this parame
-000120e0: 7465 722e 0a20 2020 2020 2020 202e 2e20  ter..        .. 
-000120f0: 7665 7273 696f 6e61 6464 6564 3a3a 2030  versionadded:: 0
-00012100: 2e39 2e30 0a20 2020 2052 6574 7572 6e73  .9.0.    Returns
-00012110: 0a20 2020 202d 2d2d 2d2d 2d2d 0a20 2020  .    -------.   
-00012120: 2047 656f 4461 7461 4672 616d 650a 2020   GeoDataFrame.  
-00012130: 2020 4578 616d 706c 6573 0a20 2020 202d    Examples.    -
-00012140: 2d2d 2d2d 2d2d 2d0a 2020 2020 3e3e 3e20  -------.    >>> 
-00012150: 6672 6f6d 2073 6861 7065 6c79 2e67 656f  from shapely.geo
-00012160: 6d65 7472 7920 696d 706f 7274 2050 6f69  metry import Poi
-00012170: 6e74 0a20 2020 203e 3e3e 2064 203d 207b  nt.    >>> d = {
-00012180: 0a20 2020 202e 2e2e 2020 2020 2022 636f  .    ...     "co
-00012190: 6c31 223a 205b 226e 616d 6531 222c 2022  l1": ["name1", "
-000121a0: 6e61 6d65 3222 2c20 226e 616d 6531 225d  name2", "name1"]
-000121b0: 2c0a 2020 2020 2e2e 2e20 2020 2020 2267  ,.    ...     "g
-000121c0: 656f 6d65 7472 7922 3a20 5b50 6f69 6e74  eometry": [Point
-000121d0: 2831 2c20 3229 2c20 506f 696e 7428 322c  (1, 2), Point(2,
-000121e0: 2031 292c 2050 6f69 6e74 2830 2c20 3129   1), Point(0, 1)
-000121f0: 5d2c 0a20 2020 202e 2e2e 207d 0a20 2020  ],.    ... }.   
-00012200: 203e 3e3e 2067 6466 203d 2067 656f 7061   >>> gdf = geopa
-00012210: 6e64 6173 2e47 656f 4461 7461 4672 616d  ndas.GeoDataFram
-00012220: 6528 642c 2063 7273 3d34 3332 3629 0a20  e(d, crs=4326). 
-00012230: 2020 203e 3e3e 2067 6466 0a20 2020 2020     >>> gdf.     
-00012240: 2020 2063 6f6c 3120 2020 2020 2020 2020     col1         
-00012250: 2020 2020 2020 2020 6765 6f6d 6574 7279          geometry
-00012260: 0a20 2020 2030 2020 6e61 6d65 3120 2050  .    0  name1  P
-00012270: 4f49 4e54 2028 312e 3030 3030 3020 322e  OINT (1.00000 2.
-00012280: 3030 3030 3029 0a20 2020 2031 2020 6e61  00000).    1  na
-00012290: 6d65 3220 2050 4f49 4e54 2028 322e 3030  me2  POINT (2.00
-000122a0: 3030 3020 312e 3030 3030 3029 0a20 2020  000 1.00000).   
-000122b0: 2032 2020 6e61 6d65 3120 2050 4f49 4e54   2  name1  POINT
-000122c0: 2028 302e 3030 3030 3020 312e 3030 3030   (0.00000 1.0000
-000122d0: 3029 0a20 2020 203e 3e3e 2064 6973 736f  0).    >>> disso
-000122e0: 6c76 6564 203d 2067 6466 2e64 6973 736f  lved = gdf.disso
-000122f0: 6c76 6528 2763 6f6c 3127 290a 2020 2020  lve('col1').    
-00012300: 3e3e 3e20 6469 7373 6f6c 7665 6420 2023  >>> dissolved  #
-00012310: 2064 6f63 7465 7374 3a20 2b53 4b49 500a   doctest: +SKIP.
-00012320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012350: 6765 6f6d 6574 7279 0a20 2020 2063 6f6c  geometry.    col
-00012360: 310a 2020 2020 6e61 6d65 3120 204d 554c  1.    name1  MUL
-00012370: 5449 504f 494e 5420 2830 2e30 3030 3030  TIPOINT (0.00000
-00012380: 2031 2e30 3030 3030 2c20 312e 3030 3030   1.00000, 1.0000
-00012390: 3020 322e 3030 3030 3029 0a20 2020 206e  0 2.00000).    n
-000123a0: 616d 6532 2020 2020 2020 2020 2020 2020  ame2            
-000123b0: 2020 2020 2020 2020 2020 2020 504f 494e              POIN
-000123c0: 5420 2832 2e30 3030 3030 2031 2e30 3030  T (2.00000 1.000
-000123d0: 3030 290a 2020 2020 5365 6520 616c 736f  00).    See also
-000123e0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
-000123f0: 2020 4765 6f44 6174 6146 7261 6d65 2e65    GeoDataFrame.e
-00012400: 7870 6c6f 6465 203a 2065 7870 6c6f 6465  xplode : explode
-00012410: 206d 756c 7469 2d70 6172 7420 6765 6f6d   multi-part geom
-00012420: 6574 7269 6573 2069 6e74 6f20 7369 6e67  etries into sing
-00012430: 6c65 2067 656f 6d65 7472 6965 730a 2020  le geometries.  
-00012440: 2020 2222 220a 0a20 2020 2069 6620 6279    """..    if by
-00012450: 2069 7320 4e6f 6e65 2061 6e64 206c 6576   is None and lev
-00012460: 656c 2069 7320 4e6f 6e65 3a0a 2020 2020  el is None:.    
-00012470: 2020 2020 6279 5f6c 6f63 616c 203d 206e      by_local = n
-00012480: 702e 7a65 726f 7328 6c65 6e28 6466 292c  p.zeros(len(df),
-00012490: 2064 7479 7065 3d22 696e 7436 3422 290a   dtype="int64").
-000124a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000124b0: 2020 6279 5f6c 6f63 616c 203d 2062 790a    by_local = by.
-000124c0: 0a20 2020 2067 726f 7570 6279 5f6b 7761  .    groupby_kwa
-000124d0: 7267 7320 3d20 7b0a 2020 2020 2020 2020  rgs = {.        
-000124e0: 2262 7922 3a20 6279 5f6c 6f63 616c 2c0a  "by": by_local,.
-000124f0: 2020 2020 2020 2020 226c 6576 656c 223a          "level":
-00012500: 206c 6576 656c 2c0a 2020 2020 2020 2020   level,.        
-00012510: 2273 6f72 7422 3a20 736f 7274 2c0a 2020  "sort": sort,.  
-00012520: 2020 2020 2020 226f 6273 6572 7665 6422        "observed"
-00012530: 3a20 6f62 7365 7276 6564 2c0a 2020 2020  : observed,.    
-00012540: 2020 2020 2264 726f 706e 6122 3a20 6472      "dropna": dr
-00012550: 6f70 6e61 2c0a 2020 2020 7d0a 2020 2020  opna,.    }.    
-00012560: 2222 220a 2020 2020 6966 206e 6f74 2063  """.    if not c
-00012570: 6f6d 7061 742e 5041 4e44 4153 5f47 455f  ompat.PANDAS_GE_
-00012580: 3131 3a0a 2020 2020 2020 2020 6772 6f75  11:.        grou
-00012590: 7062 795f 6b77 6172 6773 2e70 6f70 2822  pby_kwargs.pop("
-000125a0: 6472 6f70 6e61 2229 0a0a 2020 2020 2020  dropna")..      
-000125b0: 2020 6966 206e 6f74 2064 726f 706e 613a    if not dropna:
-000125c0: 2020 2320 4966 2074 6865 7920 7061 7373    # If they pass
-000125d0: 6564 2061 206e 6f6e 2d64 6566 6175 6c74  ed a non-default
-000125e0: 2064 726f 706e 6120 7661 6c75 650a 2020   dropna value.  
-000125f0: 2020 2020 2020 2020 2020 7761 726e 696e            warnin
-00012600: 6773 2e77 6172 6e28 2264 726f 706e 6120  gs.warn("dropna 
-00012610: 6b77 6172 6720 6973 206e 6f74 2073 7570  kwarg is not sup
-00012620: 706f 7274 6564 2066 6f72 2070 616e 6461  ported for panda
-00012630: 7320 3c20 312e 312e 3022 290a 2020 2020  s < 1.1.0").    
-00012640: 2222 220a 0a20 2020 2023 2050 726f 6365  """..    # Proce
-00012650: 7373 206e 6f6e 2d73 7061 7469 616c 2063  ss non-spatial c
-00012660: 6f6d 706f 6e65 6e74 0a20 2020 2064 6174  omponent.    dat
-00012670: 6120 3d20 7064 2e44 6174 6146 7261 6d65  a = pd.DataFrame
-00012680: 2864 662e 6472 6f70 2863 6f6c 756d 6e73  (df.drop(columns
-00012690: 3d64 662e 6765 6f6d 6574 7279 2e6e 616d  =df.geometry.nam
-000126a0: 6529 290a 0a20 2020 2069 6620 6167 6766  e))..    if aggf
-000126b0: 756e 6320 6973 206e 6f74 204e 6f6e 6520  unc is not None 
-000126c0: 616e 6420 6973 696e 7374 616e 6365 2861  and isinstance(a
-000126d0: 6767 6675 6e63 2c20 6469 6374 2920 616e  ggfunc, dict) an
-000126e0: 6420 2274 6f5f 6a73 6f6e 2220 696e 2061  d "to_json" in a
-000126f0: 6767 6675 6e63 3a0a 2020 2020 2020 2020  ggfunc:.        
-00012700: 6167 675f 636f 6c75 6d6e 7320 3d20 6c69  agg_columns = li
-00012710: 7374 2873 6574 2861 6767 6675 6e63 5b22  st(set(aggfunc["
-00012720: 746f 5f6a 736f 6e22 5d29 290a 2020 2020  to_json"])).    
-00012730: 2020 2020 6167 6772 6567 6174 6564 5f64      aggregated_d
-00012740: 6174 6120 3d20 280a 2020 2020 2020 2020  ata = (.        
-00012750: 2020 2020 6461 7461 2e67 726f 7570 6279      data.groupby
-00012760: 282a 2a67 726f 7570 6279 5f6b 7761 7267  (**groupby_kwarg
-00012770: 7329 0a20 2020 2020 2020 2020 2020 202e  s).            .
-00012780: 6170 706c 7928 6c61 6d62 6461 2067 3a20  apply(lambda g: 
-00012790: 675b 6167 675f 636f 6c75 6d6e 735d 2e74  g[agg_columns].t
-000127a0: 6f5f 6a73 6f6e 286f 7269 656e 743d 2272  o_json(orient="r
-000127b0: 6563 6f72 6473 2229 290a 2020 2020 2020  ecords")).      
-000127c0: 2020 2020 2020 2e74 6f5f 6672 616d 6528        .to_frame(
-000127d0: 6e61 6d65 3d22 5f5f 4449 5353 4f4c 5645  name="__DISSOLVE
-000127e0: 5f54 4f4a 534f 4e22 290a 2020 2020 2020  _TOJSON").      
-000127f0: 2020 290a 2020 2020 656c 6966 2069 7369    ).    elif isi
-00012800: 6e73 7461 6e63 6528 6167 6766 756e 632c  nstance(aggfunc,
-00012810: 2073 7472 2920 616e 6420 6167 6766 756e   str) and aggfun
-00012820: 6320 3d3d 2022 6d65 7267 655f 6a73 6f6e  c == "merge_json
-00012830: 5f6c 6973 7473 223a 0a20 2020 2020 2020  _lists":.       
-00012840: 2023 204d 6572 6765 2061 6e64 2066 6c61   # Merge and fla
-00012850: 7474 656e 2074 6865 206a 736f 6e20 6c69  tten the json li
-00012860: 7374 7320 696e 2074 6865 2067 726f 7570  sts in the group
-00012870: 730a 2020 2020 2020 2020 6465 6620 6772  s.        def gr
-00012880: 6f75 705f 666c 6174 7465 6e5f 6a73 6f6e  oup_flatten_json
-00012890: 5f6c 6973 7428 6729 3a0a 2020 2020 2020  _list(g):.      
-000128a0: 2020 2020 2020 2320 4576 616c 7561 7465        # Evaluate
-000128b0: 2061 6c6c 2067 726f 7570 6564 2072 6f77   all grouped row
-000128c0: 7320 746f 206a 736f 6e20 6f62 6a65 6374  s to json object
-000128d0: 732e 2054 6869 7320 7265 7375 6c74 7320  s. This results 
-000128e0: 696e 2061 206c 6973 7420 6f66 0a20 2020  in a list of.   
-000128f0: 2020 2020 2020 2020 2023 206c 6973 7473           # lists
-00012900: 206f 6620 6a73 6f6e 206f 626a 6563 7473   of json objects
-00012910: 2e0a 2020 2020 2020 2020 2020 2020 6a73  ..            js
-00012920: 6f6e 5f6e 6573 7465 645f 6c69 7374 7320  on_nested_lists 
-00012930: 3d20 5b0a 2020 2020 2020 2020 2020 2020  = [.            
-00012940: 2020 2020 6a73 6f6e 2e6c 6f61 6473 286a      json.loads(j
-00012950: 736f 6e5f 7661 6c75 6573 2920 666f 7220  son_values) for 
-00012960: 6a73 6f6e 5f76 616c 7565 7320 696e 2067  json_values in g
-00012970: 5b22 5f5f 4449 5353 4f4c 5645 5f54 4f4a  ["__DISSOLVE_TOJ
-00012980: 534f 4e22 5d0a 2020 2020 2020 2020 2020  SON"].          
-00012990: 2020 5d0a 0a20 2020 2020 2020 2020 2020    ]..           
-000129a0: 2023 2045 7874 7261 6374 2074 6865 2072   # Extract the r
-000129b0: 6f77 7320 6672 6f6d 2074 6865 206e 6573  ows from the nes
-000129c0: 7465 6420 6c69 7374 7320 2b20 7075 7420  ted lists + put 
-000129d0: 696e 2061 2066 6c61 7420 6c69 7374 2061  in a flat list a
-000129e0: 7320 7374 7269 6e67 730a 2020 2020 2020  s strings.      
-000129f0: 2020 2020 2020 6a73 6f6e 7374 725f 666c        jsonstr_fl
-00012a00: 6174 203d 205b 0a20 2020 2020 2020 2020  at = [.         
-00012a10: 2020 2020 2020 206a 736f 6e2e 6475 6d70         json.dump
-00012a20: 7328 6a73 6f6e 5f76 616c 7565 290a 2020  s(json_value).  
-00012a30: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00012a40: 7220 6a73 6f6e 5f76 616c 7565 7320 696e  r json_values in
-00012a50: 206a 736f 6e5f 6e65 7374 6564 5f6c 6973   json_nested_lis
-00012a60: 7473 0a20 2020 2020 2020 2020 2020 2020  ts.             
-00012a70: 2020 2066 6f72 206a 736f 6e5f 7661 6c75     for json_valu
-00012a80: 6520 696e 206a 736f 6e5f 7661 6c75 6573  e in json_values
-00012a90: 0a20 2020 2020 2020 2020 2020 205d 0a0a  .            ]..
-00012aa0: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
-00012ab0: 6d6f 7665 2064 7570 6c69 6361 7465 730a  move duplicates.
-00012ac0: 2020 2020 2020 2020 2020 2020 6a73 6f6e              json
-00012ad0: 7373 7472 5f64 6973 7469 6e63 7420 3d20  sstr_distinct = 
-00012ae0: 7365 7428 6a73 6f6e 7374 725f 666c 6174  set(jsonstr_flat
-00012af0: 290a 0a20 2020 2020 2020 2020 2020 2023  )..            #
-00012b00: 2043 6f6e 7665 7274 2074 6865 2064 6174   Convert the dat
-00012b10: 6120 6167 6169 6e20 746f 2061 206c 6973  a again to a lis
-00012b20: 7420 6f66 206a 736f 6e20 6f62 6a65 6374  t of json object
-00012b30: 730a 2020 2020 2020 2020 2020 2020 6a73  s.            js
-00012b40: 6f6e 5f64 6973 7469 6e63 7420 3d20 5b6a  on_distinct = [j
-00012b50: 736f 6e2e 6c6f 6164 7328 6a73 6f6e 5f76  son.loads(json_v
-00012b60: 616c 7565 2920 666f 7220 6a73 6f6e 5f76  alue) for json_v
-00012b70: 616c 7565 2069 6e20 6a73 6f6e 7373 7472  alue in jsonsstr
-00012b80: 5f64 6973 7469 6e63 745d 0a0a 2020 2020  _distinct]..    
-00012b90: 2020 2020 2020 2020 2320 5265 7475 726e          # Return
-00012ba0: 2061 7320 6a73 6f6e 2073 7472 696e 670a   as json string.
-00012bb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00012bc0: 726e 206a 736f 6e2e 6475 6d70 7328 6a73  rn json.dumps(js
-00012bd0: 6f6e 5f64 6973 7469 6e63 7429 0a0a 2020  on_distinct)..  
-00012be0: 2020 2020 2020 6167 6772 6567 6174 6564        aggregated
-00012bf0: 5f64 6174 6120 3d20 280a 2020 2020 2020  _data = (.      
-00012c00: 2020 2020 2020 6461 7461 2e67 726f 7570        data.group
-00012c10: 6279 282a 2a67 726f 7570 6279 5f6b 7761  by(**groupby_kwa
-00012c20: 7267 7329 0a20 2020 2020 2020 2020 2020  rgs).           
-00012c30: 202e 6170 706c 7928 6c61 6d62 6461 2067   .apply(lambda g
-00012c40: 3a20 6772 6f75 705f 666c 6174 7465 6e5f  : group_flatten_
-00012c50: 6a73 6f6e 5f6c 6973 7428 6729 290a 2020  json_list(g)).  
-00012c60: 2020 2020 2020 2020 2020 2e74 6f5f 6672            .to_fr
-00012c70: 616d 6528 6e61 6d65 3d22 5f5f 4449 5353  ame(name="__DISS
-00012c80: 4f4c 5645 5f54 4f4a 534f 4e22 290a 2020  OLVE_TOJSON").  
-00012c90: 2020 2020 2020 290a 2020 2020 656c 7365        ).    else
-00012ca0: 3a0a 2020 2020 2020 2020 6167 6772 6567  :.        aggreg
-00012cb0: 6174 6564 5f64 6174 6120 3d20 6461 7461  ated_data = data
-00012cc0: 2e67 726f 7570 6279 282a 2a67 726f 7570  .groupby(**group
-00012cd0: 6279 5f6b 7761 7267 7329 2e61 6767 2861  by_kwargs).agg(a
-00012ce0: 6767 6675 6e63 290a 2020 2020 2020 2020  ggfunc).        
-00012cf0: 2320 4368 6563 6b20 6966 2061 6c6c 2063  # Check if all c
-00012d00: 6f6c 756d 6e73 2077 6572 6520 7072 6f70  olumns were prop
-00012d10: 6572 6c79 2061 6767 7265 6761 7465 640a  erly aggregated.
-00012d20: 2020 2020 2020 2020 6173 7365 7274 2062          assert b
-00012d30: 795f 6c6f 6361 6c20 6973 206e 6f74 204e  y_local is not N
-00012d40: 6f6e 650a 2020 2020 2020 2020 636f 6c75  one.        colu
-00012d50: 6d6e 735f 746f 5f61 6767 203d 205b 636f  mns_to_agg = [co
-00012d60: 6c75 6d6e 2066 6f72 2063 6f6c 756d 6e20  lumn for column 
-00012d70: 696e 2064 6174 612e 636f 6c75 6d6e 7320  in data.columns 
-00012d80: 6966 2063 6f6c 756d 6e20 6e6f 7420 696e  if column not in
-00012d90: 2062 795f 6c6f 6361 6c5d 0a20 2020 2020   by_local].     
-00012da0: 2020 2069 6620 6c65 6e28 636f 6c75 6d6e     if len(column
-00012db0: 735f 746f 5f61 6767 2920 213d 206c 656e  s_to_agg) != len
-00012dc0: 2861 6767 7265 6761 7465 645f 6461 7461  (aggregated_data
-00012dd0: 2e63 6f6c 756d 6e73 293a 0a20 2020 2020  .columns):.     
-00012de0: 2020 2020 2020 2064 726f 7070 6564 5f63         dropped_c
-00012df0: 6f6c 756d 6e73 203d 205b 0a20 2020 2020  olumns = [.     
-00012e00: 2020 2020 2020 2020 2020 2063 6f6c 756d             colum
-00012e10: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00012e20: 2020 666f 7220 636f 6c75 6d6e 2069 6e20    for column in 
-00012e30: 636f 6c75 6d6e 735f 746f 5f61 6767 0a20  columns_to_agg. 
-00012e40: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00012e50: 6620 636f 6c75 6d6e 206e 6f74 2069 6e20  f column not in 
-00012e60: 6167 6772 6567 6174 6564 5f64 6174 612e  aggregated_data.
-00012e70: 636f 6c75 6d6e 730a 2020 2020 2020 2020  columns.        
-00012e80: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
-00012e90: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-00012ea0: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00012eb0: 2020 2066 2243 6f6c 756d 6e28 7329 207b     f"Column(s) {
-00012ec0: 6472 6f70 7065 645f 636f 6c75 6d6e 737d  dropped_columns}
-00012ed0: 2061 7265 206e 6f74 2073 7570 706f 7274   are not support
-00012ee0: 6564 2066 6f72 2061 6767 7265 6761 7469  ed for aggregati
-00012ef0: 6f6e 2c20 7374 6f70 220a 2020 2020 2020  on, stop".      
-00012f00: 2020 2020 2020 290a 0a20 2020 2023 2050        )..    # P
-00012f10: 726f 6365 7373 2073 7061 7469 616c 2063  rocess spatial c
-00012f20: 6f6d 706f 6e65 6e74 0a20 2020 2064 6566  omponent.    def
-00012f30: 206d 6572 6765 5f67 656f 6d65 7472 6965   merge_geometrie
-00012f40: 7328 626c 6f63 6b29 3a0a 2020 2020 2020  s(block):.      
-00012f50: 2020 6d65 7267 6564 5f67 656f 6d20 3d20    merged_geom = 
-00012f60: 626c 6f63 6b2e 756e 6172 795f 756e 696f  block.unary_unio
-00012f70: 6e0a 2020 2020 2020 2020 7265 7475 726e  n.        return
-00012f80: 206d 6572 6765 645f 6765 6f6d 0a0a 2020   merged_geom..  
-00012f90: 2020 6720 3d20 6466 2e67 726f 7570 6279    g = df.groupby
-00012fa0: 2867 726f 7570 5f6b 6579 733d 4661 6c73  (group_keys=Fals
-00012fb0: 652c 202a 2a67 726f 7570 6279 5f6b 7761  e, **groupby_kwa
-00012fc0: 7267 7329 5b64 662e 6765 6f6d 6574 7279  rgs)[df.geometry
-00012fd0: 2e6e 616d 655d 2e61 6767 280a 2020 2020  .name].agg(.    
-00012fe0: 2020 2020 6d65 7267 655f 6765 6f6d 6574      merge_geomet
-00012ff0: 7269 6573 0a20 2020 2029 0a0a 2020 2020  ries.    )..    
-00013000: 2320 4167 6772 6567 6174 650a 2020 2020  # Aggregate.    
-00013010: 6167 6772 6567 6174 6564 5f67 656f 6d65  aggregated_geome
-00013020: 7472 7920 3d20 6770 642e 4765 6f44 6174  try = gpd.GeoDat
-00013030: 6146 7261 6d65 280a 2020 2020 2020 2020  aFrame(.        
-00013040: 6461 7461 3d67 2c20 6765 6f6d 6574 7279  data=g, geometry
-00013050: 3d64 662e 6765 6f6d 6574 7279 2e6e 616d  =df.geometry.nam
-00013060: 652c 2063 7273 3d64 662e 6372 730a 2020  e, crs=df.crs.  
-00013070: 2020 290a 2020 2020 2320 5265 636f 6d62    ).    # Recomb
-00013080: 696e 650a 2020 2020 6167 6772 6567 6174  ine.    aggregat
-00013090: 6564 203d 2061 6767 7265 6761 7465 645f  ed = aggregated_
-000130a0: 6765 6f6d 6574 7279 2e6a 6f69 6e28 6167  geometry.join(ag
-000130b0: 6772 6567 6174 6564 5f64 6174 6129 0a0a  gregated_data)..
-000130c0: 2020 2020 2320 5265 7365 7420 6966 2072      # Reset if r
-000130d0: 6571 7565 7374 6564 0a20 2020 2069 6620  equested.    if 
-000130e0: 6e6f 7420 6173 5f69 6e64 6578 3a0a 2020  not as_index:.  
-000130f0: 2020 2020 2020 6167 6772 6567 6174 6564        aggregated
-00013100: 203d 2061 6767 7265 6761 7465 642e 7265   = aggregated.re
-00013110: 7365 745f 696e 6465 7828 290a 0a20 2020  set_index()..   
-00013120: 2023 204d 616b 6520 7375 7265 206f 7574   # Make sure out
-00013130: 7075 7420 7479 7065 7320 6f66 2067 726f  put types of gro
-00013140: 7570 6564 2063 6f6c 756d 6e73 2061 7265  uped columns are
-00013150: 2074 6865 2073 616d 6520 6173 2069 6e70   the same as inp
-00013160: 7574 2074 7970 6573 2e0a 2020 2020 2320  ut types..    # 
-00013170: 452e 672e 206f 626a 6563 7420 636f 6c75  E.g. object colu
-00013180: 6d6e 7320 6265 636f 6d65 2066 6c6f 6174  mns become float
-00013190: 2069 6620 616c 6c20 7661 6c75 6573 2061   if all values a
-000131a0: 7265 204e 6f6e 652e 0a20 2020 2069 6620  re None..    if 
-000131b0: 6279 2069 7320 6e6f 7420 4e6f 6e65 3a0a  by is not None:.
-000131c0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-000131d0: 7461 6e63 6528 6279 2c20 7374 7229 3a0a  tance(by, str):.
-000131e0: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-000131f0: 7920 696e 2061 6767 7265 6761 7465 642e  y in aggregated.
-00013200: 636f 6c75 6d6e 7320 616e 6420 6466 5b62  columns and df[b
-00013210: 795d 2e64 7479 7065 2021 3d20 6167 6772  y].dtype != aggr
-00013220: 6567 6174 6564 5b62 795d 2e64 7479 7065  egated[by].dtype
-00013230: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013240: 2020 6167 6772 6567 6174 6564 5b62 795d    aggregated[by]
-00013250: 203d 2061 6767 7265 6761 7465 645b 6279   = aggregated[by
-00013260: 5d2e 6173 7479 7065 2864 665b 6279 5d2e  ].astype(df[by].
-00013270: 6474 7970 6529 0a20 2020 2020 2020 2065  dtype).        e
-00013280: 6c69 6620 6973 696e 7374 616e 6365 2862  lif isinstance(b
-00013290: 792c 2049 7465 7261 626c 6529 3a0a 2020  y, Iterable):.  
-000132a0: 2020 2020 2020 2020 2020 666f 7220 636f            for co
-000132b0: 6c20 696e 2062 793a 0a20 2020 2020 2020  l in by:.       
-000132c0: 2020 2020 2020 2020 2069 6620 636f 6c20           if col 
-000132d0: 696e 2061 6767 7265 6761 7465 642e 636f  in aggregated.co
-000132e0: 6c75 6d6e 7320 616e 6420 6466 5b63 6f6c  lumns and df[col
-000132f0: 5d2e 6474 7970 6520 213d 2061 6767 7265  ].dtype != aggre
-00013300: 6761 7465 645b 636f 6c5d 2e64 7479 7065  gated[col].dtype
-00013310: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00013320: 2020 2020 2020 6167 6772 6567 6174 6564        aggregated
-00013330: 5b63 6f6c 5d20 3d20 6167 6772 6567 6174  [col] = aggregat
-00013340: 6564 5b63 6f6c 5d2e 6173 7479 7065 2864  ed[col].astype(d
-00013350: 665b 636f 6c5d 2e64 7479 7065 290a 0a20  f[col].dtype).. 
-00013360: 2020 2061 7373 6572 7420 6973 696e 7374     assert isinst
-00013370: 616e 6365 2861 6767 7265 6761 7465 642c  ance(aggregated,
-00013380: 2067 7064 2e47 656f 4461 7461 4672 616d   gpd.GeoDataFram
-00013390: 6529 0a20 2020 2072 6574 7572 6e20 6167  e).    return ag
-000133a0: 6772 6567 6174 6564 0a0a 0a64 6566 205f  gregated...def _
-000133b0: 6164 645f 6f72 6465 7262 795f 636f 6c75  add_orderby_colu
-000133c0: 6d6e 2870 6174 683a 2050 6174 682c 206c  mn(path: Path, l
-000133d0: 6179 6572 3a20 7374 722c 206e 616d 653a  ayer: str, name:
-000133e0: 2073 7472 293a 0a20 2020 2023 2050 7265   str):.    # Pre
-000133f0: 7061 7265 2074 6865 2065 7870 7265 7373  pare the express
-00013400: 696f 6e20 746f 2063 616c 6375 6c61 7465  ion to calculate
-00013410: 2074 6865 206f 7264 6572 6279 2063 6f6c   the orderby col
-00013420: 756d 6e2e 0a20 2020 2023 2049 6e20 6120  umn..    # In a 
-00013430: 7370 6174 6961 6c20 6669 6c65 2c20 6120  spatial file, a 
-00013440: 7370 6174 6961 6c20 6f72 6465 7220 7769  spatial order wi
-00013450: 6c6c 206d 616b 6520 6c61 7465 7220 7573  ll make later us
-00013460: 6520 6d6f 7265 2065 6666 6963 69c3 ab6e  e more effici..n
-00013470: 742c 0a20 2020 2023 2073 6f20 7573 6520  t,.    # so use 
-00013480: 6120 6765 6f68 6173 682e 0a20 2020 206c  a geohash..    l
-00013490: 6179 6572 696e 666f 203d 2067 666f 2e67  ayerinfo = gfo.g
-000134a0: 6574 5f6c 6179 6572 696e 666f 2870 6174  et_layerinfo(pat
-000134b0: 6829 0a20 2020 2069 6620 6c61 7965 7269  h).    if layeri
-000134c0: 6e66 6f2e 6372 7320 6973 206e 6f74 204e  nfo.crs is not N
-000134d0: 6f6e 6520 616e 6420 6c61 7965 7269 6e66  one and layerinf
-000134e0: 6f2e 6372 732e 6973 5f67 656f 6772 6170  o.crs.is_geograp
-000134f0: 6869 633a 0a20 2020 2020 2020 2023 2049  hic:.        # I
-00013500: 6620 7468 6520 636f 6f72 6469 6e61 7465  f the coordinate
-00013510: 7320 6172 6520 6765 6f67 7261 7068 6963  s are geographic
-00013520: 2028 696e 206c 6174 2f6c 6f6e 2064 6567   (in lat/lon deg
-00013530: 7265 6573 292c 206f 6b0a 2020 2020 2020  rees), ok.      
-00013540: 2020 6578 7072 6573 7369 6f6e 203d 2066    expression = f
-00013550: 2253 545f 4765 6f48 6173 6828 7b6c 6179  "ST_GeoHash({lay
-00013560: 6572 696e 666f 2e67 656f 6d65 7472 7963  erinfo.geometryc
-00013570: 6f6c 756d 6e7d 2c20 3130 2922 0a20 2020  olumn}, 10)".   
-00013580: 2065 6c73 653a 0a20 2020 2020 2020 2023   else:.        #
-00013590: 2049 6620 7468 6579 2061 7265 206e 6f74   If they are not
-000135a0: 2067 656f 6772 6170 6869 6320 2869 6e20   geographic (in 
-000135b0: 6c61 742f 6c6f 6e20 6465 6772 6565 7329  lat/lon degrees)
-000135c0: 2c20 7468 6579 206e 6565 6420 746f 2062  , they need to b
-000135d0: 650a 2020 2020 2020 2020 2320 636f 6e76  e.        # conv
-000135e0: 6572 7465 6420 746f 207e 2064 6567 7265  erted to ~ degre
-000135f0: 6573 2074 6f20 6265 2061 626c 6520 746f  es to be able to
-00013600: 2063 616c 6375 6c61 7465 2061 2067 656f   calculate a geo
-00013610: 6861 7368 2e0a 0a20 2020 2020 2020 2023  hash...        #
-00013620: 2050 726f 7065 726c 7920 6361 6c63 756c   Properly calcul
-00013630: 6174 696e 6720 7468 6520 7472 616e 7366  ating the transf
-00013640: 6f72 6d61 7469 6f6e 2074 6f20 6567 2e20  ormation to eg. 
-00013650: 5747 5320 6973 2074 6572 7269 626c 7920  WGS is terribly 
-00013660: 736c 6f77 2e2e 2e0a 2020 2020 2020 2020  slow....        
-00013670: 2320 6578 7072 6573 7369 6f6e 203d 2066  # expression = f
-00013680: 2222 2253 545f 4765 6f48 6173 6828 5354  """ST_GeoHash(ST
-00013690: 5f54 7261 6e73 666f 726d 284d 616b 6550  _Transform(MakeP
-000136a0: 6f69 6e74 280a 2020 2020 2020 2020 2320  oint(.        # 
-000136b0: 2020 2020 2020 284d 6272 4d61 7858 2867        (MbrMaxX(g
-000136c0: 656f 6d29 2b4d 6272 4d69 6e58 2867 656f  eom)+MbrMinX(geo
-000136d0: 6d29 292f 322c 0a20 2020 2020 2020 2023  m))/2,.        #
-000136e0: 2020 2020 2020 2028 4d62 724d 696e 5928         (MbrMinY(
-000136f0: 6765 6f6d 292b 4d62 724d 6178 5928 6765  geom)+MbrMaxY(ge
-00013700: 6f6d 2929 2f32 2c20 5354 5f53 5249 4428  om))/2, ST_SRID(
-00013710: 6765 6f6d 2929 2c20 3433 3236 292c 2031  geom)), 4326), 1
-00013720: 3029 2222 220a 2020 2020 2020 2020 2320  0)""".        # 
-00013730: 536f 2c20 646f 2073 6f6d 6574 6869 6e67  So, do something
-00013740: 2065 6c73 6520 7468 6174 2773 2066 6173   else that's fas
-00013750: 7465 7220 616e 6420 7374 696c 6c20 6769  ter and still gi
-00013760: 7665 7320 6120 676f 6f64 0a20 2020 2020  ves a good.     
-00013770: 2020 2023 2067 656f 6772 6170 6869 6320     # geographic 
-00013780: 636c 7573 7465 7269 6e67 2e0a 2020 2020  clustering..    
-00013790: 2020 2020 746f 5f67 656f 6772 6170 6869      to_geographi
-000137a0: 635f 6661 6374 6f72 5f61 7070 726f 7820  c_factor_approx 
-000137b0: 3d20 3930 202f 206d 6178 286c 6179 6572  = 90 / max(layer
-000137c0: 696e 666f 2e74 6f74 616c 5f62 6f75 6e64  info.total_bound
-000137d0: 7329 0a20 2020 2020 2020 2065 7870 7265  s).        expre
-000137e0: 7373 696f 6e20 3d20 6622 2222 5354 5f47  ssion = f"""ST_G
-000137f0: 656f 4861 7368 284d 616b 6550 6f69 6e74  eoHash(MakePoint
-00013800: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00013810: 2020 2828 4d62 724d 6178 5828 7b6c 6179    ((MbrMaxX({lay
-00013820: 6572 696e 666f 2e67 656f 6d65 7472 7963  erinfo.geometryc
-00013830: 6f6c 756d 6e7d 290a 2020 2020 2020 2020  olumn}).        
-00013840: 2020 2020 2020 2020 2020 2b4d 6272 4d69            +MbrMi
-00013850: 6e58 287b 6c61 7965 7269 6e66 6f2e 6765  nX({layerinfo.ge
-00013860: 6f6d 6574 7279 636f 6c75 6d6e 7d29 292f  ometrycolumn}))/
-00013870: 320a 2020 2020 2020 2020 2020 2020 2020  2.              
-00013880: 2020 292a 7b74 6f5f 6765 6f67 7261 7068    )*{to_geograph
-00013890: 6963 5f66 6163 746f 725f 6170 7072 6f78  ic_factor_approx
-000138a0: 7d2c 0a20 2020 2020 2020 2020 2020 2020  },.             
-000138b0: 2020 2028 284d 6272 4d69 6e59 287b 6c61     ((MbrMinY({la
-000138c0: 7965 7269 6e66 6f2e 6765 6f6d 6574 7279  yerinfo.geometry
-000138d0: 636f 6c75 6d6e 7d29 0a20 2020 2020 2020  column}).       
-000138e0: 2020 2020 2020 2020 2020 202b 4d62 724d             +MbrM
-000138f0: 6178 5928 7b6c 6179 6572 696e 666f 2e67  axY({layerinfo.g
-00013900: 656f 6d65 7472 7963 6f6c 756d 6e7d 2929  eometrycolumn}))
-00013910: 2f32 0a20 2020 2020 2020 2020 2020 2020  /2.             
-00013920: 2020 2029 2a7b 746f 5f67 656f 6772 6170     )*{to_geograp
-00013930: 6869 635f 6661 6374 6f72 5f61 7070 726f  hic_factor_appro
-00013940: 787d 2c20 3433 3236 292c 2031 3029 2222  x}, 4326), 10)""
-00013950: 220a 0a20 2020 2023 204e 6f77 2077 6520  "..    # Now we 
-00013960: 6361 6e20 6163 7475 616c 6c79 2061 6464  can actually add
-00013970: 2074 6865 2063 6f6c 756d 6e2e 0a20 2020   the column..   
-00013980: 2067 666f 2e61 6464 5f63 6f6c 756d 6e28   gfo.add_column(
-00013990: 7061 7468 3d70 6174 682c 206e 616d 653d  path=path, name=
-000139a0: 6e61 6d65 2c20 7479 7065 3d67 666f 2e44  name, type=gfo.D
-000139b0: 6174 6154 7970 652e 5445 5854 2c20 6578  ataType.TEXT, ex
-000139c0: 7072 6573 7369 6f6e 3d65 7870 7265 7373  pression=express
-000139d0: 696f 6e29 0a20 2020 2073 716c 6974 655f  ion).    sqlite_
-000139e0: 7374 6d74 203d 2066 2743 5245 4154 4520  stmt = f'CREATE 
-000139f0: 494e 4445 5820 7b6e 616d 657d 5f69 6478  INDEX {name}_idx
-00013a00: 204f 4e20 227b 6c61 7965 727d 2228 7b6e   ON "{layer}"({n
-00013a10: 616d 657d 2927 0a20 2020 2067 666f 2e65  ame})'.    gfo.e
-00013a20: 7865 6375 7465 5f73 716c 2870 6174 683d  xecute_sql(path=
-00013a30: 7061 7468 2c20 7371 6c5f 7374 6d74 3d73  path, sql_stmt=s
-00013a40: 716c 6974 655f 7374 6d74 290a            qlite_stmt).
+00011570: 2029 0a20 2020 2070 6572 6669 6e66 6f5b   ).    perfinfo[
+00011580: 2274 696d 655f 746f 5f66 696c 6522 5d20  "time_to_file"] 
+00011590: 3d20 2864 6174 6574 696d 652e 6e6f 7728  = (datetime.now(
+000115a0: 2920 2d20 7374 6172 745f 746f 5f66 696c  ) - start_to_fil
+000115b0: 6529 2e74 6f74 616c 5f73 6563 6f6e 6473  e).total_seconds
+000115c0: 2829 0a0a 2020 2020 2320 4669 6e61 6c69  ()..    # Finali
+000115d0: 7365 2e2e 2e0a 2020 2020 6d65 7373 6167  se....    messag
+000115e0: 6520 3d20 6622 6469 7373 6f6c 7665 2072  e = f"dissolve r
+000115f0: 6561 6479 2069 6e20 7b64 6174 6574 696d  eady in {datetim
+00011600: 652e 6e6f 7728 292d 7374 6172 745f 7469  e.now()-start_ti
+00011610: 6d65 7d20 6f6e 207b 696e 7075 745f 7061  me} on {input_pa
+00011620: 7468 7d21 220a 2020 2020 6c6f 6767 6572  th}!".    logger
+00011630: 2e64 6562 7567 286d 6573 7361 6765 290a  .debug(message).
+00011640: 0a20 2020 2023 2043 6f6c 6c65 6374 2070  .    # Collect p
+00011650: 6572 6669 6e66 6f0a 2020 2020 746f 7461  erfinfo.    tota
+00011660: 6c5f 7065 7266 5f74 696d 6520 3d20 300a  l_perf_time = 0.
+00011670: 2020 2020 7065 7266 7374 7269 6e67 203d      perfstring =
+00011680: 2022 220a 2020 2020 666f 7220 7065 7266   "".    for perf
+00011690: 636f 6465 2069 6e20 7065 7266 696e 666f  code in perfinfo
+000116a0: 3a0a 2020 2020 2020 2020 746f 7461 6c5f  :.        total_
+000116b0: 7065 7266 5f74 696d 6520 2b3d 2070 6572  perf_time += per
+000116c0: 6669 6e66 6f5b 7065 7266 636f 6465 5d0a  finfo[perfcode].
+000116d0: 2020 2020 2020 2020 7065 7266 7374 7269          perfstri
+000116e0: 6e67 202b 3d20 6622 7b70 6572 6663 6f64  ng += f"{perfcod
+000116f0: 657d 3a20 7b70 6572 6669 6e66 6f5b 7065  e}: {perfinfo[pe
+00011700: 7266 636f 6465 5d3a 2e32 667d 2c20 220a  rfcode]:.2f}, ".
+00011710: 2020 2020 7265 7475 726e 5f69 6e66 6f5b      return_info[
+00011720: 2274 6f74 616c 5f74 696d 6522 5d20 3d20  "total_time"] = 
+00011730: 2864 6174 6574 696d 652e 6e6f 7728 2920  (datetime.now() 
+00011740: 2d20 7374 6172 745f 7469 6d65 292e 746f  - start_time).to
+00011750: 7461 6c5f 7365 636f 6e64 7328 290a 2020  tal_seconds().  
+00011760: 2020 7065 7266 696e 666f 5b22 756e 6163    perfinfo["unac
+00011770: 636f 756e 7465 6422 5d20 3d20 7265 7475  counted"] = retu
+00011780: 726e 5f69 6e66 6f5b 2274 6f74 616c 5f74  rn_info["total_t
+00011790: 696d 6522 5d20 2d20 746f 7461 6c5f 7065  ime"] - total_pe
+000117a0: 7266 5f74 696d 650a 2020 2020 7065 7266  rf_time.    perf
+000117b0: 7374 7269 6e67 202b 3d20 6622 756e 6163  string += f"unac
+000117c0: 636f 756e 7465 643a 207b 7065 7266 696e  counted: {perfin
+000117d0: 666f 5b27 756e 6163 636f 756e 7465 6427  fo['unaccounted'
+000117e0: 5d3a 2e32 667d 220a 0a20 2020 2023 2052  ]:.2f}"..    # R
+000117f0: 6574 7572 6e0a 2020 2020 7265 7475 726e  eturn.    return
+00011800: 5f69 6e66 6f5b 2270 6572 6669 6e66 6f22  _info["perfinfo"
+00011810: 5d20 3d20 7065 7266 696e 666f 0a20 2020  ] = perfinfo.   
+00011820: 2072 6574 7572 6e5f 696e 666f 5b22 7065   return_info["pe
+00011830: 7266 7374 7269 6e67 225d 203d 2070 6572  rfstring"] = per
+00011840: 6673 7472 696e 670a 2020 2020 7265 7475  fstring.    retu
+00011850: 726e 5f69 6e66 6f5b 226d 6573 7361 6765  rn_info["message
+00011860: 225d 203d 206d 6573 7361 6765 0a20 2020  "] = message.   
+00011870: 2072 6574 7572 6e20 7265 7475 726e 5f69   return return_i
+00011880: 6e66 6f0a 0a0a 6465 6620 5f64 6973 736f  nfo...def _disso
+00011890: 6c76 6528 0a20 2020 2064 663a 2067 7064  lve(.    df: gpd
+000118a0: 2e47 656f 4461 7461 4672 616d 652c 0a20  .GeoDataFrame,. 
+000118b0: 2020 2062 793d 4e6f 6e65 2c0a 2020 2020     by=None,.    
+000118c0: 6167 6766 756e 633a 204f 7074 696f 6e61  aggfunc: Optiona
+000118d0: 6c5b 556e 696f 6e5b 7374 722c 2064 6963  l[Union[str, dic
+000118e0: 745d 5d20 3d20 2266 6972 7374 222c 0a20  t]] = "first",. 
+000118f0: 2020 2061 735f 696e 6465 783d 5472 7565     as_index=True
+00011900: 2c0a 2020 2020 6c65 7665 6c3d 4e6f 6e65  ,.    level=None
+00011910: 2c0a 2020 2020 736f 7274 3d54 7275 652c  ,.    sort=True,
+00011920: 0a20 2020 206f 6273 6572 7665 643d 4661  .    observed=Fa
+00011930: 6c73 652c 0a20 2020 2064 726f 706e 613d  lse,.    dropna=
+00011940: 5472 7565 2c0a 2920 2d3e 2067 7064 2e47  True,.) -> gpd.G
+00011950: 656f 4461 7461 4672 616d 653a 0a20 2020  eoDataFrame:.   
+00011960: 2022 2222 0a20 2020 2044 6973 736f 6c76   """.    Dissolv
+00011970: 6520 6765 6f6d 6574 7269 6573 2077 6974  e geometries wit
+00011980: 6869 6e20 6067 726f 7570 6279 6020 696e  hin `groupby` in
+00011990: 746f 2073 696e 676c 6520 6f62 7365 7276  to single observ
+000119a0: 6174 696f 6e2e 0a20 2020 2054 6869 7320  ation..    This 
+000119b0: 6973 2061 6363 6f6d 706c 6973 6865 6420  is accomplished 
+000119c0: 6279 2061 7070 6c79 696e 6720 7468 6520  by applying the 
+000119d0: 6075 6e61 7279 5f75 6e69 6f6e 6020 6d65  `unary_union` me
+000119e0: 7468 6f64 0a20 2020 2074 6f20 616c 6c20  thod.    to all 
+000119f0: 6765 6f6d 6574 7269 6573 2077 6974 6869  geometries withi
+00011a00: 6e20 6120 6772 6f75 7073 656c 662e 0a20  n a groupself.. 
+00011a10: 2020 204f 6273 6572 7661 7469 6f6e 7320     Observations 
+00011a20: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
+00011a30: 6561 6368 2060 6772 6f75 7062 7960 2067  each `groupby` g
+00011a40: 726f 7570 2077 696c 6c20 6265 2061 6767  roup will be agg
+00011a50: 7265 6761 7465 640a 2020 2020 7573 696e  regated.    usin
+00011a60: 6720 7468 6520 6061 6767 6675 6e63 602e  g the `aggfunc`.
+00011a70: 0a20 2020 2050 6172 616d 6574 6572 730a  .    Parameters.
+00011a80: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+00011a90: 2020 2062 7920 3a20 7374 7269 6e67 2c20     by : string, 
+00011aa0: 6465 6661 756c 7420 4e6f 6e65 0a20 2020  default None.   
+00011ab0: 2020 2020 2043 6f6c 756d 6e20 7768 6f73       Column whos
+00011ac0: 6520 7661 6c75 6573 2064 6566 696e 6520  e values define 
+00011ad0: 6772 6f75 7073 2074 6f20 6265 2064 6973  groups to be dis
+00011ae0: 736f 6c76 6564 2e20 4966 204e 6f6e 652c  solved. If None,
+00011af0: 0a20 2020 2020 2020 2077 686f 6c65 2047  .        whole G
+00011b00: 656f 4461 7461 4672 616d 6520 6973 2063  eoDataFrame is c
+00011b10: 6f6e 7369 6465 7265 6420 6120 7369 6e67  onsidered a sing
+00011b20: 6c65 2067 726f 7570 2e0a 2020 2020 6167  le group..    ag
+00011b30: 6766 756e 6320 3a20 6675 6e63 7469 6f6e  gfunc : function
+00011b40: 2c20 7374 7269 6e67 206f 7220 6469 6374  , string or dict
+00011b50: 2c20 6465 6661 756c 7420 2266 6972 7374  , default "first
+00011b60: 220a 2020 2020 2020 2020 4167 6772 6567  ".        Aggreg
+00011b70: 6174 696f 6e20 6675 6e63 7469 6f6e 2066  ation function f
+00011b80: 6f72 206d 616e 6970 756c 6174 696f 6e20  or manipulation 
+00011b90: 6f66 2064 6174 6120 6173 736f 6369 6174  of data associat
+00011ba0: 6564 0a20 2020 2020 2020 2077 6974 6820  ed.        with 
+00011bb0: 6561 6368 2067 726f 7570 2e20 5061 7373  each group. Pass
+00011bc0: 6564 2074 6f20 7061 6e64 6173 2060 6772  ed to pandas `gr
+00011bd0: 6f75 7062 792e 6167 6760 206d 6574 686f  oupby.agg` metho
+00011be0: 642e 0a20 2020 2061 735f 696e 6465 7820  d..    as_index 
+00011bf0: 3a20 626f 6f6c 6561 6e2c 2064 6566 6175  : boolean, defau
+00011c00: 6c74 2054 7275 650a 2020 2020 2020 2020  lt True.        
+00011c10: 4966 2074 7275 652c 2067 726f 7570 6279  If true, groupby
+00011c20: 2063 6f6c 756d 6e73 2062 6563 6f6d 6520   columns become 
+00011c30: 696e 6465 7820 6f66 2072 6573 756c 742e  index of result.
+00011c40: 0a20 2020 206c 6576 656c 203a 2069 6e74  .    level : int
+00011c50: 206f 7220 7374 7220 6f72 2073 6571 7565   or str or seque
+00011c60: 6e63 6520 6f66 2069 6e74 206f 7220 7365  nce of int or se
+00011c70: 7175 656e 6365 206f 6620 7374 722c 2064  quence of str, d
+00011c80: 6566 6175 6c74 204e 6f6e 650a 2020 2020  efault None.    
+00011c90: 2020 2020 4966 2074 6865 2061 7869 7320      If the axis 
+00011ca0: 6973 2061 204d 756c 7469 496e 6465 7820  is a MultiIndex 
+00011cb0: 2868 6965 7261 7263 6869 6361 6c29 2c20  (hierarchical), 
+00011cc0: 6772 6f75 7020 6279 2061 0a20 2020 2020  group by a.     
+00011cd0: 2020 2070 6172 7469 6375 6c61 7220 6c65     particular le
+00011ce0: 7665 6c20 6f72 206c 6576 656c 732e 0a20  vel or levels.. 
+00011cf0: 2020 2020 2020 202e 2e20 7665 7273 696f         .. versio
+00011d00: 6e61 6464 6564 3a3a 2030 2e39 2e30 0a20  nadded:: 0.9.0. 
+00011d10: 2020 2073 6f72 7420 3a20 626f 6f6c 2c20     sort : bool, 
+00011d20: 6465 6661 756c 7420 5472 7565 0a20 2020  default True.   
+00011d30: 2020 2020 2053 6f72 7420 6772 6f75 7020       Sort group 
+00011d40: 6b65 7973 2e20 4765 7420 6265 7474 6572  keys. Get better
+00011d50: 2070 6572 666f 726d 616e 6365 2062 7920   performance by 
+00011d60: 7475 726e 696e 6720 7468 6973 206f 6666  turning this off
+00011d70: 2e0a 2020 2020 2020 2020 4e6f 7465 2074  ..        Note t
+00011d80: 6869 7320 646f 6573 206e 6f74 2069 6e66  his does not inf
+00011d90: 6c75 656e 6365 2074 6865 206f 7264 6572  luence the order
+00011da0: 206f 6620 6f62 7365 7276 6174 696f 6e73   of observations
+00011db0: 2077 6974 6869 6e0a 2020 2020 2020 2020   within.        
+00011dc0: 6561 6368 2067 726f 7570 2e20 4772 6f75  each group. Grou
+00011dd0: 7062 7920 7072 6573 6572 7665 7320 7468  pby preserves th
+00011de0: 6520 6f72 6465 7220 6f66 2072 6f77 7320  e order of rows 
+00011df0: 7769 7468 696e 2065 6163 6820 6772 6f75  within each grou
+00011e00: 702e 0a20 2020 2020 2020 202e 2e20 7665  p..        .. ve
+00011e10: 7273 696f 6e61 6464 6564 3a3a 2030 2e39  rsionadded:: 0.9
+00011e20: 2e30 0a20 2020 206f 6273 6572 7665 6420  .0.    observed 
+00011e30: 3a20 626f 6f6c 2c20 6465 6661 756c 7420  : bool, default 
+00011e40: 4661 6c73 650a 2020 2020 2020 2020 5468  False.        Th
+00011e50: 6973 206f 6e6c 7920 6170 706c 6965 7320  is only applies 
+00011e60: 6966 2061 6e79 206f 6620 7468 6520 6772  if any of the gr
+00011e70: 6f75 7065 7273 2061 7265 2043 6174 6567  oupers are Categ
+00011e80: 6f72 6963 616c 732e 0a20 2020 2020 2020  oricals..       
+00011e90: 2049 6620 5472 7565 3a20 6f6e 6c79 2073   If True: only s
+00011ea0: 686f 7720 6f62 7365 7276 6564 2076 616c  how observed val
+00011eb0: 7565 7320 666f 7220 6361 7465 676f 7269  ues for categori
+00011ec0: 6361 6c20 6772 6f75 7065 7273 2e0a 2020  cal groupers..  
+00011ed0: 2020 2020 2020 4966 2046 616c 7365 3a20        If False: 
+00011ee0: 7368 6f77 2061 6c6c 2076 616c 7565 7320  show all values 
+00011ef0: 666f 7220 6361 7465 676f 7269 6361 6c20  for categorical 
+00011f00: 6772 6f75 7065 7273 2e0a 2020 2020 2020  groupers..      
+00011f10: 2020 2e2e 2076 6572 7369 6f6e 6164 6465    .. versionadde
+00011f20: 643a 3a20 302e 392e 300a 2020 2020 6472  d:: 0.9.0.    dr
+00011f30: 6f70 6e61 203a 2062 6f6f 6c2c 2064 6566  opna : bool, def
+00011f40: 6175 6c74 2054 7275 650a 2020 2020 2020  ault True.      
+00011f50: 2020 4966 2054 7275 652c 2061 6e64 2069    If True, and i
+00011f60: 6620 6772 6f75 7020 6b65 7973 2063 6f6e  f group keys con
+00011f70: 7461 696e 204e 4120 7661 6c75 6573 2c20  tain NA values, 
+00011f80: 4e41 2076 616c 7565 730a 2020 2020 2020  NA values.      
+00011f90: 2020 746f 6765 7468 6572 2077 6974 6820    together with 
+00011fa0: 726f 772f 636f 6c75 6d6e 2077 696c 6c20  row/column will 
+00011fb0: 6265 2064 726f 7070 6564 2e20 4966 2046  be dropped. If F
+00011fc0: 616c 7365 2c20 4e41 0a20 2020 2020 2020  alse, NA.       
+00011fd0: 2076 616c 7565 7320 7769 6c6c 2061 6c73   values will als
+00011fe0: 6f20 6265 2074 7265 6174 6564 2061 7320  o be treated as 
+00011ff0: 7468 6520 6b65 7920 696e 2067 726f 7570  the key in group
+00012000: 732e 0a20 2020 2020 2020 2054 6869 7320  s..        This 
+00012010: 7061 7261 6d65 7465 7220 6973 206e 6f74  parameter is not
+00012020: 2073 7570 706f 7274 6564 2066 6f72 2070   supported for p
+00012030: 616e 6461 7320 3c20 312e 312e 302e 0a20  andas < 1.1.0.. 
+00012040: 2020 2020 2020 2041 2077 6172 6e69 6e67         A warning
+00012050: 2077 696c 6c20 6265 2065 6d69 7474 6564   will be emitted
+00012060: 2066 6f72 2065 6172 6c69 6572 2070 616e   for earlier pan
+00012070: 6461 7320 7665 7273 696f 6e73 0a20 2020  das versions.   
+00012080: 2020 2020 2069 6620 6120 6e6f 6e2d 6465       if a non-de
+00012090: 6661 756c 7420 7661 6c75 6520 6973 2067  fault value is g
+000120a0: 6976 656e 2066 6f72 2074 6869 7320 7061  iven for this pa
+000120b0: 7261 6d65 7465 722e 0a20 2020 2020 2020  rameter..       
+000120c0: 202e 2e20 7665 7273 696f 6e61 6464 6564   .. versionadded
+000120d0: 3a3a 2030 2e39 2e30 0a20 2020 2052 6574  :: 0.9.0.    Ret
+000120e0: 7572 6e73 0a20 2020 202d 2d2d 2d2d 2d2d  urns.    -------
+000120f0: 0a20 2020 2047 656f 4461 7461 4672 616d  .    GeoDataFram
+00012100: 650a 2020 2020 4578 616d 706c 6573 0a20  e.    Examples. 
+00012110: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
+00012120: 3e3e 3e20 6672 6f6d 2073 6861 7065 6c79  >>> from shapely
+00012130: 2e67 656f 6d65 7472 7920 696d 706f 7274  .geometry import
+00012140: 2050 6f69 6e74 0a20 2020 203e 3e3e 2064   Point.    >>> d
+00012150: 203d 207b 0a20 2020 202e 2e2e 2020 2020   = {.    ...    
+00012160: 2022 636f 6c31 223a 205b 226e 616d 6531   "col1": ["name1
+00012170: 222c 2022 6e61 6d65 3222 2c20 226e 616d  ", "name2", "nam
+00012180: 6531 225d 2c0a 2020 2020 2e2e 2e20 2020  e1"],.    ...   
+00012190: 2020 2267 656f 6d65 7472 7922 3a20 5b50    "geometry": [P
+000121a0: 6f69 6e74 2831 2c20 3229 2c20 506f 696e  oint(1, 2), Poin
+000121b0: 7428 322c 2031 292c 2050 6f69 6e74 2830  t(2, 1), Point(0
+000121c0: 2c20 3129 5d2c 0a20 2020 202e 2e2e 207d  , 1)],.    ... }
+000121d0: 0a20 2020 203e 3e3e 2067 6466 203d 2067  .    >>> gdf = g
+000121e0: 656f 7061 6e64 6173 2e47 656f 4461 7461  eopandas.GeoData
+000121f0: 4672 616d 6528 642c 2063 7273 3d34 3332  Frame(d, crs=432
+00012200: 3629 0a20 2020 203e 3e3e 2067 6466 0a20  6).    >>> gdf. 
+00012210: 2020 2020 2020 2063 6f6c 3120 2020 2020         col1     
+00012220: 2020 2020 2020 2020 2020 2020 6765 6f6d              geom
+00012230: 6574 7279 0a20 2020 2030 2020 6e61 6d65  etry.    0  name
+00012240: 3120 2050 4f49 4e54 2028 312e 3030 3030  1  POINT (1.0000
+00012250: 3020 322e 3030 3030 3029 0a20 2020 2031  0 2.00000).    1
+00012260: 2020 6e61 6d65 3220 2050 4f49 4e54 2028    name2  POINT (
+00012270: 322e 3030 3030 3020 312e 3030 3030 3029  2.00000 1.00000)
+00012280: 0a20 2020 2032 2020 6e61 6d65 3120 2050  .    2  name1  P
+00012290: 4f49 4e54 2028 302e 3030 3030 3020 312e  OINT (0.00000 1.
+000122a0: 3030 3030 3029 0a20 2020 203e 3e3e 2064  00000).    >>> d
+000122b0: 6973 736f 6c76 6564 203d 2067 6466 2e64  issolved = gdf.d
+000122c0: 6973 736f 6c76 6528 2763 6f6c 3127 290a  issolve('col1').
+000122d0: 2020 2020 3e3e 3e20 6469 7373 6f6c 7665      >>> dissolve
+000122e0: 6420 2023 2064 6f63 7465 7374 3a20 2b53  d  # doctest: +S
+000122f0: 4b49 500a 2020 2020 2020 2020 2020 2020  KIP.            
+00012300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012310: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012320: 2020 2020 6765 6f6d 6574 7279 0a20 2020      geometry.   
+00012330: 2063 6f6c 310a 2020 2020 6e61 6d65 3120   col1.    name1 
+00012340: 204d 554c 5449 504f 494e 5420 2830 2e30   MULTIPOINT (0.0
+00012350: 3030 3030 2031 2e30 3030 3030 2c20 312e  0000 1.00000, 1.
+00012360: 3030 3030 3020 322e 3030 3030 3029 0a20  00000 2.00000). 
+00012370: 2020 206e 616d 6532 2020 2020 2020 2020     name2        
+00012380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012390: 504f 494e 5420 2832 2e30 3030 3030 2031  POINT (2.00000 1
+000123a0: 2e30 3030 3030 290a 2020 2020 5365 6520  .00000).    See 
+000123b0: 616c 736f 0a20 2020 202d 2d2d 2d2d 2d2d  also.    -------
+000123c0: 2d0a 2020 2020 4765 6f44 6174 6146 7261  -.    GeoDataFra
+000123d0: 6d65 2e65 7870 6c6f 6465 203a 2065 7870  me.explode : exp
+000123e0: 6c6f 6465 206d 756c 7469 2d70 6172 7420  lode multi-part 
+000123f0: 6765 6f6d 6574 7269 6573 2069 6e74 6f20  geometries into 
+00012400: 7369 6e67 6c65 2067 656f 6d65 7472 6965  single geometrie
+00012410: 730a 2020 2020 2222 220a 0a20 2020 2069  s.    """..    i
+00012420: 6620 6279 2069 7320 4e6f 6e65 2061 6e64  f by is None and
+00012430: 206c 6576 656c 2069 7320 4e6f 6e65 3a0a   level is None:.
+00012440: 2020 2020 2020 2020 6279 5f6c 6f63 616c          by_local
+00012450: 203d 206e 702e 7a65 726f 7328 6c65 6e28   = np.zeros(len(
+00012460: 6466 292c 2064 7479 7065 3d22 696e 7436  df), dtype="int6
+00012470: 3422 290a 2020 2020 656c 7365 3a0a 2020  4").    else:.  
+00012480: 2020 2020 2020 6279 5f6c 6f63 616c 203d        by_local =
+00012490: 2062 790a 0a20 2020 2067 726f 7570 6279   by..    groupby
+000124a0: 5f6b 7761 7267 7320 3d20 7b0a 2020 2020  _kwargs = {.    
+000124b0: 2020 2020 2262 7922 3a20 6279 5f6c 6f63      "by": by_loc
+000124c0: 616c 2c0a 2020 2020 2020 2020 226c 6576  al,.        "lev
+000124d0: 656c 223a 206c 6576 656c 2c0a 2020 2020  el": level,.    
+000124e0: 2020 2020 2273 6f72 7422 3a20 736f 7274      "sort": sort
+000124f0: 2c0a 2020 2020 2020 2020 226f 6273 6572  ,.        "obser
+00012500: 7665 6422 3a20 6f62 7365 7276 6564 2c0a  ved": observed,.
+00012510: 2020 2020 2020 2020 2264 726f 706e 6122          "dropna"
+00012520: 3a20 6472 6f70 6e61 2c0a 2020 2020 7d0a  : dropna,.    }.
+00012530: 2020 2020 2222 220a 2020 2020 6966 206e      """.    if n
+00012540: 6f74 2063 6f6d 7061 742e 5041 4e44 4153  ot compat.PANDAS
+00012550: 5f47 455f 3131 3a0a 2020 2020 2020 2020  _GE_11:.        
+00012560: 6772 6f75 7062 795f 6b77 6172 6773 2e70  groupby_kwargs.p
+00012570: 6f70 2822 6472 6f70 6e61 2229 0a0a 2020  op("dropna")..  
+00012580: 2020 2020 2020 6966 206e 6f74 2064 726f        if not dro
+00012590: 706e 613a 2020 2320 4966 2074 6865 7920  pna:  # If they 
+000125a0: 7061 7373 6564 2061 206e 6f6e 2d64 6566  passed a non-def
+000125b0: 6175 6c74 2064 726f 706e 6120 7661 6c75  ault dropna valu
+000125c0: 650a 2020 2020 2020 2020 2020 2020 7761  e.            wa
+000125d0: 726e 696e 6773 2e77 6172 6e28 2264 726f  rnings.warn("dro
+000125e0: 706e 6120 6b77 6172 6720 6973 206e 6f74  pna kwarg is not
+000125f0: 2073 7570 706f 7274 6564 2066 6f72 2070   supported for p
+00012600: 616e 6461 7320 3c20 312e 312e 3022 290a  andas < 1.1.0").
+00012610: 2020 2020 2222 220a 0a20 2020 2023 2050      """..    # P
+00012620: 726f 6365 7373 206e 6f6e 2d73 7061 7469  rocess non-spati
+00012630: 616c 2063 6f6d 706f 6e65 6e74 0a20 2020  al component.   
+00012640: 2064 6174 6120 3d20 7064 2e44 6174 6146   data = pd.DataF
+00012650: 7261 6d65 2864 662e 6472 6f70 2863 6f6c  rame(df.drop(col
+00012660: 756d 6e73 3d64 662e 6765 6f6d 6574 7279  umns=df.geometry
+00012670: 2e6e 616d 6529 290a 0a20 2020 2069 6620  .name))..    if 
+00012680: 6167 6766 756e 6320 6973 206e 6f74 204e  aggfunc is not N
+00012690: 6f6e 6520 616e 6420 6973 696e 7374 616e  one and isinstan
+000126a0: 6365 2861 6767 6675 6e63 2c20 6469 6374  ce(aggfunc, dict
+000126b0: 2920 616e 6420 2274 6f5f 6a73 6f6e 2220  ) and "to_json" 
+000126c0: 696e 2061 6767 6675 6e63 3a0a 2020 2020  in aggfunc:.    
+000126d0: 2020 2020 6167 675f 636f 6c75 6d6e 7320      agg_columns 
+000126e0: 3d20 6c69 7374 2873 6574 2861 6767 6675  = list(set(aggfu
+000126f0: 6e63 5b22 746f 5f6a 736f 6e22 5d29 290a  nc["to_json"])).
+00012700: 2020 2020 2020 2020 6167 6772 6567 6174          aggregat
+00012710: 6564 5f64 6174 6120 3d20 280a 2020 2020  ed_data = (.    
+00012720: 2020 2020 2020 2020 6461 7461 2e67 726f          data.gro
+00012730: 7570 6279 282a 2a67 726f 7570 6279 5f6b  upby(**groupby_k
+00012740: 7761 7267 7329 0a20 2020 2020 2020 2020  wargs).         
+00012750: 2020 202e 6170 706c 7928 6c61 6d62 6461     .apply(lambda
+00012760: 2067 3a20 675b 6167 675f 636f 6c75 6d6e   g: g[agg_column
+00012770: 735d 2e74 6f5f 6a73 6f6e 286f 7269 656e  s].to_json(orien
+00012780: 743d 2272 6563 6f72 6473 2229 290a 2020  t="records")).  
+00012790: 2020 2020 2020 2020 2020 2e74 6f5f 6672            .to_fr
+000127a0: 616d 6528 6e61 6d65 3d22 5f5f 4449 5353  ame(name="__DISS
+000127b0: 4f4c 5645 5f54 4f4a 534f 4e22 290a 2020  OLVE_TOJSON").  
+000127c0: 2020 2020 2020 290a 2020 2020 656c 6966        ).    elif
+000127d0: 2069 7369 6e73 7461 6e63 6528 6167 6766   isinstance(aggf
+000127e0: 756e 632c 2073 7472 2920 616e 6420 6167  unc, str) and ag
+000127f0: 6766 756e 6320 3d3d 2022 6d65 7267 655f  gfunc == "merge_
+00012800: 6a73 6f6e 5f6c 6973 7473 223a 0a20 2020  json_lists":.   
+00012810: 2020 2020 2023 204d 6572 6765 2061 6e64       # Merge and
+00012820: 2066 6c61 7474 656e 2074 6865 206a 736f   flatten the jso
+00012830: 6e20 6c69 7374 7320 696e 2074 6865 2067  n lists in the g
+00012840: 726f 7570 730a 2020 2020 2020 2020 6465  roups.        de
+00012850: 6620 6772 6f75 705f 666c 6174 7465 6e5f  f group_flatten_
+00012860: 6a73 6f6e 5f6c 6973 7428 6729 3a0a 2020  json_list(g):.  
+00012870: 2020 2020 2020 2020 2020 2320 4576 616c            # Eval
+00012880: 7561 7465 2061 6c6c 2067 726f 7570 6564  uate all grouped
+00012890: 2072 6f77 7320 746f 206a 736f 6e20 6f62   rows to json ob
+000128a0: 6a65 6374 732e 2054 6869 7320 7265 7375  jects. This resu
+000128b0: 6c74 7320 696e 2061 206c 6973 7420 6f66  lts in a list of
+000128c0: 0a20 2020 2020 2020 2020 2020 2023 206c  .            # l
+000128d0: 6973 7473 206f 6620 6a73 6f6e 206f 626a  ists of json obj
+000128e0: 6563 7473 2e0a 2020 2020 2020 2020 2020  ects..          
+000128f0: 2020 6a73 6f6e 5f6e 6573 7465 645f 6c69    json_nested_li
+00012900: 7374 7320 3d20 5b0a 2020 2020 2020 2020  sts = [.        
+00012910: 2020 2020 2020 2020 6a73 6f6e 2e6c 6f61          json.loa
+00012920: 6473 286a 736f 6e5f 7661 6c75 6573 2920  ds(json_values) 
+00012930: 666f 7220 6a73 6f6e 5f76 616c 7565 7320  for json_values 
+00012940: 696e 2067 5b22 5f5f 4449 5353 4f4c 5645  in g["__DISSOLVE
+00012950: 5f54 4f4a 534f 4e22 5d0a 2020 2020 2020  _TOJSON"].      
+00012960: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
+00012970: 2020 2020 2023 2045 7874 7261 6374 2074       # Extract t
+00012980: 6865 2072 6f77 7320 6672 6f6d 2074 6865  he rows from the
+00012990: 206e 6573 7465 6420 6c69 7374 7320 2b20   nested lists + 
+000129a0: 7075 7420 696e 2061 2066 6c61 7420 6c69  put in a flat li
+000129b0: 7374 2061 7320 7374 7269 6e67 730a 2020  st as strings.  
+000129c0: 2020 2020 2020 2020 2020 6a73 6f6e 7374            jsonst
+000129d0: 725f 666c 6174 203d 205b 0a20 2020 2020  r_flat = [.     
+000129e0: 2020 2020 2020 2020 2020 206a 736f 6e2e             json.
+000129f0: 6475 6d70 7328 6a73 6f6e 5f76 616c 7565  dumps(json_value
+00012a00: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00012a10: 2020 666f 7220 6a73 6f6e 5f76 616c 7565    for json_value
+00012a20: 7320 696e 206a 736f 6e5f 6e65 7374 6564  s in json_nested
+00012a30: 5f6c 6973 7473 0a20 2020 2020 2020 2020  _lists.         
+00012a40: 2020 2020 2020 2066 6f72 206a 736f 6e5f         for json_
+00012a50: 7661 6c75 6520 696e 206a 736f 6e5f 7661  value in json_va
+00012a60: 6c75 6573 0a20 2020 2020 2020 2020 2020  lues.           
+00012a70: 205d 0a0a 2020 2020 2020 2020 2020 2020   ]..            
+00012a80: 2320 5265 6d6f 7665 2064 7570 6c69 6361  # Remove duplica
+00012a90: 7465 730a 2020 2020 2020 2020 2020 2020  tes.            
+00012aa0: 6a73 6f6e 7373 7472 5f64 6973 7469 6e63  jsonsstr_distinc
+00012ab0: 7420 3d20 7365 7428 6a73 6f6e 7374 725f  t = set(jsonstr_
+00012ac0: 666c 6174 290a 0a20 2020 2020 2020 2020  flat)..         
+00012ad0: 2020 2023 2043 6f6e 7665 7274 2074 6865     # Convert the
+00012ae0: 2064 6174 6120 6167 6169 6e20 746f 2061   data again to a
+00012af0: 206c 6973 7420 6f66 206a 736f 6e20 6f62   list of json ob
+00012b00: 6a65 6374 730a 2020 2020 2020 2020 2020  jects.          
+00012b10: 2020 6a73 6f6e 5f64 6973 7469 6e63 7420    json_distinct 
+00012b20: 3d20 5b6a 736f 6e2e 6c6f 6164 7328 6a73  = [json.loads(js
+00012b30: 6f6e 5f76 616c 7565 2920 666f 7220 6a73  on_value) for js
+00012b40: 6f6e 5f76 616c 7565 2069 6e20 6a73 6f6e  on_value in json
+00012b50: 7373 7472 5f64 6973 7469 6e63 745d 0a0a  sstr_distinct]..
+00012b60: 2020 2020 2020 2020 2020 2020 2320 5265              # Re
+00012b70: 7475 726e 2061 7320 6a73 6f6e 2073 7472  turn as json str
+00012b80: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00012b90: 7265 7475 726e 206a 736f 6e2e 6475 6d70  return json.dump
+00012ba0: 7328 6a73 6f6e 5f64 6973 7469 6e63 7429  s(json_distinct)
+00012bb0: 0a0a 2020 2020 2020 2020 6167 6772 6567  ..        aggreg
+00012bc0: 6174 6564 5f64 6174 6120 3d20 280a 2020  ated_data = (.  
+00012bd0: 2020 2020 2020 2020 2020 6461 7461 2e67            data.g
+00012be0: 726f 7570 6279 282a 2a67 726f 7570 6279  roupby(**groupby
+00012bf0: 5f6b 7761 7267 7329 0a20 2020 2020 2020  _kwargs).       
+00012c00: 2020 2020 202e 6170 706c 7928 6c61 6d62       .apply(lamb
+00012c10: 6461 2067 3a20 6772 6f75 705f 666c 6174  da g: group_flat
+00012c20: 7465 6e5f 6a73 6f6e 5f6c 6973 7428 6729  ten_json_list(g)
+00012c30: 290a 2020 2020 2020 2020 2020 2020 2e74  ).            .t
+00012c40: 6f5f 6672 616d 6528 6e61 6d65 3d22 5f5f  o_frame(name="__
+00012c50: 4449 5353 4f4c 5645 5f54 4f4a 534f 4e22  DISSOLVE_TOJSON"
+00012c60: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+00012c70: 656c 7365 3a0a 2020 2020 2020 2020 6167  else:.        ag
+00012c80: 6772 6567 6174 6564 5f64 6174 6120 3d20  gregated_data = 
+00012c90: 6461 7461 2e67 726f 7570 6279 282a 2a67  data.groupby(**g
+00012ca0: 726f 7570 6279 5f6b 7761 7267 7329 2e61  roupby_kwargs).a
+00012cb0: 6767 2861 6767 6675 6e63 290a 2020 2020  gg(aggfunc).    
+00012cc0: 2020 2020 2320 4368 6563 6b20 6966 2061      # Check if a
+00012cd0: 6c6c 2063 6f6c 756d 6e73 2077 6572 6520  ll columns were 
+00012ce0: 7072 6f70 6572 6c79 2061 6767 7265 6761  properly aggrega
+00012cf0: 7465 640a 2020 2020 2020 2020 6173 7365  ted.        asse
+00012d00: 7274 2062 795f 6c6f 6361 6c20 6973 206e  rt by_local is n
+00012d10: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+00012d20: 636f 6c75 6d6e 735f 746f 5f61 6767 203d  columns_to_agg =
+00012d30: 205b 636f 6c75 6d6e 2066 6f72 2063 6f6c   [column for col
+00012d40: 756d 6e20 696e 2064 6174 612e 636f 6c75  umn in data.colu
+00012d50: 6d6e 7320 6966 2063 6f6c 756d 6e20 6e6f  mns if column no
+00012d60: 7420 696e 2062 795f 6c6f 6361 6c5d 0a20  t in by_local]. 
+00012d70: 2020 2020 2020 2069 6620 6c65 6e28 636f         if len(co
+00012d80: 6c75 6d6e 735f 746f 5f61 6767 2920 213d  lumns_to_agg) !=
+00012d90: 206c 656e 2861 6767 7265 6761 7465 645f   len(aggregated_
+00012da0: 6461 7461 2e63 6f6c 756d 6e73 293a 0a20  data.columns):. 
+00012db0: 2020 2020 2020 2020 2020 2064 726f 7070             dropp
+00012dc0: 6564 5f63 6f6c 756d 6e73 203d 205b 0a20  ed_columns = [. 
+00012dd0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+00012de0: 6f6c 756d 6e0a 2020 2020 2020 2020 2020  olumn.          
+00012df0: 2020 2020 2020 666f 7220 636f 6c75 6d6e        for column
+00012e00: 2069 6e20 636f 6c75 6d6e 735f 746f 5f61   in columns_to_a
+00012e10: 6767 0a20 2020 2020 2020 2020 2020 2020  gg.             
+00012e20: 2020 2069 6620 636f 6c75 6d6e 206e 6f74     if column not
+00012e30: 2069 6e20 6167 6772 6567 6174 6564 5f64   in aggregated_d
+00012e40: 6174 612e 636f 6c75 6d6e 730a 2020 2020  ata.columns.    
+00012e50: 2020 2020 2020 2020 5d0a 2020 2020 2020          ].      
+00012e60: 2020 2020 2020 7261 6973 6520 4578 6365        raise Exce
+00012e70: 7074 696f 6e28 0a20 2020 2020 2020 2020  ption(.         
+00012e80: 2020 2020 2020 2066 2243 6f6c 756d 6e28         f"Column(
+00012e90: 7329 207b 6472 6f70 7065 645f 636f 6c75  s) {dropped_colu
+00012ea0: 6d6e 737d 2061 7265 206e 6f74 2073 7570  mns} are not sup
+00012eb0: 706f 7274 6564 2066 6f72 2061 6767 7265  ported for aggre
+00012ec0: 6761 7469 6f6e 2c20 7374 6f70 220a 2020  gation, stop".  
+00012ed0: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00012ee0: 2023 2050 726f 6365 7373 2073 7061 7469   # Process spati
+00012ef0: 616c 2063 6f6d 706f 6e65 6e74 0a20 2020  al component.   
+00012f00: 2064 6566 206d 6572 6765 5f67 656f 6d65   def merge_geome
+00012f10: 7472 6965 7328 626c 6f63 6b29 3a0a 2020  tries(block):.  
+00012f20: 2020 2020 2020 6d65 7267 6564 5f67 656f        merged_geo
+00012f30: 6d20 3d20 626c 6f63 6b2e 756e 6172 795f  m = block.unary_
+00012f40: 756e 696f 6e0a 2020 2020 2020 2020 7265  union.        re
+00012f50: 7475 726e 206d 6572 6765 645f 6765 6f6d  turn merged_geom
+00012f60: 0a0a 2020 2020 6720 3d20 6466 2e67 726f  ..    g = df.gro
+00012f70: 7570 6279 2867 726f 7570 5f6b 6579 733d  upby(group_keys=
+00012f80: 4661 6c73 652c 202a 2a67 726f 7570 6279  False, **groupby
+00012f90: 5f6b 7761 7267 7329 5b64 662e 6765 6f6d  _kwargs)[df.geom
+00012fa0: 6574 7279 2e6e 616d 655d 2e61 6767 280a  etry.name].agg(.
+00012fb0: 2020 2020 2020 2020 6d65 7267 655f 6765          merge_ge
+00012fc0: 6f6d 6574 7269 6573 0a20 2020 2029 0a0a  ometries.    )..
+00012fd0: 2020 2020 2320 4167 6772 6567 6174 650a      # Aggregate.
+00012fe0: 2020 2020 6167 6772 6567 6174 6564 5f67      aggregated_g
+00012ff0: 656f 6d65 7472 7920 3d20 6770 642e 4765  eometry = gpd.Ge
+00013000: 6f44 6174 6146 7261 6d65 280a 2020 2020  oDataFrame(.    
+00013010: 2020 2020 6461 7461 3d67 2c20 6765 6f6d      data=g, geom
+00013020: 6574 7279 3d64 662e 6765 6f6d 6574 7279  etry=df.geometry
+00013030: 2e6e 616d 652c 2063 7273 3d64 662e 6372  .name, crs=df.cr
+00013040: 730a 2020 2020 290a 2020 2020 2320 5265  s.    ).    # Re
+00013050: 636f 6d62 696e 650a 2020 2020 6167 6772  combine.    aggr
+00013060: 6567 6174 6564 203d 2061 6767 7265 6761  egated = aggrega
+00013070: 7465 645f 6765 6f6d 6574 7279 2e6a 6f69  ted_geometry.joi
+00013080: 6e28 6167 6772 6567 6174 6564 5f64 6174  n(aggregated_dat
+00013090: 6129 0a0a 2020 2020 2320 5265 7365 7420  a)..    # Reset 
+000130a0: 6966 2072 6571 7565 7374 6564 0a20 2020  if requested.   
+000130b0: 2069 6620 6e6f 7420 6173 5f69 6e64 6578   if not as_index
+000130c0: 3a0a 2020 2020 2020 2020 6167 6772 6567  :.        aggreg
+000130d0: 6174 6564 203d 2061 6767 7265 6761 7465  ated = aggregate
+000130e0: 642e 7265 7365 745f 696e 6465 7828 290a  d.reset_index().
+000130f0: 0a20 2020 2023 204d 616b 6520 7375 7265  .    # Make sure
+00013100: 206f 7574 7075 7420 7479 7065 7320 6f66   output types of
+00013110: 2067 726f 7570 6564 2063 6f6c 756d 6e73   grouped columns
+00013120: 2061 7265 2074 6865 2073 616d 6520 6173   are the same as
+00013130: 2069 6e70 7574 2074 7970 6573 2e0a 2020   input types..  
+00013140: 2020 2320 452e 672e 206f 626a 6563 7420    # E.g. object 
+00013150: 636f 6c75 6d6e 7320 6265 636f 6d65 2066  columns become f
+00013160: 6c6f 6174 2069 6620 616c 6c20 7661 6c75  loat if all valu
+00013170: 6573 2061 7265 204e 6f6e 652e 0a20 2020  es are None..   
+00013180: 2069 6620 6279 2069 7320 6e6f 7420 4e6f   if by is not No
+00013190: 6e65 3a0a 2020 2020 2020 2020 6966 2069  ne:.        if i
+000131a0: 7369 6e73 7461 6e63 6528 6279 2c20 7374  sinstance(by, st
+000131b0: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
+000131c0: 6966 2062 7920 696e 2061 6767 7265 6761  if by in aggrega
+000131d0: 7465 642e 636f 6c75 6d6e 7320 616e 6420  ted.columns and 
+000131e0: 6466 5b62 795d 2e64 7479 7065 2021 3d20  df[by].dtype != 
+000131f0: 6167 6772 6567 6174 6564 5b62 795d 2e64  aggregated[by].d
+00013200: 7479 7065 3a0a 2020 2020 2020 2020 2020  type:.          
+00013210: 2020 2020 2020 6167 6772 6567 6174 6564        aggregated
+00013220: 5b62 795d 203d 2061 6767 7265 6761 7465  [by] = aggregate
+00013230: 645b 6279 5d2e 6173 7479 7065 2864 665b  d[by].astype(df[
+00013240: 6279 5d2e 6474 7970 6529 0a20 2020 2020  by].dtype).     
+00013250: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
+00013260: 6365 2862 792c 2049 7465 7261 626c 6529  ce(by, Iterable)
+00013270: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
+00013280: 7220 636f 6c20 696e 2062 793a 0a20 2020  r col in by:.   
+00013290: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+000132a0: 636f 6c20 696e 2061 6767 7265 6761 7465  col in aggregate
+000132b0: 642e 636f 6c75 6d6e 7320 616e 6420 6466  d.columns and df
+000132c0: 5b63 6f6c 5d2e 6474 7970 6520 213d 2061  [col].dtype != a
+000132d0: 6767 7265 6761 7465 645b 636f 6c5d 2e64  ggregated[col].d
+000132e0: 7479 7065 3a0a 2020 2020 2020 2020 2020  type:.          
+000132f0: 2020 2020 2020 2020 2020 6167 6772 6567            aggreg
+00013300: 6174 6564 5b63 6f6c 5d20 3d20 6167 6772  ated[col] = aggr
+00013310: 6567 6174 6564 5b63 6f6c 5d2e 6173 7479  egated[col].asty
+00013320: 7065 2864 665b 636f 6c5d 2e64 7479 7065  pe(df[col].dtype
+00013330: 290a 0a20 2020 2061 7373 6572 7420 6973  )..    assert is
+00013340: 696e 7374 616e 6365 2861 6767 7265 6761  instance(aggrega
+00013350: 7465 642c 2067 7064 2e47 656f 4461 7461  ted, gpd.GeoData
+00013360: 4672 616d 6529 0a20 2020 2072 6574 7572  Frame).    retur
+00013370: 6e20 6167 6772 6567 6174 6564 0a0a 0a64  n aggregated...d
+00013380: 6566 205f 6164 645f 6f72 6465 7262 795f  ef _add_orderby_
+00013390: 636f 6c75 6d6e 2870 6174 683a 2050 6174  column(path: Pat
+000133a0: 682c 206c 6179 6572 3a20 7374 722c 206e  h, layer: str, n
+000133b0: 616d 653a 2073 7472 293a 0a20 2020 2023  ame: str):.    #
+000133c0: 2050 7265 7061 7265 2074 6865 2065 7870   Prepare the exp
+000133d0: 7265 7373 696f 6e20 746f 2063 616c 6375  ression to calcu
+000133e0: 6c61 7465 2074 6865 206f 7264 6572 6279  late the orderby
+000133f0: 2063 6f6c 756d 6e2e 0a20 2020 2023 2049   column..    # I
+00013400: 6e20 6120 7370 6174 6961 6c20 6669 6c65  n a spatial file
+00013410: 2c20 6120 7370 6174 6961 6c20 6f72 6465  , a spatial orde
+00013420: 7220 7769 6c6c 206d 616b 6520 6c61 7465  r will make late
+00013430: 7220 7573 6520 6d6f 7265 2065 6666 6963  r use more effic
+00013440: 69c3 ab6e 742c 0a20 2020 2023 2073 6f20  i..nt,.    # so 
+00013450: 7573 6520 6120 6765 6f68 6173 682e 0a20  use a geohash.. 
+00013460: 2020 206c 6179 6572 696e 666f 203d 2067     layerinfo = g
+00013470: 666f 2e67 6574 5f6c 6179 6572 696e 666f  fo.get_layerinfo
+00013480: 2870 6174 6829 0a20 2020 2069 6620 6c61  (path).    if la
+00013490: 7965 7269 6e66 6f2e 6372 7320 6973 206e  yerinfo.crs is n
+000134a0: 6f74 204e 6f6e 6520 616e 6420 6c61 7965  ot None and laye
+000134b0: 7269 6e66 6f2e 6372 732e 6973 5f67 656f  rinfo.crs.is_geo
+000134c0: 6772 6170 6869 633a 0a20 2020 2020 2020  graphic:.       
+000134d0: 2023 2049 6620 7468 6520 636f 6f72 6469   # If the coordi
+000134e0: 6e61 7465 7320 6172 6520 6765 6f67 7261  nates are geogra
+000134f0: 7068 6963 2028 696e 206c 6174 2f6c 6f6e  phic (in lat/lon
+00013500: 2064 6567 7265 6573 292c 206f 6b0a 2020   degrees), ok.  
+00013510: 2020 2020 2020 6578 7072 6573 7369 6f6e        expression
+00013520: 203d 2066 2253 545f 4765 6f48 6173 6828   = f"ST_GeoHash(
+00013530: 7b6c 6179 6572 696e 666f 2e67 656f 6d65  {layerinfo.geome
+00013540: 7472 7963 6f6c 756d 6e7d 2c20 3130 2922  trycolumn}, 10)"
+00013550: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00013560: 2020 2023 2049 6620 7468 6579 2061 7265     # If they are
+00013570: 206e 6f74 2067 656f 6772 6170 6869 6320   not geographic 
+00013580: 2869 6e20 6c61 742f 6c6f 6e20 6465 6772  (in lat/lon degr
+00013590: 6565 7329 2c20 7468 6579 206e 6565 6420  ees), they need 
+000135a0: 746f 2062 650a 2020 2020 2020 2020 2320  to be.        # 
+000135b0: 636f 6e76 6572 7465 6420 746f 207e 2064  converted to ~ d
+000135c0: 6567 7265 6573 2074 6f20 6265 2061 626c  egrees to be abl
+000135d0: 6520 746f 2063 616c 6375 6c61 7465 2061  e to calculate a
+000135e0: 2067 656f 6861 7368 2e0a 0a20 2020 2020   geohash...     
+000135f0: 2020 2023 2050 726f 7065 726c 7920 6361     # Properly ca
+00013600: 6c63 756c 6174 696e 6720 7468 6520 7472  lculating the tr
+00013610: 616e 7366 6f72 6d61 7469 6f6e 2074 6f20  ansformation to 
+00013620: 6567 2e20 5747 5320 6973 2074 6572 7269  eg. WGS is terri
+00013630: 626c 7920 736c 6f77 2e2e 2e0a 2020 2020  bly slow....    
+00013640: 2020 2020 2320 6578 7072 6573 7369 6f6e      # expression
+00013650: 203d 2066 2222 2253 545f 4765 6f48 6173   = f"""ST_GeoHas
+00013660: 6828 5354 5f54 7261 6e73 666f 726d 284d  h(ST_Transform(M
+00013670: 616b 6550 6f69 6e74 280a 2020 2020 2020  akePoint(.      
+00013680: 2020 2320 2020 2020 2020 284d 6272 4d61    #       (MbrMa
+00013690: 7858 2867 656f 6d29 2b4d 6272 4d69 6e58  xX(geom)+MbrMinX
+000136a0: 2867 656f 6d29 292f 322c 0a20 2020 2020  (geom))/2,.     
+000136b0: 2020 2023 2020 2020 2020 2028 4d62 724d     #       (MbrM
+000136c0: 696e 5928 6765 6f6d 292b 4d62 724d 6178  inY(geom)+MbrMax
+000136d0: 5928 6765 6f6d 2929 2f32 2c20 5354 5f53  Y(geom))/2, ST_S
+000136e0: 5249 4428 6765 6f6d 2929 2c20 3433 3236  RID(geom)), 4326
+000136f0: 292c 2031 3029 2222 220a 2020 2020 2020  ), 10)""".      
+00013700: 2020 2320 536f 2c20 646f 2073 6f6d 6574    # So, do somet
+00013710: 6869 6e67 2065 6c73 6520 7468 6174 2773  hing else that's
+00013720: 2066 6173 7465 7220 616e 6420 7374 696c   faster and stil
+00013730: 6c20 6769 7665 7320 6120 676f 6f64 0a20  l gives a good. 
+00013740: 2020 2020 2020 2023 2067 656f 6772 6170         # geograp
+00013750: 6869 6320 636c 7573 7465 7269 6e67 2e0a  hic clustering..
+00013760: 2020 2020 2020 2020 746f 5f67 656f 6772          to_geogr
+00013770: 6170 6869 635f 6661 6374 6f72 5f61 7070  aphic_factor_app
+00013780: 726f 7820 3d20 3930 202f 206d 6178 286c  rox = 90 / max(l
+00013790: 6179 6572 696e 666f 2e74 6f74 616c 5f62  ayerinfo.total_b
+000137a0: 6f75 6e64 7329 0a20 2020 2020 2020 2065  ounds).        e
+000137b0: 7870 7265 7373 696f 6e20 3d20 6622 2222  xpression = f"""
+000137c0: 5354 5f47 656f 4861 7368 284d 616b 6550  ST_GeoHash(MakeP
+000137d0: 6f69 6e74 280a 2020 2020 2020 2020 2020  oint(.          
+000137e0: 2020 2020 2020 2828 4d62 724d 6178 5828        ((MbrMaxX(
+000137f0: 7b6c 6179 6572 696e 666f 2e67 656f 6d65  {layerinfo.geome
+00013800: 7472 7963 6f6c 756d 6e7d 290a 2020 2020  trycolumn}).    
+00013810: 2020 2020 2020 2020 2020 2020 2020 2b4d                +M
+00013820: 6272 4d69 6e58 287b 6c61 7965 7269 6e66  brMinX({layerinf
+00013830: 6f2e 6765 6f6d 6574 7279 636f 6c75 6d6e  o.geometrycolumn
+00013840: 7d29 292f 320a 2020 2020 2020 2020 2020  }))/2.          
+00013850: 2020 2020 2020 292a 7b74 6f5f 6765 6f67        )*{to_geog
+00013860: 7261 7068 6963 5f66 6163 746f 725f 6170  raphic_factor_ap
+00013870: 7072 6f78 7d2c 0a20 2020 2020 2020 2020  prox},.         
+00013880: 2020 2020 2020 2028 284d 6272 4d69 6e59         ((MbrMinY
+00013890: 287b 6c61 7965 7269 6e66 6f2e 6765 6f6d  ({layerinfo.geom
+000138a0: 6574 7279 636f 6c75 6d6e 7d29 0a20 2020  etrycolumn}).   
+000138b0: 2020 2020 2020 2020 2020 2020 2020 202b                 +
+000138c0: 4d62 724d 6178 5928 7b6c 6179 6572 696e  MbrMaxY({layerin
+000138d0: 666f 2e67 656f 6d65 7472 7963 6f6c 756d  fo.geometrycolum
+000138e0: 6e7d 2929 2f32 0a20 2020 2020 2020 2020  n}))/2.         
+000138f0: 2020 2020 2020 2029 2a7b 746f 5f67 656f         )*{to_geo
+00013900: 6772 6170 6869 635f 6661 6374 6f72 5f61  graphic_factor_a
+00013910: 7070 726f 787d 2c20 3433 3236 292c 2031  pprox}, 4326), 1
+00013920: 3029 2222 220a 0a20 2020 2023 204e 6f77  0)"""..    # Now
+00013930: 2077 6520 6361 6e20 6163 7475 616c 6c79   we can actually
+00013940: 2061 6464 2074 6865 2063 6f6c 756d 6e2e   add the column.
+00013950: 0a20 2020 2067 666f 2e61 6464 5f63 6f6c  .    gfo.add_col
+00013960: 756d 6e28 7061 7468 3d70 6174 682c 206e  umn(path=path, n
+00013970: 616d 653d 6e61 6d65 2c20 7479 7065 3d67  ame=name, type=g
+00013980: 666f 2e44 6174 6154 7970 652e 5445 5854  fo.DataType.TEXT
+00013990: 2c20 6578 7072 6573 7369 6f6e 3d65 7870  , expression=exp
+000139a0: 7265 7373 696f 6e29 0a20 2020 2073 716c  ression).    sql
+000139b0: 6974 655f 7374 6d74 203d 2066 2743 5245  ite_stmt = f'CRE
+000139c0: 4154 4520 494e 4445 5820 7b6e 616d 657d  ATE INDEX {name}
+000139d0: 5f69 6478 204f 4e20 227b 6c61 7965 727d  _idx ON "{layer}
+000139e0: 2228 7b6e 616d 657d 2927 0a20 2020 2067  "({name})'.    g
+000139f0: 666f 2e65 7865 6375 7465 5f73 716c 2870  fo.execute_sql(p
+00013a00: 6174 683d 7061 7468 2c20 7371 6c5f 7374  ath=path, sql_st
+00013a10: 6d74 3d73 716c 6974 655f 7374 6d74 290a  mt=sqlite_stmt).
```

### Comparing `geofileops-0.8.0a7/geofileops/util/_geoops_ogr.py` & `geofileops-0.8.0a8/geofileops/util/_geoops_ogr.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/util/_geoops_sql.py` & `geofileops-0.8.0a8/geofileops/util/_geoops_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # -*- coding: utf-8 -*-
 """
 Module containing the implementation of Geofile operations using a sql statement.
 """
 
 from concurrent import futures
 from datetime import datetime
+import json
 import logging
 import logging.config
 import math
 import multiprocessing
 from pathlib import Path
 import shutil
 import string
-from typing import Iterable, List, Literal, Optional, Union
+from typing import Dict, Iterable, List, Literal, Optional, Union
 import warnings
 
 import pandas as pd
 
 import geofileops as gfo
 from geofileops import GeofileType, GeometryType, PrimitiveType
 from geofileops import fileops
 from geofileops.fileops import _append_to_nolock
-from . import _general_util
-from . import _io_util
-from . import _ogr_sql_util
-from . import _ogr_util
+from geofileops.util import _general_util
+from geofileops.util import _io_util
+from geofileops.util import _ogr_sql_util
+from geofileops.util import _ogr_util
 from geofileops.helpers import _parameter_helper
-from . import _processing_util
-from . import _sqlite_util
+from geofileops.util import _processing_util
+from geofileops.util import _sqlite_util
 
 ################################################################################
 # Some init
 ################################################################################
 
 logger = logging.getLogger(__name__)
 
@@ -595,18 +596,18 @@
                 columns_to_select_str=column_formatter.prefixed_aliased(),
                 input_layer=processing_params.input1_layer,
                 batch_filter="",
             )
             cols = _sqlite_util.get_columns(
                 sql_stmt=sql_tmp, input1_path=processing_params.input1_path
             )
-            cols = [
+            attributes = [
                 col for col in cols if col.lower() != input_layerinfo.geometrycolumn
             ]
-            columns_to_select = _ogr_sql_util.columns_quoted(cols)
+            columns_to_select = _ogr_sql_util.columns_quoted(attributes)
             sql_template = f"""
                 SELECT {gridsize_op} AS {{geometrycolumn}}
                       {columns_to_select}
                   FROM ( {sql_template}
                     ) sub_gridsize
             """
 
@@ -658,15 +659,15 @@
         # Processing in threads is 2x faster for small datasets (on Windows)
         calculate_in_threads = True if input_layerinfo.featurecount <= 100 else False
         with _processing_util.PooledExecutorFactory(
             threadpool=calculate_in_threads,
             max_workers=processing_params.nb_parallel,
             initializer=_processing_util.initialize_worker(),
         ) as calculate_pool:
-            batches = {}
+            batches: Dict[int, dict] = {}
             future_to_batch_id = {}
             for batch_id in processing_params.batches:
                 batches[batch_id] = {}
                 batches[batch_id]["layer"] = output_layer
 
                 tmp_partial_output_path = (
                     tempdir / f"{output_path.stem}_{batch_id}.gpkg"
@@ -922,74 +923,79 @@
     nb_parallel: int = -1,
     batchsize: int = -1,
     force: bool = False,
     input_columns_prefix: str = "",
     output_with_spatial_index: bool = True,
 ):
     # Init
-    # In the query, important to only extract the geometry types that are expected
     input_layer_info = gfo.get_layerinfo(input_path, input_layer)
-    primitivetypeid = input_layer_info.geometrytype.to_primitivetype.value
 
     # If the input type is not point, force the output type to multi,
     # because erase can cause eg. polygons to be split to multipolygons...
     force_output_geometrytype = input_layer_info.geometrytype
     if force_output_geometrytype is not GeometryType.POINT:
         force_output_geometrytype = input_layer_info.geometrytype.to_multitype
 
     # Prepare sql template for this operation
-    # Remarks:
-    #   - ST_difference(geometry , NULL) gives NULL as result! -> hence the CASE
-    #   - use of the with instead of an inline view is a lot faster
-    #   - WHERE geom IS NOT NULL to evade rows with a NULL geom, they give issues in
-    #     later operations
+    # - WHERE geom IS NOT NULL to avoid rows with a NULL geom, they give issues in
+    #   later operations
+    # - use "LIMIT -1 OFFSET 0" to avoid the subquery flattening. Flattening e.g.
+    #   "geom IS NOT NULL" leads to ST_Difference_Collection calculated double!
+    # - ST_Intersects and ST_Touches slow down a lot when the data contains huge geoms
+    # - Calculate difference in correlated subquery in SELECT clause
+    # - Using a WITH with a GROUP BY on layer1.rowid was a few % faster, but this
+    #   processed the entire batch in memory so used > 10 * more memory. E.g. for one
+    #   test file 4-7 GB per process versus 70-700 MB). For another: crash.
+    # - Check if the result of ST_Difference_Collection is empty (NULL) using IFNULL,
+    #   and if this ois the case set to 'DIFF_EMPTY'. This way we can make the
+    #   distinction whether the subquery is finding a row (no match with spatial index)
+    #   or if the difference results in an empty/NULL geometry.
+    #   Tried to return EMPTY GEOMETRY from ST_Difference_Collection, but it didn't
+    #   work to use spatialite's ST_IsEmpty(geom) = 0 to filter on this for an unclear
+    #   reason.
+    # - Not relevant anymore, but ST_difference(geometry , NULL) gives NULL as result
     input1_layer_rtree = "rtree_{input1_layer}_{input1_geometrycolumn}"
     input2_layer_rtree = "rtree_{input2_layer}_{input2_geometrycolumn}"
+
     sql_template = f"""
-        SELECT * FROM
-          ( WITH layer2_unioned AS (
-              SELECT layer1.rowid AS layer1_rowid
-                    ,ST_union(layer2.{{input2_geometrycolumn}}) AS geom
-                FROM {{input1_databasename}}."{{input1_layer}}" layer1
-                JOIN {{input1_databasename}}."{input1_layer_rtree}" layer1tree
-                  ON layer1.fid = layer1tree.id
-                JOIN {{input2_databasename}}."{{input2_layer}}" layer2
-                JOIN {{input2_databasename}}."{input2_layer_rtree}" layer2tree
-                  ON layer2.fid = layer2tree.id
-               WHERE 1=1
-                 {{batch_filter}}
-                 AND layer1tree.minx <= layer2tree.maxx
-                 AND layer1tree.maxx >= layer2tree.minx
-                 AND layer1tree.miny <= layer2tree.maxy
-                 AND layer1tree.maxy >= layer2tree.miny
-                 AND ST_Intersects(
-                        layer1.{{input1_geometrycolumn}},
-                        layer2.{{input2_geometrycolumn}}) = 1
-                 AND ST_Touches(
-                        layer1.{{input1_geometrycolumn}},
-                        layer2.{{input2_geometrycolumn}}) = 0
-               GROUP BY layer1.rowid
-            )
-            SELECT CASE WHEN layer2_unioned.geom IS NULL
-                        THEN layer1.{{input1_geometrycolumn}}
-                        ELSE ST_CollectionExtract(
-                                ST_difference(
-                                    layer1.{{input1_geometrycolumn}},
-                                    layer2_unioned.geom),
-                                    {primitivetypeid})
-                   END as geom
-                  {{layer1_columns_prefix_alias_str}}
-              FROM {{input1_databasename}}."{{input1_layer}}" layer1
-              LEFT JOIN layer2_unioned ON layer1.rowid = layer2_unioned.layer1_rowid
-             WHERE 1=1
-               {{batch_filter}}
+        SELECT * FROM (
+          SELECT IFNULL(
+                   ( SELECT IFNULL(
+                                ST_GeomFromWKB(ST_Difference_Collection(
+                                    ST_AsBinary(layer1_sub.{{input1_geometrycolumn}}),
+                                    ST_AsBinary(ST_Collect(
+                                        layer2_sub.{{input2_geometrycolumn}})),
+                                    1)),
+                                'DIFF_EMPTY'
+                            ) AS diff_geom
+                       FROM {{input1_databasename}}."{{input1_layer}}" layer1_sub
+                       JOIN {{input1_databasename}}."{input1_layer_rtree}" layer1tree
+                         ON layer1_sub.fid = layer1tree.id
+                       JOIN {{input2_databasename}}."{{input2_layer}}" layer2_sub
+                       JOIN {{input2_databasename}}."{input2_layer_rtree}" layer2tree
+                         ON layer2_sub.fid = layer2tree.id
+                      WHERE 1=1
+                        AND layer1_sub.rowid = layer1.rowid
+                        AND layer1tree.minx <= layer2tree.maxx
+                        AND layer1tree.maxx >= layer2tree.minx
+                        AND layer1tree.miny <= layer2tree.maxy
+                        AND layer1tree.maxy >= layer2tree.miny
+                      GROUP BY layer1_sub.rowid
+                      LIMIT -1 OFFSET 0
+                   ),
+                   layer1.{{input1_geometrycolumn}}
+                 ) AS geom
+                {{layer1_columns_prefix_alias_str}}
+            FROM {{input1_databasename}}."{{input1_layer}}" layer1
+           WHERE 1=1
+             {{batch_filter}}
+           LIMIT -1 OFFSET 0
           )
          WHERE geom IS NOT NULL
-           AND ST_NPoints(geom) > 0
-           -- ST_CollectionExtract outputs empty, but not NULL geoms in spatialite 4.3
+           AND geom <> 'DIFF_EMPTY'
     """
 
     # Go!
     return _two_layer_vector_operation(
         input1_path=input_path,
         input2_path=erase_path,
         output_path=output_path,
@@ -1671,44 +1677,36 @@
     input1_layer_info = gfo.get_layerinfo(input1_path, input1_layer)
     primitivetype_to_extract = input1_layer_info.geometrytype.to_primitivetype
 
     # For the output file, force MULTI variant to evade ugly warnings
     force_output_geometrytype = primitivetype_to_extract.to_multitype
 
     # Prepare sql template for this operation
-    # Remarks:
-    #   - ST_difference(geometry , NULL) gives NULL as result! -> hence the CASE
-    #   - the group by layer1.rowid should be directly in the subquery. If it is
-    #     applied on an (other) with it is slow.
-    #   - a left join is a lot faster and memory efficient than a NOT IN or NOT EXISTS.
+    # - WHERE geom IS NOT NULL to avoid rows with a NULL geom, they give issues in
+    #   later operations
+    # - use "LIMIT -1 OFFSET 0" to avoid the subquery flattening. Flattening e.g.
+    #   "geom IS NOT NULL" leads to ST_Difference_Collection calculated double!
+    # - ST_Intersects and ST_Touches slow down a lot when the data contains huge geoms
+    # - Calculate difference in correlated subquery in SELECT clause
+    # - Using a WITH with a GROUP BY on layer1.rowid was a few % faster, but this
+    #   processed the entire batch in memory so used > 10 * more memory. E.g. for one
+    #   test file 4-7 GB per process versus 70-700 MB). For another: crash.
+    # - Check if the result of ST_Difference_Collection is empty (NULL) using IFNULL,
+    #   and if this ois the case set to 'DIFF_EMPTY'. This way we can make the
+    #   distinction whether the subquery is finding a row (no match with spatial index)
+    #   or if the difference results in an empty/NULL geometry.
+    #   Tried to return EMPTY GEOMETRY from ST_Difference_Collection, but it didn't
+    #   work to use spatialite's ST_IsEmpty(geom) = 0 to filter on this for an unclear
+    #   reason.
+    # - Not relevant anymore, but ST_difference(geometry , NULL) gives NULL as result
     input1_layer_rtree = "rtree_{input1_layer}_{input1_geometrycolumn}"
     input2_layer_rtree = "rtree_{input2_layer}_{input2_geometrycolumn}"
+
     sql_template = f"""
-        SELECT * FROM
-          ( WITH layer2_unioned AS (
-              SELECT layer1.rowid AS layer1_rowid
-                    ,ST_union(layer2.{{input2_geometrycolumn}}) AS geom
-                FROM {{input1_databasename}}."{{input1_layer}}" layer1
-                JOIN {{input1_databasename}}."{input1_layer_rtree}" layer1tree
-                  ON layer1.fid = layer1tree.id
-                JOIN {{input2_databasename}}."{{input2_layer}}" layer2
-                JOIN {{input2_databasename}}."{input2_layer_rtree}" layer2tree
-                  ON layer2.fid = layer2tree.id
-               WHERE 1=1
-                 {{batch_filter}}
-                 AND layer1tree.minx <= layer2tree.maxx
-                 AND layer1tree.maxx >= layer2tree.minx
-                 AND layer1tree.miny <= layer2tree.maxy
-                 AND layer1tree.maxy >= layer2tree.miny
-                 AND ST_Intersects(layer1.{{input1_geometrycolumn}},
-                                   layer2.{{input2_geometrycolumn}}) = 1
-                 AND ST_Touches(layer1.{{input1_geometrycolumn}},
-                                layer2.{{input2_geometrycolumn}}) = 0
-               GROUP BY layer1.rowid
-            )
+        SELECT * FROM (
             SELECT ST_CollectionExtract(
                         ST_intersection(layer1.{{input1_geometrycolumn}},
                                         layer2.{{input2_geometrycolumn}}),
                         {primitivetype_to_extract.value}) as geom
                   {{layer1_columns_prefix_alias_str}}
                   {{layer2_columns_prefix_alias_str}}
               FROM {{input1_databasename}}."{{input1_layer}}" layer1
@@ -1721,33 +1719,52 @@
                {{batch_filter}}
                AND layer1tree.minx <= layer2tree.maxx
                AND layer1tree.maxx >= layer2tree.minx
                AND layer1tree.miny <= layer2tree.maxy
                AND layer1tree.maxy >= layer2tree.miny
                AND ST_Intersects(layer1.{{input1_geometrycolumn}},
                                  layer2.{{input2_geometrycolumn}}) = 1
-               AND ST_Touches(layer1.{{input1_geometrycolumn}},
-                              layer2.{{input2_geometrycolumn}}) = 0
+               --AND ST_Touches(layer1.{{input1_geometrycolumn}},
+               --               layer2.{{input2_geometrycolumn}}) = 0
             UNION ALL
-            SELECT CASE WHEN layer2_unioned.geom IS NULL
-                        THEN layer1.{{input1_geometrycolumn}}
-                        ELSE ST_CollectionExtract(
-                                ST_difference(layer1.{{input1_geometrycolumn}},
-                                              layer2_unioned.geom),
-                                {primitivetype_to_extract.value})
-                   END as geom
+            SELECT IFNULL(
+                     ( SELECT IFNULL(
+                                  ST_GeomFromWKB(ST_Difference_Collection(
+                                      ST_AsBinary(layer1_sub.{{input1_geometrycolumn}}),
+                                      ST_AsBinary(ST_Collect(
+                                          layer2_sub.{{input2_geometrycolumn}})),
+                                      1)),
+                                  'DIFF_EMPTY'
+                              ) AS diff_geom
+                         FROM {{input1_databasename}}."{{input1_layer}}" layer1_sub
+                         JOIN {{input1_databasename}}."{input1_layer_rtree}" layer1tree
+                           ON layer1_sub.fid = layer1tree.id
+                         JOIN {{input2_databasename}}."{{input2_layer}}" layer2_sub
+                         JOIN {{input2_databasename}}."{input2_layer_rtree}" layer2tree
+                           ON layer2_sub.fid = layer2tree.id
+                        WHERE 1=1
+                          AND layer1_sub.rowid = layer1.rowid
+                          AND layer1tree.minx <= layer2tree.maxx
+                          AND layer1tree.maxx >= layer2tree.minx
+                          AND layer1tree.miny <= layer2tree.maxy
+                          AND layer1tree.maxy >= layer2tree.miny
+                        GROUP BY layer1_sub.rowid
+                        LIMIT -1 OFFSET 0
+                     ),
+                     layer1.{{input1_geometrycolumn}}
+                   ) AS geom
                   {{layer1_columns_prefix_alias_str}}
                   {{layer2_columns_prefix_alias_null_str}}
               FROM {{input1_databasename}}."{{input1_layer}}" layer1
-              LEFT JOIN layer2_unioned ON layer1.rowid = layer2_unioned.layer1_rowid
              WHERE 1=1
                {{batch_filter}}
-           )
+             LIMIT -1 OFFSET 0
+            )
          WHERE geom IS NOT NULL
-           AND ST_NPoints(geom) > 0
+           AND geom <> 'DIFF_EMPTY'
     """
 
     # Go!
     return _two_layer_vector_operation(
         input1_path=input1_path,
         input2_path=input2_path,
         output_path=output_path,
@@ -2057,15 +2074,15 @@
         raise ValueError(f"{operation_name}: input2_path doesn't exist: {input2_path}")
     if input1_path == output_path or input2_path == output_path:
         raise ValueError(
             f"{operation_name}: output_path must not equal one of input paths"
         )
     if use_ogr is True and input1_path != input2_path:
         raise ValueError(
-            f"{operation_name}: if use_ogr True, input1_path == input2_path!"
+            f"{operation_name}: if use_ogr True, input1_path should equal input2_path!"
         )
     if output_path.exists():
         if force is False:
             logger.info(f"Stop {operation_name}: output exists already {output_path}")
             return
         else:
             gfo.remove(output_path)
@@ -2175,14 +2192,28 @@
             layer2_columns_prefix_alias_null_str=input2_col_strs.null_aliased(),
             input2_layer=processing_params.input2_layer,
             input2_tmp_layer=processing_params.input2_layer,
             input2_geometrycolumn=input2_tmp_layerinfo.geometrycolumn,
             batch_filter="{batch_filter}",
         )
 
+        # Determine column names and types based on sql statement
+        column_datatypes = None
+        # Use first batch_filter to improve performance
+        sql_stmt = sql_template.format(
+            input1_databasename="{input1_databasename}",
+            input2_databasename="{input2_databasename}",
+            batch_filter=processing_params.batches[0]["batch_filter"],
+        )
+        column_datatypes = _sqlite_util.get_columns(
+            sql_stmt=sql_stmt,
+            input1_path=processing_params.input1_path,
+            input2_path=processing_params.input2_path,
+        )
+
         # Add snaptogrid around sql_template if gridsize specified
         if gridsize != 0.0:
             # Apply snaptogrid, but this results in invalid geometries, so also
             # ST_Makevalid. It can also result in collapsed (pieces of)
             # geometries, so also collectionextract.
             gridsize_op = f"ST_MakeValid(SnapToGrid(sub_gridsize.geom, {gridsize}))"
             if force_output_geometrytype is None:
@@ -2191,45 +2222,40 @@
                     "can result in inconsistent geometries in the output",
                     stacklevel=2,
                 )
             else:
                 primitivetypeid = force_output_geometrytype.to_primitivetype.value
                 gridsize_op = f"ST_CollectionExtract({gridsize_op}, {primitivetypeid})"
 
-            # Get all columns of the sql_template
-            sql_tmp = sql_template.format(
-                input1_databasename="{input1_databasename}",
-                input2_databasename="{input2_databasename}",
-                batch_filter="",
-            )
-            cols = _sqlite_util.get_columns(
-                sql_stmt=sql_tmp,
-                input1_path=processing_params.input1_path,
-                input2_path=processing_params.input2_path,
-            )
-            cols = [col for col in cols if col.lower() != "geom"]
+            # All columns need to be specified
+            # Remark:
+            # - use "LIMIT -1 OFFSET 0" to avoid the subquery flattening. Flattening
+            #   "geom IS NOT NULL" leads to ST_Difference_Collection calculated double!
+            cols = [col for col in column_datatypes if col.lower() != "geom"]
             columns_to_select = _ogr_sql_util.columns_quoted(cols)
             sql_template = f"""
                 SELECT {gridsize_op} AS geom
                         {columns_to_select}
-                    FROM ( {sql_template}
-                    ) sub_gridsize
+                  FROM ( {sql_template}
+                  ) sub_gridsize
+                 LIMIT -1 OFFSET 0
             """
 
         # Prepare/apply where parameter
         if where is not None and not explodecollections:
             # explodecollections is not True, so we can add where to sql_stmt.
             # If explodecollections would be True, we need to wait to apply the
             # where till after explodecollections is applied, so when appending the
             # partial results to the output file.
             sql_template = f"""
                 SELECT * FROM
                     ( {sql_template}
                     )
-                    WHERE {where}
+                 WHERE {where}
+                 LIMIT -1 OFFSET 0
             """
             # Where has been applied already so set to None.
             where = None
 
         # Calculate
         # ---------
         # Processing in threads is 2x faster for small datasets (on Windows)
@@ -2241,15 +2267,15 @@
         )
         with _processing_util.PooledExecutorFactory(
             threadpool=calculate_in_threads,
             max_workers=processing_params.nb_parallel,
             initializer=_processing_util.initialize_worker(),
         ) as calculate_pool:
             # Start looping
-            batches = {}
+            batches: Dict[int, dict] = {}
             future_to_batch_id = {}
             for batch_id in processing_params.batches:
                 batches[batch_id] = {}
                 batches[batch_id]["layer"] = output_layer
 
                 tmp_partial_output_path = (
                     tempdir / f"{output_path.stem}_{batch_id}.gpkg"
@@ -2275,21 +2301,20 @@
                 future = calculate_pool.submit(
                     calculate_two_layers,
                     input1_path=processing_params.batches[batch_id]["path"],
                     input1_layer=processing_params.batches[batch_id]["layer"],
                     input2_path=processing_params.input2_path,
                     output_path=tmp_partial_output_path,
                     sql_stmt=sql_stmt,
-                    input1_databasename=processing_params.input1_databasename,
-                    input2_databasename=processing_params.input2_databasename,
                     output_layer=output_layer,
                     explodecollections=explodecollections_now,
                     force_output_geometrytype=force_output_geometrytype,
                     use_ogr=use_ogr,
                     create_spatial_index=False,
+                    column_datatypes=column_datatypes,
                 )
                 future_to_batch_id[future] = batch_id
 
             # Loop till all parallel processes are ready, but process each one
             # that is ready already
             nb_done = 0
             _general_util.report_progress(
@@ -2384,20 +2409,19 @@
 
 def calculate_two_layers(
     input1_path: Path,
     input1_layer: str,
     input2_path: Path,
     output_path: Path,
     sql_stmt: str,
-    input1_databasename: str,
-    input2_databasename: str,
     output_layer: str,
     explodecollections: bool,
-    force_output_geometrytype: GeometryType,
+    force_output_geometrytype: Optional[GeometryType],
     create_spatial_index: bool,
+    column_datatypes: dict,
     use_ogr: bool,
 ):
     if use_ogr is False:
         # If explodecollections, write first to tmp file, then apply explodecollections
         # to the final output file.
         output_tmp_path = output_path
         if explodecollections:
@@ -2409,14 +2433,15 @@
             input2_path=input2_path,
             output_path=output_tmp_path,
             sql_stmt=sql_stmt,
             output_layer=output_layer,
             output_geometrytype=force_output_geometrytype,
             create_spatial_index=create_spatial_index,
             profile=_sqlite_util.SqliteProfile.SPEED,
+            column_datatypes=column_datatypes,
         )
         if explodecollections:
             _ogr_util.vector_translate(
                 input_path=output_tmp_path,
                 input_layers=output_layer,
                 output_path=output_path,
                 output_layer=output_layer,
@@ -2427,16 +2452,16 @@
             )
             gfo.remove(output_tmp_path)
     else:
         # Use ogr to run the query
         #   * input2 path (= using attach) doesn't seem to work
         #   * ogr doesn't fill out database names, so do it now
         sql_stmt = sql_stmt.format(
-            input1_databasename=input1_databasename,
-            input2_databasename=input2_databasename,
+            input1_databasename="main",
+            input2_databasename="main",
         )
 
         _ogr_util.vector_translate(
             input_path=input1_path,
             output_path=output_path,
             sql_stmt=sql_stmt,
             output_layer=output_layer,
@@ -2447,30 +2472,31 @@
 
 
 class ProcessingParams:
     def __init__(
         self,
         input1_path: Optional[Path] = None,
         input1_layer: Optional[str] = None,
-        input1_databasename: Optional[str] = None,
         input2_path: Optional[Path] = None,
         input2_layer: Optional[str] = None,
-        input2_databasename: Optional[str] = None,
         nb_parallel: int = -1,
         batches: Optional[dict] = None,
     ):
         self.input1_path = input1_path
         self.input1_layer = input1_layer
-        self.input1_databasename = input1_databasename
         self.input2_path = input2_path
         self.input2_layer = input2_layer
-        self.input2_databasename = input2_databasename
         self.nb_parallel = nb_parallel
         self.batches = batches
 
+    def to_json(self, path: Path):
+        prepared = _general_util.prepare_for_serialize(vars(self))
+        with open(path, "w") as file:
+            file.write(json.dumps(prepared, indent=4, sort_keys=True))
+
 
 def _prepare_processing_params(
     input1_path: Path,
     input1_layer: str,
     tempdir: Path,
     convert_to_spatialite_based: bool,
     nb_parallel: int,
@@ -2588,33 +2614,26 @@
                     src=input2_path,
                     src_layer=input2_layer,
                     dst=returnvalue.input2_path,
                     dst_layer=returnvalue.input2_layer,
                     preserve_fid=True,
                 )
 
-    # Fill out the database names to use in the sql statements
-    returnvalue.input1_databasename = "main"
-    if input2_path is None or input1_path == input2_path:
-        returnvalue.input2_databasename = returnvalue.input1_databasename
-    else:
-        returnvalue.input2_databasename = "input2"
-
     # Prepare batches to process
     # Get column names and info
     layer1_info = gfo.get_layerinfo(
         returnvalue.input1_path, returnvalue.input1_layer, raise_on_nogeom=False
     )
 
     # Check number of batches + appoint nb rows to batches
     nb_rows_input_layer = layer1_info.featurecount
     if nb_batches > int(nb_rows_input_layer / 10):
         nb_batches = max(int(nb_rows_input_layer / 10), 1)
 
-    batches = {}
+    batches: Dict[int, dict] = {}
     if nb_batches == 1:
         # If only one batch, no filtering is needed
         batches[0] = {}
         batches[0]["layer"] = returnvalue.input1_layer
         batches[0]["path"] = returnvalue.input1_path
         batches[0]["batch_filter"] = ""
     else:
@@ -2654,17 +2673,18 @@
                 offset += offset_per_batch
             batch_info_df = pd.DataFrame(
                 batch_info_list, columns=["id", "nb_rows", "start_rowid", "end_rowid"]
             )
         else:
             # The rowids are not consecutive, so determine the optimal rowid
             # ranges for each batch so each batch has same number of elements
-            # Remark: this might take some seconds for larger datasets!
+            # Remark: - this might take some seconds for larger datasets!
+            #         - (batch_id - 1) AS id to make the id zero-based
             sql_stmt = f"""
-                SELECT batch_id AS id
+                SELECT (batch_id - 1) AS id
                       ,COUNT(*) AS nb_rows
                       ,MIN(rowid) AS start_rowid
                       ,MAX(rowid) AS end_rowid
                   FROM
                     ( SELECT rowid
                             ,NTILE({nb_batches}) OVER (ORDER BY rowid) batch_id
                         FROM "{layer1_info.name}"
@@ -2699,14 +2719,15 @@
                 ] = f"AND {layer_alias_d}rowid >= {batch_info.start_rowid} "
 
     # No use starting more processes than the number of batches...
     if len(batches) < returnvalue.nb_parallel:
         returnvalue.nb_parallel = len(batches)
 
     returnvalue.batches = batches
+    returnvalue.to_json(tempdir / "processing_params.json")
     return returnvalue
 
 
 def dissolve_singlethread(
     input_path: Path,
     output_path: Path,
     groupby_columns: Union[str, Iterable[str], None] = None,
```

### Comparing `geofileops-0.8.0a7/geofileops/util/_io_util.py` & `geofileops-0.8.0a8/geofileops/util/_io_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/util/_ogr_sql_util.py` & `geofileops-0.8.0a8/geofileops/util/_ogr_sql_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/util/_ogr_util.py` & `geofileops-0.8.0a8/geofileops/util/_ogr_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/util/_processing_util.py` & `geofileops-0.8.0a8/geofileops/util/_processing_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/util/_sqlite_util.py` & `geofileops-0.8.0a8/geofileops/util/_sqlite_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 Module containing utilities regarding sqlite/spatialite files.
 """
 
 import datetime
 import enum
 import logging
 from pathlib import Path
+import shutil
 import sqlite3
-from typing import List, Optional, Union
-
+import tempfile
+from typing import Dict, List, Optional, Union
 
 import geofileops as gfo
 from geofileops import GeometryType
-from ._general_util import MissingRuntimeDependencyError
+from geofileops.util._general_util import MissingRuntimeDependencyError
+from geofileops.util import _sqlite_userdefined as sqlite_userdefined
 
 #####################################################################
 # First define/init some general variables/constants
 #####################################################################
 
 # Get a logger...
 logger = logging.getLogger(__name__)
@@ -87,53 +89,142 @@
         conn.close()
 
 
 def get_columns(
     sql_stmt: str,
     input1_path: Path,
     input2_path: Optional[Path] = None,
+    empty_output_ok: bool = True,
     use_spatialite: bool = True,
-) -> List[str]:
-    input1_databasename = "main"
-    conn = sqlite3.connect(str(input1_path), uri=True)
+    output_geometrytype: Optional[GeometryType] = None,
+) -> Dict[str, str]:
+    # Create temp output db to be sure the output DB is writable, even though we only
+    # create a temporary table.
+    tmp_dir = Path(tempfile.mkdtemp(prefix="geofileops/get_columns_"))
+    tmp_path = tmp_dir / f"temp{input1_path.suffix}"
+    create_new_spatialdb(path=tmp_path)
+
     sql = None
+    conn = sqlite3.connect(tmp_path, detect_types=sqlite3.PARSE_DECLTYPES)
     try:
-        if use_spatialite is True:
+        # Load spatialite if asked for
+        if use_spatialite:
             load_spatialite(conn)
-            if input1_path.suffix.lower() == ".gpkg":
+            if tmp_path.suffix.lower() == ".gpkg":
                 sql = "SELECT EnableGpkgMode();"
                 conn.execute(sql)
 
+        # Attach to input1
+        input1_databasename = "input1"
+        sql = f"ATTACH DATABASE ? AS {input1_databasename}"
+        dbSpec = (str(input1_path),)
+        conn.execute(sql, dbSpec)
+
         # If input2 isn't the same database input1, attach to it
         input2_databasename = None
         if input2_path is not None:
             if input2_path == input1_path:
                 input2_databasename = input1_databasename
             else:
                 input2_databasename = "input2"
                 sql = f"ATTACH DATABASE ? AS {input2_databasename}"
-                # dbSpec = (f"file:{input2_path.resolve().as_posix()}?mode=ro",)
                 dbSpec = (str(input2_path),)
                 conn.execute(sql, dbSpec)
-        # Prepare sql statement
+
+        # Prepare sql statement for execute
         sql = sql_stmt.format(
             input1_databasename=input1_databasename,
             input2_databasename=input2_databasename,
+            batch_filter="",
         )
 
-        # Execute sql to be able to get the column names
-        cur = conn.cursor()
-        cur.execute(sql)
-        columns = [desc[0] for desc in cur.description]
-        conn.rollback()
+        # Create temp table to get the column names + general data types
+        # + fetch one row to use it to determine geometrytype.
+        # Remark: specify redundant OFFSET 0 to keep sqlite from flattings the subquery.
+        sql = f"""
+            CREATE TEMPORARY TABLE tmp AS
+            SELECT *
+                FROM (
+                {sql}
+                )
+             LIMIT 1 OFFSET 0;
+        """
+        conn.execute(sql)
+        conn.commit()
+        sql = "PRAGMA TABLE_INFO(tmp)"
+        cur = conn.execute(sql)
+        tmpcolumns = cur.fetchall()
+        cur.close()
+
+        # Fetch one row to try to get more detailed data types if needed
+        sql = "SELECT * FROM tmp"
+        tmpdata = conn.execute(sql).fetchone()
+        if tmpdata is not None and len(tmpdata) == 0:
+            tmpdata = None
+        if not empty_output_ok and tmpdata is None:
+            # If no row was returned, stop
+            raise EmptyResultError(f"Query didn't return any rows: {sql_stmt}")
+
+        # Loop over all columns to determine the data type
+        columns = {}
+        for column_index, column in enumerate(tmpcolumns):
+            columnname = column[1]
+            columntype = column[2]
+
+            if columnname == "geom":
+                # PRAGMA TABLE_INFO gives None as column type for a
+                # geometry column. So if output_geometrytype not specified,
+                # Use ST_GeometryType to get the type
+                # based on the data + apply to_multitype to be sure
+                if output_geometrytype is None:
+                    sql = f"SELECT ST_GeometryType({columnname}) FROM tmp;"
+                    result = conn.execute(sql).fetchall()
+                    if len(result) > 0 and result[0][0] is not None:
+                        output_geometrytype = GeometryType[result[0][0]].to_multitype
+                    else:
+                        output_geometrytype = GeometryType["GEOMETRY"]
+                columns[columnname] = output_geometrytype.name
+            else:
+                # If PRAGMA TABLE_INFO doesn't specify the datatype, determine based
+                # on data.
+                if columntype is None or columntype == "":
+                    sql = f"SELECT typeof({columnname}) FROM tmp;"
+                    result = conn.execute(sql).fetchall()
+                    if len(result) > 0 and result[0][0] is not None:
+                        columns[columnname] = result[0][0]
+                    else:
+                        # If unknown, take the most general types
+                        columns[columnname] = "NUMERIC"
+                elif columntype == "NUM":
+                    # PRAGMA TABLE_INFO sometimes returns 'NUM', but apparently this
+                    # cannot be used in "CREATE TABLE".
+                    if tmpdata is not None and isinstance(
+                        tmpdata[column_index], datetime.date
+                    ):
+                        columns[columnname] = "DATE"
+                    elif tmpdata is not None and isinstance(
+                        tmpdata[column_index], datetime.datetime
+                    ):
+                        columns[columnname] = "DATETIME"
+                    else:
+                        sql = f'SELECT datetime("{columnname}") FROM tmp;'
+                        result = conn.execute(sql).fetchall()
+                        if len(result) > 0 and result[0][0] is not None:
+                            columns[columnname] = "DATETIME"
+                        else:
+                            columns[columnname] = "NUMERIC"
+                else:
+                    columns[columnname] = columntype
+
     except Exception as ex:
         conn.rollback()
-        raise Exception(f"Error {ex} executing {sql}") from ex
+        raise RuntimeError(f"Error {ex} executing {sql}") from ex
     finally:
         conn.close()
+        shutil.rmtree(tmp_dir, ignore_errors=True)
 
     return columns
 
 
 def create_table_as_sql(
     input1_path: Path,
     input1_layer: str,
@@ -195,15 +286,15 @@
         crs_epsg = input1_layerinfo.crs.to_epsg()
 
     # If output file doesn't exist yet, create and init it
     if not output_path.exists():
         create_new_spatialdb(path=output_path, crs_epsg=crs_epsg)
 
     sql = None
-    conn = sqlite3.connect(output_path, detect_types=sqlite3.PARSE_DECLTYPES)
+    conn = sqlite3.connect(output_path, detect_types=sqlite3.PARSE_DECLTYPES, uri=True)
     try:
         with conn:
 
             def to_string_for_sql(input) -> str:
                 if input is None:
                     return "NULL"
                 else:
@@ -216,35 +307,43 @@
             output_databasename = "main"
             load_spatialite(conn)
 
             if output_suffix_lower == ".gpkg":
                 sql = "SELECT EnableGpkgMode();"
                 conn.execute(sql)
 
-            # Set nb KB of cache
+            # Set cache size to 128 MB (in kibibytes)
             sql = "PRAGMA cache_size=-128000;"
             conn.execute(sql)
             # Set temp storage to MEMORY
             sql = "PRAGMA temp_store=2;"
             conn.execute(sql)
+            # Set soft heap limit to 1 GB (in bytes)
+            sql = f"PRAGMA soft_heap_limit={1024*1024*1024};"
+            conn.execute(sql)
 
             # If attach to input1
             input1_databasename = "input1"
             sql = f"ATTACH DATABASE ? AS {input1_databasename}"
             dbSpec = (str(input1_path),)
+            # input1_uri = f"file:{input1_path}?immutable=1"
+            # dbSpec = (str(input1_uri),)
             conn.execute(sql, dbSpec)
 
             # If input2 isn't the same database input1, attach to it
+            input2_databasename = None
             if input2_path is not None:
                 if input2_path == input1_path:
                     input2_databasename = input1_databasename
                 else:
                     input2_databasename = "input2"
                     sql = f"ATTACH DATABASE ? AS {input2_databasename}"
                     dbSpec = (str(input2_path),)
+                    # input2_uri = f"file:{input1_path}?immutable=1"
+                    # dbSpec = (str(input2_uri),)
                     conn.execute(sql, dbSpec)
 
             # Use the sqlite profile specified
             if profile is SqliteProfile.SPEED:
                 # Use memory mapped IO: much faster for calculations
                 # (max 30GB)
                 conn.execute("PRAGMA mmap_size=30000000000;")
@@ -258,100 +357,42 @@
                 ]:
                     conn.execute(f"PRAGMA {databasename}.journal_mode=OFF;")
 
                     # These pragma's increase speed
                     conn.execute(f"PRAGMA {databasename}.locking_mode=EXCLUSIVE;")
                     conn.execute(f"PRAGMA {databasename}.synchronous=OFF;")
 
+            # Determine columns/datatypes to create the table if not specified
+            column_types = column_datatypes
+            if column_types is None:
+                column_types = get_columns(
+                    sql_stmt=sql_stmt,
+                    input1_path=input1_path,
+                    input2_path=input2_path,
+                    empty_output_ok=empty_output_ok,
+                    use_spatialite=True,
+                    output_geometrytype=output_geometrytype,
+                )
+
+            # If geometry type was not specified, look for it in column_types
+            if output_geometrytype is None:
+                if "geom" in column_types:
+                    output_geometrytype = GeometryType(column_types["geom"])
+                else:
+                    raise ValueError(
+                        "output_geometrytype not specified + determination from "
+                        "sql_stmt failed"
+                    )
+
             # Prepare sql statement
             sql_stmt = sql_stmt.format(
                 input1_databasename=input1_databasename,
                 input2_databasename=input2_databasename,
             )
 
-            # Determine columns/datatypes to create the table
-            # Create temp table to get the column names + general data types
-            # + fetch one row to use it to determine geometrytype.
-            sql = f"""
-                CREATE TEMPORARY TABLE tmp AS
-                  SELECT *
-                    FROM (
-                      {sql_stmt}
-                    )
-                  LIMIT 1;
-            """
-            conn.execute(sql)
-            sql = "PRAGMA TABLE_INFO(tmp)"
-            cur = conn.execute(sql)
-            tmpcolumns = cur.fetchall()
-
-            # Fetch one row to try to get more detailed data types if needed
-            sql = "SELECT * FROM tmp"
-            tmpdata = conn.execute(sql).fetchone()
-            if tmpdata is not None and len(tmpdata) == 0:
-                tmpdata = None
-            if not empty_output_ok and tmpdata is None:
-                # If no row was returned, stop
-                raise EmptyResultError(f"Query didn't return any rows: {sql_stmt}")
-
-            # Loop over all columns to determine the data type
-            column_types = {}
-            for column_index, column in enumerate(tmpcolumns):
-                columnname = column[1]
-                columntype = column[2]
-
-                if column_datatypes is not None and columnname in column_datatypes:
-                    column_types[columnname] = column_datatypes[columnname]
-                elif columnname == "geom":
-                    # PRAGMA TABLE_INFO gives None as column type for a
-                    # geometry column. So if output_geometrytype not specified,
-                    # Use ST_GeometryType to get the type
-                    # based on the data + apply to_multitype to be sure
-                    if output_geometrytype is None:
-                        sql = f"SELECT ST_GeometryType({columnname}) FROM tmp;"
-                        result = conn.execute(sql).fetchall()
-                        if len(result) > 0:
-                            output_geometrytype = GeometryType[
-                                result[0][0]
-                            ].to_multitype
-                        else:
-                            output_geometrytype = GeometryType["GEOMETRY"]
-                    column_types[columnname] = output_geometrytype.name
-                else:
-                    # If PRAGMA TABLE_INFO doesn't specify the datatype, determine based
-                    # on data.
-                    if columntype is None or columntype == "":
-                        sql = f"SELECT typeof({columnname}) FROM tmp;"
-                        result = conn.execute(sql).fetchall()
-                        if len(result) > 0 and result[0][0] is not None:
-                            column_types[columnname] = result[0][0]
-                        else:
-                            # If unknown, take the most general types
-                            column_types[columnname] = "NUMERIC"
-                    elif columntype == "NUM":
-                        # PRAGMA TABLE_INFO sometimes returns 'NUM', but apparently this
-                        # cannot be used in "CREATE TABLE".
-                        if tmpdata is not None and isinstance(
-                            tmpdata[column_index], datetime.date
-                        ):
-                            column_types[columnname] = "DATE"
-                        elif tmpdata is not None and isinstance(
-                            tmpdata[column_index], datetime.datetime
-                        ):
-                            column_types[columnname] = "DATETIME"
-                        else:
-                            sql = f'SELECT datetime("{columnname}") FROM tmp;'
-                            result = conn.execute(sql).fetchall()
-                            if len(result) > 0 and result[0][0] is not None:
-                                column_types[columnname] = "DATETIME"
-                            else:
-                                column_types[columnname] = "NUMERIC"
-                    else:
-                        column_types[columnname] = columntype
-
             # Now we can create the table
             # Create output table using the gpkgAddGeometryColumn() function
             # Problem: the spatialite function gpkgAddGeometryColumn() doesn't support
             # layer names with special characters (eg. '-')...
             # Solution: mimic the behaviour of gpkgAddGeometryColumn manually.
             # Create table without geom column
             """
@@ -417,20 +458,21 @@
                         '{output_layer}', 'geom',
                         {to_string_for_sql(crs_epsg)}, '{output_geometrytype.name}');
                 """
                 conn.execute(sql)
 
             # Insert data using the sql statement specified
             try:
-                columns_for_insert = [f'"{column[1]}"' for column in tmpcolumns]
+                columns_for_insert = [f'"{column}"' for column in column_types]
                 sql = (
                     f'INSERT INTO {output_databasename}."{output_layer}" '
                     f'({", ".join(columns_for_insert)})\n{sql_stmt}'
                 )
                 conn.execute(sql)
+
             except Exception as ex:
                 ex_message = str(ex).lower()
                 if ex_message.startswith(
                     "unique constraint failed:"
                 ) and ex_message.endswith(".fid"):
                     ex.args = (
                         f"{ex}: avoid this by not selecting or aliasing fid "
@@ -463,19 +505,18 @@
                     sql = f"SELECT CreateSpatialIndex('{output_layer}', 'geom');"
                     conn.execute(sql)
             conn.commit()
 
     except EmptyResultError:
         logger.info(f"Query didn't return any rows: {sql_stmt}")
         conn.close()
-        conn = None
         if output_path.exists():
             output_path.unlink()
     except Exception as ex:
-        raise Exception(f"Error {ex} executing {sql}") from ex
+        raise RuntimeError(f"Error {ex} executing {sql}") from ex
     finally:
         if conn is not None:
             conn.close()
 
 
 def execute_sql(
     path: Path, sql_stmt: Union[str, List[str]], use_spatialite: bool = True
@@ -563,7 +604,18 @@
     conn.enable_load_extension(True)
     try:
         conn.load_extension("mod_spatialite")
     except Exception as ex:
         raise MissingRuntimeDependencyError(
             "Error trying to load mod_spatialite."
         ) from ex
+
+    # Register custom function
+    conn.create_function(
+        "st_difference_collection",
+        -1,
+        sqlite_userdefined.st_difference_collection,
+        deterministic=True,
+    )
+
+    # Register custom aggregate function
+    # conn.create_aggregate("st_difference_agg", 3, userdefined.DifferenceAgg)
```

### Comparing `geofileops-0.8.0a7/geofileops/util/geodataframe_util.py` & `geofileops-0.8.0a8/geofileops/util/geodataframe_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/util/geofiletype.py` & `geofileops-0.8.0a8/geofileops/util/geofiletype.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/util/geofiletypes.csv` & `geofileops-0.8.0a8/geofileops/util/geofiletypes.csv`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/util/geometry_util.py` & `geofileops-0.8.0a8/geofileops/util/geometry_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/util/geoseries_util.py` & `geofileops-0.8.0a8/geofileops/util/geoseries_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,17 +270,15 @@
             ):
                 # Start or end point of the simplified version is not the same anymore
                 continue
             else:
                 topo.output["arcs"][index] = list(topoline_simpl)
 
     topo_simpl_gdf = topo.to_gdf(crs=geoseries.crs)
-    topo_simpl_gdf.geometry = shapely2_or_pygeos.make_valid(
-        topo_simpl_gdf.geometry.array.data
-    )
+    topo_simpl_gdf.geometry = shapely2_or_pygeos.make_valid(topo_simpl_gdf.geometry)
     geometry_types_orig = geoseries.geom_type.unique()
     geometry_types_simpl = topo_simpl_gdf.geometry.geom_type.unique()
     if len(geometry_types_orig) == 1 and len(geometry_types_simpl) > 1:
         topo_simpl_gdf.geometry = geometry_collection_extract(
             topo_simpl_gdf.geometry,
             GeometryType(geometry_types_orig[0]).to_primitivetype,
         )
```

### Comparing `geofileops-0.8.0a7/geofileops/util/grid_util.py` & `geofileops-0.8.0a8/geofileops/util/grid_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops/util/test.gpkg` & `geofileops-0.8.0a8/geofileops/util/test.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/geofileops.egg-info/PKG-INFO` & `geofileops-0.8.0a8/geofileops.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geofileops
-Version: 0.8.0a7
+Version: 0.8.0a8
 Summary: Package to do spatial operations on large geo files.
 Home-page: https://github.com/geofileops/geofileops
 Author: Pieter Roggemans
 Author-email: pieter.roggemans@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `geofileops-0.8.0a7/geofileops.egg-info/SOURCES.txt` & `geofileops-0.8.0a8/geofileops.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 geofileops/util/_geoops_gpd.py
 geofileops/util/_geoops_ogr.py
 geofileops/util/_geoops_sql.py
 geofileops/util/_io_util.py
 geofileops/util/_ogr_sql_util.py
 geofileops/util/_ogr_util.py
 geofileops/util/_processing_util.py
+geofileops/util/_sqlite_userdefined.py
 geofileops/util/_sqlite_util.py
 geofileops/util/geodataframe_util.py
 geofileops/util/geofiletype.py
 geofileops/util/geofiletypes.csv
 geofileops/util/geometry_util.py
 geofileops/util/geoseries_util.py
 geofileops/util/grid_util.py
@@ -57,14 +58,15 @@
 tests/test_io_util.py
 tests/test_layerstyles.py
 tests/test_ogr_sql_util.py
 tests/test_ogr_util.py
 tests/test_parameter_helper.py
 tests/test_processing_util.py
 tests/test_spatialite.py
+tests/test_sqlite_userdefined.py
 tests/test_sqlite_util.py
 tests/test_version.py
 tests/data/BEFL-kbl.gpkg
 tests/data/geofileops_testdata.qgz
 tests/data/linestring-row-trees.gpkg
 tests/data/linestring-watercourse.gpkg
 tests/data/linestrings_hedges.gpkg
```

### Comparing `geofileops-0.8.0a7/pyproject.toml` & `geofileops-0.8.0a8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/setup.py` & `geofileops-0.8.0a8/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,17 +21,18 @@
         "cloudpickle",
         "fiona",
         "gdal",
         "geopandas>=0.11,<0.14",
         "numpy",
         "pandas",
         "psutil",
+        "pygeoops>=0.2,<0.3",
         "pyogrio",
         "pyproj",
-        "shapely",
+        "shapely>=2,<2.1",
         "topojson",
     ],
     extras_require={"full": ["simplification"]},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
```

### Comparing `geofileops-0.8.0a7/tests/data/BEFL-kbl.gpkg` & `geofileops-0.8.0a8/tests/data/BEFL-kbl.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/geofileops_testdata.qgz` & `geofileops-0.8.0a8/tests/data/geofileops_testdata.qgz`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/linestring-row-trees.gpkg` & `geofileops-0.8.0a8/tests/data/linestring-row-trees.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/linestring-watercourse.gpkg` & `geofileops-0.8.0a8/tests/data/linestring-watercourse.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/linestrings_hedges.gpkg` & `geofileops-0.8.0a8/tests/data/linestrings_hedges.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/point.gpkg` & `geofileops-0.8.0a8/tests/data/point.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/polygon-invalid.gpkg` & `geofileops-0.8.0a8/tests/data/polygon-invalid.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/polygon-no-rows.gpkg` & `geofileops-0.8.0a8/tests/data/polygon-no-rows.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/polygon-overlappingcircles-all.gpkg` & `geofileops-0.8.0a8/tests/data/polygon-overlappingcircles-all.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/polygon-overlappingcircles-one.gpkg` & `geofileops-0.8.0a8/tests/data/polygon-overlappingcircles-one.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/polygon-overlappingcircles-two+three.gpkg` & `geofileops-0.8.0a8/tests/data/polygon-overlappingcircles-two+three.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/polygon-parcel.gpkg` & `geofileops-0.8.0a8/tests/data/polygon-parcel.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/polygon-simplify-onborder-testcase.gpkg` & `geofileops-0.8.0a8/tests/data/polygon-simplify-onborder-testcase.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/polygon-twolayers.gpkg` & `geofileops-0.8.0a8/tests/data/polygon-twolayers.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/polygon-zone.gpkg` & `geofileops-0.8.0a8/tests/data/polygon-zone.gpkg`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/polygonstyle.qml` & `geofileops-0.8.0a8/tests/data/polygonstyle.qml`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/data/polygonstyle.sld` & `geofileops-0.8.0a8/tests/data/polygonstyle.sld`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_general_util.py` & `geofileops-0.8.0a8/tests/test_general_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_geofile.py` & `geofileops-0.8.0a8/tests/test_geofile.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_geofileops_singlelayer.py` & `geofileops-0.8.0a8/tests/test_geofileops_singlelayer.py`

 * *Files 6% similar despite different names*

```diff
@@ -655,7 +655,38 @@
     # If input was empty, we are already OK
     if empty_input:
         return
 
     # More detailed checks
     output_gdf = fileops.read_file(output_path)
     assert_geodataframe_equal(output_gdf, expected_gdf, sort_values=True)
+
+
+@pytest.mark.parametrize(
+    "algorithm",
+    [
+        "lang",
+        "rdp",
+        "vw",
+        geoops.SimplifyAlgorithm.LANG,
+        geoops.SimplifyAlgorithm.RAMER_DOUGLAS_PEUCKER,
+        geoops.SimplifyAlgorithm.VISVALINGAM_WHYATT,
+    ],
+)
+def test_simplify_algorithms(tmp_path, algorithm):
+    """
+    Rude check on supported algorithms.
+    """
+    input_path = test_helper.get_testfile("polygon-parcel")
+    output_path = tmp_path / f"{input_path.stem}_output.gpkg"
+
+    # Test specifically with geoops
+    set_geoops_module("geofileops.geoops")
+    geoops.simplify(
+        input_path=input_path,
+        output_path=output_path,
+        tolerance=1,
+        algorithm=algorithm,
+        nb_parallel=2,
+    )
+
+    assert output_path.exists()
```

### Comparing `geofileops-0.8.0a7/tests/test_geofileops_singlelayer_gpd.py` & `geofileops-0.8.0a8/tests/test_geofileops_singlelayer_gpd.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_geofileops_singlelayer_ogr.py` & `geofileops-0.8.0a8/tests/test_geofileops_singlelayer_ogr.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_geofileops_singlelayer_sql.py` & `geofileops-0.8.0a8/tests/test_geofileops_singlelayer_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     # Check result, 2 duplicates should be removed
     result_info = gfo.get_layerinfo(output_path)
     assert result_info.featurecount == input_info.featurecount - 2
     result_gdf = gfo.read_file(output_path)
     if gridsize != 0.0:
         expected_gdf.geometry = shapely2_or_pygeos.set_precision(
-            expected_gdf.geometry.array.data, grid_size=gridsize
+            expected_gdf.geometry, grid_size=gridsize
         )
     assert_geodataframe_equal(result_gdf, expected_gdf)
 
 
 def test_dissolve_singlethread_output_exists(tmp_path):
     # Prepare test data
     input_path = test_helper.get_testfile("polygon-parcel")
```

### Comparing `geofileops-0.8.0a7/tests/test_geofileops_twolayers.py` & `geofileops-0.8.0a8/tests/test_geofileops_twolayers.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,20 +48,28 @@
     clip_gdf = gfo.read_file(clip_path)
     output_gpd_gdf = gpd.clip(input_gdf, clip_gdf, keep_geom_type=True)
     assert_geodataframe_equal(
         output_gdf, output_gpd_gdf, promote_to_multi=True, sort_values=True
     )
 
 
-@pytest.mark.parametrize("testfile", TESTFILES)
 @pytest.mark.parametrize("suffix", SUFFIXES)
 @pytest.mark.parametrize(
-    "gridsize, where", [(0.0, "ST_Area(geom) > 2000"), (0.001, None)]
+    "testfile, gridsize, where",
+    [
+        ("linestring-row-trees", 0.0, "ST_Length(geom) > 100"),
+        ("linestring-row-trees", 0.001, None),
+        ("point", 0.0, None),
+        ("point", 0.001, None),
+        ("polygon-parcel", 0.0, None),
+        ("polygon-parcel", 0.0, "ST_Area(geom) > 2000"),
+        ("polygon-parcel", 0.001, None),
+    ],
 )
-def test_erase(tmp_path, testfile, suffix, gridsize, where):
+def test_erase(tmp_path, suffix, testfile, gridsize, where):
     input_path = test_helper.get_testfile(testfile, suffix=suffix)
     erase_path = test_helper.get_testfile("polygon-zone", suffix=suffix)
     input_layerinfo = gfo.get_layerinfo(input_path)
     batchsize = math.ceil(input_layerinfo.featurecount / 2)
     output_path = tmp_path / f"{input_path.stem}-output{suffix}"
 
     gfo.erase(
@@ -80,28 +88,40 @@
     input_gdf = gfo.read_file(input_path)
     erase_gdf = gfo.read_file(erase_path)
     output_gpd_gdf = gpd.overlay(
         input_gdf, erase_gdf, how="difference", keep_geom_type=True
     )
     if gridsize != 0.0:
         output_gpd_gdf.geometry = shapely2_or_pygeos.set_precision(
-            output_gpd_gdf.geometry.array.data, grid_size=gridsize
+            output_gpd_gdf.geometry, grid_size=gridsize
         )
     if where is not None:
-        output_gpd_gdf = output_gpd_gdf[output_gpd_gdf.geometry.area > 2000]
+        if where == "ST_Area(geom) > 2000":
+            output_gpd_gdf = output_gpd_gdf[output_gpd_gdf.geometry.area > 2000]
+        elif where == "ST_Length(geom) > 100":
+            output_gpd_gdf = output_gpd_gdf[output_gpd_gdf.geometry.length > 100]
+        else:
+            raise ValueError(f"where filter not implemented: {where}")
+    output_gpd_path = tmp_path / f"{input_path.stem}-output_gpd{suffix}"
+
+    if test_helper.RUNS_LOCAL:
+        gfo.to_file(output_gpd_gdf, output_gpd_path)
 
     assert_geodataframe_equal(
         output_gdf,
         output_gpd_gdf,
         promote_to_multi=True,
         sort_values=True,
         check_less_precise=True,
         normalize=True,
     )
 
+    # Make sure the output still has rows, otherwise the test isn't super useful
+    assert len(output_gdf) > 0
+
 
 def test_erase_explodecollections(tmp_path):
     input_path = test_helper.get_testfile("polygon-parcel")
     erase_path = test_helper.get_testfile("polygon-zone")
     input_layerinfo = gfo.get_layerinfo(input_path)
     batchsize = math.ceil(input_layerinfo.featurecount / 2)
 
@@ -250,29 +270,29 @@
     )
     assert output_layerinfo.geometrytype == GeometryType.MULTIPOLYGON
     if explodecollections:
         assert output_layerinfo.featurecount == 31
     else:
         assert output_layerinfo.featurecount == 30
 
-    # Check the contents of the result file
+    # Check the contents of the result file by comparing with geopandas
     output_gdf = gfo.read_file(output_path)
     assert output_gdf["geometry"][0] is not None
 
     input1_gdf = gfo.read_file(input1_path)
     input2_gdf = gfo.read_file(input2_path)
     overlay_operation = "intersection"
     expected_gdf = input1_gdf.overlay(
         input2_gdf, how=overlay_operation, keep_geom_type=True
     )
     renames = dict(zip(expected_gdf.columns, output_gdf.columns))
     expected_gdf = expected_gdf.rename(columns=renames)
     if gridsize != 0.0:
         expected_gdf.geometry = shapely2_or_pygeos.set_precision(
-            expected_gdf.geometry.array.data, grid_size=gridsize
+            expected_gdf.geometry, grid_size=gridsize
         )
     if explodecollections:
         expected_gdf = expected_gdf.explode(ignore_index=True)
     assert_geodataframe_equal(
         output_gdf, expected_gdf, check_dtype=False, sort_values=True
     )
 
@@ -810,15 +830,15 @@
               {layer2_columns_prefix_alias_str}
               layer1.invalid_column
           FROM {input1_databasename}."{input1_layer}" layer1
           CROSS JOIN {input2_databasename}."{input2_layer}" layer2
          WHERE 1=1
            AND ST_Area(layer1.{input1_geometrycolumn}) > 5
     """
-    with pytest.raises(Exception, match='Error <Error near "layer1": syntax error'):
+    with pytest.raises(RuntimeError, match='Error near "layer1": syntax error'):
         gfo.select_two_layers(
             input1_path=input1_path,
             input2_path=input2_path,
             output_path=output_path,
             sql_stmt=sql_stmt,
         )
 
@@ -1004,15 +1024,15 @@
     input1_gdf = gfo.read_file(input1_path)
     input2_gdf = gfo.read_file(input2_path)
     output_gpd_gdf = input1_gdf.overlay(input2_gdf, how="identity", keep_geom_type=True)
     renames = dict(zip(output_gpd_gdf.columns, output_gfo_gdf.columns))
     output_gpd_gdf = output_gpd_gdf.rename(columns=renames)
     if gridsize != 0.0:
         output_gpd_gdf.geometry = shapely2_or_pygeos.set_precision(
-            output_gpd_gdf.geometry.array.data, grid_size=gridsize
+            output_gpd_gdf.geometry, grid_size=gridsize
         )
     # OIDN is float vs int? -> check_column_type=False
     assert_geodataframe_equal(
         output_gfo_gdf,
         output_gpd_gdf,
         promote_to_multi=True,
         sort_values=True,
@@ -1052,15 +1072,15 @@
     output_gpd_gdf = input1_gdf.overlay(
         input2_gdf, how="symmetric_difference", keep_geom_type=True
     )
     renames = dict(zip(output_gpd_gdf.columns, output_gfo_gdf.columns))
     output_gpd_gdf = output_gpd_gdf.rename(columns=renames)
     if gridsize != 0.0:
         output_gpd_gdf.geometry = shapely2_or_pygeos.set_precision(
-            output_gpd_gdf.geometry.array.data, grid_size=gridsize
+            output_gpd_gdf.geometry, grid_size=gridsize
         )
     assert_geodataframe_equal(
         output_gfo_gdf,
         output_gpd_gdf,
         promote_to_multi=True,
         sort_values=True,
         check_column_type=False,
@@ -1125,15 +1145,15 @@
     input2_gdf = gfo.read_file(input2_path)
     output_gpd_gdf = input1_gdf.overlay(input2_gdf, how="union", keep_geom_type=True)
     renames = dict(zip(output_gpd_gdf.columns, output_gfo_gdf.columns))
     output_gpd_gdf = output_gpd_gdf.rename(columns=renames)
     output_gpd_gdf["l1_DATUM"] = pd.to_datetime(output_gpd_gdf["l1_DATUM"])
     if gridsize != 0.0:
         output_gpd_gdf.geometry = shapely2_or_pygeos.set_precision(
-            output_gpd_gdf.geometry.array.data, grid_size=gridsize
+            output_gpd_gdf.geometry, grid_size=gridsize
         )
     if explodecollections:
         output_gpd_gdf = output_gpd_gdf.explode(ignore_index=True)
     if where is not None:
         output_gpd_gdf = output_gpd_gdf[output_gpd_gdf.geometry.area > 1000]
 
     assert_geodataframe_equal(
```

### Comparing `geofileops-0.8.0a7/tests/test_geofiletype.py` & `geofileops-0.8.0a8/tests/test_geofiletype.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_geometry_util.py` & `geofileops-0.8.0a8/tests/test_geometry_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_geoseries_util.py` & `geofileops-0.8.0a8/tests/test_geoseries_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_grid_util.py` & `geofileops-0.8.0a8/tests/test_grid_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_helper.py` & `geofileops-0.8.0a8/tests/test_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 Helper functions for all tests.
 """
 
+import os
 from pathlib import Path
 import tempfile
 from typing import List, Optional, Union
 
 import geopandas as gpd
 import geopandas._compat as gpd_compat
 import geopandas.testing as gpd_testing
@@ -27,14 +28,18 @@
 SUFFIXES = [".gpkg", ".shp"]
 TESTFILES = ["polygon-parcel", "linestring-row-trees", "point"]
 WHERE_AREA_GT_400 = "ST_Area({geometrycolumn}) > 400"
 WHERE_AREA_GT_5000 = "ST_Area({geometrycolumn}) > 5000"
 WHERE_LENGTH_GT_1000 = "ST_Length({geometrycolumn}) > 1000"
 WHERE_LENGTH_GT_200000 = "ST_Length({geometrycolumn}) > 200000"
 
+RUNS_LOCAL = True
+if "GITHUB_ACTIONS" in os.environ:
+    RUNS_LOCAL = False
+
 
 def prepare_expected_result(
     gdf: gpd.GeoDataFrame,
     keep_empty_geoms: bool,
     gridsize: float = 0.0,
     where: Optional[str] = None,
     explodecollections=False,
@@ -42,15 +47,15 @@
 ) -> gpd.GeoDataFrame:
     """Prepare expected data"""
 
     expected_gdf = gdf.copy()
 
     if gridsize != 0.0:
         expected_gdf.geometry = shapely2_or_pygeos.set_precision(
-            expected_gdf.geometry.array.data, grid_size=gridsize
+            expected_gdf.geometry, grid_size=gridsize
         )
     if explodecollections:
         expected_gdf = expected_gdf.explode(ignore_index=True)
 
     # Check what filtering is needed
     filter_area_gt = None
     if where is None or where == "":
@@ -310,18 +315,18 @@
         left.loc[left.geometry.is_empty, ["geometry"]] = None
         right = right.copy()
         right.loc[right.geometry.is_empty, ["geometry"]] = None
 
     if sort_values:
         if normalize:
             left.geometry = gpd.GeoSeries(
-                shapely2_or_pygeos.normalize(left.geometry.array.data), index=left.index
+                shapely2_or_pygeos.normalize(left.geometry), index=left.index
             )
             right.geometry = gpd.GeoSeries(
-                shapely2_or_pygeos.normalize(right.geometry.array.data),
+                shapely2_or_pygeos.normalize(right.geometry),
                 index=right.index,
             )
         if promote_to_multi:
             left.geometry = geoseries_util.harmonize_geometrytypes(
                 left.geometry, force_multitype=True
             )
             right.geometry = geoseries_util.harmonize_geometrytypes(
```

### Comparing `geofileops-0.8.0a7/tests/test_io_util.py` & `geofileops-0.8.0a8/tests/test_io_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_layerstyles.py` & `geofileops-0.8.0a8/tests/test_layerstyles.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_ogr_sql_util.py` & `geofileops-0.8.0a8/tests/test_ogr_sql_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_ogr_util.py` & `geofileops-0.8.0a8/tests/test_ogr_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_parameter_helper.py` & `geofileops-0.8.0a8/tests/test_parameter_helper.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_processing_util.py` & `geofileops-0.8.0a8/tests/test_processing_util.py`

 * *Files identical despite different names*

### Comparing `geofileops-0.8.0a7/tests/test_spatialite.py` & `geofileops-0.8.0a8/tests/test_spatialite.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 # -*- coding: utf-8 -*-
 """
 Tests for functionalities in ogr_util.
 """
 
-import os
-
 import pytest
 
 import geofileops as gfo
 from tests import test_helper
 
 
 @pytest.mark.skipif(
-    "GITHUB_ACTIONS" in os.environ,
-    reason="Don't run on CI: just to followup odd behaviour in spatialite.",
+    not test_helper.RUNS_LOCAL,
+    reason="Don't this run on CI: just to followup odd behaviour in spatialite.",
 )
 def test_st_difference_null(tmp_path):
     """
     ST_difference returns NULL when 2nd argument is NULL, which is odd.
 
     In several spatial operations IIF statements are used to avoid this behaviour.
     """
```

### Comparing `geofileops-0.8.0a7/tests/test_sqlite_util.py` & `geofileops-0.8.0a8/tests/test_sqlite_util.py`

 * *Files identical despite different names*

