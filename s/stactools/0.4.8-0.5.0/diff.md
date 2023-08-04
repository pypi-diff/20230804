# Comparing `tmp/stactools-0.4.8.tar.gz` & `tmp/stactools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-0.4.8.tar", last modified: Thu Jun  1 15:10:00 2023, max compression
+gzip compressed data, was "stactools-0.5.0.tar", last modified: Fri Aug  4 19:51:59 2023, max compression
```

## Comparing `stactools-0.4.8.tar` & `stactools-0.5.0.tar`

### file list

```diff
@@ -1,63 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.200767 stactools-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-01 15:09:38.000000 stactools-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-06-01 15:10:00.200767 stactools-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-01 15:09:38.000000 stactools-0.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-01 15:09:38.000000 stactools-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 15:10:00.200767 stactools-0.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.192767 stactools-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.192767 stactools-0.4.8/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.192767 stactools-0.4.8/src/stactools/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.196767 stactools-0.4.8/src/stactools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/add_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/add_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/update_extent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/update_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.196767 stactools-0.4.8/src/stactools/core/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/add_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/add_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.196767 stactools-0.4.8/src/stactools/core/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/io/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/projection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.200767 stactools-0.4.8/src/stactools/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/utils/antimeridian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    40585 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/utils/raster_footprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/utils/round.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/utils/subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.200767 stactools-0.4.8/src/stactools/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/testing/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/testing/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.192767 stactools-0.4.8/src/stactools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-06-01 15:10:00.000000 stactools-0.4.8/src/stactools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-01 15:10:00.000000 stactools-0.4.8/src/stactools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:10:00.000000 stactools-0.4.8/src/stactools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 15:10:00.000000 stactools-0.4.8/src/stactools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-01 15:10:00.000000 stactools-0.4.8/src/stactools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 15:10:00.000000 stactools-0.4.8/src/stactools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:59.377147 stactools-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-08-04 19:51:42.000000 stactools-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-04 19:51:42.000000 stactools-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-08-04 19:51:59.377147 stactools-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-08-04 19:51:42.000000 stactools-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-08-04 19:51:43.000000 stactools-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 19:51:59.377147 stactools-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:59.373147 stactools-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:59.373147 stactools-0.5.0/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:59.373147 stactools-0.5.0/src/stactools/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:59.377147 stactools-0.5.0/src/stactools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/add_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/add_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/update_extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/update_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/cli/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:59.377147 stactools-0.5.0/src/stactools/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/add_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/add_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:59.377147 stactools-0.5.0/src/stactools/core/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/io/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:59.377147 stactools-0.5.0/src/stactools/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/utils/antimeridian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43162 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/utils/raster_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/utils/round.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/core/utils/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:59.377147 stactools-0.5.0/src/stactools/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/testing/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/testing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-08-04 19:51:43.000000 stactools-0.5.0/src/stactools/testing/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:51:59.373147 stactools-0.5.0/src/stactools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9258 2023-08-04 19:51:59.000000 stactools-0.5.0/src/stactools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-04 19:51:59.000000 stactools-0.5.0/src/stactools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:51:59.000000 stactools-0.5.0/src/stactools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-04 19:51:59.000000 stactools-0.5.0/src/stactools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-04 19:51:59.000000 stactools-0.5.0/src/stactools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 19:51:59.000000 stactools-0.5.0/src/stactools.egg-info/top_level.txt
```

### Comparing `stactools-0.4.8/LICENSE` & `stactools-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/PKG-INFO` & `stactools-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools
-Version: 0.4.8
+Version: 0.5.0
 Summary: Command line tool and Python library for working with STAC
 Author-email: Rob Emanuele <rdemanuele@gmail.com>, Pete Gadomski <pete.gadomski@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/stactools
 Project-URL: documentation, https://stactools.readthedocs.io/
 Project-URL: repository, https://github.com/stac-utils/stactools.git
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: s3
 License-File: LICENSE
 
 # stactools
 
 ![Build Status](https://github.com/stac-utils/stactools/workflows/CI/badge.svg)
 [![Documentation](https://readthedocs.org/projects/stactools/badge/?version=latest)](https://stactools.readthedocs.io/en/latest/)
@@ -228,15 +229,15 @@
 
 ```sh
 pip install -e '.[dev]'
 ```
 
 ### Developing the docs
 
-To build and serve the docs, the development requirements must be installed with `pip install -e '.[dev]'`.
+To build and serve the docs, the development requirements must be installed with `pip install -e '.[docs]'`.
 To build the docs, you can use `make html` from inside of the docs directory, and to build the docs and start a server that watches for changes, use `make livehtml`:
 
 ```sh
 cd docs
 make html
 make livehtml
 ```
```

### Comparing `stactools-0.4.8/README.md` & `stactools-0.5.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -203,15 +203,15 @@
 
 ```sh
 pip install -e '.[dev]'
 ```
 
 ### Developing the docs
 
-To build and serve the docs, the development requirements must be installed with `pip install -e '.[dev]'`.
+To build and serve the docs, the development requirements must be installed with `pip install -e '.[docs]'`.
 To build the docs, you can use `make html` from inside of the docs directory, and to build the docs and start a server that watches for changes, use `make livehtml`:
 
 ```sh
 cd docs
 make html
 make livehtml
 ```
```

### Comparing `stactools-0.4.8/pyproject.toml` & `stactools-0.5.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -21,25 +21,23 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "Shapely>=1.8.5.post1",
-    "aiohttp>=3.8.3",
     "antimeridian>=0.2.6",
     "click>=8.1.3",
-    "fsspec>=2021.7",
+    "fsspec[http]>=2021.7",
     "lxml>=4.9.2",
-    "numpy>=1.22.0",
+    "numpy>=1.23.0",
     "pyproj>=3.3",
-    "pystac[validation]>=1.6.1",
+    "pystac[validation]>=1.8.2",
     "rasterio>=1.3.2",
-    "requests>=2.27.1",
+    "shapely>=2.0.1",
     "stac-check>=1.3.2",
     "stac-validator>=3.1.0",
 ]
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://github.com/stac-utils/stactools"
@@ -52,35 +50,38 @@
 stac = "stactools.cli.cli:run_cli"
 
 [project.optional-dependencies]
 dev = [
     "black~=23.3",
     "codespell~=2.2",
     "importlib-metadata~=6.6",
-    "ipython~=8.12",
-    "jupyter~=1.0",
     "lxml-stubs~=0.4",
     "mypy~=1.3",
-    "nbsphinx~=0.9",
     "packaging~=23.1",
     "pre-commit~=3.3",
-    "pydata-sphinx-theme~=0.13",
     "pylint~=2.17",
-    "pytest~=7.3",
     "pytest-cov~=3.0",
+    "pytest~=7.3",
+    "requests>=2.27.1",
     "ruff==0.0.265",
-    "sphinx~=7.0",
-    "sphinx-autobuild==2021.3.14",
-    "sphinx-click~=4.4",
-    "sphinxcontrib-napoleon~=0.7",
     "types-certifi~=2021.10.8",
     "types-orjson~=3.6",
     "types-python-dateutil~=2.8",
     "types-requests~=2.30",
 ]
+docs = [
+    "ipython~=8.12",
+    "jupyter~=1.0",
+    "nbsphinx~=0.9",
+    "pydata-sphinx-theme~=0.13",
+    "sphinx~=7.0",
+    "sphinx-autobuild==2021.3.14",
+    "sphinx-click~=4.4",
+    "sphinxcontrib-fulltoc~=1.2",
+]
 s3 = ["s3fs>=2021.7"]
 
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
```

### Comparing `stactools-0.4.8/src/stactools/cli/__init__.py` & `stactools-0.5.0/src/stactools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/cli/cli.py` & `stactools-0.5.0/src/stactools/cli/cli.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/cli/commands/add.py` & `stactools-0.5.0/src/stactools/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/cli/commands/add_asset.py` & `stactools-0.5.0/src/stactools/cli/commands/add_asset.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 from typing import List, Optional
 
 import click
 import pystac
 import pystac.utils
-from stactools.core import add_asset_to_item
+from stactools.core import add_asset
 
 
 def _add_asset(
-    item_path: str,
+    owner_path: str,
     asset_key: str,
     asset_path: str,
     title: Optional[str] = None,
     description: Optional[str] = None,
     media_type: Optional[str] = None,
     roles: Optional[List[str]] = None,
     move_assets: bool = False,
     ignore_conflicts: bool = False,
 ) -> None:
-    item = pystac.read_file(item_path)
-    if not isinstance(item, pystac.Item):
-        raise click.BadArgumentUsage(f"{item_path} is not a STAC Item")
+    owner = pystac.read_file(owner_path)
+    if not isinstance(owner, (pystac.Item, pystac.Collection)):
+        raise click.BadArgumentUsage(f"{owner_path} is not a STAC Item or Collection")
     asset = pystac.Asset(asset_path, title, description, media_type, roles)
-    item = add_asset_to_item(
-        item,
+    owner = add_asset(
+        owner,
         asset_key,
         asset,
         move_assets=move_assets,
         ignore_conflicts=ignore_conflicts,
     )
-    item.save_object()
+    owner.save_object()
 
 
 def create_add_asset_command(cli: click.Group) -> click.Command:
-    @cli.command("add-asset", short_help="Add an asset to an item.")
-    @click.argument("item_path")
+    @cli.command("add-asset", short_help="Add an asset to an item or collection.")
+    @click.argument("owner_path")
     @click.argument("asset_key")
     @click.argument("asset_path")
     @click.option("--title", help="Optional title of the asset")
     @click.option(
         "--description",
         help=(
             "Optional description of the asset providing additional details, "
@@ -51,38 +51,38 @@
         "roles",
         help="Optional, semantic roles of the asset",
         multiple=True,
     )
     @click.option(
         "--move-assets",
         is_flag=True,
-        help="Move asset to the target Item's location.",
+        help="Move asset to the target Item or Collection's location.",
     )
     @click.option(
         "--ignore-conflicts",
         is_flag=True,
         help=(
             "If there already exists an asset with the given key or at the "
             "target path (when `--move-assets` flag is set), do not raise an "
             "error, leave the original asset from the target item in place."
         ),
     )
     def add_asset_command(
-        item_path: str,
+        owner_path: str,
         asset_key: str,
         asset_path: str,
         title: Optional[str] = None,
         description: Optional[str] = None,
         media_type: Optional[str] = None,
         roles: Optional[List[str]] = None,
         move_assets: bool = False,
         ignore_conflicts: bool = False,
     ) -> None:
         _add_asset(
-            pystac.utils.make_absolute_href(item_path),
+            pystac.utils.make_absolute_href(owner_path),
             asset_key,
             pystac.utils.make_absolute_href(asset_path),
             title,
             description,
             media_type,
             roles,
             move_assets=move_assets,
```

### Comparing `stactools-0.4.8/src/stactools/cli/commands/add_raster.py` & `stactools-0.5.0/src/stactools/cli/commands/add_raster.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/cli/commands/copy.py` & `stactools-0.5.0/src/stactools/cli/commands/copy.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 import pystac
 from pystac.utils import make_absolute_href
 from stactools.core.copy import copy_catalog, move_all_assets
 
 
 def create_move_assets_command(cli: click.Group) -> click.Command:
     @cli.command(
-        "move-assets", short_help="Move or copy assets in a STAC to the Item locations."
+        "move-assets",
+        help=(
+            "Move or copy assets in a STAC catalog to the locations of the "
+            "items or collections that own them."
+        ),
     )
     @click.argument("catalog_path")
     @click.option("-c", "--copy", help="Copy assets instead of moving.", is_flag=True)
     @click.option(
         "-s",
         "--asset-subdirectory",
         help=(
@@ -64,15 +68,15 @@
             case_sensitive=False,
         ),
     )
     @click.option(
         "--copy-assets",
         "-a",
         is_flag=True,
-        help="Copy all item assets to be alongside the new item location.",
+        help="Copy all asset files to be alongside the new location.",
     )
     @click.option(
         "-l",
         "--publish-location",
         help=(
             "Location to use for resolving HREF links "
             "instead of the destination folder."
```

### Comparing `stactools-0.4.8/src/stactools/cli/commands/create.py` & `stactools-0.5.0/src/stactools/cli/commands/create.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 import json
 import sys
+from typing import List
 
 import click
 from stactools.core import create
 
 
 def create_create_item_command(cli: click.Group) -> click.Command:
     @cli.command("create-item", short_help="Creates an item from an asset")
     @click.argument("href")
-    def create_item_command(href: str) -> None:
+    @click.argument("asset_key", default="data")
+    @click.option(
+        "-r",
+        "--role",
+        "roles",
+        help="Optional, semantic roles of the asset",
+        multiple=True,
+        default=["data"],
+    )
+    def create_item_command(href: str, asset_key: str, roles: List[str]) -> None:
         """Creates an Item from a href.
 
         The href must be a `rasterio` readable asset. The item's dictionary will
         be printed to stdout. This item is intentinonally _extremely_ minimal.
         If you need additional capabilities, we recommend using [rio
         stac](https://github.com/developmentseed/rio-stac/).
         """
-        item = create.item(href)
+        item = create.item(href, asset_key=asset_key, roles=roles)
         json.dump(item.to_dict(), sys.stdout)
 
     return create_item_command
```

### Comparing `stactools-0.4.8/src/stactools/cli/commands/info.py` & `stactools-0.5.0/src/stactools/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/cli/commands/layout.py` & `stactools-0.5.0/src/stactools/cli/commands/layout.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/cli/commands/lint.py` & `stactools-0.5.0/src/stactools/cli/commands/lint.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/cli/commands/merge.py` & `stactools-0.5.0/src/stactools/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/cli/commands/summary.py` & `stactools-0.5.0/src/stactools/cli/commands/summary.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/cli/commands/update_extent.py` & `stactools-0.5.0/src/stactools/cli/commands/update_extent.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/cli/commands/update_geometry.py` & `stactools-0.5.0/src/stactools/cli/commands/update_geometry.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/cli/commands/validate.py` & `stactools-0.5.0/src/stactools/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/cli/commands/version.py` & `stactools-0.5.0/src/stactools/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/cli/registry.py` & `stactools-0.5.0/src/stactools/cli/registry.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/core/__init__.py` & `stactools-0.5.0/src/stactools/core/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 from stactools.core.add import add_item
-from stactools.core.add_asset import add_asset_to_item
+from stactools.core.add_asset import add_asset, add_asset_to_item
 from stactools.core.add_raster import add_raster_to_item
 from stactools.core.copy import (
     copy_catalog,
     move_all_assets,
+    move_asset_file,
     move_asset_file_to_item,
     move_assets,
 )
 from stactools.core.io import use_fsspec
 from stactools.core.layout import layout_catalog
 from stactools.core.merge import merge_all_items, merge_items
 
 __all__ = [
     "add_item",
+    "add_asset",
     "add_asset_to_item",
     "add_raster_to_item",
     "copy_catalog",
     "layout_catalog",
     "merge_all_items",
     "merge_items",
+    "move_asset_file",
     "move_asset_file_to_item",
     "move_assets",
     "move_all_assets",
     "use_fsspec",
 ]
-__version__ = "0.4.8"
+__version__ = "0.5.0"
```

### Comparing `stactools-0.4.8/src/stactools/core/add.py` & `stactools-0.5.0/src/stactools/core/add.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/core/add_asset.py` & `stactools-0.5.0/src/stactools/core/add_asset.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,99 @@
 import logging
+import warnings
+from typing import Union, cast
 
-from pystac import Asset, Item
+from pystac import Asset, Collection, Item
 from pystac.utils import is_absolute_href, make_relative_href
-from stactools.core.copy import move_asset_file_to_item
+from stactools.core.copy import move_asset_file
 
 logger = logging.getLogger(__name__)
 
 
-def add_asset_to_item(
-    item: Item,
+def add_asset(
+    owner: Union[Collection, Item],
     key: str,
     asset: Asset,
     move_assets: bool = False,
     ignore_conflicts: bool = False,
-) -> Item:
-    """Adds an asset to an item.
+) -> Union[Collection, Item]:
+    """Adds an asset to an item or collection.
 
     Args:
-        item (Item): The PySTAC Item to which the asset will be added.
+        owner (Item or Collection): The PySTAC Item or Collecitonto which the asset
+            will be added.
         key (str): The unique key of the asset.
         asset (Asset): The PySTAC Asset to add.
-        move_assets (bool): If True, move the asset file alongside the target item.
+        move_assets (bool): If True, move the asset file alongside the target owner.
         ignore_conflicts (bool): If True, asset with the same key will not be added,
             and asset file that would overwrite an existing file will not be moved.
             If False, either of these situations will throw an error.
 
     Returns:
-        Item: Returns an updated Item with the added Asset.
-            This operation mutates the Item.
+        owner: Returns an updated Item or Collection with the added Asset.
+            This operation mutates the owner.
     """
-    item_href = item.get_self_href()
+    owner_href = owner.get_self_href()
     asset_href = asset.get_absolute_href()
-    if key in item.assets:
+    if key in owner.assets:
         if not ignore_conflicts:
             raise Exception(
-                f"Target item {item} already has an asset with key {key}, "
+                f"Target {owner} already has an asset with key {key}, "
                 "cannot add asset in from {asset_href}"
             )
     else:
         if not asset_href:
             raise ValueError(
                 f"Asset {asset} must have an href to be added. The href "
                 "value should be an absolute path or URL."
             )
-        if not item_href and move_assets:
+        if not owner_href and move_assets:
+            raise ValueError(f"Target {owner} must have an href to move an asset to it")
+        if not owner_href and not is_absolute_href(asset.href):
             raise ValueError(
-                f"Target Item {item} must have an href to move an asset to the item"
-            )
-        if not item_href and not is_absolute_href(asset.href):
-            raise ValueError(
-                f"Target Item {item} must have an href to add "
+                f"Target {owner} must have an href to add "
                 "an asset with a relative href"
             )
         if move_assets:
-            new_asset_href = move_asset_file_to_item(
-                item, asset_href, ignore_conflicts=ignore_conflicts
+            new_asset_href = move_asset_file(
+                owner, asset_href, ignore_conflicts=ignore_conflicts
             )
         else:
-            if not is_absolute_href(asset.href) and item_href is not None:
-                asset_href = make_relative_href(asset_href, item_href)
+            if not is_absolute_href(asset.href) and owner_href is not None:
+                asset_href = make_relative_href(asset_href, owner_href)
             new_asset_href = asset_href
         asset.href = new_asset_href
-        item.add_asset(key, asset)
-    return item
+        owner.add_asset(key, asset)
+    return owner
+
+
+def add_asset_to_item(
+    item: Item,
+    key: str,
+    asset: Asset,
+    move_assets: bool = False,
+    ignore_conflicts: bool = False,
+) -> Item:
+    """Adds an asset to an item.
+
+    Args:
+        item (Item): The PySTAC Item to which the asset will be added.
+        key (str): The unique key of the asset.
+        asset (Asset): The PySTAC Asset to add.
+        move_assets (bool): If True, move the asset file alongside the target item.
+        ignore_conflicts (bool): If True, asset with the same key will not be added,
+            and asset file that would overwrite an existing file will not be moved.
+            If False, either of these situations will throw an error.
+
+    Returns:
+        Item: Returns an updated Item with the added Asset.
+            This operation mutates the Item.
+    """
+    warnings.warn(
+        "'add_asset_to_item' is deprecated. Use 'add_asset' instead", DeprecationWarning
+    )
+    return cast(
+        Item,
+        add_asset(
+            item, key, asset, move_assets=move_assets, ignore_conflicts=ignore_conflicts
+        ),
+    )
```

### Comparing `stactools-0.4.8/src/stactools/core/add_raster.py` & `stactools-0.5.0/src/stactools/core/add_raster.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/core/copy.py` & `stactools-0.5.0/src/stactools/core/copy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 import logging
 import os
-from typing import Optional
+import warnings
+from typing import Optional, Union
 
 import fsspec
 from fsspec.core import split_protocol
 from fsspec.registry import get_filesystem_class
-from pystac import Catalog, CatalogType, Item
+from pystac import Catalog, CatalogType, Collection, Item
 from pystac.utils import is_absolute_href, make_absolute_href, make_relative_href
 
 logger = logging.getLogger(__name__)
 
 
-def move_asset_file_to_item(
-    item: Item,
+def move_asset_file(
+    owner: Union[Item, Collection],
     asset_href: str,
     asset_subdirectory: Optional[str] = None,
     copy: bool = False,
     ignore_conflicts: bool = False,
 ) -> str:
-    """Moves an asset file to be alongside an item.
+    """Moves an asset file to be alongside its owner.
 
     Args:
-        item (Item):
-            The PySTAC Item to perform the asset transformation on.
+        owner (Item or Collection):
+            The PySTAC Item or Collection to perform the asset transformation on.
         asset_href (str): The absolute HREF to the asset file.
         asset_subdirectory (str or None):
             A subdirectory that will be used to store the assets. If not
             supplied, the assets will be moved or copied to the same directory
-            as their item.
+            as their owner.
         copy (bool):
             If False this function will move the asset file; if True, the asset
             file will be copied.
         ignore_conflicts (bool):
             If the asset destination file already exists, this function will
             throw an error unless ignore_conflicts is True.
 
     Returns:
         str: The new absolute href for the asset file.
     """
-    item_href = item.get_self_href()
-    if item_href is None:
+    owner_href = owner.get_self_href()
+    if owner_href is None:
         raise ValueError(
-            f"Self HREF is not available for item {item.id}. This operation "
-            "requires that the Item HREFs are available."
+            f"Self HREF is not available for {owner}. This operation "
+            "requires that the HREFs are available."
         )
 
     # TODO this shouldn't have to be absolute
     if not is_absolute_href(asset_href):
         raise ValueError("asset_href must be absolute.")
 
-    item_dir = os.path.dirname(item_href)
+    owner_dir = os.path.dirname(owner_href)
 
     fname = os.path.basename(asset_href)
     if asset_subdirectory is None:
-        target_dir = item_dir
+        target_dir = owner_dir
     else:
-        target_dir = os.path.join(item_dir, asset_subdirectory)
+        target_dir = os.path.join(owner_dir, asset_subdirectory)
     new_asset_href = os.path.join(target_dir, fname)
 
     if asset_href != new_asset_href:
         dest_protocol = split_protocol(new_asset_href)[0]
         fs_dest = get_filesystem_class(dest_protocol)()
         op = None
 
@@ -116,26 +117,61 @@
 
         if op is not None:
             op(dry_run=False)
 
     return new_asset_href
 
 
-def move_assets(
+def move_asset_file_to_item(
     item: Item,
+    asset_href: str,
     asset_subdirectory: Optional[str] = None,
-    make_hrefs_relative: bool = True,
     copy: bool = False,
     ignore_conflicts: bool = False,
-) -> Item:
-    """Moves an Item's assets to be alongside that item.
+) -> str:
+    """Moves an asset file to be alongside an item.
 
     Args:
         item (Item):
             The PySTAC Item to perform the asset transformation on.
+        asset_href (str): The absolute HREF to the asset file.
+        asset_subdirectory (str or None):
+            A subdirectory that will be used to store the assets. If not
+            supplied, the assets will be moved or copied to the same directory
+            as their item.
+        copy (bool):
+            If False this function will move the asset file; if True, the asset
+            file will be copied.
+        ignore_conflicts (bool):
+            If the asset destination file already exists, this function will
+            throw an error unless ignore_conflicts is True.
+
+    Returns:
+        str: The new absolute href for the asset file.
+    """
+    warnings.warn(
+        "'move_asset_file_to_item' is deprecated. Use 'move_asset_file' instead",
+        DeprecationWarning,
+    )
+    return move_asset_file(item, asset_href, asset_subdirectory, copy, ignore_conflicts)
+
+
+def move_assets(
+    owner: Optional[Union[Item, Collection]] = None,
+    asset_subdirectory: Optional[str] = None,
+    make_hrefs_relative: bool = True,
+    copy: bool = False,
+    ignore_conflicts: bool = False,
+    item: Optional[Item] = None,
+) -> Union[Item, Collection]:
+    """Moves an Item or Collection's assets to be alongside it.
+
+    Args:
+        owner (Item or Collection):
+            The PySTAC Item or Collection to perform the asset transformation on.
         asset_subdirectory (str or None):
             A subdirectory that will be used to store the assets. If not
             supplied, the assets will be moved or copied to the same directory
             as the item.
         make_assets_relative (bool):
             If True, will make the asset HREFs relative to the assets. If false,
             the asset will be an absolute href. Defaults to True.
@@ -144,66 +180,73 @@
             the asset file will be copied.
         ignore_conflicts (bool):
             If the asset destination file already exists, this function will
             throw an error unless ignore_conflicts is True.
 
     Returns:
         Item:
-            Returns an updated catalog or collection.  This operation mutates
+            Returns an updated item or collection.  This operation mutates
             the Item.
     """
-    item_href = item.get_self_href()
-    if item_href is None:
+    if item is not None:
+        warnings.warn(
+            "item is a deprecated option on this function. Use 'owner' instead",
+            DeprecationWarning,
+        )
+        owner = item
+    if owner is None:
+        raise TypeError("move_assets missing 1 required positional argument: 'owner'")
+
+    owner_href = owner.get_self_href()
+    if owner_href is None:
         raise ValueError(
-            f"Self HREF is not available for item {item.id}. This operation "
-            "requires that the Item HREFs are available."
+            f"Self HREF is not available for {owner}. This operation "
+            "requires that HREFs are available."
         )
 
-    for asset in item.assets.values():
+    for asset in owner.assets.values():
         abs_asset_href = asset.get_absolute_href()
         if abs_asset_href is None:
             raise ValueError(
-                f"Asset {asset.title} HREF is not available for item {item.id}. "
-                "This operation "
-                "requires that the Asset HREFs are available."
+                f"Asset {asset.title} HREF is not available for {owner}. "
+                "This operation requires that the Asset HREFs are available."
             )
-
-        new_asset_href = move_asset_file_to_item(
-            item,
+        new_asset_href = move_asset_file(
+            owner,
             abs_asset_href,
             asset_subdirectory=asset_subdirectory,
             copy=copy,
             ignore_conflicts=ignore_conflicts,
         )
 
         if make_hrefs_relative:
-            asset.href = make_relative_href(new_asset_href, item_href)
+            asset.href = make_relative_href(new_asset_href, owner_href)
         else:
             asset.href = new_asset_href
 
-    return item
+    return owner
 
 
 def move_all_assets(
     catalog: Catalog,
     asset_subdirectory: Optional[str] = None,
     make_hrefs_relative: bool = True,
     copy: bool = False,
     ignore_conflicts: bool = False,
 ) -> Catalog:
-    """Moves assets in a catalog to be alongside the items that own them.
+    """Moves assets in a catalog to be alongside the item or collections that own them.
 
     Args:
         catalog (Catalog or Collection):
             The PySTAC Catalog or Collection to perform the asset transformation
             on.
         asset_subdirectory (str or None):
             A subdirectory that will be used to store the assets. If not
             supplied, the assets will be moved or copied to the same directory
-            as their item.
+            as their owner.
         make_assets_relative (bool):
             If True, will make the asset HREFs relative to the assets. If false,
             the asset will be an absolute href.
         copy (bool):
             If False this function will move the asset file; if True, the asset
             file will be copied.
         ignore_conflicts (bool):
@@ -217,14 +260,19 @@
     """
 
     for item in catalog.get_all_items():
         move_assets(
             item, asset_subdirectory, make_hrefs_relative, copy, ignore_conflicts
         )
 
+    for collection in catalog.get_all_collections():
+        move_assets(
+            collection, asset_subdirectory, make_hrefs_relative, copy, ignore_conflicts
+        )
+
     return catalog
 
 
 def copy_catalog(
     source_catalog: Catalog,
     dest_directory: str,
     catalog_type: Optional[CatalogType] = None,
@@ -235,16 +283,17 @@
     if resolve_links:
         catalog = source_catalog.full_copy()
     else:
         catalog = source_catalog.clone()
         catalog.set_root(catalog)
 
     dest_directory = make_absolute_href(dest_directory)
-
     if copy_assets:
+        catalog.make_all_asset_hrefs_absolute()
+        catalog.normalize_hrefs(dest_directory, skip_unresolved=not resolve_links)
         catalog = move_all_assets(catalog, copy=True, make_hrefs_relative=True)
 
     if publish_location is not None:
         catalog.normalize_hrefs(publish_location, skip_unresolved=not resolve_links)
         catalog.save(catalog_type, dest_directory)
     else:
         catalog.normalize_hrefs(dest_directory, skip_unresolved=not resolve_links)
```

### Comparing `stactools-0.4.8/src/stactools/core/create.py` & `stactools-0.5.0/src/stactools/core/create.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 import datetime
 import os.path
-from typing import Optional
+from typing import List, Optional
 
 import rasterio
 import shapely.geometry
 import stactools.core.projection
 from pystac import Asset, Item
 from pystac.extensions.projection import ProjectionExtension
 
 from .io import ReadHrefModifier
 
 
-def item(href: str, read_href_modifier: Optional[ReadHrefModifier] = None) -> Item:
+def item(
+    href: str,
+    *,
+    asset_key: str = "data",
+    roles: List[str] = ["data"],
+    read_href_modifier: Optional[ReadHrefModifier] = None,
+) -> Item:
     """Creates a STAC Item from the asset at the provided href.
 
     The ``read_href_modifer`` argument can be used to modify the href for the
     rasterio read, e.g. if you need to sign a url.
 
     This function is intentionally minimal in its signature and capabilities. If
     you need to customize your Item, do so after creation.
 
     Args:
         href (str): The href of the asset that will be used to create the item.
+        asset_key (str): The unique key of the asset
+        roles (List[str]): The semantic roles of the asset
         read_href_modifier (Optional[ReadHrefModifier]):
             An optional callable that will be used to modify the href before reading.
 
     Returns:
         pystac.Item: A PySTAC Item.
     """
     id = os.path.splitext(os.path.basename(href))[0]
@@ -34,32 +42,32 @@
     else:
         modified_href = href
     with rasterio.open(modified_href) as dataset:
         crs = dataset.crs
         proj_bbox = dataset.bounds
         proj_transform = list(dataset.transform)[0:6]
         proj_shape = dataset.shape
-    proj_geometry = shapely.geometry.mapping(shapely.geometry.box(*proj_bbox))
-    geometry = stactools.core.projection.reproject_geom(
-        crs, "EPSG:4326", proj_geometry, precision=6
+    geom = stactools.core.projection.reproject_shape(
+        crs, "EPSG:4326", shapely.geometry.box(*proj_bbox), precision=6
     )
-    bbox = list(shapely.geometry.shape(geometry).bounds)
+    bbox = list(geom.bounds)
+    geojson = shapely.geometry.mapping(geom)
     item = Item(
         id=id,
-        geometry=geometry,
+        geometry=geojson,
         bbox=bbox,
         datetime=datetime.datetime.now(),
         properties={},
     )
 
     projection = ProjectionExtension.ext(item, add_if_missing=True)
     epsg = crs.to_epsg()
     if epsg:
         projection.epsg = epsg
     else:
         projection.wkt2 = crs.to_wkt("WKT2")
     projection.transform = proj_transform
     projection.shape = proj_shape
 
-    item.add_asset("data", Asset(href=href, roles=["data"]))
+    item.add_asset(asset_key, Asset(href=href, roles=roles))
 
     return item
```

### Comparing `stactools-0.4.8/src/stactools/core/io/__init__.py` & `stactools-0.5.0/src/stactools/core/io/__init__.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/core/io/xml.py` & `stactools-0.5.0/src/stactools/core/io/xml.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/core/layout.py` & `stactools-0.5.0/src/stactools/core/layout.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/core/merge.py` & `stactools-0.5.0/src/stactools/core/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from typing import Optional
 
 import pystac
 from pystac.layout import BestPracticesLayoutStrategy
 from pystac.utils import is_absolute_href, make_relative_href
 from shapely.geometry import mapping, shape
-from stactools.core.copy import copy_catalog, move_asset_file_to_item
+from stactools.core.copy import copy_catalog, move_asset_file
 from stactools.core.copy import move_assets as do_move_assets
 
 
 def merge_items(
     source_item: pystac.Item,
     target_item: pystac.Item,
     move_assets: bool = False,
@@ -47,15 +47,15 @@
                     )
                 )
         else:
             asset_href = asset.get_absolute_href()
             if asset_href is None:
                 raise ValueError(f"Asset {asset.title} must have an HREF for merge")
             if move_assets:
-                new_asset_href = move_asset_file_to_item(
+                new_asset_href = move_asset_file(
                     target_item, asset_href, ignore_conflicts=ignore_conflicts
                 )
             else:
                 if not is_absolute_href(asset.href):
                     asset_href = make_relative_href(asset_href, target_item_href)
                 new_asset_href = asset_href
             new_asset = asset.clone()
```

### Comparing `stactools-0.4.8/src/stactools/core/projection.py` & `stactools-0.5.0/src/stactools/core/projection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,20 @@
-from copy import deepcopy
-from typing import Any, Dict, List, Optional, Sequence, Union
+import json
+import warnings
+from typing import Any, Dict, List, Optional, Union, cast
 
 import pyproj
 import rasterio.crs
 import rasterio.transform
+from rasterio.warp import transform_geom
+from shapely import Geometry
+from shapely.constructive import remove_repeated_points
+from shapely.geometry import mapping, shape
+
+from .geometry import GeoInterface
 
 
 def epsg_from_utm_zone_number(utm_zone_number: int, south: bool) -> int:
     """Returns the EPSG code for a UTM zone number.
 
     Args:
         utm_zone_number (int): The UTM zone number.
@@ -17,54 +24,76 @@
         int: The EPSG code number for the UTM zone.
     """
     crs = pyproj.CRS.from_dict({"proj": "utm", "zone": utm_zone_number, "south": south})
 
     return int(crs.to_authority()[1])
 
 
+def reproject_shape(
+    src_crs: rasterio.crs.CRS,
+    dst_crs: rasterio.crs.CRS,
+    geom: GeoInterface,
+    precision: Optional[int] = None,
+) -> Geometry:
+    """Projects a shapely.Geometry and rounds the projected vertex coordinates
+    to ``precision``.
+
+    Duplicate points caused by rounding are removed.
+
+    Args:
+        src_crs (rasterio.crs.CRS): The CRS of the input geometry.
+        dst_crs (rasterio.crs.CRS): The CRS of the output geometry.
+        geom (GeoInterface): GeoJSON like dict or shapely geometry object to reproject
+        precision (int): The number of decimal places to include in the final
+            Geometry vertex coordinates.
+
+    Returns:
+        geom: the reprojected shapely geometry object
+    """
+    return remove_repeated_points(
+        shape(transform_geom(src_crs, dst_crs, geom, precision=precision))
+    )
+
+
 def reproject_geom(
     src_crs: Union[pyproj.CRS, rasterio.crs.CRS, str],
     dest_crs: Union[pyproj.CRS, rasterio.crs.CRS, str],
     geom: Dict[str, Any],
     precision: Optional[int] = None,
 ) -> Dict[str, Any]:
-    """Reprojects a geometry represented as GeoJSON from the src_crs to the
+    """DEPRECATED.
+
+    .. deprecated:: 0.5.0
+        Use :func:`reproject_shape` instead.
+
+    Reprojects a geometry represented as GeoJSON from the src_crs to the
     dest crs.
 
     Args:
         src_crs (pyproj.crs.CRS, rasterio.crs.CRS, or str): Projection of input data.
         dest_crs (pyproj.crs.CRS, rasterio.crs.CRS, or str): Projection of output data.
         geom (dict): The GeoJSON geometry
         precision (int, optional): The precision of the reprojection operation.
 
     Returns:
         dict: The reprojected geometry
     """
-    transformer = pyproj.Transformer.from_crs(src_crs, dest_crs, always_xy=True)
-    result = deepcopy(geom)
-
-    def fn(coords: Sequence[Any]) -> Sequence[Any]:
-        coords = list(coords)
-        for i in range(0, len(coords)):
-            coord = coords[i]
-            if isinstance(coord[0], Sequence):
-                coords[i] = fn(coord)
-            else:
-                x, y = coord
-                reprojected_coords = list(transformer.transform(x, y, errcheck=True))
-                if precision is not None:
-                    reprojected_coords = [
-                        round(n, precision) for n in reprojected_coords
-                    ]
-                coords[i] = reprojected_coords
-        return coords
-
-    result["coordinates"] = fn(result["coordinates"])
-
-    return result
+    warnings.warn(
+        "``reproject_geom`` is deprecated and will be removed in v0.6.0. "
+        "Use ``reproject_shape`` instead.",
+        DeprecationWarning,
+    )
+    return cast(
+        Dict[str, Any],
+        json.loads(
+            json.dumps(
+                mapping(reproject_shape(src_crs, dest_crs, shape(geom), precision))
+            )
+        ),
+    )
 
 
 def transform_from_bbox(bbox: List[float], shape: List[int]) -> List[float]:
     """Calculate the affine transformation from the bbox and shape.
 
     Only take the first 6 elements, as that is all that is necessary.
```

### Comparing `stactools-0.4.8/src/stactools/core/utils/__init__.py` & `stactools-0.5.0/src/stactools/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/core/utils/antimeridian.py` & `stactools-0.5.0/src/stactools/core/utils/antimeridian.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/core/utils/convert.py` & `stactools-0.5.0/src/stactools/core/utils/convert.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/core/utils/raster_footprint.py` & `stactools-0.5.0/src/stactools/core/utils/raster_footprint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,51 @@
 """Generate convex hulls of valid raster data for use in STAC Item
 geometries."""
 
 import logging
 import warnings
-from itertools import groupby
+from enum import Enum, auto
 from typing import Any, Dict, Iterator, List, Optional, Tuple, Type, TypeVar, Union
 
 import numpy as np
 import numpy.typing as npt
 import rasterio
 import rasterio.features
 from pystac import Item
 from rasterio import Affine, DatasetReader
 from rasterio.crs import CRS
-from rasterio.warp import transform_geom
 from shapely.geometry import mapping, shape
 from shapely.geometry.multipolygon import MultiPolygon
 from shapely.geometry.polygon import Polygon, orient
+from shapely.ops import unary_union
+from stactools.core.geometry import mutual_intersection
+
+from ..projection import reproject_shape
 
 logger = logging.getLogger(__name__)
 
 # Roughly 1 centimeter in geodetic coordinates
 DEFAULT_PRECISION = 7
 
 T = TypeVar("T", bound="RasterFootprint")
 
 
+class FootprintMergeStrategy(Enum):
+    """Strategy for handling the aggregation of differing asset footprints."""
+
+    FIRST = auto()
+    """Use the footprint of the first matching asset."""
+
+    UNION = auto()
+    """Union the geometries of all matching assets."""
+
+    INTERSECTION = auto()
+    """Use the mutual intersection of all matching asset footprints."""
+
+
 def densify_by_factor(
     point_list: List[Tuple[float, float]], factor: int
 ) -> List[Tuple[float, float]]:
     """Densifies the number of points in a list of points by a ``factor``. For
     example, a list of 5 points and a factor of 2 will result in 10 points (one
     new point between each original adjacent points).
 
@@ -90,79 +106,91 @@
         )
     final_point = points[-1].reshape(1, -1)
     densified_array = np.concatenate((*densified_points, final_point), axis=0)
     return [(float(row[0]), float(row[1])) for row in densified_array]
 
 
 def reproject_polygon(
-    polygon: Polygon, crs: CRS, precision: Optional[int] = DEFAULT_PRECISION
+    polygon: Polygon,
+    crs: CRS,
+    precision: Optional[int] = DEFAULT_PRECISION,
+    dst_crs: CRS = "EPSG:4326",
 ) -> Polygon:
-    """Projects a polygon to EPSG 4326 and rounds the projected vertex
-    coordinates to ``precision``.
+    """DEPRECATED.
+
+    .. deprecated:: 0.5.0
+        Use :func:`projection.reproject_shape` instead.
+
+    Projects a polygon and rounds the projected vertex coordinates to ``precision``.
 
     Duplicate points caused by rounding are removed.
 
     Args:
         polygon (Polygon): The polygon to reproject.
         crs (CRS): The CRS of the input polygon.
         precision (int): The number of decimal places to include in the final
             polygon vertex coordinates.
+        dst_crs (CRS): The CRS of the output polygon. Defaults to EPSG 4326
 
     Returns:
-        Polygon: Polygon in EPSG 4326.
+        Polygon: Polygon in 'dst_crs'. Default to EPSG 4326
     """
-    polygon = shape(transform_geom(crs, "EPSG:4326", polygon, precision=precision))
-    # Rounding to precision can produce duplicate coordinates, so we remove
-    # them. Once once shapely>=2.0.0 is required, this can be replaced with
-    # shapely.constructive.remove_repeated_points
-    polygon = Polygon([k for k, _ in groupby(polygon.exterior.coords)])
-    return polygon
+    warnings.warn(
+        "``utils.reproject_polygon`` is deprecated and will be removed in v0.6.0. "
+        "Use ``projection.reproject_shape`` instead.",
+        DeprecationWarning,
+    )
+    return reproject_shape(
+        src_crs=crs, dst_crs=dst_crs, geom=polygon, precision=precision
+    )
 
 
 class RasterFootprint:
     """An object for creating a convex hull polygon around all areas within an
     raster that have data values (i.e., they do not have the nodata value).
     This convex hull is termed the "footprint" of the raster data and is
     returned by the :meth:`footprint` method as a polygon in a GeoJSON
     dictionary for use as the geometry attribute of a STAC Item.
 
     Two important operations during this calculation are the densification of
     the footprint in the native CRS and simplification of the footprint after
-    reprojection to EPSG 4326. If the initial low-vertex polygon in the native
+    reprojection. If the initial low-vertex polygon in the native
     CRS is not densified, this can result in a reprojected polygon that does not
     accurately represent the data footprint. For example, a MODIS asset
     represented by a rectangular 5 point Polygon in a sinusoidal projection will
     reproject to a parallelogram in EPSG 4326, when it would be more accurately
     represented by a polygon with two parallel sides and two curved sides. The
     difference between these representations is greater the further away from
     the meridian and equator the asset is located.
 
-    After reprojection to EPSG 4326, the footprint may have more points than
+    After reprojection, the footprint may have more points than
     desired. This can be simplified to a polygon with fewer points that maintain
     a maximum distance to the original geometry.
 
     Args:
         data_array (numpy.NDArray[Any]): The raster data used for the
             footprint calculation.
         crs (CRS): Coordinate reference system of the raster data.
+        dst_crs (CRS): Coordinate reference system of the footprint data. Defaults
+            to EPSG 4236.
         transform (Affine): Matrix defining the transformation from pixel to CRS
             coordinates.
         precision (int): The number of decimal places to include in the
             final footprint coordinates.
         densification_factor (Optional[int]): The factor by which to
             increase point density within the footprint polygon before
-            projection to EPSG 4326. A factor of 2 would double the density of
+            projection. A factor of 2 would double the density of
             points (placing one new point between each existing pair of points),
             a factor of 3 would place two points between each point, etc. Higher
             densities produce higher fidelity footprints in areas of high
             projection distortion. Mutually exclusive with
             ``densification_distance``.
         densification_distance (Optional[float]): The distance by which to
             increase point density within the footprint polygon before
-            projection to EPSG 4326. If the distance is set to 2 and the segment
+            projection. If the distance is set to 2 and the segment
             length between two polygon vertices is 10, 4 new vertices would be
             created along the segment. Higher densities produce higher
             fidelity footprints in areas of high projection distortion.
             Mutually exclusive with ``densification_factor``.
         simplify_tolerance (Optional[float]): Distance, in degrees, within
             which all locations on the simplified polygon will be to the original
             polygon.
@@ -170,24 +198,25 @@
             ``data_array``. If set to None, this will return a footprint
             including nodata values.
     """
 
     crs: CRS
     """Coordinate reference system of the raster data."""
 
+    dst_crs: CRS = "EPSG:4326"
+    """Coordinate reference system of the footprint."""
+
     data_array: npt.NDArray[Any]
     """2D or 3D array of raster data."""
 
     densification_distance: Optional[float]
-    """Optional distance for densifying polygon vertices before reprojection to
-    EPSG 4326."""
+    """Optional distance for densifying polygon vertices before reprojection."""
 
     densification_factor: Optional[int]
-    """Optional factor for densifying polygon vertices before reprojection to
-    EPSG 4326."""
+    """Optional factor for densifying polygon vertices before reprojection."""
 
     no_data: Optional[Union[int, float]]
     """Optional value defining pixels to exclude from the footprint."""
 
     precision: int
     """Number of decimal places in the final footprint coordinates."""
 
@@ -200,24 +229,26 @@
 
     def __init__(
         self,
         data_array: npt.NDArray[Any],
         crs: CRS,
         transform: Affine,
         *,
+        dst_crs: CRS = "EPSG:4326",
         precision: int = DEFAULT_PRECISION,
         densification_factor: Optional[int] = None,
         densification_distance: Optional[float] = None,
         simplify_tolerance: Optional[float] = None,
         no_data: Optional[Union[int, float]] = None,
     ) -> None:
         if data_array.ndim == 2:
             data_array = data_array[np.newaxis, :]
         self.data_array = data_array
         self.crs = crs
+        self.dst_crs = dst_crs
         self.transform = transform
         self.precision = precision
         if densification_factor is not None and densification_distance is not None:
             raise ValueError(
                 "Only one of 'densification_factor' or 'densification_distance' "
                 "can be specified."
             )
@@ -316,26 +347,31 @@
                     polygon.exterior.coords, self.densification_distance
                 )
             )
         else:
             return polygon
 
     def reproject_polygon(self, polygon: Polygon) -> Polygon:
-        """Projects a polygon to EPSG 4326 and rounds the projected vertex
-        coordinates to ``self.precision``.
+        """Projects a polygon and rounds the projected vertex coordinates to
+        ``self.precision``.
 
         Duplicate points caused by rounding are removed.
 
         Args:
             polygon (Polygon): Footprint polygon in the native CRS.
 
         Returns:
-            Polygon: Footprint polygon in EPSG 4326.
+            Polygon: Footprint polygon in 'dst_crs'.
         """
-        return reproject_polygon(polygon, self.crs, self.precision)
+        return reproject_shape(
+            src_crs=self.crs,
+            dst_crs=self.dst_crs,
+            geom=polygon,
+            precision=self.precision,
+        )
 
     def simplify_polygon(self, polygon: Polygon) -> Polygon:
         """Reduces the number of polygon vertices such that the simplified
         polygon shape is no further away than the original polygon vertices
         than ``self.simplify_tolerance``.
 
         Args:
@@ -353,40 +389,43 @@
         return polygon
 
     @classmethod
     def from_href(
         cls: Type[T],
         href: str,
         *,
+        dst_crs: CRS = "EPSG:4326",
         precision: int = DEFAULT_PRECISION,
         densification_factor: Optional[int] = None,
         densification_distance: Optional[float] = None,
         simplify_tolerance: Optional[float] = None,
         no_data: Optional[Union[int, float]] = None,
         bands: List[int] = [1],
     ) -> T:
         """Produces a :class:`RasterFootprint` instance from an image href.
 
         The href can point to any file that is openable by rasterio.
 
         Args:
             href (str): The href of the image to process.
+            dst_crs (CRS): Coordinate reference system of the footprint data. Defaults
+                to EPSG 4236.
             precision (int): The number of decimal places to include in the
                 final footprint coordinates.
             densification_factor (Optional[int]): The factor by which to
                 increase point density within the footprint polygon before
-                projection to EPSG 4326. A factor of 2 would double the density
+                projection. A factor of 2 would double the density
                 of points (placing one new point between each existing pair of
                 points), a factor of 3 would place two points between each point,
                 etc. Higher densities produce higher fidelity footprints in
                 areas of high projection distortion. Mutually exclusive with
                 ``densification_distance``.
             densification_distance (Optional[float]): The distance by which to
                 increase point density within the footprint polygon before
-                projection to EPSG 4326. If the distance is set to 2 and the
+                projection. If the distance is set to 2 and the
                 segment length between two polygon vertices is 10, 4 new
                 vertices would be created along the segment. Higher densities
                 produce higher fidelity footprints in areas of high projection
                 distortion.  Mutually exclusive with ``densification_factor``.
             simplify_tolerance (Optional[float]): Distance, in degrees, within
                 which all locations on the simplified polygon will be to the
                 original polygon.
@@ -400,54 +439,58 @@
 
         Returns:
             RasterFootprint: A :class:`RasterFootprint` instance.
         """
         with rasterio.open(href) as source:
             return cls.from_rasterio_dataset_reader(
                 reader=source,
+                dst_crs=dst_crs,
                 no_data=no_data,
                 bands=bands,
                 precision=precision,
                 densification_factor=densification_factor,
                 densification_distance=densification_distance,
                 simplify_tolerance=simplify_tolerance,
             )
 
     @classmethod
     def from_rasterio_dataset_reader(
         cls: Type[T],
         reader: DatasetReader,
         *,
+        dst_crs: CRS = "EPSG:4326",
         precision: int = DEFAULT_PRECISION,
         densification_factor: Optional[int] = None,
         densification_distance: Optional[float] = None,
         simplify_tolerance: Optional[float] = None,
         no_data: Optional[Union[int, float]] = None,
         bands: List[int] = [1],
     ) -> T:
         """Produces a :class:`RasterFootprint` instance from a
         :class:`rasterio.io.DatasetReader`  object, i.e., an opened dataset
         object returned by a :func:`rasterio.open` call.
 
         Args:
             reader (DatasetReader): A rasterio dataset reader object for the
                 image to process.
+            dst_crs (CRS): Coordinate reference system of the footprint data. Defaults
+                to EPSG 4236.
             precision (int): The number of decimal places to include in the
                 final footprint coordinates.
             densification_factor (Optional[int]): The factor by which to
                 increase point density within the footprint polygon before
-                projection to EPSG 4326. A factor of 2 would double the density
+                projection. A factor of 2 would double the density
                 of points (placing one new point between each existing pair of
                 points), a factor of 3 would place two points between each point,
                 etc. Higher densities produce higher fidelity footprints in
                 areas of high projection distortion. Mutually exclusive with
                 ``densification_distance``.
             densification_distance (Optional[float]): The distance by which to
                 increase point density within the footprint polygon before
-                projection to EPSG 4326. If the distance is set to 2 and the
+                projection. If the distance is set to 2 and the
                 segment length between two polygon vertices is 10, 4 new
                 vertices would be created along the segment. Higher densities
                 produce higher fidelity footprints in areas of high projection
                 distortion.  Mutually exclusive with ``densification_factor``.
             simplify_tolerance (Optional[float]): Distance, in degrees, within
                 which all locations on the simplified polygon will be to the
                 original polygon.
@@ -477,35 +520,38 @@
         band_data = []
         for index in bands:
             band_data.append(reader.read(index))
 
         return cls(
             data_array=np.asarray(band_data),
             crs=reader.crs,
+            dst_crs=dst_crs,
             transform=reader.transform,
             no_data=no_data,
             precision=precision,
             densification_factor=densification_factor,
             densification_distance=densification_distance,
             simplify_tolerance=simplify_tolerance,
         )
 
     @classmethod
     def update_geometry_from_asset_footprint(
         cls,
         item: Item,
         *,
         asset_names: List[str] = [],
+        dst_crs: CRS = "EPSG:4326",
         precision: int = DEFAULT_PRECISION,
         densification_factor: Optional[int] = None,
         densification_distance: Optional[float] = None,
         simplify_tolerance: Optional[float] = None,
         no_data: Optional[Union[int, float]] = None,
         bands: List[int] = [1],
         skip_errors: bool = True,
+        footprint_merge_strategy: FootprintMergeStrategy = FootprintMergeStrategy.FIRST,
     ) -> bool:
         """Accepts an Item and an optional list of asset names within that
         Item, and updates the geometry of that Item in-place with the data
         footprint derived from the first of the assets that exists in the Item.
         The Item bbox is also updated in-place to bound the new footprint
         extents.
 
@@ -513,27 +559,29 @@
         calculation.
 
         Args:
             item (Item): The PySTAC Item to update.
             asset_names (List[str]): The names of the assets for which to attempt to
                 extract footprints. The first successful footprint will be used. If
                 the list is empty, all assets will be tried until one is successful.
+            dst_crs (CRS): Coordinate reference system of the footprint data. Defaults
+                to EPSG 4236.
             precision (int): The number of decimal places to include in the final
                 footprint coordinates.
             densification_factor (Optional[int]): The factor by which to
                 increase point density within the footprint polygon before
-                projection to EPSG 4326. A factor of 2 would double the density
+                projection. A factor of 2 would double the density
                 of points (placing one new point between each existing pair of
                 points), a factor of 3 would place two points between each point,
                 etc. Higher densities produce higher fidelity footprints in
                 areas of high projection distortion. Mutually exclusive with
                 ``densification_distance``.
             densification_distance (Optional[float]): The distance by which to
                 increase point density within the footprint polygon before
-                projection to EPSG 4326. If the distance is set to 2 and the
+                projection. If the distance is set to 2 and the
                 segment length between two polygon vertices is 10, 4 new
                 vertices would be created along the segment. Higher densities
                 produce higher fidelity footprints in areas of high projection
                 distortion.  Mutually exclusive with ``densification_factor``.
             simplify_tolerance (Optional[float]): Distance, in degrees, within which
                 all locations on the simplified polygon will be to the original
                 polygon.
@@ -542,46 +590,63 @@
                 a footprint including nodata values.
             bands (List[int]): The bands to use to compute the footprint.
                 Defaults to [1]. If an empty list is provided, the bands will be ORd
                 together; e.g., for a pixel to be outside of the footprint, all
                 bands must have nodata in that pixel.
             skip_errors (bool): If False, raise an error for a missing href or
                 footprint calculation failure.
+            footprint_aggregator (FootprintMergeStrategy): Provides a
+                means to control how the footprints of assets are aggregated;
+                see :class:`FootprintMergeStrategy` for details; defaults to using
+                the `FIRST` strategy
 
         Returns:
             bool: True if the Item geometry was successfully updated, False if not.
         """
-        asset_name_and_extent = next(
-            cls.data_footprints_for_data_assets(
-                item,
-                asset_names=asset_names,
-                precision=precision,
-                densification_factor=densification_factor,
-                densification_distance=densification_distance,
-                simplify_tolerance=simplify_tolerance,
-                no_data=no_data,
-                bands=bands,
-                skip_errors=skip_errors,
-            ),
-            None,
+        asset_extent_iterator = cls.data_footprints_for_data_assets(
+            item,
+            asset_names=asset_names,
+            dst_crs=dst_crs,
+            precision=precision,
+            densification_factor=densification_factor,
+            densification_distance=densification_distance,
+            simplify_tolerance=simplify_tolerance,
+            no_data=no_data,
+            bands=bands,
+            skip_errors=skip_errors,
         )
-        if asset_name_and_extent is not None:
-            _, extent = asset_name_and_extent
-            item.geometry = extent
-            item.bbox = list(shape(extent).bounds)
-            return True
+
+        if footprint_merge_strategy == FootprintMergeStrategy.FIRST:
+            asset_name_extent = next(asset_extent_iterator, None)
+            if asset_name_extent is None:
+                return False
+            _, extent = asset_name_extent
         else:
-            return False
+            extents = [shape(extent) for _, extent in asset_extent_iterator]
+            if extents == []:
+                return False
+            if footprint_merge_strategy == FootprintMergeStrategy.INTERSECTION:
+                extent = mutual_intersection(extents)
+            elif footprint_merge_strategy == FootprintMergeStrategy.UNION:
+                extent = unary_union(extents)
+            else:
+                raise Exception(
+                    f"Unrecognized aggregation strategy: {footprint_merge_strategy}"
+                )
+        item.geometry = extent
+        item.bbox = list(shape(extent).bounds)
+        return True
 
     @classmethod
     def data_footprints_for_data_assets(
         cls,
         item: Item,
         *,
         asset_names: List[str] = [],
+        dst_crs: CRS = "EPSG:4326",
         precision: int = DEFAULT_PRECISION,
         densification_factor: Optional[int] = None,
         densification_distance: Optional[float] = None,
         simplify_tolerance: Optional[float] = None,
         no_data: Optional[Union[int, float]] = None,
         bands: List[int] = [1],
         skip_errors: bool = True,
@@ -595,27 +660,29 @@
         calculation.
 
         Args:
             item (Item): The PySTAC Item to update.
             asset_names (List[str]): The names of the assets for which to attempt to
                 extract footprints. The first successful footprint will be used. If
                 the list is empty, all assets will be tried until one is successful.
+            dst_crs (CRS): Coordinate reference system of the footprint data. Defaults
+                to EPSG 4236.
             precision (int): The number of decimal places to include in the final
                 footprint coordinates.
             densification_factor (Optional[int]): The factor by which to
                 increase point density within the footprint polygon before
-                projection to EPSG 4326. A factor of 2 would double the density
+                projection. A factor of 2 would double the density
                 of points (placing one new point between each existing pair of
                 points), a factor of 3 would place two points between each point,
                 etc. Higher densities produce higher fidelity footprints in
                 areas of high projection distortion. Mutually exclusive with
                 ``densification_distance``.
             densification_distance (Optional[float]): The distance by which to
                 increase point density within the footprint polygon before
-                projection to EPSG 4326. If the distance is set to 2 and the
+                projection. If the distance is set to 2 and the
                 segment length between two polygon vertices is 10, 4 new
                 vertices would be created along the segment. Higher densities
                 produce higher fidelity footprints in areas of high projection
                 distortion.  Mutually exclusive with ``densification_factor``.
             simplify_tolerance (Optional[float]): Distance, in degrees, within which
                 all locations on the simplified polygon will be to the original
                 polygon.
@@ -647,14 +714,15 @@
                 if href is None:
                     handle_error(
                         f"Could not determine extent for asset '{name}', missing href"
                     )
                 else:
                     extent = cls.from_href(
                         href=href,
+                        dst_crs=dst_crs,
                         no_data=no_data,
                         bands=bands,
                         precision=precision,
                         densification_factor=densification_factor,
                         densification_distance=densification_distance,
                         simplify_tolerance=simplify_tolerance,
                     ).footprint()
@@ -872,30 +940,32 @@
     ).footprint()
 
 
 def densify_reproject_simplify(
     polygon: Polygon,
     crs: CRS,
     *,
+    dst_crs: CRS = "EPSG:4326",
     densification_factor: Optional[int] = None,
     precision: int = DEFAULT_PRECISION,
     simplify_tolerance: Optional[float] = None,
 ) -> Polygon:
-    """Densifies the input polygon, reprojects it to EPSG 4326, and simplifies
+    """Densifies the input polygon, reprojects it, and simplifies
     the resulting polygon.
 
     See :class:`RasterFootprint` for details on densification and
     simplification.
 
     Args:
         polygon (Polygon): The input polygon.
         crs (CRS): The CRS of the input polygon.
+        dst_crs (CRS): The CRS of the output polygon. Defaults to EPSG 4326
         densification_factor (Optional[int]): The factor by which to
-            increase point density within the polygon before projection to
-            EPSG 4326. A factor of 2 would double the density of points (placing
+            increase point density within the polygon before projection.
+            A factor of 2 would double the density of points (placing
             one new point between each existing pair of points), a factor of
             3 would place two points between each point, etc. Higher
             densities produce higher fidelity footprints in areas of high
             projection distortion.
         precision (int): The number of decimal places to include in the final
             polygon vertex coordinates.
         simplify_tolerance (Optional[float]): Distance, in degrees, within which
@@ -905,13 +975,15 @@
     Returns:
         Polygon: The reprojected Polygon.
     """
     if densification_factor is not None:
         polygon = Polygon(
             densify_by_factor(polygon.exterior.coords, factor=densification_factor)
         )
-    polygon = reproject_polygon(polygon, crs, precision)
+    polygon = reproject_shape(
+        geom=polygon, src_crs=crs, dst_crs=dst_crs, precision=precision
+    )
     if simplify_tolerance is not None:
         polygon = polygon.simplify(
             tolerance=simplify_tolerance, preserve_topology=False
         )
     return polygon
```

### Comparing `stactools-0.4.8/src/stactools/core/utils/round.py` & `stactools-0.5.0/src/stactools/core/utils/round.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/core/utils/subprocess.py` & `stactools-0.5.0/src/stactools/core/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/testing/cli.py` & `stactools-0.5.0/src/stactools/testing/cli.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.8/src/stactools/testing/cli_test.py` & `stactools-0.5.0/src/stactools/testing/cli_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import unittest
+import warnings
 from abc import ABC, abstractmethod
 from typing import Callable, List, Optional, Sequence, Union
 
 import click
 from click.testing import CliRunner, Result
 
 
@@ -25,14 +26,19 @@
     def setUp(self) -> None:
         """Sets up a mock cli group for testing."""
 
         @click.group()
         def cli() -> None:
             pass
 
+        warnings.warn(
+            "CliTestCase is deprecated in v0.5.0 and will be removed in v0.6.0. "
+            "Please use `click.testing.CliRunner` instead",
+            DeprecationWarning,
+        )
         for create_subcommand in self.create_subcommand_functions():
             create_subcommand(cli)
         self.cli = cli
 
     def run_command(self, cmd: Optional[Union[str, Sequence[str]]]) -> Result:
         """Runs a command, returning its result.
```

### Comparing `stactools-0.4.8/src/stactools/testing/test_data.py` & `stactools-0.5.0/src/stactools/testing/test_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,136 +1,181 @@
 import os
 import shutil
+from dataclasses import dataclass
 from tempfile import TemporaryDirectory
-from typing import Any, Dict
+from typing import Any, Dict, Optional, Union
 from zipfile import ZipFile
 
 import fsspec
 import requests
 
-# TODO make external data a dataclass
 
-# example external data:
-# {
-#     'AST_L1T_00305032000040446_20150409135350_78838.hdf': {
-#         'url':
-#         ('https://ai4epublictestdata.blob.core.windows.net/'
-#          'stactools/aster/AST_L1T_00305032000040446_20150409135350_78838.zip'),
-#         'compress':
-#         'zip'
-#     }
-# }
+@dataclass
+class ExternalData:
+    """External data configurations for fetching and storing remote files.
 
+    Args:
+        url (str): URL at which the external data is found.
+        compress (str): Compression method that has been used on external data.
+            If provided, data is extracted after it is fetched.
+            Only zip is supported. Defaults to None.
+        s3 (Dict[str, Any]): Dictionary containing keyword arguments to use
+            when instantiating ``s3fs.S3FileSystem``. Defaults to None.
+        planetary_computer (bool): Whether external data is on planetary computer
+            and needs to be signed. Defaults to False.
+
+    """
 
+    url: str
+    compress: Optional[str] = None
+    s3: Optional[Dict[str, Any]] = None
+    planetary_computer: bool = False
+
+
+@dataclass
 class TestData:
     """A structure for getting paths to test data files, and fetching external
     data for local testing.
 
-    Initialize this from, e.g., ``tests/__init__.py``:
+    Initializing this from, e.g., ``/home/user/my-package/tests/__init__.py``:
 
     .. code-block:: python
 
         test_data = TestData(__file__)
 
-    The external data dictionary should look something like this:
+    Means that ``get_path`` will be relative to ``/home/user/my-package/tests``.
+
+    .. code-block:: python
+
+        test_data.get_path("data-files/basic")
+        # "/home/user/my-package/tests/data-files/basic"
+
+    When caching external data that base path is appended with
+    ``test_data.external_subpath``  which by default is 'data-files/external'.
+
+    For instance with the following external data configuration the external
+    data file will be fetched from the URL, extracted from its zip file and
+    locally stored at:
+    ``/home/user/my-package/tests/data-files/external/AST_L1T_00305032000040446_20150409135350_78838.hdf``
 
     .. code-block:: python
 
-        {
+        test_data.external_data = {
             'AST_L1T_00305032000040446_20150409135350_78838.hdf': {
                 'url':
                     ('https://ai4epublictestdata.blob.core.windows.net/'
                     'stactools/aster/AST_L1T_00305032000040446_20150409135350_78838.zip'),
                 'compress': 'zip'
             }
         }
+        test_data.get_external_data("AST_L1T_00305032000040446_20150409135350_78838.hdf")
 
     Args:
-        path (str): The path to the file at the root of the test data directory.
-        external_data (dict[str, Any]):
-            External data configurations. These dictionaries can be used to
-            configure files that are fetched from remote locations and stored
-            locally for testing.
+        path (str): The path to any file in the directory where data is
+            (or will be) stored. The directory information is taken from this
+            path and used as the base for relative paths for the local data. It
+            is stored on the class as ``self.base_path``
+        external_data (Dict[str, ExternalData]):
+            External data configurations for fetching and storing remote files.
+            This is defined as a dictionary with the following structure: the
+            key is the relative path (relative to
+            ``self.base_path / self.external_subpath``) for cached data
+            after it is fetched from remote and the value is the configuration
+            as defined in :class:`ExternalData`.
+        external_subpath (str): The subpath under ``self.base_path`` that is
+            used for storing external data files. Defaults to 'data-files/external'
     """
 
     __test__ = False
 
-    def __init__(self, path: str, external_data: Dict[str, Any] = {}) -> None:
-        self.path = path
+    def __init__(
+        self,
+        path: str,
+        external_data: Dict[str, Union[Dict[str, Any], ExternalData]] = {},
+        external_subpath: str = "data-files/external",
+    ) -> None:
+        self.base_path = os.path.abspath(os.path.dirname(path))
+        self.external_subpath = external_subpath
         self.external_data = external_data
 
     def get_path(self, rel_path: str) -> str:
-        """Returns an absolute path to a local test file.
+        """Returns an absolute path to a local data file.
 
         Args:
             rel_path (str):
                 The relative path to the test data file. The path is
-                assumed to be relative to the directory containing ``self.path``.
+                assumed to be relative to ``self.base_path``.
 
         Returns:
-            str: An absolute path.
+            str: The absolute path joining ``self.base_path`` and ``rel_path``
         """
-        return os.path.abspath(os.path.join(os.path.dirname(self.path), rel_path))
+        return os.path.join(self.base_path, rel_path)
 
     def get_external_data(self, rel_path: str) -> str:
-        """Returns an absolute path to a local test file after downloading it
-        from an external source.
+        """Returns the path to the local cached version of the external data.
+
+        If data is not yet cached, this method fetches it, caches it, then returns
+        the path to the local cached version.
 
         Args:
-            rel_path (str): The key to the external data, as configured in class
-                instantiation.
+            rel_path (str): This is both the filename that the local data will be
+                stored at _and_ a key in the ``external_data`` dictionary where the
+                corresponding value is the configuration information for the external
+                data.
 
         Returns:
-            str: The absolute path to the external data file.
+            str: The absolute path to the local cached version of the
+                external data file.
         """
-        path = self.get_path(os.path.join("data-files/external", rel_path))
+        path = self.get_path(os.path.join(self.external_subpath, rel_path))
         if not os.path.exists(path):
-            entry = self.external_data.get(rel_path)
-            if entry is None:
+            config = self.external_data.get(rel_path)
+            if config is None:
                 raise Exception(
-                    "Path {} does not exist and there is no entry "
-                    "for external test data {}.".format(path, rel_path)
+                    f"Local path {path} does not exist and there is no key "
+                    f"in ``external_data`` that matches {rel_path}"
                 )
 
-            print("Downloading external test data {}...".format(rel_path))
+            print(f"Downloading external test data {rel_path}...")
             os.makedirs(os.path.dirname(path), exist_ok=True)
 
-            s3_config = entry.get("s3")
-            is_pc = entry.get("planetary_computer")  # True if from PC, needs signing
-            if s3_config:
+            if not isinstance(config, ExternalData):
+                config = ExternalData(**config)
+
+            if config.s3:
                 try:
                     import s3fs
                 except ImportError as e:
                     print(
                         "Trying to download external test data via s3, "
                         "but s3fs is not installed and the download requires "
                         "configuring the s3fs filesystem. Install stactools "
                         "with s3fs via `pip install stactools[s3]` and try again."
                     )
                     raise (e)
-                s3 = s3fs.S3FileSystem(**s3_config)
-                with s3.open(entry["url"]) as f:
+                s3 = s3fs.S3FileSystem(**config.s3)
+                with s3.open(config.url) as f:
                     data = f.read()
-            elif is_pc:
-                href = entry["url"]
+            elif config.planetary_computer:
+                href = config.url
                 r = requests.get(
                     "https://planetarycomputer.microsoft.com/api/sas/v1/sign?"
                     f"href={href}"
                 )
                 r.raise_for_status()
                 signed_href = r.json()["href"]
 
                 with fsspec.open(signed_href) as f:
                     data = f.read()
 
             else:
-                with fsspec.open(entry["url"]) as f:
+                with fsspec.open(config.url) as f:
                     data = f.read()
 
-            if entry.get("compress") == "zip":
+            if config.compress == "zip":
                 with TemporaryDirectory() as tmp_dir:
                     tmp_path = os.path.join(tmp_dir, "file.zip")
                     with open(tmp_path, "wb") as f:
                         f.write(data)
                     z = ZipFile(tmp_path)
                     name = z.namelist()[0]
                     extracted_path = z.extract(name)
```

### Comparing `stactools-0.4.8/src/stactools.egg-info/PKG-INFO` & `stactools-0.5.0/src/stactools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactools
-Version: 0.4.8
+Version: 0.5.0
 Summary: Command line tool and Python library for working with STAC
 Author-email: Rob Emanuele <rdemanuele@gmail.com>, Pete Gadomski <pete.gadomski@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/stactools
 Project-URL: documentation, https://stactools.readthedocs.io/
 Project-URL: repository, https://github.com/stac-utils/stactools.git
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: docs
 Provides-Extra: s3
 License-File: LICENSE
 
 # stactools
 
 ![Build Status](https://github.com/stac-utils/stactools/workflows/CI/badge.svg)
 [![Documentation](https://readthedocs.org/projects/stactools/badge/?version=latest)](https://stactools.readthedocs.io/en/latest/)
@@ -228,15 +229,15 @@
 
 ```sh
 pip install -e '.[dev]'
 ```
 
 ### Developing the docs
 
-To build and serve the docs, the development requirements must be installed with `pip install -e '.[dev]'`.
+To build and serve the docs, the development requirements must be installed with `pip install -e '.[docs]'`.
 To build the docs, you can use `make html` from inside of the docs directory, and to build the docs and start a server that watches for changes, use `make livehtml`:
 
 ```sh
 cd docs
 make html
 make livehtml
 ```
```

### Comparing `stactools-0.4.8/src/stactools.egg-info/SOURCES.txt` & `stactools-0.5.0/src/stactools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
+MANIFEST.in
 README.md
 pyproject.toml
 src/stactools.egg-info/PKG-INFO
 src/stactools.egg-info/SOURCES.txt
 src/stactools.egg-info/dependency_links.txt
 src/stactools.egg-info/entry_points.txt
 src/stactools.egg-info/requires.txt
 src/stactools.egg-info/top_level.txt
 src/stactools/cli/__init__.py
 src/stactools/cli/__main__.py
 src/stactools/cli/cli.py
+src/stactools/cli/py.typed
 src/stactools/cli/registry.py
 src/stactools/cli/commands/__init__.py
 src/stactools/cli/commands/add.py
 src/stactools/cli/commands/add_asset.py
 src/stactools/cli/commands/add_raster.py
 src/stactools/cli/commands/copy.py
 src/stactools/cli/commands/create.py
@@ -33,19 +35,21 @@
 src/stactools/core/add_raster.py
 src/stactools/core/copy.py
 src/stactools/core/create.py
 src/stactools/core/geometry.py
 src/stactools/core/layout.py
 src/stactools/core/merge.py
 src/stactools/core/projection.py
+src/stactools/core/py.typed
 src/stactools/core/io/__init__.py
 src/stactools/core/io/xml.py
 src/stactools/core/utils/__init__.py
 src/stactools/core/utils/antimeridian.py
 src/stactools/core/utils/convert.py
 src/stactools/core/utils/raster_footprint.py
 src/stactools/core/utils/round.py
 src/stactools/core/utils/subprocess.py
 src/stactools/testing/__init__.py
 src/stactools/testing/cli.py
 src/stactools/testing/cli_test.py
+src/stactools/testing/py.typed
 src/stactools/testing/test_data.py
```

