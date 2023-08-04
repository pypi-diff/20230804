# Comparing `tmp/hazen-1.2.0.tar.gz` & `tmp/hazen-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazen-1.2.0.tar", last modified: Tue Apr 18 13:39:05 2023, max compression
+gzip compressed data, was "hazen-1.3.0.tar", last modified: Fri Aug  4 09:39:33 2023, max compression
```

## Comparing `hazen-1.2.0.tar` & `hazen-1.3.0.tar`

### file list

```diff
@@ -1,65 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.439765 hazen-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-18 13:38:53.000000 hazen-1.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-18 13:38:53.000000 hazen-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-18 13:39:05.439765 hazen-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-18 13:38:53.000000 hazen-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.435765 hazen-1.2.0/hazen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-18 13:39:05.000000 hazen-1.2.0/hazen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-04-18 13:39:05.000000 hazen-1.2.0/hazen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:39:05.000000 hazen-1.2.0/hazen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-18 13:39:05.000000 hazen-1.2.0/hazen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 13:39:05.000000 hazen-1.2.0/hazen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 13:39:05.000000 hazen-1.2.0/hazen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.435765 hazen-1.2.0/hazenlib/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/HazenTask.py
--rw-r--r--   0 runner    (1001) docker     (123)    15280 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.431765 hazen-1.2.0/hazenlib/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.435765 hazen-1.2.0/hazenlib/data/relaxometry/
--rw-r--r--   0 runner    (1001) docker     (123)   157178 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/data/relaxometry/Plate4_T1_signed
--rw-r--r--   0 runner    (1001) docker     (123)   168984 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/data/relaxometry/Plate4_T2
--rw-r--r--   0 runner    (1001) docker     (123)   157180 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/data/relaxometry/Plate5_T1_signed
--rw-r--r--   0 runner    (1001) docker     (123)   168984 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/data/relaxometry/Plate5_T2
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    47189 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/relaxometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/shapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.439765 hazen-1.2.0/hazenlib/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_geometric_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_ghosting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11634 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_slice_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_slice_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    15174 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_spatial_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/acr_uniformity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11307 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/ghosting.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/relaxometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/slice_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    35489 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/slice_width.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/snr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/snr_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/spatial_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tasks/uniformity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-18 13:38:54.000000 hazen-1.2.0/hazenlib/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-18 13:38:54.000000 hazen-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-18 13:39:05.443765 hazen-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:39:05.439765 hazen-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_geometric_accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_ghosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_slice_position.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_slice_thickness.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_spatial_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_acr_uniformity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6567 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_ghosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9397 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_hazenlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    31794 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_relaxometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_slice_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_slice_width.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_snr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_snr_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    39521 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_spatial_resolution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-18 13:38:54.000000 hazen-1.2.0/tests/test_uniformity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:39:33.612922 hazen-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-08-04 09:39:17.000000 hazen-1.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 09:39:17.000000 hazen-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-08-04 09:39:33.612922 hazen-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-08-04 09:39:17.000000 hazen-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:39:33.604922 hazen-1.3.0/hazen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-08-04 09:39:33.000000 hazen-1.3.0/hazen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-08-04 09:39:33.000000 hazen-1.3.0/hazen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:39:33.000000 hazen-1.3.0/hazen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-04 09:39:33.000000 hazen-1.3.0/hazen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-04 09:39:33.000000 hazen-1.3.0/hazen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-04 09:39:33.000000 hazen-1.3.0/hazen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:39:33.604922 hazen-1.3.0/hazenlib/
+-rw-r--r--   0 runner    (1001) docker     (123)    11252 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/ACRObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/HazenTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:39:33.604922 hazen-1.3.0/hazenlib/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:39:33.608922 hazen-1.3.0/hazenlib/data/relaxometry/
+-rw-r--r--   0 runner    (1001) docker     (123)   157178 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/data/relaxometry/Plate4_T1_signed
+-rw-r--r--   0 runner    (1001) docker     (123)   168984 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/data/relaxometry/Plate4_T2
+-rw-r--r--   0 runner    (1001) docker     (123)   157180 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/data/relaxometry/Plate5_T1_signed
+-rw-r--r--   0 runner    (1001) docker     (123)   168984 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/data/relaxometry/Plate5_T2
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/relaxometry_params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:39:33.608922 hazen-1.3.0/hazenlib/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/acr_geometric_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8757 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/acr_ghosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10865 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/acr_slice_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/acr_slice_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/acr_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13693 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/acr_spatial_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5540 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/acr_uniformity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/ghosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43985 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/relaxometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9097 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/slice_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35559 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/slice_width.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13986 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11173 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/snr_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/spatial_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/tasks/uniformity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10883 2023-08-04 09:39:17.000000 hazen-1.3.0/hazenlib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-04 09:39:17.000000 hazen-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-04 09:39:33.612922 hazen-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:39:33.612922 hazen-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_ACRObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_acr_geometric_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_acr_ghosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_acr_slice_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_acr_slice_thickness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_acr_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4496 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_acr_spatial_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_acr_uniformity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_ghosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_hazenlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31104 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_relaxometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4088 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_slice_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16823 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_slice_width.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_snr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_snr_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39330 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_spatial_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_uniformity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-08-04 09:39:17.000000 hazen-1.3.0/tests/test_utils.py
```

### Comparing `hazen-1.2.0/PKG-INFO` & `hazen-1.3.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: hazen
-Version: 1.2.0
+Version: 1.3.0
 Summary: An automatic MRI QA tool
 Home-page: https://bitbucket.org/gsttmri/hazen
 Author: Shuaib, Haris
 Author-email: mohammad_haris.shuaib@kcl.ac.uk
 Requires-Python: <3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 <!-- PROJECT HEADING -->
 <br />
 <p align="center">
-<img src="https://raw.githubusercontent.com/GSTT-CSC/hazen/readme-dev/docs/assets/ibn-al-haytham.jpeg" alt="Ibn Al-Haytham">
+<img src="https://upload.wikimedia.org/wikipedia/commons/a/a3/Ibn_Al-Haytham_portrait.jpg" alt="Ibn Al-Haytham" width="512">
 </p>   
 <h1 align="center">hazen</h1>
 <p align="center">
 Quality assurance framework for Magnetic Resonance Imaging
 <br />
 <a href="https://hazen.readthedocs.io/en/latest/"><strong>Explore the docs »</strong></a>
 <br />
@@ -33,154 +33,151 @@
 </p>
 <p align="center">Please <b>STAR</b> this repo to receive updates about new versions of hazen!</p>
 
 ---
 
 ## Overview
 
-hazen is a software framework for performing automated analysis of magnetic resonance imaging (MRI) Quality Assurance data.
+hazen is a software framework for performing automated analysis of magnetic resonance imaging (MRI) quality assurance 
+(QA) data. hazen consists of multiple [Tasks](hazenlib/tasks) which perform quantitative processing and analysis of 
+MRI phantom data. Currently, hazen supports the [ACR Large MRI Phantom](https://www.acraccreditation.org/-/media/acraccreditation/documents/mri/largephantomguidance.pdf)
+and the MagNET Test Objects collection of phantoms.
 
-It provides automatic quantitative analysis for the following measurements of MRI phantom data:
+The hazen Tasks provide the following measurements within these phantoms:
 - Signal-to-noise ratio (SNR)
 - Spatial resolution
-- Slice position and width
+- Slice position
+- Slice width
 - Uniformity
 - Ghosting
-- MR Relaxometry
+- MR relaxometry
 
-Some example outputs from hazen:
+Each Task outputs numerical results to the user's terminal. Below is an output from the `hazen snr` Task performed on 
+some example MRI data:
 
-| hazen acr_ghosting                        | hazen ghosting                |
-|----------------------------------|-------------------------------|
-| ![](docs/assets/SNR.png) | ![](docs/assets/ghosting.png) |
+```shell
+hazen snr tests/data/snr/Siemens
+{
+  'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 173.97,
+  'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 177.91,
+  'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 1698.21,
+  'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 1736.66,
+  'snr_subtraction_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 220.73,
+  'snr_subtraction_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 2154.69
+}
+```
+
+The optional `--report` flag allows the user to visualise the image processing performed by each hazen Task:
+
+| `hazen snr tests/data/snr/Siemens --report` | `hazen acr_ghosting tests/data/acr/Siemens --report` |
+|---------------------------------------------|------------------------------------------------------|
+| <img src="/docs/assets/snr.jpg?raw=true"> | <img src="/docs/assets/acr_ghosting.jpg?raw=true"> |
 
 ---
 
-## Installation
+## Installation and usage
 
-### pip
+There are two main options for running hazen.
+1. Install using Python and run directly via command line interface (CLI)
+2. Run using the latest Docker container build
 
-Hazen can be installed using pip on python 3.9 or higher, it is recommended to use a virtual environment
+### 1) Python install and run (CLI)
+
+hazen can be installed with Python 3.9 or higher via pip. It is strongly recommended to use a virtual environment.
 
 ```bash
 python3 -m venv hazen-venv
 source hazen-venv/bin/activate
 pip install hazen
 ```
 
-#### Docker
-
-The Docker version of hazen as it is easy to get up-and-running and is linked to the most stable release. Refer to the [Docker installation instructions](https://docs.docker.com/engine/install) to install Docker on your host computer.
-
-For ease of use, it is recommended to copy the `hazen-app` script to a location accessible on the path such as `/usr/local/bin`. This will allow you to run hazen from any location on your computer. Then, to use Docker hazen, simply run the `hazen-app` script appended with the function you want to use (e.g.: `snr`). 
-
-In Terminal:
-
-```bash 
-cd hazen
-cp ./hazen-app /usr/local/bin
-
-# run hazen with CLI arguments
-hazen-app snr tests/data/snr/Siemens/
+#### Updating hazen
+If you already have an old version of hazen installed, upgrade to the latest version with:
 
-latest: Pulling from gsttmriphysics/hazen
-Digest: sha256:18603e40b45f3af4bf45f07559a08a7833af92a6efe21cb7306f758e8eeab24a
-Status: Image is up to date for gsttmriphysics/hazen:latest
-docker.io/gsttmriphysics/hazen:latest
-{   'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 191.16,
-    'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 195.58,
-    'snr_smoothing_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 1866.09,
-    'snr_smoothing_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 1909.2,
-    'snr_subtraction_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 220.73,
-    'snr_subtraction_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 2154.69}
+```shell
+source hazen-venv/bin/activate
+pip install --upgrade pip
+pip install --upgrade hazen
 ```
 
-
-#### Linux & MacOS
-
-For developers, hazen can be installed from source using `pip`. We highly recommend using a virtual environment.
+#### Running hazen via CLI
+The CLI version of hazen is designed to be pointed at single folders containing DICOM file(s). Example datasets are 
+provided in the `tests/data/` directory. If you are using the Docker version of hazen (installation described below), 
+replace `hazen` with `hazen-app` in the following commands.
 
 ```bash
-# Install OpenSSL
-# Go to local hazen repo directory
-cd hazen
-
-# Create and activate a virtual environment
-python3 -m venv ./hazen-venv
-source hazen-venv/bin/activate
+# To see the full list of available Tasks, enter:
+hazen -h
 
-# Install requirements
-pip install --upgrade pip setuptools wheel
-pip install -r requirements.txt
+# To perform the spatial resolution Task on example data:
+hazen spatial_resolution tests/data/resolution/philips
 
-# Install hazen
-pip install .
+# To perform the SNR Task on example data:
+hazen snr tests/data/snr/Philips
 
-# Run tests to ensure everything is working
-pytest tests/
+# The `--report` option provides additional information about the image processing measurement methods and is available 
+# for all Tasks. Example usage for the SNR Task, which returns images showing the regions used for SNR calculation.
+hazen snr tests/data/snr/Philips --report
 ```
 
----
-
-## Usage
-
-### Command Line
+### 2) Docker
 
-The CLI version of hazen is designed to be pointed at single folders containing DICOM file(s). Example datasets are provided in the `tests/data/` directory. If you are not using the Docker version of hazen, replace `hazen-app` with `hazen` in the following commands.
+The Docker version of hazen has been made available as it is easy to get up-and-running and is linked to the most recent 
+stable release. Refer to the [Docker installation instructions](https://docs.docker.com/engine/install) to install 
+Docker on your host computer.
+
+The containerised version of hazen can be obtained from DockerHub (see commands below). For ease of use, it is 
+recommended to copy the `hazen-app` script to a location accessible on the PATH such as `/usr/local/bin`. This will 
+allow you to run hazen from any directory on your computer. Then, to use Docker hazen, simply run the `hazen-app` script 
+appended with the function you want to use (e.g.: `snr`). 
 
-To perform an SNR measurement on the provided example Philips DICOMs:
-
-`hazen-app snr tests/data/snr/Philips`
-
-To perform a spatial resolution measurement on example data provided by the East Kent Trust:
+In Terminal:
 
-`hazen-app spatial_resolution tests/data/resolution/philips`
+```shell
+# Ensure Docker installed and running, then pull the latest hazen Docker container
+docker pull gsttmriphysics/hazen:latest
 
-To see the full list of available tools, enter:
+# Command line output will look something like:
+latest: Pulling from gsttmriphysics/hazen
+Digest: sha256:18603e40b45f3af4bf45f07559a08a7833af92a6efe21cb7306f758e8eeab24a
+Status: Image is up to date for gsttmriphysics/hazen:latest
+docker.io/gsttmriphysics/hazen:latest
 
-`hazen-app -h`
+# Copy the 'hazen-app' executable file into your local bin folder
+cd hazen
+cp hazen-app /usr/local/bin
 
-The `--report` option provides additional information for some of the functions. For example, the user can gain additional insight into the performance of the snr function by entering:
+# Run hazen via Docker with the normal CLI inputs
+hazen-app snr tests/data/snr/Siemens/
 
-`hazen-app snr tests/data/snr/Philips --report`
+# Example command line output for the SNR Task:
+{
+  'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 173.97,
+  'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 177.91,
+  'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 1698.21,
+  'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 1736.66,
+  'snr_subtraction_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 220.73,
+  'snr_subtraction_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 2154.69
+}
+```
 
 ### Web Interface
 
-WIP: we are developing a web interface for hazen.
+Development of a [web interface for hazen](https://github.com/GSTT-CSC/hazen-web-app) is in progress.
 
 ---
 
-## Contributing
-- The Release Manager should create a release branch for the future planned release e.g. release-X.X.X
-- The RMs shall organise backlog refinement sessions to ensure issues are allocated to the appropriate release
-- The RM should ensure their release branch is kept up-to-date with master
-- PRs should be merged into the appropriate release branch for the issue(s) it is addressing
-
-If you want to contribute to the development of hazen, please take a look at: `CONTRIBUTING.md`.
+## Contributing to hazen
 
----
-
-## Users
+### Users
+Please [raise an Issue](https://github.com/GSTT-CSC/hazen/issues) for any of the following reasons:
+- Problems installing or running hazen
+- Suggestions for improvements
+- Requests for new features
 
-Please [raise an Issue](https://github.com/GSTT-CSC/hazen/issues) if you have any problems installing or running hazen.
+We have used hazen with MRI data from a handful of different MRI scanners, including multiple different vendors. If 
+hazen does not perform with your MRI data, or the results are unexpected, please raise an Issue.
 
-We have used hazen with MRI data from a handful of different MRI scanners, including multiple different vendors. If your MRI data doesn't work with hazen, or the results are unexpected, please submit an Issue and we will investigate. 
+### Developers
+Please see [CONTRIBUTING.md](CONTRIBUTING.md) for developer guidelines.
 
 ---
-
-## Releasing
-
-The Release Manager should ensure:
-- All outstanding issues for the current release have been closed, or, transferred to future release.
-- All tests are passing on GitHub Actions.
-- All documentation has been updated with correct version numbers:
-   - Update version number `hazenlib/_version.py`, i.e. imported into `docs/conf.py`, `hazenlib/__init__.py` and `setup.cfg`
-   - Update version number in `CITATION.cff`
-- The `release` branch has been merged into `main` branch
-- A new release has been created with a new version tag (tag = version number)
-
-- RMs of other branches should update their release from the latest release as soon as possible and deal with any merge conflicts.
-
-![image](https://user-images.githubusercontent.com/19840489/143266366-06e33949-12c7-44b4-9ed7-c0a795b5d492.png)
-
-- RMs: Tom Roberts, Lucrezia Cester
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: hazen Version: 1.2.0 Summary: An automatic MRI QA
+Metadata-Version: 2.1 Name: hazen Version: 1.3.0 Summary: An automatic MRI QA
 tool Home-page: https://bitbucket.org/gsttmri/hazen Author: Shuaib, Haris
 Author-email: mohammad_haris.shuaib@kcl.ac.uk Requires-Python: <3.11
 Description-Content-Type: text/markdown License-File: LICENSE.txt
                                [Ibn Al-Haytham]
                               ****** hazen ******
           Quality assurance framework for Magnetic Resonance Imaging
                              Explore_the_docs_Â»
@@ -10,81 +10,92 @@
                   View_repo Â· Report_Bug Â· Request_Feature
     [https://github.com/GSTT-CSC/hazen/actions/workflows/tests_release.yml/
      badge.svg?branch=main] [https://img.shields.io/endpoint?url=https://
  gist.githubusercontent.com/laurencejackson/ba102d5f3e592fcd50451c2eff8a803d/
                     raw/hazen_pytest-coverage-comment.json]
      Please STAR this repo to receive updates about new versions of hazen!
 --- ## Overview hazen is a software framework for performing automated analysis
-of magnetic resonance imaging (MRI) Quality Assurance data. It provides
-automatic quantitative analysis for the following measurements of MRI phantom
-data: - Signal-to-noise ratio (SNR) - Spatial resolution - Slice position and
-width - Uniformity - Ghosting - MR Relaxometry Some example outputs from hazen:
-| hazen acr_ghosting | hazen ghosting | |----------------------------------|---
-----------------------------| | ![](docs/assets/SNR.png) | ![](docs/assets/
-ghosting.png) | --- ## Installation ### pip Hazen can be installed using pip on
-python 3.9 or higher, it is recommended to use a virtual environment ```bash
+of magnetic resonance imaging (MRI) quality assurance (QA) data. hazen consists
+of multiple [Tasks](hazenlib/tasks) which perform quantitative processing and
+analysis of MRI phantom data. Currently, hazen supports the [ACR Large MRI
+Phantom](https://www.acraccreditation.org/-/media/acraccreditation/documents/
+mri/largephantomguidance.pdf) and the MagNET Test Objects collection of
+phantoms. The hazen Tasks provide the following measurements within these
+phantoms: - Signal-to-noise ratio (SNR) - Spatial resolution - Slice position -
+Slice width - Uniformity - Ghosting - MR relaxometry Each Task outputs
+numerical results to the user's terminal. Below is an output from the `hazen
+snr` Task performed on some example MRI data: ```shell hazen snr tests/data/
+snr/Siemens
+{ 'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+173.97,
+'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
+177.91,
+'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+1698.21,
+'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
+1736.66,
+'snr_subtraction_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+220.73,
+'snr_subtraction_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+2154.69 } ``` The optional `--report` flag allows the user to visualise the
+image processing performed by each hazen Task: | `hazen snr tests/data/snr/
+Siemens --report` | `hazen acr_ghosting tests/data/acr/Siemens --report` | |---
+------------------------------------------|------------------------------------
+------------------| | [/docs/assets/snr.jpg?raw=true] | [/docs/assets/
+acr_ghosting.jpg?raw=true] | --- ## Installation and usage There are two main
+options for running hazen. 1. Install using Python and run directly via command
+line interface (CLI) 2. Run using the latest Docker container build ### 1)
+Python install and run (CLI) hazen can be installed with Python 3.9 or higher
+via pip. It is strongly recommended to use a virtual environment. ```bash
 python3 -m venv hazen-venv source hazen-venv/bin/activate pip install hazen ```
-#### Docker The Docker version of hazen as it is easy to get up-and-running and
-is linked to the most stable release. Refer to the [Docker installation
-instructions](https://docs.docker.com/engine/install) to install Docker on your
-host computer. For ease of use, it is recommended to copy the `hazen-app`
-script to a location accessible on the path such as `/usr/local/bin`. This will
-allow you to run hazen from any location on your computer. Then, to use Docker
-hazen, simply run the `hazen-app` script appended with the function you want to
-use (e.g.: `snr`). In Terminal: ```bash cd hazen cp ./hazen-app /usr/local/bin
-# run hazen with CLI arguments hazen-app snr tests/data/snr/Siemens/ latest:
-Pulling from gsttmriphysics/hazen Digest: sha256:
+#### Updating hazen If you already have an old version of hazen installed,
+upgrade to the latest version with: ```shell source hazen-venv/bin/activate pip
+install --upgrade pip pip install --upgrade hazen ``` #### Running hazen via
+CLI The CLI version of hazen is designed to be pointed at single folders
+containing DICOM file(s). Example datasets are provided in the `tests/data/
+` directory. If you are using the Docker version of hazen (installation
+described below), replace `hazen` with `hazen-app` in the following commands.
+```bash # To see the full list of available Tasks, enter: hazen -h # To perform
+the spatial resolution Task on example data: hazen spatial_resolution tests/
+data/resolution/philips # To perform the SNR Task on example data: hazen snr
+tests/data/snr/Philips # The `--report` option provides additional information
+about the image processing measurement methods and is available # for all
+Tasks. Example usage for the SNR Task, which returns images showing the regions
+used for SNR calculation. hazen snr tests/data/snr/Philips --report ``` ### 2)
+Docker The Docker version of hazen has been made available as it is easy to get
+up-and-running and is linked to the most recent stable release. Refer to the
+[Docker installation instructions](https://docs.docker.com/engine/install) to
+install Docker on your host computer. The containerised version of hazen can be
+obtained from DockerHub (see commands below). For ease of use, it is
+recommended to copy the `hazen-app` script to a location accessible on the PATH
+such as `/usr/local/bin`. This will allow you to run hazen from any directory
+on your computer. Then, to use Docker hazen, simply run the `hazen-app` script
+appended with the function you want to use (e.g.: `snr`). In Terminal: ```shell
+# Ensure Docker installed and running, then pull the latest hazen Docker
+container docker pull gsttmriphysics/hazen:latest # Command line output will
+look something like: latest: Pulling from gsttmriphysics/hazen Digest: sha256:
 18603e40b45f3af4bf45f07559a08a7833af92a6efe21cb7306f758e8eeab24a Status: Image
 is up to date for gsttmriphysics/hazen:latest docker.io/gsttmriphysics/hazen:
-latest
-{ 'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
-191.16,
-'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
-195.58,
-'snr_smoothing_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
-1866.09,
-'snr_smoothing_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
-1909.2,
-'snr_subtraction_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+latest # Copy the 'hazen-app' executable file into your local bin folder cd
+hazen cp hazen-app /usr/local/bin # Run hazen via Docker with the normal CLI
+inputs hazen-app snr tests/data/snr/Siemens/ # Example command line output for
+the SNR Task:
+{ 'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+173.97,
+'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
+177.91,
+'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+1698.21,
+'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
+1736.66,
+'snr_subtraction_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
 220.73,
-'snr_subtraction_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
-2154.69} ``` #### Linux & MacOS For developers, hazen can be installed from
-source using `pip`. We highly recommend using a virtual environment. ```bash #
-Install OpenSSL # Go to local hazen repo directory cd hazen # Create and
-activate a virtual environment python3 -m venv ./hazen-venv source hazen-venv/
-bin/activate # Install requirements pip install --upgrade pip setuptools wheel
-pip install -r requirements.txt # Install hazen pip install . # Run tests to
-ensure everything is working pytest tests/ ``` --- ## Usage ### Command Line
-The CLI version of hazen is designed to be pointed at single folders containing
-DICOM file(s). Example datasets are provided in the `tests/data/` directory. If
-you are not using the Docker version of hazen, replace `hazen-app` with `hazen`
-in the following commands. To perform an SNR measurement on the provided
-example Philips DICOMs: `hazen-app snr tests/data/snr/Philips` To perform a
-spatial resolution measurement on example data provided by the East Kent Trust:
-`hazen-app spatial_resolution tests/data/resolution/philips` To see the full
-list of available tools, enter: `hazen-app -h` The `--report` option provides
-additional information for some of the functions. For example, the user can
-gain additional insight into the performance of the snr function by entering:
-`hazen-app snr tests/data/snr/Philips --report` ### Web Interface WIP: we are
-developing a web interface for hazen. --- ## Contributing - The Release Manager
-should create a release branch for the future planned release e.g. release-
-X.X.X - The RMs shall organise backlog refinement sessions to ensure issues are
-allocated to the appropriate release - The RM should ensure their release
-branch is kept up-to-date with master - PRs should be merged into the
-appropriate release branch for the issue(s) it is addressing If you want to
-contribute to the development of hazen, please take a look at:
-`CONTRIBUTING.md`. --- ## Users Please [raise an Issue](https://github.com/
-GSTT-CSC/hazen/issues) if you have any problems installing or running hazen. We
-have used hazen with MRI data from a handful of different MRI scanners,
-including multiple different vendors. If your MRI data doesn't work with hazen,
-or the results are unexpected, please submit an Issue and we will investigate.
---- ## Releasing The Release Manager should ensure: - All outstanding issues
-for the current release have been closed, or, transferred to future release. -
-All tests are passing on GitHub Actions. - All documentation has been updated
-with correct version numbers: - Update version number `hazenlib/_version.py`,
-i.e. imported into `docs/conf.py`, `hazenlib/__init__.py` and `setup.cfg` -
-Update version number in `CITATION.cff` - The `release` branch has been merged
-into `main` branch - A new release has been created with a new version tag (tag
-= version number) - RMs of other branches should update their release from the
-latest release as soon as possible and deal with any merge conflicts. ![image]
-(https://user-images.githubusercontent.com/19840489/143266366-06e33949-12c7-
-44b4-9ed7-c0a795b5d492.png) - RMs: Tom Roberts, Lucrezia Cester
+'snr_subtraction_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+2154.69 } ``` ### Web Interface Development of a [web interface for hazen]
+(https://github.com/GSTT-CSC/hazen-web-app) is in progress. --- ## Contributing
+to hazen ### Users Please [raise an Issue](https://github.com/GSTT-CSC/hazen/
+issues) for any of the following reasons: - Problems installing or running
+hazen - Suggestions for improvements - Requests for new features We have used
+hazen with MRI data from a handful of different MRI scanners, including
+multiple different vendors. If hazen does not perform with your MRI data, or
+the results are unexpected, please raise an Issue. ### Developers Please see
+[CONTRIBUTING.md](CONTRIBUTING.md) for developer guidelines. ---
```

### Comparing `hazen-1.2.0/README.md` & `hazen-1.3.0/hazen.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,22 @@
+Metadata-Version: 2.1
+Name: hazen
+Version: 1.3.0
+Summary: An automatic MRI QA tool
+Home-page: https://bitbucket.org/gsttmri/hazen
+Author: Shuaib, Haris
+Author-email: mohammad_haris.shuaib@kcl.ac.uk
+Requires-Python: <3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 <!-- PROJECT HEADING -->
 <br />
 <p align="center">
-<img src="https://raw.githubusercontent.com/GSTT-CSC/hazen/readme-dev/docs/assets/ibn-al-haytham.jpeg" alt="Ibn Al-Haytham">
+<img src="https://upload.wikimedia.org/wikipedia/commons/a/a3/Ibn_Al-Haytham_portrait.jpg" alt="Ibn Al-Haytham" width="512">
 </p>   
 <h1 align="center">hazen</h1>
 <p align="center">
 Quality assurance framework for Magnetic Resonance Imaging
 <br />
 <a href="https://hazen.readthedocs.io/en/latest/"><strong>Explore the docs »</strong></a>
 <br />
@@ -22,154 +33,151 @@
 </p>
 <p align="center">Please <b>STAR</b> this repo to receive updates about new versions of hazen!</p>
 
 ---
 
 ## Overview
 
-hazen is a software framework for performing automated analysis of magnetic resonance imaging (MRI) Quality Assurance data.
+hazen is a software framework for performing automated analysis of magnetic resonance imaging (MRI) quality assurance 
+(QA) data. hazen consists of multiple [Tasks](hazenlib/tasks) which perform quantitative processing and analysis of 
+MRI phantom data. Currently, hazen supports the [ACR Large MRI Phantom](https://www.acraccreditation.org/-/media/acraccreditation/documents/mri/largephantomguidance.pdf)
+and the MagNET Test Objects collection of phantoms.
 
-It provides automatic quantitative analysis for the following measurements of MRI phantom data:
+The hazen Tasks provide the following measurements within these phantoms:
 - Signal-to-noise ratio (SNR)
 - Spatial resolution
-- Slice position and width
+- Slice position
+- Slice width
 - Uniformity
 - Ghosting
-- MR Relaxometry
+- MR relaxometry
+
+Each Task outputs numerical results to the user's terminal. Below is an output from the `hazen snr` Task performed on 
+some example MRI data:
+
+```shell
+hazen snr tests/data/snr/Siemens
+{
+  'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 173.97,
+  'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 177.91,
+  'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 1698.21,
+  'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 1736.66,
+  'snr_subtraction_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 220.73,
+  'snr_subtraction_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 2154.69
+}
+```
 
-Some example outputs from hazen:
+The optional `--report` flag allows the user to visualise the image processing performed by each hazen Task:
 
-| hazen acr_ghosting                        | hazen ghosting                |
-|----------------------------------|-------------------------------|
-| ![](docs/assets/SNR.png) | ![](docs/assets/ghosting.png) |
+| `hazen snr tests/data/snr/Siemens --report` | `hazen acr_ghosting tests/data/acr/Siemens --report` |
+|---------------------------------------------|------------------------------------------------------|
+| <img src="/docs/assets/snr.jpg?raw=true"> | <img src="/docs/assets/acr_ghosting.jpg?raw=true"> |
 
 ---
 
-## Installation
+## Installation and usage
+
+There are two main options for running hazen.
+1. Install using Python and run directly via command line interface (CLI)
+2. Run using the latest Docker container build
 
-### pip
+### 1) Python install and run (CLI)
 
-Hazen can be installed using pip on python 3.9 or higher, it is recommended to use a virtual environment
+hazen can be installed with Python 3.9 or higher via pip. It is strongly recommended to use a virtual environment.
 
 ```bash
 python3 -m venv hazen-venv
 source hazen-venv/bin/activate
 pip install hazen
 ```
 
-#### Docker
-
-The Docker version of hazen as it is easy to get up-and-running and is linked to the most stable release. Refer to the [Docker installation instructions](https://docs.docker.com/engine/install) to install Docker on your host computer.
+#### Updating hazen
+If you already have an old version of hazen installed, upgrade to the latest version with:
 
-For ease of use, it is recommended to copy the `hazen-app` script to a location accessible on the path such as `/usr/local/bin`. This will allow you to run hazen from any location on your computer. Then, to use Docker hazen, simply run the `hazen-app` script appended with the function you want to use (e.g.: `snr`). 
-
-In Terminal:
-
-```bash 
-cd hazen
-cp ./hazen-app /usr/local/bin
-
-# run hazen with CLI arguments
-hazen-app snr tests/data/snr/Siemens/
-
-latest: Pulling from gsttmriphysics/hazen
-Digest: sha256:18603e40b45f3af4bf45f07559a08a7833af92a6efe21cb7306f758e8eeab24a
-Status: Image is up to date for gsttmriphysics/hazen:latest
-docker.io/gsttmriphysics/hazen:latest
-{   'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 191.16,
-    'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 195.58,
-    'snr_smoothing_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 1866.09,
-    'snr_smoothing_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 1909.2,
-    'snr_subtraction_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 220.73,
-    'snr_subtraction_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 2154.69}
+```shell
+source hazen-venv/bin/activate
+pip install --upgrade pip
+pip install --upgrade hazen
 ```
 
-
-#### Linux & MacOS
-
-For developers, hazen can be installed from source using `pip`. We highly recommend using a virtual environment.
+#### Running hazen via CLI
+The CLI version of hazen is designed to be pointed at single folders containing DICOM file(s). Example datasets are 
+provided in the `tests/data/` directory. If you are using the Docker version of hazen (installation described below), 
+replace `hazen` with `hazen-app` in the following commands.
 
 ```bash
-# Install OpenSSL
-# Go to local hazen repo directory
-cd hazen
-
-# Create and activate a virtual environment
-python3 -m venv ./hazen-venv
-source hazen-venv/bin/activate
+# To see the full list of available Tasks, enter:
+hazen -h
 
-# Install requirements
-pip install --upgrade pip setuptools wheel
-pip install -r requirements.txt
+# To perform the spatial resolution Task on example data:
+hazen spatial_resolution tests/data/resolution/philips
 
-# Install hazen
-pip install .
+# To perform the SNR Task on example data:
+hazen snr tests/data/snr/Philips
 
-# Run tests to ensure everything is working
-pytest tests/
+# The `--report` option provides additional information about the image processing measurement methods and is available 
+# for all Tasks. Example usage for the SNR Task, which returns images showing the regions used for SNR calculation.
+hazen snr tests/data/snr/Philips --report
 ```
 
----
-
-## Usage
-
-### Command Line
+### 2) Docker
 
-The CLI version of hazen is designed to be pointed at single folders containing DICOM file(s). Example datasets are provided in the `tests/data/` directory. If you are not using the Docker version of hazen, replace `hazen-app` with `hazen` in the following commands.
+The Docker version of hazen has been made available as it is easy to get up-and-running and is linked to the most recent 
+stable release. Refer to the [Docker installation instructions](https://docs.docker.com/engine/install) to install 
+Docker on your host computer.
+
+The containerised version of hazen can be obtained from DockerHub (see commands below). For ease of use, it is 
+recommended to copy the `hazen-app` script to a location accessible on the PATH such as `/usr/local/bin`. This will 
+allow you to run hazen from any directory on your computer. Then, to use Docker hazen, simply run the `hazen-app` script 
+appended with the function you want to use (e.g.: `snr`). 
 
-To perform an SNR measurement on the provided example Philips DICOMs:
-
-`hazen-app snr tests/data/snr/Philips`
-
-To perform a spatial resolution measurement on example data provided by the East Kent Trust:
+In Terminal:
 
-`hazen-app spatial_resolution tests/data/resolution/philips`
+```shell
+# Ensure Docker installed and running, then pull the latest hazen Docker container
+docker pull gsttmriphysics/hazen:latest
 
-To see the full list of available tools, enter:
+# Command line output will look something like:
+latest: Pulling from gsttmriphysics/hazen
+Digest: sha256:18603e40b45f3af4bf45f07559a08a7833af92a6efe21cb7306f758e8eeab24a
+Status: Image is up to date for gsttmriphysics/hazen:latest
+docker.io/gsttmriphysics/hazen:latest
 
-`hazen-app -h`
+# Copy the 'hazen-app' executable file into your local bin folder
+cd hazen
+cp hazen-app /usr/local/bin
 
-The `--report` option provides additional information for some of the functions. For example, the user can gain additional insight into the performance of the snr function by entering:
+# Run hazen via Docker with the normal CLI inputs
+hazen-app snr tests/data/snr/Siemens/
 
-`hazen-app snr tests/data/snr/Philips --report`
+# Example command line output for the SNR Task:
+{
+  'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 173.97,
+  'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 177.91,
+  'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 1698.21,
+  'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 1736.66,
+  'snr_subtraction_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 220.73,
+  'snr_subtraction_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 2154.69
+}
+```
 
 ### Web Interface
 
-WIP: we are developing a web interface for hazen.
+Development of a [web interface for hazen](https://github.com/GSTT-CSC/hazen-web-app) is in progress.
 
 ---
 
-## Contributing
-- The Release Manager should create a release branch for the future planned release e.g. release-X.X.X
-- The RMs shall organise backlog refinement sessions to ensure issues are allocated to the appropriate release
-- The RM should ensure their release branch is kept up-to-date with master
-- PRs should be merged into the appropriate release branch for the issue(s) it is addressing
-
-If you want to contribute to the development of hazen, please take a look at: `CONTRIBUTING.md`.
+## Contributing to hazen
 
----
-
-## Users
+### Users
+Please [raise an Issue](https://github.com/GSTT-CSC/hazen/issues) for any of the following reasons:
+- Problems installing or running hazen
+- Suggestions for improvements
+- Requests for new features
 
-Please [raise an Issue](https://github.com/GSTT-CSC/hazen/issues) if you have any problems installing or running hazen.
+We have used hazen with MRI data from a handful of different MRI scanners, including multiple different vendors. If 
+hazen does not perform with your MRI data, or the results are unexpected, please raise an Issue.
 
-We have used hazen with MRI data from a handful of different MRI scanners, including multiple different vendors. If your MRI data doesn't work with hazen, or the results are unexpected, please submit an Issue and we will investigate. 
+### Developers
+Please see [CONTRIBUTING.md](CONTRIBUTING.md) for developer guidelines.
 
 ---
-
-## Releasing
-
-The Release Manager should ensure:
-- All outstanding issues for the current release have been closed, or, transferred to future release.
-- All tests are passing on GitHub Actions.
-- All documentation has been updated with correct version numbers:
-   - Update version number `hazenlib/_version.py`, i.e. imported into `docs/conf.py`, `hazenlib/__init__.py` and `setup.cfg`
-   - Update version number in `CITATION.cff`
-- The `release` branch has been merged into `main` branch
-- A new release has been created with a new version tag (tag = version number)
-
-- RMs of other branches should update their release from the latest release as soon as possible and deal with any merge conflicts.
-
-![image](https://user-images.githubusercontent.com/19840489/143266366-06e33949-12c7-44b4-9ed7-c0a795b5d492.png)
-
-- RMs: Tom Roberts, Lucrezia Cester
-
```

#### html2text {}

```diff
@@ -1,87 +1,101 @@
-
+Metadata-Version: 2.1 Name: hazen Version: 1.3.0 Summary: An automatic MRI QA
+tool Home-page: https://bitbucket.org/gsttmri/hazen Author: Shuaib, Haris
+Author-email: mohammad_haris.shuaib@kcl.ac.uk Requires-Python: <3.11
+Description-Content-Type: text/markdown License-File: LICENSE.txt
                                [Ibn Al-Haytham]
                               ****** hazen ******
           Quality assurance framework for Magnetic Resonance Imaging
                              Explore_the_docs_Â»
 
                   View_repo Â· Report_Bug Â· Request_Feature
     [https://github.com/GSTT-CSC/hazen/actions/workflows/tests_release.yml/
      badge.svg?branch=main] [https://img.shields.io/endpoint?url=https://
  gist.githubusercontent.com/laurencejackson/ba102d5f3e592fcd50451c2eff8a803d/
                     raw/hazen_pytest-coverage-comment.json]
      Please STAR this repo to receive updates about new versions of hazen!
 --- ## Overview hazen is a software framework for performing automated analysis
-of magnetic resonance imaging (MRI) Quality Assurance data. It provides
-automatic quantitative analysis for the following measurements of MRI phantom
-data: - Signal-to-noise ratio (SNR) - Spatial resolution - Slice position and
-width - Uniformity - Ghosting - MR Relaxometry Some example outputs from hazen:
-| hazen acr_ghosting | hazen ghosting | |----------------------------------|---
-----------------------------| | ![](docs/assets/SNR.png) | ![](docs/assets/
-ghosting.png) | --- ## Installation ### pip Hazen can be installed using pip on
-python 3.9 or higher, it is recommended to use a virtual environment ```bash
+of magnetic resonance imaging (MRI) quality assurance (QA) data. hazen consists
+of multiple [Tasks](hazenlib/tasks) which perform quantitative processing and
+analysis of MRI phantom data. Currently, hazen supports the [ACR Large MRI
+Phantom](https://www.acraccreditation.org/-/media/acraccreditation/documents/
+mri/largephantomguidance.pdf) and the MagNET Test Objects collection of
+phantoms. The hazen Tasks provide the following measurements within these
+phantoms: - Signal-to-noise ratio (SNR) - Spatial resolution - Slice position -
+Slice width - Uniformity - Ghosting - MR relaxometry Each Task outputs
+numerical results to the user's terminal. Below is an output from the `hazen
+snr` Task performed on some example MRI data: ```shell hazen snr tests/data/
+snr/Siemens
+{ 'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+173.97,
+'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
+177.91,
+'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+1698.21,
+'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
+1736.66,
+'snr_subtraction_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+220.73,
+'snr_subtraction_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+2154.69 } ``` The optional `--report` flag allows the user to visualise the
+image processing performed by each hazen Task: | `hazen snr tests/data/snr/
+Siemens --report` | `hazen acr_ghosting tests/data/acr/Siemens --report` | |---
+------------------------------------------|------------------------------------
+------------------| | [/docs/assets/snr.jpg?raw=true] | [/docs/assets/
+acr_ghosting.jpg?raw=true] | --- ## Installation and usage There are two main
+options for running hazen. 1. Install using Python and run directly via command
+line interface (CLI) 2. Run using the latest Docker container build ### 1)
+Python install and run (CLI) hazen can be installed with Python 3.9 or higher
+via pip. It is strongly recommended to use a virtual environment. ```bash
 python3 -m venv hazen-venv source hazen-venv/bin/activate pip install hazen ```
-#### Docker The Docker version of hazen as it is easy to get up-and-running and
-is linked to the most stable release. Refer to the [Docker installation
-instructions](https://docs.docker.com/engine/install) to install Docker on your
-host computer. For ease of use, it is recommended to copy the `hazen-app`
-script to a location accessible on the path such as `/usr/local/bin`. This will
-allow you to run hazen from any location on your computer. Then, to use Docker
-hazen, simply run the `hazen-app` script appended with the function you want to
-use (e.g.: `snr`). In Terminal: ```bash cd hazen cp ./hazen-app /usr/local/bin
-# run hazen with CLI arguments hazen-app snr tests/data/snr/Siemens/ latest:
-Pulling from gsttmriphysics/hazen Digest: sha256:
+#### Updating hazen If you already have an old version of hazen installed,
+upgrade to the latest version with: ```shell source hazen-venv/bin/activate pip
+install --upgrade pip pip install --upgrade hazen ``` #### Running hazen via
+CLI The CLI version of hazen is designed to be pointed at single folders
+containing DICOM file(s). Example datasets are provided in the `tests/data/
+` directory. If you are using the Docker version of hazen (installation
+described below), replace `hazen` with `hazen-app` in the following commands.
+```bash # To see the full list of available Tasks, enter: hazen -h # To perform
+the spatial resolution Task on example data: hazen spatial_resolution tests/
+data/resolution/philips # To perform the SNR Task on example data: hazen snr
+tests/data/snr/Philips # The `--report` option provides additional information
+about the image processing measurement methods and is available # for all
+Tasks. Example usage for the SNR Task, which returns images showing the regions
+used for SNR calculation. hazen snr tests/data/snr/Philips --report ``` ### 2)
+Docker The Docker version of hazen has been made available as it is easy to get
+up-and-running and is linked to the most recent stable release. Refer to the
+[Docker installation instructions](https://docs.docker.com/engine/install) to
+install Docker on your host computer. The containerised version of hazen can be
+obtained from DockerHub (see commands below). For ease of use, it is
+recommended to copy the `hazen-app` script to a location accessible on the PATH
+such as `/usr/local/bin`. This will allow you to run hazen from any directory
+on your computer. Then, to use Docker hazen, simply run the `hazen-app` script
+appended with the function you want to use (e.g.: `snr`). In Terminal: ```shell
+# Ensure Docker installed and running, then pull the latest hazen Docker
+container docker pull gsttmriphysics/hazen:latest # Command line output will
+look something like: latest: Pulling from gsttmriphysics/hazen Digest: sha256:
 18603e40b45f3af4bf45f07559a08a7833af92a6efe21cb7306f758e8eeab24a Status: Image
 is up to date for gsttmriphysics/hazen:latest docker.io/gsttmriphysics/hazen:
-latest
-{ 'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
-191.16,
-'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
-195.58,
-'snr_smoothing_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
-1866.09,
-'snr_smoothing_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
-1909.2,
-'snr_subtraction_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+latest # Copy the 'hazen-app' executable file into your local bin folder cd
+hazen cp hazen-app /usr/local/bin # Run hazen via Docker with the normal CLI
+inputs hazen-app snr tests/data/snr/Siemens/ # Example command line output for
+the SNR Task:
+{ 'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+173.97,
+'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
+177.91,
+'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+1698.21,
+'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
+1736.66,
+'snr_subtraction_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
 220.73,
-'snr_subtraction_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
-2154.69} ``` #### Linux & MacOS For developers, hazen can be installed from
-source using `pip`. We highly recommend using a virtual environment. ```bash #
-Install OpenSSL # Go to local hazen repo directory cd hazen # Create and
-activate a virtual environment python3 -m venv ./hazen-venv source hazen-venv/
-bin/activate # Install requirements pip install --upgrade pip setuptools wheel
-pip install -r requirements.txt # Install hazen pip install . # Run tests to
-ensure everything is working pytest tests/ ``` --- ## Usage ### Command Line
-The CLI version of hazen is designed to be pointed at single folders containing
-DICOM file(s). Example datasets are provided in the `tests/data/` directory. If
-you are not using the Docker version of hazen, replace `hazen-app` with `hazen`
-in the following commands. To perform an SNR measurement on the provided
-example Philips DICOMs: `hazen-app snr tests/data/snr/Philips` To perform a
-spatial resolution measurement on example data provided by the East Kent Trust:
-`hazen-app spatial_resolution tests/data/resolution/philips` To see the full
-list of available tools, enter: `hazen-app -h` The `--report` option provides
-additional information for some of the functions. For example, the user can
-gain additional insight into the performance of the snr function by entering:
-`hazen-app snr tests/data/snr/Philips --report` ### Web Interface WIP: we are
-developing a web interface for hazen. --- ## Contributing - The Release Manager
-should create a release branch for the future planned release e.g. release-
-X.X.X - The RMs shall organise backlog refinement sessions to ensure issues are
-allocated to the appropriate release - The RM should ensure their release
-branch is kept up-to-date with master - PRs should be merged into the
-appropriate release branch for the issue(s) it is addressing If you want to
-contribute to the development of hazen, please take a look at:
-`CONTRIBUTING.md`. --- ## Users Please [raise an Issue](https://github.com/
-GSTT-CSC/hazen/issues) if you have any problems installing or running hazen. We
-have used hazen with MRI data from a handful of different MRI scanners,
-including multiple different vendors. If your MRI data doesn't work with hazen,
-or the results are unexpected, please submit an Issue and we will investigate.
---- ## Releasing The Release Manager should ensure: - All outstanding issues
-for the current release have been closed, or, transferred to future release. -
-All tests are passing on GitHub Actions. - All documentation has been updated
-with correct version numbers: - Update version number `hazenlib/_version.py`,
-i.e. imported into `docs/conf.py`, `hazenlib/__init__.py` and `setup.cfg` -
-Update version number in `CITATION.cff` - The `release` branch has been merged
-into `main` branch - A new release has been created with a new version tag (tag
-= version number) - RMs of other branches should update their release from the
-latest release as soon as possible and deal with any merge conflicts. ![image]
-(https://user-images.githubusercontent.com/19840489/143266366-06e33949-12c7-
-44b4-9ed7-c0a795b5d492.png) - RMs: Tom Roberts, Lucrezia Cester
+'snr_subtraction_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+2154.69 } ``` ### Web Interface Development of a [web interface for hazen]
+(https://github.com/GSTT-CSC/hazen-web-app) is in progress. --- ## Contributing
+to hazen ### Users Please [raise an Issue](https://github.com/GSTT-CSC/hazen/
+issues) for any of the following reasons: - Problems installing or running
+hazen - Suggestions for improvements - Requests for new features We have used
+hazen with MRI data from a handful of different MRI scanners, including
+multiple different vendors. If hazen does not perform with your MRI data, or
+the results are unexpected, please raise an Issue. ### Developers Please see
+[CONTRIBUTING.md](CONTRIBUTING.md) for developer guidelines. ---
```

### Comparing `hazen-1.2.0/hazen.egg-info/PKG-INFO` & `hazen-1.3.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,11 @@
-Metadata-Version: 2.1
-Name: hazen
-Version: 1.2.0
-Summary: An automatic MRI QA tool
-Home-page: https://bitbucket.org/gsttmri/hazen
-Author: Shuaib, Haris
-Author-email: mohammad_haris.shuaib@kcl.ac.uk
-Requires-Python: <3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 <!-- PROJECT HEADING -->
 <br />
 <p align="center">
-<img src="https://raw.githubusercontent.com/GSTT-CSC/hazen/readme-dev/docs/assets/ibn-al-haytham.jpeg" alt="Ibn Al-Haytham">
+<img src="https://upload.wikimedia.org/wikipedia/commons/a/a3/Ibn_Al-Haytham_portrait.jpg" alt="Ibn Al-Haytham" width="512">
 </p>   
 <h1 align="center">hazen</h1>
 <p align="center">
 Quality assurance framework for Magnetic Resonance Imaging
 <br />
 <a href="https://hazen.readthedocs.io/en/latest/"><strong>Explore the docs »</strong></a>
 <br />
@@ -33,154 +22,151 @@
 </p>
 <p align="center">Please <b>STAR</b> this repo to receive updates about new versions of hazen!</p>
 
 ---
 
 ## Overview
 
-hazen is a software framework for performing automated analysis of magnetic resonance imaging (MRI) Quality Assurance data.
+hazen is a software framework for performing automated analysis of magnetic resonance imaging (MRI) quality assurance 
+(QA) data. hazen consists of multiple [Tasks](hazenlib/tasks) which perform quantitative processing and analysis of 
+MRI phantom data. Currently, hazen supports the [ACR Large MRI Phantom](https://www.acraccreditation.org/-/media/acraccreditation/documents/mri/largephantomguidance.pdf)
+and the MagNET Test Objects collection of phantoms.
 
-It provides automatic quantitative analysis for the following measurements of MRI phantom data:
+The hazen Tasks provide the following measurements within these phantoms:
 - Signal-to-noise ratio (SNR)
 - Spatial resolution
-- Slice position and width
+- Slice position
+- Slice width
 - Uniformity
 - Ghosting
-- MR Relaxometry
+- MR relaxometry
+
+Each Task outputs numerical results to the user's terminal. Below is an output from the `hazen snr` Task performed on 
+some example MRI data:
+
+```shell
+hazen snr tests/data/snr/Siemens
+{
+  'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 173.97,
+  'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 177.91,
+  'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 1698.21,
+  'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 1736.66,
+  'snr_subtraction_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 220.73,
+  'snr_subtraction_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 2154.69
+}
+```
 
-Some example outputs from hazen:
+The optional `--report` flag allows the user to visualise the image processing performed by each hazen Task:
 
-| hazen acr_ghosting                        | hazen ghosting                |
-|----------------------------------|-------------------------------|
-| ![](docs/assets/SNR.png) | ![](docs/assets/ghosting.png) |
+| `hazen snr tests/data/snr/Siemens --report` | `hazen acr_ghosting tests/data/acr/Siemens --report` |
+|---------------------------------------------|------------------------------------------------------|
+| <img src="/docs/assets/snr.jpg?raw=true"> | <img src="/docs/assets/acr_ghosting.jpg?raw=true"> |
 
 ---
 
-## Installation
+## Installation and usage
+
+There are two main options for running hazen.
+1. Install using Python and run directly via command line interface (CLI)
+2. Run using the latest Docker container build
 
-### pip
+### 1) Python install and run (CLI)
 
-Hazen can be installed using pip on python 3.9 or higher, it is recommended to use a virtual environment
+hazen can be installed with Python 3.9 or higher via pip. It is strongly recommended to use a virtual environment.
 
 ```bash
 python3 -m venv hazen-venv
 source hazen-venv/bin/activate
 pip install hazen
 ```
 
-#### Docker
-
-The Docker version of hazen as it is easy to get up-and-running and is linked to the most stable release. Refer to the [Docker installation instructions](https://docs.docker.com/engine/install) to install Docker on your host computer.
+#### Updating hazen
+If you already have an old version of hazen installed, upgrade to the latest version with:
 
-For ease of use, it is recommended to copy the `hazen-app` script to a location accessible on the path such as `/usr/local/bin`. This will allow you to run hazen from any location on your computer. Then, to use Docker hazen, simply run the `hazen-app` script appended with the function you want to use (e.g.: `snr`). 
-
-In Terminal:
-
-```bash 
-cd hazen
-cp ./hazen-app /usr/local/bin
-
-# run hazen with CLI arguments
-hazen-app snr tests/data/snr/Siemens/
-
-latest: Pulling from gsttmriphysics/hazen
-Digest: sha256:18603e40b45f3af4bf45f07559a08a7833af92a6efe21cb7306f758e8eeab24a
-Status: Image is up to date for gsttmriphysics/hazen:latest
-docker.io/gsttmriphysics/hazen:latest
-{   'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 191.16,
-    'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 195.58,
-    'snr_smoothing_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 1866.09,
-    'snr_smoothing_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 1909.2,
-    'snr_subtraction_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 220.73,
-    'snr_subtraction_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 2154.69}
+```shell
+source hazen-venv/bin/activate
+pip install --upgrade pip
+pip install --upgrade hazen
 ```
 
-
-#### Linux & MacOS
-
-For developers, hazen can be installed from source using `pip`. We highly recommend using a virtual environment.
+#### Running hazen via CLI
+The CLI version of hazen is designed to be pointed at single folders containing DICOM file(s). Example datasets are 
+provided in the `tests/data/` directory. If you are using the Docker version of hazen (installation described below), 
+replace `hazen` with `hazen-app` in the following commands.
 
 ```bash
-# Install OpenSSL
-# Go to local hazen repo directory
-cd hazen
-
-# Create and activate a virtual environment
-python3 -m venv ./hazen-venv
-source hazen-venv/bin/activate
+# To see the full list of available Tasks, enter:
+hazen -h
 
-# Install requirements
-pip install --upgrade pip setuptools wheel
-pip install -r requirements.txt
+# To perform the spatial resolution Task on example data:
+hazen spatial_resolution tests/data/resolution/philips
 
-# Install hazen
-pip install .
+# To perform the SNR Task on example data:
+hazen snr tests/data/snr/Philips
 
-# Run tests to ensure everything is working
-pytest tests/
+# The `--report` option provides additional information about the image processing measurement methods and is available 
+# for all Tasks. Example usage for the SNR Task, which returns images showing the regions used for SNR calculation.
+hazen snr tests/data/snr/Philips --report
 ```
 
----
-
-## Usage
-
-### Command Line
+### 2) Docker
 
-The CLI version of hazen is designed to be pointed at single folders containing DICOM file(s). Example datasets are provided in the `tests/data/` directory. If you are not using the Docker version of hazen, replace `hazen-app` with `hazen` in the following commands.
+The Docker version of hazen has been made available as it is easy to get up-and-running and is linked to the most recent 
+stable release. Refer to the [Docker installation instructions](https://docs.docker.com/engine/install) to install 
+Docker on your host computer.
+
+The containerised version of hazen can be obtained from DockerHub (see commands below). For ease of use, it is 
+recommended to copy the `hazen-app` script to a location accessible on the PATH such as `/usr/local/bin`. This will 
+allow you to run hazen from any directory on your computer. Then, to use Docker hazen, simply run the `hazen-app` script 
+appended with the function you want to use (e.g.: `snr`). 
 
-To perform an SNR measurement on the provided example Philips DICOMs:
-
-`hazen-app snr tests/data/snr/Philips`
-
-To perform a spatial resolution measurement on example data provided by the East Kent Trust:
+In Terminal:
 
-`hazen-app spatial_resolution tests/data/resolution/philips`
+```shell
+# Ensure Docker installed and running, then pull the latest hazen Docker container
+docker pull gsttmriphysics/hazen:latest
 
-To see the full list of available tools, enter:
+# Command line output will look something like:
+latest: Pulling from gsttmriphysics/hazen
+Digest: sha256:18603e40b45f3af4bf45f07559a08a7833af92a6efe21cb7306f758e8eeab24a
+Status: Image is up to date for gsttmriphysics/hazen:latest
+docker.io/gsttmriphysics/hazen:latest
 
-`hazen-app -h`
+# Copy the 'hazen-app' executable file into your local bin folder
+cd hazen
+cp hazen-app /usr/local/bin
 
-The `--report` option provides additional information for some of the functions. For example, the user can gain additional insight into the performance of the snr function by entering:
+# Run hazen via Docker with the normal CLI inputs
+hazen-app snr tests/data/snr/Siemens/
 
-`hazen-app snr tests/data/snr/Philips --report`
+# Example command line output for the SNR Task:
+{
+  'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 173.97,
+  'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 177.91,
+  'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 1698.21,
+  'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1': 1736.66,
+  'snr_subtraction_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 220.73,
+  'snr_subtraction_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1': 2154.69
+}
+```
 
 ### Web Interface
 
-WIP: we are developing a web interface for hazen.
+Development of a [web interface for hazen](https://github.com/GSTT-CSC/hazen-web-app) is in progress.
 
 ---
 
-## Contributing
-- The Release Manager should create a release branch for the future planned release e.g. release-X.X.X
-- The RMs shall organise backlog refinement sessions to ensure issues are allocated to the appropriate release
-- The RM should ensure their release branch is kept up-to-date with master
-- PRs should be merged into the appropriate release branch for the issue(s) it is addressing
-
-If you want to contribute to the development of hazen, please take a look at: `CONTRIBUTING.md`.
+## Contributing to hazen
 
----
-
-## Users
+### Users
+Please [raise an Issue](https://github.com/GSTT-CSC/hazen/issues) for any of the following reasons:
+- Problems installing or running hazen
+- Suggestions for improvements
+- Requests for new features
 
-Please [raise an Issue](https://github.com/GSTT-CSC/hazen/issues) if you have any problems installing or running hazen.
+We have used hazen with MRI data from a handful of different MRI scanners, including multiple different vendors. If 
+hazen does not perform with your MRI data, or the results are unexpected, please raise an Issue.
 
-We have used hazen with MRI data from a handful of different MRI scanners, including multiple different vendors. If your MRI data doesn't work with hazen, or the results are unexpected, please submit an Issue and we will investigate. 
+### Developers
+Please see [CONTRIBUTING.md](CONTRIBUTING.md) for developer guidelines.
 
 ---
-
-## Releasing
-
-The Release Manager should ensure:
-- All outstanding issues for the current release have been closed, or, transferred to future release.
-- All tests are passing on GitHub Actions.
-- All documentation has been updated with correct version numbers:
-   - Update version number `hazenlib/_version.py`, i.e. imported into `docs/conf.py`, `hazenlib/__init__.py` and `setup.cfg`
-   - Update version number in `CITATION.cff`
-- The `release` branch has been merged into `main` branch
-- A new release has been created with a new version tag (tag = version number)
-
-- RMs of other branches should update their release from the latest release as soon as possible and deal with any merge conflicts.
-
-![image](https://user-images.githubusercontent.com/19840489/143266366-06e33949-12c7-44b4-9ed7-c0a795b5d492.png)
-
-- RMs: Tom Roberts, Lucrezia Cester
-
```

#### html2text {}

```diff
@@ -1,90 +1,98 @@
-Metadata-Version: 2.1 Name: hazen Version: 1.2.0 Summary: An automatic MRI QA
-tool Home-page: https://bitbucket.org/gsttmri/hazen Author: Shuaib, Haris
-Author-email: mohammad_haris.shuaib@kcl.ac.uk Requires-Python: <3.11
-Description-Content-Type: text/markdown License-File: LICENSE.txt
+
                                [Ibn Al-Haytham]
                               ****** hazen ******
           Quality assurance framework for Magnetic Resonance Imaging
                              Explore_the_docs_Â»
 
                   View_repo Â· Report_Bug Â· Request_Feature
     [https://github.com/GSTT-CSC/hazen/actions/workflows/tests_release.yml/
      badge.svg?branch=main] [https://img.shields.io/endpoint?url=https://
  gist.githubusercontent.com/laurencejackson/ba102d5f3e592fcd50451c2eff8a803d/
                     raw/hazen_pytest-coverage-comment.json]
      Please STAR this repo to receive updates about new versions of hazen!
 --- ## Overview hazen is a software framework for performing automated analysis
-of magnetic resonance imaging (MRI) Quality Assurance data. It provides
-automatic quantitative analysis for the following measurements of MRI phantom
-data: - Signal-to-noise ratio (SNR) - Spatial resolution - Slice position and
-width - Uniformity - Ghosting - MR Relaxometry Some example outputs from hazen:
-| hazen acr_ghosting | hazen ghosting | |----------------------------------|---
-----------------------------| | ![](docs/assets/SNR.png) | ![](docs/assets/
-ghosting.png) | --- ## Installation ### pip Hazen can be installed using pip on
-python 3.9 or higher, it is recommended to use a virtual environment ```bash
+of magnetic resonance imaging (MRI) quality assurance (QA) data. hazen consists
+of multiple [Tasks](hazenlib/tasks) which perform quantitative processing and
+analysis of MRI phantom data. Currently, hazen supports the [ACR Large MRI
+Phantom](https://www.acraccreditation.org/-/media/acraccreditation/documents/
+mri/largephantomguidance.pdf) and the MagNET Test Objects collection of
+phantoms. The hazen Tasks provide the following measurements within these
+phantoms: - Signal-to-noise ratio (SNR) - Spatial resolution - Slice position -
+Slice width - Uniformity - Ghosting - MR relaxometry Each Task outputs
+numerical results to the user's terminal. Below is an output from the `hazen
+snr` Task performed on some example MRI data: ```shell hazen snr tests/data/
+snr/Siemens
+{ 'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+173.97,
+'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
+177.91,
+'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+1698.21,
+'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
+1736.66,
+'snr_subtraction_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+220.73,
+'snr_subtraction_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+2154.69 } ``` The optional `--report` flag allows the user to visualise the
+image processing performed by each hazen Task: | `hazen snr tests/data/snr/
+Siemens --report` | `hazen acr_ghosting tests/data/acr/Siemens --report` | |---
+------------------------------------------|------------------------------------
+------------------| | [/docs/assets/snr.jpg?raw=true] | [/docs/assets/
+acr_ghosting.jpg?raw=true] | --- ## Installation and usage There are two main
+options for running hazen. 1. Install using Python and run directly via command
+line interface (CLI) 2. Run using the latest Docker container build ### 1)
+Python install and run (CLI) hazen can be installed with Python 3.9 or higher
+via pip. It is strongly recommended to use a virtual environment. ```bash
 python3 -m venv hazen-venv source hazen-venv/bin/activate pip install hazen ```
-#### Docker The Docker version of hazen as it is easy to get up-and-running and
-is linked to the most stable release. Refer to the [Docker installation
-instructions](https://docs.docker.com/engine/install) to install Docker on your
-host computer. For ease of use, it is recommended to copy the `hazen-app`
-script to a location accessible on the path such as `/usr/local/bin`. This will
-allow you to run hazen from any location on your computer. Then, to use Docker
-hazen, simply run the `hazen-app` script appended with the function you want to
-use (e.g.: `snr`). In Terminal: ```bash cd hazen cp ./hazen-app /usr/local/bin
-# run hazen with CLI arguments hazen-app snr tests/data/snr/Siemens/ latest:
-Pulling from gsttmriphysics/hazen Digest: sha256:
+#### Updating hazen If you already have an old version of hazen installed,
+upgrade to the latest version with: ```shell source hazen-venv/bin/activate pip
+install --upgrade pip pip install --upgrade hazen ``` #### Running hazen via
+CLI The CLI version of hazen is designed to be pointed at single folders
+containing DICOM file(s). Example datasets are provided in the `tests/data/
+` directory. If you are using the Docker version of hazen (installation
+described below), replace `hazen` with `hazen-app` in the following commands.
+```bash # To see the full list of available Tasks, enter: hazen -h # To perform
+the spatial resolution Task on example data: hazen spatial_resolution tests/
+data/resolution/philips # To perform the SNR Task on example data: hazen snr
+tests/data/snr/Philips # The `--report` option provides additional information
+about the image processing measurement methods and is available # for all
+Tasks. Example usage for the SNR Task, which returns images showing the regions
+used for SNR calculation. hazen snr tests/data/snr/Philips --report ``` ### 2)
+Docker The Docker version of hazen has been made available as it is easy to get
+up-and-running and is linked to the most recent stable release. Refer to the
+[Docker installation instructions](https://docs.docker.com/engine/install) to
+install Docker on your host computer. The containerised version of hazen can be
+obtained from DockerHub (see commands below). For ease of use, it is
+recommended to copy the `hazen-app` script to a location accessible on the PATH
+such as `/usr/local/bin`. This will allow you to run hazen from any directory
+on your computer. Then, to use Docker hazen, simply run the `hazen-app` script
+appended with the function you want to use (e.g.: `snr`). In Terminal: ```shell
+# Ensure Docker installed and running, then pull the latest hazen Docker
+container docker pull gsttmriphysics/hazen:latest # Command line output will
+look something like: latest: Pulling from gsttmriphysics/hazen Digest: sha256:
 18603e40b45f3af4bf45f07559a08a7833af92a6efe21cb7306f758e8eeab24a Status: Image
 is up to date for gsttmriphysics/hazen:latest docker.io/gsttmriphysics/hazen:
-latest
-{ 'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
-191.16,
-'snr_smoothing_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
-195.58,
-'snr_smoothing_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
-1866.09,
-'snr_smoothing_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
-1909.2,
-'snr_subtraction_measured_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+latest # Copy the 'hazen-app' executable file into your local bin folder cd
+hazen cp hazen-app /usr/local/bin # Run hazen via Docker with the normal CLI
+inputs hazen-app snr tests/data/snr/Siemens/ # Example command line output for
+the SNR Task:
+{ 'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+173.97,
+'snr_smoothing_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
+177.91,
+'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+1698.21,
+'snr_smoothing_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_3_1':
+1736.66,
+'snr_subtraction_measured_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
 220.73,
-'snr_subtraction_normalised_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
-2154.69} ``` #### Linux & MacOS For developers, hazen can be installed from
-source using `pip`. We highly recommend using a virtual environment. ```bash #
-Install OpenSSL # Go to local hazen repo directory cd hazen # Create and
-activate a virtual environment python3 -m venv ./hazen-venv source hazen-venv/
-bin/activate # Install requirements pip install --upgrade pip setuptools wheel
-pip install -r requirements.txt # Install hazen pip install . # Run tests to
-ensure everything is working pytest tests/ ``` --- ## Usage ### Command Line
-The CLI version of hazen is designed to be pointed at single folders containing
-DICOM file(s). Example datasets are provided in the `tests/data/` directory. If
-you are not using the Docker version of hazen, replace `hazen-app` with `hazen`
-in the following commands. To perform an SNR measurement on the provided
-example Philips DICOMs: `hazen-app snr tests/data/snr/Philips` To perform a
-spatial resolution measurement on example data provided by the East Kent Trust:
-`hazen-app spatial_resolution tests/data/resolution/philips` To see the full
-list of available tools, enter: `hazen-app -h` The `--report` option provides
-additional information for some of the functions. For example, the user can
-gain additional insight into the performance of the snr function by entering:
-`hazen-app snr tests/data/snr/Philips --report` ### Web Interface WIP: we are
-developing a web interface for hazen. --- ## Contributing - The Release Manager
-should create a release branch for the future planned release e.g. release-
-X.X.X - The RMs shall organise backlog refinement sessions to ensure issues are
-allocated to the appropriate release - The RM should ensure their release
-branch is kept up-to-date with master - PRs should be merged into the
-appropriate release branch for the issue(s) it is addressing If you want to
-contribute to the development of hazen, please take a look at:
-`CONTRIBUTING.md`. --- ## Users Please [raise an Issue](https://github.com/
-GSTT-CSC/hazen/issues) if you have any problems installing or running hazen. We
-have used hazen with MRI data from a handful of different MRI scanners,
-including multiple different vendors. If your MRI data doesn't work with hazen,
-or the results are unexpected, please submit an Issue and we will investigate.
---- ## Releasing The Release Manager should ensure: - All outstanding issues
-for the current release have been closed, or, transferred to future release. -
-All tests are passing on GitHub Actions. - All documentation has been updated
-with correct version numbers: - Update version number `hazenlib/_version.py`,
-i.e. imported into `docs/conf.py`, `hazenlib/__init__.py` and `setup.cfg` -
-Update version number in `CITATION.cff` - The `release` branch has been merged
-into `main` branch - A new release has been created with a new version tag (tag
-= version number) - RMs of other branches should update their release from the
-latest release as soon as possible and deal with any merge conflicts. ![image]
-(https://user-images.githubusercontent.com/19840489/143266366-06e33949-12c7-
-44b4-9ed7-c0a795b5d492.png) - RMs: Tom Roberts, Lucrezia Cester
+'snr_subtraction_normalised_SNR_seFoV250_2meas_slice5mm_tra_repeat_PSN_noDC_2_1':
+2154.69 } ``` ### Web Interface Development of a [web interface for hazen]
+(https://github.com/GSTT-CSC/hazen-web-app) is in progress. --- ## Contributing
+to hazen ### Users Please [raise an Issue](https://github.com/GSTT-CSC/hazen/
+issues) for any of the following reasons: - Problems installing or running
+hazen - Suggestions for improvements - Requests for new features We have used
+hazen with MRI data from a handful of different MRI scanners, including
+multiple different vendors. If hazen does not perform with your MRI data, or
+the results are unexpected, please raise an Issue. ### Developers Please see
+[CONTRIBUTING.md](CONTRIBUTING.md) for developer guidelines. ---
```

### Comparing `hazen-1.2.0/hazen.egg-info/SOURCES.txt` & `hazen-1.3.0/hazen.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 setup.cfg
 hazen.egg-info/PKG-INFO
 hazen.egg-info/SOURCES.txt
 hazen.egg-info/dependency_links.txt
 hazen.egg-info/entry_points.txt
 hazen.egg-info/requires.txt
 hazen.egg-info/top_level.txt
+hazenlib/ACRObject.py
 hazenlib/HazenTask.py
 hazenlib/__init__.py
 hazenlib/_version.py
 hazenlib/exceptions.py
 hazenlib/logger.py
-hazenlib/relaxometry.py
-hazenlib/shapes.py
-hazenlib/tools.py
+hazenlib/relaxometry_params.py
+hazenlib/utils.py
 hazenlib/data/relaxometry/Plate4_T1_signed
 hazenlib/data/relaxometry/Plate4_T2
 hazenlib/data/relaxometry/Plate5_T1_signed
 hazenlib/data/relaxometry/Plate5_T2
 hazenlib/tasks/__init__.py
 hazenlib/tasks/acr_geometric_accuracy.py
 hazenlib/tasks/acr_ghosting.py
@@ -34,14 +34,15 @@
 hazenlib/tasks/slice_position.py
 hazenlib/tasks/slice_width.py
 hazenlib/tasks/snr.py
 hazenlib/tasks/snr_map.py
 hazenlib/tasks/spatial_resolution.py
 hazenlib/tasks/uniformity.py
 tests/__init__.py
+tests/test_ACRObject.py
 tests/test_acr_geometric_accuracy.py
 tests/test_acr_ghosting.py
 tests/test_acr_slice_position.py
 tests/test_acr_slice_thickness.py
 tests/test_acr_snr.py
 tests/test_acr_spatial_resolution.py
 tests/test_acr_uniformity.py
@@ -49,9 +50,9 @@
 tests/test_hazenlib.py
 tests/test_relaxometry.py
 tests/test_slice_position.py
 tests/test_slice_width.py
 tests/test_snr.py
 tests/test_snr_map.py
 tests/test_spatial_resolution.py
-tests/test_tools.py
-tests/test_uniformity.py
+tests/test_uniformity.py
+tests/test_utils.py
```

### Comparing `hazen-1.2.0/hazenlib/HazenTask.py` & `hazen-1.3.0/hazenlib/HazenTask.py`

 * *Files identical despite different names*

### Comparing `hazen-1.2.0/hazenlib/data/relaxometry/Plate4_T1_signed` & `hazen-1.3.0/hazenlib/data/relaxometry/Plate4_T1_signed`

 * *Files identical despite different names*

### Comparing `hazen-1.2.0/hazenlib/data/relaxometry/Plate4_T2` & `hazen-1.3.0/hazenlib/data/relaxometry/Plate4_T2`

 * *Files identical despite different names*

### Comparing `hazen-1.2.0/hazenlib/data/relaxometry/Plate5_T1_signed` & `hazen-1.3.0/hazenlib/data/relaxometry/Plate5_T1_signed`

 * *Files identical despite different names*

### Comparing `hazen-1.2.0/hazenlib/data/relaxometry/Plate5_T2` & `hazen-1.3.0/hazenlib/data/relaxometry/Plate5_T2`

 * *Files identical despite different names*

### Comparing `hazen-1.2.0/hazenlib/exceptions.py` & `hazen-1.3.0/hazenlib/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,13 +26,13 @@
     def __init__(self, shape, msg=None):
         if msg is None:
             # Default message
             msg = f"Multiple {shape}s found. Multiple shape detection is currently unsupported."
 
         super(ShapeDetectionError, self).__init__(msg)
         self.shape = shape
-        
+
 
 class ArgumentCombinationError(Exception):
     """Argument combination not valid."""
     def __init__(self, msg='Invalid combination of arguments.'):
         super().__init__(msg)
```

### Comparing `hazen-1.2.0/hazenlib/logger.py` & `hazen-1.3.0/hazenlib/logger.py`

 * *Files identical despite different names*

### Comparing `hazen-1.2.0/hazenlib/relaxometry.py` & `hazen-1.3.0/hazenlib/tasks/relaxometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Measure T1 and T2 in Caliber relaxometry phantom.
 
 Introduction
 ============
 
 This module determines the T1 and T2 decay constants for the relaxometry
 spheres in the Caliber (HPD) system phantom
-qmri.com/qmri-solutions/t1-t2-pd-imaging-phantom (plates 4 and 5). Values are
-compared to published values (without temperature correction). Graphs of fit
-and phantom registration images can optionally be produced.
+qmri.com/qmri-solutions/t1-t2-pd-imaging-phantom (plates 4 and 5).
+Values are compared to published values (without temperature correction).
+Graphs of fit and phantom registration images can optionally be produced.
 
 
 Scan parameters
 ===============
 
 Manufacturer's details of recommended scan parameters for GE, Philips and
 Siemens scanners are available in the 'System Phantom Manual' which can be
@@ -77,138 +77,285 @@
     of individual DICOM files (as ``pydicom`` objects) in the ``.images``
     attribute.
 2. Obtain the RT (rotation / translation) matrix to register the template
     image to the test image. Four template images are provided, one for
     each relaxation parameter (T1 or T2) on plates 4 and 5, and regression
     is performed on the first image in the sequence. Optionally output the
     overlay image to visually check the fit.
-3. An ROI is generated for each target sphere using stored coordinates, the
-    RT transformation above, and a structuring element (default is a 5x5
-    boxcar).
-4. Store pixel data for each ROI, at various times, in an ``ROITimeSeries``
+3. A ROI is generated for each target sphere using stored coordinates, the RT
+    transformation above, and a structuring element (default is a 5x5 boxcar).
+4. Store pixel data for each ROI at various times, in an ``ROITimeSeries``
     object. A list of these objects is stored in 
     ``ImageStack.ROI_time_series``.
 5. Generate the fit function. For T1 this looks up TR for the given TI 
     (using piecewise linear interpolation if required) and determines if a
     magnitude or signed image is used. No customisation is required for T2
     measurements.
 6. Determine relaxation time (T1 or T2) by fitting the decay equation to
     the ROI data for each sphere. The published values of the relaxation
-    times are used to seed the optimisation algorithm. For T2 fitting the
-    input data are truncated for TE > 5*T2 to avoid fitting Rician noise in
-    magnitude images with low signal intensity. Optionally plot and save the
-    decay curves.
+    times are used to seed the optimisation algorithm. A Rician noise model is
+    used for T2 fitting [1]_. Optionally plot and save the decay curves.
 7. Return plate number, relaxation type (T1 or T2), measured relaxation
     times, published relaxation times, and fractional differences in a
     dictionary.
 
+References
+==========
+.. [1] Raya, J.G., Dietrich, O., Horng, A., Weber, J., Reiser, M.F.
+and Glaser, C., 2010. T2 measurement in articular cartilage: impact of the
+fitting method on accuracy and precision at low SNR. Magnetic Resonance in
+Medicine: An Official Journal of the International Society for Magnetic
+Resonance in Medicine, 63(1), pp.181-193.
 
 Feature enhancements
 ====================
 Template fit on bolt holes--possibly better with large rotation angles
     -have bolthole template, find 3 positions in template and image, figure out
     transformation.
 
-Template fit on outline image--poss run though edge detection algorithms then
-fit.
+Template fit on outline image--possibly run though edge detection algorithms
+then fit.
 
 Use normalised structuring element in ROITimeSeries. This will allow correct
 calculation of mean if elements are not 0 or 1.
 
 Get r-squared measure of fit.
 
 """
-import pydicom
+import json
+import os.path
+import pathlib
+
 import cv2 as cv
-import numpy as np
 import matplotlib.pyplot as plt
-import os
-import os.path
-import skimage.morphology
+import numpy as np
+import pydicom
 import scipy.ndimage
 import scipy.optimize
+import skimage.morphology
 from scipy.interpolate import UnivariateSpline
+from scipy.special import i0e, ive
 
 import hazenlib.exceptions
+from hazenlib.HazenTask import HazenTask
+from hazenlib.relaxometry_params import (
+    MAX_RICIAN_NOISE, SEED_RICIAN_NOISE, TEMPLATE_VALUES, SMOOTH_TIMES,
+    TEMPLATE_FIT_ITERS, TERMINATION_EPS
+)
 
 # Use dict to store template and reference information
 # Coordinates are in array format (row,col), rather than plt.patches 
 # format (col,row)
 #
 # Access as:
 #    TEMPLATE_VALUES[f'plate{plate_num}']['sphere_centres_row_col']
 #    TEMPLATE_VALUES[f'plate{plate_num}']['t1'|'t2']['filename']
 #    TEMPLATE_VALUES[f'plate{plate_num}']['t1'|'t2']['1.5T'|'3.0T']['relax_times']
 
-TEMPLATE_DIR = os.path.join(os.path.dirname(os.path.realpath(__file__)),
-                            'data', 'relaxometry')
-TEMPLATE_VALUES = {
-    'plate3': {
-        'sphere_centres_row_col': (),
-        'bolt_centres_row_col': (),
-        't1': {
-            'filename': '',
-            'relax_times': []}},
-
-    'plate4': {
-        'sphere_centres_row_col': (
-            (56, 94), (62, 117), (81, 132), (105, 134), (125, 120), (133, 99),
-            (127, 75), (108, 60), (84, 59), (64, 72), (80, 81), (78, 111),
-            (109, 113), (111, 82), (148, 118)),
-        'bolt_centres_row_col': (),
-        't1': {
-            'filename': os.path.join(TEMPLATE_DIR, 'Plate4_T1_signed'),
-            'relax_times': {
-                '1.5T':
-                    np.array([2376, 2183, 1870, 1539, 1237, 1030, 752.2, 550.2,
-                              413.4, 292.9, 194.9, 160.2, 106.4, 83.3, 2700]),
-                '3.0T':
-                    np.array([2480, 2173, 1907, 1604, 1332, 1044, 801.7, 608.6,
-                              458.4, 336.5, 244.2, 176.6, 126.9, 90.9, 2700])}},
-        't2': {
-            'filename': os.path.join(TEMPLATE_DIR, 'Plate4_T2'),
-            'relax_times': {
-                '1.5T':
-                    np.array([939.4, 594.3, 416.5, 267.0, 184.9, 140.6, 91.76,
-                              64.84, 45.28, 30.62, 19.76, 15.99, 10.47, 8.15,
-                              2400]),
-                '3.0T':
-                    np.array([581.3, 403.5, 278.1, 190.94, 133.27, 96.89,
-                              64.07, 46.42, 31.97, 22.56, 15.813, 11.237,
-                              7.911, 5.592, 2400])}}},
-
-    'plate5': {
-        'sphere_centres_row_col': (
-            (56, 95), (62, 117), (81, 133), (104, 134), (124, 121), (133, 98),
-            (127, 75), (109, 61), (84, 60), (64, 72), (80, 81), (78, 111),
-            (109, 113), (110, 82), (97, 43)),
-        'bolt_centres_row_col': ((52, 80), (92, 141), (138, 85)),
-        't1': {
-            'filename': os.path.join(TEMPLATE_DIR, 'Plate5_T1_signed'),
-            'relax_times': {
-                '1.5T':
-                    np.array([2033, 1489, 1012, 730.8, 514.1, 367.9, 260.1,
-                              184.6, 132.7, 92.7, 65.4, 46.32, 32.45, 22.859,
-                              2700]),
-                '3.0T':
-                    np.array([1989, 1454, 984.1, 706, 496.7, 351.5, 247.13,
-                              175.3, 125.9, 89.0, 62.7, 44.53, 30.84,
-                              21.719, 2700])}},
-
-        't2': {
-            'filename': os.path.join(TEMPLATE_DIR, 'Plate5_T2'),
-            'relax_times': {
-                '1.5T':
-                    np.array([1669.0, 1244.0, 859.3, 628.5, 446.3, 321.2,
-                              227.7, 161.9, 117.1, 81.9, 57.7, 41.0, 28.7,
-                              20.2, 2400]),
-                '3.0T':
-                    np.array([1465, 1076, 717.9, 510.1, 359.6, 255.5, 180.8,
-                              127.3, 90.3, 64.3, 45.7, 31.86, 22.38,
-                              15.83, 2400])}}}}
+
+class Relaxometry(HazenTask):
+
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+    def run(self, calc: str = 'T1', plate_number=None, verbose=False):
+        """
+        Calculate T1 or T2 values for relaxometry phantom.
+
+        Note: either ``calc_t1`` or ``calc_t2`` (but not both) must be True.
+        Variables set in parent class:
+        data : list of pydicom.dataset.FileDataSet objects
+            List of DICOM images of a plate of the HPD relaxometry phantom.
+        report : bool, optional
+            Whether to save images showing the measurement details
+        report_dir : path, optional
+            Folder path to save images to. The default is False.
+
+        Parameters
+        ----------
+        calc : str, required
+            Whether to calculate T1 or T2 relaxation. Default is T1.
+        plate_number : str, required
+            Plate number of the HPD relaxometry phantom (either 4 or 5)
+        verbose : bool, optional
+            Provide verbose output. If True, the following key / values will be
+            added to the output dictionary:
+                plate : plate_number,
+                relaxation_type : 't1' | 't2',
+                calc_times : list of T1|T2 for each sphere,
+                manufacturers_times : list of manufacturer's values for T1|T2,
+                frac_time_difference : (calc_times - manufacturers_times) / manufacturers_times
+                institution_name=index_im.InstitutionName,
+                manufacturer=index_im.Manufacturer,
+                model=index_im.ManufacturerModelName,
+                date=index_im.StudyDate,
+                detailed_output : dict with extensive information
+            The default is False.
+
+        Returns
+        -------
+
+        dict
+            {
+                rms_frac_time_difference : RMS fractional difference between
+                    calculated relaxometry times and manufacturer provided data.
+            }
+        """
+
+        # check plate number specified: should be either 4 or 5
+        try:
+            plate_number = int(plate_number)  # convert to int if required
+        except (ValueError, TypeError):
+            pass  # will raise error at next statement
+        if plate_number not in [4, 5]:
+            raise hazenlib.exceptions.ArgumentCombinationError(
+                'Must specify plate_number (4 or 5)')
+
+        # Set up parameters specific to T1 or T2
+        relax_str = calc.lower()
+
+        if calc in ['T1', 't1']:
+            image_stack = T1ImageStack(self.data)
+            try:
+                template_dcm = pydicom.read_file(
+                    TEMPLATE_VALUES[f'plate{plate_number}'][relax_str]['filename'])
+            except KeyError:
+                print(f'Could not find template with plate number: {plate_number}.'
+                    f' Please pass plate number as arg.')
+                exit()
+        elif calc in ['T2', 't2']:
+            image_stack = T2ImageStack(self.data)
+            try:
+                template_dcm = pydicom.read_file(
+                    TEMPLATE_VALUES[f'plate{plate_number}'][relax_str]['filename'])
+            except KeyError:
+                print(f'Could not find template with plate number: {plate_number}.'
+                    f' Please pass plate number as arg.')
+                exit()
+        else:
+            print("Please provide 'T1' or 'T2' for the --calc argument.")
+            exit()
+
+        warp_matrix = image_stack.template_fit(template_dcm)
+        image_stack.generate_time_series(
+            TEMPLATE_VALUES[f'plate{plate_number}']['sphere_centres_row_col'],
+            warp_matrix=warp_matrix)
+        # only applies to T1
+        image_stack.generate_fit_function()
+
+        # Published relaxation time for matching plate and T1/T2
+        relax_published = TEMPLATE_VALUES [f'plate{plate_number}'][relax_str] \
+                ['relax_times'][image_stack.b0_str]
+        s0_est = image_stack.initialise_fit_parameters(relax_published)
+
+        image_stack.find_relax_times(relax_published, s0_est)
+        frac_time_diff = (image_stack.relax_times - relax_published) \
+                        / relax_published
+        # last value is for background water. Strip before calculating RMS frac error
+        frac_time = frac_time_diff[:-1]
+        RMS_frac_error = np.sqrt(np.mean(np.square(frac_time)))
+
+        # Generate output dict
+        index_im = image_stack.images[0]
+        output_key = f"{index_im.SeriesDescription}_{index_im.SeriesNumber}_{index_im.InstanceNumber}_" \
+                    f"P{plate_number}_{relax_str}"
+
+        relax_result = {'rms_frac_time_difference' : RMS_frac_error}
+
+        if self.report:
+            img_path = os.path.join(self.report_path, output_key)
+            # Show template fit
+            template_fit_fig = image_stack.plot_fit()
+            # Improve saved image quality
+            template_fit_fig.set_size_inches(24, 24)
+            for subplt in template_fit_fig.get_axes():
+                subplt.title.set_fontsize(40)
+            template_fit_img = f'{img_path}_template_fit.png'
+            template_fit_fig.savefig(template_fit_img, dpi=150)
+            self.report_files.append(('template_fit', template_fit_img))
+
+            # Show ROIs
+            roi_fig = image_stack.plot_rois()
+            plt.title(f'ROI positions ({calc.upper()}, plate {plate_number})')
+            roi_img = f'{img_path}_rois.png'
+            roi_fig.savefig(roi_img, dpi=300)
+            self.report_files.append(('rois', roi_img))
+
+            # Show relax fits
+            rois = image_stack.ROI_time_series
+            relax_fit_fig = plt.figure()
+            relax_fit_fig.suptitle(calc.upper() + ' relaxometry fits')
+            smooth_times = SMOOTH_TIMES[calc.lower()]
+            for i in range(15):
+                plt.subplot(5, 3, i + 1)
+                plt.plot(smooth_times,
+                        image_stack.fit_function(
+                            np.array(smooth_times),
+                            *np.array(image_stack.relax_fit[i][0])),
+                        'b-')
+                plt.plot(rois[i].times, rois[i].means, 'rx')
+                if i == 14:
+                    plt.title(f'[Free water] fit={image_stack.relax_times[i]:.4g}',
+                            fontsize=8)
+                else:
+                    plt.title(f'[{i + 1}] fit={image_stack.relax_times[i]:.4g}, '
+                            f'pub={relax_published[i]:.4g} '
+                            f'({frac_time_diff[i] * 100:+.2f}%)',
+                            fontsize=8)
+            # Improve saved image quality
+            relax_fit_fig.set_size_inches(9, 15)
+            plt.tight_layout(rect=(0, 0, 1, 0.97))
+            relax_fit_img = f'{img_path}_decay_graphs.png'
+            relax_fit_fig.savefig(relax_fit_img, dpi=300)
+            self.report_files.append(('decay_graphs', relax_fit_img))
+
+        if verbose:
+            # Dump additional details about the images and the measurement to a file
+            pathlib.Path(self.report_path).mkdir(parents=True, exist_ok=True)
+            detailed_output = {}
+            detailed_outpath = os.path.join(self.report_path, f"{output_key}_details.json")
+
+            metadata = dict(
+                files=[im.filename for im in image_stack.images],
+                plate=plate_number,
+                relaxation_type=calc.upper(),
+                institution_name=index_im.InstitutionName,
+                manufacturer=index_im.Manufacturer,
+                model=index_im.ManufacturerModelName,
+                date=index_im.StudyDate,
+                manufacturers_times=relax_published.tolist(),
+                calc_times=image_stack.relax_times,
+                frac_time_difference=frac_time_diff.tolist())
+            # , output_graphics=output_files_path
+            relax_result.update(metadata)
+
+            detailed_output['measurement details'] = {
+                'Echo Time': [im.EchoTime for im in image_stack.images],
+                'Repetition Time': [im.RepetitionTime for im in image_stack.images],
+                'Inversion Time': [im.InversionTime if hasattr(
+                    im, 'InversionTime') else None for im in image_stack.images],
+                # fit_paramters (T1) = [[T1, s0, A1] for each ROI]
+                # fit_parameters (T2) = [[T2, s0, C] for each ROI]
+                'ROI_means': {i: im.means for i, im in enumerate(image_stack.ROI_time_series)},
+                'fit_parameters': [tuple(param[0].tolist()) for param in image_stack.relax_fit],
+                'fit_equation': image_stack.fit_eqn_str
+            }
+            detailed_output['metadata'] = metadata
+            json_object = json.dumps(detailed_output, indent = 4)
+            with open(detailed_outpath, "w") as f:
+                f.write(json_object)
+            self.report_files.append(
+                ('further_details', detailed_outpath))
+
+        result = {output_key: relax_result}
+        if self.report:
+            result['images'] = self.report_files
+
+        # plt.show()
+        return result
 
 
 def outline_mask(im):
     """
     Create contour lines to outline pixels.
     
     Creates a series of ``line`` objects to outline contours on an image. Used
@@ -251,15 +398,14 @@
     starts = np.argwhere(im1 == 1)
     ends = np.argwhere(im1 == -1)
     lines += [([s[1] + .5, e[1] + .5], [s[0] - .5, s[0] - .5]) for s, e
               in zip(starts, ends)]
 
     return lines
 
-
 def transform_coords(coords, rt_matrix, input_row_col=True,
                      output_row_col=True):
     """
     Convert coordinates using RT transformation matrix.
 
     Note that arrays containing pixel information as displayed using
     plt.imshow(pixel_array), for example are referenced using the row_col (y,x)
@@ -299,256 +445,60 @@
 
     """
     in_coords = np.array(coords)  # ensure using np array
 
     if input_row_col:  # convert to col_row (xy) format
         in_coords = np.flip(in_coords, axis=1)
 
-    out_coords = cv.transform(np.array([in_coords]), rt_matrix)
-    out_coords = out_coords[0]  # reduce to two dimensions
+    out_coords = cv.transform(np.array([in_coords]), rt_matrix)[0]  # reduce to two dimensions
+    # out_coords = out_coords
 
     if output_row_col:
         out_coords = np.flip(out_coords, axis=1)
 
     return out_coords
 
-
-def pixel_rescale(dcmfile):
+def pixel_rescale(dcm):
     """
     Transforms pixel values according to scale values in DICOM header.
     
     DICOM pixel values arrays cannot directly represent signed or float values.
     This function converts the ``.pixel_array`` using the scaling values in the
     DICOM header.
 
     For Philips scanners the private DICOM fields 2005,100d (=SI) and 2005,100e
     (=SS) are used as inverse scaling factors to perform the inverse
-    transformation [1]_
+    transformation [1]_.
 
     Parameters
     ----------
-    dcmfile : Pydicom.dataset.FileDataset
+    dcm : Pydicom.dataset.FileDataset
         DICOM file containing one image.
 
     Returns
     -------
     numpy.array
-        Values in ``dcmfile.pixel_array`` transformed using DICOM scaling.
+        Values in ``dcm.pixel_array`` transformed using DICOM scaling.
 
     References
     ----------
     .. [1] Chenevert, Thomas L., et al. "Errors in quantitative image analysis
      due to platform-dependent image scaling." Translational Oncology 7.1
      (2014): 65-71. https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3998685/
 
     """
     # Check for Philips
-    if dcmfile.Manufacturer.startswith('Philips'):
-        ss = dcmfile['2005100e'].value  # Scale slope
-        si = dcmfile['2005100d'].value  # Scale intercept
+    if dcm.Manufacturer.startswith('Philips'):
+        ss = dcm['2005100e'].value  # Scale slope
+        si = dcm['2005100d'].value  # Scale intercept
 
-        return (dcmfile.pixel_array - si) / ss
+        return (dcm.pixel_array - si) / ss
     else:
         return pydicom.pixel_data_handlers.util.apply_modality_lut(
-            dcmfile.pixel_array, dcmfile)
-
-
-def generate_t1_function(ti_interp_vals, tr_interp_vals, mag_image=False):
-    """
-    Generate T1 signal function and jacobian with interpolated TRs.
-    
-    Signal intensity on T1 decay is a function of both TI and TR. Ideally, TR
-    should be constant and at least 5*T1. However, scan time can be reduced by
-    allowing a shorter TR which increases at long TIs. For example::
-        TI |   50 |  100 |  200 |  400 |  600 |  800 
-        ---+------+------+------+------+------+------
-        TR | 1000 | 1000 | 1000 | 1260 | 1860 | 2460
-    
-    This function factory returns a function which calculates the signal
-    magnitude using the expression::
-        S = S0 * (1 - a1 * np.exp(-TI / t1) + np.exp(-TR / t1))
-    where ``S0`` is the recovered intensity, ``a1`` is theoretically 2.0 but
-    varies due to inhomogeneous B0 field, ``t1`` is the longitudinal
-    relaxation time, and the repetition time, ``TR``, is calculated  from
-    ``TI`` using piecewise linear interpolation.
-
-    Parameters
-    ----------
-    ti_interp_vals : array_like
-        Array of TI values used as a look-up table to calculate TR
-    tr_interp_vals : array_like
-        Array of TR values used as a lookup table to calculate TR from the TI
-        used in the sequence.
-    mag_image : bool, optional
-        If True, the generated function returns the magnitude of the signal
-        (i.e. negative outputs become positive). The default is False.
-
-    Returns
-    -------
-    t1_function : function
-        S = S0 * (1 - a1 * np.exp(-TI / t1) + np.exp(-TR / t1))
-    
-    t1_jacobian : function
-        Tuple of partial derivatives for curve fitting.
-
-    eqn_str : string
-        String representation of fit function.
-    """
-    #  Create piecewise liner fit function. k=1 gives linear, s=0 ensures all
-    #  points are on line. Using UnivariateSpline (rather than numpy.interp())
-    #  enables derivative calculation if required.
-    tr = UnivariateSpline(ti_interp_vals, tr_interp_vals, k=1, s=0)
-    # tr_der = tr.derivative()
-
-    eqn_str = 's0 * (1 - a1 * np.exp(-TI / t1) + np.exp(-TR / t1))'
-    if mag_image:
-        eqn_str = f'abs({eqn_str})'
-
-    def _t1_function_signed(ti, t1, s0, a1):
-        pv = s0 * (1 - a1 * np.exp(-ti / t1) + np.exp(-tr(ti) / t1))
-        return pv
-
-    def t1_function(ti, t1, s0, a1):
-        pv = _t1_function_signed(ti, t1, s0, a1)
-        if mag_image:
-            return abs(pv)
-        else:
-            return pv
-
-    def t1_jacobian(ti, t1, s0, a1):
-        t1_der = s0 / (t1 ** 2) * (-ti * a1 * np.exp(-ti / t1) + tr(ti)
-                                   * np.exp(-tr(ti) / t1))
-        s0_der = 1 - a1 * np.exp(-ti / t1) + np.exp(-tr(ti) / t1)
-        a1_der = -s0 * np.exp(-ti / t1)
-        jacobian = np.array([t1_der, s0_der, a1_der])
-
-        if mag_image:
-            pv = _t1_function_signed(ti, t1, s0, a1)
-            jacobian = (jacobian * (pv >= 0)) - (jacobian * (pv < 0))
-
-        return jacobian.T
-
-    return t1_function, t1_jacobian, eqn_str
-
-
-def est_t1_s0(ti, tr, t1, pv):
-    """
-    Return initial guess of s0 to seed T1 curve fitting.
-
-    Parameters
-    ----------
-    ti : array_like
-        TI values.
-    tr : array_like
-        TR values.
-    t1 : array_like
-        Estimated T1 (typically from manufacturer's documentation).
-    pv : array_like
-        Mean pixel value (signal) in ROI.
-
-    Returns
-    -------
-    array_like
-        Initial s0 guess for calculating T1 relaxation time.
-
-    """
-    return -pv / (1 - 2 * np.exp(-ti / t1) + np.exp(-tr / t1))
-
-
-def t2_function(te, t2, s0):
-    """
-    Calculated pixel value given TE, T2, S0 and C.
-    
-    Calculates pixel value from::
-        S = S0 * np.exp(-te / t2)
-
-    Parameters
-    ----------
-    te : array_like
-        Echo times.
-    t2 : float
-        T2 decay constant.
-    S0 : float
-        Initial pixel magnitude.
-
-    Returns
-    -------
-    pv : array_like
-        Theoretical pixel values (signal) at each TE.
-
-    """
-    pv = s0 * np.exp(-te / t2)
-    return pv
-
-
-def t2_jacobian(te, t2, s0):
-    """
-    Jacobian of ``t2_function`` used for curve fitting.
-
-    Parameters
-    ----------
-    te : array_like
-        Echo times.
-    t2 : float
-        T2 decay constant.
-    s0 : float
-        Initial signal magnitude.
-
-    Returns
-    -------
-    array
-        [t2_der, s0_der].T, where x_der is a 1-D array of the partial
-        derivatives at each ``te``.
-
-    """
-    t2_der = s0 * te / t2 ** 2 * np.exp(-te / t2)
-    s0_der = np.exp(-te / t2)
-    jacobian = np.array([t2_der, s0_der])
-    return jacobian.T
-
-
-def est_t2_s0(te, t2, pv, c=0.0):
-    """
-    Initial guess for s0 to seed curve fitting.
-
-    Parameters
-    ----------
-    te : array_like
-        Echo time(s).
-    t2 : array_like
-        T2 decay constant.
-    pv : array_like
-        Mean pixel value (signal) in ROI with ``te`` echo time.
-    c : array_like
-        Constant offset, theoretically ``full_like(te, 0.0)``.
-
-    Returns
-    -------
-    array_like
-        Initial s0 estimate ``s0 = (pv - c) / np.exp(-te/t2)``.
-
-    """
-    return (pv - c) / np.exp(-te / t2)
-    
-    
-def rms(arr):
-    """
-    Calculate RMS of an array.
-
-    Parameters
-    ----------
-    arr : array_like
-         Input array
-
-    Returns
-    -------
-    rms : float
-        sqrt(mean(square(arr)))
-    """
-    return np.sqrt(np.mean(np.square(arr)))
+            dcm.pixel_array, dcm)
 
 
 class ROITimeSeries:
     """
     Samples at one image location (ROI) at numerous sample times.
     
     Estimating T1 and T2 relaxation parameters at any ROI requires a series
@@ -577,18 +527,15 @@
     trs : list of floats
         Values of TR for each image.
         
     means : list of floats
         Mean pixel value of ROI for each image in series.
     """
 
-    SAMPLE_ELEMENT = skimage.morphology.square(5)
-
-    def __init__(self, dcm_images, poi_coords_row_col, time_attr=None,
-                 kernel=None):
+    def __init__(self, dcm_images, poi_coords_row_col, time_attr):
         """
         Create ROITimeSeries for ROI parameters at sequential scans.
 
         Parameters
         ----------
         dcm_images : list
             List of pydicom images of same object with different scan
@@ -597,34 +544,34 @@
             Two element array with coordinates of point of interest (POI),
             typically the centre of the ROI, in row_col (y,x) format.
         time_attr : string, optional
             If present, lookup the DICOM attribute ``[time_attr]`` (typically
             ``'InversionTime'`` or ``'EchoTime'``) and store in the list
             ``self.times``. The default is ``None``, which does not create
             ``self.times``
-        kernel : array_like, optional
-            Structuring element which defines ROI size and shape, centred on
-            POI. Each element should be 1 or 0, otherwise calculation of mean
-            will be incorrect. If ``None``, use a 5x5 square. The default is
-            ``None``.
         """
 
-        if kernel is None:
-            kernel = self.SAMPLE_ELEMENT
         self.POI_mask = np.zeros((dcm_images[0].pixel_array.shape[0],
                                   dcm_images[0].pixel_array.shape[1]),
                                  dtype=np.int8)
         self.POI_mask[poi_coords_row_col[0], poi_coords_row_col[1]] = 1
 
+
+        kernel = skimage.morphology.square(5)
+        """kernel
+            Structuring element which defines ROI size and shape, centred on
+            POI. Each element should be 1 or 0, otherwise calculation of mean
+            will be incorrect. If ``None``, use a 5x5 square. The default is
+            ``None``.
+        """
+
         self.ROI_mask = np.zeros_like(self.POI_mask)
         self.ROI_mask = scipy.ndimage.filters.convolve(self.POI_mask, kernel)
-        self._time_attr = time_attr
 
-        if time_attr is not None:
-            self.times = [x[time_attr].value.real for x in dcm_images]
+        self.times = [x[time_attr].value.real for x in dcm_images]
         self.pixel_values = [
             pixel_rescale(img)[self.ROI_mask > 0] for img in dcm_images]
 
         self.trs = [x['RepetitionTime'].value.real for x in dcm_images]
 
     def __len__(self):
         """Number of time samples in series."""
@@ -643,16 +590,15 @@
 
 
 class ImageStack():
     """
     Object to hold image_slices and methods for T1, T2 calculation.
     """
 
-    def __init__(self, image_slices, template_dcm, plate_number=None,
-                 dicom_order_key=None):
+    def __init__(self, image_slices, time_attribute=None):
         """
         Create ImageStack object.
 
         Parameters
         ----------
         image_slices : list of pydicom.FileDataSet objects
             List of pydicom objects to perform relaxometry analysis on.
@@ -660,46 +606,44 @@
         template_dcm : pydicom FileDataSet (or None)
             DICOM template object.
             
         plate_number : int {3,4,5}, optional
             For future use. Reference to the plate in the relaxometry phantom.
             The default is None.
             
-        dicom_order_key : string, optional
+        time_attribute : string, optional
             DICOM attribute to order images. Typically 'InversionTime' for T1
             relaxometry or 'EchoTime' for T2.
         """
-        self.plate_number = plate_number
-        # Store template pixel array, after scaling in 0028,1052 and 0028,1053
-        # applied
-        self.template_dcm = template_dcm
-        if template_dcm is not None:
-            self.template_px = pixel_rescale(template_dcm)
-
-        self.dicom_order_key = dicom_order_key
-        self.images = image_slices  # store images
-        if dicom_order_key is not None:
-            self.order_by(dicom_order_key)
+        self.time_attr = time_attribute
+        # store sorted images
+        self.images = self.order_by(image_slices, time_attribute)
 
         b0_val = self.images[0]['MagneticFieldStrength'].value
-        if b0_val == 1.5:
-            self.b0_str = '1.5T'
-        elif b0_val == 3.0:
-            self.b0_str = '3.0T'
-        else:
+        if b0_val not in [1.5, 3.0]:
             # TODO incorporate warning through e.g. logging module
             print('Unable to match B0 to default values. Using 1.5T.\n'
                   f" {self.images[0]['MagneticFieldStrength']}")
             self.b0_str = '1.5T'
+        else:
+            if b0_val == 3:
+                self.b0_str = "3.0T"
+            else:
+                self.b0_str = f"{b0_val}T"
 
-    def template_fit(self, image_index=0):
+    def order_by(self, images, att):
+        """Order images by attribute (e.g. EchoTime, InversionTime)."""
+        sorted_images = sorted(images, key=lambda x: x[att].value.real)
+        return sorted_images
+
+    def template_fit(self, template_dcm, image_index=0):
         """
         Calculate transformation matrix to fit template to image.
 
-        The template pixel array, self.template_px, is fitted to one of the
+        The template pixel array, template_px, is fitted to one of the
         images in self.images (default=0). The resultant RT matrix is stored as
         self.warp_matrix.
 
         This matrix can be used to map coordinates from template space to image
         space using transform_coords(...), or to map masks from template space
         to image space using cv2.warpAffine(...).
 
@@ -731,59 +675,88 @@
         Need to check if image is real valued, typically signed then shifted so
         background is 2048, or magnitude image. Currently it forces converts
         all images to magnitude images before regression.
 
         Despite these limitations, this method works well in practice for small
         angle rotations.
         """
+        # Store template pixel array, after scaling in 0028,1052 and
+        # 0028,1053 applied
+        template_px = pixel_rescale(template_dcm)
         target_px = pixel_rescale(self.images[0])
-        template_px = self.template_px
 
-        # Pad template or target pixels if required
-        scale_factor = len(target_px) / len(template_px)
+        ## Pad template or target pixels if required
+        # Determine difference in shape
         pad_size = np.subtract(template_px.shape, target_px.shape)
         assert pad_size[0] == pad_size[1], "Image matrices must be square."
         if pad_size[0] > 0:  # pad target--UNTESTED
+            # add pixels to target if smaller than template
             target_px = np.pad(target_px, pad_width=(0, pad_size[0]))
         elif pad_size[0] < 0:  # pad template
+            # add pixels to template if smaller than target
             template_px = np.pad(template_px, pad_width=(0, -pad_size[0]))
 
         # Always fit on magnitude images for simplicity. May be suboptimal
-        self.template8bit = \
-            cv.normalize(abs(template_px),
-                         None, 0, 255, norm_type=cv.NORM_MINMAX,
-                         dtype=cv.CV_8U)
-
-        self.target8bit = cv.normalize(abs(target_px),
-                                       None, 0, 255, norm_type=cv.NORM_MINMAX,
-                                       dtype=cv.CV_8U)
+        self.template8bit = cv.normalize(abs(template_px), None, 0, 255,
+                            norm_type=cv.NORM_MINMAX, dtype=cv.CV_8U)
+
+        self.target8bit = cv.normalize(abs(target_px), None, 0, 255,
+                            norm_type=cv.NORM_MINMAX, dtype=cv.CV_8U)
 
         # initialise transformation fitting parameters.
-        number_of_iterations = 500
-        termination_eps = 1e-10
-        criteria = (cv.TERM_CRITERIA_EPS | cv.TERM_CRITERIA_COUNT,
-                    number_of_iterations, termination_eps)
-        self.warp_matrix = scale_factor * np.eye(2, 3, dtype=np.float32)
+        scale_factor = len(target_px) / len(template_px)
+        scale_matrix = scale_factor * np.eye(2, 3, dtype=np.float32)
 
-        self.scaled_template8bit = cv.warpAffine(self.template8bit,
-                                                 self.warp_matrix,
-                                                 (self.template8bit.shape[1],
-                                                  self.template8bit.shape[0]))
+        self.scaled_template8bit = cv.warpAffine(
+                    self.template8bit, scale_matrix,
+                    (self.template8bit.shape[1],self.template8bit.shape[0]))
 
         # Apply transformation
-        self.template_cc, self.warp_matrix = \
-            cv.findTransformECC(self.template8bit, self.target8bit,
-                                self.warp_matrix, criteria=criteria)
-
-        self.warped_template8bit = cv.warpAffine(self.template8bit,
-                                                 self.warp_matrix,
-                                                 (self.template8bit.shape[1],
-                                                  self.template8bit.shape[0]))
+        criteria = (cv.TERM_CRITERIA_EPS | cv.TERM_CRITERIA_COUNT,
+                    TEMPLATE_FIT_ITERS, TERMINATION_EPS)
+        # Find the geometric transform (warp) between two images in terms of the ECC criterion
+        self.template_cc, warp_matrix = cv.findTransformECC(
+                                        self.template8bit, self.target8bit,
+                                        scale_matrix, criteria=criteria)
+
+        self.warped_template8bit = cv.warpAffine(
+                    self.template8bit, warp_matrix,
+                    (self.template8bit.shape[1], self.template8bit.shape[0]))
+
+        return warp_matrix
 
-        return self.warp_matrix
+    def generate_time_series(self, coords_row_col, warp_matrix, fit_coords=True):
+        """
+        Create list of ROITimeSeries objects.
+
+        Parameters
+        ----------
+        coords_row_col : array_like
+            Array of coordinates points of interest (POIs) for each centre of
+            each ROI. They should be in [[col0, row0], [col1, row1], ...]
+            format.
+        time_attribute : string, optional
+            DICOM attribute to order images. Typically 'InversionTime' for T1
+            relaxometry or 'EchoTime' for T2.
+        warp_matrix : np.array
+            RT transform matrix (2,3).
+        """
+        num_coords = np.size(coords_row_col, axis=0)
+
+        # adjustment may not be required for the template DICOM
+        if fit_coords:
+            adjusted_coords_row_col = transform_coords(coords_row_col,
+                    warp_matrix, input_row_col=True, output_row_col=True)
+        else:  # used in testing
+            adjusted_coords_row_col = coords_row_col
+
+        self.ROI_time_series = []
+        for i in range(num_coords):
+            self.ROI_time_series.append(ROITimeSeries(
+                self.images, adjusted_coords_row_col[i], self.time_attr))
 
     def plot_fit(self):
         """
         Visual representation of target fitting.
 
         Create 2x2 subplot showing 8-bit version of:
             1. Template
@@ -844,457 +817,358 @@
                 combined_ROI_map += roi.ROI_mask
             lines = outline_mask(combined_ROI_map)
             for line in lines:
                 plt.plot(line[1], line[0], color='r', alpha=1)
 
         return fig
 
-    def order_by(self, att):
-        """Order images by attribute (e.g. EchoTime, InversionTime)."""
-        self.images.sort(key=lambda x: x[att].value.real)
+    @property
+    def relax_times(self):
+        """List of T1 for each ROI."""
+        return [fit[0][0] for fit in self.relax_fit]
 
-    def generate_time_series(self, coords_row_col, fit_coords=True,
-                             kernel=None):
+class T1ImageStack(ImageStack):
+    """
+    Calculate T1 relaxometry.
+    """
+
+    def __init__(self, image_slices):
+        time_attribute = "InversionTime"
+        super().__init__(image_slices, time_attribute)
+
+    def generate_t1_function(self, ti_interp_vals, tr_interp_vals, mag_image=False):
         """
-        Create list of ROITimeSeries objects.
+        Generate T1 signal function and jacobian with interpolated TRs.
+        
+        Signal intensity on T1 decay is a function of both TI and TR. Ideally, TR
+        should be constant and at least 5*T1. However, scan time can be reduced by
+        allowing a shorter TR which increases at long TIs. For example::
+            TI |   50 |  100 |  200 |  400 |  600 |  800 
+            ---+------+------+------+------+------+------
+            TR | 1000 | 1000 | 1000 | 1260 | 1860 | 2460
+        
+        This function factory returns a function which calculates the signal
+        magnitude using the expression::
+            S = S0 * (1 - a1 * np.exp(-TI / t1) + np.exp(-TR / t1))
+        where ``S0`` is the recovered intensity, ``a1`` is theoretically 2.0 but
+        varies due to inhomogeneous B0 field, ``t1`` is the longitudinal
+        relaxation time, and the repetition time, ``TR``, is calculated  from
+        ``TI`` using piecewise linear interpolation.
 
         Parameters
         ----------
-        coords_row_col : array_like
-            Array of coordinates points of interest (POIs) for each centre of
-            each ROI. They should be in [[col0, row0], [col1, row1], ...]
-            format.
-        fit_coords : bool, optional
-            If ``True``, the coordinates provided are for the template ROIs and
-            will be transformed to the image space using ``transfor_coords()``.
-            The default is True.
-        kernel : array, optional
-            Structuring element which should be an array of 1s and possibly 0s.
-            If ``None``, use the default from ``ROItimeSeries`` constructor.
-            The default is None.
-        """
-        num_coords = np.size(coords_row_col, axis=0)
-        if fit_coords:
-            coords_row_col = transform_coords(coords_row_col, self.warp_matrix,
-                                              input_row_col=True,
-                                              output_row_col=True)
+        ti_interp_vals : array_like
+            Array of TI values used as a look-up table to calculate TR
+        tr_interp_vals : array_like
+            Array of TR values used as a lookup table to calculate TR from the TI
+            used in the sequence.
+        mag_image : bool, optional
+            If True, the generated function returns the magnitude of the signal
+            (i.e. negative outputs become positive). The default is False.
 
-        self.ROI_time_series = []
-        for i in range(num_coords):
-            self.ROI_time_series.append(ROITimeSeries(
-                self.images, coords_row_col[i], time_attr=self.dicom_order_key,
-                kernel=kernel))
+        Returns
+        -------
+        t1_function : function
+            S = S0 * (1 - a1 * np.exp(-TI / t1) + np.exp(-TR / t1))
+        
+        t1_jacobian : function
+            Tuple of partial derivatives for curve fitting.
 
-    def generate_fit_function(self):
-        """Null method in base class, may be overwritten in subclass."""
+        eqn_str : string
+            String representation of fit function.
+        """
+        #  Create piecewise linear fit function. k=1 gives linear, s=0 ensures all
+        #  points are on line. Using UnivariateSpline (rather than numpy.interp())
+        #  enables derivative calculation if required.
+        tr = UnivariateSpline(ti_interp_vals, tr_interp_vals, k=1, s=0)
+        # tr_der = tr.derivative()
 
+        eqn_str = 's0 * (1 - a1 * np.exp(-TI / t1) + np.exp(-TR / t1))'
+        if mag_image:
+            eqn_str = f'abs({eqn_str})'
 
-class T1ImageStack(ImageStack):
-    """
-    Calculate T1 relaxometry.
+        def _t1_function_signed(ti, t1, s0, a1):
+            pv = s0 * (1 - a1 * np.exp(-ti / t1) + np.exp(-tr(ti) / t1))
+            return pv
 
-    Overloads the following methods from ``ImageStack``:
-        ``generate_fit_function``
-        ``initialise_fit_parameters``
-        ``find_relax_times``
+        def t1_function(ti, t1, s0, a1):
+            pv = _t1_function_signed(ti, t1, s0, a1)
+            if mag_image:
+                return abs(pv)
+            else:
+                return pv
 
-    """
+        def t1_jacobian(ti, t1, s0, a1):
+            t1_der = s0 / (t1 ** 2) * (-ti * a1 * np.exp(-ti / t1) + tr(ti)
+                                    * np.exp(-tr(ti) / t1))
+            s0_der = 1 - a1 * np.exp(-ti / t1) + np.exp(-tr(ti) / t1)
+            a1_der = -s0 * np.exp(-ti / t1)
+            jacobian = np.array([t1_der, s0_der, a1_der])
+
+            if mag_image:
+                pv = _t1_function_signed(ti, t1, s0, a1)
+                jacobian = (jacobian * (pv >= 0)) - (jacobian * (pv < 0))
 
-    def __init__(self, image_slices, template_dcm=None, plate_number=None):
-        super().__init__(image_slices, template_dcm, plate_number=plate_number,
-                         dicom_order_key='InversionTime')
+            return jacobian.T
+
+        return t1_function, t1_jacobian, eqn_str
 
     def generate_fit_function(self):
         """"Create T1 fit function for magnitude/signed image and variable TI."""
         #  check if image is signed or magnitude
         if np.all(pixel_rescale(self.images[0]) >= 0):
             mag_image = True
         else:
             mag_image = False
         self.fit_function, self.fit_jacobian, self.fit_eqn_str = \
-            generate_t1_function(self.ROI_time_series[0].times,
-                                 self.ROI_time_series[0].trs,
-                                 mag_image=mag_image)
+            self.generate_t1_function(
+                self.ROI_time_series[0].times, self.ROI_time_series[0].trs,
+                mag_image=mag_image)
+
+    def est_t1_s0(self, ti, tr, t1, pv):
+        """
+        Return initial guess of s0 to seed T1 curve fitting.
+
+        Parameters
+        ----------
+        ti : array_like
+            TI values.
+        tr : array_like
+            TR values.
+        t1 : array_like
+            Estimated T1 (typically from manufacturer's documentation).
+        pv : array_like
+            Mean pixel value (signal) in ROI.
+
+        Returns
+        -------
+        array_like
+            Initial s0 guess for calculating T1 relaxation time.
+
+        """
+        return -pv / (1 - 2 * np.exp(-ti / t1) + np.exp(-tr / t1))
 
     def initialise_fit_parameters(self, t1_estimates):
         """
         Estimate fit parameters (t1, s0, a1) for T1 curve fitting.
         
         T1 estimates are provided.
         
         s0 is estimated using abs(est_t1_s0(ti, tr, t1_est, mean_pv))
             For each ROI, s0 is calculated using from both the smallest and
             largest TI, and the value with the largest mean_pv used. This
             guards against the case where division by a mean_pv close to zero
             causes a large rounding error.
             
         A1 is estimated as 2.0, the theoretical value assuming homogeneous B0
-   
+
         Parameters
         ----------
         t1_estimates : array_like
             T1 values to seed estimation. These should be the manufacturer
             provided T1 values where known.
 
         Returns
         -------
-        None.
+        s0_est
 
         """
         self.t1_est = t1_estimates
         rois = self.ROI_time_series
         rois_first_mean = np.array([roi.means[0] for roi in rois])
         rois_last_mean = np.array([roi.means[-1] for roi in rois])
-        s0_est_last = abs(est_t1_s0(rois[0].times[-1], rois[0].trs[-1],
-                                    t1_estimates, rois_last_mean))
-        s0_est_first = abs(est_t1_s0(rois[0].times[0], rois[0].trs[0],
-                                     t1_estimates, rois_first_mean))
-        self.s0_est = np.where(rois_first_mean > rois_last_mean,
+        s0_est_last = abs(self.est_t1_s0(rois[0].times[-1], rois[0].trs[-1],
+                                    self.t1_est, rois_last_mean))
+        s0_est_first = abs(self.est_t1_s0(rois[0].times[0], rois[0].trs[0],
+                                     self.t1_est, rois_first_mean))
+        s0_est = np.where(rois_first_mean > rois_last_mean,
                                s0_est_first, s0_est_last)
-        self.a1_est = np.full_like(self.s0_est, 2.0)
+        self.a1_est = np.full_like(s0_est, 2.0)
+
+        return s0_est
 
-    def find_relax_times(self):
+    def find_relax_times(self, t1_estimates, s0_est):
         """
-        Calculate T1 values. Access as ``image_stack.t1s``
+        Calculate T1 values. Access as ``image_stack.relax_fits``
+
+        Parameters
+        ----------
+        t1_estimates : array_like
+            T1 values to seed estimation. These should be the manufacturer
+            provided T1 values where known.
 
         Returns
         -------
         None.
 
         """
         rois = self.ROI_time_series
-        self.relax_fit = [scipy.optimize.curve_fit(self.fit_function,
-                                                   rois[i].times,
-                                                   rois[i].means,
-                                                   p0=[self.t1_est[i],
-                                                       self.s0_est[i],
-                                                       self.a1_est[i]],
-                                                   jac=self.fit_jacobian,
-                                                   method='lm')
-                          for i in range(len(rois))]
-
-    @property
-    def t1s(self):
-        """List T1 values for each ROI."""
-        return [fit[0][0] for fit in self.relax_fit]
-
-    @property
-    def relax_times(self):
-        """List of T1 for each ROI."""
-        return self.t1s
+        self.relax_fit = [scipy.optimize.curve_fit(
+            self.fit_function, rois[i].times, rois[i].means,
+            p0=[t1_estimates[i], s0_est[i], self.a1_est[i]],
+            jac=self.fit_jacobian, method='lm') for i in range(len(rois))]
 
 
 class T2ImageStack(ImageStack):
     """
     Calculate T2 relaxometry.
+    """
 
-    Overloads the following methods from ``ImageStack``:
-        ``generate_fit_function``
-        ``initialise_fit_parameters``
-        ``find_relax_times``
+    def __init__(self, image_slices):
+        time_attribute = "EchoTime"
+        super().__init__(image_slices, time_attribute)
 
-    """
+        self.fit_eqn_str = 'T2 with Rician noise (Raya et al 2010)'
+
+    def generate_fit_function(self):
+        """Null method in base class, may be overwritten in subclass."""
+
+    def fit_function(self, te, t2, s0, c):
+        """
+        Calculated pixel value with Rician noise model.
+        
+        Calculates pixel value from [1]_::
+            .. math::
+                S=sqrt{frac{pi alpha^2}{2}} exp(- alpha) left( (1+ 2 alpha)
+                text{I_0}(alpha) + 2 alpha text{I_1}(alpha) right)
+
+                alpha() = left(frac{S_0}{2 sigma} exp{left(-frac{text{TE}}{text{T}_2}right)} right)^2
+
+                text{I}_n() = n^text{th} text{order modified Bessel function of the first kind}
+
+        Parameters
+        ----------
+        te : array_like
+            Echo times.
+        t2 : float
+            T2 decay constant.
+        S0 : float
+            Initial pixel magnitude.
+        C : float
+            Noise parameter for Rician model (equivalent to st dev).
+
+        Returns
+        -------
+        pv : array_like
+            Theoretical pixel values (signal) at each TE.
 
-    def __init__(self, image_slices, template_dcm=None, plate_number=None):
-        super().__init__(image_slices, template_dcm, plate_number=plate_number,
-                         dicom_order_key='EchoTime')
-
-        self.fit_function = t2_function
-        self.fit_jacobian = t2_jacobian
-        self.fit_eqn_str = 's0 * np.exp(-te / t2)'
+        References
+        ----------
+        .. [1] Raya, J.G., Dietrich, O., Horng, A., Weber, J., Reiser, M.F. and
+        Glaser, C., 2010. T2 measurement in articular cartilage: impact of the
+        fitting method on accuracy and precision at low SNR. Magnetic Resonance in
+        Medicine: An Official Journal of the International Society for Magnetic
+        Resonance in Medicine, 63(1), pp.181-193.
+        """
+
+        alpha = (s0 / (2 * c) * np.exp(-te / t2)) **2
+        # NB need to use `i0e` and `ive` below to avoid numeric inaccuracy from
+        # multiplying by huge exponentials then dividing by the same exponential
+        pv = np.sqrt(np.pi/2 * c ** 2) *  \
+            ((1 + 2 * alpha) * i0e(alpha) + 2 * alpha * ive(1, alpha))
+
+        return pv
+
+    def est_t2_s0(self, te, t2, pv, c=0.0):
+        """
+        Initial guess for s0 to seed curve fitting::
+            .. math::
+                S_0=\\frac{pv-c}{exp(-TE/T_2)}
+
+
+        Parameters
+        ----------
+        te : array_like
+            Echo time(s).
+        t2 : array_like
+            T2 decay constant.
+        pv : array_like
+            Mean pixel value (signal) in ROI with ``te`` echo time.
+        c : array_like
+            Constant offset, theoretically ``full_like(te, 0.0)``.
+
+        Returns
+        -------
+        array_like
+            Initial s0 estimate.
+
+        """
+        return (pv - c) / np.exp(-te / t2)
 
     def initialise_fit_parameters(self, t2_estimates):
         """
         Estimate fit parameters (t2, s0, c) for T2 curve fitting.
         
         T2 estimates are provided.
         
         s0 is estimated using est_t2_s0(te, t2_est, mean_pv, c).
             
-        C is estimated as 0.0, the theoretical value assuming Gaussian noise.
-   
+        C is estimated as 5.0.
+
         Parameters
         ----------
         t2_estimates : array_like
             T2 values to seed estimation. These should be the manufacturer
             provided T2 values where known.
 
         Returns
         -------
-        None.
+        s0_est.
 
         """
         self.t2_est = t2_estimates
         rois = self.ROI_time_series
         rois_second_mean = np.array([roi.means[1] for roi in rois])
-        self.c_est = np.full_like(self.t2_est, 0.0)
+        self.c_est = np.full_like(self.t2_est, SEED_RICIAN_NOISE)
         # estimate s0 from second image--first image is too low.
-        self.s0_est = est_t2_s0(rois[0].times[1], t2_estimates,
+        s0_est = self.est_t2_s0(rois[0].times[1], self.t2_est,
                                 rois_second_mean, self.c_est)
-        # Get maximum time to use on fitting algorithm (5*t2_est)
-        # Truncating data after this avoids fitting Rician noise
-        self.max_fit_times = 5 * t2_estimates
 
-    def find_relax_times(self):
+        return s0_est
+
+    def find_relax_times(self, t2_estimates, s0_est):
         """
-        Calculate T2 values. Access as ``image_stack.t2s``.
+        Calculate T2 values. Access as ``image_stack.relax_times``
         
-        Uses the 'skip first echo' fit method [1]_. At times >> T2, the signal
-        is dwarfed by Rician noise (for magnitude images). This can lead to
-        inaccuracies in determining T2 as the measured signal does not tend to
-        zero. To counter this, the signal is truncated after
-        ``self.max_fit_times[i]``. At least three signals are used in the fit
-        even if this exceeds the above criteria.
-    
+        Uses the 'skip first echo' fit method [1]_ with a Rician noise model
+        [2]_. Ideally the Rician noise parameter should be determined from the
+        images rather than fitted. However, this is not possible as the noise
+        profile varies across the image due to spatial coil sensitivities and
+        whether the image is normalised or unfiltered. Fitting the noise
+        parameter makes this easier. It has an upper limit of MAX_RICIAN_NOISE,
+        currently set to 20.0.
+
+        Parameters
+        ----------
+        t2_estimates : array_like
+            T2 values to seed estimation. These should be the manufacturer
+            provided T2 values where known.
+
         Returns
         -------
         None.
         
         References
         ----------
         .. [1] McPhee, K. C., & Wilman, A. H. (2018). Limitations of skipping 
         echoes for exponential T2 fitting. Journal of Magnetic Resonance 
         Imaging, 48(5), 1432-1440. https://doi.org/10.1002/jmri.26052
+
+        .. [2] Raya, J.G., Dietrich, O., Horng, A., Weber, J., Reiser, M.F. and
+        Glaser, C., 2010. T2 measurement in articular cartilage: impact of the
+        fitting method on accuracy and precision at low SNR. Magnetic Resonance
+        in Medicine: An Official Journal of the International Society for
+         Magnetic Resonance in Medicine, 63(1), pp.181-193.
         """
-        # Require at least 4 samples (nb first sample is omitted)
-        min_number_times = 4
+
         rois = self.ROI_time_series
         #  Omit the first image data from the curve fit. This is achieved by
-        #  slicing rois[i].times[1:] and rois[i].means[1:]. Skipping odd echoes
-        #  can be implemented with rois[i].times[1::2] and .means[1::2]
-        bounds = ([0, 0], [np.inf, np.inf])
-        self.relax_fit = []
-        for i in range(len(rois)):
-            times = [t for t in rois[i].times if t < self.max_fit_times[i]]
-            if len(times) < min_number_times:
-                times = rois[i].times[:min_number_times]
-            self.relax_fit.append(
-                scipy.optimize.curve_fit(self.fit_function,
-                                         times[1:],
-                                         rois[i].means[1:len(times)],
-                                         p0=[self.t2_est[i],
-                                             self.s0_est[i]],
-                                         jac=self.fit_jacobian,
-                                         bounds=bounds,
-                                         method='trf'
-                                         )
-            )
-
-    @property
-    def t2s(self):
-        """List of T2 values for each ROI."""
-        return [fit[0][0] for fit in self.relax_fit]
-
-    @property
-    def relax_times(self):
-        """List of T2 values for each ROI."""
-        return self.t2s
-
-
-def main(dcm_target_list, *, plate_number=None,
-         show_template_fit=False, show_relax_fits=False, calc_t1=False,
-         calc_t2=False, report_path=False, show_rois=False, verbose=False):
-    """
-    Calculate T1 or T2 values for relaxometry phantom.
-    
-    Note: either ``calc_t1`` or ``calc_t2`` (but not both) must be True.
-
-    Parameters
-    ----------
-    dcm_target_list : list of pydicom.dataset.FileDataSet objects
-        List of DICOM images of a plate of the HPD relaxometry phantom.
-    plate_number : int
-        Plate number of the HPD relaxometry phantom (either 4 or 5)
-    show_template_fit : bool, optional
-        If True, displays images to show template fitting and ROIs. The 
-        default is False.
-    show_relax_fits : bool, optional
-        If True, displays graphs to show relaxometry fitting. The  default
-        is False.
-    show_rois : bool, optional
-        If True, display original image with ROIs overlaid. The default is
-        False
-    calc_t1 : bool, optional
-        Calculate T1. The default is False.
-    calc_t2 : bool, optional
-        Calculate T2. The default is False.
-    report_path : path, optional
-        If a valid file root, save template_fit images and relax_fit graphs.
-        These must first have been generated with ``show_template_fit=True``
-        or ``show_relax_fit=True``. The default is False.
-    verbose : bool, optional
-        Provide verbose output. If True, the following key / values will be
-        added to the output dictionary:
-            plate : plate_number,
-            relaxation_type : 't1' | 't2',
-            calc_times : list of T1|T2 for each sphere,
-            manufacturers_times : list of manufacturer's values for T1|T2,
-            frac_time_difference : (calc_times - manufacturers_times) / manufacturers_times
-            institution_name=index_im.InstitutionName,
-            manufacturer=index_im.Manufacturer,
-            model=index_im.ManufacturerModelName,
-            date=index_im.StudyDate,
-            output_graphics=output_files_path
-            detailed_output : dict with extensive information
-
-        The default is False.
-
-    Returns
-    -------
-
-    dict
-        {
-            rms_frac_time_difference : RMS fractional difference between
-                calculated relaxometry times and manufacturer provided data.
-        }
-    """
-
-    # check for exactly one relaxometry.py calculation
-    if all([calc_t1, calc_t2]) or not any([calc_t1, calc_t2]):
-        raise hazenlib.exceptions.ArgumentCombinationError(
-            'Must specify either calc_t1=True OR calc_t2=True.')
-
-    # check plate number specified and either 4 or 5
-    try:
-        plate_number = int(plate_number)  # convert to int if required
-    except (ValueError, TypeError):
-        pass  # will raise error at next statement
-
-    if plate_number not in [4, 5]:
-        raise hazenlib.exceptions.ArgumentCombinationError(
-            'Must specify plate_number (4 or 5)')
-
-    # Set up parameters specific to T1 or T2
-    if calc_t1:
-        ImStack = T1ImageStack
-        relax_str = 't1'
-        smooth_times = range(0, 1000, 10)
-        try:
-            template_dcm = pydicom.read_file(
-                TEMPLATE_VALUES[f'plate{plate_number}']['t1']['filename'])
-        except KeyError:
-            print(f'Could not find template with plate number: {plate_number}.'
-                  f' Please pass plate number as arg.')
-            exit()
-
-    elif calc_t2:
-        ImStack = T2ImageStack
-        relax_str = 't2'
-        smooth_times = range(0, 500, 5)
-        try:
-            template_dcm = pydicom.read_file(
-                TEMPLATE_VALUES[f'plate{plate_number}']['t2']['filename'])
-        except KeyError:
-            print(f'Could not find template with plate number: {plate_number}.'
-                  f' Please pass plate number as arg.')
-            exit()
-
-    output_files_path = {}  # save path to output files
-    image_stack = ImStack(dcm_target_list, template_dcm,
-                          plate_number=plate_number)
-    image_stack.template_fit()
-    image_stack.generate_time_series(
-        TEMPLATE_VALUES[f'plate{image_stack.plate_number}']
-        ['sphere_centres_row_col'])
-    image_stack.generate_fit_function()
-
-    if show_template_fit:
-        fig = image_stack.plot_fit()
-        if report_path:
-            old_dims = fig.get_size_inches()
-            # Improve saved image quality
-            fig.set_size_inches(24, 24)
-            save_path = f'{report_path}_template_fit.png'
-            for subplt in fig.get_axes():
-                subplt.title.set_fontsize(40)
-            fig.savefig(save_path, dpi=150)
-            output_files_path['template_fit'] = save_path
-            # Restore screen quality
-            for subplt in fig.get_axes():
-                subplt.title.set_fontsize('large')
-            fig.set_size_inches(old_dims)
-
-    if show_rois:
-        fig = image_stack.plot_rois()
-        plt.title(f'ROI positions ({relax_str.upper()}, plate {plate_number})')
-        if report_path:
-            save_path = f'{report_path}_rois.png'
-            fig.savefig(save_path, dpi=300)
-            output_files_path['rois'] = save_path
-
-    relax_published = \
-        TEMPLATE_VALUES [f'plate{image_stack.plate_number}'][relax_str] \
-            ['relax_times'][image_stack.b0_str]
-    image_stack.initialise_fit_parameters(relax_published)
-    image_stack.find_relax_times()
-    frac_time_diff = (image_stack.relax_times - relax_published) \
-                     / relax_published
-
-    if show_relax_fits:
-        rois = image_stack.ROI_time_series
-        fig = plt.figure()
-        fig.suptitle(relax_str.upper() + ' relaxometry fits')
-
-        for i in range(15):
-            plt.subplot(5, 3, i + 1)
-            plt.plot(smooth_times,
-                     image_stack.fit_function(
-                         np.array(smooth_times),
-                         *np.array(image_stack.relax_fit[i][0])),
-                     'b-')
-            plt.plot(rois[i].times, rois[i].means, 'rx')
-            if i == 14:
-                plt.title(f'[Free water] fit={image_stack.relax_times[i]:.4g}',
-                          fontsize=8)
-            else:
-                plt.title(f'[{i + 1}] fit={image_stack.relax_times[i]:.4g}, '
-                          f'pub={relax_published[i]:.4g} '
-                          f'({frac_time_diff[i] * 100:+.2f}%)',
-                          fontsize=8)
-        # plt.tight_layout(rect=(0,0,0,0.95)) # Leave suptitle space at top
-        if report_path:
-            # Improve saved image quality
-            old_dims = fig.get_size_inches()
-            fig.set_size_inches(9, 15)
-            plt.tight_layout(rect=(0, 0, 1, 0.97))
-            save_path = f'{report_path}_decay_graphs.png'
-            fig.savefig(save_path, dpi=300)
-            output_files_path['decay_graphs'] = save_path
-            # Restore screen quality
-            fig.set_size_inches(old_dims)
-
-    # Generate output dict
-    index_im = image_stack.images[0]
-    # last value is for background water. Strip before calculating RMS frac error
-    output = {'rms_frac_time_difference' : rms(frac_time_diff[:-1])}
-    if verbose:
-        output.update(dict(plate=image_stack.plate_number,
-                      relaxation_type=relax_str,
-                      calc_times=image_stack.relax_times,
-                      manufacturers_times=relax_published,
-                      frac_time_difference=frac_time_diff,
-                      institution_name=index_im.InstitutionName,
-                      manufacturer=index_im.Manufacturer,
-                      model=index_im.ManufacturerModelName,
-                      date=index_im.StudyDate,
-                      output_graphics=output_files_path))
-
-        detailed_output = {
-            'filenames': [im.filename for im in image_stack.images],
-            'ROI_means': {i: im.means for i, im in enumerate(image_stack.ROI_time_series)},
-            'TE': [im.EchoTime for im in image_stack.images],
-            'TR': [im.RepetitionTime for im in image_stack.images],
-            'TI': [im.InversionTime if hasattr(im, 'InversionTime') else None \
-                   for im in image_stack.images],
-            # fit_paramters (T1) = [[T1, s0, A1] for each ROI]
-            # fit_parameters (T2) = [[T2, s0, C] for each ROI]
-            'fit_parameters': [param[0] for param in image_stack.relax_fit],
-            'fit_equation': image_stack.fit_eqn_str
-        }
-
-        output['detailed'] = detailed_output
-
-    output_key = f"{index_im.SeriesDescription}_{index_im.SeriesNumber}_{index_im.InstanceNumber}_" \
-                 f"P{image_stack.plate_number}_{relax_str}"
-
-    plt.show()
-    return {output_key: output}
+        #  slicing rois[i].times[1:] and rois[i].means[1:].
+        #  Skipping odd echoes can be implemented with
+        #  rois[i].times[1::2] and .means[1::2]
+
+        bounds = ([0, 0, 1], [np.inf, np.inf, MAX_RICIAN_NOISE])
+
+        self.relax_fit = [scipy.optimize.curve_fit(
+            self.fit_function, rois[i].times[1:], rois[i].means[1:],
+            p0=[t2_estimates[i], s0_est[i], self.c_est[i]],
+            jac=None, bounds=bounds, method='trf') for i in range(len(rois))]
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hazen-1.2.0/hazenlib/tasks/acr_geometric_accuracy.py` & `hazen-1.3.0/hazenlib/tasks/acr_geometric_accuracy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 ACR Geometric Accuracy
+
 https://www.acraccreditation.org/-/media/acraccreditation/documents/mri/largephantomguidance.pdf
 
 Calculates geometric accuracy for slices 1 and 5 of the ACR phantom.
 
 This script calculates the horizontal and vertical lengths of the ACR phantom in Slice 1 in accordance with the ACR Guidance.
 This script calculates the horizontal, vertical and diagonal lengths of the ACR phantom in Slice 5 in accordance with the ACR Guidance.
 The average distance measurement error, maximum distance measurement error and coefficient of variation of all distance
@@ -23,219 +24,184 @@
 import os
 import numpy as np
 import skimage.morphology
 import skimage.measure
 import skimage.transform
 
 from hazenlib.HazenTask import HazenTask
+from hazenlib.ACRObject import ACRObject
 
 
 class ACRGeometricAccuracy(HazenTask):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
+        self.ACR_obj = None
 
     def run(self) -> dict:
         results = {}
-        z = []
-        for dcm in self.data:
-            z.append(dcm.ImagePositionPatient[2])
-
-        idx_sort = np.argsort(z)
-
-        for dcm in self.data:
-            if dcm.ImagePositionPatient[2] == z[idx_sort[0]]:
-                try:
-                    result1 = self.get_geometric_accuracy_slice1(dcm)
-                except Exception as e:
-                    print(f"Could not calculate the geometric accuracy for {self.key(dcm)} because of : {e}")
-                    traceback.print_exc(file=sys.stdout)
-                    continue
-
-                results[self.key(dcm)] = result1
-            elif dcm.ImagePositionPatient[2] == z[idx_sort[4]]:
-                try:
-                    result5 = self.get_geometric_accuracy_slice5(dcm)
-                except Exception as e:
-                    print(f"Could not calculate the geometric accuracy for {self.key(dcm)} because of : {e}")
-                    traceback.print_exc(file=sys.stdout)
-                    continue
+        self.ACR_obj = ACRObject(self.data)
+        slice1_dcm = self.ACR_obj.dcm[0]
+        slice5_dcm = self.ACR_obj.dcm[4]
+
+        try:
+            lengths_1 = self.get_geometric_accuracy_slice1(slice1_dcm)
+            results[self.key(slice1_dcm)] = lengths_1
+        except Exception as e:
+            print(f"Could not calculate the geometric accuracy for {self.key(slice1_dcm)} because of : {e}")
+            traceback.print_exc(file=sys.stdout)
+
+        try:
+            lengths_5 = self.get_geometric_accuracy_slice5(slice5_dcm)
+            results[self.key(slice5_dcm)] = lengths_5
+        except Exception as e:
+            print(f"Could not calculate the geometric accuracy for {self.key(slice5_dcm)} because of : {e}")
+            traceback.print_exc(file=sys.stdout)
 
-                results[self.key(dcm)] = result5
 
-        results['reports'] = {'images': self.report_files}
+        L = lengths_1 + lengths_5
 
-        L = result1 + result5
         mean_err, max_err, cov_l = self.distortion_metric(L)
+
         print(f"Mean relative measurement error is equal to {np.round(mean_err, 2)}mm")
         print(f"Maximum absolute measurement error is equal to {np.round(max_err, 2)}mm")
         print(f"Coefficient of variation of measurements is equal to {np.round(cov_l, 2)}%")
-        return results
-
-    def centroid_com(self, dcm):
-        # Calculate centroid of object using a centre-of-mass calculation
-        thresh_img = dcm > 0.25 * np.max(dcm)
-        open_img = skimage.morphology.area_opening(thresh_img, area_threshold=500)
-        bhull = skimage.morphology.convex_hull_image(open_img)
-        coords = np.nonzero(bhull)  # row major - first array is columns
-
-        sum_x = np.sum(coords[1])
-        sum_y = np.sum(coords[0])
-        cx, cy = sum_x / coords[0].shape[0], sum_y / coords[1].shape[0]
-        cxy = (round(cx), round(cy))
-
-        return bhull, cxy
-
-    def horizontal_length(self, res, mask, cxy):
-        dims = mask.shape
-        start_h = (cxy[1], 0)
-        end_h = (cxy[1], dims[0] - 1)
-        line_profile_h = skimage.measure.profile_line(mask, start_h, end_h, mode='reflect')
-        extent_h = np.nonzero(line_profile_h)[0]
-        dist_h = (extent_h[-1] - extent_h[0]) * res[0]
-
-        h_dict = {
-            'Start': start_h,
-            'End': end_h,
-            'Extent': extent_h,
-            'Distance': dist_h
-        }
-        return h_dict
 
-    def vertical_length(self, res, mask, cxy):
-        dims = mask.shape
-        start_v = (0, cxy[0])
-        end_v = (dims[1] - 1, cxy[0])
-        line_profile_v = skimage.measure.profile_line(mask, start_v, end_v, mode='reflect')
-        extent_v = np.nonzero(line_profile_v)[0]
-        dist_v = (extent_v[-1] - extent_v[0]) * res[1]
-
-        v_dict = {
-            'Start': start_v,
-            'End': end_v,
-            'Extent': extent_v,
-            'Distance': dist_v
-        }
-        return v_dict
-
-    def rotate_point(self, origin, point, angle):
-        theta = np.radians(angle)
-        c, s = np.cos(theta), np.sin(theta)
+        # only return reports if requested
+        if self.report:
+            results['reports'] = {'images': self.report_files}
 
-        x_prime = origin[0] + c * (point[0] - origin[0]) - s * (point[1] - origin[1])
-        y_prime = origin[1] + s * (point[0] - origin[0]) + c * (point[1] - origin[1])
-        return x_prime, y_prime
+        return results
 
-    def diagonal_lengths(self, res, mask, cxy):
+    def diagonal_lengths(self, res, img, cxy):
         eff_res = np.sqrt(np.mean(np.square(res)))
-        mask_rotate = skimage.transform.rotate(mask, 45, center=(cxy[0], cxy[1]))
+        img_rotate = skimage.transform.rotate(img, 45, center=(cxy[0], cxy[1]))
 
-        h_dict = self.horizontal_length(res, mask_rotate, cxy)
-        extent_h = h_dict['Extent']
+        length_dict = self.ACR_obj.measure_orthogonal_lengths(img_rotate)
+        extent_h = length_dict['Horizontal Extent']
 
         origin = (cxy[0], cxy[1])
         start = (extent_h[0], cxy[1])
         end = (extent_h[-1], cxy[1])
-        se_x_start, se_y_start = self.rotate_point(origin, start, 45)
-        se_x_end, se_y_end = self.rotate_point(origin, end, 45)
+        se_x_start, se_y_start = ACRObject.rotate_point(origin, start, 45)
+        se_x_end, se_y_end = ACRObject.rotate_point(origin, end, 45)
 
         dist_se = np.sqrt(np.sum(np.square([se_x_end - se_x_start, se_y_end - se_y_start]))) * eff_res
         se_dict = {
             'Start': (se_x_start, se_y_start),
             'End': (se_x_end, se_y_end),
             'Extent': (se_x_end - se_x_start, se_y_end - se_y_start),
             'Distance': dist_se
         }
 
-        v_dict = self.vertical_length(res, mask_rotate, cxy)
-        extent_v = v_dict['Extent']
+        extent_v = length_dict['Vertical Extent']
 
         start = (cxy[0], extent_v[0])
         end = (cxy[0], extent_v[-1])
-        sw_x_start, sw_y_start = self.rotate_point(origin, start, 45)
-        sw_x_end, sw_y_end = self.rotate_point(origin, end, 45)
+        sw_x_start, sw_y_start = ACRObject.rotate_point(origin, start, 45)
+        sw_x_end, sw_y_end = ACRObject.rotate_point(origin, end, 45)
 
         dist_sw = np.sqrt(np.sum(np.square([sw_x_end - sw_x_start, sw_y_end - sw_y_start]))) * eff_res
         sw_dict = {
             'Start': (sw_x_start, sw_y_start),
             'End': (sw_x_end, sw_y_end),
             'Extent': (sw_x_end - sw_x_start, sw_y_end - sw_y_start),
             'Distance': dist_sw
         }
 
         return sw_dict, se_dict
 
     def get_geometric_accuracy_slice1(self, dcm):
         img = dcm.pixel_array
-        res = dcm.PixelSpacing
-        mask, cxy = self.centroid_com(img)
 
-        h_dict = self.horizontal_length(res, mask, cxy)
-        v_dict = self.vertical_length(res, mask, cxy)
+        mask = self.ACR_obj.mask_image(self.ACR_obj.images[6])
+        cxy = self.ACR_obj.centre
+        length_dict = self.ACR_obj.measure_orthogonal_lengths(mask)
 
         if self.report:
             import matplotlib.pyplot as plt
-            fig = plt.figure()
-            fig.set_size_inches(8, 8)
-            plt.imshow(img)
-
-            plt.arrow(h_dict['Extent'][0], cxy[1], h_dict['Extent'][-1] - h_dict['Extent'][0], 1, color='blue',
-                      length_includes_head=True, head_width=5)
-            plt.arrow(cxy[0], v_dict['Extent'][0], 1, v_dict['Extent'][-1] - v_dict['Extent'][0], color='orange',
-                      length_includes_head=True, head_width=5)
-            plt.legend([str(np.round(h_dict['Distance'], 2)) + 'mm',
-                        str(np.round(v_dict['Distance'], 2)) + 'mm'])
-            plt.axis('off')
-            plt.title('Geometric Accuracy for Slice 1')
+            fig, axes = plt.subplots(3, 1)
+            fig.set_size_inches(8, 24)
+            fig.tight_layout(pad=4)
+
+            axes[0].imshow(img)
+            axes[0].scatter(cxy[0], cxy[1], c='red')
+            axes[0].set_title('Centroid Location')
+
+            axes[1].imshow(mask)
+            axes[1].set_title('Thresholding Result')
+
+            axes[2].imshow(img)
+            axes[2].arrow(length_dict['Horizontal Extent'][0], cxy[1],
+                          length_dict['Horizontal Extent'][-1] - length_dict['Horizontal Extent'][0], 1, color='blue',
+                          length_includes_head=True, head_width=5)
+            axes[2].arrow(cxy[0], length_dict['Vertical Extent'][0], 1, length_dict['Vertical Extent'][-1] -
+                          length_dict['Vertical Extent'][0], color='orange', length_includes_head=True, head_width=5)
+            axes[2].legend([str(np.round(length_dict['Horizontal Distance'], 2)) + 'mm',
+                            str(np.round(length_dict['Vertical Distance'], 2)) + 'mm'])
+            axes[2].axis('off')
+            axes[2].set_title('Geometric Accuracy for Slice 1')
 
             img_path = os.path.realpath(os.path.join(self.report_path, f'{self.key(dcm)}.png'))
             fig.savefig(img_path)
             self.report_files.append(img_path)
 
-        return h_dict['Distance'], v_dict['Distance']
+        return length_dict['Horizontal Distance'], length_dict['Vertical Distance']
 
     def get_geometric_accuracy_slice5(self, dcm):
         img = dcm.pixel_array
         res = dcm.PixelSpacing
-        mask, cxy = self.centroid_com(img)
+        mask = self.ACR_obj.mask_image(self.ACR_obj.images[6])
+        cxy = self.ACR_obj.centre
 
-        h_dict = self.horizontal_length(res, mask, cxy)
-        v_dict = self.vertical_length(res, mask, cxy)
+        length_dict = self.ACR_obj.measure_orthogonal_lengths(mask)
         sw_dict, se_dict = self.diagonal_lengths(res, mask, cxy)
 
         if self.report:
             import matplotlib.pyplot as plt
-            fig = plt.figure()
-            fig.set_size_inches(8, 8)
-            plt.imshow(img)
-
-            plt.arrow(h_dict['Extent'][0], cxy[1], h_dict['Extent'][-1] - h_dict['Extent'][0], 1, color='blue',
-                      length_includes_head=True, head_width=5)
-            plt.arrow(cxy[0], v_dict['Extent'][0], 1, v_dict['Extent'][-1] - v_dict['Extent'][0], color='orange',
-                      length_includes_head=True, head_width=5)
-
-            plt.arrow(se_dict['Start'][0], se_dict['Start'][1], se_dict['Extent'][0], se_dict['Extent'][1],
-                      color='purple', length_includes_head=True, head_width=5)
-            plt.arrow(sw_dict['Start'][0], sw_dict['Start'][1], sw_dict['Extent'][0], sw_dict['Extent'][1],
-                      color='yellow', length_includes_head=True, head_width=5)
-
-            plt.legend([str(np.round(h_dict['Distance'], 2)) + 'mm',
-                        str(np.round(v_dict['Distance'], 2)) + 'mm',
-                        str(np.round(sw_dict['Distance'], 2)) + 'mm',
-                        str(np.round(se_dict['Distance'], 2)) + 'mm'])
-            plt.axis('off')
-            plt.title('Geometric Accuracy for Slice 5')
+            fig, axes = plt.subplots(3, 1)
+            fig.set_size_inches(8, 24)
+            fig.tight_layout(pad=4)
+
+            axes[0].imshow(img)
+            axes[0].scatter(cxy[0], cxy[1], c='red')
+            axes[0].axis('off')
+            axes[0].set_title('Centroid Location')
+
+            axes[1].imshow(mask)
+            axes[1].axis('off')
+            axes[1].set_title('Thresholding Result')
+
+            axes[2].imshow(img)
+            axes[2].arrow(length_dict['Horizontal Extent'][0], cxy[1], length_dict['Horizontal Extent'][-1]
+                          - length_dict['Horizontal Extent'][0], 1, color='blue', length_includes_head=True,
+                          head_width=5)
+            axes[2].arrow(cxy[0], length_dict['Vertical Extent'][0], 1, length_dict['Vertical Extent'][-1] -
+                          length_dict['Vertical Extent'][0], color='orange', length_includes_head=True, head_width=5)
+            axes[2].arrow(se_dict['Start'][0], se_dict['Start'][1], se_dict['Extent'][0], se_dict['Extent'][1],
+                          color='purple', length_includes_head=True, head_width=5)
+            axes[2].arrow(sw_dict['Start'][0], sw_dict['Start'][1], sw_dict['Extent'][0], sw_dict['Extent'][1],
+                          color='yellow', length_includes_head=True, head_width=5)
+
+            axes[2].legend([str(np.round(length_dict['Horizontal Distance'], 2)) + 'mm',
+                            str(np.round(length_dict['Vertical Distance'], 2)) + 'mm',
+                            str(np.round(sw_dict['Distance'], 2)) + 'mm',
+                            str(np.round(se_dict['Distance'], 2)) + 'mm'])
+            axes[2].axis('off')
+            axes[2].set_title('Geometric Accuracy for Slice 5')
 
             img_path = os.path.realpath(os.path.join(self.report_path, f'{self.key(dcm)}.png'))
             fig.savefig(img_path)
             self.report_files.append(img_path)
 
-        return h_dict['Distance'], v_dict['Distance'], sw_dict['Distance'], se_dict['Distance']
+        return length_dict['Horizontal Distance'], length_dict['Vertical Distance'], \
+            sw_dict['Distance'], se_dict['Distance']
 
-    def distortion_metric(self, L):
+    @staticmethod
+    def distortion_metric(L):
         err = [x - 190 for x in L]
         mean_err = np.mean(err)
 
         max_err = np.max(np.absolute(err))
         cov_l = 100 * np.std(L) / np.mean(L)
 
         return mean_err, max_err, cov_l
```

### Comparing `hazen-1.2.0/hazenlib/tasks/acr_ghosting.py` & `hazen-1.3.0/hazenlib/tasks/acr_ghosting.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 ACR Ghosting
 
 https://www.acraccreditation.org/-/media/acraccreditation/documents/mri/largephantomguidance.pdf
 
-Calculates percent-signal ghosting for slice 7 of the ACR phantom.
+Calculates the percent-signal ghosting for slice 7 of the ACR phantom.
 
 This script calculates the percentage signal ghosting in accordance with the ACR Guidance.
 This is done by first defining a large 200cm2 ROI before placing 10cm2 elliptical ROIs outside the phantom along the
 cardinal directions. The results are also visualised.
 
 Created by Yassine Azma
 yassine.azma@rmh.nhs.uk
@@ -15,67 +15,51 @@
 14/11/2022
 """
 
 import sys
 import traceback
 import os
 import numpy as np
-import skimage.morphology
 
 from hazenlib.HazenTask import HazenTask
+from hazenlib.ACRObject import ACRObject
 
 
 class ACRGhosting(HazenTask):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
+        self.ACR_obj = None
 
     def run(self) -> dict:
         results = {}
-        z = []
-        for dcm in self.data:
-            z.append(dcm.ImagePositionPatient[2])
-
-        idx_sort = np.argsort(z)
-
-        for dcm in self.data:
-            if dcm.ImagePositionPatient[2] == z[idx_sort[6]]:
-                try:
-                    result = self.get_signal_ghosting(dcm)
-                except Exception as e:
-                    print(f"Could not calculate the percent-signal ghosting for {self.key(dcm)} because of : {e}")
-                    traceback.print_exc(file=sys.stdout)
-                    continue
+        self.ACR_obj = ACRObject(self.data)
+        ghosting_dcm = self.ACR_obj.dcm[6]
 
-                results[self.key(dcm)] = result
+        try:
+            result = self.get_signal_ghosting(ghosting_dcm)
+            results[self.key(ghosting_dcm)] = result
+        except Exception as e:
+            print(f"Could not calculate the percent-signal ghosting for {self.key(ghosting_dcm)} because of : {e}")
+            traceback.print_exc(file=sys.stdout)
 
-        results['reports'] = {'images': self.report_files}
+        # only return reports if requested
+        if self.report:
+            results['reports'] = {'images': self.report_files}
 
         return results
 
-    def centroid_com(self, dcm):
-        # Calculate centroid of object using a centre-of-mass calculation
-        thresh_img = dcm > 0.25 * np.max(dcm)
-        open_img = skimage.morphology.area_opening(thresh_img, area_threshold=500)
-        bhull = skimage.morphology.convex_hull_image(open_img)
-        coords = np.nonzero(bhull)  # row major - first array is columns
-
-        sum_x = np.sum(coords[1])
-        sum_y = np.sum(coords[0])
-        cxy = sum_x / coords[0].shape, sum_y / coords[1].shape
-
-        cxy = [cxy[0].astype(int), cxy[1].astype(int)]
-        return bhull, cxy
-
     def get_signal_ghosting(self, dcm):
         img = dcm.pixel_array
         res = dcm.PixelSpacing  # In-plane resolution from metadata
         r_large = np.ceil(80 / res[0]).astype(int)  # Required pixel radius to produce ~200cm2 ROI
         dims = img.shape
-        mask, cxy = self.centroid_com(img)
+
+        mask = self.ACR_obj.mask_image(img)
+        cxy = self.ACR_obj.centre
 
         nx = np.linspace(1, dims[0], dims[0])
         ny = np.linspace(1, dims[1], dims[1])
 
         x, y = np.meshgrid(nx, ny)
 
         lroi = np.square(x - cxy[0]) + np.square(y - cxy[1] - np.divide(5, res[1])) <= np.square(r_large)
@@ -90,23 +74,23 @@
         if left_fov_to_centre < 0 or centre_to_left_phantom > w_point:
             diffs = [left_fov_to_centre, centre_to_left_phantom - w_point]
             ind = diffs.index(max(diffs, key=abs))
             w_factor = (sad / 2) / (sad / 2 - np.absolute(diffs[ind]))  # ellipse scaling factor
         else:
             w_factor = 1
 
-        w_ellipse = np.square((y - w_centre[0]) / (4 * w_factor)) + np.square(
-            (x - w_centre[1]) * w_factor) <= np.square(
-            10 / res[0])  # generate ellipse mask
+        w_ellipse = np.square((y - w_centre[0]) / (4 * w_factor)) + np.square((x - w_centre[1]) * w_factor) <= \
+                    np.square(10 / res[0])  # generate ellipse mask
 
         # EAST ELLIPSE
         e_point = np.argwhere(np.sum(mask, 0) > 0)[-1]  # find last column in mask
         e_centre = [cxy[1], e_point + np.ceil((dims[1] - e_point) / 2)]  # initialise centre of ellipse
         right_fov_to_centre = e_centre[1] + sad / 2 + 5  # edge of ellipse towards right FoV (+ tolerance)
-        centre_to_right_phantom = e_centre[1] - sad/2 - 5  # edge of ellipse towards right side of phantom (+ tolerance)
+        centre_to_right_phantom = e_centre[
+                                      1] - sad / 2 - 5  # edge of ellipse towards right side of phantom (+ tolerance)
         if right_fov_to_centre > dims[1] - 1 or centre_to_right_phantom < e_point:
             diffs = [dims[1] - 1 - right_fov_to_centre, centre_to_right_phantom - e_point]
             ind = diffs.index(max(diffs, key=abs))
             e_factor = (sad / 2) / (sad / 2 - np.absolute(diffs[ind]))  # ellipse scaling factor
         else:
             e_factor = 1
 
@@ -151,46 +135,54 @@
         e_ellipse_val = np.mean(img[np.nonzero(e_ellipse)])
         n_ellipse_val = np.mean(img[np.nonzero(n_ellipse)])
         s_ellipse_val = np.mean(img[np.nonzero(s_ellipse)])
 
         psg = 100 * np.absolute(
             ((n_ellipse_val + s_ellipse_val) - (w_ellipse_val + e_ellipse_val)) / (2 * large_roi_val))
 
-        psg = np.round(psg,3)
+        psg = np.round(psg, 3)
 
         if self.report:
             import matplotlib.pyplot as plt
+            fig, axes = plt.subplots(2, 1)
+            fig.set_size_inches(8, 16)
+            fig.tight_layout(pad=4)
+
             theta = np.linspace(0, 2 * np.pi, 360)
-            fig = plt.figure()
-            fig.set_size_inches(8, 8)
-            plt.imshow(img)
-
-            plt.plot(r_large * np.cos(theta) + cxy[0], r_large * np.sin(theta) + cxy[1] + 5 / res[1], c='black')
-            plt.text(cxy[0] - 3 * np.floor(10 / res[0]), cxy[1] + np.floor(10 / res[1]),
-                     "Mean = " + str(np.round(large_roi_val, 2)), c='white')
-
-            plt.plot(10. / res[0] * np.cos(theta) / w_factor + w_centre[1],
-                     10. / res[0] * np.sin(theta) * 4 * w_factor + w_centre[0], c='red')
-            plt.text(w_centre[1] - np.floor(10 / res[0]), w_centre[0], "Mean = " + str(np.round(w_ellipse_val, 2)),
-                     c='white')
-
-            plt.plot(10. / res[0] * np.cos(theta) / e_factor + e_centre[1],
-                     10. / res[0] * np.sin(theta) * 4 * e_factor + e_centre[0], c='red')
-            plt.text(e_centre[1] - np.floor(30 / res[0]), e_centre[0], "Mean = " + str(np.round(e_ellipse_val, 2)),
-                     c='white')
-
-            plt.plot(10. / res[0] * np.cos(theta) * 4 * n_factor + n_centre[1],
-                     10. / res[0] * np.sin(theta) / n_factor + n_centre[0], c='red')
-            plt.text(n_centre[1] - 5 * np.floor(10 / res[0]), n_centre[0], "Mean = " + str(np.round(n_ellipse_val, 2)),
-                     c='white')
-
-            plt.plot(10. / res[0] * np.cos(theta) * 4 * s_factor + s_centre[1],
-                     10. / res[0] * np.sin(theta) / s_factor + s_centre[0], c='red')
-            plt.text(s_centre[1], s_centre[0], "Mean = " + str(np.round(s_ellipse_val, 2)), c='white')
 
-            plt.axis('off')
-            plt.title('Percent Signal Ghosting = ' + str(np.round(psg, 3)) + '%')
+            axes[0].imshow(img)
+            axes[0].scatter(cxy[0], cxy[1], c='red')
+            axes[0].axis('off')
+            axes[0].set_title('Centroid Location')
+
+            axes[1].imshow(img)
+            axes[1].plot(r_large * np.cos(theta) + cxy[0], r_large * np.sin(theta) + cxy[1] + 5 / res[1], c='black')
+            axes[1].text(cxy[0] - 3 * np.floor(10 / res[0]), cxy[1] + np.floor(10 / res[1]),
+                         "Mean = " + str(np.round(large_roi_val, 2)), c='white')
+
+            axes[1].plot(10. / res[0] * np.cos(theta) / w_factor + w_centre[1],
+                         10. / res[0] * np.sin(theta) * 4 * w_factor + w_centre[0], c='red')
+            axes[1].text(w_centre[1] - np.floor(10 / res[0]), w_centre[0], "Mean = " + str(np.round(w_ellipse_val, 2)),
+                         c='white')
+
+            axes[1].plot(10. / res[0] * np.cos(theta) / e_factor + e_centre[1],
+                         10. / res[0] * np.sin(theta) * 4 * e_factor + e_centre[0], c='red')
+            axes[1].text(e_centre[1] - np.floor(30 / res[0]), e_centre[0], "Mean = " + str(np.round(e_ellipse_val, 2)),
+                         c='white')
+
+            axes[1].plot(10. / res[0] * np.cos(theta) * 4 * n_factor + n_centre[1],
+                         10. / res[0] * np.sin(theta) / n_factor + n_centre[0], c='red')
+            axes[1].text(n_centre[1] - 5 * np.floor(10 / res[0]), n_centre[0],
+                         "Mean = " + str(np.round(n_ellipse_val, 2)),
+                         c='white')
+
+            axes[1].plot(10. / res[0] * np.cos(theta) * 4 * s_factor + s_centre[1],
+                         10. / res[0] * np.sin(theta) / s_factor + s_centre[0], c='red')
+            axes[1].text(s_centre[1], s_centre[0], "Mean = " + str(np.round(s_ellipse_val, 2)), c='white')
+
+            axes[1].axis('off')
+            axes[1].set_title('Percent Signal Ghosting = ' + str(np.round(psg, 3)) + '%')
             img_path = os.path.realpath(os.path.join(self.report_path, f'{self.key(dcm)}.png'))
             fig.savefig(img_path)
             self.report_files.append(img_path)
 
         return psg
```

### Comparing `hazen-1.2.0/hazenlib/tasks/acr_slice_position.py` & `hazen-1.3.0/hazenlib/tasks/acr_slice_position.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,68 +29,41 @@
 import scipy
 import os
 import numpy as np
 import skimage.morphology
 import skimage.measure
 
 from hazenlib.HazenTask import HazenTask
-
-
-def find_n_peaks(data, n, height=1):
-    peaks = scipy.signal.find_peaks(data, height)
-    pk_heights = peaks[1]['peak_heights']
-    pk_ind = peaks[0]
-    highest_peaks = pk_ind[(-pk_heights).argsort()[:n]]  # find n highest peaks
-
-    return np.sort(highest_peaks)
+from hazenlib.ACRObject import ACRObject
 
 
 class ACRSlicePosition(HazenTask):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
+        self.ACR_obj = None
 
     def run(self) -> dict:
         results = {}
-        z = []
-        for dcm in self.data:
-            z.append(dcm.ImagePositionPatient[2])
-
-        idx_sort = np.argsort(z)
-
-        for dcm in self.data:
-            curr_z = dcm.ImagePositionPatient[2]
-            if curr_z in (z[idx_sort[0]], z[idx_sort[10]]):
-                try:
-                    result = self.get_slice_position(dcm)
-                except Exception as e:
-                    print(f"Could not calculate the bar length difference for {self.key(dcm)} because of : {e}")
-                    traceback.print_exc(file=sys.stdout)
-                    continue
-
+        self.ACR_obj = ACRObject(self.data)
+        dcms = [self.ACR_obj.dcm[0], self.ACR_obj.dcm[-1]]
+        for dcm in dcms:
+            try:
+                result = self.get_slice_position(dcm)
                 results[self.key(dcm)] = result
-
-        results['reports'] = {'images': self.report_files}
+            except Exception as e:
+                print(f"Could not calculate the bar length difference for {self.key(dcm)} because of : {e}")
+                traceback.print_exc(file=sys.stdout)
+                continue
+        # only return reports if requested
+        if self.report:
+            results['reports'] = {'images': self.report_files}
 
         return results
 
-    def centroid_com(self, dcm):
-        # Calculate centroid of object using a centre-of-mass calculation
-        thresh_img = dcm > 0.25 * np.max(dcm)
-        open_img = skimage.morphology.area_opening(thresh_img, area_threshold=500)
-        bhull = skimage.morphology.convex_hull_image(open_img)
-        coords = np.nonzero(bhull)  # row major - first array is columns
-
-        sum_x = np.sum(coords[1])
-        sum_y = np.sum(coords[0])
-        cxy = sum_x / coords[0].shape, sum_y / coords[1].shape
-
-        cxy = [cxy[0].astype(int), cxy[1].astype(int)]
-        return bhull, cxy
-
     def find_wedges(self, img, mask, res):
         # X COORDINATES
         x_investigate_region = np.ceil(35 / res[0]).astype(int)  # define width of region to test (comparable to wedges)
 
         if np.mod(x_investigate_region, 2) == 0:
             # we want an odd number to see -N to N points in the x direction
             x_investigate_region = x_investigate_region + 1
@@ -109,15 +82,15 @@
 
             invest_x.append(t * line_prof_x)  # mask unwanted values out and append
 
         invest_x = np.array(invest_x).T  # transpose array
         mean_x_profile = np.mean(invest_x, 1)  # mean of horizontal projections of phantom
         abs_diff_x_profile = np.abs(np.diff(mean_x_profile))  # absolute first derivative of mean
 
-        x_peaks = find_n_peaks(abs_diff_x_profile, 2)  # find two highest peaks
+        x_peaks, _ = self.ACR_obj.find_n_highest_peaks(abs_diff_x_profile, 2)  # find two highest peaks
         x_locs = w_point + x_peaks  # x coordinates of these peaks in image coordinate system(before diff operation)
 
         width_pts = [x_locs[0], x_locs[1]]  # width of wedges
         width = np.max(width_pts) - np.min(width_pts)  # width
 
         # rough midpoints of wedges
         x_pts = np.round([np.min(width_pts) + 0.25 * width, np.max(width_pts) - 0.25 * width]).astype(int)
@@ -141,31 +114,32 @@
                                                        mode='constant').flatten()
             invest_y.append(c * line_prof_y)
 
         invest_y = np.array(invest_y).T  # transpose array
         mean_y_profile = np.mean(invest_y, 1)  # mean of vertical projections of phantom
         abs_diff_y_profile = np.abs(np.diff(mean_y_profile))  # absolute first derivative of mean
 
-        y_peaks = find_n_peaks(abs_diff_y_profile, 2)  # find two highest peaks
+        y_peaks, _ = self.ACR_obj.find_n_highest_peaks(abs_diff_y_profile, 2)  # find two highest peaks
         y_locs = w_point + y_peaks - 1  # y coordinates of these peaks in image coordinate system(before diff operation)
 
         if y_locs[1] - y_locs[0] < 5 / res[1]:
             y = [n_point + round(10 / res[1])]  # if peaks too close together, use phantom geometry
         else:
             y = np.round(np.min(y_locs) + 0.25 * np.abs(np.diff(y_locs)))  # define y coordinate
 
         dist_to_y = np.abs(n_point - y[0]) * res[1]  # distance to y from top of phantom
-        y_pts = np.append(y, np.round(y[0] + (47 - dist_to_y) / res[1])).astype(int)  # place 2nd y point 47mm from top of phantom
+        y_pts = np.append(y, np.round(y[0] + (47 - dist_to_y) / res[1])).astype(
+            int)  # place 2nd y point 47mm from top of phantom
 
         return x_pts, y_pts
 
     def get_slice_position(self, dcm):
         img = dcm.pixel_array
         res = dcm.PixelSpacing  # In-plane resolution from metadata
-        mask, cxy = self.centroid_com(img)
+        mask = self.ACR_obj.mask_image(self.ACR_obj.images[6])
         x_pts, y_pts = self.find_wedges(img, mask, res)
 
         line_prof_L = skimage.measure.profile_line(img, (y_pts[0], x_pts[0]), (y_pts[1], x_pts[0]),
                                                    mode='constant').flatten()  # line profile through left wedge
         line_prof_R = skimage.measure.profile_line(img, (y_pts[0], x_pts[1]), (y_pts[1], x_pts[1]),
                                                    mode='constant').flatten()  # line profile through right wedge
 
@@ -173,15 +147,15 @@
         x = np.arange(1, len(line_prof_L) + 1)
         new_x = np.arange(1, len(line_prof_L) + (1 / interp_factor), (1 / interp_factor))
 
         interp_line_prof_L = scipy.interpolate.interp1d(x, line_prof_L)(new_x)  # interpolate left line profile
         interp_line_prof_R = scipy.interpolate.interp1d(x, line_prof_R)(new_x)  # interpolate right line profile
 
         delta = interp_line_prof_L - interp_line_prof_R  # difference of line profiles
-        peaks = find_n_peaks(abs(delta), 2, 0.5 * np.max(abs(delta)))  # find two highest peaks
+        peaks, _ = ACRObject.find_n_highest_peaks(abs(delta), 2, 0.5 * np.max(abs(delta)))  # find two highest peaks
 
         if len(peaks) == 1:
             peaks = [peaks[0] - 50, peaks[0] + 50]  # if only one peak, set dummy range
 
         # set multiplier for right or left shift based on sign of peak
         pos = 1 if np.max(-delta[peaks[0]:peaks[1]]) < np.max(delta[peaks[0]:peaks[1]]) else -1
 
@@ -207,54 +181,55 @@
         temp = np.argwhere(err == np.min(err[err > 0]))[0]  # find minimum non-zero error
         shift = -lag[temp][0] if pos == 1 else lag[temp][0]  # find shift corresponding to above error
 
         dL = np.round(pos * np.abs(shift) * (1 / interp_factor) * res[1], 2)  # calculate bar length difference
 
         if self.report:
             import matplotlib.pyplot as plt
-            fig = plt.figure()
-            plt.suptitle('Bar Length Difference = ' + str(np.round(dL, 2)) + 'mm', x=0.5, ha='center')
-            fig.set_size_inches(8, 8)
-
-            plt.subplot(2, 2, (1, 3))
-            plt.imshow(img)
-            plt.plot([x_pts[0], x_pts[0]], [y_pts[0], y_pts[1]], 'b')
-            plt.plot([x_pts[1], x_pts[1]], [y_pts[0], y_pts[1]], 'r')
-            plt.axis('off')
-            plt.tight_layout()
-
-            plt.subplot(2, 2, 2)
-            plt.grid()
-            plt.plot((1 / interp_factor) * np.linspace(1, len(interp_line_prof_L), len(interp_line_prof_L)) * res[1],
-                     interp_line_prof_L, 'b')
-            plt.plot((1 / interp_factor) * np.linspace(1, len(interp_line_prof_R), len(interp_line_prof_R)) * res[1],
-                     interp_line_prof_R, 'r')
-            plt.title('Original Line Profiles')
-            plt.xlabel('Relative Pixel Position (mm)')
-            plt.tight_layout()
-
-            plt.subplot(2, 2, 4)
-            plt.grid()
-            plt.plot((1 / interp_factor) * np.linspace(1, len(interp_line_prof_L), len(interp_line_prof_L)) * res[1],
+            fig, axes = plt.subplots(4, 1)
+            fig.set_size_inches(8, 32)
+            fig.tight_layout(pad=4)
+
+            axes[0].imshow(mask)
+            axes[0].axis('off')
+            axes[0].set_title('Thresholding Result')
+
+            axes[1].imshow(img)
+            axes[1].plot([x_pts[0], x_pts[0]], [y_pts[0], y_pts[1]], 'b')
+            axes[1].plot([x_pts[1], x_pts[1]], [y_pts[0], y_pts[1]], 'r')
+            axes[1].axis('off')
+            axes[1].set_title('Line Profiles')
+
+            axes[2].grid()
+            axes[2].plot(
+                (1 / interp_factor) * np.linspace(1, len(interp_line_prof_L), len(interp_line_prof_L)) * res[1],
+                interp_line_prof_L, 'b')
+            axes[2].plot(
+                (1 / interp_factor) * np.linspace(1, len(interp_line_prof_R), len(interp_line_prof_R)) * res[1],
+                interp_line_prof_R, 'r')
+            axes[2].set_title('Original Line Profiles')
+            axes[2].set_xlabel('Relative Pixel Position (mm)')
+
+            axes[3].plot((1 / interp_factor) * np.linspace(1, len(interp_line_prof_L), len(interp_line_prof_L)) * res[1],
                      interp_line_prof_L, 'b')
 
             shift_line = np.roll(interp_line_prof_R, pos * shift)
             if shift < 0 and pos == -1:
                 shift_line[0:np.abs(shift)] = np.nan
             elif shift < 0 and pos == 1:
                 shift_line[pos * shift:] = np.nan
             elif shift > 0 and pos == -1:
                 shift_line[pos * shift:] = np.nan
             else:
                 shift_line[0:np.abs(pos) * shift] = np.nan
 
-            plt.plot((1 / interp_factor) * np.linspace(1, len(interp_line_prof_L), len(interp_line_prof_L)) * res[1],
+            axes[3].grid()
+            axes[3].plot((1 / interp_factor) * np.linspace(1, len(interp_line_prof_L), len(interp_line_prof_L)) * res[1],
                      shift_line, 'r')
-            plt.title('Shifted Line Profiles')
-            plt.xlabel('Relative Pixel Position (mm)')
-            plt.tight_layout()
+            axes[3].set_title('Shifted Line Profiles')
+            axes[3].set_xlabel('Relative Pixel Position (mm)')
 
             img_path = os.path.realpath(os.path.join(self.report_path, f'{self.key(dcm)}.png'))
             fig.savefig(img_path)
             self.report_files.append(img_path)
 
         return dL
```

### Comparing `hazen-1.2.0/hazenlib/tasks/acr_slice_thickness.py` & `hazen-1.3.0/hazenlib/tasks/acr_slice_thickness.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,71 +12,45 @@
 
 31/01/2022
 """
 
 import sys
 import traceback
 import os
-from hazenlib.HazenTask import HazenTask
 import numpy as np
 import skimage.morphology
 import skimage.measure
 import scipy
 
-
-def find_n_peaks(data, n, height=1):
-    peaks = scipy.signal.find_peaks(data, height)
-    pk_heights = peaks[1]['peak_heights']
-    pk_ind = peaks[0]
-    highest_peaks = pk_ind[(-pk_heights).argsort()[:n]]  # find n highest peaks
-
-    return np.sort(highest_peaks)
+from hazenlib.HazenTask import HazenTask
+from hazenlib.ACRObject import ACRObject
 
 
 class ACRSliceThickness(HazenTask):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
+        self.ACR_obj = None
 
     def run(self) -> dict:
         results = {}
-        z = []
-        for dcm in self.data:
-            z.append(dcm.ImagePositionPatient[2])
-
-        idx_sort = np.argsort(z)
-        for dcm in self.data:
-            curr_z = dcm.ImagePositionPatient[2]
-            if curr_z == z[idx_sort[0]]:
-                try:
-                    result = self.get_slice_thickness(dcm)
-                except Exception as e:
-                    print(f"Could not calculate the slice thickness for {self.key(dcm)} because of : {e}")
-                    traceback.print_exc(file=sys.stdout)
-                    continue
+        self.ACR_obj = ACRObject(self.data)
+        slice_thickness_dcm = self.ACR_obj.dcm[0]
+        try:
+            result = self.get_slice_thickness(slice_thickness_dcm)
+            results[self.key(slice_thickness_dcm)] = result
+        except Exception as e:
+            print(f"Could not calculate the slice thickness for {self.key(slice_thickness_dcm)} because of : {e}")
+            traceback.print_exc(file=sys.stdout)
 
-                results[self.key(dcm)] = result
-
-        results['reports'] = {'images': self.report_files}
+        # only return reports if requested
+        if self.report:
+            results['reports'] = {'images': self.report_files}
 
         return results
 
-    def centroid_com(self, dcm):
-        # Calculate centroid of object using a centre-of-mass calculation
-        thresh_img = dcm > 0.25 * np.max(dcm)
-        open_img = skimage.morphology.area_opening(thresh_img, area_threshold=500)
-        bhull = skimage.morphology.convex_hull_image(open_img)
-        coords = np.nonzero(bhull)  # row major - first array is columns
-
-        sum_x = np.sum(coords[1])
-        sum_y = np.sum(coords[0])
-        cxy = sum_x / coords[0].shape, sum_y / coords[1].shape
-
-        cxy = [int(cxy[0]), int(cxy[1])]
-        return bhull, cxy
-
     def find_ramps(self, img, centre, res):
         # X
         investigate_region = int(np.ceil(5.5 / res[1]).item())
 
         if np.mod(investigate_region, 2) == 0:
             investigate_region = (investigate_region + 1)
 
@@ -91,30 +65,29 @@
 
         # find the points corresponding to the transition between:
         # [0] - background and the hyperintense phantom
         # [1] - hyperintense phantom and hypointense region with ramps
         # [2] - hypointense region with ramps and hyperintense phantom
         # [3] - hyperintense phantom and background
 
-        x_peaks = find_n_peaks(abs_diff_x_profile, 4)
+        x_peaks, _ = self.ACR_obj.find_n_highest_peaks(abs_diff_x_profile, 4)
         x_locs = np.sort(x_peaks) - 1
 
         width_pts = [x_locs[1], x_locs[2]]
         width = np.max(width_pts) - np.min(width_pts)
 
         # take rough estimate of x points for later line profiles
         x = np.round([np.min(width_pts) + 0.2 * width, np.max(width_pts) - 0.2 * width])
-
         # Y
         c = skimage.measure.profile_line(img, (centre[1] - 2 * investigate_region, centre[0]),
                                          (centre[1] + 2 * investigate_region, centre[0]), mode='constant').flatten()
 
         abs_diff_y_profile = np.absolute(np.diff(c))
 
-        y_peaks = find_n_peaks(abs_diff_y_profile, 2)
+        y_peaks, _ = self.ACR_obj.find_n_highest_peaks(abs_diff_y_profile, 2)
         y_locs = centre[1] - 2 * investigate_region + 1 + y_peaks
         height = np.max(y_locs) - np.min(y_locs)
 
         y = np.round([np.max(y_locs) - 0.25 * height, np.min(y_locs) + 0.25 * height])
 
         return x, y
 
@@ -143,32 +116,30 @@
         FWHM_pts = simple_interp(half_max_points[0], data), simple_interp(half_max_points[1], data)
 
         return FWHM_pts
 
     def get_slice_thickness(self, dcm):
         img = dcm.pixel_array
         res = dcm.PixelSpacing  # In-plane resolution from metadata
-        mask, cxy = self.centroid_com(img)
+        cxy = self.ACR_obj.centre
         x_pts, y_pts = self.find_ramps(img, cxy, res)
 
         interp_factor = 5
         sample = np.arange(1, x_pts[1] - x_pts[0] + 2)
         new_sample = np.arange(1, x_pts[1] - x_pts[0] + (1 / interp_factor), (1 / interp_factor))
         offsets = np.arange(-3, 4)
         ramp_length = np.zeros((2, 7))
 
         line_store = []
         fwhm_store = []
         for i, offset in enumerate(offsets):
             lines = [skimage.measure.profile_line(img, (offset + y_pts[0], x_pts[0]), (offset + y_pts[0], x_pts[1]),
-                                                  linewidth=2,
-                                                  mode='constant').flatten(),
+                                                  linewidth=2, mode='constant').flatten(),
                      skimage.measure.profile_line(img, (offset + y_pts[1], x_pts[0]), (offset + y_pts[1], x_pts[1]),
-                                                  linewidth=2,
-                                                  mode='constant').flatten()]
+                                                  linewidth=2, mode='constant').flatten()]
 
             interp_lines = [scipy.interpolate.interp1d(sample, line)(new_sample) for line in lines]
             fwhm = [self.FWHM(interp_line) for interp_line in interp_lines]
             ramp_length[0, i] = (1 / interp_factor) * np.diff(fwhm[0]) * res[0]
             ramp_length[1, i] = (1 / interp_factor) * np.diff(fwhm[1]) * res[0]
 
             line_store.append(interp_lines)
@@ -180,66 +151,68 @@
         dz = dz[~np.isnan(dz)]
         z_ind = np.argmin(np.abs(dcm.SliceThickness - dz))
 
         slice_thickness = dz[z_ind]
 
         if self.report:
             import matplotlib.pyplot as plt
-            fig = plt.figure()
-
-            plt.subplot(2, 2, (1, 3))
-            plt.imshow(img)
-            plt.plot([x_pts[0], x_pts[1]], offsets[z_ind] + [y_pts[0], y_pts[0]], 'b-')
-            plt.plot([x_pts[0], x_pts[1]], offsets[z_ind] + [y_pts[1], y_pts[1]], 'r-')
-            plt.axis('off')
-            plt.title(f'Slice Thickness = {np.round(dz[z_ind], 2)}mm')
-            plt.tight_layout()
+            fig, axes = plt.subplots(4, 1)
+            fig.set_size_inches(8, 24)
+            fig.tight_layout(pad=4)
+
+            axes[0].imshow(img)
+            axes[0].scatter(cxy[0], cxy[1], c='red')
+            axes[0].axis('off')
+            axes[0].set_title('Centroid Location')
+
+            axes[1].imshow(img)
+            axes[1].plot([x_pts[0], x_pts[1]], offsets[z_ind] + [y_pts[0], y_pts[0]], 'b-')
+            axes[1].plot([x_pts[0], x_pts[1]], offsets[z_ind] + [y_pts[1], y_pts[1]], 'r-')
+            axes[1].axis('off')
+            axes[1].set_title('Line Profiles')
 
-            width = fwhm_store[z_ind][1][0] * (1 / interp_factor) * res[0], fwhm_store[z_ind][1][1] * (1 / interp_factor) * \
-                    res[0]
+            width = fwhm_store[z_ind][1][0] * (1 / interp_factor) * res[0], fwhm_store[z_ind][1][1] * (
+                    1 / interp_factor) * res[0]
             x_ramp = new_sample * res[0]
             x_extent = np.max(x_ramp)
             y_ramp = line_store[z_ind][1]
             y_extent = np.max(y_ramp)
             max_loc = np.argmax(y_ramp) * (1 / interp_factor) * res[0]
 
-            plt.subplot(2, 2, 2)
-            plt.plot(x_ramp, y_ramp, 'r', label=f'FWHM={np.round(ramp_length[1][z_ind], 2)}mm')
-            plt.axhline(0.5 * y_extent, xmin=width[0] / x_extent, xmax=width[1] / x_extent, linestyle='dashdot', color='k')
-            plt.axvline(max_loc, ymin=0, ymax=10 / 11, linestyle='dashdot', color='k')
-
-            plt.xlabel('Relative Position (mm)')
-            plt.xlim([0, x_extent])
-            plt.ylim([0, y_extent * 1.1])
-            plt.title('Upper Ramp')
-            plt.grid()
-            plt.legend(loc='best')
-            plt.tight_layout()
+            axes[2].plot(x_ramp, y_ramp, 'r', label=f'FWHM={np.round(ramp_length[1][z_ind], 2)}mm')
+            axes[2].axhline(0.5 * y_extent, xmin=width[0] / x_extent, xmax=width[1] / x_extent, linestyle='dashdot',
+                        color='k')
+            axes[2].axvline(max_loc, ymin=0, ymax=10 / 11, linestyle='dashdot', color='k')
+
+            axes[2].set_xlabel('Relative Position (mm)')
+            axes[2].set_xlim([0, x_extent])
+            axes[2].set_ylim([0, y_extent * 1.1])
+            axes[2].set_title('Upper Ramp')
+            axes[2].grid()
+            axes[2].legend(loc='best')
 
-            width = fwhm_store[z_ind][0][0] * (1 / interp_factor) * res[0], fwhm_store[z_ind][0][1] * (1 / interp_factor) * \
+            width = fwhm_store[z_ind][0][0] * (1 / interp_factor) * res[0], fwhm_store[z_ind][0][1] * (
+                    1 / interp_factor) * \
                     res[0]
             x_ramp = new_sample * res[0]
             x_extent = np.max(x_ramp)
             y_ramp = line_store[z_ind][0]
             y_extent = np.max(y_ramp)
             max_loc = np.argmax(y_ramp) * (1 / interp_factor) * res[0]
 
-            plt.subplot(2, 2, 4)
-            plt.plot(x_ramp, y_ramp, 'b', label=f'FWHM={np.round(ramp_length[0][z_ind], 2)}mm')
-            plt.axhline(0.5 * y_extent, xmin=width[0] / x_extent, xmax=width[1] / x_extent, linestyle='dashdot', color='k')
-            plt.axvline(max_loc, ymin=0, ymax=10 / 11, linestyle='dashdot', color='k')
-
-            plt.xlabel('Relative Position (mm)')
-            plt.xlim([0, x_extent])
-            plt.ylim([0, y_extent * 1.1])
-            plt.title('Lower Ramp')
-            plt.grid()
-            plt.legend(loc='best')
-            plt.tight_layout()
+            axes[3].plot(x_ramp, y_ramp, 'b', label=f'FWHM={np.round(ramp_length[0][z_ind], 2)}mm')
+            axes[3].axhline(0.5 * y_extent, xmin=width[0] / x_extent, xmax=width[1] / x_extent, linestyle='dashdot',
+                        color='k')
+            axes[3].axvline(max_loc, ymin=0, ymax=10 / 11, linestyle='dashdot', color='k')
+
+            axes[3].set_xlabel('Relative Position (mm)')
+            axes[3].set_xlim([0, x_extent])
+            axes[3].set_ylim([0, y_extent * 1.1])
+            axes[3].set_title('Lower Ramp')
+            axes[3].grid()
+            axes[3].legend(loc='best')
 
             img_path = os.path.realpath(os.path.join(self.report_path, f'{self.key(dcm)}_slice_thickness.png'))
             fig.savefig(img_path)
             self.report_files.append(img_path)
 
         return slice_thickness
-
-
```

### Comparing `hazen-1.2.0/hazenlib/tasks/acr_snr.py` & `hazen-1.3.0/hazenlib/tasks/acr_snr.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,96 +12,93 @@
 
 09/01/2023
 """
 
 import sys
 import traceback
 import os
-import hazenlib
+
+import hazenlib.utils
 from hazenlib.HazenTask import HazenTask
 from scipy import ndimage
+
 import numpy as np
 import skimage.morphology
 import pydicom
+from scipy import ndimage
+
+from hazenlib.HazenTask import HazenTask
+from hazenlib.ACRObject import ACRObject
 
 
 class ACRSNR(HazenTask):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
+        self.ACR_obj = None
+
         self.data2 = []
 
     def run(self, measured_slice_width=None, subtract=None) -> dict:
+        
+        if measured_slice_width is not None:
+            measured_slice_width = float(measured_slice_width)
+        
         snr_results = {}
+        self.ACR_obj = [ACRObject(self.data)]
+        snr_dcm = self.ACR_obj[0].dcm[6]
+
         # SINGLE METHOD (SMOOTHING)
         if subtract is None:
-            z = [dcm.ImagePositionPatient[2] for dcm in self.data]
-
-            idx_sort = np.argsort(z)
-            ind = idx_sort[6]
             try:
-                snr, normalised_snr = self.snr_by_smoothing(self.data[ind], measured_slice_width)
-                snr_results[f"snr_smoothing_measured_{self.key(self.data[0])}"] = round(snr, 2)
-                snr_results[f"snr_smoothing_normalised_{self.key(self.data[0])}"] = round(normalised_snr, 2)
+                snr, normalised_snr = self.snr_by_smoothing(snr_dcm, measured_slice_width)
+                snr_results[f"snr_smoothing_measured_{self.key(snr_dcm)}"] = round(snr, 2)
+                snr_results[f"snr_smoothing_normalised_{self.key(snr_dcm)}"] = round(normalised_snr, 2)
             except Exception as e:
-                print(f"Could not calculate the SNR for {self.key(self.data)} because of : {e}")
+                print(f"Could not calculate the SNR for {self.key(snr_dcm)} because of : {e}")
                 traceback.print_exc(file=sys.stdout)
         # SUBTRACTION METHOD
         else:
             temp = [f for f in os.listdir(subtract) if os.path.isfile(os.path.join(subtract, f))]
             filenames = [f'{subtract}/{file}' for file in temp]
 
             self.data2 = [pydicom.dcmread(dicom) for dicom in filenames]
-
-            z = [dcm.ImagePositionPatient[2] for dcm in self.data]
-            z2 = [dcm.ImagePositionPatient[2] for dcm in self.data2]
-
-            idx_sort, idx_sort2 = np.argsort(z), np.argsort(z2)
-            ind, ind2 = idx_sort[6], idx_sort2[6]
+            self.ACR_obj.append(ACRObject(self.data2))
+            snr_dcm2 = self.ACR_obj[1].dcm[6]
             try:
-                snr, normalised_snr = self.snr_by_subtraction(self.data[ind], self.data2[ind2])
-                snr_results[f"snr_subtraction_measured_{self.key(self.data[0])}"] = round(snr, 2)
-                snr_results[f"snr_subtraction_normalised_{self.key(self.data[0])}"] = round(normalised_snr, 2)
+                snr, normalised_snr = self.snr_by_subtraction(snr_dcm, snr_dcm2)
+                snr_results[f"snr_subtraction_measured_{self.key(snr_dcm)}"] = round(snr, 2)
+                snr_results[f"snr_subtraction_normalised_{self.key(snr_dcm)}"] = round(normalised_snr, 2)
             except Exception as e:
-                print(f"Could not calculate the SNR for {self.key(self.data)} and "
-                      f"{self.key(self.data2)} because of : {e}")
+                print(f"Could not calculate the SNR for {self.key(snr_dcm)} and "
+                      f"{self.key(snr_dcm2)} because of : {e}")
                 traceback.print_exc(file=sys.stdout)
 
-        results = {self.key(self.data[0]): snr_results, 'reports': {'images': self.report_files}}
 
-        return results
+        results = {self.key(snr_dcm): snr_results}
 
-    def centroid(self, dcm):
-        img = dcm.pixel_array
-        mask = img > 0.25 * np.max(img)
-        open_img = skimage.morphology.area_opening(mask, area_threshold=500)
-        mask = skimage.morphology.convex_hull_image(open_img)
-
-        coords = np.nonzero(mask)  # row major - first array is columns
-
-        sum_x = np.sum(coords[1])
-        sum_y = np.sum(coords[0])
-        cxy = sum_x / coords[0].shape, sum_y / coords[1].shape
+        # only return reports if requested
+        if self.report:
+            results['reports'] = {'images': self.report_files}
 
-        cxy = [cxy[0].astype(int), cxy[1].astype(int)]
-        return mask, cxy
+        return results
 
     def get_normalised_snr_factor(self, dcm, measured_slice_width=None) -> float:
-        dx, dy = hazenlib.get_pixel_size(dcm)
-        bandwidth = hazenlib.get_bandwidth(dcm)
-        TR = hazenlib.get_TR(dcm)
-        rows = hazenlib.get_rows(dcm)
-        columns = hazenlib.get_columns(dcm)
+        dx, dy = hazenlib.utils.get_pixel_size(dcm)
+        bandwidth = hazenlib.utils.get_bandwidth(dcm)
+        TR = hazenlib.utils.get_TR(dcm)
+        rows = hazenlib.utils.get_rows(dcm)
+        columns = hazenlib.utils.get_columns(dcm)
 
         if measured_slice_width:
             slice_thickness = measured_slice_width
         else:
-            slice_thickness = hazenlib.get_slice_thickness(dcm)
+            slice_thickness = hazenlib.utils.get_slice_thickness(dcm)
 
-        averages = hazenlib.get_average(dcm)
+        averages = hazenlib.utils.get_average(dcm)
         bandwidth_factor = np.sqrt((bandwidth * columns / 2) / 1000) / np.sqrt(30)
         voxel_factor = (1 / (0.001 * dx * dy * slice_thickness))
 
         normalised_snr_factor = bandwidth_factor * voxel_factor * (1 / (np.sqrt(averages * rows * (TR / 1000))))
         return normalised_snr_factor
 
     def filtered_image(self, dcm: pydicom.Dataset) -> np.array:
@@ -115,15 +112,16 @@
 
         returns:
         ---------------
         filtered numpy array
         """
         a = dcm.pixel_array.astype('int')
 
-        # filter size = 9, following MATLAB code and McCann 2013 paper for head coil, although note McCann 2013 recommends 25x25 for body coil.
+        # filter size = 9, following MATLAB code and McCann 2013 paper for head coil, although note McCann 2013
+        # recommends 25x25 for body coil.
         filtered_array = ndimage.uniform_filter(a, 25, mode='constant')
         return filtered_array
 
     def get_noise_image(self, dcm: pydicom.Dataset) -> np.array:
         """
         Separates the image noise by smoothing the image and subtracting the smoothed image
         from the original.
@@ -185,40 +183,43 @@
         measured_slice_width
 
         Returns
         -------
         normalised_snr: float
 
         """
-        _, centre = self.centroid(dcm)
+        centre = self.ACR_obj[0].centre
         col, row = centre
         noise_img = self.get_noise_image(dcm)
 
         signal = [np.mean(roi) for roi in
                   self.get_roi_samples(ax=None, dcm=dcm, centre_col=int(col), centre_row=int(row))]
 
         noise = [np.std(roi, ddof=1) for roi in
                  self.get_roi_samples(ax=None, dcm=noise_img, centre_col=int(col), centre_row=int(row))]
-        # note no root_2 factor in noise for smoothed subtraction (one image) method, replicating Matlab approach and McCann 2013
+        # note no root_2 factor in noise for smoothed subtraction (one image) method, replicating Matlab approach and
+        # McCann 2013
 
         snr = np.mean(np.divide(signal, noise))
 
         normalised_snr = snr * self.get_normalised_snr_factor(dcm, measured_slice_width)
 
         if self.report:
             import matplotlib.pyplot as plt
-            fig, axes = plt.subplots(1, 1)
-            fig.set_size_inches(5, 5)
-            fig.tight_layout(pad=1)
-
-            axes.set_title('smoothed noise image')
-            axes.imshow(noise_img, cmap='gray', label='smoothed noise image')
-            axes.scatter(col, row, 10, marker="+", label='centre')
-            self.get_roi_samples(axes, dcm, int(col), int(row))
-            axes.legend()
+            fig, axes = plt.subplots(2, 1)
+            fig.set_size_inches(8, 16)
+            fig.tight_layout(pad=4)
+
+            axes[0].imshow(dcm.pixel_array)
+            axes[0].scatter(centre[0], centre[1], c='red')
+            axes[0].set_title('Centroid Location')
+
+            axes[1].set_title('Smoothed Noise Image')
+            axes[1].imshow(noise_img, cmap='gray')
+            self.get_roi_samples(axes[1], dcm, int(col), int(row))
 
             img_path = os.path.realpath(os.path.join(self.report_path, f'{self.key(dcm)}_smoothing.png'))
             fig.savefig(img_path)
             self.report_files.append(img_path)
 
         return snr, normalised_snr
 
@@ -231,15 +232,15 @@
         dcm2
         measured_slice_width
 
         Returns
         -------
 
         """
-        _, centre = self.centroid(dcm1)
+        centre = self.ACR_obj[0].centre
         col, row = centre
 
         difference = np.subtract(dcm1.pixel_array.astype('int'), dcm2.pixel_array.astype('int'))
 
         signal = [np.mean(roi) for roi in
                   self.get_roi_samples(ax=None, dcm=dcm1, centre_col=int(col), centre_row=int(row))]
         noise = np.divide(
@@ -248,22 +249,26 @@
             np.sqrt(2))
         snr = np.mean(np.divide(signal, noise))
 
         normalised_snr = snr * self.get_normalised_snr_factor(dcm1, measured_slice_width)
 
         if self.report:
             import matplotlib.pyplot as plt
-            fig, axes = plt.subplots(1, 1)
-            fig.set_size_inches(5, 5)
-            fig.tight_layout(pad=1)
-
-            axes.set_title('difference image')
-            axes.imshow(difference, cmap='gray', label='difference image')
-            axes.scatter(col, row, 10, marker="+", label='centre')
-            self.get_roi_samples(axes, dcm1, int(col), int(row))
-            axes.legend()
+            fig, axes = plt.subplots(2, 1)
+            fig.set_size_inches(8, 16)
+            fig.tight_layout(pad=4)
+
+            axes[0].imshow(dcm1.pixel_array)
+            axes[0].scatter(centre[0], centre[1], c='red')
+            axes[0].axis('off')
+            axes[0].set_title('Centroid Location')
+
+            axes[1].set_title('Difference Image')
+            axes[1].imshow(difference, cmap='gray',)
+            self.get_roi_samples(axes[1], dcm1, int(col), int(row))
+            axes[1].axis('off')
 
             img_path = os.path.realpath(os.path.join(self.report_path, f'{self.key(dcm1)}_snr_subtraction.png'))
             fig.savefig(img_path)
             self.report_files.append(img_path)
 
         return snr, normalised_snr
```

### Comparing `hazen-1.2.0/hazenlib/tasks/acr_spatial_resolution.py` & `hazen-1.3.0/hazenlib/tasks/acr_spatial_resolution.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,88 +40,51 @@
 import cv2
 import os
 import numpy as np
 import skimage.morphology
 import skimage.measure
 
 from hazenlib.HazenTask import HazenTask
-
-
-def find_n_peaks(data, n, height=1):
-    peaks = scipy.signal.find_peaks(data, height)
-    pk_heights = peaks[1]['peak_heights']
-    pk_ind = peaks[0]
-
-    peak_heights = pk_heights[(-pk_heights).argsort()[:n]]
-    peak_locs = pk_ind[(-pk_heights).argsort()[:n]]  # find n highest peaks
-
-    return np.sort(peak_locs), np.sort(peak_heights)
+from hazenlib.ACRObject import ACRObject
+from hazenlib.logger import logger
 
 
 class ACRSpatialResolution(HazenTask):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
+        self.ACR_obj = None
 
     def run(self) -> dict:
         mtf_results = {}
-        z = []
-        for dcm in self.data:
-            z.append(dcm.ImagePositionPatient[2])
-
-        idx_sort = np.argsort(z)
-
-        for dcm in self.data:
-            if dcm.ImagePositionPatient[2] == z[idx_sort[0]]:
-                try:
-                    raw_res, fitted_res = self.get_mtf50(dcm)
-                    mtf_results[f"raw_mtf50_{self.key(self.data[0])}"] = raw_res
-                    mtf_results[f"fitted_mtf50_{self.key(self.data[0])}"] = fitted_res
-                except Exception as e:
-                    print(f"Could not calculate the spatial resolution for {self.key(dcm)} because of : {e}")
-                    traceback.print_exc(file=sys.stdout)
-                    continue
+        self.ACR_obj = ACRObject(self.data)
+        rot_ang = self.ACR_obj.rot_angle
 
-        results = {self.key(self.data[0]): mtf_results, 'reports': {'images': self.report_files}}
-
-        return results
+        if np.round(np.abs(rot_ang), 2) < 3:
+            logger.warning(f'The estimated rotation angle of the ACR phantom is {np.round(rot_ang, 3)} degrees, which '
+                           f'is less than the recommended 3 degrees. Results will be unreliable!')
 
-    def centroid_com(self, dcm):
-        # Calculate centroid of object using a centre-of-mass calculation
-        thresh_img = dcm > 0.25 * np.max(dcm)
-        open_img = skimage.morphology.area_opening(thresh_img, area_threshold=500)
-        bhull = skimage.morphology.convex_hull_image(open_img)
-        coords = np.nonzero(bhull)  # row major - first array is columns
-
-        sum_x = np.sum(coords[1])
-        sum_y = np.sum(coords[0])
-        cx, cy = sum_x / coords[0].shape[0], sum_y / coords[1].shape[0]
-        cxy = (round(cx), round(cy))
-
-        return bhull, cxy
-
-    def find_rotation(self, dcm):
-        thresh = dcm * (dcm > 0.2 * np.max(dcm))
-
-        kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
-        dilate = cv2.morphologyEx(thresh, cv2.MORPH_DILATE, kernel)
-        diff = cv2.absdiff(dilate, thresh)
+        mtf_dcm = self.ACR_obj.dcm[0]
 
-        edges = (diff >= 200) * 1
+        try:
+            raw_res, fitted_res = self.get_mtf50(mtf_dcm)
+            mtf_results[f"estimated_rotation_angle_{self.key(mtf_dcm)}"] = rot_ang
+            mtf_results[f"raw_mtf50_{self.key(mtf_dcm)}"] = raw_res
+            mtf_results[f"fitted_mtf50_{self.key(mtf_dcm)}"] = fitted_res
+        except Exception as e:
+            print(f"Could not calculate the spatial resolution for {self.key(mtf_dcm)} because of : {e}")
+            traceback.print_exc(file=sys.stdout)
 
-        h, theta, d = skimage.transform.hough_line(edges)
-        accum, angles, dists = skimage.transform.hough_line_peaks(h, theta, d)
+        results = {self.key(self.data[0]): mtf_results}
 
-        try:
-            angle = np.rad2deg(scipy.stats.mode(angles)[0][0])
-            rot_angle = angle + 90 if angle < 0 else angle - 90
-        except IndexError:
-            rot_angle = 0
+        # only return reports if requested
+        if self.report:
+            results['reports'] = {'images': self.report_files}
 
-        return rot_angle
+        return results
 
     def y_position_for_ramp(self, res, img, cxy):
         investigate_region = int(np.ceil(5.5 / res[1]).item())
 
         if np.mod(investigate_region, 2) == 0:
             investigate_region = (investigate_region + 1)
 
@@ -148,16 +111,16 @@
 
         return crop_img
 
     def get_edge_type(self, crop_img):
         edge_sum_rows = np.sum(crop_img, axis=1).astype(np.int_)
         edge_sum_cols = np.sum(crop_img, axis=0).astype(np.int_)
 
-        _, pk_rows_height = find_n_peaks(np.abs(np.diff(edge_sum_rows)), 1)
-        _, pk_cols_height = find_n_peaks(np.abs(np.diff(edge_sum_cols)), 1)
+        _, pk_rows_height = self.ACR_obj.find_n_highest_peaks(np.abs(np.diff(edge_sum_rows)), 1)
+        _, pk_cols_height = self.ACR_obj.find_n_highest_peaks(np.abs(np.diff(edge_sum_cols)), 1)
 
         edge_type = 'vertical' if pk_rows_height > pk_cols_height else 'horizontal'
 
         thresh_roi_crop = crop_img > 0.6 * np.max(crop_img)
         edge_dir = np.sum(thresh_roi_crop, axis=0) if edge_type == 'vertical' else np.sum(thresh_roi_crop, axis=1)
         if edge_type == 'vertical':
             direction = 'downward' if edge_dir[-1] > edge_dir[0] else 'upward'
@@ -254,15 +217,15 @@
         weights[turning_points[0]:turning_points[1]] = 1
 
         def func(x, a, b, c, d, e):
             sigmoid = a + b / (1 + np.exp(c * (x - d))) ** e
 
             return sigmoid
 
-        popt, pcov = scipy.optimize.curve_fit(func, np.arange(1, len(erf) + 1), erf, sigma=np.diag(1 / weights),
+        popt, pcov = scipy.optimize.curve_fit(func, np.arange(1, len(erf) + 1), erf, sigma=(1 / weights),
                                               p0=[np.min(erf), np.max(erf), 0, sum(turning_points) / 2, 1], maxfev=5000)
         erf_fit = func(np.arange(1, len(erf) + 1), popt[0], popt[1], popt[2], popt[3], popt[4])
 
         return erf_fit
 
     def calculate_MTF(self, erf, res):
         lsf = np.diff(erf)
@@ -288,22 +251,15 @@
         eff_res = 1 / (equivalent_linepairs * 2)
 
         return eff_res
 
     def get_mtf50(self, dcm):
         img = dcm.pixel_array
         res = dcm.PixelSpacing
-        _, cxy = self.centroid_com(img)
-        rot_ang = self.find_rotation(img)
-
-        if np.round(np.abs(rot_ang), 2) < 3:
-            print(f'Rotation angle of the ACR phantom is {np.round(rot_ang, 3)}, which has an absolute is less than 3 '
-                  f'degree. Results will be unreliable!')
-        else:
-            print(f'Rotation angle of the ACR phantom is {np.round(rot_ang, 3)}')
+        cxy = self.ACR_obj.centre
 
         ramp_x, ramp_y = int(cxy[0]), self.y_position_for_ramp(res, img, cxy)
         width = int(13 * img.shape[0] / 256)
         crop_img = self.crop_image(img, ramp_x, ramp_y, width)
         edge_type, direction = self.get_edge_type(crop_img)
         slope, surface = self.fit_normcdf_surface(crop_img, edge_type, direction)
         erf = self.sample_erf(crop_img, slope, edge_type)
@@ -316,61 +272,57 @@
         eff_fit_res = round(self.identify_MTF50(freq, MTF_fit), 2)
 
         if self.report:
             edge_loc = self.edge_location_for_plot(crop_img, edge_type)
             import matplotlib.pyplot as plt
             import matplotlib.patches as patches
 
-            fig = plt.figure(figsize=(8, 8))
+            fig, axes = plt.subplots(5, 1)
+            fig.set_size_inches(8, 40)
+            fig.tight_layout(pad=4)
 
-            gs = fig.add_gridspec(3, 2)
-            ax0 = fig.add_subplot(gs[:2, 0])
-            ax2 = fig.add_subplot(gs[2:, 0])
-            ax3 = fig.add_subplot(gs[0, 1])
-            ax4 = fig.add_subplot(gs[1, 1])
-            ax5 = fig.add_subplot(gs[2, 1])
-
-            ax0.imshow(img, interpolation='none')
+            axes[0].imshow(img, interpolation='none')
             rect = patches.Rectangle((ramp_x - width // 2 - 1, ramp_y - width // 2 - 1), width, width, linewidth=1,
                                      edgecolor='w', facecolor='none')
-            ax0.add_patch(rect)
-            ax0.axis('off')
+            axes[0].add_patch(rect)
+            axes[0].axis('off')
+            axes[0].set_title('Segmented Edge')
 
-            ax2.imshow(crop_img)
+            axes[1].imshow(crop_img)
             if edge_type == 'vertical':
-                ax2.plot(np.arange(0, width - 1), np.mean(edge_loc) - slope * np.arange(0, width - 1), color='r')
+                axes[1].plot(np.arange(0, width - 1), np.mean(edge_loc) - slope * np.arange(0, width - 1), color='r')
             else:
-                ax2.plot(np.mean(edge_loc) + slope * np.arange(0, width - 1), np.arange(0, width - 1), color='r')
-            ax2.axis('off')
-            ax2.set_title('Cropped Edge', fontsize=14)
-
-            ax3.plot(erf, 'rx', ms=5)
-            ax3.plot(erf_fit, 'k', lw=3)
-            ax3.set_ylabel('Signal Intensity')
-            ax3.set_xlabel('Pixel')
-            ax3.grid()
-            ax3.set_title('ERF', fontsize=14)
-
-            ax4.plot(lsf_raw, 'rx', ms=5)
-            ax4.plot(lsf_fit, 'k', lw=3)
-            ax4.set_ylabel(r'$\Delta$' + ' Signal Intensity')
-            ax4.set_xlabel('Pixel')
-            ax4.grid()
-            ax4.set_title('LSF', fontsize=14)
-
-            ax5.plot(freq, MTF_raw, 'rx', ms=8, label=f'Raw Data - {round(eff_raw_res, 2)}mm @ 50%')
-            ax5.plot(freq, MTF_fit, 'k', lw=3, label=f'Weighted Sigmoid Fit of ERF - {round(eff_fit_res, 2)}mm @ 50%')
-            ax5.set_xlabel('Spatial Frequency (lp/mm)')
-            ax5.set_ylabel('Modulation Transfer Ratio')
-            ax5.set_xlim([-0.05, 1])
-            ax5.set_ylim([0, 1.05])
-            ax5.grid()
-            ax5.legend(fancybox='true', bbox_to_anchor=[1.05, -0.25, 0, 0])
-            ax5.set_title('MTF', fontsize=14)
-
-            plt.tight_layout()
+                axes[1].plot(np.mean(edge_loc) + slope * np.arange(0, width - 1), np.arange(0, width - 1), color='r')
+            axes[1].axis('off')
+            axes[1].set_title('Cropped Edge', fontsize=14)
+
+            axes[2].plot(erf, 'rx', ms=5, label='Raw Data')
+            axes[2].plot(erf_fit, 'k', lw=3, label='Fitted Data')
+            axes[2].set_ylabel('Signal Intensity')
+            axes[2].set_xlabel('Pixel')
+            axes[2].grid()
+            axes[2].legend(fancybox='true')
+            axes[2].set_title('ERF', fontsize=14)
+
+            axes[3].plot(lsf_raw, 'rx', ms=5, label='Raw Data')
+            axes[3].plot(lsf_fit, 'k', lw=3, label='Fitted Data')
+            axes[3].set_ylabel(r'$\Delta$' + ' Signal Intensity')
+            axes[3].set_xlabel('Pixel')
+            axes[3].grid()
+            axes[3].legend(fancybox='true')
+            axes[3].set_title('LSF', fontsize=14)
+
+            axes[4].plot(freq, MTF_raw, 'rx', ms=8, label=f'Raw Data - {round(eff_raw_res, 2)}mm @ 50%')
+            axes[4].plot(freq, MTF_fit, 'k', lw=3, label=f'Weighted Sigmoid Fit of ERF - {round(eff_fit_res, 2)}mm @ 50%')
+            axes[4].set_xlabel('Spatial Frequency (lp/mm)')
+            axes[4].set_ylabel('Modulation Transfer Ratio')
+            axes[4].set_xlim([-0.05, 1])
+            axes[4].set_ylim([0, 1.05])
+            axes[4].grid()
+            axes[4].legend(fancybox='true')
+            axes[4].set_title('MTF', fontsize=14)
 
             img_path = os.path.realpath(os.path.join(self.report_path, f'{self.key(dcm)}.png'))
             fig.savefig(img_path)
             self.report_files.append(img_path)
 
         return eff_raw_res, eff_fit_res
```

### Comparing `hazen-1.2.0/hazenlib/tasks/ghosting.py` & `hazen-1.3.0/hazenlib/tasks/ghosting.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 import traceback
 
 import numpy as np
 import cv2 as cv
 
-import hazenlib
+import hazenlib.utils
 from hazenlib.HazenTask import HazenTask
 
 
 class Ghosting(HazenTask):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
@@ -22,16 +22,19 @@
                 fig, ghosting_results[key] = self.get_ghosting(dcm)
 
             except Exception as e:
                 print(f"Could not calculate the ghosting for {key} because of : {e}")
                 traceback.print_exc(file=sys.stdout)
                 continue
 
-        results = {'ghosting_results': ghosting_results,
-                   'reports': self.report_files}
+        results = {'ghosting_results': ghosting_results}
+
+        # only return reports if requested
+        if self.report:
+            results['reports'] = {'images': self.report_files}
 
         return results
 
     def calculate_ghost_intensity(self, ghost, phantom, noise) -> float:
         """
         Calculates the ghost intensity using the formula from IPEM Report 112
         Ghosting = (Sg-Sn)/(Sp-Sn) x 100%
@@ -192,15 +195,15 @@
         )
         return ghost_slice
 
     def get_ghosting(self, dcm) -> dict:
 
         bbox = self.get_signal_bounding_box(dcm.pixel_array)
 
-        x, y = hazenlib.get_pixel_size(dcm)  # assume square pixels i.e. x=y
+        x, y = hazenlib.utils.get_pixel_size(dcm)  # assume square pixels i.e. x=y
         # ROIs need to be 10mmx10mm
         slice_radius = int(10 // (2 * x))
 
         signal_centre = [(bbox[0] + bbox[1]) // 2, (bbox[2] + bbox[3]) // 2]
         background_rois = self.get_background_rois(dcm, signal_centre)
         ghost_col, ghost_row = self.get_ghost_slice(bbox, dcm, slice_radius=slice_radius)
         ghost = dcm.pixel_array[(ghost_col, ghost_row)]
@@ -219,15 +222,15 @@
             fig, ax = plt.subplots()
             x1, x2, y1, y2 = bbox
 
             img = dcm.pixel_array
             img = img.astype('float64')
             # print('this is img',img)
             img *= 255.0 / img.max()
-            # img = hazenlib.rescale_to_byte(dcm.pixel_array)
+            # img = hazenlib.utils.rescale_to_byte(dcm.pixel_array)
             img = cv.rectangle(img.copy(), (x1, y1), (x2, y2), (255, 0, 0), 1)
 
             for roi in background_rois:
                 #  slice_size = 10
                 x1 = roi[0] - 5
                 y1 = roi[1] - 5
                 x2 = roi[0] + 5
```

### Comparing `hazen-1.2.0/hazenlib/tasks/slice_position.py` & `hazen-1.3.0/hazenlib/tasks/slice_position.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 """
 
 Local Otsu thresholding
 http://scikit-image.org/docs/0.11.x/auto_examples/plot_local_otsu.html
 
 """
 from hazenlib.logger import logger
-import sys
 import os
 import copy
 
-import traceback
-from hazenlib.HazenTask import HazenTask
 import pydicom
 from skimage import measure, filters
 import numpy as np
 import cv2 as cv
 
-import hazenlib
-import hazenlib.tools
+import hazenlib.utils
 import hazenlib.exceptions
+from hazenlib.HazenTask import HazenTask
 
 
 class SlicePosition(HazenTask):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
@@ -41,16 +38,19 @@
             raise
 
         import decimal
         decimal.getcontext().prec = 3
         result = [str(abs(decimal.Decimal(i) * 1)) for i in result]
         del decimal
 
-        results = {self.key(self.data[0]): {'slice_positions': result},
-                   'reports': {'images': self.report_files}}
+        results = {self.key(self.data[0]): {'slice_positions': result}}
+
+        # only return reports if requested
+        if self.report:
+            results['reports'] = {'images': self.report_files}
 
         return results
 
     def get_rod_rotation(self, x_pos: list, y_pos: list) -> float:
         """
         Determine the in-plane rotation i.e. the x-position of the rods should not vary with y-position. If they do it's
         because the phantom is rotated in-plane.
@@ -80,15 +80,15 @@
 
         m, c = np.linalg.lstsq(X, np.array(x_pos), rcond=None)[0]
 
         theta = np.arctan(m)
         return theta
 
     def get_rods_coords(self, dcm: pydicom.Dataset):
-        shape_detector = hazenlib.tools.ShapeDetector(arr=dcm.pixel_array)
+        shape_detector = hazenlib.utils.ShapeDetector(arr=dcm.pixel_array)
         try:
             x, y, r = shape_detector.get_shape('circle')
 
         except hazenlib.exceptions.MultipleShapesError as e:
             # logger.info(f'Warning: found multiple shapes: {list(shape_detector.shapes.keys())}')
             shape_detector.find_contours()
             shape_detector.detect()
@@ -195,15 +195,15 @@
     def slice_position_error(self, data: list):
 
         # get rod positions and nominal positions
         left_rod, right_rod, nominal_positions = self.get_rods(data)
         # Correct for phantom rotation
         left_rod, right_rod = self.correct_rods_for_rotation(left_rod, right_rod)
 
-        fov = hazenlib.get_field_of_view(data[0])
+        fov = hazenlib.utils.get_field_of_view(data[0])
 
         # x_length_mm = np.subtract(right_rod['x_pos'], left_rod['x_pos']) * fov/data[0].Columns
         y_length_mm = np.subtract(left_rod['y_pos'], right_rod['y_pos']) * fov / data[0].Columns
 
         z_length_mm = np.divide(y_length_mm, 2)
 
         if z_length_mm[0] > z_length_mm[-1]:
```

### Comparing `hazen-1.2.0/hazenlib/tasks/slice_width.py` & `hazen-1.3.0/hazenlib/tasks/slice_width.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import scipy.optimize as opt
 from matplotlib import pyplot as plt
 from scipy import ndimage
 from scipy.interpolate import interp1d
 from skimage.measure import regionprops
 
 from hazenlib.HazenTask import HazenTask
-from hazenlib.shapes import Rod
+from hazenlib.utils import Rod
 
 
 class SliceWidth(HazenTask):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
@@ -32,15 +32,17 @@
             try:
                 results[self.key(dcm)] = self.get_slice_width(dcm)
             except Exception as e:
                 print(f"Could not calculate the slice_width for {self.key(dcm)} because of : {e}")
                 traceback.print_exc(file=sys.stdout)
                 continue
 
-        results['reports'] = {'images': self.report_files}
+        # only return reports if requested
+        if self.report:
+            results['reports'] = {'images': self.report_files}
 
         return results
 
     def sort_rods(self, rods):
 
         lower_row = sorted(rods, key=lambda rod: rod.y)[-3:]
         lower_row = sorted(lower_row, key=lambda rod: rod.x)
```

### Comparing `hazen-1.2.0/hazenlib/tasks/snr.py` & `hazen-1.3.0/hazenlib/tasks/snr.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,39 +14,45 @@
 import os
 import cv2 as cv
 import numpy as np
 import pydicom
 import skimage.filters
 from scipy import ndimage
 
-import hazenlib
+import hazenlib.utils
 import hazenlib.exceptions as exc
-import hazenlib.tools
 from hazenlib.HazenTask import HazenTask
 from hazenlib.logger import logger
 
 
 class SNR(HazenTask):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def run(self, measured_slice_width=None) -> dict:
+        if measured_slice_width is not None:
+            measured_slice_width = float(measured_slice_width)
         snr_results = {}
+
         if len(self.data) == 2:
             snr, normalised_snr = self.snr_by_subtraction(self.data[0], self.data[1], measured_slice_width)
             snr_results[f"snr_subtraction_measured_{self.key(self.data[0])}"] = round(snr, 2)
             snr_results[f"snr_subtraction_normalised_{self.key(self.data[0])}"] = round(normalised_snr, 2)
 
         for idx, dcm in enumerate(self.data):
             snr, normalised_snr = self.snr_by_smoothing(dcm, measured_slice_width)
             snr_results[f"snr_smoothing_measured_{self.key(dcm)}"] = round(snr, 2)
             snr_results[f"snr_smoothing_normalised_{self.key(dcm)}"] = round(normalised_snr, 2)
 
-        results = {self.key(self.data[0]): snr_results, 'reports': {'images': self.report_files}}
+        results = {self.key(self.data[0]): snr_results}
+
+        # only return reports if requested
+        if self.report:
+            results['reports'] = {'images': self.report_files}
 
         return results
 
     def two_inputs_match(self, dcm1: pydicom.Dataset, dcm2: pydicom.Dataset) -> bool:
         """
         Checks if two DICOMs are sufficiently similar
 
@@ -80,26 +86,26 @@
 
         Returns
         -------
         normalised snr factor: float
 
         """
 
-        dx, dy = hazenlib.get_pixel_size(dcm)
-        bandwidth = hazenlib.get_bandwidth(dcm)
-        TR = hazenlib.get_TR(dcm)
-        rows = hazenlib.get_rows(dcm)
-        columns = hazenlib.get_columns(dcm)
+        dx, dy = hazenlib.utils.get_pixel_size(dcm)
+        bandwidth = hazenlib.utils.get_bandwidth(dcm)
+        TR = hazenlib.utils.get_TR(dcm)
+        rows = hazenlib.utils.get_rows(dcm)
+        columns = hazenlib.utils.get_columns(dcm)
 
         if measured_slice_width:
             slice_thickness = measured_slice_width
         else:
-            slice_thickness = hazenlib.get_slice_thickness(dcm)
+            slice_thickness = hazenlib.utils.get_slice_thickness(dcm)
 
-        averages = hazenlib.get_average(dcm)
+        averages = hazenlib.utils.get_average(dcm)
         bandwidth_factor = np.sqrt((bandwidth * columns / 2) / 1000) / np.sqrt(30)
         voxel_factor = (1 / (0.001 * dx * dy * slice_thickness))
 
         normalised_snr_factor = bandwidth_factor * voxel_factor * (1 / (np.sqrt(averages * rows * (TR / 1000))))
 
         return normalised_snr_factor
 
@@ -115,15 +121,18 @@
         returns:
         ---------------
         filtered numpy array
         """
         a = dcm.pixel_array.astype('int')
 
         # filter size = 9, following MATLAB code and McCann 2013 paper for head coil, although note McCann 2013 recommends 25x25 for body coil.
-        filtered_array = ndimage.uniform_filter(a, 25, mode='constant')
+        filter_size = 9
+        # 9 for head coil, 25 for body coil
+        # TODO make kernel size optional
+        filtered_array = ndimage.uniform_filter(a, filter_size, mode='constant')
         return filtered_array
 
     def get_noise_image(self, dcm: pydicom.Dataset) -> np.array:
         """
         Separates the image noise by smoothing the image and subtracting the smoothed image
         from the original.
 
@@ -243,16 +252,16 @@
             centre: (col:int, row:int)
 
         """
 
         # Shape Detection
         try:
             logger.debug('Performing phantom shape detection.')
-            shape_detector = hazenlib.tools.ShapeDetector(arr=dcm.pixel_array)
-            orientation = hazenlib.tools.get_image_orientation(dcm.ImageOrientationPatient)
+            shape_detector = hazenlib.utils.ShapeDetector(arr=dcm.pixel_array)
+            orientation = hazenlib.utils.get_image_orientation(dcm.ImageOrientationPatient)
 
             if orientation in ['Sagittal', 'Coronal']:
                 logger.debug('Orientation = sagittal or coronal.')
                 # orientation is sagittal to patient
                 try:
                     (col, row), size, angle = shape_detector.get_shape('rectangle')
                 except exc.ShapeError as e:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hazen-1.2.0/hazenlib/tasks/snr_map.py` & `hazen-1.3.0/hazenlib/tasks/snr_map.py`

 * *Files 2% similar despite different names*

```diff
@@ -257,17 +257,14 @@
         self.roi_distance = 40
 
         # ----
         # * Scale ROI distance to account for different image sizes.
         # * Pass kernel_len and roi_size parameters from command line.
 
         results = {}
-        if self.report:
-            # Create nested report folder and ignore if already exists
-            pathlib.Path.mkdir(pathlib.Path(self.report_path), parents=True, exist_ok=True)
 
         for self.current_dcm in self.data:
 
             key = self.key(self.current_dcm)
 
             #  Create original, smoothed and noise images
             #  ==========================================
```

### Comparing `hazen-1.2.0/hazenlib/tasks/spatial_resolution.py` & `hazen-1.3.0/hazenlib/tasks/spatial_resolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 Spatial Resolution
 
 Contributors:
 Haris Shuaib, haris.shuaib@gstt.nhs.uk
 Neil Heraghty, neil.heraghty@nhs.net, 16/05/2018
 
 .. todo::
-    Replace shape finding functions with hazenlib.tools equivalents
+    Replace shape finding functions with hazenlib.utils equivalents
     
 """
 import copy
 import os
 import sys
 import traceback
 from hazenlib.logger import logger
 
 import cv2 as cv
 import numpy as np
 from numpy.fft import fftfreq
 
-import hazenlib
+import hazenlib.utils
 from hazenlib.HazenTask import HazenTask
 
 
 class SpatialResolution(HazenTask):
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
@@ -34,15 +34,17 @@
             try:
                 results[self.key(dcm)] = self.calculate_mtf(dcm)
             except Exception as e:
                 print(f"Could not calculate the spatial resolution for {self.key(dcm)} because of : {e}")
                 traceback.print_exc(file=sys.stdout)
                 continue
 
-        results['reports'] = {'images': self.report_files}
+        # only return reports if requested
+        if self.report:
+            results['reports'] = {'images': self.report_files}
 
         return results
 
     def deri(self, a):
         # This function calculated the LSF by taking the derivative of the ESF. Reference: https://www.ncbi.nlm.nih.gov/pmc/articles/PMC3643984/
         b = np.gradient(a)
         return b
@@ -294,27 +296,27 @@
 
         return u, esf
 
     def calculate_mtf_for_edge(self, dicom, edge):
         pixels = dicom.pixel_array
         pe = dicom.InPlanePhaseEncodingDirection
 
-        img = hazenlib.rescale_to_byte(pixels)  # rescale for OpenCV operations
+        img = hazenlib.utils.rescale_to_byte(pixels)  # rescale for OpenCV operations
         thresh = self.thresh_image(img)
         circle = self.get_circles(img)
         square, box = self.find_square(thresh)
         if edge == 'right':
             _, centre = self.get_right_edge_vector_and_centre(square)
         else:
             _, centre = self.get_top_edge_vector_and_centre(square)
 
         edge_arr = self.get_edge_roi(pixels, centre)
         void_arr = self.get_void_roi(pixels, circle)
         signal_arr = self.get_signal_roi(pixels, edge, centre, circle)
-        spacing = hazenlib.get_pixel_size(dicom)
+        spacing = hazenlib.utils.get_pixel_size(dicom)
         mean = np.mean([void_arr, signal_arr])
         x_edge, y_edge, edge_arr = self.get_edge(edge_arr, mean, spacing)
         angle, intercept = self.get_edge_angle_and_intercept(x_edge, y_edge)
         x, y = self.get_edge_profile_coords(angle, intercept, spacing)
         u, esf = self.get_esf(edge_arr, y)
         lsf = self.deri(esf)
         lsf = np.array(lsf)
```

### Comparing `hazen-1.2.0/hazenlib/tasks/uniformity.py` & `hazen-1.3.0/hazenlib/tasks/uniformity.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 """
 
 import sys
 import traceback
 import os
 import numpy as np
 
-import hazenlib.tools
+import hazenlib.utils
 import hazenlib.exceptions as exc
 from hazenlib.HazenTask import HazenTask
 
 
 class Uniformity(HazenTask):
 
     def __init__(self, **kwargs):
@@ -42,15 +42,17 @@
             except Exception as e:
                 print(f"Could test not calculate the uniformity for {self.key(dcm)} because of : {e}")
                 traceback.print_exc(file=sys.stdout)
                 continue
 
             results[self.key(dcm)] = result
 
-        results['reports'] = {'images': self.report_files}
+        # only return reports if requested
+        if self.report:
+            results['reports'] = {'images': self.report_files}
 
         return results
 
     def mode(self, a, axis=0):
         """
         Finds the modal value of an array. From scipy.stats.mode
 
@@ -77,16 +79,16 @@
             old_counts = np.maximum(counts, old_counts)
             old_most_frequent = most_frequent
 
         return most_frequent, old_counts
 
     def get_object_centre(self, dcm):
         arr = dcm.pixel_array
-        shape_detector = hazenlib.tools.ShapeDetector(arr=arr)
-        orientation = hazenlib.tools.get_image_orientation(dcm.ImageOrientationPatient)
+        shape_detector = hazenlib.utils.ShapeDetector(arr=arr)
+        orientation = hazenlib.utils.get_image_orientation(dcm.ImageOrientationPatient)
 
         if orientation in ['Sagittal', 'Coronal']:
             # orientation is sagittal to patient
             try:
                 (x, y), size, angle = shape_detector.get_shape('rectangle')
             except exc.ShapeError:
                 raise
@@ -142,9 +144,9 @@
             ax.add_collection(pc)
             ax.scatter(x, y, 5)
 
             img_path = os.path.realpath(os.path.join(self.report_path, f'{self.key(dcm)}.png'))
             fig.savefig(img_path)
             self.report_files.append(img_path)
 
-        return {'horizontal': {'IPEM': fractional_uniformity_horizontal},
-                'vertical': {'IPEM': fractional_uniformity_vertical}}
+        return {'horizontal': fractional_uniformity_horizontal,
+                'vertical': fractional_uniformity_vertical}
```

### Comparing `hazen-1.2.0/setup.cfg` & `hazen-1.3.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -21,13 +21,13 @@
 	scipy==1.8.0
 	imutils==0.5.3
 	colorlog==6.6.0
 include_package_data = True
 
 [options.entry_points]
 console_scripts = 
-	hazen = hazenlib:entry_point
+	hazen = hazenlib:main
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `hazen-1.2.0/tests/test_acr_geometric_accuracy.py` & `hazen-1.3.0/tests/test_acr_geometric_accuracy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,81 +1,78 @@
 import os
 import unittest
 import pathlib
 import pydicom
 import numpy as np
 
 from hazenlib.tasks.acr_geometric_accuracy import ACRGeometricAccuracy
+from hazenlib.ACRObject import ACRObject
 from tests import TEST_DATA_DIR, TEST_REPORT_DIR
 
 
 class TestACRGeometricAccuracySiemens(unittest.TestCase):
     ACR_GEOMETRIC_ACCURACY_DATA = pathlib.Path(TEST_DATA_DIR / 'acr')
-    centre = (128, 129)
-    L1 = 190.43, 186.52
-    L5 = 190.43, 186.52, 189.45, 191.41
-    test_point = (-60.98, -45.62)
+    L1 = 192.38, 188.48
+    L5 = 192.38, 188.48, 190.43, 192.38
 
     def setUp(self):
         self.acr_geometric_accuracy_task = ACRGeometricAccuracy(data_paths=[os.path.join(TEST_DATA_DIR, 'acr')],
                                                                 report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
-        self.dcm = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens', '0.dcm'))
-        self.dcm2 = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens', '4.dcm'))
+        self.acr_geometric_accuracy_task.ACR_obj = ACRObject(
+            [pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens', f'{i}')) for i in
+             os.listdir(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens'))])
 
-    def test_object_centre(self):
-        data = self.dcm.pixel_array
-        assert self.acr_geometric_accuracy_task.centroid_com(data)[1] == self.centre
+        self.dcm_1 = self.acr_geometric_accuracy_task.ACR_obj.dcm[0]
+        self.dcm_5 = self.acr_geometric_accuracy_task.ACR_obj.dcm[4]
 
-    def test_geo_accuracy_slice1(self):
-        slice1_vals = np.array(self.acr_geometric_accuracy_task.get_geometric_accuracy_slice1(self.dcm))
+    def test_geometric_accuracy_slice_1(self):
+        slice1_vals = np.array(self.acr_geometric_accuracy_task.get_geometric_accuracy_slice1(self.dcm_1))
         slice1_vals = np.round(slice1_vals, 2)
 
         print("\ntest_geo_accuracy.py::TestGeoAccuracy::test_geo_accuracy_slice1")
         print("new_release:", slice1_vals)
         print("fixed value:", self.L1)
 
         assert (slice1_vals == self.L1).all() == True
 
-    def test_geo_accuracy_slice5(self):
-        slice5_vals = np.array(self.acr_geometric_accuracy_task.get_geometric_accuracy_slice5(self.dcm2))
+    def test_geometric_accuracy_slice_5(self):
+        slice5_vals = np.array(self.acr_geometric_accuracy_task.get_geometric_accuracy_slice5(self.dcm_5))
         slice5_vals = np.round(slice5_vals, 2)
 
         print("\ntest_geo_accuracy.py::TestGeoAccuracy::test_geo_accuracy_slice1")
         print("new_release:", slice5_vals)
         print("fixed value:", self.L5)
         assert (slice5_vals == self.L5).all() == True
 
-    def test_rotate_point(self):
-        rotated_point = np.array(self.acr_geometric_accuracy_task.rotate_point((0, 0), (30, 70), 150))
-        rotated_point = np.round(rotated_point, 2)
-        print(rotated_point)
-        assert (rotated_point == self.test_point).all() == True
 
-
-# class TestACRUniformityPhilips(unittest.TestCase):
+# TODO: Add unit tests for Philips datasets.
 
 class TestACRGeometricAccuracyGE(unittest.TestCase):
     ACR_GEOMETRIC_ACCURACY_DATA = pathlib.Path(TEST_DATA_DIR / 'acr')
-    L1 = 189.92, 187.89
-    L5 = 189.92, 188.39, 190.43, 189.92
-    distortion_metrics = [-0.59, 2.11, 0.49]
+    L1 = 191.44, 191.44
+    L5 = 191.44, 191.44, 191.44, 189.41
+    distortion_metrics = [1.1, 1.44, 0.4]
 
     def setUp(self):
         self.acr_geometric_accuracy_task = ACRGeometricAccuracy(data_paths=[os.path.join(TEST_DATA_DIR, 'acr')],
                                                                 report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
-        self.dcm = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'GE', '10.dcm'))
-        self.dcm2 = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'GE', '6.dcm'))
+        self.acr_geometric_accuracy_task.ACR_obj = ACRObject(
+            [pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'GE', f'{i}')) for i in
+             os.listdir(os.path.join(TEST_DATA_DIR, 'acr', 'GE'))])
+
+        self.dcm_1 = self.acr_geometric_accuracy_task.ACR_obj.dcm[0]
+        self.dcm_5 = self.acr_geometric_accuracy_task.ACR_obj.dcm[4]
 
     def test_geo_accuracy_slice1(self):
-        slice1_vals = np.array(self.acr_geometric_accuracy_task.get_geometric_accuracy_slice1(self.dcm))
+        slice1_vals = np.array(self.acr_geometric_accuracy_task.get_geometric_accuracy_slice1(self.dcm_1))
         slice1_vals = np.round(slice1_vals, 2)
         assert (slice1_vals == self.L1).all() == True
 
     def test_geo_accuracy_slice5(self):
-        slice5_vals = np.array(self.acr_geometric_accuracy_task.get_geometric_accuracy_slice5(self.dcm2))
+        slice5_vals = np.array(self.acr_geometric_accuracy_task.get_geometric_accuracy_slice5(self.dcm_5))
         slice5_vals = np.round(slice5_vals, 2)
         assert (slice5_vals == self.L5).all() == True
 
     def test_distortion_metrics(self):
-        metrics = np.array(self.acr_geometric_accuracy_task.distortion_metric(self.L1+self.L5))
+        metrics = np.array(self.acr_geometric_accuracy_task.distortion_metric(self.L1 + self.L5))
         metrics = np.round(metrics, 2)
         assert (metrics == self.distortion_metrics).all() == True
```

### Comparing `hazen-1.2.0/tests/test_acr_ghosting.py` & `hazen-1.3.0/tests/test_acr_ghosting.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 import os
 import unittest
 import pathlib
 import pydicom
 
 from hazenlib.tasks.acr_ghosting import ACRGhosting
+from hazenlib.ACRObject import ACRObject
 from tests import TEST_DATA_DIR, TEST_REPORT_DIR
 
 
 class TestACRGhostingSiemens(unittest.TestCase):
     ACR_GHOSTING_DATA = pathlib.Path(TEST_DATA_DIR / 'acr')
     centre = [129, 128]
-    psg = 0.056
+    psg = 0.035
 
     def setUp(self):
         self.acr_ghosting_task = ACRGhosting(data_paths=[os.path.join(TEST_DATA_DIR, 'acr')],
                                              report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
-        self.dcm = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens', '6.dcm'))
 
-    def test_object_centre(self):
-        assert self.acr_ghosting_task.centroid_com(self.dcm.pixel_array)[1] == self.centre
+        self.acr_ghosting_task.ACR_obj = ACRObject(
+            [pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens', f'{i}')) for i in
+             os.listdir(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens'))])
+
+        self.dcm = self.acr_ghosting_task.ACR_obj.dcm[6]
 
     def test_ghosting(self):
         ghosting_val = round(self.acr_ghosting_task.get_signal_ghosting(self.dcm), 3)
 
         print("\ntest_ghosting.py::TestGhosting::test_ghosting")
         print("new_release_value:", ghosting_val)
         print("fixed_value:", self.psg)
 
         assert ghosting_val == self.psg
 
 
 class TestACRGhostingGE(unittest.TestCase):
     ACR_GHOSTING_DATA = pathlib.Path(TEST_DATA_DIR / 'acr')
     centre = [253, 256]
-    psg = 0.487
+    psg = 0.471
 
     def setUp(self):
         self.acr_ghosting_task = ACRGhosting(data_paths=[os.path.join(TEST_DATA_DIR, 'acr')],
                                              report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
-        self.dcm = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'GE', '4.dcm'))
+        self.acr_ghosting_task.ACR_obj = ACRObject(
+            [pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'GE', f'{i}')) for i in
+             os.listdir(os.path.join(TEST_DATA_DIR, 'acr', 'GE'))])
 
-    def test_object_centre(self):
-        assert self.acr_ghosting_task.centroid_com(self.dcm.pixel_array)[1] == self.centre
+        self.dcm = self.acr_ghosting_task.ACR_obj.dcm[6]
 
     def test_ghosting(self):
         assert round(self.acr_ghosting_task.get_signal_ghosting(self.dcm), 3) == self.psg
```

### Comparing `hazen-1.2.0/tests/test_acr_slice_thickness.py` & `hazen-1.3.0/tests/test_acr_slice_thickness.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import os
 import unittest
 import pathlib
 import pydicom
 
 from hazenlib.tasks.acr_slice_thickness import ACRSliceThickness
+from hazenlib.ACRObject import ACRObject
 from tests import TEST_DATA_DIR
 
 
 class TestACRSliceThicknessSiemens(unittest.TestCase):
     ACR_SLICE_POSITION_DATA = pathlib.Path(TEST_DATA_DIR / 'acr')
-    centre = [128, 129]
     x_pts = [71, 181]
     y_pts = [132, 126]
     dz = 4.91
 
     def setUp(self):
         self.acr_slice_thickness_task = ACRSliceThickness(data_paths=[os.path.join(TEST_DATA_DIR, 'acr')])
-        self.dcm = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens', '0.dcm'))
+        self.acr_slice_thickness_task.ACR_obj = ACRObject(
+            [pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens', f'{i}')) for i in
+             os.listdir(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens'))])
 
-    def test_object_centre(self):
-        assert self.acr_slice_thickness_task.centroid_com(self.dcm.pixel_array)[1] == self.centre
+        self.dcm = self.acr_slice_thickness_task.ACR_obj.dcm[0]
 
     def test_ramp_find(self):
         res = self.dcm.PixelSpacing
-        _, centre = self.acr_slice_thickness_task.centroid_com(self.dcm.pixel_array)
+        centre = self.acr_slice_thickness_task.ACR_obj.centre
         assert (self.acr_slice_thickness_task.find_ramps(self.dcm.pixel_array, centre, res)[0] ==
                 self.x_pts).all() == True
 
         assert (self.acr_slice_thickness_task.find_ramps(self.dcm.pixel_array, centre, res)[1] ==
                 self.y_pts).all() == True
 
     def test_slice_thickness(self):
@@ -38,30 +39,29 @@
         print("fixed_value:", self.dz)
 
         assert slice_thickness_val == self.dz
 
 
 class TestACRSliceThicknessGE(unittest.TestCase):
     ACR_SLICE_POSITION_DATA = pathlib.Path(TEST_DATA_DIR / 'acr')
-    centre = [253, 255]
     x_pts = [146, 356]
     y_pts = [262, 250]
     dz = 5.02
 
     def setUp(self):
         self.acr_slice_thickness_task = ACRSliceThickness(data_paths=[os.path.join(TEST_DATA_DIR, 'acr')])
-        self.dcm = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'GE', '10.dcm'))
+        self.acr_slice_thickness_task.ACR_obj = ACRObject(
+            [pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'GE', f'{i}')) for i in
+             os.listdir(os.path.join(TEST_DATA_DIR, 'acr', 'GE'))])
 
-    def test_object_centre(self):
-        assert self.acr_slice_thickness_task.centroid_com(self.dcm.pixel_array)[1] == self.centre
+        self.dcm = self.acr_slice_thickness_task.ACR_obj.dcm[0]
 
     def test_ramp_find(self):
         res = self.dcm.PixelSpacing
-        _, centre = self.acr_slice_thickness_task.centroid_com(self.dcm.pixel_array)
+        centre = self.acr_slice_thickness_task.ACR_obj.centre
         assert (self.acr_slice_thickness_task.find_ramps(self.dcm.pixel_array, centre, res)[0] ==
                 self.x_pts).all() == True
-
         assert (self.acr_slice_thickness_task.find_ramps(self.dcm.pixel_array, centre, res)[1] ==
                 self.y_pts).all() == True
 
     def test_slice_thickness(self):
         assert round(self.acr_slice_thickness_task.get_slice_thickness(self.dcm), 2) == self.dz
```

### Comparing `hazen-1.2.0/tests/test_acr_snr.py` & `hazen-1.3.0/tests/test_acr_snr.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,67 @@
 import os
 import unittest
 import pathlib
 import pydicom
 
 from hazenlib.tasks.acr_snr import ACRSNR
+from hazenlib.ACRObject import ACRObject
 from tests import TEST_DATA_DIR, TEST_REPORT_DIR
 
 
 class TestACRSNRSiemens(unittest.TestCase):
     ACR_SNR_DATA = pathlib.Path(TEST_DATA_DIR / 'acr')
-    centre = [129, 128]
     norm_factor = 9.761711312090041
-    snr = 335.27
-    sub_snr = 76.48
+    snr = 344.15
+    sub_snr = 75.94
 
     def setUp(self):
         self.acr_snr_task = ACRSNR(data_paths=[os.path.join(TEST_DATA_DIR, 'acr')],
                                    report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
-        self.dcm = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens', '6.dcm'))
-        self.dcm2 = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens2', '7.dcm'))
+        self.acr_snr_task.ACR_obj = [ACRObject(
+            [pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens', f'{i}')) for i in
+             os.listdir(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens'))])]
+        self.acr_snr_task.ACR_obj.append(
+            ACRObject([pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens2', f'{i}')) for i in
+                       os.listdir(os.path.join(TEST_DATA_DIR, 'acr', 'Siemens2'))]))
 
-    def test_object_centre(self):
-        assert self.acr_snr_task.centroid(self.dcm)[1] == self.centre
+        self.dcm = [i.dcm[6] for i in self.acr_snr_task.ACR_obj]
 
     def test_normalisation_factor(self):
-        SNR_factor = self.acr_snr_task.get_normalised_snr_factor(self.dcm)
+        SNR_factor = self.acr_snr_task.get_normalised_snr_factor(self.dcm[0])
         assert SNR_factor == self.norm_factor
 
     def test_snr_by_smoothing(self):
-        snr, _ = self.acr_snr_task.snr_by_smoothing(self.dcm)
+        snr, _ = self.acr_snr_task.snr_by_smoothing(self.dcm[0])
         assert round(snr, 2) == self.snr
 
     def test_snr_by_subtraction(self):
-        snr, _ = self.acr_snr_task.snr_by_subtraction(self.dcm, self.dcm2)
+        snr, _ = self.acr_snr_task.snr_by_subtraction(self.dcm[0], self.dcm[1])
         rounded_snr = round(snr, 2)
 
         print("\ntest_snr_by_subtraction.py::TestSnrBySubtraction::test_snr_by_subtraction")
         print("new_release_value:", rounded_snr)
         print("fixed_value:", self.sub_snr)
 
         assert rounded_snr == self.sub_snr
 
 
 class TestACRSNRGE(unittest.TestCase):
     ACR_SNR_DATA = pathlib.Path(TEST_DATA_DIR / 'acr')
-    centre = [253, 256]
     norm_factor = 57.12810400630368
-    snr = 39.97
+    snr = 40.19
 
     def setUp(self):
         self.acr_snr_task = ACRSNR(data_paths=[os.path.join(TEST_DATA_DIR, 'acr')],
                                    report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
-        self.dcm = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'GE', '4.dcm'))
+        self.acr_snr_task.ACR_obj = [ACRObject(
+            [pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'GE', f'{i}')) for i in
+             os.listdir(os.path.join(TEST_DATA_DIR, 'acr', 'GE'))])]
 
-    def test_object_centre(self):
-        assert self.acr_snr_task.centroid(self.dcm)[1] == self.centre
+        self.dcm = self.acr_snr_task.ACR_obj[0].dcm[6]
 
     def test_normalisation_factor(self):
         SNR_factor = self.acr_snr_task.get_normalised_snr_factor(self.dcm)
         assert SNR_factor == self.norm_factor
 
     def test_snr_by_smoothing(self):
         snr, _ = self.acr_snr_task.snr_by_smoothing(self.dcm)
```

### Comparing `hazen-1.2.0/tests/test_acr_spatial_resolution.py` & `hazen-1.3.0/tests/test_acr_spatial_resolution.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 import os
 import unittest
 import pathlib
 import pydicom
 import numpy as np
 
 from hazenlib.tasks.acr_spatial_resolution import ACRSpatialResolution
+from hazenlib.ACRObject import ACRObject
 from tests import TEST_DATA_DIR, TEST_REPORT_DIR
 
 
 class TestACRSpatialResolutionSiemens(unittest.TestCase):
     ACR_SPATIAL_RESOLUTION_DATA = pathlib.Path(TEST_DATA_DIR / 'acr')
     centre = (128, 124)
     rotation_angle = 9
     y_ramp_pos = 118
     width = 13
     edge_type = 'vertical', 'downward'
     edge_loc = [5, 7]
     slope = -0.165
-    MTF50 = (1.16, 1.32)
+    MTF50 = (1.18, 1.35)
 
     def setUp(self):
         self.acr_spatial_resolution_task = ACRSpatialResolution(data_paths=[os.path.join(TEST_DATA_DIR, 'acr')],
                                                                 report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
-        self.dcm = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'SiemensMTF', '0.dcm'))
+        self.acr_spatial_resolution_task.ACR_obj = ACRObject(
+            [pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'SiemensMTF', f'{i}')) for i in
+             os.listdir(os.path.join(TEST_DATA_DIR, 'acr', 'SiemensMTF'))])
+
+        self.dcm = self.acr_spatial_resolution_task.ACR_obj.dcm[0]
         self.crop_image = self.acr_spatial_resolution_task.crop_image(self.dcm.pixel_array, self.centre[0],
                                                                       self.y_ramp_pos, self.width)
 
-    def test_object_centre(self):
-        data = self.dcm.pixel_array
-        assert self.acr_spatial_resolution_task.centroid_com(data)[1] == self.centre
-
-    def test_rotation(self):
-        data = self.dcm.pixel_array
-        assert self.acr_spatial_resolution_task.find_rotation(data) == self.rotation_angle
-
     def test_find_y_ramp(self):
         data = self.dcm.pixel_array
         res = self.dcm.PixelSpacing
         assert self.acr_spatial_resolution_task.y_position_for_ramp(res, data, self.centre) == self.y_ramp_pos
 
     def test_get_edge_type(self):
         assert self.acr_spatial_resolution_task.get_edge_type(self.crop_image) == self.edge_type
@@ -64,31 +61,27 @@
     centre = (254, 255)
     rotation_angle = 0
     y_ramp_pos = 244
     width = 26
     edge_type = 'vertical', 'upward'
     edge_loc = [5, 7]
     slope = 0.037
-    MTF50 = (0.71, 0.69)
+    MTF50 = (0.72, 0.71)
 
     def setUp(self):
         self.acr_spatial_resolution_task = ACRSpatialResolution(data_paths=[os.path.join(TEST_DATA_DIR, 'acr')],
                                                                 report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
-        self.dcm = pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'GE', '10.dcm'))
+        self.acr_spatial_resolution_task.ACR_obj = ACRObject(
+            [pydicom.read_file(os.path.join(TEST_DATA_DIR, 'acr', 'GE', f'{i}')) for i in
+             os.listdir(os.path.join(TEST_DATA_DIR, 'acr', 'GE'))])
+
+        self.dcm = self.acr_spatial_resolution_task.ACR_obj.dcm[0]
         self.crop_image = self.acr_spatial_resolution_task.crop_image(self.dcm.pixel_array, self.centre[0],
                                                                       self.y_ramp_pos, self.width)
 
-    def test_object_centre(self):
-        data = self.dcm.pixel_array
-        assert self.acr_spatial_resolution_task.centroid_com(data)[1] == self.centre
-
-    def test_rotation(self):
-        data = self.dcm.pixel_array
-        assert self.acr_spatial_resolution_task.find_rotation(data) == self.rotation_angle
-
     def test_find_y_ramp(self):
         data = self.dcm.pixel_array
         res = self.dcm.PixelSpacing
         assert self.acr_spatial_resolution_task.y_position_for_ramp(res, data, self.centre) == self.y_ramp_pos
 
     def test_get_edge_type(self):
         assert self.acr_spatial_resolution_task.get_edge_type(self.crop_image) == self.edge_type
```

### Comparing `hazen-1.2.0/tests/test_ghosting.py` & `hazen-1.3.0/tests/test_ghosting.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import pydicom
 import pytest
 import os
 import pathlib
 from tests import TEST_DATA_DIR, TEST_REPORT_DIR
 from hazenlib.tasks.ghosting import Ghosting
-from hazenlib.tools import get_dicom_files
+from hazenlib.utils import get_dicom_files
 
 
 class TestGhosting(unittest.TestCase):
     SIGNAL_BOUNDING_BOX = (252, 334, 243, 325)
     SIGNAL_CENTRE = [293, 284]
     BACKGROUND_ROIS = [(293, 88), (220, 88), (147, 88), (74, 88)]
     PADDING_FROM_BOX = 30
@@ -106,15 +106,15 @@
         self.dcm = pydicom.read_file(
             os.path.join(TEST_DATA_DIR, 'ghosting', 'PE_COL_PHANTOM_BOTTOM_RIGHT', 'PE_COL_PHANTOM_BOTTOM_RIGHT.IMA'))
         self.ghosting = Ghosting(
             data_paths=get_dicom_files(os.path.join(TEST_DATA_DIR, 'ghosting', 'PE_COL_PHANTOM_BOTTOM_RIGHT')),
             report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
 
 
-class TestAxialPhilipsBroomfields(TestGhosting):
+class TestAxialPhilipsGhosting(TestGhosting):
     SIGNAL_BOUNDING_BOX = (217, 299, 11, 93)
     SIGNAL_CENTRE = [(SIGNAL_BOUNDING_BOX[0] + SIGNAL_BOUNDING_BOX[1]) // 2,
                      (SIGNAL_BOUNDING_BOX[2] + SIGNAL_BOUNDING_BOX[3]) // 2]
     BACKGROUND_ROIS = [(258, 264), (194, 264), (130, 264), (66, 264)]
     PADDING_FROM_BOX = 30
     SLICE_RADIUS = 5
     ELIGIBLE_GHOST_AREA = range(SLICE_RADIUS, SIGNAL_BOUNDING_BOX[0] - PADDING_FROM_BOX), range(
@@ -126,10 +126,10 @@
         range(min(ELIGIBLE_GHOST_AREA[1]), max(ELIGIBLE_GHOST_AREA[1])), dtype=np.intp)[:, np.newaxis], np.array(
         range(min(ELIGIBLE_GHOST_AREA[0]), max(ELIGIBLE_GHOST_AREA[0])))
 
     GHOSTING = (None, 0.007246960909896829)
 
     def setUp(self):
         self.dcm = pydicom.read_file(
-            os.path.join(TEST_DATA_DIR, 'ghosting', 'GHOSTING', 'axial_philips_broomfields.dcm'))
+            os.path.join(TEST_DATA_DIR, 'ghosting', 'GHOSTING', 'axial_philips_ghosting.dcm'))
         self.ghosting = Ghosting(data_paths=get_dicom_files(os.path.join(TEST_DATA_DIR, 'ghosting', 'GHOSTING')),
                                  report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
```

### Comparing `hazen-1.2.0/tests/test_relaxometry.py` & `hazen-1.3.0/tests/test_relaxometry.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 import unittest
 import pydicom
 import numpy as np
 import os
 import os.path
 from pydicom.errors import InvalidDicomError
 
-import hazenlib.relaxometry as hazen_relaxometry
+from hazenlib.tasks.relaxometry import (
+    transform_coords, T1ImageStack, T2ImageStack, Relaxometry)
+from hazenlib.utils import get_dicom_files
 from hazenlib.exceptions import ArgumentCombinationError
 from tests import TEST_DATA_DIR, TEST_REPORT_DIR
+from hazenlib.relaxometry_params import TEMPLATE_VALUES
 
 
 class TestRelaxometry(unittest.TestCase):
     # test parameters here
 
     # Values for transform_coords tests
     TEST_COORDS = [[0, 0], [0, 1], [1, 2]]
@@ -87,17 +90,17 @@
     ROI_TEMPLATE_MEANS_T0 = [-683.840, -819.28, -1019.84]
 
     # Values from IDL routine
     PLATE5_T1 = [1862.6, 1435.8, 999.9, 740.7, 498.2, 351.6, 255.2, 178.0,
                  131.7, 93.3, 66.6, 45.1, 32.5, 22.4, 2632]
 
     # Values from testing (to check for variations)
-    PLATE4_T2 = [816.633328, 590.521423, 430.902617, 310.985158, 217.258533,
-                 156.093083, 109.839424, 79.269721, 55.998743, 39.044842,
-                 27.143183, 18.448322, 12.514836, 9.351455, 2376]
+    PLATE4_T2 = [ 816.33093, 590.26915, 430.69191, 310.801929, 216.998622,
+                  155.68107, 109.346141, 78.967168, 55.986545, 39.080988,
+                  27.59972,   18.389453, 12.336855, 8.035046, 2374.533555]
 
     TEMPLATE_PATH_T2 = os.path.join(TEST_DATA_DIR, 'relaxometry', 'T2',
                                     'Template_plate4_T2')
 
     TEMPLATE_P4_TEST_COORDS_ROW_COL = [[56, 95], [62, 117], [81, 133],
                                        [104, 134], [124, 121], [133, 98],
                                        [127, 75], [109, 61], [84, 60],
@@ -195,15 +198,15 @@
     SITE3_T2_P5_VALS = [1878.80, 1227.30, 790.39, 582.16, 419.24, 298.09, 216.68,
                         154.16, 114.25, 80.52, 57.17, 39.56, 28.10, 19.72, 3456]
     SITE3_T2_P5_DIR = os.path.join(TEST_DATA_DIR, 'relaxometry', 'T2',
                                    'site3_ge', 'plate5')
     SITE3_T2_P5_FILES = ['Z812', 'Z813', 'Z814', 'Z819', 'Z823', 'Z825', 'Z830',
                          'Z834']
 
-    # Site 5 tests - Philisp 3T
+    # Site 5 tests - Philips 3T
     SITE5_T1_P4_DIR = os.path.join(TEST_DATA_DIR, 'relaxometry', 'T1',
                                    'site5_philips_3T', 'plate4')
 
     SITE5_T1_P4_FILES = ['IM_0086', 'IM_0038', 'IM_0054', 'IM_0070', 'IM_0599',
                          'IM_0485']
 
     SITE5_T1_P4 = [2156.1, 2013.6, 1866.8, 1573.8, 1479.4, 1031.9, 799.8,
@@ -245,399 +248,392 @@
 
     SITE5_T2_P5 = [1591.4, 1119.2, 742.7, 524.5, 370.7, 256.0, 180.5, 125.9,
                    91.2, 64.4, 45.2, 30.8, 22.0, 15.4, 2706.2]
 
     def test_transform_coords(self):
         # no translation, no rotation, input = yx, output = yx
         warp_matrix = np.array([[1, 0, 0], [0, 1, 0]])
-        op = hazen_relaxometry.transform_coords(self.TEST_COORDS,
+        op = transform_coords(self.TEST_COORDS,
                                                 warp_matrix,
                                                 input_row_col=True,
                                                 output_row_col=True)
         np.testing.assert_allclose(op, self.TEST_COORDS)
         # 'Identity coordinate transformation row_col (yx) -> row_col (yx)' 
         # ' failed'
 
         # no translation, no rotation, flip
         # input = col_row (xy), output = row_col (yx)
-        op = hazen_relaxometry.transform_coords(self.TEST_COORDS, warp_matrix,
+        op = transform_coords(self.TEST_COORDS, warp_matrix,
                                                 input_row_col=False,
                                                 output_row_col=True)
 
         np.testing.assert_allclose(op, self.COORDS_FLIP)
 
         # no translation, no rotation, input = col_row (xy), 
         # output = col_row (xy)
-        op = hazen_relaxometry.transform_coords(self.TEST_COORDS, warp_matrix,
+        op = transform_coords(self.TEST_COORDS, warp_matrix,
                                                 input_row_col=False,
                                                 output_row_col=False)
         np.testing.assert_allclose(op, self.TEST_COORDS)
         # 'Identity coordinate transformation XY -> XY failed'
 
         # translation x=1, y=3, no rotation, input = row_col (yx),
         # output = row_col (yx)
         warp_matrix = np.array([[1, 0, 1], [0, 1, 3]])
-        op = hazen_relaxometry.transform_coords(self.TEST_COORDS, warp_matrix,
+        op = transform_coords(self.TEST_COORDS, warp_matrix,
                                                 input_row_col=True,
                                                 output_row_col=True)
         np.testing.assert_allclose(op, self.COORDS_TRANS)
         # 'Translation coordinate transformation YX -> YX failed'
 
         # translation x=1, y=3, no rotation, input = col_row (xy),
         # output = row_col (yx)
         warp_matrix = np.array([[1, 0, 1], [0, 1, 3]])
-        op = hazen_relaxometry.transform_coords(self.TEST_COORDS, warp_matrix,
+        op = transform_coords(self.TEST_COORDS, warp_matrix,
                                                 input_row_col=False,
                                                 output_row_col=True)
         np.testing.assert_allclose(op, self.COORDS_TRANS_FLIP)
         # 'Translation coordinate transformation XY -> YX failed'
 
         # translation x=1, y=3, no rotation, input = col_row (xy),
         # output = col_row (xy)
         warp_matrix = np.array([[1, 0, 1], [0, 1, 3]])
-        op = hazen_relaxometry.transform_coords(self.TEST_COORDS, warp_matrix,
+        op = transform_coords(self.TEST_COORDS, warp_matrix,
                                                 input_row_col=False,
                                                 output_row_col=False)
         np.testing.assert_allclose(op, self.COORDS_TRANS_COL_ROW)
         # 'Translation coordinate transformation XY -> XY failed'
 
         # rotation (-30) degrees, translation col=10, row=20,
         # input = col_row (xy), output = col_row (xy)
         warp_matrix = np.array([[np.sqrt(3) / 2, 0.5, 10],
                                 [-0.5, np.sqrt(3) / 2, 20]])
         # use float64 rather than int32 for coordinates to better test rotation
-        op = hazen_relaxometry.transform_coords(np.array(self.TEST_COORDS,
+        op = transform_coords(np.array(self.TEST_COORDS,
                                                          dtype=np.float64),
                                                 warp_matrix,
                                                 input_row_col=False,
                                                 output_row_col=False)
         np.testing.assert_allclose(op, self.COORDS_TRANS_ROTATE)
 
     def test_template_fit(self):
         template_dcm = pydicom.read_file(self.TEMPLATE_PATH_T1_P5)
 
         target_dcm = pydicom.dcmread(self.TEMPLATE_TARGET_PATH_T1_P5)
-        t1_image_stack = hazen_relaxometry.T1ImageStack([target_dcm],
-                                                        template_dcm,
-                                                        plate_number=5)
-        t1_image_stack.template_fit()
+        t1_image_stack = T1ImageStack([target_dcm])
+        warp_matrix = t1_image_stack.template_fit(template_dcm)
 
-        transformed_coordinates_xy = hazen_relaxometry.transform_coords(
-            self.TEMPLATE_TEST_COORDS_ROW_COL, t1_image_stack.warp_matrix,
+        transformed_coordinates_xy = transform_coords(
+            self.TEMPLATE_TEST_COORDS_ROW_COL, warp_matrix,
             input_row_col=True, output_row_col=False)
 
         # test to within +/- 1 pixel (also checks YX-XY change)
         np.testing.assert_allclose(
             transformed_coordinates_xy, self.TEMPLATE_TARGET_COORDS_COL_ROW,
             atol=1)
 
     def test_image_stack_T1_sort(self):
         # read list of un-ordered T1 files, sort by TI, test sorted
         t1_dcms = [pydicom.dcmread(os.path.join(self.T1_DIR, fname))
                    for fname in self.T1_FILES]
-        t1_image_stack = hazen_relaxometry.T1ImageStack(t1_dcms)
+        t1_image_stack = T1ImageStack(t1_dcms)
         sorted_output = [image.InversionTime.real for image in
                          t1_image_stack.images]
         assert sorted_output == self.T1_TI_SORTED
 
     def test_image_stack_T2_sort(self):
         # read list of un-ordered T2 files, sort by TE, test sorted
         t2_dcms = [pydicom.dcmread(os.path.join(self.T2_DIR, fname))
                    for fname in self.T2_FILES]
-        t2_image_stack = hazen_relaxometry.T2ImageStack(t2_dcms)
+        t2_image_stack = T2ImageStack(t2_dcms)
 
         sorted_output = [image.EchoTime.real for image in
                          t2_image_stack.images]
 
         assert sorted_output == self.T2_TE_SORTED
 
     def test_generate_time_series_template_POIs(self):
         # Test on template first, no image fitting needed
         # Need image to get correct size
         template_dcm = pydicom.dcmread(self.TEMPLATE_PATH_T1_P5)
-        template_image_stack = hazen_relaxometry.T1ImageStack([template_dcm])
+        template_image_stack = T1ImageStack([template_dcm])
+        warp_matrix = template_image_stack.template_fit(template_dcm)
         template_image_stack.generate_time_series(
             self.TEMPLATE_TEST_COORDS_ROW_COL,
-            fit_coords=False)
+            warp_matrix=warp_matrix, fit_coords=False)
 
         for i in range(np.size(self.MASK_POI_TEMPLATE, 0)):
             np.testing.assert_equal(
                 template_image_stack.ROI_time_series[i].POI_mask,
                 self.MASK_POI_TEMPLATE[i])
 
     def test_generate_time_series_target_POIs(self):
         # Test on target and check image fitting too.
         template_dcm = pydicom.read_file(self.TEMPLATE_PATH_T1_P5)
 
         target_dcm = pydicom.dcmread(self.TEMPLATE_TARGET_PATH_T1_P5)
-        target_image_stack = hazen_relaxometry.T1ImageStack([target_dcm],
-                                                            template_dcm)
-        target_image_stack.template_fit()
-        # transformed_coordinates_yx = hazen_relaxometry.transform_coords(
+        target_image_stack = T1ImageStack([target_dcm])
+        warp_matrix = target_image_stack.template_fit(template_dcm)
+        # transformed_coordinates_yx = transform_coords(
         #     self.TEMPLATE_TEST_COORDS_YX, target_image_stack.warp_matrix,
         #     input_yx=True, output_yx=True)
         target_image_stack.generate_time_series(
-            self.TEMPLATE_TEST_COORDS_ROW_COL, fit_coords=True)
+            self.TEMPLATE_TEST_COORDS_ROW_COL,
+            warp_matrix=warp_matrix)
         for i in range(np.size(self.MASK_POI_TARGET, 0)):
             np.testing.assert_equal(
                 target_image_stack.ROI_time_series[i].POI_mask,
                 self.MASK_POI_TARGET[i])
 
     def test_extract_single_roi(self):
         # Test that ROI pixel value extraction works. Use template DICOM for
         # both template and image to avoid errors due to slight variation in
         # fitting.
         template_dcm = pydicom.read_file(self.TEMPLATE_PATH_T1_P5)
 
-        template_image_stack = hazen_relaxometry.T1ImageStack([template_dcm],
-                                                              template_dcm)
+        template_image_stack = T1ImageStack([template_dcm])
         # set warp_matrix to identity matrix
         # template_image_stack.warp_matrix = np.eye(2, 3, dtype=np.float32)
+        warp_matrix = template_image_stack.template_fit(template_dcm)
         template_image_stack.generate_time_series(
-            self.TEMPLATE_TEST_COORDS_ROW_COL, fit_coords=False)
+            self.TEMPLATE_TEST_COORDS_ROW_COL,
+            warp_matrix=warp_matrix, fit_coords=False)
 
         np.testing.assert_equal(
             template_image_stack.ROI_time_series[0].pixel_values[0],
             self.ROI0_TEMPLATE_PIXELS)
 
     def test_template_roi_means(self):
         # Check mean of first 3 ROIs in template match with ImageJ calculations
         template_dcm = pydicom.read_file(self.TEMPLATE_PATH_T1_P5)
 
-        template_image_stack = hazen_relaxometry.T1ImageStack([template_dcm],
-                                                              template_dcm)
+        template_image_stack = T1ImageStack([template_dcm])
 
+        warp_matrix = template_image_stack.template_fit(template_dcm)
         template_image_stack.generate_time_series(
-            self.TEMPLATE_TEST_COORDS_ROW_COL, fit_coords=False)
+            self.TEMPLATE_TEST_COORDS_ROW_COL,
+            warp_matrix=warp_matrix, fit_coords=False)
 
         # Check all pixels in ROI[0] match
         np.testing.assert_allclose(
             template_image_stack.ROI_time_series[0].pixel_values[0],
             self.ROI0_TEMPLATE_PIXELS)
 
         # Check mean ROI for first three ROIs are correct
         for i in range(len(self.ROI_TEMPLATE_MEANS_T0)):
-            self.assertAlmostEquals(
+            self.assertAlmostEqual(
                 np.mean(template_image_stack.ROI_time_series[i].pixel_values),
                 self.ROI_TEMPLATE_MEANS_T0[i])
 
     def test_t1_calc_magnitude_image(self):
         """Test T1 value for plate 5 spheres."""
         template_dcm = pydicom.read_file(self.TEMPLATE_PATH_T1_P5)
         t1_dcms = [pydicom.dcmread(os.path.join(self.T1_DIR, fname))
                    for fname in self.T1_FILES]
-        t1_image_stack = hazen_relaxometry.T1ImageStack(t1_dcms, template_dcm)
-        t1_image_stack.template_fit()
+        t1_image_stack = T1ImageStack(t1_dcms)
+        warp_matrix = t1_image_stack.template_fit(template_dcm)
         t1_image_stack.generate_time_series(
-            self.TEMPLATE_TEST_COORDS_ROW_COL, fit_coords=True)
+            self.TEMPLATE_TEST_COORDS_ROW_COL,
+            warp_matrix=warp_matrix)
         t1_image_stack.generate_fit_function()
-        t1_published = \
-            hazen_relaxometry.TEMPLATE_VALUES['plate5']['t1']['relax_times']['1.5T']
-        t1_image_stack.initialise_fit_parameters(t1_estimates=t1_published)
+        t1_published = TEMPLATE_VALUES['plate5']['t1']['relax_times']['1.5T']
+        s0_est = t1_image_stack.initialise_fit_parameters(t1_estimates=t1_published)
 
-        t1_image_stack.find_relax_times()
+        t1_image_stack.find_relax_times(
+            t1_estimates=t1_published, s0_est=s0_est)
 
-        np.testing.assert_allclose(t1_image_stack.t1s, self.PLATE5_T1,
+        np.testing.assert_allclose(t1_image_stack.relax_times, self.PLATE5_T1,
                                    rtol=0.02, atol=1)
 
     def test_t2_calc_magnitude_image(self):
         """Test T2 value for plate 4 spheres."""
         template_dcm = pydicom.read_file(self.TEMPLATE_PATH_T2)
         t2_dcms = [pydicom.dcmread(os.path.join(self.T2_DIR, fname))
                    for fname in self.T2_FILES]
-        t2_image_stack = hazen_relaxometry.T2ImageStack(t2_dcms, template_dcm)
-        t2_image_stack.template_fit()
+        t2_image_stack = T2ImageStack(t2_dcms)
+        warp_matrix = t2_image_stack.template_fit(template_dcm)
         t2_image_stack.generate_time_series(
-            self.TEMPLATE_P4_TEST_COORDS_ROW_COL, fit_coords=True)
-        t2_published = \
-            hazen_relaxometry.TEMPLATE_VALUES['plate4']['t2']['relax_times']['1.5T']
-        t2_image_stack.initialise_fit_parameters(t2_estimates=t2_published)
-        t2_image_stack.initialise_fit_parameters(t2_published)
-        t2_image_stack.find_relax_times()
+            self.TEMPLATE_P4_TEST_COORDS_ROW_COL,
+            warp_matrix=warp_matrix)
+        t2_published = TEMPLATE_VALUES['plate4']['t2']['relax_times']['1.5T']
+        s0_est = t2_image_stack.initialise_fit_parameters(
+            t2_estimates=t2_published)
+        t2_image_stack.find_relax_times(
+            t2_estimates=t2_published, s0_est=s0_est)
 
-        np.testing.assert_allclose(t2_image_stack.t2s, self.PLATE4_T2,
+        np.testing.assert_allclose(t2_image_stack.relax_times, self.PLATE4_T2,
                                    rtol=0.01, atol=1)
 
     def test_t1_calc_signed_image(self):
         """Test T1 value for signed plate 5 spheres (site 2)."""
         template_dcm = pydicom.read_file(self.TEMPLATE_PATH_T1_P5)
         t1_dcms = [pydicom.dcmread(os.path.join(self.SITE2_T1_DIR, fname))
                    for fname in self.SITE2_T1_FILES]
-        t1_image_stack = hazen_relaxometry.T1ImageStack(t1_dcms, template_dcm)
-        t1_image_stack.template_fit()
+        t1_image_stack = T1ImageStack(t1_dcms)
+        warp_matrix = t1_image_stack.template_fit(template_dcm)
         t1_image_stack.generate_time_series(
-            self.TEMPLATE_TEST_COORDS_ROW_COL, fit_coords=True)
+            self.TEMPLATE_TEST_COORDS_ROW_COL,
+            warp_matrix=warp_matrix)
         t1_image_stack.generate_fit_function()
-        t1_published = \
-            hazen_relaxometry.TEMPLATE_VALUES['plate5']['t1']['relax_times']['1.5T']
-        t1_image_stack.initialise_fit_parameters(t1_estimates=t1_published)
-        t1_image_stack.find_relax_times()
-
-        np.testing.assert_allclose(t1_image_stack.t1s, self.SITE2_PLATE5_T1,
-                                   rtol=0.02, atol=1)
-
-    def test_neither_t1_or_t2(self):
-        """Test exception raised if neither T1 nor T2 to be calculated."""
-        self.assertRaises(ArgumentCombinationError,
-                          hazen_relaxometry.main, [], calc_t1=False,
-                          calc_t2=False, plate_number=5)
-
-    def test_both_t1_or_t2(self):
-        """Test exception raised if neither T1 nor T2 to be calculated."""
-        self.assertRaises(ArgumentCombinationError,
-                          hazen_relaxometry.main, [], calc_t1=True,
-                          calc_t2=True, plate_number=5)
+        t1_published = TEMPLATE_VALUES['plate5']['t1']['relax_times']['1.5T']
+        s0_est = t1_image_stack.initialise_fit_parameters(
+            t1_estimates=t1_published)
+        t1_image_stack.find_relax_times(
+            t1_estimates=t1_published, s0_est=s0_est)
+
+        np.testing.assert_allclose(t1_image_stack.relax_times, self.SITE2_PLATE5_T1,
+                                   rtol=0.02, atol=1)
 
     def test_t1_siemens(self):
         """Test T1 values on Siemens images."""
-        dcms = [pydicom.dcmread(os.path.join(self.T1_DIR, fname)) for fname in
-                self.T1_FILES]
-        t1_results = hazen_relaxometry.main(dcms, plate_number=5,
-                                            calc_t1=True, verbose=True)
+        dcms = get_dicom_files(self.T1_DIR)
+        # dcms = [pydicom.dcmread(os.path.join(self.T1_DIR, fname)) for fname in
+        #         self.T1_FILES]
+        task = Relaxometry(data_paths=dcms)
+        t1_results = task.run(plate_number=5, calc="T1", verbose=True)
         # `t1_results` is a dict with one item where we don't know the key.
         # Need to extract via unpacking
         results, = t1_results.values()
         np.testing.assert_allclose(results['calc_times'], self.PLATE5_T1,
                                    rtol=0.02, atol=1)
 
     def test_t1_p4_philips(self):
         """Test T1 values on plate 4 on Philips."""
-        dcms = [pydicom.dcmread(os.path.join(self.SITE4_T1_P4_DIR, fname))
-                for fname in self.SITE4_T1_P4_FILES]
-        t1_results = hazen_relaxometry.main(dcms, plate_number=4,
-                                            calc_t1=True, verbose=True)
+        dcms = get_dicom_files(self.SITE4_T1_P4_DIR)
+        # dcms = [pydicom.dcmread(os.path.join(self.SITE4_T1_P4_DIR, fname))
+        #         for fname in self.SITE4_T1_P4_FILES]
+        task = Relaxometry(data_paths=dcms)
+        t1_results = task.run(plate_number=4, calc="T1", verbose=True)
         # `t1_results` is a dict with one item where we don't know the key.
         # Need to extract via unpacking
         results, = t1_results.values()
         np.testing.assert_allclose(results['calc_times'],
                                    self.SITE4_T1_P4,
                                    rtol=0.02, atol=1)
 
     def test_t1_p5_philips(self):
         """Test T1 values on plate 5 on Philips."""
-        dcms = [pydicom.dcmread(os.path.join(self.SITE4_T1_P5_DIR, fname))
-                for fname in self.SITE4_T1_P5_FILES]
-        t1_results = hazen_relaxometry.main(dcms, plate_number=5,
-                                            calc_t1=True, verbose=True)
+        dcms = get_dicom_files(self.SITE4_T1_P5_DIR)
+        # dcms = [pydicom.dcmread(os.path.join(self.SITE4_T1_P5_DIR, fname))
+        #         for fname in self.SITE4_T1_P5_FILES]
+        task = Relaxometry(data_paths=dcms)
+        t1_results = task.run(plate_number=5, calc="T1", verbose=True)
         results, = t1_results.values()
         np.testing.assert_allclose(results['calc_times'],
                                    self.SITE4_T1_P5,
                                    rtol=0.02, atol=1)
 
     def test_t2_p4_philips(self):
         """Test T2 values on plate 4 on Philips."""
-        dcms = [pydicom.dcmread(os.path.join(self.SITE4_T2_P4_DIR, fname))
-                for fname in self.SITE4_T2_P4_FILES]
-        t2_results = hazen_relaxometry.main(dcms, plate_number=4,
-                                            calc_t2=True, verbose=True)
+        dcms = get_dicom_files(self.SITE4_T2_P4_DIR)
+        # dcms = [pydicom.dcmread(os.path.join(self.SITE4_T2_P4_DIR, fname))
+        #         for fname in self.SITE4_T2_P4_FILES]
+        task = Relaxometry(data_paths=dcms)
+        t2_results = task.run(plate_number=4, calc="T2", verbose=True)
         results, = t2_results.values()
         np.testing.assert_allclose(results['calc_times'],
                                    self.SITE4_T2_P4,
                                    rtol=0.02, atol=1)
 
     def test_t2_p5_philips(self):
         """Test T2 values on plate 4 on Philips."""
-        dcms = [pydicom.dcmread(os.path.join(self.SITE4_T2_P5_DIR, fname))
-                for fname in self.SITE4_T2_P5_FILES]
-        t2_results = hazen_relaxometry.main(dcms, plate_number=5,
-                                            calc_t2=True, verbose=True)
+        dcms = get_dicom_files(self.SITE4_T2_P5_DIR)
+        # dcms = [pydicom.dcmread(os.path.join(self.SITE4_T2_P5_DIR, fname))
+        #         for fname in self.SITE4_T2_P5_FILES]
+        task = Relaxometry(data_paths=dcms)
+        t2_results = task.run(plate_number=5, calc="T2", verbose=True)
         results, = t2_results.values()
         np.testing.assert_allclose(results['calc_times'],
                                    self.SITE4_T2_P5,
                                    rtol=0.02, atol=1)
 
     def test_scale_up_template(self):
         """Test fit for 256x256 GE image with 192x192 template"""
         template_dcm = pydicom.read_file(
-            hazen_relaxometry.TEMPLATE_VALUES['plate4']['t1']['filename'])
+                            TEMPLATE_VALUES['plate4']['t1']['filename'])
 
         target_dcm = pydicom.dcmread(self.PATH_256_MATRIX)
-        t1_image_stack = hazen_relaxometry.T1ImageStack([target_dcm],
-                                                        template_dcm,
-                                                        plate_number=4)
-        t1_image_stack.template_fit()
-
-        transformed_coordinates_xy = hazen_relaxometry.transform_coords(
-            hazen_relaxometry.TEMPLATE_VALUES['plate4']['sphere_centres_row_col'],
-            t1_image_stack.warp_matrix,
-            input_row_col=True, output_row_col=True)
+        t1_image_stack = T1ImageStack([target_dcm])
+        warp_matrix = t1_image_stack.template_fit(template_dcm)
+
+        transformed_coordinates_xy = transform_coords(
+            TEMPLATE_VALUES['plate4']['sphere_centres_row_col'],
+            warp_matrix, input_row_col=True, output_row_col=True)
 
         # test to within +/- 1 pixel (also checks YX-XY change)
         np.testing.assert_allclose(
             transformed_coordinates_xy, self.TARGET_COORDS_256,
             atol=1)
 
     def test_ge(self):
         """Test relaxometry.py values on GE."""
         for plate in (4, 5):
-            for tparam in ('T1', 'T2'):
-                calc_t1 = tparam == 'T1'
-                calc_t2 = tparam == 'T2'
-                dcms = [pydicom.dcmread(os.path.join(
-                    getattr(self, f'SITE3_{tparam}_P{plate}_DIR'), fname))
-                    for fname in getattr(self, f'SITE3_{tparam}_P{plate}_FILES')]
-
-                t_results = hazen_relaxometry.main(dcms, plate_number=plate,
-                                                   calc_t2=calc_t2,
-                                                   calc_t1=calc_t1,
-                                                   verbose=True)
+            for tparam in ['T1', 'T2']:
+                dcms = get_dicom_files(
+                    getattr(self, f'SITE3_{tparam}_P{plate}_DIR'))
+                # dcms = [pydicom.dcmread(os.path.join(
+                #     getattr(self, f'SITE3_{tparam}_P{plate}_DIR'), fname))
+                #     for fname in getattr(self, f'SITE3_{tparam}_P{plate}_FILES')]
+                task = Relaxometry(data_paths=dcms)
+                t_results = task.run(plate_number=plate,
+                                calc = tparam, verbose=True)
                 results, = t_results.values()
                 np.testing.assert_allclose(
                     results['calc_times'],
                     getattr(self, f'SITE3_{tparam}_P{plate}_VALS'),
                     rtol=0.02, atol=1)
 
-    def test_plate_number_not_specified(self):
-        """Test exception raised if plate_number not specified."""
-        self.assertRaises(ArgumentCombinationError,
-                          hazen_relaxometry.main, [], calc_t1=True)
-
-    def test_rms(self):
-        """Test rms calculated correctly."""
-        self.assertAlmostEqual(hazen_relaxometry.rms([i for i in range(10)]),
-                               5.338539126015656)
+    # # This type of expection is raised automatically at the arg parse level
+    # def test_plate_number_not_specified(self):
+    #     """Test exception raised if plate_number not specified."""
+    #     self.assertRaises(ArgumentCombinationError,
+    #                       Relaxometry.run, [], calc="T1")
 
     def test_philips_3T(self):
         """Test calculation on 3T dataset."""
 
         # T1 plate 4
-        dcms = [pydicom.dcmread(os.path.join(self.SITE5_T1_P4_DIR, fname))
-                for fname in self.SITE5_T1_P4_FILES]
-        t1_results = hazen_relaxometry.main(dcms, plate_number=4,
-                                            calc_t1=True, verbose=True)
+        dcms = get_dicom_files(self.SITE5_T1_P4_DIR)
+        # dcms = [pydicom.dcmread(os.path.join(self.SITE5_T1_P4_DIR, fname))
+        #         for fname in self.SITE5_T1_P4_FILES]
+        task = Relaxometry(data_paths=dcms)
+        t1_results = task.run(plate_number=4, calc="T1", verbose=True)
         results, = t1_results.values()
         np.testing.assert_allclose(results['calc_times'],
                                    self.SITE5_T1_P4,
                                    rtol=0.02, atol=1)
 
         # T1 plate 5
-        dcms = [pydicom.dcmread(os.path.join(self.SITE5_T1_P5_DIR, fname))
-                for fname in self.SITE5_T1_P5_FILES]
-        t1_results = hazen_relaxometry.main(dcms, plate_number=5,
-                                            calc_t1=True, verbose=True)
+        dcms = get_dicom_files(self.SITE5_T1_P5_DIR)
+        # dcms = [pydicom.dcmread(os.path.join(self.SITE5_T1_P5_DIR, fname))
+        #         for fname in self.SITE5_T1_P5_FILES]
+        task = Relaxometry(data_paths=dcms)
+        t1_results = task.run(plate_number=5, calc="T1", verbose=True)
         results, = t1_results.values()
         np.testing.assert_allclose(results['calc_times'],
                                    self.SITE5_T1_P5,
                                    rtol=0.02, atol=1)
 
         # T2 plate 4
-        dcms = [pydicom.dcmread(os.path.join(self.SITE5_T2_P4_DIR, fname))
-                for fname in self.SITE5_T2_P4_FILES]
-        t2_results = hazen_relaxometry.main(dcms, plate_number=4,
-                                            calc_t2=True, verbose=True)
+        dcms = get_dicom_files(self.SITE5_T2_P4_DIR)
+        # dcms = [pydicom.dcmread(os.path.join(self.SITE5_T2_P4_DIR, fname))
+        #         for fname in self.SITE5_T2_P4_FILES]
+        task = Relaxometry(data_paths=dcms)
+        t2_results = task.run(plate_number=4, calc="T2", verbose=True)
         results, = t2_results.values()
         np.testing.assert_allclose(results['calc_times'],
                                    self.SITE5_T2_P4,
                                    rtol=0.02, atol=1)
 
         # T2 plate 5
-        dcms = [pydicom.dcmread(os.path.join(self.SITE5_T2_P5_DIR, fname))
-                for fname in self.SITE5_T2_P5_FILES]
-        t2_results = hazen_relaxometry.main(dcms, plate_number=5,
-                                            calc_t2=True, verbose=True)
+        dcms = get_dicom_files(self.SITE5_T2_P5_DIR)
+        # dcms = [pydicom.dcmread(os.path.join(self.SITE5_T2_P5_DIR, fname))
+        #         for fname in self.SITE5_T2_P5_FILES]
+        task = Relaxometry(data_paths=dcms)
+        t2_results = task.run(plate_number=5, calc="T2", verbose=True)
         results, = t2_results.values()
         np.testing.assert_allclose(results['calc_times'],
                                    self.SITE5_T2_P5,
                                    rtol=0.02, atol=1)
 
 
 if __name__ == '__main__':
```

### Comparing `hazen-1.2.0/tests/test_slice_position.py` & `hazen-1.3.0/tests/test_slice_position.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 import pathlib
 import os
 import pydicom
 
 from tests import TEST_DATA_DIR, TEST_REPORT_DIR
 from hazenlib.tasks.slice_position import SlicePosition
-from hazenlib.tools import get_dicom_files
+from hazenlib.utils import get_dicom_files
 import copy
 
 
 class TestSlicePosition(unittest.TestCase):
     SLICE_POS = pathlib.Path(TEST_DATA_DIR / 'slicepos')
     ROD_COORDS = (122.22222222222223, 83.0, 132.88888888888889, 180.33333333333334)
     # SLICE_POSITION_OUTPUT = ['0.151', '0.0964', '0.237', '0.101', '0.224', '0.103', '0.0873', '0.0386', '0.0458',
```

### Comparing `hazen-1.2.0/tests/test_slice_width.py` & `hazen-1.3.0/tests/test_slice_width.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 import numpy as np
 import pydicom
 
 # import hazenlib.slice_width as hazen_slice_width
 from tests import TEST_DATA_DIR, TEST_REPORT_DIR
 from hazenlib.tasks.slice_width import SliceWidth
-from hazenlib.shapes import Rod
-from hazenlib.tools import get_dicom_files
+from hazenlib.utils import get_dicom_files, Rod
 import os
 
 
 class TestSliceWidth(unittest.TestCase):
     SLICE_WIDTH_DATA = pathlib.Path(TEST_DATA_DIR / 'slicewidth')
 
     """
```

### Comparing `hazen-1.2.0/tests/test_snr.py` & `hazen-1.3.0/tests/test_snr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 import pathlib
 
 import pydicom
 import os
 from tests import TEST_DATA_DIR, TEST_REPORT_DIR
-from hazenlib.tools import get_dicom_files
+from hazenlib.utils import get_dicom_files
 from hazenlib.tasks.snr import SNR
 
 
 
 # Note all SNR tests assume 5mm slice thickness
 class TestSnr(unittest.TestCase):
```

### Comparing `hazen-1.2.0/tests/test_snr_map.py` & `hazen-1.3.0/tests/test_snr_map.py`

 * *Files identical despite different names*

### Comparing `hazen-1.2.0/tests/test_spatial_resolution.py` & `hazen-1.3.0/tests/test_spatial_resolution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import unittest
 import pathlib
 import pytest
 
 import numpy as np
-import pydicom
 import os
 
-import hazenlib
-from hazenlib.tasks.spatial_resolution import SpatialResolution
 from tests import TEST_DATA_DIR, TEST_REPORT_DIR
-from hazenlib.tools import get_dicom_files
+from hazenlib.tasks.spatial_resolution import SpatialResolution
+from hazenlib.utils import get_dicom_files, rescale_to_byte
 
 
 class TestSpatialResolution(unittest.TestCase):
     files = get_dicom_files(os.path.join(TEST_DATA_DIR, 'resolution', 'RESOLUTION'))
     TEST_SQUARE = [[300, 220], [219, 206], [205, 287], [286, 301]]
     CIRCLE = [[[254, 256, 197]]]
     CENTRE = {'x': 293, 'y': 260}  # of right edge
@@ -326,32 +324,32 @@
         pixels = np.ones((256, 256))
         roi = self.hazen_spatial_resolution.get_roi(pixels, centre, size)
         assert roi.shape == (20, 20)
         assert roi.mean() == 1.0
         assert roi.max() == 1.0
 
     def test_get_circles(self):
-        img = hazenlib.rescale_to_byte(self.hazen_spatial_resolution.data[0].pixel_array)
+        img = rescale_to_byte(self.hazen_spatial_resolution.data[0].pixel_array)
         circles = self.hazen_spatial_resolution.get_circles(img)
         assert np.testing.assert_allclose(circles[0][0][:], self.CIRCLE[0][0][:]) is None
 
     def test_thresh_image(self):
-        img = hazenlib.rescale_to_byte(self.hazen_spatial_resolution.data[0].pixel_array)
+        img = rescale_to_byte(self.hazen_spatial_resolution.data[0].pixel_array)
         thresh = self.hazen_spatial_resolution.thresh_image(img)
         assert np.count_nonzero(thresh) < np.count_nonzero(img)
 
     def test_find_square(self):
-        img = hazenlib.rescale_to_byte(self.hazen_spatial_resolution.data[0].pixel_array)
+        img = rescale_to_byte(self.hazen_spatial_resolution.data[0].pixel_array)
         thresh = self.hazen_spatial_resolution.thresh_image(img)
         square, _ = self.hazen_spatial_resolution.find_square(thresh)
 
         assert np.testing.assert_allclose(square, self.TEST_SQUARE) is None
 
     def test_get_bisecting_normals(self):
-        img = hazenlib.rescale_to_byte(self.hazen_spatial_resolution.data[0].pixel_array)
+        img = rescale_to_byte(self.hazen_spatial_resolution.data[0].pixel_array)
         thresh = self.hazen_spatial_resolution.thresh_image(img)
         square, _ = self.hazen_spatial_resolution.find_square(thresh)
         vector = {"x": square[3][0] - square[0][0], "y": square[3][1] - square[0][1]}
         centre = {"x": square[0][0] + int(vector["x"] / 2), "y": square[0][1] + int(vector["y"] / 2)}
         n1x, n1y, n2x, n2y = self.hazen_spatial_resolution.get_bisecting_normal(vector, centre)
         assert (n1x, n1y, n2x, n2y) == self.bisecting_normal
 
@@ -439,18 +437,18 @@
     TOP_EDGE_MEAN = 205.28
     SIGNAL_MEAN = 348.5525
     MTF_FE = 0.6017507296855603
     MTF_PE = 0.4923415061063675
     bisecting_normal = (281, 245, 319, 239)
 
 
-class TestEastKentResolution(TestSpatialResolution):
-    # RESOLUTION_DATA = pathlib.Path(TEST_DATA_DIR / 'resolution')
-    # dicom = pydicom.read_file(str(RESOLUTION_DATA / 'eastkent' / "256_sag.IMA"))
-    files = get_dicom_files(os.path.join(TEST_DATA_DIR, 'resolution', 'eastkent'))
+class TestSite01Resolution(TestSpatialResolution):
+
+    files = get_dicom_files(os.path.join(TEST_DATA_DIR, 'resolution', 'resolution_site01'))
+
     TEST_SQUARE = [[142, 105], [104, 113], [112, 152], [150, 144]]
     CIRCLE = [[[127, 128, 96]]]
     TOP_CENTRE = {'x': 123, 'y': 109}
     CENTRE = {'x': 146, 'y': 124}
     VOID_MEAN = 10.6375
     EDGE_MEAN = 530.86
     TOP_EDGE_MEAN = 648.46
```

### Comparing `hazen-1.2.0/tests/test_uniformity.py` & `hazen-1.3.0/tests/test_uniformity.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     def setUp(self):
         self.uniformity_task = Uniformity(data_paths=[os.path.join(self.UNIFORMITY_DATA, 'axial_oil.IMA')],
                                           report_dir=pathlib.PurePath.joinpath(TEST_REPORT_DIR))
 
     def test_uniformity(self):
         results = self.uniformity_task.run()
         key = self.uniformity_task.key(self.uniformity_task.data[0])
-        horizontal_ipem = results[key]['horizontal']['IPEM']
-        vertical_ipem = results[key]['vertical']['IPEM']
+        horizontal_ipem = results[key]['horizontal']
+        vertical_ipem = results[key]['vertical']
 
         print("\ntest_uniformity.py::TestUniformity::test_uniformity")
 
         print("new_release_value:", vertical_ipem)
 
         print("fixed_value:", self.IPEM_VERTICAL)
```

